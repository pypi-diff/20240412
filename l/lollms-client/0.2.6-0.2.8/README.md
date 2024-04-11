# Comparing `tmp/lollms_client-0.2.6.tar.gz` & `tmp/lollms_client-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.2.6.tar", last modified: Thu Apr 11 21:39:15 2024, max compression
+gzip compressed data, was "lollms_client-0.2.8.tar", last modified: Thu Apr 11 22:05:38 2024, max compression
```

## Comparing `lollms_client-0.2.6.tar` & `lollms_client-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.159492 lollms_client-0.2.6/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:39:15.158493 lollms_client-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.134927 lollms_client-0.2.6/lollms_client/
--rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.6/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    12136 2024-04-11 21:39:05.000000 lollms_client-0.2.6/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.6/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.6/lollms_client/lollms_types.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.157478 lollms_client-0.2.6/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-11 21:39:15.000000 lollms_client-0.2.6/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 21:39:15.159492 lollms_client-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-11 21:39:11.000000 lollms_client-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 22:05:38.770987 lollms_client-0.2.8/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-11 22:05:38.768982 lollms_client-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 22:05:38.745195 lollms_client-0.2.8/lollms_client/
+-rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.8/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    13011 2024-04-11 22:00:30.000000 lollms_client-0.2.8/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.8/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.8/lollms_client/lollms_types.py
+drwxrwxrwx   0        0        0        0 2024-04-11 22:05:38.768982 lollms_client-0.2.8/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-11 22:05:38.000000 lollms_client-0.2.8/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-04-11 22:05:38.000000 lollms_client-0.2.8/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 22:05:38.000000 lollms_client-0.2.8/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 22:05:38.000000 lollms_client-0.2.8/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 22:05:38.000000 lollms_client-0.2.8/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 22:05:38.770987 lollms_client-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-11 22:03:08.000000 lollms_client-0.2.8/setup.py
```

### Comparing `lollms_client-0.2.6/LICENSE` & `lollms_client-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.6/PKG-INFO` & `lollms_client-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.6
+Version: 0.2.8
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.6/README.md` & `lollms_client-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.6/lollms_client/lollms_core.py` & `lollms_client-0.2.8/lollms_client/lollms_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.repeat_last_n = repeat_last_n
         self.seed = seed
         self.n_threads = n_threads
 
         self.service_key = service_key
 
 
-    def generate_text(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str=""):
+    def generate_text(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
         temperature = temperature if temperature is not None else self.temperature
@@ -67,28 +67,47 @@
             "top_p": self.top_p,
             "repeat_penalty": repeat_penalty,
             "repeat_last_n": repeat_last_n,
             "seed": seed,
             "n_threads": n_threads
         }
 
-        response = requests.post(url, json=data, headers=headers)
-
-        if response.status_code == 200:
-            try:
-                text = response.text.strip().replace('\"','"')
-                if text[0]=='"':
-                    text = text[1:]
-                if text[-1]=='"':
-                    text = text[:-1]
-                return text
-            except Exception as ex:
-                return {"status": False, "error": str(ex)}
+        response = requests.post(url, json=data, headers=headers, stream=stream)
+        if not stream:
+            if response.status_code == 200:
+                try:
+                    text = response.text.strip().replace('\"','"')
+                    if text[0]=='"':
+                        text = text[1:]
+                    if text[-1]=='"':
+                        text = text[:-1]
+                    return text
+                except Exception as ex:
+                    return {"status": False, "error": str(ex)}
+            else:
+                return {"status": False, "error": response.text}
         else:
-            return {"status": False, "error": response.text}
+            text = ""
+            if response.status_code==200:
+                try:
+                    for line in response.iter_lines():
+                        chunk = line.decode("utf-8")
+                        text += chunk
+                        if streaming_callback:
+                            streaming_callback(chunk, MSG_TYPE.MSG_TYPE_CHUNK)
+                    if text[0]=='"':
+                        text = text[1:]
+                    if text[-1]=='"':
+                        text = text[:-1]
+                    return text
+                except Exception as ex:
+                    return {"status": False, "error": str(ex)}
+            else:
+                return {"status": False, "error": response.text}
+
 
     def generate_completion(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format="vllm instruct", service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
```

### Comparing `lollms_client-0.2.6/lollms_client/lollms_tasks.py` & `lollms_client-0.2.8/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.6/lollms_client/lollms_types.py` & `lollms_client-0.2.8/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.6/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.2.8/lollms_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.6
+Version: 0.2.8
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.6/setup.py` & `lollms_client-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lollms_client",
-    version="0.2.6",
+    version="0.2.8",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

