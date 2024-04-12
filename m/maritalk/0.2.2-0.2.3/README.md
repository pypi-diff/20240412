# Comparing `tmp/maritalk-0.2.2.tar.gz` & `tmp/maritalk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maritalk-0.2.2.tar", last modified: Mon Mar 25 12:18:44 2024, max compression
+gzip compressed data, was "maritalk-0.2.3.tar", last modified: Fri Apr 12 17:58:36 2024, max compression
```

## Comparing `maritalk-0.2.2.tar` & `maritalk-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.406365 maritalk-0.2.2/
--rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10205 2024-03-25 12:18:44.406365 maritalk-0.2.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8364 2024-03-22 17:23:17.000000 maritalk-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.402365 maritalk-0.2.2/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.406365 maritalk-0.2.2/examples/local/
--rw-rw-r--   0 root         (0) root         (0)      996 2024-03-22 17:23:17.000000 maritalk-0.2.2/examples/local/question_answering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.406365 maritalk-0.2.2/maritalk/
--rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.2/maritalk/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1238 2024-03-22 17:23:17.000000 maritalk-0.2.2/maritalk/download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.406365 maritalk-0.2.2/maritalk/resources/
--rw-rw-r--   0 root         (0) root         (0)     8917 2024-03-22 17:23:17.000000 maritalk-0.2.2/maritalk/resources/api.py
--rw-rw-r--   0 root         (0) root         (0)    11210 2024-03-25 12:18:15.000000 maritalk-0.2.2/maritalk/resources/local.py
--rw-rw-r--   0 root         (0) root         (0)     1042 2024-03-22 17:23:17.000000 maritalk-0.2.2/maritalk/start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 12:18:44.406365 maritalk-0.2.2/maritalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10205 2024-03-25 12:18:44.000000 maritalk-0.2.2/maritalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      351 2024-03-25 12:18:44.000000 maritalk-0.2.2/maritalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 12:18:44.000000 maritalk-0.2.2/maritalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-03-25 12:18:44.000000 maritalk-0.2.2/maritalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-25 12:18:44.000000 maritalk-0.2.2/maritalk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      721 2024-03-25 12:18:15.000000 maritalk-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 12:18:44.406365 maritalk-0.2.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/
+-rw-rw-r--   0 root         (0) root         (0)     1088 2023-09-04 19:10:06.000000 maritalk-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10180 2024-04-12 17:58:36.836048 maritalk-0.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8339 2024-04-12 17:58:00.000000 maritalk-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.832048 maritalk-0.2.3/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.832048 maritalk-0.2.3/examples/local/
+-rw-rw-r--   0 root         (0) root         (0)      996 2024-04-12 17:58:00.000000 maritalk-0.2.3/examples/local/question_answering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk/
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-12-03 16:28:52.000000 maritalk-0.2.3/maritalk/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1238 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk/resources/
+-rw-rw-r--   0 root         (0) root         (0)     8917 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/resources/api.py
+-rw-rw-r--   0 root         (0) root         (0)    11855 2024-04-12 17:58:02.000000 maritalk-0.2.3/maritalk/resources/local.py
+-rw-rw-r--   0 root         (0) root         (0)     1042 2024-04-12 17:58:00.000000 maritalk-0.2.3/maritalk/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:58:36.836048 maritalk-0.2.3/maritalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10180 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      351 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 17:58:36.000000 maritalk-0.2.3/maritalk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      721 2024-04-12 17:58:30.000000 maritalk-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 17:58:36.836048 maritalk-0.2.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)       37 2023-09-04 19:10:06.000000 maritalk-0.2.3/setup.py
```

### Comparing `maritalk-0.2.2/LICENSE` & `maritalk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.2/PKG-INFO` & `maritalk-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 
 - [Introdução](#introdução)  
 - [Instalação](#instalação)  
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
-- [Exemplo Maritalk no LlamaIndex](https://github.com/run-llama/llama_index/blob/main/docs/examples/llm/maritalk.ipynb)
+- [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
 [MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
```

### Comparing `maritalk-0.2.2/README.md` & `maritalk-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 - [Introdução](#introdução)  
 - [Instalação](#instalação)  
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
-- [Exemplo Maritalk no LlamaIndex](https://github.com/run-llama/llama_index/blob/main/docs/examples/llm/maritalk.ipynb)
+- [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
 [MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
```

### Comparing `maritalk-0.2.2/examples/local/question_answering.py` & `maritalk-0.2.3/examples/local/question_answering.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.2/maritalk/download.py` & `maritalk-0.2.3/maritalk/download.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.2/maritalk/resources/api.py` & `maritalk-0.2.3/maritalk/resources/api.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.2/maritalk/resources/local.py` & `maritalk-0.2.3/maritalk/resources/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import re
 import csv
 import time
-import shutil
 import atexit
 import subprocess
 from tqdm import tqdm
 from pathlib import Path
 from typing import List, Dict, Optional, Union, Optional
-from ctypes.util import find_library
 import requests
 from requests.exceptions import ConnectionError
 
 
 def check_gpu():
     try:
         result = subprocess.run(
@@ -21,17 +19,15 @@
                 '--query-gpu=name,compute_cap',
                 '--format=csv',
             ],
             capture_output=True,
             text=True,
             check=True,
         )
-
         reader = csv.reader(result.stdout.strip().split('\n'))
-
         headers = next(reader)
         rows = list(reader)
 
         for row in rows:
             gpu_name, compute_cap = row
             if float(compute_cap) >= 8.0:
                 return True
@@ -39,35 +35,53 @@
         raise Exception(
             f"The detected device is not supported: {gpu_name}. We currently support Nvidia GPUs with compute capability >= 8.0."
         )
     except subprocess.CalledProcessError as e:
         raise Exception(f"Error executing command: {e}")
     except FileNotFoundError as e:
         raise Exception(
-            "Nvidia-smi is not installed. Please install the Nvidia driver and the CUDA toolkit."
+            "Nvidia-SMI is not installed. Please install the Nvidia driver and the CUDA toolkit."
         )
 
 
 def find_libs():
     versions = {
         "cuda_version": None,
     }
 
-    cublas_lib = find_library("cublas")
-    if cublas_lib and ".11" in cublas_lib:
-        versions["cuda_version"] = 11
-    if cublas_lib and ".12" in cublas_lib:
-        versions["cuda_version"] = 12
+    try:
+        output = subprocess.run(
+            ['nvidia-smi'],
+            stdout=subprocess.PIPE,
+        ).stdout.decode('utf-8')
+        cuda_version_match = re.search(r"CUDA Version: (\d+\.\d+)", output)
+
+        if not cuda_version_match:
+            raise Exception("""Could not automatically detect the CUDA version. Verify the CUDA Toolkit installation or set the `cuda_version` parameter manually. For example:
+
+```
+model.start_server("<YOUR LICENSE>", cuda_version="12.3")
+```
+
+To install the CUDA Toolkit, please refer to: https://developer.nvidia.com/cuda-downloads""")
+
+        versions["cuda_version"] = cuda_version_match.group(1)
+    except subprocess.CalledProcessError as e:
+        raise Exception(f"Error executing command: {e}")
+    except FileNotFoundError as e:
+        raise Exception(
+            "Nvidia-SMI is not installed. Please install the Nvidia driver and the CUDA toolkit."
+        )
 
     return versions
 
 
 def download(license: str, bin_path: str, dependencies: Dict[str, int]):
     download_url = (
-        "https://m64xplb35dhr3se7ipvtmbdnk40ahktr.lambda-url.us-east-1.on.aws/"
+        "https://functions.maritaca.ai/local/download"
     )
     response = requests.post(
         download_url,
         json={
             "license": license,
             "cuda_version": dependencies["cuda_version"],
         },
```

### Comparing `maritalk-0.2.2/maritalk/start.py` & `maritalk-0.2.3/maritalk/start.py`

 * *Files identical despite different names*

### Comparing `maritalk-0.2.2/maritalk.egg-info/PKG-INFO` & `maritalk-0.2.3/maritalk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maritalk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Client library for the MariTalk API
 Author-email: Maritaca AI <info@maritaca.ai>
 License: The MIT License
         
         Copyright (c) Maritaca AI (https://maritaca.ai)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 
 - [Introdução](#introdução)  
 - [Instalação](#instalação)  
 - [Exemplo de uso](#exemplo-de-uso)
 - [Exemplo de uso via requisições HTTP - Python](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.ipynb)
 - [Exemplo de uso via requisições HTTP - JavaScript](https://github.com/maritaca-ai/maritalk-api/blob/main/examples/api/maritalk_via_requisições_https.js)
 - [Exemplo MariTalk + RAG com LangChain](https://python.langchain.com/docs/integrations/chat/maritalk)
-- [Exemplo Maritalk no LlamaIndex](https://github.com/run-llama/llama_index/blob/main/docs/examples/llm/maritalk.ipynb)
+- [Exemplo Maritalk no LlamaIndex](https://docs.llamaindex.ai/en/latest/examples/llm/maritalk)
 - [Documentação Swagger](https://chat.maritaca.ai/docs)
 
 [MariTalk local](https://github.com/maritaca-ai/maritalk-api/blob/main/README-Local.md)
 
 [Chat (gratuito)](#web-chat)
 
 # Introdução
```

### Comparing `maritalk-0.2.2/pyproject.toml` & `maritalk-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maritalk"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Maritaca AI", email="info@maritaca.ai" },
 ]
 description = "Client library for the MariTalk API"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
```

