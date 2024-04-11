# Comparing `tmp/wasmstore-0.2.0.tar.gz` & `tmp/wasmstore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasmstore-0.2.0.tar", max compression
+gzip compressed data, was "wasmstore-0.3.0.tar", max compression
```

## Comparing `wasmstore-0.2.0.tar` & `wasmstore-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1457 2023-07-28 19:57:30.233640 wasmstore-0.2.0/LICENSE
--rw-r--r--   0        0        0       83 2023-07-28 19:57:15.213364 wasmstore-0.2.0/README.md
--rw-r--r--   0        0        0      433 2023-07-28 19:57:15.213364 wasmstore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-28 19:57:15.213364 wasmstore-0.2.0/wasmstore/__init__.py
--rw-r--r--   0        0        0     3461 2023-07-28 19:57:15.213364 wasmstore-0.2.0/wasmstore/wasmstore.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 wasmstore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1457 2024-04-11 22:55:43.339382 wasmstore-0.3.0/LICENSE
+-rw-r--r--   0        0        0       83 2024-04-11 22:55:35.843181 wasmstore-0.3.0/README.md
+-rw-r--r--   0        0        0      433 2024-04-11 22:55:35.843181 wasmstore-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-11 22:55:35.843181 wasmstore-0.3.0/wasmstore/__init__.py
+-rw-r--r--   0        0        0     3326 2024-04-11 22:55:35.843181 wasmstore-0.3.0/wasmstore/wasmstore.py
+-rw-r--r--   0        0        0      652 1970-01-01 00:00:00.000000 wasmstore-0.3.0/PKG-INFO
```

### Comparing `wasmstore-0.2.0/LICENSE` & `wasmstore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wasmstore-0.2.0/wasmstore/wasmstore.py` & `wasmstore-0.3.0/wasmstore/wasmstore.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,17 @@
         return path.lstrip("/")
     else:
         raise Error("invalid path")
 
 
 class Client:
 
-    def __init__(self,
-                 url="http://127.0.0.1:6384",
-                 version="v1",
-                 auth=None,
-                 branch=None):
+    def __init__(
+        self, url="http://127.0.0.1:6384", version="v1", auth=None, branch=None
+    ):
         self.url = url + "/api/" + version
         self.auth = auth
         self.branch = branch
 
     def request(self, method, route, body=None):
         headers = {}
         if self.auth is not None:
@@ -36,22 +34,19 @@
     def find(self, path):
         res = self.request("GET", "/module/" + normalize_path(path))
         if res.status_code == 404:
             return None
         return res.content
 
     def add(self, path, data):
-        res = self.request("POST",
-                           "/module/" + normalize_path(path),
-                           body=data)
+        res = self.request("POST", "/module/" + normalize_path(path), body=data)
         return res.text
 
     def set(self, path, hash):
-        res = self.request("POST",
-                           "/hash/" + hash + "/" + normalize_pathr(path))
+        res = self.request("POST", "/hash/" + hash + "/" + normalize_pathr(path))
         return res.text
 
     def hash(self, path):
         res = self.request("GET", "/hash/" + normalize_path(path))
         if not res.ok:
             return None
         return res.text
```

### Comparing `wasmstore-0.2.0/PKG-INFO` & `wasmstore-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: wasmstore
-Version: 0.2.0
+Version: 0.3.0
 Summary: Wasmstore client for Python
 License: BSD-3-Clause
 Author: Dylibso
 Author-email: oss@dylib.so
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # wasmstore
 
 A Python client for [wasmstore](https://github.com/dylibso/wasmstore)
```

