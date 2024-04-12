# Comparing `tmp/safe_init-1.0.1.tar.gz` & `tmp/safe_init-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_init-1.0.1.tar", max compression
+gzip compressed data, was "safe_init-1.0.2.tar", max compression
```

## Comparing `safe_init-1.0.1.tar` & `safe_init-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2024-04-11 09:07:19.830757 safe_init-1.0.1/LICENSE
--rw-r--r--   0        0        0    11999 2024-04-11 09:07:19.830757 safe_init-1.0.1/README.md
--rw-r--r--   0        0        0     3205 2024-04-11 09:07:19.834757 safe_init-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      736 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/__init__.py
--rw-r--r--   0        0        0     7429 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/decorator.py
--rw-r--r--   0        0        0     4240 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/dlq.py
--rw-r--r--   0        0        0      751 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/errors.py
--rw-r--r--   0        0        0     5422 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/handler.py
--rw-r--r--   0        0        0        0 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/py.typed
--rw-r--r--   0        0        0     3909 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/safe_logging.py
--rw-r--r--   0        0        0     1339 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/sentry.py
--rw-r--r--   0        0        0     5621 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/slack.py
--rw-r--r--   0        0        0     5895 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/timeout.py
--rw-r--r--   0        0        0     3918 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/tracer.py
--rw-r--r--   0        0        0     3237 2024-04-11 09:07:19.834757 safe_init-1.0.1/safe_init/utils.py
--rw-r--r--   0        0        0    13484 1970-01-01 00:00:00.000000 safe_init-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-12 09:41:11.874812 safe_init-1.0.2/LICENSE
+-rw-r--r--   0        0        0    12409 2024-04-12 09:41:11.878812 safe_init-1.0.2/README.md
+-rw-r--r--   0        0        0     3205 2024-04-12 09:41:11.890812 safe_init-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      736 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/__init__.py
+-rw-r--r--   0        0        0     7429 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/decorator.py
+-rw-r--r--   0        0        0     4240 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/dlq.py
+-rw-r--r--   0        0        0      751 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/errors.py
+-rw-r--r--   0        0        0     5456 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/handler.py
+-rw-r--r--   0        0        0        0 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/py.typed
+-rw-r--r--   0        0        0     3909 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/safe_logging.py
+-rw-r--r--   0        0        0     2551 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/sentry.py
+-rw-r--r--   0        0        0     5621 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/slack.py
+-rw-r--r--   0        0        0     6334 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/timeout.py
+-rw-r--r--   0        0        0     3918 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/tracer.py
+-rw-r--r--   0        0        0     3237 2024-04-12 09:41:11.890812 safe_init-1.0.2/safe_init/utils.py
+-rw-r--r--   0        0        0    13894 1970-01-01 00:00:00.000000 safe_init-1.0.2/PKG-INFO
```

### Comparing `safe_init-1.0.1/LICENSE` & `safe_init-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/README.md` & `safe_init-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,26 @@
 
 [Read the Docs](https://safe-init.readthedocs.io/en/latest/) | [GitHub Repository](https://github.com/Kalepa/safe-init) | [PyPI Package](https://pypi.org/project/safe-init/) 
 
 ## Features
 
 ### Error Handling and Logging
 - **Error Handling**: Safe Init wraps your Lambda handler with robust error handling and logging, ensuring that any unhandled exceptions are captured and logged for easy debugging.
+
+![Uncaught exception Slack notification](https://github.com/Kalepa/safe-init/blob/main/docs/static/uncaught_exception.png?raw=true)
+
 - **Execution Time Tracing**: Traces the execution time of all function calls within the Lambda handler, helping you identify performance bottlenecks and optimize your code.
 
+![Timeout Slack notification with traces](https://github.com/Kalepa/safe-init/blob/main/docs/static/traced_timeout.png?raw=true)
+
 ### Monitoring and Alerting
 - **Sentry Integration**: Automatically captures and logs exceptions with Sentry, providing detailed error tracking and monitoring capabilities.
+
+![Execution with missing Sentry init Slack notification](https://github.com/Kalepa/safe-init/blob/main/docs/static/missing_sentry.png?raw=true)
+
 - **Slack Notifications**: Sends informative Slack notifications with error details, keeping your team informed about any issues in real-time.
 - **Datadog Integration**: Integrates seamlessly with the Datadog Lambda wrapper for enhanced monitoring and metrics collection.
 
 ### Resilience and Reliability
 - **Dead-Letter Queue (DLQ) Support**: Pushes failed events to a dead-letter queue for later processing, ensuring that no events are lost due to errors.
 - **Initialization Checks**: Detects missing Sentry initialization and Lambda init phase timeouts, preventing silent failures and providing early warning signs.
 - **Timeout Notifications**: Sends notifications a configurable number of seconds before the Lambda timeout occurs, giving you a heads-up to investigate and address potential issues.
```

### Comparing `safe_init-1.0.1/pyproject.toml` & `safe_init-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-init"
-version = "1.0.1"
+version = "1.0.2"
 description = "Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications."
 license = "MIT"
 authors = ["Maciej Wilczyński <maciej@lupine.software>"]
 repository = "https://github.com/kalepa/safe-init"
 readme = "README.md"
 packages = [{ include = "safe_init" }]
 include = ["safe_init/py.typed"]
```

### Comparing `safe_init-1.0.1/safe_init/__init__.py` & `safe_init-1.0.2/safe_init/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-__VERSION__ = "1.0.1"
+__VERSION__ = "1.0.2"
 
 _wrapped_handler = None
 
 
 class LazyHandler:
     @staticmethod
     def _init_handler() -> None:
```

### Comparing `safe_init-1.0.1/safe_init/decorator.py` & `safe_init-1.0.2/safe_init/decorator.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/dlq.py` & `safe_init-1.0.2/safe_init/dlq.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/errors.py` & `safe_init-1.0.2/safe_init/errors.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/handler.py` & `safe_init-1.0.2/safe_init/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
                 SafeInitMissingSentryWarning(msg),
                 handler_name=target_handler,
                 message_title="Sentry detector warning",
             )
 
         return exec_result  # noqa: TRY300
     except Exception as e:
-        sentry_result = sentry_capture(e)
+        sentry_result = sentry_capture(e, tags={"handler": target_handler})
         msg = (
             "Failed to import handler"
             if isinstance(e, ImportError)
             else "Unexpected error during handler initialization"
         )
         log_exception(msg, sentry_capture_result=sentry_result)
         slack_notify(msg, e, handler_name=target_handler, sentry_capture_result=sentry_result)
```

### Comparing `safe_init-1.0.1/safe_init/safe_logging.py` & `safe_init-1.0.2/safe_init/safe_logging.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/slack.py` & `safe_init-1.0.2/safe_init/slack.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/timeout.py` & `safe_init-1.0.2/safe_init/timeout.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,28 +113,40 @@
                 log_debug("Tracer is active")
                 fn_calls = tracer.get_function_calls()
                 aggregated_calls = aggregate_traced_fn_calls(fn_calls)
                 log_debug("Got aggregated calls", aggregated_calls=aggregated_calls)
                 calls_by_time = sorted(aggregated_calls, key=lambda x: x[2], reverse=True)
                 log_debug("Sorted calls by time", calls_by_time=calls_by_time)
 
+        additional_log_data: dict[str, Any] = {}
+        if include_lambda_data:
+            additional_log_data["lambda_name"] = os.environ.get(
+                "AWS_LAMBDA_FUNCTION_NAME",
+                self.call_args[1].function_name,
+            )
+
         exc = SafeInitTimeoutWarning(self.timeout_message)
         exc.traces = calls_by_time
 
-        sentry_result = sentry_capture(exc, fingerprint=self.execution_fingerprint)
+        sentry_result = sentry_capture(
+            exc,
+            fingerprint=self.execution_fingerprint,
+            tags={
+                "is_timeout": "true",
+                "timeout_value_seconds": str(self.waiting_time),
+                "is_lambda": "true" if include_lambda_data else "false",
+                "has_dlq": "true" if context_has_dlq() else "false",
+                **additional_log_data,
+            },
+            attachments={"longest_calls": calls_by_time} if calls_by_time else None,
+        )
         log_debug("Sentry capture result", sentry_capture_result=sentry_result)
 
-        additional_log_data: dict[str, Any] = {}
         if calls_by_time:
             additional_log_data["longest_calls"] = calls_by_time[:40]
-        if include_lambda_data:
-            additional_log_data["lambda_name"] = os.environ.get(
-                "AWS_LAMBDA_FUNCTION_NAME",
-                self.call_args[1].function_name,
-            )
 
         log_error(
             self.timeout_message,
             sentry_capture_result=sentry_result,
             exc_info=exc,
             **additional_log_data,
         )
```

### Comparing `safe_init-1.0.1/safe_init/tracer.py` & `safe_init-1.0.2/safe_init/tracer.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/safe_init/utils.py` & `safe_init-1.0.2/safe_init/utils.py`

 * *Files identical despite different names*

### Comparing `safe_init-1.0.1/PKG-INFO` & `safe_init-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-init
-Version: 1.0.1
+Version: 1.0.2
 Summary: Safe Init is a Python library that enhances AWS Lambda functions with advanced error handling, logging, monitoring, and resilience features, providing comprehensive observability and reliability for serverless applications.
 Home-page: https://github.com/kalepa/safe-init
 License: MIT
 Author: Maciej Wilczyński
 Author-email: maciej@lupine.software
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,18 +42,26 @@
 
 [Read the Docs](https://safe-init.readthedocs.io/en/latest/) | [GitHub Repository](https://github.com/Kalepa/safe-init) | [PyPI Package](https://pypi.org/project/safe-init/) 
 
 ## Features
 
 ### Error Handling and Logging
 - **Error Handling**: Safe Init wraps your Lambda handler with robust error handling and logging, ensuring that any unhandled exceptions are captured and logged for easy debugging.
+
+![Uncaught exception Slack notification](https://github.com/Kalepa/safe-init/blob/main/docs/static/uncaught_exception.png?raw=true)
+
 - **Execution Time Tracing**: Traces the execution time of all function calls within the Lambda handler, helping you identify performance bottlenecks and optimize your code.
 
+![Timeout Slack notification with traces](https://github.com/Kalepa/safe-init/blob/main/docs/static/traced_timeout.png?raw=true)
+
 ### Monitoring and Alerting
 - **Sentry Integration**: Automatically captures and logs exceptions with Sentry, providing detailed error tracking and monitoring capabilities.
+
+![Execution with missing Sentry init Slack notification](https://github.com/Kalepa/safe-init/blob/main/docs/static/missing_sentry.png?raw=true)
+
 - **Slack Notifications**: Sends informative Slack notifications with error details, keeping your team informed about any issues in real-time.
 - **Datadog Integration**: Integrates seamlessly with the Datadog Lambda wrapper for enhanced monitoring and metrics collection.
 
 ### Resilience and Reliability
 - **Dead-Letter Queue (DLQ) Support**: Pushes failed events to a dead-letter queue for later processing, ensuring that no events are lost due to errors.
 - **Initialization Checks**: Detects missing Sentry initialization and Lambda init phase timeouts, preventing silent failures and providing early warning signs.
 - **Timeout Notifications**: Sends notifications a configurable number of seconds before the Lambda timeout occurs, giving you a heads-up to investigate and address potential issues.
```

