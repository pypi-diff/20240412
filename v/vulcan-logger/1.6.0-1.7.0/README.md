# Comparing `tmp/vulcan-logger-1.6.0.tar.gz` & `tmp/vulcan-logger-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.6.0.tar", last modified: Fri Apr 12 00:58:52 2024, max compression
+gzip compressed data, was "vulcan-logger-1.7.0.tar", last modified: Fri Apr 12 01:36:09 2024, max compression
```

## Comparing `vulcan-logger-1.6.0.tar` & `vulcan-logger-1.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.129582 vulcan-logger-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5614 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:36:09.260316 vulcan-logger-1.7.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 01:36:09.260316 vulcan-logger-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:36:09.260316 vulcan-logger-1.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:36:09.256316 vulcan-logger-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:36:09.260316 vulcan-logger-1.7.0/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6567 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 01:36:00.000000 vulcan-logger-1.7.0/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:36:09.260316 vulcan-logger-1.7.0/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 01:36:09.000000 vulcan-logger-1.7.0/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 01:36:09.000000 vulcan-logger-1.7.0/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:36:09.000000 vulcan-logger-1.7.0/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 01:36:09.000000 vulcan-logger-1.7.0/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 01:36:09.000000 vulcan-logger-1.7.0/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.6.0/LICENSE` & `vulcan-logger-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.6.0/PKG-INFO` & `vulcan-logger-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.6.0
+Version: 1.7.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan-logger-1.6.0/tests/test_decorator.py` & `vulcan-logger-1.7.0/tests/test_decorator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from unittest.mock import patch
-import pytest
+import json
 import time
+from datetime import datetime
 from typing import List
-from vulcan_logger.decorator import log, retry, Logger
+from unittest.mock import patch
+
+import pytest
+
+from vulcan_logger.decorator import log, retry, to_json
+from vulcan_logger.encoder import Encoder
 
 
 def _sample_function(x: int, y: int = 2) -> int:
     """
     Simple function that adds two integers.
 
     Args:
@@ -154,7 +159,37 @@
             decorated(attempts=attempts_list, max_attempts=max_attempts)
         except ValueError:
             pass
         expected_warning_calls = max_attempts - 1
         assert mock_logger.return_value.warning.call_count == expected_warning_calls
         assert mock_logger.return_value.error.called == (
             attempts_list[0] == max_attempts)
+
+
+def test_to_json_decorator():
+    """
+    Test the to_json decorator to ensure it correctly serializes the return value of a function to a JSON string using
+    a custom encoder. The function will return a dictionary which should be serialized into a JSON string.
+    """
+
+    @to_json
+    def sample_function():
+        return {"name": "Alice", "age": 30, "time": datetime(2020, 5, 17)}
+
+    result = sample_function()
+    expected_json = json.dumps(
+        {"name": "Alice", "age": 30, "time": "2020-05-17T00:00:00"}, cls=Encoder)
+
+    assert result == expected_json, "The JSON output from the decorated function did not match the expected JSON string."
+
+    # Also ensure that it raises no error when trying to serialize more complex data types
+    @to_json
+    def complex_data_function():
+        return {"date": datetime.now(), "data": [1, 2, 3]}
+
+    try:
+        json_result = complex_data_function()
+        # this will confirm json_result is a valid JSON string
+        json.loads(json_result)
+        assert True, "Serialization of complex data types was successful."
+    except Exception as e:
+        assert False, f"Serialization failed with error: {e}"
```

### Comparing `vulcan-logger-1.6.0/tests/test_encoder.py` & `vulcan-logger-1.7.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.6.0/tests/test_logger.py` & `vulcan-logger-1.7.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.6.0/vulcan_logger/decorator.py` & `vulcan-logger-1.7.0/vulcan_logger/decorator.py`

 * *Files 8% similar despite different names*

```diff
@@ -152,7 +152,31 @@
                             f"{func.__name__} retry attemps failed: {e}")
                         break
             raise last_exception
         return wrapper
     if _func is not None:
         return decorator_retry(_func)
     return decorator_retry
+
+
+def to_json(_func: Union[Callable[[F], F], F] = None) -> Union[Callable[[F], F], F]:
+    """
+    A decorator that serializes the return value of the decorated function to JSON.
+    This uses a custom JSON encoder to handle complex data types not typically serializable by the default JSON encoder.
+
+    Args:
+        _func (Callable[[F], F], optional): The function to decorate. If None, this allows other parameters to be 
+            passed first as keyword arguments. Defaults to None.
+
+    Returns:
+        Callable[[F], F]: The decorated function with its return value serialized as a JSON string.
+    """
+
+    def decorator_to_json(func: F) -> F:
+        @wraps(func)
+        def wrapper(*args, **kwargs) -> str:
+            result = func(*args, **kwargs)
+            return json.dumps(result, cls=Encoder, ensure_ascii=False)
+        return wrapper
+    if _func is not None:
+        return decorator_to_json(_func)
+    return decorator_to_json
```

### Comparing `vulcan-logger-1.6.0/vulcan_logger/encoder.py` & `vulcan-logger-1.7.0/vulcan_logger/encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,12 +40,15 @@
         elif isinstance(obj, Enum):
             return obj.value
         elif isinstance(obj, uuid.UUID):
             return str(obj)
         elif HAS_NUMPY_PANDAS:
             if isinstance(obj, np.ndarray):
                 return obj.tolist()
-            elif 'pandas' in str(type(obj)):
-                return obj.to_dict(orient='records')
+            elif "pandas" in str(type(obj)):
+                return obj.to_dict(orient="records")
         elif hasattr(obj, "__dict__"):
-            return obj.__dict__
-        return json.JSONEncoder.default(self, obj)
+            # Serialize objects by their dictionary representation, filtering out non-serializable attributes
+            return {key: self.default(value) for key, value in obj.__dict__.items()}
+        else:
+            # Skip serialization for other non-handled types
+            return str(obj)  # Fallback to a simple string representation
```

### Comparing `vulcan-logger-1.6.0/vulcan_logger/logger.py` & `vulcan-logger-1.7.0/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.6.0/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.7.0/vulcan_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.6.0
+Version: 1.7.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

