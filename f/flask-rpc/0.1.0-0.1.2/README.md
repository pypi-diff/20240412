# Comparing `tmp/flask_rpc-0.1.0.tar.gz` & `tmp/flask_rpc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.1.0.tar` & `flask_rpc-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3200 2024-04-10 12:50:11.305808 flask_rpc-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.0/LICENSE
--rw-r--r--   0        0        0      737 2024-04-12 11:19:22.327411 flask_rpc-0.1.0/README.md
--rw-r--r--   0        0        0      727 2024-04-12 10:42:46.785979 flask_rpc-0.1.0/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.0/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.0/app/models/__init__.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967937 flask_rpc-0.1.0/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.0/app/models/users.py
--rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.0/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.0/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.0/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      217 2024-04-12 11:03:24.917423 flask_rpc-0.1.0/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      164 2024-04-12 11:03:56.126349 flask_rpc-0.1.0/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      156 2024-04-12 11:03:56.122181 flask_rpc-0.1.0/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.0/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     2074 2024-04-12 11:04:28.754607 flask_rpc-0.1.0/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0     1515 2024-04-12 13:38:57.054850 flask_rpc-0.1.0/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-12 10:45:09.004528 flask_rpc-0.1.0/flask_rpc/__init__.py
--rw-r--r--   0        0        0       98 2024-04-12 13:16:07.239139 flask_rpc-0.1.0/flask_rpc/latest.py
--rw-r--r--   0        0        0     2356 2024-04-12 13:16:07.242159 flask_rpc-0.1.0/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.0/requirements.txt
--rw-r--r--   0        0        0        9 2024-04-12 10:27:38.122766 flask_rpc-0.1.0/requirements_dev.txt
--rw-r--r--   0        0        0     2313 2024-04-12 13:16:57.768922 flask_rpc-0.1.0/test.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 flask_rpc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3200 2024-04-10 12:50:11.305808 flask_rpc-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.2/LICENSE
+-rw-r--r--   0        0        0      737 2024-04-12 11:19:22.327411 flask_rpc-0.1.2/README.md
+-rw-r--r--   0        0        0      727 2024-04-12 10:42:46.785979 flask_rpc-0.1.2/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.2/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.2/app/models/__init__.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967937 flask_rpc-0.1.2/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.2/app/models/users.py
+-rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.2/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.2/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.2/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-12 11:03:24.917423 flask_rpc-0.1.2/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      164 2024-04-12 11:03:56.126349 flask_rpc-0.1.2/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      156 2024-04-12 11:03:56.122181 flask_rpc-0.1.2/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.2/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     2074 2024-04-12 11:04:28.754607 flask_rpc-0.1.2/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0     1207 2024-04-12 15:03:23.917921 flask_rpc-0.1.2/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-12 16:13:25.827124 flask_rpc-0.1.2/flask_rpc/__init__.py
+-rw-r--r--   0        0        0       98 2024-04-12 13:16:07.239139 flask_rpc-0.1.2/flask_rpc/latest.py
+-rw-r--r--   0        0        0     2364 2024-04-12 15:24:47.873967 flask_rpc-0.1.2/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.2/requirements.txt
+-rw-r--r--   0        0        0        9 2024-04-12 10:27:38.122766 flask_rpc-0.1.2/requirements_dev.txt
+-rw-r--r--   0        0        0     2313 2024-04-12 13:16:57.768922 flask_rpc-0.1.2/test.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 flask_rpc-0.1.2/PKG-INFO
```

### Comparing `flask_rpc-0.1.0/.gitignore` & `flask_rpc-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/LICENSE` & `flask_rpc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/README.md` & `flask_rpc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/app/__init__.py` & `flask_rpc-0.1.2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/app/models/clients.py` & `flask_rpc-0.1.2/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/app/models/users.py` & `flask_rpc-0.1.2/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.1.2/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/app/templates/index.html` & `flask_rpc-0.1.2/app/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 <html lang="gb">
 <head>
     <title>Development</title>
+    <script src="https://unpkg.com/flask-rpc-js@latest/cdn.js"></script>
     <script>
         function set_session() {
             fetch(
                 'http://127.0.0.1:5000/rpc/auth',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
-                    body: JSON.stringify({
-                        frpc: 1.0,
-                        function: 'login',
-                        data: {
-                            username: 'admin',
-                            password: 'admin',
-                        }
-                    }),
+                    body: frpc('session', null),
                 }
             )
                 .then(response => response.json())
                 .then(data => console.log(data));
         }
 
         function do_fetch() {
             fetch(
                 'http://127.0.0.1:5000/rpc/auth',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
-                    body: JSON.stringify({
-                        frpc: 1.0,
-                        function: 'session',
-                        data: null
-                    }),
+                    body: frpc('session', null),
                 }
             )
                 .then(response => response.json())
                 .then(data => console.log(data));
         }
     </script>
 </head>
```

### Comparing `flask_rpc-0.1.0/flask_rpc/version_1_0.py` & `flask_rpc-0.1.2/flask_rpc/version_1_0.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,18 @@
 
         try:
             rpcm = RPCModel(**request.json)
         except ValidationError:
             return RPCResponse.failed_response("Invalid request.")
 
         try:
-            assert rpcm.func in self.LOOKUP
+            assert rpcm.function in self.LOOKUP
         except AssertionError:
             return RPCResponse.failed_response("Invalid function.")
 
-        if successful_response := self.LOOKUP[rpcm.func](params=rpcm.data):
+        if successful_response := self.LOOKUP[rpcm.function](params=rpcm.data):
             return successful_response
 
         return RPCResponse.failed_response("Unsuccessful command execution.")
 
 
 __all__ = ["RPC", "RPCResponse", "RPCModel"]
```

### Comparing `flask_rpc-0.1.0/test.py` & `flask_rpc-0.1.2/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.0/PKG-INFO` & `flask_rpc-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.1.0
+Version: 0.1.2
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Flask
 Requires-Dist: pydantic
```

