# Comparing `tmp/drf_error_handler-0.14.0.tar.gz` & `tmp/drf_error_handler-0.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_error_handler-0.14.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drf_error_handler-0.14.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drf_error_handler-0.14.0.tar` & `drf_error_handler-0.14.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.14.0/LICENSE
--rw-r--r--   0        0        0     3946 2024-04-11 09:40:24.445050 drf_error_handler-0.14.0/README.md
--rw-r--r--   0        0        0       68 2024-04-11 09:46:01.424078 drf_error_handler-0.14.0/drf_error_handler/__init__.py
--rw-r--r--   0        0        0      149 2024-04-11 09:36:50.402046 drf_error_handler-0.14.0/drf_error_handler/apps.py
--rw-r--r--   0        0        0     3272 2024-04-11 09:35:25.189498 drf_error_handler-0.14.0/drf_error_handler/exceptions.py
--rw-r--r--   0        0        0     4633 2024-04-11 01:00:35.078000 drf_error_handler-0.14.0/drf_error_handler/formatter.py
--rw-r--r--   0        0        0     7263 2024-04-11 01:01:47.049815 drf_error_handler-0.14.0/drf_error_handler/handler.py
--rw-r--r--   0        0        0    14833 2024-04-11 09:38:28.371623 drf_error_handler-0.14.0/drf_error_handler/openapi.py
--rw-r--r--   0        0        0    10597 2024-04-10 09:09:34.411384 drf_error_handler-0.14.0/drf_error_handler/openapi_hooks.py
--rw-r--r--   0        0        0     3435 2024-04-11 00:59:42.813350 drf_error_handler-0.14.0/drf_error_handler/openapi_serializers.py
--rw-r--r--   0        0        0    18810 2024-04-11 00:47:13.504479 drf_error_handler-0.14.0/drf_error_handler/openapi_utils.py
--rw-r--r--   0        0        0     8811 2024-04-11 09:38:49.055569 drf_error_handler-0.14.0/drf_error_handler/openapi_validation_errors.py
--rw-r--r--   0        0        0        0 2024-04-10 09:09:35.928084 drf_error_handler-0.14.0/drf_error_handler/py.typed
--rw-r--r--   0        0        0     3645 2024-04-11 09:30:32.773921 drf_error_handler-0.14.0/drf_error_handler/settings.py
--rw-r--r--   0        0        0     1062 2024-04-11 09:36:59.302312 drf_error_handler-0.14.0/drf_error_handler/types.py
--rw-r--r--   0        0        0     2143 2024-04-11 09:45:43.377245 drf_error_handler-0.14.0/pyproject.toml
--rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 drf_error_handler-0.14.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-11 08:59:04.011100 drf_error_handler-0.14.1/LICENSE
+-rw-r--r--   0        0        0     3946 2024-04-11 09:40:24.445050 drf_error_handler-0.14.1/README.md
+-rw-r--r--   0        0        0       68 2024-04-11 10:00:44.756681 drf_error_handler-0.14.1/drf_error_handler/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-11 09:36:50.402046 drf_error_handler-0.14.1/drf_error_handler/apps.py
+-rw-r--r--   0        0        0     3272 2024-04-11 09:35:25.189498 drf_error_handler-0.14.1/drf_error_handler/exceptions.py
+-rw-r--r--   0        0        0     4633 2024-04-11 01:00:35.078000 drf_error_handler-0.14.1/drf_error_handler/formatter.py
+-rw-r--r--   0        0        0     7263 2024-04-11 01:01:47.049815 drf_error_handler-0.14.1/drf_error_handler/handler.py
+-rw-r--r--   0        0        0    14833 2024-04-11 09:38:28.371623 drf_error_handler-0.14.1/drf_error_handler/openapi.py
+-rw-r--r--   0        0        0    10597 2024-04-10 09:09:34.411384 drf_error_handler-0.14.1/drf_error_handler/openapi_hooks.py
+-rw-r--r--   0        0        0     3435 2024-04-11 00:59:42.813350 drf_error_handler-0.14.1/drf_error_handler/openapi_serializers.py
+-rw-r--r--   0        0        0    18810 2024-04-11 00:47:13.504479 drf_error_handler-0.14.1/drf_error_handler/openapi_utils.py
+-rw-r--r--   0        0        0     8811 2024-04-11 09:38:49.055569 drf_error_handler-0.14.1/drf_error_handler/openapi_validation_errors.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:09:35.928084 drf_error_handler-0.14.1/drf_error_handler/py.typed
+-rw-r--r--   0        0        0     3645 2024-04-11 09:30:32.773921 drf_error_handler-0.14.1/drf_error_handler/settings.py
+-rw-r--r--   0        0        0     1073 2024-04-11 10:00:14.462657 drf_error_handler-0.14.1/drf_error_handler/types.py
+-rw-r--r--   0        0        0     2143 2024-04-11 10:01:31.851099 drf_error_handler-0.14.1/pyproject.toml
+-rw-r--r--   0        0        0     5780 1970-01-01 00:00:00.000000 drf_error_handler-0.14.1/PKG-INFO
```

### Comparing `drf_error_handler-0.14.0/LICENSE` & `drf_error_handler-0.14.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/README.md` & `drf_error_handler-0.14.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/exceptions.py` & `drf_error_handler-0.14.1/drf_error_handler/exceptions.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/formatter.py` & `drf_error_handler-0.14.1/drf_error_handler/formatter.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/handler.py` & `drf_error_handler-0.14.1/drf_error_handler/handler.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/openapi.py` & `drf_error_handler-0.14.1/drf_error_handler/openapi.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/openapi_hooks.py` & `drf_error_handler-0.14.1/drf_error_handler/openapi_hooks.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/openapi_serializers.py` & `drf_error_handler-0.14.1/drf_error_handler/openapi_serializers.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/openapi_utils.py` & `drf_error_handler-0.14.1/drf_error_handler/openapi_utils.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/openapi_validation_errors.py` & `drf_error_handler-0.14.1/drf_error_handler/openapi_validation_errors.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/settings.py` & `drf_error_handler-0.14.1/drf_error_handler/settings.py`

 * *Files identical despite different names*

### Comparing `drf_error_handler-0.14.0/drf_error_handler/types.py` & `drf_error_handler-0.14.1/drf_error_handler/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 BUSINESS_CODE_NAME = cast(str, package_settings.EXCEPTION_RESPONSE_BUSINESS_ATTRIBUTE)
 class ErrorType(str, Enum):
     VALIDATION_ERROR = "validation_error"
     CLIENT_ERROR = "client_error"
     SERVER_ERROR = "server_error"
 
 
+@dataclass
 class Error:
     detail: str
     attr: Optional[str]
     BUSINESS_CODE_NAME: Optional[int]
 
 
 @dataclass
```

### Comparing `drf_error_handler-0.14.0/pyproject.toml` & `drf_error_handler-0.14.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     "drf-spectacular>=0.27.0",
     "inflection",
 ]
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.14.0"
+current = "0.14.1"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `drf_error_handler-0.14.0/PKG-INFO` & `drf_error_handler-0.14.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-error-handler
-Version: 0.14.0
+Version: 0.14.1
 Summary: Standardize your API error responses.
 Keywords: standardized errors,errors formatter,django rest framework,exception handler
 Author: Ghazi Abbassi, Nazar Korchizhinskiy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

