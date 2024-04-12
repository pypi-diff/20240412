# Comparing `tmp/l2m2-0.0.5.tar.gz` & `tmp/l2m2-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.5.tar", last modified: Thu Apr 11 22:43:09 2024, max compression
+gzip compressed data, was "l2m2-0.0.6.tar", last modified: Fri Apr 12 01:21:42 2024, max compression
```

## Comparing `l2m2-0.0.5.tar` & `l2m2-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:43:09.039595 l2m2-0.0.5/
--rw-r--r--   0 pierce     (503) staff       (20)      411 2024-04-11 22:43:09.039386 l2m2-0.0.5/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      203 2024-04-11 22:35:34.000000 l2m2-0.0.5/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:43:09.038245 l2m2-0.0.5/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       35 2024-04-11 20:10:27.000000 l2m2-0.0.5/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     4365 2024-04-11 20:09:11.000000 l2m2-0.0.5/l2m2/llm_manager.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-11 22:43:09.039162 l2m2-0.0.5/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)      411 2024-04-11 22:43:09.000000 l2m2-0.0.5/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      194 2024-04-11 22:43:09.000000 l2m2-0.0.5/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-11 22:43:09.000000 l2m2-0.0.5/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       59 2024-04-11 22:43:09.000000 l2m2-0.0.5/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-11 22:43:09.000000 l2m2-0.0.5/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-11 22:43:09.039640 l2m2-0.0.5/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      357 2024-04-11 22:42:10.000000 l2m2-0.0.5/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.741205 l2m2-0.0.6/
+-rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.6/LICENSE
+-rw-r--r--   0 pierce     (503) staff       (20)     3619 2024-04-12 01:21:42.740925 l2m2-0.0.6/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)     3347 2024-04-12 01:20:04.000000 l2m2-0.0.6/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.739292 l2m2-0.0.6/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.6/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     5784 2024-04-12 01:19:14.000000 l2m2-0.0.6/l2m2/llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.740560 l2m2-0.0.6/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)     3619 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      226 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 01:21:42.741257 l2m2-0.0.6/setup.cfg
+-rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 01:21:15.000000 l2m2-0.0.6/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.740296 l2m2-0.0.6/tests/
+-rw-r--r--   0 pierce     (503) staff       (20)     4162 2024-04-12 01:19:45.000000 l2m2-0.0.6/tests/test_llm_client.py
```

### Comparing `l2m2-0.0.5/l2m2/llm_manager.py` & `l2m2-0.0.6/l2m2/llm_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,27 @@
+import google.generativeai as google
 from cohere import Client as CohereClient
 from openai import OpenAI
 from anthropic import Anthropic
 from groq import Groq
 
 
 _MODEL_INFO = {
     "gpt-4-turbo": {
         "provider": "openai",
         "model_id": "gpt-4-0125-preview",
     },
+    "gemini-1.5-pro": {
+        "provider": "google",
+        "model_id": "gemini-1.5-pro-latest",
+    },
+    "gemini-1.0-pro": {
+        "provider": "google",
+        "model_id": "gemini-1.0-pro-latest",
+    },
     "claude-3-opus": {
         "provider": "anthropic",
         "model_id": "claude-3-opus-20240229",
     },
     "claude-3-sonnet": {
         "provider": "anthropic",
         "model_id": "claude-3-sonnet-20240229",
@@ -42,24 +51,25 @@
         "model_id": "gemma-7b-it",
     },
 }
 
 _PROVIDERS = set([info["provider"] for info in _MODEL_INFO.values()])
 
 
-class LLMManager:
+class LLMClient:
 
     def __init__(self):
         self.API_KEYS = {}
         self.active_providers = set()
         self.active_models = set()
 
     def add_provider(self, provider, api_key):
         if provider not in _PROVIDERS:
-            raise ValueError(f"Invalid provider: {provider}")
+            msg = f"Invalid provider: {provider}. Must be one of {_PROVIDERS}"
+            raise ValueError(msg)
 
         self.API_KEYS[provider] = api_key
         self.active_providers.add(provider)
         self.active_models.update(
             model for model, info in _MODEL_INFO.items() if info["provider"] == provider
         )
 
@@ -83,17 +93,25 @@
         self.active_providers.remove(provider)
         self.active_models.difference_update(
             model for model, info in _MODEL_INFO.items() if info["provider"] == provider
         )
 
     def call(self, *, prompt, model, temperature=0.0, system_prompt=None):
         if model not in self.active_models:
-            raise ValueError(f"Invalid model: {model}")
+            if model in self.get_available_models():
+                provider = _MODEL_INFO[model]["provider"]
+                msg = (
+                    f"Model {model} is available, but not active."
+                    + f" Please add provider {provider} to activate it."
+                )
+                raise ValueError(msg)
+            else:
+                raise ValueError(f"Invalid model: {model}")
 
-        model_info = self._MODEL_INFO[model]
+        model_info = _MODEL_INFO[model]
 
         if model_info["provider"] == "openai":
             oai = OpenAI(api_key=self.API_KEYS["openai"])
             messages = [{"role": "user", "content": prompt}]
             if system_prompt:
                 messages.insert(0, {"role": "system", "content": system_prompt})
             result = oai.chat.completions.create(
@@ -131,7 +149,22 @@
                 messages.insert(0, {"role": "system", "content": system_prompt})
             result = groq.chat.completions.create(
                 model=model_info["model_id"],
                 messages=messages,
                 temperature=temperature,
             )
             return result.choices[0].message.content
+
+        elif model_info["provider"] == "google":
+            print("here")
+            google.configure(api_key=self.API_KEYS["google"])
+            if model_info["model_id"] not in ["gemini-1.5-pro-latest"]:
+                prompt = f"{system_prompt}\n{prompt}"
+                model = google.GenerativeModel(model_name=model_info["model_id"])
+            else:
+                model = google.GenerativeModel(
+                    model_name=model_info["model_id"],
+                    system_instruction=system_prompt,
+                )
+            config = {"max_output_tokens": 2048, "temperature": temperature, "top_p": 1}
+            response = model.generate_content(prompt, generation_config=config)
+            return response.candidates[0].content.parts[0].text
```

