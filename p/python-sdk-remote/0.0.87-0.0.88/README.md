# Comparing `tmp/python-sdk-remote-0.0.87.tar.gz` & `tmp/python-sdk-remote-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sdk-remote-0.0.87.tar", last modified: Fri Apr 12 14:36:34 2024, max compression
+gzip compressed data, was "python-sdk-remote-0.0.88.tar", last modified: Fri Apr 12 14:44:51 2024, max compression
```

## Comparing `python-sdk-remote-0.0.87.tar` & `python-sdk-remote-0.0.88.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.790686 python-sdk-remote-0.0.87/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:44:51.496799 python-sdk-remote-0.0.88/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:44:51.496799 python-sdk-remote-0.0.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:44:51.492799 python-sdk-remote-0.0.88/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:44:51.496799 python-sdk-remote-0.0.88/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:44:51.496799 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 14:44:51.000000 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 14:44:51.000000 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:44:51.000000 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 14:44:51.000000 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 14:44:51.000000 python-sdk-remote-0.0.88/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:44:51.496799 python-sdk-remote-0.0.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-12 14:44:36.000000 python-sdk-remote-0.0.88/setup.py
```

### Comparing `python-sdk-remote-0.0.87/PKG-INFO` & `python-sdk-remote-0.0.88/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.87
+Version: 0.0.88
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: url-remote
+Requires-Dist: http-status-codes
 
 This is a package for sharing common functions used in different repositories
```

### Comparing `python-sdk-remote-0.0.87/README.md` & `python-sdk-remote-0.0.88/README.md`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/constants.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/mini_logger.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/our_object.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/unified_json.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/utilities.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 from datetime import date, datetime, time, timedelta
 from dotenv import load_dotenv
 from url_remote.environment_name_enum import EnvironmentName
 from urllib.parse import urlparse
+from http_constants import status
 
 from .mini_logger import MiniLogger as logger
 
 load_dotenv()
 
 
 def timedelta_to_time_format(time_delta: timedelta) -> str:
@@ -247,19 +248,18 @@
 
 # TODO Align those methods with typescript-sdk https://github.com/circles-zone/typescript-sdk-remote-typescript-package/blob/dev/typescript-sdk/src/utils/index.ts  # noqa501
 # TODO Take those three functions to a separate file http_response.py
 # TODO Shall we create also createInternalServerErrorHttpResponse(), createOkHttpResponse() like we have in TypeScript?
 
 # Former name was create_http_headers()
 def create_authorization_http_headers(user_jwt: str) -> dict:
-    http_headers = {
+    return {
         'Content-Type': 'application/json',
         'Authorization': f'Bearer {user_jwt}',
     }
-    return http_headers
 
 
 def get_jwt_from_event(event: dict) -> str:
     auth_header = event.get('headers', {}).get('authorization')
     if auth_header is None:
         auth_header = event.get('headers', {}).get('Authorization')
     return auth_header.split('Bearer ')[1]
@@ -267,14 +267,28 @@
 
 def create_return_http_headers() -> dict:
     return {
         "Content-Type": "application/json",
         "Access-Control-Allow-Origin": "*",
     }
 
+def create_error_http_response(exception: Exception) -> dict:
+    return {
+            "statusCode": status.BAD_GATEWAY,
+            "headers": create_return_http_headers(),
+            "body": create_http_body({"error": str(exception)})
+        }
+
+def create_ok_http_response(body: dict) -> dict:
+    return {
+        "statusCode": status.OK,
+        "headers": create_return_http_headers(),
+        "body": create_http_body(body)
+    }
+
 
 # https://google.github.io/styleguide/jsoncstyleguide.xml?showone=Property_Name_Format#Property_Name_Format
 def create_http_body(body: dict) -> str:
     # TODO console.warning() if the body is not a valid camelCase JSON
     # https://stackoverflow.com/questions/17156078/converting-identifier-naming-between-camelcase-and-underscores-during-json-seria
     return json.dumps(body)
```

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote/src/validate_environment.py` & `python-sdk-remote-0.0.88/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote.egg-info/PKG-INFO` & `python-sdk-remote-0.0.88/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.87
+Version: 0.0.88
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
 Requires-Dist: url-remote
+Requires-Dist: http-status-codes
 
 This is a package for sharing common functions used in different repositories
```

### Comparing `python-sdk-remote-0.0.87/python_sdk_remote.egg-info/SOURCES.txt` & `python-sdk-remote-0.0.88/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.87/setup.py` & `python-sdk-remote-0.0.88/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.87',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.88',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
@@ -20,10 +20,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "python-dotenv",
-        "url-remote"
+        "url-remote",
+        "http-status-codes"
     ]
 )
```

