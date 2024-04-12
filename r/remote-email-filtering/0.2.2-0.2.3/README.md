# Comparing `tmp/remote_email_filtering-0.2.2.tar.gz` & `tmp/remote_email_filtering-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote_email_filtering-0.2.2.tar", max compression
+gzip compressed data, was "remote_email_filtering-0.2.3.tar", max compression
```

## Comparing `remote_email_filtering-0.2.2.tar` & `remote_email_filtering-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      124 2022-08-08 08:09:18.667224 remote_email_filtering-0.2.2/README.rst
--rw-r--r--   0        0        0     1213 2023-12-07 18:12:37.819516 remote_email_filtering-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      132 2023-12-07 18:12:41.059551 remote_email_filtering-0.2.2/src/remote_email_filtering/__init__.py
--rw-r--r--   0        0        0     2470 2022-09-06 23:03:47.134890 remote_email_filtering-0.2.2/src/remote_email_filtering/action.py
--rw-r--r--   0        0        0      295 2022-08-08 08:09:18.667224 remote_email_filtering-0.2.2/src/remote_email_filtering/auth.py
--rw-r--r--   0        0        0     2235 2022-09-15 09:30:51.858153 remote_email_filtering-0.2.2/src/remote_email_filtering/main.py
--rw-r--r--   0        0        0     3027 2022-10-28 03:25:53.352950 remote_email_filtering-0.2.2/src/remote_email_filtering/message.py
--rw-r--r--   0        0        0     9910 2022-09-15 09:30:51.859154 remote_email_filtering-0.2.2/src/remote_email_filtering/remote.py
--rw-r--r--   0        0        0     1305 2023-12-07 18:09:47.639684 remote_email_filtering-0.2.2/src/remote_email_filtering/types.py
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 remote_email_filtering-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.3/COPYING
+-rw-r--r--   0        0        0      124 2024-01-07 09:17:16.134292 remote_email_filtering-0.2.3/README.rst
+-rw-r--r--   0        0        0     1213 2024-04-12 01:06:26.782605 remote_email_filtering-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-04-12 01:06:13.559214 remote_email_filtering-0.2.3/src/remote_email_filtering/__init__.py
+-rw-r--r--   0        0        0     2470 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/action.py
+-rw-r--r--   0        0        0      295 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/auth.py
+-rw-r--r--   0        0        0     2235 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/main.py
+-rw-r--r--   0        0        0     3027 2024-01-07 09:17:16.137292 remote_email_filtering-0.2.3/src/remote_email_filtering/message.py
+-rw-r--r--   0        0        0     9915 2024-04-12 00:50:48.119309 remote_email_filtering-0.2.3/src/remote_email_filtering/remote.py
+-rw-r--r--   0        0        0     1305 2024-01-16 10:29:23.216073 remote_email_filtering-0.2.3/src/remote_email_filtering/types.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 remote_email_filtering-0.2.3/PKG-INFO
```

### Comparing `remote_email_filtering-0.2.2/pyproject.toml` & `remote_email_filtering-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remote-email-filtering"
-version = "0.2.2"
+version = "0.2.3"
 description = "Email client library for automation"
 authors = ["Gaurav Juvekar <gauravjuvekar@gmail.com>"]
 license = "MIT"
 readme = 'README.rst'
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: No Input/Output (Daemon)",
```

### Comparing `remote_email_filtering-0.2.2/src/remote_email_filtering/action.py` & `remote_email_filtering-0.2.3/src/remote_email_filtering/action.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.2/src/remote_email_filtering/main.py` & `remote_email_filtering-0.2.3/src/remote_email_filtering/main.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.2/src/remote_email_filtering/message.py` & `remote_email_filtering-0.2.3/src/remote_email_filtering/message.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.2/src/remote_email_filtering/remote.py` & `remote_email_filtering-0.2.3/src/remote_email_filtering/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,17 +156,17 @@
             local_uids = [uid[1] for uid in uids]
             ret = self.connection.fetch(local_uids, ['UID', 'ENVELOPE'])
             yield from (ret[uid][b'ENVELOPE'] for uid in local_uids)
 
     def fetch_body(self, msg_id):
         dir_, uid = msg_id
         self.connection.select_folder('/'.join(dir_))
-        ret = self.connection.fetch(uid, ['UID', 'RFC822'])
+        ret = self.connection.fetch(uid, ['UID', 'BODY.PEEK[]'])
         msg = ret[uid]
-        return msg[b'RFC822']
+        return msg[b'BODY[]']
 
     def move_message_id(self, msg_id, target_dir):
         dir_, uid = msg_id
         self.connection.select_folder('/'.join(dir_))
         self.connection.move([uid], '/'.join(target_dir))
         return (target_dir, uid)
```

### Comparing `remote_email_filtering-0.2.2/src/remote_email_filtering/types.py` & `remote_email_filtering-0.2.3/src/remote_email_filtering/types.py`

 * *Files identical despite different names*

### Comparing `remote_email_filtering-0.2.2/PKG-INFO` & `remote_email_filtering-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: remote-email-filtering
-Version: 0.2.2
+Version: 0.2.3
 Summary: Email client library for automation
 Home-page: https://github.com/gauravjuvekar/remote-email-filtering
 License: MIT
 Author: Gaurav Juvekar
 Author-email: gauravjuvekar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications :: Email :: Email Clients (MUA)
 Classifier: Topic :: Communications :: Email :: Filters
 Requires-Dist: IMAPClient (>=2.3.1,<3.0.0)
 Requires-Dist: exchangelib (>=4.7.6,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/gauravjuvekar/remote-email-filtering/issues
 Project-URL: Repository, https://github.com/gauravjuvekar/remote-email-filtering
 Description-Content-Type: text/x-rst
```

