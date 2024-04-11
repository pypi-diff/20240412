# Comparing `tmp/lollms_client-0.2.5.tar.gz` & `tmp/lollms_client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms_client-0.2.5.tar", last modified: Thu Apr 11 21:25:48 2024, max compression
+gzip compressed data, was "lollms_client-0.2.6.tar", last modified: Thu Apr 11 21:39:15 2024, max compression
```

## Comparing `lollms_client-0.2.5.tar` & `lollms_client-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.942571 lollms_client-0.2.5/
--rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:25:48.941569 lollms_client-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.922446 lollms_client-0.2.5/lollms_client/
--rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.5/lollms_client/__init__.py
--rw-rw-rw-   0        0        0    12127 2024-04-11 21:17:29.000000 lollms_client-0.2.5/lollms_client/lollms_core.py
--rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.5/lollms_client/lollms_tasks.py
--rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.5/lollms_client/lollms_types.py
-drwxrwxrwx   0        0        0        0 2024-04-11 21:25:48.940568 lollms_client-0.2.5/lollms_client.egg-info/
--rw-rw-rw-   0        0        0     3258 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-11 21:25:48.000000 lollms_client-0.2.5/lollms_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 21:25:48.942571 lollms_client-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-11 21:25:01.000000 lollms_client-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.159492 lollms_client-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-03-30 19:02:48.000000 lollms_client-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     3258 2024-04-11 21:39:15.158493 lollms_client-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2780 2024-04-08 23:28:01.000000 lollms_client-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.134927 lollms_client-0.2.6/lollms_client/
+-rw-rw-rw-   0        0        0      105 2024-04-11 21:24:53.000000 lollms_client-0.2.6/lollms_client/__init__.py
+-rw-rw-rw-   0        0        0    12136 2024-04-11 21:39:05.000000 lollms_client-0.2.6/lollms_client/lollms_core.py
+-rw-rw-rw-   0        0        0     1457 2024-04-11 21:23:29.000000 lollms_client-0.2.6/lollms_client/lollms_tasks.py
+-rw-rw-rw-   0        0        0     2059 2024-04-11 21:15:36.000000 lollms_client-0.2.6/lollms_client/lollms_types.py
+drwxrwxrwx   0        0        0        0 2024-04-11 21:39:15.157478 lollms_client-0.2.6/lollms_client.egg-info/
+-rw-rw-rw-   0        0        0     3258 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-04-11 21:39:15.000000 lollms_client-0.2.6/lollms_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 21:39:14.000000 lollms_client-0.2.6/lollms_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-11 21:39:15.159492 lollms_client-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      720 2024-04-11 21:39:11.000000 lollms_client-0.2.6/setup.py
```

### Comparing `lollms_client-0.2.5/LICENSE` & `lollms_client-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.5/PKG-INFO` & `lollms_client-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.5
+Version: 0.2.6
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.5/README.md` & `lollms_client-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.5/lollms_client/lollms_core.py` & `lollms_client-0.2.6/lollms_client/lollms_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                     text = text[:-1]
                 return text
             except Exception as ex:
                 return {"status": False, "error": str(ex)}
         else:
             return {"status": False, "error": response.text}
 
-    def generate_completion(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format="vllm", service_key:str="", streaming_callback=None):
+    def generate_completion(self, prompt, host_address=None, model_name=None, personality=None, n_predict=None, stream=False, temperature=0.1, top_k=50, top_p=0.95, repeat_penalty=0.8, repeat_last_n=40, seed=None, n_threads=8, completion_format="vllm instruct", service_key:str="", streaming_callback=None):
         # Set default values to instance variables if optional arguments are None
         host_address = host_address if host_address else self.host_address
         model_name = model_name if model_name else self.model_name
         n_predict = n_predict if n_predict else self.n_predict
         personality = personality if personality is not None else self.personality
         # Set temperature, top_k, top_p, repeat_penalty, repeat_last_n, seed, n_threads to the instance variables if they are not provided or None
         temperature = temperature if temperature is not None else self.temperature
```

### Comparing `lollms_client-0.2.5/lollms_client/lollms_tasks.py` & `lollms_client-0.2.6/lollms_client/lollms_tasks.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.5/lollms_client/lollms_types.py` & `lollms_client-0.2.6/lollms_client/lollms_types.py`

 * *Files identical despite different names*

### Comparing `lollms_client-0.2.5/lollms_client.egg-info/PKG-INFO` & `lollms_client-0.2.6/lollms_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms_client
-Version: 0.2.5
+Version: 0.2.6
 Summary: A client library for LoLLMs generate endpoint
 Home-page: https://github.com/ParisNeo/lollms_client
 Author: ParisNeo
 Author-email: parisneoai@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms_client-0.2.5/setup.py` & `lollms_client-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lollms_client",
-    version="0.2.5",
+    version="0.2.6",
     author="ParisNeo",
     author_email="parisneoai@gmail.com",
     description="A client library for LoLLMs generate endpoint",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms_client",
     packages=setuptools.find_packages(),
```

