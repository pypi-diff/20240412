# Comparing `tmp/openaichatlib-1.0.4.tar.gz` & `tmp/openaichatlib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openaichatlib-1.0.4.tar", last modified: Sun Mar 31 03:02:32 2024, max compression
+gzip compressed data, was "openaichatlib-1.0.5.tar", last modified: Fri Apr 12 01:55:13 2024, max compression
```

## Comparing `openaichatlib-1.0.4.tar` & `openaichatlib-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-03-31 03:02:32.544312 openaichatlib-1.0.4/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/LICENSE
--rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-03-31 03:02:32.543923 openaichatlib-1.0.4/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/README.md
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-03-31 03:02:32.539927 openaichatlib-1.0.4/openaichatlib/
--rw-r--r--   0 chenshuai   (501) staff       (20)    63458 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/openaichatlib/V1.py
--rw-r--r--   0 chenshuai   (501) staff       (20)    18114 2024-03-31 03:00:17.000000 openaichatlib-1.0.4/openaichatlib/V3.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      886 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/openaichatlib/__init__.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     4805 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/openaichatlib/typings.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     2667 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/openaichatlib/utils.py
--rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-03-30 14:32:45.000000 openaichatlib-1.0.4/openaichatlib/version.py
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-03-31 03:02:32.543424 openaichatlib-1.0.4/openaichatlib.egg-info/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-03-31 03:02:32.000000 openaichatlib-1.0.4/openaichatlib.egg-info/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      349 2024-03-31 03:02:32.000000 openaichatlib-1.0.4/openaichatlib.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-03-31 03:02:32.000000 openaichatlib-1.0.4/openaichatlib.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       90 2024-03-31 03:02:32.000000 openaichatlib-1.0.4/openaichatlib.egg-info/requires.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-03-31 03:02:32.000000 openaichatlib-1.0.4/openaichatlib.egg-info/top_level.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-03-31 03:02:32.544403 openaichatlib-1.0.4/setup.cfg
--rw-r--r--   0 chenshuai   (501) staff       (20)     1237 2024-03-31 03:01:12.000000 openaichatlib-1.0.4/setup.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.821527 openaichatlib-1.0.5/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.5/LICENSE
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-04-12 01:55:13.820964 openaichatlib-1.0.5/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.5/README.md
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.817033 openaichatlib-1.0.5/openaichatlib/
+-rw-r--r--   0 chenshuai   (501) staff       (20)    63458 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/V1.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)    18400 2024-04-12 01:52:23.000000 openaichatlib-1.0.5/openaichatlib/V3.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      886 2023-11-08 06:33:39.000000 openaichatlib-1.0.5/openaichatlib/__init__.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     4805 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/typings.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     2667 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/utils.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)       18 2023-11-08 06:24:35.000000 openaichatlib-1.0.5/openaichatlib/version.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-12 01:55:13.820221 openaichatlib-1.0.5/openaichatlib.egg-info/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1419 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      349 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       90 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/requires.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-12 01:55:13.000000 openaichatlib-1.0.5/openaichatlib.egg-info/top_level.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-12 01:55:13.821653 openaichatlib-1.0.5/setup.cfg
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1237 2024-04-12 01:54:50.000000 openaichatlib-1.0.5/setup.py
```

### Comparing `openaichatlib-1.0.4/LICENSE` & `openaichatlib-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/PKG-INFO` & `openaichatlib-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.4
+Version: 1.0.5
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.4/README.md` & `openaichatlib-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/openaichatlib/V1.py` & `openaichatlib-1.0.5/openaichatlib/V1.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/openaichatlib/V3.py` & `openaichatlib-1.0.5/openaichatlib/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 A simple wrapper for the official ChatGPT API
 """
 import json
 import os
 from pathlib import Path
 from typing import AsyncGenerator
+from typing import Optional
 
 import httpx
 import requests
 import tiktoken
 
 from . import typings as t
 from .utils import get_filtered_keys_from_object
@@ -92,23 +93,25 @@
         temperature: float = 0.5,
         top_p: float = 1.0,
         presence_penalty: float = 0.0,
         frequency_penalty: float = 0.0,
         reply_count: int = 1,
         truncate_limit: int = None,
         system_prompt: str = "You are ChatGPT, a large language model trained by OpenAI. Respond conversationally",
+        count_tokens: bool = True,
     ) -> None:
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.api_url: str = api_url
         self.engine: str = engine
         self.api_key: str = api_key
         self.customize_header = customize_header
         self.system_prompt: str = system_prompt
+        self.count_tokens = count_tokens
         self.max_tokens: int = max_tokens or (
             16_000
             if engine in ENGINES_GPT35_TURBO
             else 120_000
             if engine in ENGINES_PREVIEW
             else 32_000
             if engine in ENGINES_GPT4_32K
@@ -188,14 +191,16 @@
         """
         self.conversation[convo_id].append({"role": role, "content": message})
 
     def __truncate_conversation(self, convo_id: str = "default") -> None:
         """
         Truncate the conversation
         """
+        if not self.count_tokens:
+            return
         if self.engine in ENGINES_CLAUDE:
             return
         while True:
             if (
                 self.get_token_count(convo_id) > self.truncate_limit
                 and len(self.conversation[convo_id]) > 1
             ):
@@ -205,14 +210,16 @@
                 break
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
+        if not self.count_tokens:
+            return 0
         if self.engine not in ENGINES:
             raise NotImplementedError(
                 f"Engine {self.engine} is not supported. Select from {ENGINES}",
             )
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
@@ -231,18 +238,20 @@
                         except Exception as e:
                             print(f"Warning: error count token type: {e}")
                 if key == "name":  # if there's a name, the role is omitted
                     num_tokens += 5  # role is always required and always 1 token
         num_tokens += 5  # every reply is primed with <im_start>assistant
         return num_tokens
 
-    def get_max_tokens(self, convo_id: str) -> int:
+    def get_max_tokens(self, convo_id: str) -> Optional[int]:
         """
         Get max tokens
         """
+        if not self.count_tokens:
+            return None
         if self.engine in ENGINES_GPT35_TURBO or self.engine in ENGINES_PREVIEW or self.engine in ENGINES_CLAUDE:
             return 4096
         return self.max_tokens - self.get_token_count(convo_id)
 
     def ask_stream(
         self,
         prompt,
@@ -290,19 +299,18 @@
             ),
             "frequency_penalty": kwargs.get(
                 "frequency_penalty",
                 self.frequency_penalty,
             ),
             "n": kwargs.get("n", self.reply_count),
             "user": role,
-            "max_tokens": min(
-                self.get_max_tokens(convo_id=convo_id),
-                kwargs.get("max_tokens", self.max_tokens),
-            ),
         }
+        max_tokens = kwargs.get("max_tokens", None) or self.get_max_tokens(convo_id=convo_id)
+        if max_tokens:
+            payload["max_tokens"] = max_tokens
         if json_format:
             payload["response_format"] = {
                 "type": "json_object"
             }
         if self.customize_header:
             headers.update(self.customize_header)
         response = self.session.post(
@@ -380,19 +388,18 @@
             ),
             "frequency_penalty": kwargs.get(
                 "frequency_penalty",
                 self.frequency_penalty,
             ),
             "n": kwargs.get("n", self.reply_count),
             "user": role,
-            "max_tokens": min(
-                self.get_max_tokens(convo_id=convo_id),
-                kwargs.get("max_tokens", self.max_tokens),
-            ),
         }
+        max_tokens = kwargs.get("max_tokens", None) or self.get_max_tokens(convo_id=convo_id)
+        if max_tokens:
+            payload["max_tokens"] = max_tokens
         if json_format:
             payload["response_format"] = {
                 "type": "json_object"
             }
         headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         if self.customize_header:
             headers.update(self.customize_header)
```

### Comparing `openaichatlib-1.0.4/openaichatlib/__init__.py` & `openaichatlib-1.0.5/openaichatlib/__init__.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/openaichatlib/typings.py` & `openaichatlib-1.0.5/openaichatlib/typings.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/openaichatlib/utils.py` & `openaichatlib-1.0.5/openaichatlib/utils.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.4/openaichatlib.egg-info/PKG-INFO` & `openaichatlib-1.0.5/openaichatlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.4
+Version: 1.0.5
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.4/setup.py` & `openaichatlib-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "rich",
     "tiktoken>=0.3.0",
     "openai",
 ]
 
 setup(
     name="openaichatlib",
-    version="1.0.4",
+    version="1.0.5",
     description="OpenAI Chat API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IAn2018cs/OpenAIChatLib",
     author="IAn2018",
     author_email="ian2018cs@gmail.com",
     classifiers=[
```

