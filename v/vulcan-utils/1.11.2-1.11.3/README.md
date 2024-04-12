# Comparing `tmp/vulcan_utils-1.11.2.tar.gz` & `tmp/vulcan_utils-1.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.2.tar", last modified: Fri Apr 12 18:19:22 2024, max compression
+gzip compressed data, was "vulcan_utils-1.11.3.tar", last modified: Fri Apr 12 19:17:07 2024, max compression
```

## Comparing `vulcan_utils-1.11.2.tar` & `vulcan_utils-1.11.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:19:22.032607 vulcan_utils-1.11.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 18:19:22.032607 vulcan_utils-1.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:19:22.032607 vulcan_utils-1.11.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:19:22.028607 vulcan_utils-1.11.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:19:22.032607 vulcan_utils-1.11.2/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8117 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 18:19:13.000000 vulcan_utils-1.11.2/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:19:22.032607 vulcan_utils-1.11.2/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 18:19:21.000000 vulcan_utils-1.11.2/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 18:19:22.000000 vulcan_utils-1.11.2/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:19:21.000000 vulcan_utils-1.11.2/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 18:19:21.000000 vulcan_utils-1.11.2/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:19:21.000000 vulcan_utils-1.11.2/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.871774 vulcan_utils-1.11.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.871774 vulcan_utils-1.11.3/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11.2/LICENSE` & `vulcan_utils-1.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/PKG-INFO` & `vulcan_utils-1.11.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.2
-Summary: A utility package Python
+Version: 1.11.3
+Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Utils
 Vulcan Utils is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan_utils-1.11.2/tests/test_decorator.py` & `vulcan_utils-1.11.3/tests/test_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from datetime import datetime
 from typing import List
 from unittest.mock import patch
 
 import pytest
 
-from vulcan_utils.decorator import log, rate_limit, retry, to_json
+from vulcan_utils.decorator import Decorator as decorator
 from vulcan_utils.encoder import Encoder
 
 
 def _sample_function(x: int, y: int = 2) -> int:
     """
     Simple function that adds two integers.
 
@@ -70,92 +70,92 @@
     This verifies that the decorator appends execution time information to the log.
 
     Args:
         delay (float): Simulated function execution delay to test timing accuracy.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = log(_slow_function)
+        decorated = decorator.log(_slow_function)
         decorated(delay)
         last_call_args = mock_logger.return_value.debug.call_args_list[-1][0][0]
         assert "milliseconds" in last_call_args
 
 
 def test_log_decorator_basic() -> None:
     """
     Tests the basic functionality of the log decorator to ensure it logs function calls,
     returns, and execution times correctly and returns the expected function results.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = log(_sample_function)
+        decorated = decorator.log(_sample_function)
         result = decorated(1, y=3)
         assert result == 4
         assert mock_logger.return_value.debug.call_count == 3
 
 
 def test_log_decorator_condition_false() -> None:
     """
     Tests the log decorator when the logging condition is set to False.
     Ensures that no logging occurs when the condition evaluates to False but the function
     still executes and returns correctly.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = log(_sample_function, condition=False)
+        decorated = decorator.log(_sample_function, condition=False)
         result = decorated(1, y=3)
         assert result == 4
         mock_logger.return_value.debug.assert_not_called()
 
 
 def test_log_decorator_log_level() -> None:
     """
     Tests the log decorator's ability to log at a specified level.
     This test ensures that the decorator respects the 'level' parameter and logs at the correct severity.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = log(_sample_function, level="INFO")
+        decorated = decorator.log(_sample_function, level="INFO")
         decorated(1, 2)
         assert mock_logger.return_value.info.call_count == 3
 
 
 def test_retry_success() -> None:
     """
     Verifies that the retry decorator retries the correct number of times and then successfully returns
     the result of the function when it finally succeeds.
     """
 
     attempts = [0]
-    decorated = retry(_failing_function, retries=2, delay=0.1)
+    decorated = decorator.retry(_failing_function, retries=2, delay=0.1)
     result = decorated(attempts=attempts, max_attempts=2)
     assert result == "Success"
     assert attempts[0] == 2
 
 
 def test_retry_fail() -> None:
     """
     Ensures that the retry decorator properly raises the last encountered exception after all retries are exhausted.
     """
 
     attempts = [0]
-    decorated = retry(_failing_function, retries=1, delay=0.1)
+    decorated = decorator.retry(_failing_function, retries=1, delay=0.1)
     with pytest.raises(ValueError):
         decorated(attempts=attempts, max_attempts=3)
     assert attempts[0] == 2
 
 
 @pytest.mark.parametrize("attempts_list, max_attempts", [([0], 2), ([0], 3)])
 def test_retry_logging(attempts_list, max_attempts) -> None:
     """
     Tests that logging occurs as expected during retries and at failure.
     """
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
-        decorated = retry(
+        decorated = decorator.retry(
             _failing_function,
             retries=max_attempts - 1, delay=0.1
         )
         try:
             decorated(attempts=attempts_list, max_attempts=max_attempts)
         except ValueError:
             pass
@@ -167,23 +167,23 @@
 
 def test_to_json():
     """
     Test the to_json decorator to ensure it correctly serializes the return value of a function to a JSON string using
     a custom encoder. The function will return a dictionary which should be serialized into a JSON string.
     """
 
-    @to_json
+    @decorator.to_json
     def sample_function():
         return {"name": "Alice", "age": 30, "time": datetime(2020, 5, 17)}
     result = sample_function()
     expected_json = json.dumps(
         {"name": "Alice", "age": 30, "time": "2020-05-17T00:00:00"}, cls=Encoder)
     assert result == expected_json, "The JSON output from the decorated function did not match the expected JSON string."
 
-    @to_json
+    @decorator.to_json
     def complex_data_function():
         return {"date": datetime.now(), "data": [1, 2, 3]}
     try:
         json_result = complex_data_function()
         # this will confirm json_result is a valid JSON string
         json.loads(json_result)
         assert True, "Serialization of complex data types was successful."
@@ -203,30 +203,30 @@
 
     Args:
         num_calls (int): Number of times to call the decorated function.
         sleep_time (float): Time to sleep between each call, in seconds.
         expected_errors (int): Number of times the rate limit should trigger and log an error.
     """
 
-    @rate_limit(limit=50, interval=10)
+    @decorator.rate_limit(limit=50, interval=10)
     def test_function():
         return
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
         for _ in range(num_calls):
             test_function()
             time.sleep(sleep_time)
         assert mock_logger.return_value.error.call_count == expected_errors
 
 
 def test_rate_limit_reset():
     """
     Test that the rate limit properly resets after the cooldown interval.
     """
-    @rate_limit(limit=5, interval=1)  # Very short interval for test speed
+    @decorator.rate_limit(limit=5, interval=1)  # Very short interval for test speed
     def test_function():
         return
 
     with patch('vulcan_utils.decorator.Logger') as mock_logger:
         for _ in range(5):
             test_function()  # These should all pass
         time.sleep(1.1)      # Wait for the interval to pass
```

### Comparing `vulcan_utils-1.11.2/tests/test_encoder.py` & `vulcan_utils-1.11.3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/tests/test_formatter.py` & `vulcan_utils-1.11.3/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/tests/test_logger.py` & `vulcan_utils-1.11.3/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/tests/test_printable.py` & `vulcan_utils-1.11.3/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/vulcan_utils/decorator.py` & `vulcan_utils-1.11.3/vulcan_utils/decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,214 +7,230 @@
 from .encoder import Encoder
 from .logger import Logger
 
 # TypeVar for decorator type preservation
 F = TypeVar('F', bound=Callable[..., Any])
 
 
-def _call_message(func: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
+class Decorator:
     """
-    Constructs a log message string for function calls, including function name,
-    positional arguments, and keyword arguments.
-
-    Args:
-        func: The function being called.
-        *args: Positional arguments passed to the function.
-        **kwargs: Keyword arguments passed to the function.
-
-    Returns:
-        A formatted log message string.
-    """
-
-    log_message_parts = [f"{func.__name__} call:"]
-    if args:
-        log_message_parts.append(f"args:{args}")
-    if kwargs:
-        log_message_parts.append(f"kwargs:{kwargs}")
-    return ' '.join(log_message_parts)
-
-
-def _return_message(func: Callable[..., Any], result: Any) -> str:
-    """
-    Constructs a log message string for function returns, including function name and the serialized return value.
-
-    Args:
-        func: The function that returned a value.
-        result: The return value of the function.
-
-    Returns:
-        A formatted log message string with the serialized return value.
-    """
-
-    json_result = json.dumps(result, cls=Encoder, ensure_ascii=False)
-    return f"{func.__name__} return: {json_result} {type(result)}"
-
-
-def _log_func(logger: Logger, level: str) -> Callable[[str], None]:
-    """
-    Retrieves the appropriate logging function based on the specified log level.
-
-    Args:
-        logger: An instance of Logger.
-        level: A string representing the logging level.
-
-    Returns:
-        A logging function from the Logger instance.
-    """
-
-    levels = {
-        "DEBUG": logger.debug,
-        "INFO": logger.info,
-        "WARNING": logger.warning,
-        "CRITICAL": logger.critical,
-        "ERROR": logger.error,
-    }
-    return levels.get(level.upper(), logger.debug)
-
-
-def log(_func: Optional[F] = None, *, condition: bool = True, level: str = "DEBUG") -> Union[Callable[[F], F], F]:
-    """
-    A decorator that logs the call and return of functions, including execution time. Optionally, logging can be
-    conditioned on a boolean expression.
-
-    Args:
-        _func: The function to be decorated. Defaults to None, allowing other parameters to be specified first.
-        condition: A boolean flag to determine if logging should occur. Defaults to True.
-        level: A string indicating the logging level. Defaults to "DEBUG".
-
-    Returns:
-        The decorated function, with logging capabilities added.
-    """
-
-    def decorator_log(func: F):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            result = None
-            if condition:
-                start_time = time.time()
-                logger = Logger(func.__module__)
-                log_func = _log_func(logger, level)
-                log_func(_call_message(func, *args, **kwargs))
-                result = func(*args, **kwargs)
-                log_func(_return_message(func, result))
-                end_time = time.time()
-                execution_time_ms = round(
-                    (end_time - start_time) * 1000,
-                    ndigits=4
-                )
-                log_func(
-                    f"{func.__name__} executed: {execution_time_ms} milliseconds")
-            else:
-                result = func(*args, **kwargs)
-            return result
-        return wrapper
-    if _func is None:
-        return decorator_log
-    else:
-        return decorator_log(_func)
-
-
-def retry(_func: Optional[F] = None, *, retries: int = 3, delay: Union[int, float] = 1, infinite: bool = False) -> Union[Callable[[F], F], F]:
-    """
-    Decorator to retry a function if it raises an exception. Optionally retries the function indefinitely if
-    the 'infinite' parameter is True. If not, it retries a specified number of times with a given delay between each attempt.
-    If all finite attempts fail, the last exception is raised.
-
-    Args:
-        _func: The function to be decorated. Defaults to None, allowing other parameters to be specified first.
-        retries: The maximum number of retries before giving up and raising the exception if not infinite.
-        delay: The delay between retries in seconds, which can be an integer or a float for partial seconds.
-        infinite: If True, the function will retry indefinitely. Defaults to False.
-
-    Returns:
-        The decorated function that will retry on exceptions, or raises the last encountered exception if all retries fail and not infinite.
-
-    Raises:
-        Exception: The last exception encountered if the retry attempts exceed the specified limit and not infinite.
-    """
-
-    def decorator_retry(func: F):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            attempt = 0
-            while True:
-                try:
-                    return func(*args, **kwargs)
-                except Exception as e:
-                    logger = Logger(__name__)
-                    if infinite:
-                        logger.warning(
-                            f"{func.__name__} failed, retrying indefinitely: {e}"
-                        )
-                        time.sleep(delay)
-                    else:
-                        if attempt < retries:
+    A collection of decorators designed to enhance function capabilities with additional behaviors such as logging,
+    retrying on exceptions, converting return values to JSON, and rate-limiting function calls.his class primarily 
+    serves as a namespace for decorator methods.
+
+    This class implements static and class methods to provide utility functions that can be applied to other functions
+    to log details about their calls and results, retry execution on failures, serialize outputs to JSON, and limit
+    the rate of function execution. T
+
+    Methods:
+        log: Decorates a function to log its call and return details, including execution time.
+        retry: Decorates a function to retry execution a specified number of times upon failure.
+        to_json: Decorates a function to serialize its return value to a JSON string using a custom encoder.
+        rate_limit: Decorates a function to limit its call rate to a specified threshold over a given time interval.
+    """
+
+    @staticmethod
+    def _call_message(func: Callable[..., Any], *args: Any, **kwargs: Any) -> str:
+        """
+        Constructs a log message string for function calls, including function name,
+        positional arguments, and keyword arguments.
+
+        Args:
+            func (Callable[..., Any]): The function being called.
+            *args (Any): Positional arguments passed to the function.
+            **kwargs (Any): Keyword arguments passed to the function.
+
+        Returns:
+            A formatted log message string.
+        """
+
+        log_message_parts = [f"{func.__name__} call:"]
+        if args:
+            log_message_parts.append(f"args:{args}")
+        if kwargs:
+            log_message_parts.append(f"kwargs:{kwargs}")
+        return ' '.join(log_message_parts)
+
+    @staticmethod
+    def _return_message(func: Callable[..., Any], result: Any) -> str:
+        """
+        Constructs a log message string for function returns, including function name and the serialized return value.
+
+        Args:
+            func (Callable[..., Any]): The function that returned a value.
+            result (Any): The return value of the function.
+
+        Returns:
+            A formatted log message string with the serialized return value.
+        """
+
+        json_result = json.dumps(result, cls=Encoder, ensure_ascii=False)
+        return f"{func.__name__} return: {json_result} {type(result)}"
+
+    @staticmethod
+    def _log_func(logger: Logger, level: str) -> Callable[[str], None]:
+        """
+        Retrieves the appropriate logging function based on the specified log level.
+
+        Args:
+            logger (logger.Logger): An instance of Logger configured for logging messages.
+            level (str): A string representing the logging level.
+
+        Returns:
+            A logging function from the Logger instance corresponding to the specified level.
+        """
+
+        levels = {
+            "DEBUG": logger.debug,
+            "INFO": logger.info,
+            "WARNING": logger.warning,
+            "CRITICAL": logger.critical,
+            "ERROR": logger.error,
+        }
+        return levels.get(level.upper(), logger.debug)
+
+    @classmethod
+    def log(cls, _func: Optional[F] = None, *, condition: bool = True, level: str = "DEBUG") -> Union[Callable[[F], F], F]:
+        """
+        A decorator that logs the call and return of functions, including execution time.
+        Logging can be conditioned on a boolean expression.
+
+        Args:
+            _func (Callable[..., Any]): The function to be decorated. If None, other parameters are allowed to be specified first.
+            condition (bool): A boolean flag to determine if logging should occur, defaults to True.
+            level (str): A string indicating the logging level, defaults to "DEBUG".
+
+        Returns:
+            The decorated function with logging capabilities added.
+        """
+
+        def decorator_log(func: F):
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                result = None
+                if condition:
+                    start_time = time.time()
+                    logger = Logger(func.__module__)
+                    log_func = cls._log_func(logger, level)
+                    log_func(cls._call_message(func, *args, **kwargs))
+                    result = func(*args, **kwargs)
+                    log_func(cls._return_message(func, result))
+                    end_time = time.time()
+                    execution_time_ms = round(
+                        (end_time - start_time) * 1000,
+                        ndigits=4
+                    )
+                    log_func(
+                        f"{func.__name__} executed: {execution_time_ms} milliseconds")
+                else:
+                    result = func(*args, **kwargs)
+                return result
+            return wrapper
+        if _func is None:
+            return decorator_log
+        else:
+            return decorator_log(_func)
+
+    @classmethod
+    def retry(cls, _func: Optional[F] = None, *, retries: int = 3, delay: Union[int, float] = 1, infinite: bool = False) -> Union[Callable[[F], F], F]:
+        """
+        Decorator to retry a function if it raises an exception. Optionally retries the function indefinitely if
+        'infinite' is True. If not, it retries a specified number of times with a given delay between each attempt.
+
+        Args:
+            _func (Callable[..., Any]): The function to be decorated. If None, other parameters can be specified first.
+            retries (int): The maximum number of retries before giving up and raising the exception if not infinite.
+            delay (Union[int, float]): The delay between retries in seconds, can be an integer or a float for partial seconds.
+            infinite (bool): If True, the function will retry indefinitely, defaults to False.
+
+        Returns:
+            The decorated function that will retry on exceptions, or raises the last encountered exception if all retries fail and not infinite.
+
+        Raises:
+            Exception: The last exception encountered if the retry attempts exceed the specified limit and not infinite.
+        """
+
+        def decorator_retry(func: F):
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                attempt = 0
+                while True:
+                    try:
+                        return func(*args, **kwargs)
+                    except Exception as e:
+                        logger = Logger(__name__)
+                        if infinite:
                             logger.warning(
-                                f"{func.__name__} failed, retrying: {e}, attempts left: {retries - attempt - 1}")
+                                f"{func.__name__} failed, retrying indefinitely: {e}"
+                            )
                             time.sleep(delay)
-                            attempt += 1
                         else:
-                            logger.error(
-                                f"{func.__name__} retry attempts failed: {e}")
-                            raise e
-        return wrapper
-    if _func is not None:
-        return decorator_retry(_func)
-    return decorator_retry
-
-
-def to_json(_func: Union[Callable[[F], F], F] = None) -> Union[Callable[[F], F], F]:
-    """
-    A decorator that serializes the return value of the decorated function to JSON.
-    This uses a custom JSON encoder to handle complex data types not typically serializable by the default JSON encoder.
-
-    Args:
-        _func (Callable[[F], F], optional): The function to decorate. If None, this allows other parameters to be 
-            passed first as keyword arguments. Defaults to None.
-
-    Returns:
-        Callable[[F], F]: The decorated function with its return value serialized as a JSON string.
-    """
-
-    def decorator_to_json(func: F) -> F:
-        @wraps(func)
-        def wrapper(*args, **kwargs) -> str:
-            result = func(*args, **kwargs)
-            return json.dumps(result, cls=Encoder, ensure_ascii=False)
-        return wrapper
-    if _func is not None:
-        return decorator_to_json(_func)
-    return decorator_to_json
-
-
-def rate_limit(limit: int, interval: float):
-    """
-    Decorator to rate limit the execution of a function. Allows a burst of 'limit' calls,
-    and then enforces a cooldown period of 'interval' seconds before allowing another burst.
-
-    Args:
-        limit (int): Maximum number of calls allowed within the burst.
-        interval (float): Cooldown interval (in seconds) after a burst before resetting the limit.
-    """
-
-    def decorator(func):
-        call_times = []
-        first_call_time = None
-
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            nonlocal first_call_time
-            now = time.time()
-            if first_call_time and now - first_call_time > interval:
-                call_times.clear()
-                first_call_time = None
-            if not first_call_time:
-                first_call_time = now
-            if len(call_times) < limit:
-                call_times.append(now)
-                return func(*args, **kwargs)
-            else:
-                logger = Logger(func.__module__)
-                logger.error(f"Rate limit exceeded for {func.__name__}")
-                return
-        return wrapper
-    return decorator
+                            if attempt < retries:
+                                logger.warning(
+                                    f"{func.__name__} failed, retrying: {e}, attempts left: {retries - attempt - 1}")
+                                time.sleep(delay)
+                                attempt += 1
+                            else:
+                                logger.error(
+                                    f"{func.__name__} retry attempts failed: {e}")
+                                raise e
+            return wrapper
+        if _func is not None:
+            return decorator_retry(_func)
+        return decorator_retry
+
+    @classmethod
+    def to_json(cls, _func: Union[Callable[[F], F], F] = None) -> Union[Callable[[F], F], F]:
+        """
+        A decorator that serializes the return value of the decorated function to JSON using a custom encoder.
+
+        Args:
+            _func (Optional[Callable[[F], F]]): The function to decorate. If None, allows other parameters to be 
+                specified first as keyword arguments.
+
+        Returns:
+            Callable[[F], F]: The decorated function with its return value serialized as a JSON string.
+        """
+
+        def decorator_to_json(func: F) -> F:
+            @wraps(func)
+            def wrapper(*args, **kwargs) -> str:
+                result = func(*args, **kwargs)
+                return json.dumps(result, cls=Encoder, ensure_ascii=False)
+            return wrapper
+        if _func is not None:
+            return decorator_to_json(_func)
+        return decorator_to_json
+
+    @classmethod
+    def rate_limit(cls, limit: int, interval: float):
+        """
+        Decorator to rate limit the execution of a function. Allows a burst of 'limit' calls,
+        and then enforces a cooldown period of 'interval' seconds before allowing another burst.
+
+        Args:
+            limit (int): Maximum number of calls allowed within the burst.
+            interval (float): Cooldown interval (in seconds) after a burst before resetting the limit.
+        """
+
+        def decorator(func):
+            call_times = []
+            first_call_time = None
+
+            @wraps(func)
+            def wrapper(*args, **kwargs):
+                nonlocal first_call_time
+                now = time.time()
+                if first_call_time and now - first_call_time > interval:
+                    call_times.clear()
+                    first_call_time = None
+                if not first_call_time:
+                    first_call_time = now
+                if len(call_times) < limit:
+                    call_times.append(now)
+                    return func(*args, **kwargs)
+                else:
+                    logger = Logger(func.__module__)
+                    logger.error(f"Rate limit exceeded for {func.__name__}")
+                    return
+            return wrapper
+        return decorator
```

### Comparing `vulcan_utils-1.11.2/vulcan_utils/encoder.py` & `vulcan_utils-1.11.3/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/vulcan_utils/formatter.py` & `vulcan_utils-1.11.3/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/vulcan_utils/logger.py` & `vulcan_utils-1.11.3/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/vulcan_utils/printable.py` & `vulcan_utils-1.11.3/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.2/vulcan_utils.egg-info/PKG-INFO` & `vulcan_utils-1.11.3/vulcan_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.2
-Summary: A utility package Python
+Version: 1.11.3
+Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Utils
 Vulcan Utils is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

