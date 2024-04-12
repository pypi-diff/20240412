# Comparing `tmp/flask_rpc-0.1.3.tar.gz` & `tmp/flask_rpc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.1.3.tar` & `flask_rpc-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3200 2024-04-10 12:50:11.305808 flask_rpc-0.1.3/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.3/LICENSE
--rw-r--r--   0        0        0      737 2024-04-12 11:19:22.327411 flask_rpc-0.1.3/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.3/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.3/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.3/app/models/__init__.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967937 flask_rpc-0.1.3/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.3/app/models/users.py
--rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.3/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.3/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.3/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      217 2024-04-12 11:03:24.917423 flask_rpc-0.1.3/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      164 2024-04-12 11:03:56.126349 flask_rpc-0.1.3/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      156 2024-04-12 11:03:56.122181 flask_rpc-0.1.3/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.3/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     2074 2024-04-12 11:04:28.754607 flask_rpc-0.1.3/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0     1207 2024-04-12 15:03:23.917921 flask_rpc-0.1.3/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-12 16:27:21.107450 flask_rpc-0.1.3/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.3/flask_rpc/latest.py
--rw-r--r--   0        0        0     2843 2024-04-12 16:27:03.486282 flask_rpc-0.1.3/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.3/requirements.txt
--rw-r--r--   0        0        0        9 2024-04-12 10:27:38.122766 flask_rpc-0.1.3/requirements_dev.txt
--rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.3/test.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 flask_rpc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3200 2024-04-10 12:50:11.305808 flask_rpc-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.4/LICENSE
+-rw-r--r--   0        0        0      737 2024-04-12 11:19:22.327411 flask_rpc-0.1.4/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.4/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.4/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.4/app/models/__init__.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967937 flask_rpc-0.1.4/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.4/app/models/users.py
+-rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.4/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.4/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.4/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-12 11:03:24.917423 flask_rpc-0.1.4/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      164 2024-04-12 11:03:56.126349 flask_rpc-0.1.4/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      156 2024-04-12 11:03:56.122181 flask_rpc-0.1.4/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.4/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     2074 2024-04-12 11:04:28.754607 flask_rpc-0.1.4/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0     1207 2024-04-12 15:03:23.917921 flask_rpc-0.1.4/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-12 16:30:25.595445 flask_rpc-0.1.4/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.4/flask_rpc/latest.py
+-rw-r--r--   0        0        0     2839 2024-04-12 16:29:53.380243 flask_rpc-0.1.4/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.4/requirements.txt
+-rw-r--r--   0        0        0        9 2024-04-12 10:27:38.122766 flask_rpc-0.1.4/requirements_dev.txt
+-rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.4/test.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 flask_rpc-0.1.4/PKG-INFO
```

### Comparing `flask_rpc-0.1.3/.gitignore` & `flask_rpc-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/LICENSE` & `flask_rpc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/README.md` & `flask_rpc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/app/__init__.py` & `flask_rpc-0.1.4/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/app/models/clients.py` & `flask_rpc-0.1.4/app/models/clients.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/app/models/users.py` & `flask_rpc-0.1.4/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.1.4/app/rpc/clients/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/app/templates/index.html` & `flask_rpc-0.1.4/app/templates/index.html`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/flask_rpc/version_1_0.py` & `flask_rpc-0.1.4/flask_rpc/version_1_0.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,18 @@
     frpc: float
     function: str
     data: t.Any
 
 
 class RPCRequest:
     @classmethod
-    def build(cls, function: str, data: t.Optional[dict[str, t.Any]] = None) -> dict[str, t.Any]:
-        return {
-            "frpc": 1.0,
-            "function": function,
-            "data": data
-        }
+    def build(
+        cls, function: str, data: t.Optional[dict[str, t.Any]] = None
+    ) -> dict[str, t.Any]:
+        return {"frpc": 1.0, "function": function, "data": data}
 
 
 class RPCResponse:
     @classmethod
     def failed_response(cls, message: str = None, data: dict[str, t.Any] = None):
         r = {"frpc": 1.0, "ok": False}
 
@@ -43,15 +41,17 @@
 
         return r
 
 
 class RPC:
     LOOKUP: dict[str, t.Callable]
 
-    def __init__(self, app_or_blueprint: t.Union[Flask, Blueprint], url_prefix: str = "/"):
+    def __init__(
+        self, app_or_blueprint: t.Union[Flask, Blueprint], url_prefix: str = "/"
+    ):
         self.LOOKUP = {}
 
         if not hasattr(app_or_blueprint, "add_url_rule"):
             raise TypeError(
                 f"Looks like {app_or_blueprint}, type({type(app_or_blueprint)}) might "
                 f"not be an instance of Flask, Flask Blueprint or be compatible with "
                 "setting Flask routes."
@@ -59,15 +59,17 @@
 
         self._register_route(app_or_blueprint, url_prefix)
 
     def functions(self, **kwargs: t.Callable):
         for k, v in kwargs.items():
             self.LOOKUP[k] = v
 
-    def _register_route(self, route_compatible: t.Union[Flask, Blueprint], url_prefix: str):
+    def _register_route(
+        self, route_compatible: t.Union[Flask, Blueprint], url_prefix: str
+    ):
         route_compatible.add_url_rule(
             url_prefix,
             view_func=self._rpc_route,
             provide_automatic_options=True,
             methods=["POST"],
         )
```

### Comparing `flask_rpc-0.1.3/test.py` & `flask_rpc-0.1.4/test.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.3/PKG-INFO` & `flask_rpc-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-rpc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Turn Flask into a simple RPC server
 Author-email: David Carmichael <david@uilix.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Flask
 Requires-Dist: pydantic
```

