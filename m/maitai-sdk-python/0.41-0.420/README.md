# Comparing `tmp/maitai-sdk-python-0.41.tar.gz` & `tmp/maitai-sdk-python-0.420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai-sdk-python-0.41.tar", last modified: Tue Apr  9 05:28:26 2024, max compression
+gzip compressed data, was "maitai-sdk-python-0.420.tar", last modified: Fri Apr 12 15:28:18 2024, max compression
```

## Comparing `maitai-sdk-python-0.41.tar` & `maitai-sdk-python-0.420.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 05:28:26.321935 maitai-sdk-python-0.41/
--rw-rw-rw-   0        0        0      355 2024-04-09 05:28:26.320935 maitai-sdk-python-0.41/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai-sdk-python-0.41/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 05:28:26.301882 maitai-sdk-python-0.41/maitai/
--rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai-sdk-python-0.41/maitai/__init__.py
--rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai-sdk-python-0.41/maitai/_config.py
--rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.41/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     7111 2024-04-09 05:13:46.000000 maitai-sdk-python-0.41/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.41/maitai/_loadable.py
--rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai-sdk-python-0.41/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-04-09 05:28:26.318946 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      355 2024-04-09 05:28:25.000000 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-09 05:28:26.000000 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 05:28:25.000000 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-09 05:28:25.000000 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-09 05:28:25.000000 maitai-sdk-python-0.41/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-09 05:28:26.321935 maitai-sdk-python-0.41/setup.cfg
--rw-rw-rw-   0        0        0      553 2024-04-09 05:28:19.000000 maitai-sdk-python-0.41/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.936898 maitai-sdk-python-0.420/
+-rw-rw-rw-   0        0        0      356 2024-04-12 15:28:18.934899 maitai-sdk-python-0.420/PKG-INFO
+-rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai-sdk-python-0.420/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.899668 maitai-sdk-python-0.420/maitai/
+-rw-rw-rw-   0        0        0      359 2024-03-30 19:31:01.000000 maitai-sdk-python-0.420/maitai/__init__.py
+-rw-rw-rw-   0        0        0      811 2024-03-30 19:21:46.000000 maitai-sdk-python-0.420/maitai/_config.py
+-rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.420/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0     7137 2024-04-09 05:44:47.000000 maitai-sdk-python-0.420/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.420/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      266 2024-03-30 18:24:42.000000 maitai-sdk-python-0.420/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:28:18.932899 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      356 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-12 15:28:18.000000 maitai-sdk-python-0.420/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:28:18.937898 maitai-sdk-python-0.420/setup.cfg
+-rw-rw-rw-   0        0        0      554 2024-04-12 15:27:37.000000 maitai-sdk-python-0.420/setup.py
```

### Comparing `maitai-sdk-python-0.41/README.md` & `maitai-sdk-python-0.420/README.md`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.41/maitai/_config.py` & `maitai-sdk-python-0.420/maitai/_config.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.41/maitai/_eval_request.py` & `maitai-sdk-python-0.420/maitai/_eval_request.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.41/maitai/_evaluator.py` & `maitai-sdk-python-0.420/maitai/_evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     # MAITAI_HOST = 'https://maitai.ai.yewpay.com'
     MAITAI_HOST = 'https://api.dev.yewpay.com'
 
     def __init__(self):
         super().__init__()
 
     @classmethod
-    def evaluate(cls, session_id, reference_id, content):
-        eval_request: EvalRequest = cls.create_eval_request(session_id, reference_id, content)
+    def evaluate(cls, session_id, reference_id, action_type, content):
+        eval_request: EvalRequest = cls.create_eval_request(session_id, reference_id, action_type, content)
         cls.send_evaluation_request(eval_request)
 
     @classmethod
     def create_eval_request(cls, session_id, reference_id, action_type, content):
         if type(content) != str:
             raise Exception('Content must be a string')
         eval_request: EvalRequest = EvalRequest()
```

### Comparing `maitai-sdk-python-0.41/maitai/_loadable.py` & `maitai-sdk-python-0.420/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.41/setup.py` & `maitai-sdk-python-0.420/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai-sdk-python',
-    version='0.41',
+    version='0.420',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     # Optional metadata
     author='Christian DalSanto',
     author_email='christian@yewpay.com',
```

