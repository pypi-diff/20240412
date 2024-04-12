# Comparing `tmp/feliz-0.0.2.tar.gz` & `tmp/feliz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feliz-0.0.2.tar", last modified: Tue Jan 30 03:02:24 2024, max compression
+gzip compressed data, was "feliz-0.0.3.tar", last modified: Fri Apr 12 07:11:57 2024, max compression
```

## Comparing `feliz-0.0.2.tar` & `feliz-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-01-30 03:02:24.120413 feliz-0.0.2/
--rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-01-22 07:12:10.000000 feliz-0.0.2/LICENSE
--rw-r--r--   0 zenith3092   (501) staff       (20)      527 2024-01-30 03:02:24.120297 feliz-0.0.2/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)       54 2024-01-22 07:12:10.000000 feliz-0.0.2/README.md
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-01-30 03:02:24.119574 feliz-0.0.2/feliz/
--rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-01-22 07:30:36.000000 feliz-0.0.2/feliz/__init__.py
--rw-r--r--   0 zenith3092   (501) staff       (20)     3999 2024-01-22 08:21:35.000000 feliz-0.0.2/feliz/api_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)      348 2024-01-22 07:14:13.000000 feliz-0.0.2/feliz/auth_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)     1860 2024-01-22 07:14:13.000000 feliz-0.0.2/feliz/file_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)     2063 2024-01-30 02:59:37.000000 feliz-0.0.2/feliz/global_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)     9599 2024-01-23 05:05:03.000000 feliz-0.0.2/feliz/initialware_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)     1360 2024-01-22 07:44:29.000000 feliz-0.0.2/feliz/inspector_tools.py
--rw-r--r--   0 zenith3092   (501) staff       (20)    16423 2024-01-24 09:09:38.000000 feliz-0.0.2/feliz/middleware_tools.py
-drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-01-30 03:02:24.120137 feliz-0.0.2/feliz.egg-info/
--rw-r--r--   0 zenith3092   (501) staff       (20)      527 2024-01-30 03:02:24.000000 feliz-0.0.2/feliz.egg-info/PKG-INFO
--rw-r--r--   0 zenith3092   (501) staff       (20)      347 2024-01-30 03:02:24.000000 feliz-0.0.2/feliz.egg-info/SOURCES.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-01-30 03:02:24.000000 feliz-0.0.2/feliz.egg-info/dependency_links.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       84 2024-01-30 03:02:24.000000 feliz-0.0.2/feliz.egg-info/requires.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)        6 2024-01-30 03:02:24.000000 feliz-0.0.2/feliz.egg-info/top_level.txt
--rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-01-30 03:02:24.120449 feliz-0.0.2/setup.cfg
--rw-r--r--   0 zenith3092   (501) staff       (20)      862 2024-01-30 03:01:32.000000 feliz-0.0.2/setup.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 07:11:57.196282 feliz-0.0.3/
+-rw-r--r--   0 zenith3092   (501) staff       (20)     1071 2024-01-22 07:12:10.000000 feliz-0.0.3/LICENSE
+-rw-r--r--   0 zenith3092   (501) staff       (20)    10834 2024-04-12 07:11:57.196097 feliz-0.0.3/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)    10361 2024-04-12 07:10:59.000000 feliz-0.0.3/README.md
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 07:11:57.194959 feliz-0.0.3/feliz/
+-rw-r--r--   0 zenith3092   (501) staff       (20)        0 2024-01-22 07:30:36.000000 feliz-0.0.3/feliz/__init__.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)     4749 2024-04-12 07:10:59.000000 feliz-0.0.3/feliz/api_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)      348 2024-01-22 07:14:13.000000 feliz-0.0.3/feliz/auth_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)     1860 2024-01-22 07:14:13.000000 feliz-0.0.3/feliz/file_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)     2063 2024-01-30 02:59:37.000000 feliz-0.0.3/feliz/global_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    11227 2024-04-12 07:10:59.000000 feliz-0.0.3/feliz/initialware_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)     1360 2024-01-22 07:44:29.000000 feliz-0.0.3/feliz/inspector_tools.py
+-rw-r--r--   0 zenith3092   (501) staff       (20)    16423 2024-01-24 09:09:38.000000 feliz-0.0.3/feliz/middleware_tools.py
+drwxr-xr-x   0 zenith3092   (501) staff       (20)        0 2024-04-12 07:11:57.195894 feliz-0.0.3/feliz.egg-info/
+-rw-r--r--   0 zenith3092   (501) staff       (20)    10834 2024-04-12 07:11:57.000000 feliz-0.0.3/feliz.egg-info/PKG-INFO
+-rw-r--r--   0 zenith3092   (501) staff       (20)      347 2024-04-12 07:11:57.000000 feliz-0.0.3/feliz.egg-info/SOURCES.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        1 2024-04-12 07:11:57.000000 feliz-0.0.3/feliz.egg-info/dependency_links.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       84 2024-04-12 07:11:57.000000 feliz-0.0.3/feliz.egg-info/requires.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)        6 2024-04-12 07:11:57.000000 feliz-0.0.3/feliz.egg-info/top_level.txt
+-rw-r--r--   0 zenith3092   (501) staff       (20)       38 2024-04-12 07:11:57.196326 feliz-0.0.3/setup.cfg
+-rw-r--r--   0 zenith3092   (501) staff       (20)      862 2024-04-12 07:10:59.000000 feliz-0.0.3/setup.py
```

### Comparing `feliz-0.0.2/LICENSE` & `feliz-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feliz-0.0.2/feliz/api_tools.py` & `feliz-0.0.3/feliz/api_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,31 +13,32 @@
         **options: The options of the request.
     
     Returns:
         func: The function to handle the request with the following parameters:
         - input_request: The input request from the client.
         - DB: The database objects (Postgres Handler).
         - CONFIGS: The configurations of the server.
-        - API: The configurations of the API.
+        - API_CONFIGS: The configurations of the API.
+        - USER_DATA: The informations of the user.
     """
     def decorator(func):
         @blueprint.route(endpoint, **options)
         @wraps(func)
         def wrapper():
             if api_use_inspector(request):
                 user_list = g.get("user_list", [])
                 if len(user_list) == 1:
                     user_data = user_list[0]
                 else:
                     user_data = {}
                 params = {"input_request": g.get("input_request", {}),
-                        "DB": g.get("DB", {}),
-                        "USER_DATA": user_data,
-                        "CONFIGS": g.get("CONFIGS", {}),
-                        "API_CONFIGS": g.get("API_CONFIGS", {})}
+                          "API_CONFIGS":   g.get("API_CONFIGS", {}),
+                          "CONFIGS":       g.get("CONFIGS", {}),
+                          "DB":            g.get("DB", {}),
+                          "USER_DATA":     user_data}
                 return func(**params)
             else:
                 raise DevelopmentError("The server_api.yaml is not used, so 'handler' decorator is invalid.")
         return wrapper
     return decorator
 
 def TrueResponse(message: str, content=None) -> dict:
@@ -49,56 +50,73 @@
         content (any): The content to return to the client.
     
     Returns:
         dict: The message to return to the client.
     """
     return {"indicator": True, "message": message, "content": content}
 
-def FalseResponse(message: str) -> dict:
+def FalseResponse(message: str, content=None) -> dict:
     """
     This function is used to return the message to the client with {"indicator": False, "message": message}
     
     Args:
         message (str): The message to return to the client.
     
     Returns:
         dict: The message to return to the client.
     """
-    raise IndicatorFalseException(message)
+    raise IndicatorFalseException(message, content=content)
 
 class IndicatorFalseException(Exception):
     """
     This class is used to raise errors in the server.
     If developers want to return indicator False, they should raise this error.
     Then, server will return the message to the client with {"indicator": False, "message": message}
     """
-    def __init__(self, message):
+    def __init__(self, message, content=None):
         super().__init__()
         self.message = message
+        self.content = content
         self.filename, self.lineno, self.function, self.text = traceback.extract_stack()[-2]
     
     def __str__(self):
-        # logging.warning("\nServer API Indicator False:")
-        # logging.warning(f"{self.filename}  Line:{self.lineno}  {self.function}")
-        # logging.warning(self.message, "\n")
         return self.message
+    
+    def get_json_response(self):
+        return {"indicator": False, "message": self.message, "content": self.content}
 
 class DevelopmentError(Exception):
     def __init__(self, message):
         super().__init__()
         self.message = message
         self.filename, self.lineno, self.function, self.text = traceback.extract_stack()[-2]
     
     def __str__(self):
-        print("\nServer Development Error:")
-        print(f"{self.filename}   Line:{self.lineno} {self.function}")
-        print(self.message, "\n")
         return self.message
 
-def error_handler(e):
-    if not isinstance(e, IndicatorFalseException):
+def error_handler(e, loggerIndicatorFalse=False):
+    """
+    This function is used to handle the error in the server.
+
+    Args:
+        e (Exception): The exception to handle.
+        loggerIndicatorFalse (bool): If True, the server will log the error message when the class is IndicatorFalseException.
+    """
+    if isinstance(e, IndicatorFalseException):
+        if loggerIndicatorFalse:
+            logging.warning(f"\n============ Server API Indicator False ============")
+            logging.warning(traceback.format_exc())
+            logging.warning("=====================================================\n")
+        return e.get_json_response()
+    else:
         logging.warning(f"\n====================================================")
         logging.warning(traceback.format_exc())
         logging.warning("=====================================================\n")
+        return {"indicator": False, "message": str(e), "content": None}
 
 def api_route_register(app, blueprint: Blueprint):
-    app.register_blueprint(blueprint, url_prefix=f"/api/{blueprint.name}")
+    """
+    This function is used to register the blueprint to the app.
+    The url_prefix is f"/api/{blueprint.name}".
+    """
+    app.register_blueprint(blueprint, url_prefix=f"/api/{blueprint.name}")
+
```

### Comparing `feliz-0.0.2/feliz/file_tools.py` & `feliz-0.0.3/feliz/file_tools.py`

 * *Files identical despite different names*

### Comparing `feliz-0.0.2/feliz/global_tools.py` & `feliz-0.0.3/feliz/global_tools.py`

 * *Files identical despite different names*

### Comparing `feliz-0.0.2/feliz/initialware_tools.py` & `feliz-0.0.3/feliz/initialware_tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import datetime
 import time
 import os
 from abc import ABC, abstractmethod
 from flask import Flask
+from flask.json.provider import DefaultJSONProvider, _default
 from flask_jwt_extended import JWTManager
 from flask_cors import CORS
 from .file_tools import read_ini
 from .global_tools import load_globals_from_yaml, get_configs, set_db, get_globals
 from .inspector_tools import jwt_use_inspector, cors_use_inspector, db_use_inspector
 
 ## =============== Original Initialware =============== ##
@@ -112,34 +113,39 @@
             if EXPIRE_HOURS == "INFINITE":
                 JWT_CONFIGS.update({"JWT_ACCESS_TOKEN_EXPIRES": False})
             else:
                 JWT_CONFIGS.update({"JWT_ACCESS_TOKEN_EXPIRES": datetime.timedelta(hours=JWT_CONFIGS["EXPIRE_HOURS"])})
             prev_data["app"].config.update(JWT_CONFIGS)
             jwt = JWTManager(prev_data["app"])
             
+            RETURN_MESSAGE = JWT_CONFIGS.get("MESSAGE", {})
+
             @jwt.unauthorized_loader
             def unauthorized_callback(error):
-                return {'indicator': False, 'message': 'Missing JWT token'}
+                return {"indicator": False, "message": RETURN_MESSAGE.get("UNAUTHORIZED", "Missing JWT token")}
 
             @jwt.invalid_token_loader
             def invalid_token_callback(error):
-                return {'indicator': False, 'message': 'Invalid JWT token'}
+                return {"indicator": False, "message": RETURN_MESSAGE.get("INVALID_TOKEN", "Invalid JWT token")}
 
             @jwt.revoked_token_loader
             def revoked_token_callback(error):
-                return {'indicator': False, 'message': 'Revoked JWT token'}
+                return {"indicator": False, "message": RETURN_MESSAGE.get("REVOKED_TOKEN", "Revoked JWT token")}
 
             @jwt.expired_token_loader
             def expired_token_callback(error, expired_token):
-                return {'indicator': False, 'message': 'Your login session has expired, please log in again.'}
+                return {"indicator": False, "message": RETURN_MESSAGE.get("EXPIRED_TOKEN", "Expired JWT token")}
         return prev_data
 
 class CorsInitialware(Initialware):
     """
     The CorsInitialware class is used to initialize the CORS.
+    
+    Args:
+        settings (dict)
     """
     def __init__(self, settings={}):
         self.kwargs = settings
     
     def process(self, prev_data):
         """
         Initialize the CORS.
@@ -255,8 +261,39 @@
                         key = keys_list[index]
                         model = init_models[key]
                         model.create_sql()
                         if index == len(keys_list) - 1:
                             model.execute_sql(db_obj)
                             model.clear_sql()
                 set_db(PostgresInitialware.POSTGRES, section, db_obj)
+        return prev_data
+
+class JsonifyInitialware(Initialware):
+    """
+    The JsonifyInitialware class is used to define the method of jsonify.
+    Some classes may not be able to use jsonify directly, so this class is used to define jsonify.
+    
+    Args:
+        customized_jsonify (function): The customized jsonify function. The function must have two arguments: obj and default_jsonify.
+            \- obj: The object to jsonify.
+            \- default_jsonify: If the obj is not the type that the customized jsonify function can handle, you should use this function to jsonify the obj.
+    
+    Example:
+        def customized_jsonify(obj, default_jsonify):
+            if isinstance(obj, YourClass):
+                return obj.to_json()
+            return default_jsonify(obj)
+    """
+    def __init__(self, customized_jsonify=None):
+        self.customized_jsonify = customized_jsonify
+    
+    def process(self, prev_data: dict):
+        class CustomJSONEncoder(DefaultJSONProvider):
+            @staticmethod
+            def default_action(obj):
+                if self.customized_jsonify:
+                    return self.customized_jsonify(obj, default_jsonify=_default)
+                else:
+                    return _default(obj)
+            default = default_action
+        prev_data["app"].json = CustomJSONEncoder(prev_data["app"])
         return prev_data
```

### Comparing `feliz-0.0.2/feliz/inspector_tools.py` & `feliz-0.0.3/feliz/inspector_tools.py`

 * *Files identical despite different names*

### Comparing `feliz-0.0.2/feliz/middleware_tools.py` & `feliz-0.0.3/feliz/middleware_tools.py`

 * *Files identical despite different names*

### Comparing `feliz-0.0.2/setup.py` & `feliz-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open(os.path.join(os.path.dirname(__file__), "requirements.txt"), "r") as f:
     requirements = f.read().split("\n")
 
 setuptools.setup(
     name="feliz",
-    version="0.0.2",
+    version="0.0.3",
     author="Vincent Wu, Linga Chen, Brian Yin",
     author_email="zenith3092@gmail.com",
     description="A framework designed to assist in using Flask",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zenith3092/feliz",
     license="MIT",
```

