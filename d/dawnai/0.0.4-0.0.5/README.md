# Comparing `tmp/dawnai-0.0.4.tar.gz` & `tmp/dawnai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawnai-0.0.4.tar", last modified: Wed Apr 10 22:38:17 2024, max compression
+gzip compressed data, was "dawnai-0.0.5.tar", last modified: Fri Apr 12 05:38:38 2024, max compression
```

## Comparing `dawnai-0.0.4.tar` & `dawnai-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:38:17.088808 dawnai-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 22:38:17.088808 dawnai-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-10 22:38:07.000000 dawnai-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:38:17.084808 dawnai-0.0.4/dawnai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 22:38:07.000000 dawnai-0.0.4/dawnai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-10 22:38:07.000000 dawnai-0.0.4/dawnai/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:38:17.088808 dawnai-0.0.4/dawnai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-10 22:38:17.000000 dawnai-0.0.4/dawnai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-10 22:38:17.000000 dawnai-0.0.4/dawnai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 22:38:17.000000 dawnai-0.0.4/dawnai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 22:38:17.000000 dawnai-0.0.4/dawnai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 22:38:17.000000 dawnai-0.0.4/dawnai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 22:38:17.088808 dawnai-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-10 22:38:07.000000 dawnai-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 22:38:17.088808 dawnai-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-10 22:38:07.000000 dawnai-0.0.4/tests/test_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.683211 dawnai-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 05:38:38.683211 dawnai-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 05:38:30.000000 dawnai-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.679211 dawnai-0.0.5/dawnai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:30.000000 dawnai-0.0.5/dawnai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-12 05:38:30.000000 dawnai-0.0.5/dawnai/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.683211 dawnai-0.0.5/dawnai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:38:38.683211 dawnai-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-12 05:38:30.000000 dawnai-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.679211 dawnai-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-12 05:38:30.000000 dawnai-0.0.5/tests/test_analytics.py
```

### Comparing `dawnai-0.0.4/PKG-INFO` & `dawnai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.4/dawnai/analytics.py` & `dawnai-0.0.5/dawnai/analytics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 buffer = []
 flush_task = None
 debug_logs = False
 
 
 def identify(user_id: str, traits: Dict[str, Union[str, int, bool, float]]) -> None:
     data = {"user_id": user_id, "traits": traits}
-    asyncio.run(save_to_buffer({"type": "track-ai", "data": data}))
+    asyncio.run(save_to_buffer({"type": "identify", "data": data}))
 
 
 def track(
     user_id: str,
     event: str,
     properties: Optional[Dict[str, Union[str, int, bool, float]]] = None,
 ) -> None:
@@ -87,16 +87,19 @@
     for event in current_buffer:
         endpoint = event["type"]
         data = event["data"]
         if endpoint not in grouped_events:
             grouped_events[endpoint] = []
         grouped_events[endpoint].append(data)
 
+    tasks = []
     for endpoint, events_data in grouped_events.items():
-        asyncio.create_task(send_request(endpoint, events_data))
+        tasks.append(asyncio.create_task(send_request(endpoint, events_data)))
+
+    await asyncio.gather(*tasks)
 
 
 async def send_request(
     endpoint: str, dataEntries: List[Dict[str, Union[str, Dict]]]
 ) -> None:
     if write_key is None:
         raise ValueError("write_key is not set")
```

### Comparing `dawnai-0.0.4/dawnai.egg-info/PKG-INFO` & `dawnai-0.0.5/dawnai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.4/setup.py` & `dawnai-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dawnai",
-    version="0.0.4",
+    version="0.0.5",
     description="Dawn (Python SDK)",
     author="Dawn",
     author_email="sdk@dawnai.com",
     long_description="For questions, email us at sdk@dawnai.com",
     long_description_content_type="text/markdown",
     url="https://dawnai.com",
     packages=find_packages(include=["dawnai", "README.md"]),
```

### Comparing `dawnai-0.0.4/tests/test_analytics.py` & `dawnai-0.0.5/tests/test_analytics.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,50 @@
+import asyncio
 import unittest
 from unittest.mock import patch
 import dawnai.analytics as analytics
 
 
 class TestAnalytics(unittest.TestCase):
     def setUp(self):
         # Set up any necessary test data or configurations
         analytics.write_key = "0000"
+        analytics.debug_logs = True
+        analytics.api_url = "http://localhost:3000/"
 
     def tearDown(self):
         # Clean up any resources or reset any state after each test
         pass
 
     def test_identify(self):
 
         user_id = "user123"
         traits = {"email": "john@example.com", "name": "John"}
 
         try:
             analytics.identify(user_id, traits)
         except e:
             print("Error")
+        asyncio.run(analytics.flush())
         # No assertion needed as the SDK handles the request internally
 
     def test_track(self):
         user_id = "user123"
-        event = "Signed Up"
+        event = "signed_up"
         properties = {"plan": "Premium"}
         analytics.track(user_id, event, properties)
+        asyncio.run(analytics.flush())
         # No assertion needed as the SDK handles the request internally
 
     def test_track_ai(self):
         user_id = "user123"
-        event = "AI Chat"
+        event = "ai_chat"
         model = "GPT-3"
         input_text = "Hello"
         output_text = "Hi there!"
         analytics.track_ai(
             user_id, event, model=model, user_input=input_text, output=output_text
         )
+
+        asyncio.run(analytics.flush())
+
         # No assertion needed as the SDK handles the request internally
```

