# Comparing `tmp/rtrafactor-0.2.tar.gz` & `tmp/rtrafactor-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrafactor-0.2.tar", last modified: Fri Apr 12 10:26:27 2024, max compression
+gzip compressed data, was "rtrafactor-0.3.tar", last modified: Fri Apr 12 10:39:21 2024, max compression
```

## Comparing `rtrafactor-0.2.tar` & `rtrafactor-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.733166 rtrafactor-0.2/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:26:27.732893 rtrafactor-0.2/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.731788 rtrafactor-0.2/rtrafactor/
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:25:01.000000 rtrafactor-0.2/rtrafactor/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.2/rtrafactor/webconnect.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.732582 rtrafactor-0.2/rtrafactor.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:26:27.733213 rtrafactor-0.2/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:26:02.000000 rtrafactor-0.2/setup.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.732704 rtrafactor-0.2/tests/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.2/tests/test_webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.662244 rtrafactor-0.3/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:39:21.662047 rtrafactor-0.3/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661065 rtrafactor-0.3/rtrafactor/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.3/rtrafactor/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.3/rtrafactor/webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661770 rtrafactor-0.3/rtrafactor.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:39:21.662292 rtrafactor-0.3/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:36:29.000000 rtrafactor-0.3/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661898 rtrafactor-0.3/tests/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.3/tests/test_webconnect.py
```

### Comparing `rtrafactor-0.2/rtrafactor/__init__.py` & `rtrafactor-0.3/rtrafactor/webconnect.py`

 * *Files identical despite different names*

### Comparing `rtrafactor-0.2/rtrafactor/webconnect.py` & `rtrafactor-0.3/rtrafactor/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from googlesearch import search
 import requests
 from bs4 import BeautifulSoup
 
 class RTRAConnector:
-    def __init__(self, huggingface_model, huggingface_api_token):
-        self.huggingface_model = huggingface_model
-        self.huggingface_api_token = huggingface_api_token
+    def __init__(self, model, api_token):
+        self.model = model
+        self.api_token = api_token
         self.max_tokens = 60000
 
     def search(self, query):
         try:
             results = search(query, num_results=5)  # Use num_results to limit search results
             urls = list(results)
             return urls
@@ -43,16 +43,16 @@
             return scraped_text
         elif data_source == "HuggingFace":
             return self.generate_huggingface_response(query)
 
     def generate_huggingface_response(self, query):
         prompt = f"Search results for '{query}':\n{self.generate_response(query, 'Google')}\n\nNow, give answers to this query:\n"
         payload = {"inputs": prompt}
-        headers = {"Authorization": f"Bearer {self.huggingface_api_token}"}
-        huggingface_url = f"https://api-inference.huggingface.co/models/{self.huggingface_model}"
+        headers = {"Authorization": f"Bearer {self.api_token}"}
+        huggingface_url = f"https://api-inference.huggingface.co/models/{self.model}"
         response = requests.post(huggingface_url, headers=headers, json=payload)
 
         if response.status_code == 200:
             response_data = response.json()
             if isinstance(response_data, list) and len(response_data) > 0:
                 generated_text = response_data[0].get("generated_text", "")
                 # Extract only the answer part
```

