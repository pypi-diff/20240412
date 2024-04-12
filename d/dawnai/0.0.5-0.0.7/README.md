# Comparing `tmp/dawnai-0.0.5.tar.gz` & `tmp/dawnai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dawnai-0.0.5.tar", last modified: Fri Apr 12 05:38:38 2024, max compression
+gzip compressed data, was "dawnai-0.0.7.tar", last modified: Fri Apr 12 21:31:39 2024, max compression
```

## Comparing `dawnai-0.0.5.tar` & `dawnai-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.683211 dawnai-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 05:38:38.683211 dawnai-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 05:38:30.000000 dawnai-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.679211 dawnai-0.0.5/dawnai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:30.000000 dawnai-0.0.5/dawnai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-12 05:38:30.000000 dawnai-0.0.5/dawnai/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.683211 dawnai-0.0.5/dawnai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 05:38:38.000000 dawnai-0.0.5/dawnai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:38:38.683211 dawnai-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-12 05:38:30.000000 dawnai-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:38:38.679211 dawnai-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-12 05:38:30.000000 dawnai-0.0.5/tests/test_analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:39.934969 dawnai-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 21:31:39.934969 dawnai-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 21:31:31.000000 dawnai-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:39.930969 dawnai-0.0.7/dawnai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:31.000000 dawnai-0.0.7/dawnai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-12 21:31:31.000000 dawnai-0.0.7/dawnai/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:39.934969 dawnai-0.0.7/dawnai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-12 21:31:39.000000 dawnai-0.0.7/dawnai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-12 21:31:39.000000 dawnai-0.0.7/dawnai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:31:39.000000 dawnai-0.0.7/dawnai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 21:31:39.000000 dawnai-0.0.7/dawnai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 21:31:39.000000 dawnai-0.0.7/dawnai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:31:39.934969 dawnai-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-12 21:31:31.000000 dawnai-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:31:39.934969 dawnai-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-12 21:31:31.000000 dawnai-0.0.7/tests/test_analytics.py
```

### Comparing `dawnai-0.0.5/PKG-INFO` & `dawnai-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.5
+Version: 0.0.7
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.5/dawnai/analytics.py` & `dawnai-0.0.7/dawnai/analytics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import time
 from typing import Union, List, Dict, Optional
 import aiohttp
 
 write_key = None
-api_url = "http://api.dawnai.com/"
+api_url = "https://api.dawnai.com/"
 buffer_size = 50
 buffer_timeout = 5
 buffer = []
 flush_task = None
 debug_logs = False
 
 
@@ -50,15 +50,15 @@
     asyncio.run(save_to_buffer({"type": "track-ai", "data": data}))
 
 
 async def save_to_buffer(event: Dict[str, Union[str, Dict]]) -> None:
     global buffer, flush_task
 
     if debug_logs:
-        print(f"Added to buffer: {event}")
+        print(f"[dawn] Added to buffer: {event}")
 
     buffer.append(event)
 
     if len(buffer) >= buffer_size:
         await flush()
     elif flush_task is None:
         flush_task = asyncio.create_task(schedule_flush())
@@ -110,11 +110,12 @@
         "Authorization": f"Bearer {write_key}",
     }
 
     async with aiohttp.ClientSession() as session:
         async with session.post(url, json=dataEntries, headers=headers) as response:
             try:
                 response.raise_for_status()
+                if debug_logs:
+                    print(f"[dawn] Response: {response.status}")
             except aiohttp.ClientResponseError as e:
                 print(f"Error: {response.text}")
                 raise
-        raise e
```

### Comparing `dawnai-0.0.5/dawnai.egg-info/PKG-INFO` & `dawnai-0.0.7/dawnai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dawnai
-Version: 0.0.5
+Version: 0.0.7
 Summary: Dawn (Python SDK)
 Home-page: https://dawnai.com
 Author: Dawn
 Author-email: sdk@dawnai.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

### Comparing `dawnai-0.0.5/setup.py` & `dawnai-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dawnai",
-    version="0.0.5",
+    version="0.0.7",
     description="Dawn (Python SDK)",
     author="Dawn",
     author_email="sdk@dawnai.com",
     long_description="For questions, email us at sdk@dawnai.com",
     long_description_content_type="text/markdown",
     url="https://dawnai.com",
     packages=find_packages(include=["dawnai", "README.md"]),
```

### Comparing `dawnai-0.0.5/tests/test_analytics.py` & `dawnai-0.0.7/tests/test_analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 from unittest.mock import patch
 import dawnai.analytics as analytics
 
 
 class TestAnalytics(unittest.TestCase):
     def setUp(self):
         # Set up any necessary test data or configurations
-        analytics.write_key = "0000"
+        analytics.write_key = "XXXX"
         analytics.debug_logs = True
-        analytics.api_url = "http://localhost:3000/"
+
+    #  analytics.api_url = "http://localhost:3000/"
 
     def tearDown(self):
         # Clean up any resources or reset any state after each test
         pass
 
     def test_identify(self):
 
@@ -37,14 +38,15 @@
 
     def test_track_ai(self):
         user_id = "user123"
         event = "ai_chat"
         model = "GPT-3"
         input_text = "Hello"
         output_text = "Hi there!"
+
         analytics.track_ai(
             user_id, event, model=model, user_input=input_text, output=output_text
         )
 
         asyncio.run(analytics.flush())
 
         # No assertion needed as the SDK handles the request internally
```

