# Comparing `tmp/vulcan-logger-1.5.6.tar.gz` & `tmp/vulcan-logger-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.5.6.tar", last modified: Thu Apr 11 23:10:06 2024, max compression
+gzip compressed data, was "vulcan-logger-1.6.0.tar", last modified: Fri Apr 12 00:58:52 2024, max compression
```

## Comparing `vulcan-logger-1.5.6.tar` & `vulcan-logger-1.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-11 23:09:58.000000 vulcan-logger-1.5.6/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 23:10:06.136261 vulcan-logger-1.5.6/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-11 23:10:06.000000 vulcan-logger-1.5.6/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-11 23:10:06.000000 vulcan-logger-1.5.6/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 23:10:06.000000 vulcan-logger-1.5.6/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 23:10:06.000000 vulcan-logger-1.5.6/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-11 23:10:06.000000 vulcan-logger-1.5.6/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.129582 vulcan-logger-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8174 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5614 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 00:58:43.000000 vulcan-logger-1.6.0/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:58:52.133582 vulcan-logger-1.6.0/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 00:58:52.000000 vulcan-logger-1.6.0/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.5.6/LICENSE` & `vulcan-logger-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.6/PKG-INFO` & `vulcan-logger-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.6
+Version: 1.6.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan-logger-1.5.6/tests/test_encoder.py` & `vulcan-logger-1.6.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.6/tests/test_logger.py` & `vulcan-logger-1.6.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.6/vulcan_logger/decorator.py` & `vulcan-logger-1.6.0/vulcan_logger/decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -107,7 +107,52 @@
                 result = func(*args, **kwargs)
             return result
         return wrapper
     if _func is None:
         return decorator_log
     else:
         return decorator_log(_func)
+
+
+def retry(_func: Optional[F] = None, *, retries: int = 3, delay: Union[int, float] = 1) -> Union[Callable[[F], F], F]:
+    """
+    Decorator to retry a function if it raises an exception. Retries the function a specified number of times with
+    a given delay between each attempt. If all attempts fail, the last exception is raised.
+
+    Args:
+        _func: The function to be decorated. Defaults to None, allowing other parameters to be specified first.
+        retries: The maximum number of retries before giving up and raising the exception.
+        delay: The delay between retries in seconds, which can be an integer or a float for partial seconds.
+
+    Returns:
+        The decorated function that will retry on exceptions, or raises the last encountered exception if all retries fail.
+
+    Raises:
+        Exception: The last exception encountered if the retry attempts exceed the specified limit.
+    """
+
+    def decorator_retry(func: F):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            nonlocal retries
+            last_exception = None
+            for attempt in range(retries + 1):
+                try:
+                    return func(*args, **kwargs)
+                except Exception as e:
+                    last_exception = e
+                    if attempt < retries:
+                        logger = Logger(func.__module__)
+                        left = retries - attempt - 1
+                        logger.warning(
+                            f"{func.__name__} failed, retrying: {e}, attempts left: {left}"
+                        )
+                        time.sleep(delay)
+                    else:
+                        logger.error(
+                            f"{func.__name__} retry attemps failed: {e}")
+                        break
+            raise last_exception
+        return wrapper
+    if _func is not None:
+        return decorator_retry(_func)
+    return decorator_retry
```

### Comparing `vulcan-logger-1.5.6/vulcan_logger/encoder.py` & `vulcan-logger-1.6.0/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.6/vulcan_logger/logger.py` & `vulcan-logger-1.6.0/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.5.6/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.6.0/vulcan_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.5.6
+Version: 1.6.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

