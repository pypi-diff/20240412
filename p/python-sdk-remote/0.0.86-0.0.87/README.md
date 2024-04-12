# Comparing `tmp/python-sdk-remote-0.0.86.tar.gz` & `tmp/python-sdk-remote-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-sdk-remote-0.0.86.tar", last modified: Mon Apr  8 16:55:34 2024, max compression
+gzip compressed data, was "python-sdk-remote-0.0.87.tar", last modified: Fri Apr 12 14:36:34 2024, max compression
```

## Comparing `python-sdk-remote-0.0.86.tar` & `python-sdk-remote-0.0.87.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:55:34.518566 python-sdk-remote-0.0.86/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 16:55:34.514566 python-sdk-remote-0.0.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:55:34.510566 python-sdk-remote-0.0.86/python_sdk_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:55:34.514566 python-sdk-remote-0.0.86/python_sdk_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/mini_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/our_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11637 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/valid_json_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/python_sdk_remote/src/validate_environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:55:34.514566 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 16:55:34.000000 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-08 16:55:34.000000 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:55:34.000000 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 16:55:34.000000 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-08 16:55:34.000000 python-sdk-remote-0.0.86/python_sdk_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:55:34.518566 python-sdk-remote-0.0.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 16:55:04.000000 python-sdk-remote-0.0.86/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.790686 python-sdk-remote-0.0.87/python_sdk_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/python_sdk_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/mini_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/our_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/valid_json_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/python_sdk_remote/src/validate_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 14:36:34.000000 python-sdk-remote-0.0.87/python_sdk_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:36:34.794686 python-sdk-remote-0.0.87/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 14:36:17.000000 python-sdk-remote-0.0.87/setup.py
```

### Comparing `python-sdk-remote-0.0.86/PKG-INFO` & `python-sdk-remote-0.0.87/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.86
+Version: 0.0.87
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.86/README.md` & `python-sdk-remote-0.0.87/README.md`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/constants.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/constants.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/mini_logger.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/mini_logger.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/our_object.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/our_object.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/unified_json.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/unified_json.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/utilities.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             return False
 
     logger.end(IS_VALID_TIME_RANGE_METHOD_NAME, object={
         "is_valid_time_range_result": True})
     return True
 
 
-def validate_url(url):
+def validate_url(url: str):
     if url is not None or url != "":
         parsed_url = urlparse(url)
         return parsed_url.scheme and parsed_url.netloc
     return True
 
 
 def is_valid_date_range(date_range: tuple) -> bool:
@@ -121,35 +121,34 @@
                 "is_valid_datetime_range_result": False, "reason": "datetime_range contains non-datetime objects"})
             return False
     logger.end(IS_VALID_DATETIME_RANGE_METHOD_NAME, object={
         "is_valid_datetime_range_result": True})
     return True
 
 
-def is_list_of_dicts(obj):
+def is_list_of_dicts(obj: object) -> bool:
     """
     Check if an object is a list of dictionaries.
 
     Parameters:
         obj (object): The object to be checked.
 
     Returns:
         bool: True if the object is a list of dictionaries, False otherwise.
 
     Example:
         Usage of is_list_of_dicts:
 
-        >>> data = [{'name': 'Alice', 'age': 30}, {'name': 'Bob', 'age': 25}]
-        >>> result = is_list_of_dicts(data)
-        >>> print(result)
+        >>> is_list_of_dicts([{'name': 'Alice', 'age': 30}, {'name': 'Bob', 'age': 25}])
         True
 
-        >>> data = [1, 2, 3]
-        >>> result = is_list_of_dicts(data)
-        >>> print(result)
+        >>> is_list_of_dicts([1, 2, 3])
+        False
+
+        >>> is_list_of_dicts(1)
         False
     """
     IS_LIST_OF_DICTS_FUNCTION_NAME = "is_list_of_dicts"
     logger.start(IS_LIST_OF_DICTS_FUNCTION_NAME, object={"obj": obj})
     try:
         if not isinstance(obj, list):
             is_list_of_dicts_result = False
@@ -247,41 +246,48 @@
 
 
 # TODO Align those methods with typescript-sdk https://github.com/circles-zone/typescript-sdk-remote-typescript-package/blob/dev/typescript-sdk/src/utils/index.ts  # noqa501
 # TODO Take those three functions to a separate file http_response.py
 # TODO Shall we create also createInternalServerErrorHttpResponse(), createOkHttpResponse() like we have in TypeScript?
 
 # Former name was create_http_headers()
-def create_authorization_http_headers(user_jwt: str):
+def create_authorization_http_headers(user_jwt: str) -> dict:
     http_headers = {
         'Content-Type': 'application/json',
         'Authorization': f'Bearer {user_jwt}',
     }
     return http_headers
 
 
-def create_return_http_headers():
+def get_jwt_from_event(event: dict) -> str:
+    auth_header = event.get('headers', {}).get('authorization')
+    if auth_header is None:
+        auth_header = event.get('headers', {}).get('Authorization')
+    return auth_header.split('Bearer ')[1]
+
+
+def create_return_http_headers() -> dict:
     return {
         "Content-Type": "application/json",
         "Access-Control-Allow-Origin": "*",
     }
 
 
 # https://google.github.io/styleguide/jsoncstyleguide.xml?showone=Property_Name_Format#Property_Name_Format
-def create_http_body(body):
+def create_http_body(body: dict) -> str:
     # TODO console.warning() if the body is not a valid camelCase JSON
     # https://stackoverflow.com/questions/17156078/converting-identifier-naming-between-camelcase-and-underscores-during-json-seria
     return json.dumps(body)
 
 
-def get_brand_name():
+def get_brand_name() -> str:
     return our_get_env("BRAND_NAME")
 
 
-def get_environment_name():
+def get_environment_name() -> str:
     environment_name = our_get_env("ENVIRONMENT_NAME")
     EnvironmentName(environment_name)  # if invalid, raises ValueError: x is not a valid EnvironmentName
     return environment_name
 
 
 def our_get_env(key: str, default: str = None, raise_if_not_found: bool = True) -> str:
     result = os.getenv(key, default)
```

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote/src/validate_environment.py` & `python-sdk-remote-0.0.87/python_sdk_remote/src/validate_environment.py`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote.egg-info/PKG-INFO` & `python-sdk-remote-0.0.87/python_sdk_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sdk-remote
-Version: 0.0.86
+Version: 0.0.87
 Summary: PyPI Package for Circles Python SDK Local Python
 Home-page: https://github.com/circles-zone/python-sdk-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-sdk-remote-0.0.86/python_sdk_remote.egg-info/SOURCES.txt` & `python-sdk-remote-0.0.87/python_sdk_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-sdk-remote-0.0.86/setup.py` & `python-sdk-remote-0.0.87/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 PACKAGE_NAME = "python-sdk-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.86',  # https://pypi.org/project/python-sdk-remote/
+    version='0.0.87',  # https://pypi.org/project/python-sdk-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Python SDK Local Python",
     long_description="This is a package for sharing common functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

