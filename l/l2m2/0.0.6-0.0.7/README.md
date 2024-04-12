# Comparing `tmp/l2m2-0.0.6.tar.gz` & `tmp/l2m2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.6.tar", last modified: Fri Apr 12 01:21:42 2024, max compression
+gzip compressed data, was "l2m2-0.0.7.tar", last modified: Fri Apr 12 03:14:55 2024, max compression
```

## Comparing `l2m2-0.0.6.tar` & `l2m2-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.741205 l2m2-0.0.6/
--rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.6/LICENSE
--rw-r--r--   0 pierce     (503) staff       (20)     3619 2024-04-12 01:21:42.740925 l2m2-0.0.6/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)     3347 2024-04-12 01:20:04.000000 l2m2-0.0.6/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.739292 l2m2-0.0.6/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.6/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     5784 2024-04-12 01:19:14.000000 l2m2-0.0.6/l2m2/llm_client.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.740560 l2m2-0.0.6/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)     3619 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      226 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 01:21:42.000000 l2m2-0.0.6/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 01:21:42.741257 l2m2-0.0.6/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 01:21:15.000000 l2m2-0.0.6/setup.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 01:21:42.740296 l2m2-0.0.6/tests/
--rw-r--r--   0 pierce     (503) staff       (20)     4162 2024-04-12 01:19:45.000000 l2m2-0.0.6/tests/test_llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.404041 l2m2-0.0.7/
+-rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.7/LICENSE
+-rw-r--r--   0 pierce     (503) staff       (20)     3629 2024-04-12 03:14:55.403780 l2m2-0.0.7/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)     3357 2024-04-12 03:13:29.000000 l2m2-0.0.7/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.402640 l2m2-0.0.7/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.7/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     6578 2024-04-12 03:13:04.000000 l2m2-0.0.7/l2m2/llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.403554 l2m2-0.0.7/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)     3629 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      226 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 03:14:55.000000 l2m2-0.0.7/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 03:14:55.404083 l2m2-0.0.7/setup.cfg
+-rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 03:14:40.000000 l2m2-0.0.7/setup.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 03:14:55.403353 l2m2-0.0.7/tests/
+-rw-r--r--   0 pierce     (503) staff       (20)     4224 2024-04-12 03:01:46.000000 l2m2-0.0.7/tests/test_llm_client.py
```

### Comparing `l2m2-0.0.6/LICENSE` & `l2m2-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `l2m2-0.0.6/PKG-INFO` & `l2m2-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2m2
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cohere>=5.2.5
 Requires-Dist: openai>=1.17.0
 Requires-Dist: anthropic>=0.25.1
 Requires-Dist: groq>=0.5.0
 Requires-Dist: google-generativeai>=0.5.0
@@ -71,16 +71,16 @@
 `system_prompt` and `temperature` are optional, and default to `None` and `0.0` respectively.
 
 **List Available Models and Providers**
 
 These will return all valid models that can be passed into `call` and providers that can be passed into `add_provider`.
 
 ```python
-print(llms.get_available_models())
-print(llms.get_available_providers())
+print(LLMClient.get_available_models())
+print(LLMClient.get_available_providers())
 ```
 
 **List Active Models and Providers**
 
 These will only return models and providers added with `add_provider`.
 
 ```python
```

### Comparing `l2m2-0.0.6/README.md` & `l2m2-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,16 @@
 `system_prompt` and `temperature` are optional, and default to `None` and `0.0` respectively.
 
 **List Available Models and Providers**
 
 These will return all valid models that can be passed into `call` and providers that can be passed into `add_provider`.
 
 ```python
-print(llms.get_available_models())
-print(llms.get_available_providers())
+print(LLMClient.get_available_models())
+print(LLMClient.get_available_providers())
 ```
 
 **List Active Models and Providers**
 
 These will only return models and providers added with `add_provider`.
 
 ```python
```

### Comparing `l2m2-0.0.6/l2m2/llm_client.py` & `l2m2-0.0.7/l2m2/llm_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,89 +5,101 @@
 from groq import Groq
 
 
 _MODEL_INFO = {
     "gpt-4-turbo": {
         "provider": "openai",
         "model_id": "gpt-4-0125-preview",
+        "provider_homepage": "https://openai.com/product",
     },
     "gemini-1.5-pro": {
         "provider": "google",
         "model_id": "gemini-1.5-pro-latest",
+        "provider_homepage": "https://ai.google.dev/",
     },
     "gemini-1.0-pro": {
         "provider": "google",
         "model_id": "gemini-1.0-pro-latest",
+        "provider_homepage": "https://ai.google.dev/",
     },
     "claude-3-opus": {
         "provider": "anthropic",
         "model_id": "claude-3-opus-20240229",
+        "provider_homepage": "https://www.anthropic.com/api",
     },
     "claude-3-sonnet": {
         "provider": "anthropic",
         "model_id": "claude-3-sonnet-20240229",
+        "provider_homepage": "https://www.anthropic.com/api",
     },
     "claude-3-haiku": {
         "provider": "anthropic",
         "model_id": "claude-3-haiku-20240307",
+        "provider_homepage": "https://www.anthropic.com/api",
     },
     "command-r": {
         "provider": "cohere",
         "model_id": "command-r",
+        "provider_homepage": "https://docs.cohere.com/",
     },
     "command-r-plus": {
         "provider": "cohere",
         "model_id": "command-r-plus",
+        "provider_homepage": "https://docs.cohere.com/",
     },
     "llama2-70b": {
         "provider": "groq",
         "model_id": "llama2-70b-4096",
+        "provider_homepage": "https://wow.groq.com/",
     },
     "mixtral-8x7b": {
         "provider": "groq",
         "model_id": "mixtral-8x7b-32768",
+        "provider_homepage": "https://wow.groq.com/",
     },
     "gemma-7b": {
         "provider": "groq",
         "model_id": "gemma-7b-it",
+        "provider_homepage": "https://wow.groq.com/",
     },
 }
 
-_PROVIDERS = set([info["provider"] for info in _MODEL_INFO.values()])
-
 
 class LLMClient:
 
     def __init__(self):
         self.API_KEYS = {}
         self.active_providers = set()
         self.active_models = set()
 
-    def add_provider(self, provider, api_key):
-        if provider not in _PROVIDERS:
-            msg = f"Invalid provider: {provider}. Must be one of {_PROVIDERS}"
-            raise ValueError(msg)
+    @staticmethod
+    def get_available_providers():
+        return set([info["provider"] for info in _MODEL_INFO.values()])
 
-        self.API_KEYS[provider] = api_key
-        self.active_providers.add(provider)
-        self.active_models.update(
-            model for model, info in _MODEL_INFO.items() if info["provider"] == provider
-        )
+    @staticmethod
+    def get_available_models():
+        return set(_MODEL_INFO.keys())
 
     def get_active_providers(self):
         return set(self.active_providers)
 
     def get_active_models(self):
         return set(self.active_models)
 
-    def get_available_providers(self):
-        return set(_PROVIDERS)
+    def add_provider(self, provider, api_key):
+        providers = self.get_available_providers()
+        if provider not in providers:
+            msg = f"Invalid provider: {provider}. Must be one of {providers}"
+            raise ValueError(msg)
 
-    def get_available_models(self):
-        return set(_MODEL_INFO.keys())
+        self.API_KEYS[provider] = api_key
+        self.active_providers.add(provider)
+        self.active_models.update(
+            model for model, info in _MODEL_INFO.items() if info["provider"] == provider
+        )
 
     def remove_provider(self, provider):
         if provider not in self.active_providers:
             raise ValueError(f"Provider not active: {provider}")
 
         del self.API_KEYS[provider]
         self.active_providers.remove(provider)
@@ -104,67 +116,70 @@
                     + f" Please add provider {provider} to activate it."
                 )
                 raise ValueError(msg)
             else:
                 raise ValueError(f"Invalid model: {model}")
 
         model_info = _MODEL_INFO[model]
+        provider_method = getattr(self, f"_call_{model_info['provider']}", None)
+        return provider_method(model_info, prompt, temperature, system_prompt)
 
-        if model_info["provider"] == "openai":
-            oai = OpenAI(api_key=self.API_KEYS["openai"])
-            messages = [{"role": "user", "content": prompt}]
-            if system_prompt:
-                messages.insert(0, {"role": "system", "content": system_prompt})
-            result = oai.chat.completions.create(
-                model=model_info["model_id"],
-                messages=messages,
-                temperature=temperature,
-            )
-            return result.choices[0].message.content
+    def _call_openai(self, model_info, prompt, temperature, system_prompt):
+        oai = OpenAI(api_key=self.API_KEYS["openai"])
+        messages = [{"role": "user", "content": prompt}]
+        if system_prompt:
+            messages.insert(0, {"role": "system", "content": system_prompt})
+        result = oai.chat.completions.create(
+            model=model_info["model_id"],
+            messages=messages,
+            temperature=temperature,
+        )
+        return result.choices[0].message.content
 
-        elif model_info["provider"] == "anthropic":
-            anthr = Anthropic(api_key=self.API_KEYS["anthropic"])
-            result = anthr.messages.create(
-                model=model_info["model_id"],
-                max_tokens=1000,
-                temperature=temperature,
-                system=system_prompt,
-                messages=[{"role": "user", "content": prompt}],
-            )
-            return result.content[0].text
+    def _call_anthropic(self, model_info, prompt, temperature, system_prompt):
+        anthr = Anthropic(api_key=self.API_KEYS["anthropic"])
+        result = anthr.messages.create(
+            model=model_info["model_id"],
+            max_tokens=1000,
+            temperature=temperature,
+            system=system_prompt,
+            messages=[{"role": "user", "content": prompt}],
+        )
+        return result.content[0].text
 
-        elif model_info["provider"] == "cohere":
-            cohere = CohereClient(api_key=self.API_KEYS["cohere"])
-            result = cohere.chat(
-                model=model_info["model_id"],
-                message=prompt,
-                preamble=system_prompt,
-                temperature=temperature,
-            )
-            return result.text
+    def _call_cohere(self, model_info, prompt, temperature, system_prompt):
+        cohere = CohereClient(api_key=self.API_KEYS["cohere"])
+        result = cohere.chat(
+            model=model_info["model_id"],
+            message=prompt,
+            preamble=system_prompt,
+            temperature=temperature,
+        )
+        return result.text
+
+    def _call_groq(self, model_info, prompt, temperature, system_prompt):
+        groq = Groq(api_key=self.API_KEYS["groq"])
+        messages = [{"role": "user", "content": prompt}]
+        if system_prompt:
+            messages.insert(0, {"role": "system", "content": system_prompt})
+        result = groq.chat.completions.create(
+            model=model_info["model_id"],
+            messages=messages,
+            temperature=temperature,
+        )
+        return result.choices[0].message.content
 
-        elif model_info["provider"] == "groq":
-            groq = Groq(api_key=self.API_KEYS["groq"])
-            messages = [{"role": "user", "content": prompt}]
-            if system_prompt:
-                messages.insert(0, {"role": "system", "content": system_prompt})
-            result = groq.chat.completions.create(
-                model=model_info["model_id"],
-                messages=messages,
-                temperature=temperature,
+    def _call_google(self, model_info, prompt, temperature, system_prompt):
+        google.configure(api_key=self.API_KEYS["google"])
+
+        # Earlier versions don't support system prompts
+        if model_info["model_id"] not in ["gemini-1.5-pro-latest"]:
+            prompt = f"{system_prompt}\n{prompt}"
+            model = google.GenerativeModel(model_name=model_info["model_id"])
+        else:
+            model = google.GenerativeModel(
+                model_name=model_info["model_id"], system_instruction=system_prompt
             )
-            return result.choices[0].message.content
 
-        elif model_info["provider"] == "google":
-            print("here")
-            google.configure(api_key=self.API_KEYS["google"])
-            if model_info["model_id"] not in ["gemini-1.5-pro-latest"]:
-                prompt = f"{system_prompt}\n{prompt}"
-                model = google.GenerativeModel(model_name=model_info["model_id"])
-            else:
-                model = google.GenerativeModel(
-                    model_name=model_info["model_id"],
-                    system_instruction=system_prompt,
-                )
-            config = {"max_output_tokens": 2048, "temperature": temperature, "top_p": 1}
-            response = model.generate_content(prompt, generation_config=config)
-            return response.candidates[0].content.parts[0].text
+        config = {"max_output_tokens": 2048, "temperature": temperature, "top_p": 1}
+        response = model.generate_content(prompt, generation_config=config)
+        return response.candidates[0].content.parts[0].text
```

### Comparing `l2m2-0.0.6/l2m2.egg-info/PKG-INFO` & `l2m2-0.0.7/l2m2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2m2
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cohere>=5.2.5
 Requires-Dist: openai>=1.17.0
 Requires-Dist: anthropic>=0.25.1
 Requires-Dist: groq>=0.5.0
 Requires-Dist: google-generativeai>=0.5.0
@@ -71,16 +71,16 @@
 `system_prompt` and `temperature` are optional, and default to `None` and `0.0` respectively.
 
 **List Available Models and Providers**
 
 These will return all valid models that can be passed into `call` and providers that can be passed into `add_provider`.
 
 ```python
-print(llms.get_available_models())
-print(llms.get_available_providers())
+print(LLMClient.get_available_models())
+print(LLMClient.get_available_providers())
 ```
 
 **List Active Models and Providers**
 
 These will only return models and providers added with `add_provider`.
 
 ```python
```

### Comparing `l2m2-0.0.6/tests/test_llm_client.py` & `l2m2-0.0.7/tests/test_llm_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 def test_initialization(llm_client):
     assert llm_client.API_KEYS == {}
     assert llm_client.active_providers == set()
     assert llm_client.active_models == set()
 
 
 def test_add_provider_valid(llm_client):
-    with patch("l2m2.llm_client._PROVIDERS", new={"openai", "cohere"}):
+    with patch.object(
+        LLMClient, "get_available_providers", return_value={"openai", "cohere"}
+    ):
         llm_client.add_provider("openai", "test-key-openai")
         assert "openai" in llm_client.active_providers
         assert "gpt-4-turbo" in llm_client.active_models
 
 
 def test_add_provider_invalid(llm_client):
     with pytest.raises(ValueError):
         llm_client.add_provider("invalid_provider", "some-key")
 
 
 def test_remove_provider(llm_client):
-    with patch("l2m2.llm_client._PROVIDERS", new={"openai"}):
+    with patch.object(LLMClient, "get_available_providers", return_value={"openai"}):
         llm_client.add_provider("openai", "test-key-openai")
         llm_client.remove_provider("openai")
         assert "openai" not in llm_client.active_providers
         assert "gpt-4-turbo" not in llm_client.active_models
 
 
 def test_remove_provider_not_active(llm_client):
```

