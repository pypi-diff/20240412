# Comparing `tmp/logflake-1.1.1.tar.gz` & `tmp/logflake-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logflake-1.1.1.tar", last modified: Fri Apr  5 15:23:49 2024, max compression
+gzip compressed data, was "logflake-1.2.0.tar", last modified: Fri Apr 12 10:06:03 2024, max compression
```

## Comparing `logflake-1.1.1.tar` & `logflake-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.206165 logflake-1.1.1/
--rw-r--r--   0 dedo1911   (501) staff       (20)     2422 2024-04-05 15:23:49.205986 logflake-1.1.1/PKG-INFO
--rw-r--r--   0 dedo1911   (501) staff       (20)     2038 2024-04-05 15:21:57.000000 logflake-1.1.1/README.md
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.205075 logflake-1.1.1/logflake/
--rw-r--r--   0 dedo1911   (501) staff       (20)        0 2024-02-05 16:12:08.000000 logflake-1.1.1/logflake/__init__.py
--rw-r--r--   0 dedo1911   (501) staff       (20)     6260 2024-04-05 15:23:32.000000 logflake-1.1.1/logflake/logflake.py
-drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-05 15:23:49.205768 logflake-1.1.1/logflake.egg-info/
--rw-r--r--   0 dedo1911   (501) staff       (20)     2422 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/PKG-INFO
--rw-r--r--   0 dedo1911   (501) staff       (20)      225 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/SOURCES.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)        1 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/dependency_links.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)       26 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/requires.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)        9 2024-04-05 15:23:49.000000 logflake-1.1.1/logflake.egg-info/top_level.txt
--rw-r--r--   0 dedo1911   (501) staff       (20)      500 2024-04-05 14:26:58.000000 logflake-1.1.1/pyproject.toml
--rw-r--r--   0 dedo1911   (501) staff       (20)       38 2024-04-05 15:23:49.206201 logflake-1.1.1/setup.cfg
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-12 10:06:03.040354 logflake-1.2.0/
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2452 2024-04-12 10:06:03.040181 logflake-1.2.0/PKG-INFO
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2046 2024-04-05 15:24:47.000000 logflake-1.2.0/README.md
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-12 10:06:03.039265 logflake-1.2.0/logflake/
+-rw-r--r--   0 dedo1911   (501) staff       (20)        0 2024-02-05 16:12:08.000000 logflake-1.2.0/logflake/__init__.py
+-rw-r--r--   0 dedo1911   (501) staff       (20)     6601 2024-04-12 10:04:03.000000 logflake-1.2.0/logflake/logflake.py
+drwxr-xr-x   0 dedo1911   (501) staff       (20)        0 2024-04-12 10:06:03.039958 logflake-1.2.0/logflake.egg-info/
+-rw-r--r--   0 dedo1911   (501) staff       (20)     2452 2024-04-12 10:06:03.000000 logflake-1.2.0/logflake.egg-info/PKG-INFO
+-rw-r--r--   0 dedo1911   (501) staff       (20)      225 2024-04-12 10:06:03.000000 logflake-1.2.0/logflake.egg-info/SOURCES.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)        1 2024-04-12 10:06:03.000000 logflake-1.2.0/logflake.egg-info/dependency_links.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)       33 2024-04-12 10:06:03.000000 logflake-1.2.0/logflake.egg-info/requires.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)        9 2024-04-12 10:06:03.000000 logflake-1.2.0/logflake.egg-info/top_level.txt
+-rw-r--r--   0 dedo1911   (501) staff       (20)      514 2024-04-12 10:05:29.000000 logflake-1.2.0/pyproject.toml
+-rw-r--r--   0 dedo1911   (501) staff       (20)       38 2024-04-12 10:06:03.040391 logflake-1.2.0/setup.cfg
```

### Comparing `logflake-1.1.1/PKG-INFO` & `logflake-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: logflake
-Version: 1.1.1
+Version: 1.2.0
 Summary: LogFlake Python Client
 Author-email: CloudPhoenix Srl <info@cloudphoenix.it>
 Project-URL: Homepage, https://github.com/CloudPhoenix/logflake-client-python
 Keywords: logflake
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: snappy
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">LogFlake Client Python</h1>
 
 > This repository contains the sources for the client-side components of the LogFlake product suite for applications logs and performance collection for Python applications.
 
@@ -32,15 +33,15 @@
 
 logger = logflake.LogFlake('application-key')
 logger.send_log(logflake.LogLevels.DEBUG, None, 'Hello World')
 
 logger.shutdown()
 ```
 
-### Use logging handler
+### Use logging handler example
 
 ```python
 LOGGING = {
     "version": 1,
     "formatters": {
         "logflake": {
             "()": "django.utils.log.ServerFormatter",
```

### Comparing `logflake-1.1.1/README.md` & `logflake-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 logger = logflake.LogFlake('application-key')
 logger.send_log(logflake.LogLevels.DEBUG, None, 'Hello World')
 
 logger.shutdown()
 ```
 
-### Use logging handler
+### Use logging handler example
 
 ```python
 LOGGING = {
     "version": 1,
     "formatters": {
         "logflake": {
             "()": "django.utils.log.ServerFormatter",
```

### Comparing `logflake-1.1.1/logflake/logflake.py` & `logflake-1.2.0/logflake/logflake.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 import os
 import threading
+import snappy
+from base64 import b64encode
 from logging import Handler
 from json import dumps
 from enum import Enum
 from queue import Queue
 from sys import exc_info
 from traceback import format_exc
 from platform import node
@@ -75,14 +77,15 @@
         self.server = log_flake_server.rstrip('/')
         self._hostname = node()
         self.app_id = app_id
         self._logs_queue = Queue()
         self._process_logs = threading.Event()
         self.failed_post_retries = 3
         self.post_timeout_seconds = 3
+        self.enable_compression = True
         self.is_shutting_down = False
         self.show_greeting = show_greeting
         self._logs_processor_thread = threading.Thread(target=self._logs_processor)
         self._logs_processor_thread.start()
 
     def __del__(self):
         self.shutdown()
@@ -115,15 +118,20 @@
     def _post(self, queue_name, json_string):
         if queue_name not in (Queues.LOGS.value, Queues.PERFORMANCES.value):
             return False
 
         try:
             url = f"{self.server}/api/ingestion/{self.app_id}/{queue_name}"
             headers = {'Content-Type': 'application/json'}
-            response = post(url, data=json_string, headers=headers, timeout=self.post_timeout_seconds)
+            body = json_string
+            if self.enable_compression:
+                headers = {'Content-Type': 'application/octet-stream'}
+                encoded = b64encode(json_string.encode()).decode()
+                body = snappy.compress(encoded, "utf-8")
+            response = post(url, data=body, headers=headers, timeout=self.post_timeout_seconds)
             return response.status_code == 200
         except:
             return False
 
     def send_log(self, level, correlation, content, params=None):
         obj = LogObject(
             level=level.value,
```

### Comparing `logflake-1.1.1/logflake.egg-info/PKG-INFO` & `logflake-1.2.0/logflake.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: logflake
-Version: 1.1.1
+Version: 1.2.0
 Summary: LogFlake Python Client
 Author-email: CloudPhoenix Srl <info@cloudphoenix.it>
 Project-URL: Homepage, https://github.com/CloudPhoenix/logflake-client-python
 Keywords: logflake
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
+Requires-Dist: snappy
 Provides-Extra: dev
 Requires-Dist: pip-tools; extra == "dev"
 
 <h1 align="center">LogFlake Client Python</h1>
 
 > This repository contains the sources for the client-side components of the LogFlake product suite for applications logs and performance collection for Python applications.
 
@@ -32,15 +33,15 @@
 
 logger = logflake.LogFlake('application-key')
 logger.send_log(logflake.LogLevels.DEBUG, None, 'Hello World')
 
 logger.shutdown()
 ```
 
-### Use logging handler
+### Use logging handler example
 
 ```python
 LOGGING = {
     "version": 1,
     "formatters": {
         "logflake": {
             "()": "django.utils.log.ServerFormatter",
```

