# Comparing `tmp/acrclient-0.4.4.tar.gz` & `tmp/acrclient-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrclient-0.4.4.tar", max compression
+gzip compressed data, was "acrclient-0.4.5.tar", max compression
```

## Comparing `acrclient-0.4.4.tar` & `acrclient-0.4.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2287 2024-03-25 20:15:31.538626 acrclient-0.4.4/README.md
--rw-r--r--   0        0        0      322 2024-03-25 20:15:31.538626 acrclient-0.4.4/acrclient/__init__.py
--rw-r--r--   0        0        0     5367 2024-03-25 20:15:31.538626 acrclient-0.4.4/acrclient/client.py
--rw-r--r--   0        0        0      819 2024-03-25 20:15:31.538626 acrclient-0.4.4/acrclient/models.py
--rw-r--r--   0        0        0        0 2024-03-25 20:15:31.538626 acrclient-0.4.4/acrclient/py.typed
--rw-r--r--   0        0        0     1284 2024-03-25 20:15:46.418621 acrclient-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 acrclient-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     2287 2024-04-12 09:06:39.845582 acrclient-0.4.5/README.md
+-rw-r--r--   0        0        0      322 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/__init__.py
+-rw-r--r--   0        0        0     5367 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/client.py
+-rw-r--r--   0        0        0      819 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/models.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:06:39.845582 acrclient-0.4.5/acrclient/py.typed
+-rw-r--r--   0        0        0     1284 2024-04-12 09:06:54.197681 acrclient-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 acrclient-0.4.5/PKG-INFO
```

### Comparing `acrclient-0.4.4/README.md` & `acrclient-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.4/acrclient/client.py` & `acrclient-0.4.5/acrclient/client.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.4/acrclient/models.py` & `acrclient-0.4.5/acrclient/models.py`

 * *Files identical despite different names*

### Comparing `acrclient-0.4.4/pyproject.toml` & `acrclient-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrclient"
-version = "v0.4.4"
+version = "v0.4.5"
 description = "API wrapper for the v2 ACRCloud API"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-v3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `acrclient-0.4.4/PKG-INFO` & `acrclient-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrclient
-Version: 0.4.4
+Version: 0.4.5
 Summary: API wrapper for the v2 ACRCloud API
 License: AGPL-v3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

