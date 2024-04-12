# Comparing `tmp/flask_rpc-0.1.4.tar.gz` & `tmp/flask_rpc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_rpc-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "flask_rpc-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `flask_rpc-0.1.4.tar` & `flask_rpc-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3200 2024-04-10 12:50:11.305808 flask_rpc-0.1.4/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.4/LICENSE
--rw-r--r--   0        0        0      737 2024-04-12 11:19:22.327411 flask_rpc-0.1.4/README.md
--rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.4/app/__init__.py
--rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.4/app/extensions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.4/app/models/__init__.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967937 flask_rpc-0.1.4/app/models/clients.py
--rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.4/app/models/users.py
--rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.4/app/rpc/__init__.py
--rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.4/app/rpc/auth/__init__.py
--rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.4/app/rpc/auth/funcs/__init__.py
--rw-r--r--   0        0        0      217 2024-04-12 11:03:24.917423 flask_rpc-0.1.4/app/rpc/auth/funcs/login.py
--rw-r--r--   0        0        0      164 2024-04-12 11:03:56.126349 flask_rpc-0.1.4/app/rpc/auth/funcs/logout.py
--rw-r--r--   0        0        0      156 2024-04-12 11:03:56.122181 flask_rpc-0.1.4/app/rpc/auth/funcs/session.py
--rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.4/app/rpc/clients/__init__.py
--rw-r--r--   0        0        0     2074 2024-04-12 11:04:28.754607 flask_rpc-0.1.4/app/rpc/clients/funcs/__init__.py
--rw-r--r--   0        0        0     1207 2024-04-12 15:03:23.917921 flask_rpc-0.1.4/app/templates/index.html
--rw-r--r--   0        0        0       22 2024-04-12 16:30:25.595445 flask_rpc-0.1.4/flask_rpc/__init__.py
--rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.4/flask_rpc/latest.py
--rw-r--r--   0        0        0     2839 2024-04-12 16:29:53.380243 flask_rpc-0.1.4/flask_rpc/version_1_0.py
--rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.4/requirements.txt
--rw-r--r--   0        0        0        9 2024-04-12 10:27:38.122766 flask_rpc-0.1.4/requirements_dev.txt
--rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.4/test.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 flask_rpc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3222 2024-04-12 19:58:26.539229 flask_rpc-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-12 10:28:56.406133 flask_rpc-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2522 2024-04-12 19:41:44.625491 flask_rpc-0.1.5/README.md
+-rw-r--r--   0        0        0      763 2024-04-12 16:22:33.729380 flask_rpc-0.1.5/app/__init__.py
+-rw-r--r--   0        0        0       59 2024-04-12 10:26:26.537975 flask_rpc-0.1.5/app/extensions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 20:04:31.966024 flask_rpc-0.1.5/app/models/__init__.py
+-rw-r--r--   0        0        0     1637 2024-04-12 20:03:10.485400 flask_rpc-0.1.5/app/models/clients.py
+-rw-r--r--   0        0        0     1707 2024-04-12 07:34:15.967950 flask_rpc-0.1.5/app/models/users.py
+-rw-r--r--   0        0        0      273 2024-04-12 07:31:36.707974 flask_rpc-0.1.5/app/rpc/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-12 11:18:08.444428 flask_rpc-0.1.5/app/rpc/auth/__init__.py
+-rw-r--r--   0        0        0        1 2024-04-11 20:44:17.134954 flask_rpc-0.1.5/app/rpc/auth/funcs/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-12 19:45:53.495758 flask_rpc-0.1.5/app/rpc/auth/funcs/login.py
+-rw-r--r--   0        0        0      229 2024-04-12 19:46:23.649313 flask_rpc-0.1.5/app/rpc/auth/funcs/logout.py
+-rw-r--r--   0        0        0      221 2024-04-12 19:46:13.766886 flask_rpc-0.1.5/app/rpc/auth/funcs/session.py
+-rw-r--r--   0        0        0      341 2024-04-12 11:18:17.395564 flask_rpc-0.1.5/app/rpc/clients/__init__.py
+-rw-r--r--   0        0        0     1546 2024-04-12 19:46:38.040859 flask_rpc-0.1.5/app/rpc/clients/funcs/__init__.py
+-rw-r--r--   0        0        0     1289 2024-04-12 19:44:05.326618 flask_rpc-0.1.5/app/templates/index.html
+-rw-r--r--   0        0        0       22 2024-04-12 20:06:47.742786 flask_rpc-0.1.5/flask_rpc/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-12 16:20:34.358527 flask_rpc-0.1.5/flask_rpc/latest.py
+-rw-r--r--   0        0        0     2911 2024-04-12 20:04:57.691367 flask_rpc-0.1.5/flask_rpc/version_1_0.py
+-rw-r--r--   0        0        0      415 2024-04-12 11:01:16.320086 flask_rpc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       59 2024-04-10 22:19:07.350737 flask_rpc-0.1.5/requirements.txt
+-rw-r--r--   0        0        0       16 2024-04-12 19:48:22.616554 flask_rpc-0.1.5/requirements_dev.txt
+-rw-r--r--   0        0        0     2808 2024-04-12 16:25:40.835378 flask_rpc-0.1.5/test.py
+-rw-r--r--   0        0        0     2807 1970-01-01 00:00:00.000000 flask_rpc-0.1.5/PKG-INFO
```

### Comparing `flask_rpc-0.1.4/.gitignore` & `flask_rpc-0.1.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -166,7 +166,9 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this from_file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea from_folder.
 #.idea/
 /old_code/
 /Dockerfile
 /src_dif/
+/venv_3_8/
+/venv_3_9/
```

### Comparing `flask_rpc-0.1.4/LICENSE` & `flask_rpc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.4/app/__init__.py` & `flask_rpc-0.1.5/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.4/app/models/clients.py` & `flask_rpc-0.1.5/app/models/users.py`

 * *Files identical despite different names*

### Comparing `flask_rpc-0.1.4/app/models/users.py` & `flask_rpc-0.1.5/app/models/clients.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,49 +9,47 @@
 class Clients(db.Model):
     client_id = db.Column(db.Integer, primary_key=True)
     name = db.Column(db.String(50), nullable=False)
     created_at = db.Column(db.DateTime, default=datetime.now())
     updated_at = db.Column(db.DateTime, default=datetime.now(), onupdate=datetime.now())
 
     @classmethod
-    def create(cls, name: str, **_) -> tuple[bool, str, t.Union[None, t.Self]]:
+    def create(cls, name: str, **_) -> t.Tuple[bool, str, t.Any]:
         client = cls(name=name)
 
         db.session.add(client)
         db.session.commit()
 
         return True, "OK", client
 
     @classmethod
-    def read(cls, client_id: int, **_) -> tuple[bool, str, t.Union[None, t.Self]]:
+    def read(cls, client_id: int, **_) -> t.Tuple[bool, str, t.Any]:
         q = select(cls).where(cls.client_id == client_id)
         r = db.session.execute(q).scalar_one_or_none()
 
         if not r:
             return False, "Client not found.", None
 
         return True, "OK", r
 
     @classmethod
-    def update(
-        cls, client_id: int, name: str, **_
-    ) -> tuple[bool, str, t.Union[None, t.Self]]:
+    def update(cls, client_id: int, name: str, **_) -> t.Tuple[bool, str, t.Any]:
         q = select(cls).where(cls.client_id == client_id)
         r = db.session.execute(q).scalar_one_or_none()
 
         if not r:
             return False, "Client not found.", None
 
         r.name = name
         db.session.commit()
 
         return True, "OK", r
 
     @classmethod
-    def delete(cls, client_id: int, **_) -> tuple[bool, str, t.Union[None, t.Self]]:
+    def delete(cls, client_id: int, **_) -> t.Tuple[bool, str, t.Any]:
         q = select(cls).where(cls.client_id == client_id)
         r = db.session.execute(q).scalar_one_or_none()
 
         if not r:
             return False, "Client not found.", None
 
         db.session.delete(r)
```

### Comparing `flask_rpc-0.1.4/app/rpc/clients/funcs/__init__.py` & `flask_rpc-0.1.5/app/rpc/clients/funcs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,61 @@
-from flask_rpc.latest import RPCResponse
 from app.models.clients import Clients
-
-"""
-The functions below are fairly simple, and it's hard to see the value
-in abstracting the logic into their own functions. However, the idea is
-that as the application grows, these functions will become more complex,
-and it will be easier to manage.
-
-For example, the rpc.clients.funcs package should be the only place where
-the logic for creating, reading, updating, and deleting clients should be
-located.
-
-It's also easier to test these functions in isolation without the need to
-call a route.
-"""
+from flask_rpc.latest import RPCResponse
 
 
-def create_client(params):
-    status, message, result = Clients.create(**params)
+def create_client(data):
+    status, message, result = Clients.create(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, params)
+        return RPCResponse.failed_response(message, data)
 
     return RPCResponse.successful_response(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
-def read_client(params):
-    status, message, result = Clients.read(**params)
+def read_client(data):
+    status, message, result = Clients.read(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, params)
+        return RPCResponse.failed_response(message, data)
 
     return RPCResponse.successful_response(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
-def update_client(params):
-    status, message, result = Clients.update(**params)
+def update_client(data):
+    status, message, result = Clients.update(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, params)
+        return RPCResponse.failed_response(message, data)
 
     return RPCResponse.successful_response(
         data={
             "client_id": result.client_id,
             "name": result.name,
             "created_at": result.created_at,
             "updated_at": result.updated_at,
         }
     )
 
 
-def delete_client(params):
-    status, message, result = Clients.delete(**params)
+def delete_client(data):
+    status, message, result = Clients.delete(**data)
 
     if not status:
-        return RPCResponse.failed_response(message, params)
+        return RPCResponse.failed_response(message, data)
 
     return RPCResponse.successful_response(
         {"client_id": result.client_id, "name": result.name}
     )
```

### Comparing `flask_rpc-0.1.4/app/templates/index.html` & `flask_rpc-0.1.5/app/templates/index.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 <html lang="gb">
 <head>
     <title>Development</title>
     <script src="https://unpkg.com/flask-rpc-js@latest/cdn.js"></script>
     <script>
+        {# The examples below are setting and getting session cookies over fetch #}
         function set_session() {
             fetch(
                 'http://127.0.0.1:5000/rpc/auth',
                 {
                     method: 'POST',
                     headers: {
                         'Content-Type': 'application/json',
                     },
-                    body: frpc('session', null),
+                    body: frpc('login', null),
                 }
             )
                 .then(response => response.json())
                 .then(data => console.log(data));
         }
 
         function do_fetch() {
```

### Comparing `flask_rpc-0.1.4/flask_rpc/version_1_0.py` & `flask_rpc-0.1.5/flask_rpc/version_1_0.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,45 +9,49 @@
     function: str
     data: t.Any
 
 
 class RPCRequest:
     @classmethod
     def build(
-        cls, function: str, data: t.Optional[dict[str, t.Any]] = None
-    ) -> dict[str, t.Any]:
+        cls, function: str, data: t.Optional[t.Dict[str, t.Any]] = None
+    ) -> t.Dict[str, t.Any]:
         return {"frpc": 1.0, "function": function, "data": data}
 
 
 class RPCResponse:
     @classmethod
-    def failed_response(cls, message: str = None, data: dict[str, t.Any] = None):
+    def failed_response(cls, message: str = None, data: t.Dict[str, t.Any] = None):
         r = {"frpc": 1.0, "ok": False}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
 
     @classmethod
-    def successful_response(cls, data: dict[str, t.Any] = None, message: str = None):
+    def successful_response(
+        cls,
+        data: t.Union[str, int, float, list, bool, t.Dict[str, t.Any]] = None,
+        message: str = None,
+    ):
         r = {"frpc": 1.0, "ok": True}
 
         if message:
             r["message"] = message
         if data:
             r["data"] = data
 
         return r
 
 
 class RPC:
-    LOOKUP: dict[str, t.Callable]
+    LOOKUP: t.Dict[str, t.Callable]
 
     def __init__(
         self, app_or_blueprint: t.Union[Flask, Blueprint], url_prefix: str = "/"
     ):
         self.LOOKUP = {}
 
         if not hasattr(app_or_blueprint, "add_url_rule"):
@@ -89,14 +93,14 @@
             return RPCResponse.failed_response("Invalid request.")
 
         try:
             assert rpcm.function in self.LOOKUP
         except AssertionError:
             return RPCResponse.failed_response("Invalid function.")
 
-        if successful_response := self.LOOKUP[rpcm.function](params=rpcm.data):
+        if successful_response := self.LOOKUP[rpcm.function](rpcm.data):
             return successful_response
 
         return RPCResponse.failed_response("Unsuccessful command execution.")
 
 
 __all__ = ["RPC", "RPCResponse", "RPCModel"]
```

### Comparing `flask_rpc-0.1.4/test.py` & `flask_rpc-0.1.5/test.py`

 * *Files identical despite different names*

