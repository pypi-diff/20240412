# Comparing `tmp/tuneapi-0.2.7.tar.gz` & `tmp/tuneapi-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.7.tar", max compression
+gzip compressed data, was "tuneapi-0.2.8.tar", max compression
```

## Comparing `tuneapi-0.2.7.tar` & `tuneapi-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.7/README.md
--rw-r--r--   0        0        0      696 2024-04-09 05:56:27.169497 tuneapi-0.2.7/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-09 05:56:19.006229 tuneapi-0.2.7/tuneapi/__init__.py
--rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.7/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6712 2024-04-09 05:54:45.329815 tuneapi-0.2.7/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.7/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.7/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      659 2024-04-07 20:07:56.771955 tuneapi-0.2.7/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.7/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.7/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.7/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.7/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.7/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.7/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.7/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.2.7/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.7/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.7/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.7/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.7/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.7/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.7/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.8/README.md
+-rw-r--r--   0        0        0      696 2024-04-12 08:21:20.179027 tuneapi-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-12 08:21:15.818709 tuneapi-0.2.8/tuneapi/__init__.py
+-rw-r--r--   0        0        0      230 2024-04-12 08:19:21.664606 tuneapi-0.2.8/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6710 2024-04-12 08:20:50.001225 tuneapi-0.2.8/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     3064 2024-04-12 08:08:55.997351 tuneapi-0.2.8/tuneapi/apis/model_grok.py
+-rw-r--r--   0        0        0     3082 2024-04-12 08:19:03.799303 tuneapi-0.2.8/tuneapi/apis/model_mistral.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.8/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5519 2024-04-12 08:20:35.218980 tuneapi-0.2.8/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      659 2024-04-07 20:07:56.771955 tuneapi-0.2.8/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.8/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.8/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.8/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.8/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.8/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.8/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.8/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3712 2024-04-07 20:01:31.642080 tuneapi-0.2.8/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.8/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.8/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.8/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.8/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.8/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.8/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.8/PKG-INFO
```

### Comparing `tuneapi-0.2.7/pyproject.toml` & `tuneapi-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.7"
+version = "0.2.8"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.2.7/tuneapi/apis/model_anthropic.py` & `tuneapi-0.2.8/tuneapi/apis/model_anthropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from tuneapi.utils import ENV, SimplerTimes as stime, from_json, to_json
 from tuneapi.types import Thread, human, Message
 
 
 class Anthropic:
     def __init__(self, model: Optional[str] = "claude-3-haiku-20240307"):
         self.anthropic_model = model
-        self.anthropic_token = ENV.ANTHROPIC_TOKEN("")
+        self.anthropic_api_token = ENV.ANTHROPIC_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
-        self.anthropic_token = token
+        self.anthropic_api_token = token
 
     def tool_to_claude_xml(self, tool):
         tool_signature = ""
         if len(tool["parameters"]) > 0:
             for name, p in tool["parameters"]["properties"].items():
                 param = f"""<parameter>
                 <name> {name} </name>
@@ -43,33 +43,33 @@
             "</tool_description>"
         )
         return constructed_prompt
 
     def _process_input(
         self, chats, tools: Optional[List] = None, token: Optional[str] = None
     ):
-        if not token and not self.anthropic_token:  # type: ignore
+        if not token and not self.anthropic_api_token:  # type: ignore
             raise Exception(
-                "Anthropic API key not found. Please set ANTHROPIC_TOKEN environment variable or pass through function"
+                "Please set ANTHROPIC_TOKEN environment variable or pass through function"
             )
-        token = token or self.anthropic_token
+        token = token or self.anthropic_api_token
         if isinstance(chats, Thread):
             messages = chats.to_dict()["chats"]
         elif isinstance(chats, str):
             messages = Thread(human(chats)).to_dict()["chats"]
         else:
             messages = chats
 
         # create the anthropic style data
         system = ""
         claude_messages = []
         if messages[0]["role"] == Message.SYSTEM:
-            system = messages[0]["content"]
-        start_idx = 1 if system else 0
-        for m in messages[start_idx:]:
+            system_message = messages.pop(0)
+            system = system_message["content"]
+        for m in messages:
             role = m["role"]
             if m["role"] == Message.HUMAN:
                 role = "user"
             content = m["content"]
             if type(content) == str:
                 content = [{"type": "text", "text": content.strip()}]
             claude_messages.append(
@@ -140,23 +140,23 @@
         max_tokens: int = 1024,
         temperature: float = 1,
         token: Optional[str] = None,
         timeout=(5, 60),
         raw: bool = False,
         **kwargs,
     ) -> Any:
-        headers, system, messages = self._process_input(
+        headers, system, claude_messages = self._process_input(
             chats=chats,
             tools=tools,
             token=token,
         )
         data = {
             "model": model or self.anthropic_model,
             "max_tokens": max_tokens,
-            "messages": messages,
+            "messages": claude_messages,
             "temperature": temperature,
             "system": system,
             "stream": True,
             **kwargs,
         }
         r = requests.post(
             "https://api.anthropic.com/v1/messages",
```

### Comparing `tuneapi-0.2.7/tuneapi/apis/model_openai.py` & `tuneapi-0.2.8/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/apis/model_tune.py` & `tuneapi-0.2.8/tuneapi/apis/model_tune.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from tuneapi.types import Thread, human, Message
 
 
 class TuneModel:
     """Defines the model used in tune.app. See [Tune Studio](https://studio.tune.app/) for more information."""
 
     def __init__(self, id: Optional[str] = "rohan/mixtral-8x7b-inst-v0-1-32k"):
-        self._tune_model_id = id
+        self.tune_model_id = id
         self.tune_api_token = ENV.TUNEAPI_TOKEN("")
 
     def set_api_token(self, token: str) -> None:
         self.tune_api_token = token
 
     def _process_input(self, chats, token: Optional[str] = None):
         if not token and not self.tune_api_token:  # type: ignore
@@ -63,15 +63,15 @@
             Dict[str, Any]: The response from the API
         """
         _st = stime.get_now_float()
         headers, messages = self._process_input(chats, token)
         data = {
             "temperature": temperature,
             "messages": messages,
-            "model": model or self._tune_model_id,
+            "model": model or self.tune_model_id,
             "stream": False,
             "max_tokens": max_tokens,
         }
         response = requests.post(
             "https://proxy.tune.app/chat/completions",
             headers=headers,
             json=data,
```

### Comparing `tuneapi-0.2.7/tuneapi/apis/threads.py` & `tuneapi-0.2.8/tuneapi/apis/threads.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/types/chats.py` & `tuneapi-0.2.8/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/__init__.py` & `tuneapi-0.2.8/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/fs.py` & `tuneapi-0.2.8/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/logger.py` & `tuneapi-0.2.8/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/mime.py` & `tuneapi-0.2.8/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/misc.py` & `tuneapi-0.2.8/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/networking.py` & `tuneapi-0.2.8/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/parallel.py` & `tuneapi-0.2.8/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/serdeser.py` & `tuneapi-0.2.8/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/subway.py` & `tuneapi-0.2.8/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/tuneapi/utils/terminal.py` & `tuneapi-0.2.8/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.7/PKG-INFO` & `tuneapi-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.7
+Version: 0.2.8
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

