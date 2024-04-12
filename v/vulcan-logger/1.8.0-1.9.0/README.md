# Comparing `tmp/vulcan-logger-1.8.0.tar.gz` & `tmp/vulcan-logger-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.8.0.tar", last modified: Fri Apr 12 03:41:17 2024, max compression
+gzip compressed data, was "vulcan-logger-1.9.0.tar", last modified: Fri Apr 12 03:46:43 2024, max compression
```

## Comparing `vulcan-logger-1.8.0.tar` & `vulcan-logger-1.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6935 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 03:41:09.000000 vulcan-logger-1.8.0/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:41:17.723229 vulcan-logger-1.8.0/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 03:41:17.000000 vulcan-logger-1.8.0/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 03:41:17.000000 vulcan-logger-1.8.0/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:41:17.000000 vulcan-logger-1.8.0/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 03:41:17.000000 vulcan-logger-1.8.0/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 03:41:17.000000 vulcan-logger-1.8.0/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 03:46:34.000000 vulcan-logger-1.9.0/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:46:43.006220 vulcan-logger-1.9.0/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 03:46:42.000000 vulcan-logger-1.9.0/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 03:46:42.000000 vulcan-logger-1.9.0/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:46:42.000000 vulcan-logger-1.9.0/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 03:46:42.000000 vulcan-logger-1.9.0/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 03:46:42.000000 vulcan-logger-1.9.0/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.8.0/LICENSE` & `vulcan-logger-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.8.0/PKG-INFO` & `vulcan-logger-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.8.0
+Version: 1.9.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan-logger-1.8.0/tests/test_decorator.py` & `vulcan-logger-1.9.0/tests/test_decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from datetime import datetime
 from typing import List
 from unittest.mock import patch
 
 import pytest
 
-from vulcan_logger.decorator import log, retry, to_json
+from vulcan_logger.decorator import log, rate_limit, retry, to_json
 from vulcan_logger.encoder import Encoder
 
 
 def _sample_function(x: int, y: int = 2) -> int:
     """
     Simple function that adds two integers.
 
@@ -170,26 +170,66 @@
     Test the to_json decorator to ensure it correctly serializes the return value of a function to a JSON string using
     a custom encoder. The function will return a dictionary which should be serialized into a JSON string.
     """
 
     @to_json
     def sample_function():
         return {"name": "Alice", "age": 30, "time": datetime(2020, 5, 17)}
-
     result = sample_function()
     expected_json = json.dumps(
         {"name": "Alice", "age": 30, "time": "2020-05-17T00:00:00"}, cls=Encoder)
-
     assert result == expected_json, "The JSON output from the decorated function did not match the expected JSON string."
 
-    # Also ensure that it raises no error when trying to serialize more complex data types
     @to_json
     def complex_data_function():
         return {"date": datetime.now(), "data": [1, 2, 3]}
-
     try:
         json_result = complex_data_function()
         # this will confirm json_result is a valid JSON string
         json.loads(json_result)
         assert True, "Serialization of complex data types was successful."
     except Exception as e:
         assert False, f"Serialization failed with error: {e}"
+
+
+@pytest.mark.parametrize("num_calls, sleep_time, expected_errors", [
+    (10, 0.1, 0),  # All calls succeed without hitting the rate limit
+    (60, 0.1, 10),  # 10 calls fail because they exceed the limit within the interval
+    (50, 0.1, 0)    # Exactly at the limit, all should pass
+])
+def test_rate_limit(num_calls, sleep_time, expected_errors):
+    """
+    Test the rate_limit decorator to ensure it allows a specified number of function calls within a time interval
+    and blocks additional calls until the interval has elapsed.
+
+    Args:
+        num_calls (int): Number of times to call the decorated function.
+        sleep_time (float): Time to sleep between each call, in seconds.
+        expected_errors (int): Number of times the rate limit should trigger and log an error.
+    """
+
+    @rate_limit(limit=50, interval=10)
+    def test_function():
+        return
+
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
+        for _ in range(num_calls):
+            test_function()
+            time.sleep(sleep_time)
+        assert mock_logger.return_value.error.call_count == expected_errors
+
+
+def test_rate_limit_reset():
+    """
+    Test that the rate limit properly resets after the cooldown interval.
+    """
+    @rate_limit(limit=5, interval=1)  # Very short interval for test speed
+    def test_function():
+        return
+
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
+        for _ in range(5):
+            test_function()  # These should all pass
+        time.sleep(1.1)      # Wait for the interval to pass
+        for _ in range(5):
+            test_function()  # These should also pass after the reset
+        assert mock_logger.return_value.error.call_count == 0
```

### Comparing `vulcan-logger-1.8.0/tests/test_encoder.py` & `vulcan-logger-1.9.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.8.0/tests/test_logger.py` & `vulcan-logger-1.9.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.8.0/vulcan_logger/decorator.py` & `vulcan-logger-1.9.0/vulcan_logger/decorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -180,7 +180,41 @@
         def wrapper(*args, **kwargs) -> str:
             result = func(*args, **kwargs)
             return json.dumps(result, cls=Encoder, ensure_ascii=False)
         return wrapper
     if _func is not None:
         return decorator_to_json(_func)
     return decorator_to_json
+
+
+def rate_limit(limit: int, interval: float):
+    """
+    Decorator to rate limit the execution of a function. Allows a burst of 'limit' calls,
+    and then enforces a cooldown period of 'interval' seconds before allowing another burst.
+
+    Args:
+        limit (int): Maximum number of calls allowed within the burst.
+        interval (float): Cooldown interval (in seconds) after a burst before resetting the limit.
+    """
+
+    def decorator(func):
+        call_times = []
+        first_call_time = None
+
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            nonlocal first_call_time
+            now = time.time()
+            if first_call_time and now - first_call_time > interval:
+                call_times.clear()
+                first_call_time = None
+            if not first_call_time:
+                first_call_time = now
+            if len(call_times) < limit:
+                call_times.append(now)
+                return func(*args, **kwargs)
+            else:
+                logger = Logger(func.__module__)
+                logger.error(f"Rate limit exceeded for {func.__name__}")
+                return
+        return wrapper
+    return decorator
```

### Comparing `vulcan-logger-1.8.0/vulcan_logger/encoder.py` & `vulcan-logger-1.9.0/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.8.0/vulcan_logger/logger.py` & `vulcan-logger-1.9.0/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.8.0/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.9.0/vulcan_logger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.8.0
+Version: 1.9.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

