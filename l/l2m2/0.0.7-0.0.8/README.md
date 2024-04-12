# Comparing `tmp/l2m2-0.0.7.tar.gz` & `tmp/l2m2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.7.tar", last modified: Fri Apr 12 03:14:55 2024, max compression
+gzip compressed data, was "l2m2-0.0.8.tar", last modified: Fri Apr 12 07:59:48 2024, max compression
```

## Comparing `l2m2-0.0.7.tar` & `l2m2-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.404041 l2m2-0.0.7/
--rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.7/LICENSE
--rw-r--r--   0 pierce     (503) staff       (20)     3629 2024-04-12 03:14:55.403780 l2m2-0.0.7/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)     3357 2024-04-12 03:13:29.000000 l2m2-0.0.7/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.402640 l2m2-0.0.7/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.7/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     6578 2024-04-12 03:13:04.000000 l2m2-0.0.7/l2m2/llm_client.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.403554 l2m2-0.0.7/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)     3629 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      226 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 03:14:55.404083 l2m2-0.0.7/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 03:14:40.000000 l2m2-0.0.7/setup.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.403353 l2m2-0.0.7/tests/
--rw-r--r--   0 pierce     (503) staff       (20)     4224 2024-04-12 03:01:46.000000 l2m2-0.0.7/tests/test_llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.495719 l2m2-0.0.8/
+-rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.8/LICENSE
+-rw-r--r--   0 pierce     (503) staff       (20)     5056 2024-04-12 07:59:48.495510 l2m2-0.0.8/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)     3163 2024-04-12 04:51:33.000000 l2m2-0.0.8/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.494117 l2m2-0.0.8/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.8/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     6578 2024-04-12 07:57:54.000000 l2m2-0.0.8/l2m2/llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.495037 l2m2-0.0.8/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)     5056 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      258 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)      755 2024-04-12 07:59:43.000000 l2m2-0.0.8/pyproject.toml
+-rw-r--r--   0 pierce     (503) staff       (20)       85 2024-04-12 00:57:10.000000 l2m2-0.0.8/requirements.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 07:59:48.495772 l2m2-0.0.8/setup.cfg
+-rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 07:47:38.000000 l2m2-0.0.8/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.494858 l2m2-0.0.8/tests/
+-rw-r--r--   0 pierce     (503) staff       (20)     4224 2024-04-12 03:01:46.000000 l2m2-0.0.8/tests/test_llm_client.py
```

### Comparing `l2m2-0.0.7/LICENSE` & `l2m2-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `l2m2-0.0.7/PKG-INFO` & `l2m2-0.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,10 @@
-Metadata-Version: 2.1
-Name: l2m2
-Version: 0.0.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: cohere>=5.2.5
-Requires-Dist: openai>=1.17.0
-Requires-Dist: anthropic>=0.25.1
-Requires-Dist: groq>=0.5.0
-Requires-Dist: google-generativeai>=0.5.0
+# L2M2: A Simple Python LLM Manager 💬👍
 
-# L2M2: Simple LLM Manager for Python
-
-[L2M2](https://pypi.org/project/l2m2/) ("LLM Manager" &rarr; "LLMM" &rarr; "L2M2") is a very simple LLM manager for Python.
+**[L2M2](https://pypi.org/project/l2m2/)** ("LLM Manager" &rarr; "LLMM" &rarr; "L2M2") is a very simple LLM manager for Python that allows you to expose lots of models through a single API. This is useful for evaluation, demos, and production LLM apps that use multiple models.
 
 ## Supported Models
 
 L2M2 currently supports the following models:
 
 | Provider                                     | Model Name        | Model Version              |
 | -------------------------------------------- | ----------------- | -------------------------- |
@@ -40,72 +29,54 @@
 ## Usage
 
 **Import the LLM Client**
 
 ```python
 from l2m2 import LLMClient
 
-llms = LLMClient()
+client = LLMClient()
 ```
 
 **Add a Provider**
 
-In order to activate any of the available models, you must add the provider of that model and pass in your API key for that provider's API. Make sure to use the provider name as shown in the table above.
+In order to activate any of the available models, you must add the provider of that model and pass in your API key for that provider's API. Make sure to pass in a valid provider as shown in the table above.
 
 ```python
-llms.add_provider("<provider name>", "<API key>")
+client.add_provider("<provider name>", "<API key>")
 ```
 
-**Call your LLM**
+**Call your LLM 💬👍**
 
-The `call` API is the same regardless of model or provider.
+The `call` API is the same regardless of model or provider. Make sure to pass in a valid model name as shown in the table above.
 
 ```python
-response = llms.call(
+response = client.call(
     system_prompt="<system prompt>",
     prompt="<prompt>",
     model="<model name>",
     temperature=<temperature>,
 )
 ```
 
 `system_prompt` and `temperature` are optional, and default to `None` and `0.0` respectively.
 
-**List Available Models and Providers**
-
-These will return all valid models that can be passed into `call` and providers that can be passed into `add_provider`.
-
-```python
-print(LLMClient.get_available_models())
-print(LLMClient.get_available_providers())
-```
-
-**List Active Models and Providers**
-
-These will only return models and providers added with `add_provider`.
-
-```python
-print(llms.get_active_models())
-print(llms.get_active_providers())
-```
-
 ### Example
 
 ```python
 import os
 from dotenv import load_dotenv
 from l2m2 import LLMClient
 
 load_dotenv()
 
 
-llms = LLMClient()
-llms.add_provider("openai", os.getenv("OAI_APIKEY"))
+client = LLMClient()
+client.add_provider("openai", os.getenv("OPENAI_API_KEY"))
 
-response = llms.call(
+response = client.call(
     system_prompt="Respond as if you were a pirate.",
     prompt="How's the weather today?",
     model="gpt-4-turbo",
     temperature=0.5,
 )
 
 print(response)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `l2m2-0.0.7/l2m2/llm_client.py` & `l2m2-0.0.8/l2m2/llm_client.py`

 * *Files identical despite different names*

### Comparing `l2m2-0.0.7/tests/test_llm_client.py` & `l2m2-0.0.8/tests/test_llm_client.py`

 * *Files identical despite different names*

