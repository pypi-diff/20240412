# Comparing `tmp/flask_rpc-0.1.5.tar.gz` & `tmp/flask_rpc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.1.5.tar` & `flask_rpc-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.1.5/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.5/LICENSE
--rw-r--r--   0        0        0     2522 2024-04-12 19:41:44.625491 flask_rpc-0.1.5/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.5/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.5/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.5/app/models/__init__.py
--rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.1.5/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.5/app/models/users.py
--rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.5/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.5/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.5/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      286 2024-04-12 19:45:53.495758 flask_rpc-0.1.5/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      229 2024-04-12 19:46:23.649313 flask_rpc-0.1.5/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      221 2024-04-12 19:46:13.766886 flask_rpc-0.1.5/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.5/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     1546 2024-04-12 19:46:38.040859 flask_rpc-0.1.5/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.1.5/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-12 20:06:47.742786 flask_rpc-0.1.5/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.5/flask_rpc/latest.py
--rw-r--r--   0        0        0     2911 2024-04-12 20:04:57.691367 flask_rpc-0.1.5/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.5/requirements.txt
--rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.1.5/requirements_dev.txt
--rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.5/test.py
--rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 flask_rpc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2523 2024-04-12 20:16:40.012404 flask_rpc-0.1.6/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.6/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.6/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.6/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.1.6/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.6/app/models/users.py
+-rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.6/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.6/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.6/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-12 19:45:53.495758 flask_rpc-0.1.6/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      229 2024-04-12 19:46:23.649313 flask_rpc-0.1.6/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      221 2024-04-12 19:46:13.766886 flask_rpc-0.1.6/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.6/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1546 2024-04-12 19:46:38.040859 flask_rpc-0.1.6/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.1.6/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-12 20:17:44.668059 flask_rpc-0.1.6/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.6/flask_rpc/latest.py
+-rw-r--r--   0        0        0     2911 2024-04-12 20:04:57.691367 flask_rpc-0.1.6/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.6/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.1.6/requirements_dev.txt
+-rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.6/test.py
+-rw-r--r--   0        0        0     2808 1970-01-01 00:00:00.000000 flask_rpc-0.1.6/PKG-INFO
```

### Comparing `flask_rpc-0.1.5/.gitignore` & `flask_rpc-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/LICENSE` & `flask_rpc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/README.md` & `flask_rpc-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 ```js
 fetch("/rpc", {
   method: "POST",
   headers: {
     "Content-Type": "application/json"
   },
   body: frpc(
-    function="add_numbers",
+    function_="add_numbers",
     data=[1, 2, 3]
   )
 })
 ```
 
 Will return:
```

### Comparing `flask_rpc-0.1.5/app/__init__.py` & `flask_rpc-0.1.6/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/app/models/clients.py` & `flask_rpc-0.1.6/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/app/models/users.py` & `flask_rpc-0.1.6/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.1.6/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/app/templates/index.html` & `flask_rpc-0.1.6/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/flask_rpc/version_1_0.py` & `flask_rpc-0.1.6/flask_rpc/version_1_0.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/test.py` & `flask_rpc-0.1.6/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.5/PKG-INFO` & `flask_rpc-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Flask
 Requires-Dist: pydantic
 
@@ -123,15 +123,15 @@
 ```js
 fetch("/rpc", {
   method: "POST",
   headers: {
     "Content-Type": "application/json"
   },
   body: frpc(
-    function="add_numbers",
+    function_="add_numbers",
     data=[1, 2, 3]
   )
 })
 ```
 
 Will return:
```

