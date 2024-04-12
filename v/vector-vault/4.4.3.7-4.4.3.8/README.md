# Comparing `tmp/vector_vault-4.4.3.7.tar.gz` & `tmp/vector_vault-4.4.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.3.7.tar", last modified: Thu Apr 11 19:22:03 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.8.tar", last modified: Fri Apr 12 02:37:18 2024, max compression
```

## Comparing `vector_vault-4.4.3.7.tar` & `vector_vault-4.4.3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 19:22:03.197538 vector_vault-4.4.3.7/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.7/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 19:22:03.197390 vector_vault-4.4.3.7/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.7/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-11 19:22:03.197573 vector_vault-4.4.3.7/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-11 19:12:12.000000 vector_vault-4.4.3.7/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 19:22:03.192603 vector_vault-4.4.3.7/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-11 19:22:03.000000 vector_vault-4.4.3.7/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-11 19:22:03.000000 vector_vault-4.4.3.7/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-11 19:22:03.000000 vector_vault-4.4.3.7/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-11 19:22:03.000000 vector_vault-4.4.3.7/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-11 19:22:03.000000 vector_vault-4.4.3.7/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-11 19:22:03.197006 vector_vault-4.4.3.7/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.7/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16810 2024-04-08 20:07:41.000000 vector_vault-4.4.3.7/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.7/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.3.7/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.7/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.7/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.7/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.7/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62653 2024-04-11 19:21:38.000000 vector_vault-4.4.3.7/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5364 2024-04-04 04:33:57.000000 vector_vault-4.4.3.7/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.7/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.808434 vector_vault-4.4.3.8/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.8/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 02:37:18.808286 vector_vault-4.4.3.8/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.8/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-12 02:37:18.808472 vector_vault-4.4.3.8/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-12 02:37:13.000000 vector_vault-4.4.3.8/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.805340 vector_vault-4.4.3.8/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.808134 vector_vault-4.4.3.8/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.8/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.3.8/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.8/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.3.8/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.8/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.8/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.8/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.8/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62687 2024-04-12 02:37:09.000000 vector_vault-4.4.3.8/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.3.8/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.8/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.3.7/LICENSE` & `vector_vault-4.4.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/PKG-INFO` & `vector_vault-4.4.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.3.7
+Version: 4.4.3.8
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.7/README.md` & `vector_vault-4.4.3.8/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/setup.py` & `vector_vault-4.4.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.3.7",
+    version="4.4.3.8",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.3.7/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3.8/vector_vault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.3.7
+Version: 4.4.3.8
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.7/vectorvault/ai.py` & `vector_vault-4.4.3.8/vectorvault/ai.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         'gpt-3.5-turbo': 16000,
         'gpt-3.5-turbo-0125': 16000,
         'gpt-3.5-turbo-16k': 16000,
         'gpt-4': 8000,
         'gpt-4-32k': 32000,
         'gpt-4-32k-0613': 32000,
         'gpt-4-1106-preview': 128000,
+        'gpt-4-turbo': 128000,
         'gpt-4-turbo-preview': 128000,
         'gpt-4-0125-preview': 128000,
     }
         
         self.main_prompt_with_context = """Use the following Context to answer the Question at the end. 
     Answer as if you were the modern voice of the context, without referencing the context or mentioning 
     the fact that any context has been given. Make sure to not just repeat what is referenced. Don't preface or give any warnings at the end.
```

### Comparing `vector_vault-4.4.3.7/vectorvault/cloud_api.py` & `vector_vault-4.4.3.8/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/cloudmanager.py` & `vector_vault-4.4.3.8/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/creds.py` & `vector_vault-4.4.3.8/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/download.py` & `vector_vault-4.4.3.8/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/itemize.py` & `vector_vault-4.4.3.8/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/tools_gpt.py` & `vector_vault-4.4.3.8/vectorvault/tools_gpt.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.7/vectorvault/vault.py` & `vector_vault-4.4.3.8/vectorvault/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -739,15 +739,15 @@
         '''
             Returns similar items from the Vault as the text you enter.
 
             Param `include_distances = True` adds the "distance" field to the return.
             The distance can be useful for assessing similarity differences in the items returned. 
             Each item has its' own distance number, and this changes the structure of the output.
         '''
-        return call_get_similar(self.user, vault if vault else self.vault, self.api, self.openai_key, text, n, include_distances=include_distances, verbose=self.verbose)
+        return call_get_similar(self.user, vault if vault else self.vault, self.api, self.openai_key, text, n, include_distances=include_distances, verbose=self.verbose, embeddings=self.embeddings_model)
 
 
     def add_item(self, text: str, meta: dict = None, name: str = None):
         """
             If your text length is greater than 15000 characters, you should use Vault.split_text(your_text) to 
             get a list of text segments that are the right size
         """
```

### Comparing `vector_vault-4.4.3.7/vectorvault/vecreq.py` & `vector_vault-4.4.3.8/vectorvault/vecreq.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,22 +54,23 @@
 
         format_executor = Formatter(wrapped_v, wrapped_x)
         return format_executor.execute()
     except Exception as e:
         raise Exception(f"HTTP error: {e}")
     
 
-def call_get_similar(user, vault, api_key, openai_key, text, num_items=4, include_distances=False, verbose=False):
+def call_get_similar(user, vault, api_key, openai_key, text, num_items=4, include_distances=False, verbose=False, embeddings=None):
     url = f"https://api.vectorvault.io/get_similar"
     payload = {
         'user': user,
         'vault': vault,
         'api_key': api_key,
         'openai_key': openai_key,
         'include_distances': include_distances,
+        'embeddings_model': embeddings,
         'text': text,
         'num_items': num_items
     }
     response = requests.post(url, json=payload)
     
     try:
         if verbose==True:
```

