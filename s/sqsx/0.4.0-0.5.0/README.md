# Comparing `tmp/sqsx-0.4.0.tar.gz` & `tmp/sqsx-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqsx-0.4.0.tar", last modified: Fri Feb 23 11:06:46 2024, max compression
+gzip compressed data, was "sqsx-0.5.tar", last modified: Fri Apr 12 21:28:25 2024, max compression
```

## Comparing `sqsx-0.4.0.tar` & `sqsx-0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-02-23 11:06:46.418371 sqsx-0.4.0/
--rw-r--r--   0 allisson   (501) staff       (20)     1073 2024-02-23 10:48:45.000000 sqsx-0.4.0/LICENSE
--rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-02-23 11:06:46.418144 sqsx-0.4.0/PKG-INFO
--rw-r--r--   0 allisson   (501) staff       (20)     6844 2024-02-23 10:48:45.000000 sqsx-0.4.0/README.md
--rw-r--r--   0 allisson   (501) staff       (20)      598 2024-02-23 11:03:00.000000 sqsx-0.4.0/pyproject.toml
--rw-r--r--   0 allisson   (501) staff       (20)       38 2024-02-23 11:06:46.418423 sqsx-0.4.0/setup.cfg
--rw-r--r--   0 allisson   (501) staff       (20)     1091 2024-02-23 11:03:50.000000 sqsx-0.4.0/setup.py
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-02-23 11:06:46.415576 sqsx-0.4.0/sqsx/
--rw-r--r--   0 allisson   (501) staff       (20)       47 2024-02-23 10:48:45.000000 sqsx-0.4.0/sqsx/__init__.py
--rw-r--r--   0 allisson   (501) staff       (20)      443 2024-02-23 10:48:45.000000 sqsx-0.4.0/sqsx/exceptions.py
--rw-r--r--   0 allisson   (501) staff       (20)      406 2024-02-23 10:48:45.000000 sqsx-0.4.0/sqsx/helper.py
--rw-r--r--   0 allisson   (501) staff       (20)     7354 2024-02-23 10:56:59.000000 sqsx-0.4.0/sqsx/queue.py
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-02-23 11:06:46.417826 sqsx-0.4.0/sqsx.egg-info/
--rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-02-23 11:06:46.000000 sqsx-0.4.0/sqsx.egg-info/PKG-INFO
--rw-r--r--   0 allisson   (501) staff       (20)      322 2024-02-23 11:06:46.000000 sqsx-0.4.0/sqsx.egg-info/SOURCES.txt
--rw-r--r--   0 allisson   (501) staff       (20)        1 2024-02-23 11:06:46.000000 sqsx-0.4.0/sqsx.egg-info/dependency_links.txt
--rw-r--r--   0 allisson   (501) staff       (20)       31 2024-02-23 11:06:46.000000 sqsx-0.4.0/sqsx.egg-info/requires.txt
--rw-r--r--   0 allisson   (501) staff       (20)       11 2024-02-23 11:06:46.000000 sqsx-0.4.0/sqsx.egg-info/top_level.txt
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-02-23 11:06:46.417250 sqsx-0.4.0/tests/
--rw-r--r--   0 allisson   (501) staff       (20)        0 2024-02-23 10:48:45.000000 sqsx-0.4.0/tests/__init__.py
--rw-r--r--   0 allisson   (501) staff       (20)     1941 2024-02-23 10:48:45.000000 sqsx-0.4.0/tests/conftest.py
--rw-r--r--   0 allisson   (501) staff       (20)      954 2024-02-23 10:48:45.000000 sqsx-0.4.0/tests/test_helper.py
--rw-r--r--   0 allisson   (501) staff       (20)     9437 2024-02-23 10:48:45.000000 sqsx-0.4.0/tests/test_queue.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.903609 sqsx-0.5/
+-rw-r--r--   0 allisson   (501) staff       (20)     1073 2024-02-23 10:48:45.000000 sqsx-0.5/LICENSE
+-rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-12 21:28:25.903378 sqsx-0.5/PKG-INFO
+-rw-r--r--   0 allisson   (501) staff       (20)     6844 2024-02-23 10:48:45.000000 sqsx-0.5/README.md
+-rw-r--r--   0 allisson   (501) staff       (20)      598 2024-04-12 21:27:51.000000 sqsx-0.5/pyproject.toml
+-rw-r--r--   0 allisson   (501) staff       (20)       38 2024-04-12 21:28:25.903653 sqsx-0.5/setup.cfg
+-rw-r--r--   0 allisson   (501) staff       (20)     1091 2024-04-12 21:27:51.000000 sqsx-0.5/setup.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.901067 sqsx-0.5/sqsx/
+-rw-r--r--   0 allisson   (501) staff       (20)       47 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/__init__.py
+-rw-r--r--   0 allisson   (501) staff       (20)      443 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/exceptions.py
+-rw-r--r--   0 allisson   (501) staff       (20)      406 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/helper.py
+-rw-r--r--   0 allisson   (501) staff       (20)     7481 2024-04-12 21:27:51.000000 sqsx-0.5/sqsx/queue.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.903078 sqsx-0.5/sqsx.egg-info/
+-rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/PKG-INFO
+-rw-r--r--   0 allisson   (501) staff       (20)      322 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/SOURCES.txt
+-rw-r--r--   0 allisson   (501) staff       (20)        1 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/dependency_links.txt
+-rw-r--r--   0 allisson   (501) staff       (20)       31 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/requires.txt
+-rw-r--r--   0 allisson   (501) staff       (20)       11 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/top_level.txt
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.902331 sqsx-0.5/tests/
+-rw-r--r--   0 allisson   (501) staff       (20)        0 2024-02-23 10:48:45.000000 sqsx-0.5/tests/__init__.py
+-rw-r--r--   0 allisson   (501) staff       (20)     1941 2024-02-23 10:48:45.000000 sqsx-0.5/tests/conftest.py
+-rw-r--r--   0 allisson   (501) staff       (20)      954 2024-02-23 10:48:45.000000 sqsx-0.5/tests/test_helper.py
+-rw-r--r--   0 allisson   (501) staff       (20)     9485 2024-04-12 21:27:51.000000 sqsx-0.5/tests/test_queue.py
```

### Comparing `sqsx-0.4.0/LICENSE` & `sqsx-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqsx-0.4.0/PKG-INFO` & `sqsx-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqsx
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple task processor for Amazon SQS
 Home-page: https://github.com/allisson/pysqsx
 Author: Allisson Azevedo
 Author-email: allisson@gmail.com
 Keywords: aws,sqs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sqsx-0.4.0/README.md` & `sqsx-0.5/README.md`

 * *Files identical despite different names*

### Comparing `sqsx-0.4.0/pyproject.toml` & `sqsx-0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqsx"
-version = "0.3.1"
+version = "0.5.0"
 description = "A simple task processor for Amazon SQS"
 authors = ["Allisson Azevedo"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.33.13"
```

### Comparing `sqsx-0.4.0/setup.py` & `sqsx-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="sqsx",
-    version="0.4.0",
+    version="0.5.0",
     description="A simple task processor for Amazon SQS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allisson/pysqsx",
     author="Allisson Azevedo",
     author_email="allisson@gmail.com",
     classifiers=[
```

### Comparing `sqsx-0.4.0/sqsx/queue.py` & `sqsx-0.5/sqsx/queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 
 logger = logging.getLogger(__name__)
 queue_url_regex = r"(http|https)[:][\/]{2}[a-zA-Z0-9-_:.]+[\/][0-9]{12}[\/]{1}[a-zA-Z0-9-_]{0,80}"
 
 
 class BaseQueueMixin:
     def consume_messages(
-        self, max_messages: int = 1, max_threads: int = 1, wait_seconds: int = 10, run_forever: bool = True
+        self,
+        max_messages: int = 1,
+        max_threads: int = 1,
+        wait_seconds: int = 10,
+        polling_wait_seconds: int = 10,
+        run_forever: bool = True,
     ) -> None:
         logger.info(f"Starting consuming tasks, queue_url={self.url}")
         signal.signal(signal.SIGINT, self._exit_gracefully)
         signal.signal(signal.SIGTERM, self._exit_gracefully)
 
         while True:
             if self._should_consume_tasks_stop:
@@ -27,14 +32,15 @@
                 break
 
             response = self.sqs_client.receive_message(
                 QueueUrl=self.url,
                 AttributeNames=["All"],
                 MaxNumberOfMessages=min(max_messages, 10),
                 MessageAttributeNames=["All"],
+                WaitTimeSeconds=polling_wait_seconds,
             )
 
             sqs_messages = response.get("Messages", [])
             if not sqs_messages:
                 logger.debug(
                     f"Waiting some seconds because no message was received, seconds={wait_seconds}, queue_url={self.url}"
                 )
```

### Comparing `sqsx-0.4.0/sqsx.egg-info/PKG-INFO` & `sqsx-0.5/sqsx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqsx
-Version: 0.4.0
+Version: 0.5.0
 Summary: A simple task processor for Amazon SQS
 Home-page: https://github.com/allisson/pysqsx
 Author: Allisson Azevedo
 Author-email: allisson@gmail.com
 Keywords: aws,sqs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sqsx-0.4.0/tests/conftest.py` & `sqsx-0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqsx-0.4.0/tests/test_helper.py` & `sqsx-0.5/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `sqsx-0.4.0/tests/test_queue.py` & `sqsx-0.5/tests/test_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     thread.daemon = True
     thread.start()
     handler = SumHandler()
 
     queue.add_task_handler("my_task", handler)
     queue.add_task("my_task", a=1, b=2, c=3)
 
-    queue.consume_messages(wait_seconds=1, run_forever=True)
+    queue.consume_messages(wait_seconds=1, polling_wait_seconds=0, run_forever=True)
 
     assert handler.result_sum == 6
 
 
 def test_raw_queue_add_message(raw_queue):
     expected_md5_message_body = "069840f6917e85a02167febb964f0041"
     expected_md5_message_attribute = "90f34a800b9d242c1b32320e4a3ed630"
@@ -287,10 +287,10 @@
     handler = handler = CallCountHandler()
     raw_queue.message_handler_function = handler
 
     raw_queue.add_message(message_body="Message Body")
     raw_queue.add_message(message_body="Message Body")
     raw_queue.add_message(message_body="Message Body")
 
-    raw_queue.consume_messages(wait_seconds=1, run_forever=True)
+    raw_queue.consume_messages(wait_seconds=1, polling_wait_seconds=0, run_forever=True)
 
     assert handler.call_count == 3
```

