# Comparing `tmp/vector_vault-4.4.3.8.tar.gz` & `tmp/vector_vault-4.4.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-4.4.3.8.tar", last modified: Fri Apr 12 02:37:18 2024, max compression
+gzip compressed data, was "vector_vault-4.4.3.9.tar", last modified: Fri Apr 12 03:17:41 2024, max compression
```

## Comparing `vector_vault-4.4.3.8.tar` & `vector_vault-4.4.3.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.808434 vector_vault-4.4.3.8/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.8/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 02:37:18.808286 vector_vault-4.4.3.8/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.8/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-12 02:37:18.808472 vector_vault-4.4.3.8/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-12 02:37:13.000000 vector_vault-4.4.3.8/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.805340 vector_vault-4.4.3.8/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-12 02:37:18.000000 vector_vault-4.4.3.8/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 02:37:18.808134 vector_vault-4.4.3.8/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.8/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.3.8/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.8/vectorvault/cloud_api.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.3.8/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.8/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.8/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.8/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)    21194 2024-04-11 17:18:01.000000 vector_vault-4.4.3.8/vectorvault/tools_gpt.py
--rw-r--r--   0 johnrood   (501) staff       (20)    62687 2024-04-12 02:37:09.000000 vector_vault-4.4.3.8/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.3.8/vectorvault/vecreq.py
--rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.8/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 03:17:41.360415 vector_vault-4.4.3.9/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-4.4.3.9/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 03:17:41.360273 vector_vault-4.4.3.9/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    22680 2024-01-15 21:39:47.000000 vector_vault-4.4.3.9/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2024-04-12 03:17:41.360448 vector_vault-4.4.3.9/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1113 2024-04-12 03:16:18.000000 vector_vault-4.4.3.9/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 03:17:41.356420 vector_vault-4.4.3.9/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    23347 2024-04-12 03:17:41.000000 vector_vault-4.4.3.9/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      456 2024-04-12 03:17:41.000000 vector_vault-4.4.3.9/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2024-04-12 03:17:41.000000 vector_vault-4.4.3.9/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       88 2024-04-12 03:17:41.000000 vector_vault-4.4.3.9/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2024-04-12 03:17:41.000000 vector_vault-4.4.3.9/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2024-04-12 03:17:41.359946 vector_vault-4.4.3.9/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      171 2023-11-01 18:30:43.000000 vector_vault-4.4.3.9/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    16841 2024-04-12 02:24:53.000000 vector_vault-4.4.3.9/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     2119 2023-12-28 19:05:59.000000 vector_vault-4.4.3.9/vectorvault/cloud_api.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6046 2024-04-11 19:12:06.000000 vector_vault-4.4.3.9/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1883 2024-04-11 18:02:55.000000 vector_vault-4.4.3.9/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      707 2023-11-29 18:24:09.000000 vector_vault-4.4.3.9/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3871 2024-04-11 17:18:09.000000 vector_vault-4.4.3.9/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    22426 2024-04-12 03:17:31.000000 vector_vault-4.4.3.9/vectorvault/tools_gpt.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    62687 2024-04-12 02:37:09.000000 vector_vault-4.4.3.9/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     5421 2024-04-12 02:36:29.000000 vector_vault-4.4.3.9/vectorvault/vecreq.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      399 2023-06-08 04:36:04.000000 vector_vault-4.4.3.9/vectorvault/wrap.py
```

### Comparing `vector_vault-4.4.3.8/LICENSE` & `vector_vault-4.4.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/PKG-INFO` & `vector_vault-4.4.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 4.4.3.8
+Version: 4.4.3.9
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.8/README.md` & `vector_vault-4.4.3.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/setup.py` & `vector_vault-4.4.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="4.4.3.8",
+    version="4.4.3.9",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-4.4.3.8/vector_vault.egg-info/PKG-INFO` & `vector_vault-4.4.3.9/vector_vault.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 4.4.3.8
+Version: 4.4.3.9
 Summary: Quickly create ChatGPT RAG apps and Unleash the full potential of GenAI with Vector Vault
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vector_vault-4.4.3.8/vectorvault/ai.py` & `vector_vault-4.4.3.9/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/cloud_api.py` & `vector_vault-4.4.3.9/vectorvault/cloud_api.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/cloudmanager.py` & `vector_vault-4.4.3.9/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/creds.py` & `vector_vault-4.4.3.9/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/download.py` & `vector_vault-4.4.3.9/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/itemize.py` & `vector_vault-4.4.3.9/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/tools_gpt.py` & `vector_vault-4.4.3.9/vectorvault/tools_gpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .ai import AI
-import time
 import ast
+import queue
+import threading
 
 '''
     ToolsGPT is a set of tools special to large language models. 
     Every tool turns unstructured data into structured data.
     
     Structure data is required to run programs. 
     Unstructured data is the primary human output.
@@ -40,17 +41,18 @@
             -> out: (list of exact matches -> list type)
 
         6. `get_topic`:
             Useful to classify the topic of conversation
 '''
 
 class ToolsGPT():
-    def __init__(self, verbose=False):
+    def __init__(self, verbose=False, timeout=300):
         self.verbose = verbose
         self.llm = AI(verbose=verbose).llm
+        self.timeout = timeout
 
 
     def get_rating(self, text: str = None, concept_to_rate_for: str = None, model='gpt-3.5-turbo', loop_limit=20) -> int:
         '''
             Get a numeric rating out of 10. Input plain text, and concept to rate for. Defualts to 'quality'
             Output is integer. Leave no text and pass concept only to format custom
         '''
@@ -141,76 +143,76 @@
             answer = self.isolate_yes_no(answer)
             print(f"Y/N Answer {loops}: {answer}") if self.verbose else 0
             loops += 1
 
         return answer
 
 
-    def get_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4) -> str:
+    def get_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4, timeout=None) -> str:
         '''
         This function can be used in a variety of Natural Language Processing (NLP) tasks, 
         such as text classification or intent recognition.
 
         Classify any text input to a single option contained in a list of options. - Returns exact match to one of items on list.
         Input text, and list of options: ["list of options", "is a list of strings", "do not forget"]
         '''
 
         list_copy = []
         for option in list_of_options:
             list_copy.append(option.strip().replace('.', '').lower().strip('"').strip("'"))
         prompt = f"""Respond with one of the options on this list: {list_copy} 
 Content to classify: "{text}"  \n\nDo not respond with anything other than the option on the list. Do not add any additional spaces or characters other than the label: {list_copy}"""
 
-        answer = self.retry_llm(prompt, model, loop_limit)
+        answer = self.retry_llm(prompt, model, loop_limit, timeout=timeout)
 
         print(f'''Get Answer: {answer}''') if self.verbose else 0
 
         final = None
         temp = 0
 
         while not final:
             if answer is not None:
                 try:
                     try:
                         new_answer = list_of_options[list_copy.index(answer)]  # return original answer
                         final = True
                     except:
                         temp += .2 if temp < .7 else 0
-                        answer = self.retry_llm(prompt, model, loop_limit, temperature=temp)
+                        answer = self.retry_llm(prompt, model, loop_limit, temperature=temp, timeout=timeout)
                 except:
                     pass
 
         return new_answer
 
 
-    def get_multi_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4) -> str:
+    def get_multi_match(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4, timeout=None) -> str:
         '''
         This function can be used in a variety of Natural Language Processing (NLP) tasks, 
         such as text classification or intent recognition.
 
         Classify any text input to a single option contained in a list of options. - Returns exact match to one of items on list.
         Input text, and list of options: ["list of options", "is a list of strings", "do not forget"]
         '''
         prompt = f"""Respond with a list of items from this list: {list_of_options} 
 Content to classify: "{text}"  \n\n Respond with a subset list that matches the content: {list_of_options}"""
 
         # Simulate a call to a function that retries a language model query
-        answer = self.retry_llm(prompt, model, loop_limit)
+        answer = self.retry_llm(prompt, model, loop_limit, timeout=timeout)
 
         # Logging for debug purposes
         print(f'''Get Answer: {answer}''') if self.verbose else None
         print(ast.literal_eval(answer)) if self.verbose else None
 
         # Process the answer, directly adding matches, and using get_match for others
         processed_results = []
         for i in ast.literal_eval(answer):
             if i in list_of_options:
                 processed_results.append(i)
             else:
-                processed_results.append(self.get_match(i, list_of_options, model, loop_limit))
+                processed_results.append(self.get_match(i, list_of_options, model, loop_limit, timeout))
         
         return processed_results
 
 
     def get_topic(self, text: str, list_of_options: list, model='gpt-3.5-turbo', loop_limit=4) -> str:
         '''
         Like get_match, default optimized for topic recognition
@@ -384,24 +386,47 @@
 
         prompt = prompt_template.format(content=content)
 
         return self.retry_llm(custom_prompt=prompt, model=model)
 
 
     # This function is called by the others to handle retries:
-    def retry_llm(self, custom_prompt, model='gpt-3.5-turbo', loop_limit=2, temperature=0):
+    def retry_llm(self, custom_prompt, model='gpt-3.5-turbo', loop_limit=2, temperature=0, timeout=None):
         for i in range(loop_limit):
             try:
-                return self.llm(custom_prompt=custom_prompt, model=model, temperature=temperature).strip().replace('.', '').lower().strip('"').strip("'")
+                response_queue = queue.Queue()
+                def call_llm(response_queue, prompt, model, temperature):
+                    try:
+                        response = self.llm(custom_prompt=prompt, model=model, temperature=temperature)
+                        response_queue.put(response)
+                    except Exception as e:
+                        response_queue.put(e)
+
+                # Create and start the thread to call the LLM
+                thread = threading.Thread(target=call_llm, args=(response_queue, custom_prompt, model, temperature))
+                thread.start()
+
+                # Wait for the response with a timeout
+                timeout = self.timeout if timeout is None else timeout
+                try:
+                    response = response_queue.get(timeout=timeout)
+                    if isinstance(response, Exception):
+                        raise response
+                    return response.strip().replace('.', '').lower().strip('"').strip("'")
+                except queue.Empty:
+                    print(f"Attempt {i+1}: Request timed out. Retrying...")
+                    continue  # Continue to retry until loop_limit is reached
+
             except Exception as e:
                 if i < loop_limit - 1:  # i is zero indexed
-                    time.sleep(5)  # wait 5 seconds before trying again
                     print(f"Attempt {i+1} failed with error: {str(e)}. Retrying...")
                 else:
-                    raise f"Attempt {i+1} failed with error: {str(e)}. No more retries."
+                    print(f"Final attempt {i+1} failed with error: {str(e)}. No more retries.")
+                    raise e  # Optionally, re-raise the exception or handle it accordingly
+
 
 
     def perfect(self, content, instructions: str, model='gpt-3.5-turbo'):
         '''Wrapper function ensures that you get exactly what you wanted, and will not return until you get what you wanted'''
         output = self.get_yes_no(model=model, text=f"These are the instructions: {instructions} and this is the Output: {content}", 
                     question=f"Does the output match the instructions?", ) == 'no'
```

### Comparing `vector_vault-4.4.3.8/vectorvault/vault.py` & `vector_vault-4.4.3.9/vectorvault/vault.py`

 * *Files identical despite different names*

### Comparing `vector_vault-4.4.3.8/vectorvault/vecreq.py` & `vector_vault-4.4.3.9/vectorvault/vecreq.py`

 * *Files identical despite different names*

