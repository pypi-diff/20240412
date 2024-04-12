# Comparing `tmp/pyaskit-1.4.1.tar.gz` & `tmp/pyaskit-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaskit-1.4.1.tar", last modified: Sat Mar  9 02:38:51 2024, max compression
+gzip compressed data, was "pyaskit-1.4.2.tar", last modified: Fri Apr 12 04:36:27 2024, max compression
```

## Comparing `pyaskit-1.4.1.tar` & `pyaskit-1.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 02:38:51.878229 pyaskit-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-09 02:38:37.000000 pyaskit-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19303 2024-03-09 02:38:51.878229 pyaskit-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15879 2024-03-09 02:38:37.000000 pyaskit-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 02:38:51.878229 pyaskit-1.4.1/pyaskit/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/function_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm_claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm_cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm_gemini.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm_llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/llm_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/py_askit.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 02:38:51.878229 pyaskit-1.4.1/pyaskit/types/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/types/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/types/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/types/type_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-03-09 02:38:37.000000 pyaskit-1.4.1/pyaskit/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 02:38:51.878229 pyaskit-1.4.1/pyaskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19303 2024-03-09 02:38:51.000000 pyaskit-1.4.1/pyaskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-09 02:38:51.000000 pyaskit-1.4.1/pyaskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 02:38:51.000000 pyaskit-1.4.1/pyaskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-09 02:38:51.000000 pyaskit-1.4.1/pyaskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-09 02:38:51.000000 pyaskit-1.4.1/pyaskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 02:38:51.878229 pyaskit-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-09 02:38:37.000000 pyaskit-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:36:27.190403 pyaskit-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 04:36:18.000000 pyaskit-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-12 04:36:27.190403 pyaskit-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15906 2024-04-12 04:36:18.000000 pyaskit-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:36:27.186403 pyaskit-1.4.2/pyaskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7993 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/function_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm_claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm_cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm_llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/llm_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/py_askit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:36:27.190403 pyaskit-1.4.2/pyaskit/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/types/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/types/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/types/type_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-12 04:36:18.000000 pyaskit-1.4.2/pyaskit/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:36:27.190403 pyaskit-1.4.2/pyaskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-12 04:36:26.000000 pyaskit-1.4.2/pyaskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 04:36:27.000000 pyaskit-1.4.2/pyaskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:36:26.000000 pyaskit-1.4.2/pyaskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 04:36:26.000000 pyaskit-1.4.2/pyaskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 04:36:26.000000 pyaskit-1.4.2/pyaskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 04:36:27.190403 pyaskit-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-12 04:36:18.000000 pyaskit-1.4.2/setup.py
```

### Comparing `pyaskit-1.4.1/LICENSE` & `pyaskit-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/PKG-INFO` & `pyaskit-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaskit
-Version: 1.4.1
+Version: 1.4.2
 Summary: AskIt: Unified programming interface for programming with large language models (GPT-3.5, GPT-4, Gemini, Claude, COHERE, Llama 2)
 Home-page: https://github.com/katsumiok/pyaskit
 Author: Katsumi Okuda
 Author-email: okuda@csail.mit.edu
 License: MIT
 Description: <!-- {% raw %} -->
         # *AskIt* (pyaskit)
@@ -104,14 +104,15 @@
         
         Before using *AskIt*, you need to set your API key as an appropriate environment variable:
         
         - OpenAI API: `OPENAI_API_KEY`
         - Gemini API: `GOOGLE_API_KEY`
         - Claude API: `ANTHROPIC_API_KEY`
         - COHERE API: `CO_API_KEY`
+        - groq API: `GROQ_API_KEY`
         
         For example, to use OpenAI API, you need to set your OpenAI API key as an environment variable `OPENAI_API_KEY`:
         ```bash
         export OPENAI_API_KEY=<your OpenAI API key>
         ```
         `<your OpenAI API key>` is a string that looks like this: `sk-<your key>`.
          You can find your OpenAI API key in the [OpenAI dashboard](https://platform.openai.com/account/api-keys).
```

### Comparing `pyaskit-1.4.1/README.md` & `pyaskit-1.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 Before using *AskIt*, you need to set your API key as an appropriate environment variable:
 
 - OpenAI API: `OPENAI_API_KEY`
 - Gemini API: `GOOGLE_API_KEY`
 - Claude API: `ANTHROPIC_API_KEY`
 - COHERE API: `CO_API_KEY`
+- groq API: `GROQ_API_KEY`
 
 For example, to use OpenAI API, you need to set your OpenAI API key as an environment variable `OPENAI_API_KEY`:
 ```bash
 export OPENAI_API_KEY=<your OpenAI API key>
 ```
 `<your OpenAI API key>` is a string that looks like this: `sk-<your key>`.
  You can find your OpenAI API key in the [OpenAI dashboard](https://platform.openai.com/account/api-keys).
```

### Comparing `pyaskit-1.4.1/pyaskit/code_generator.py` & `pyaskit-1.4.2/pyaskit/code_generator.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/decorator.py` & `pyaskit-1.4.2/pyaskit/decorator.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/dialog.py` & `pyaskit-1.4.2/pyaskit/dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,28 @@
         new_messages.append(
             {
                 "role": "user",
                 "content": f"Correct the answer in JSON again to solve the following error: {validator.feedback}\nProvide the whole answer.",
             }
         )
         data, reason, errors, completion = ask_and_parse(return_type, new_messages)
-    return data, reason, errors, completion
+    return data, reason, errors, completion, messages
+
+
+def improve(answer, answer_type, messages, feedback: str):
+    new_messages = messages.copy()
+    new_messages.append({"role": "assistant", "content": make_answer(answer)})
+    new_messages.append(
+        {
+            "role": "user",
+            "content": f"Improve or correct the answer in JSON again based on the following feedback: {feedback}\nProvide the whole answer. Explain your answer step-by-step in the 'reason' field.",
+        }
+    )
+    answer, reason, errors, completion = ask_and_parse(answer_type, new_messages)
+    return answer, reason, errors, completion, new_messages
 
 
 def chat_raw(return_type, messages):
     merged_messages = merge_messages(messages, return_type)
     return ask_and_parse(return_type, merged_messages)
```

### Comparing `pyaskit-1.4.1/pyaskit/example.py` & `pyaskit-1.4.2/pyaskit/example.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/function.py` & `pyaskit-1.4.2/pyaskit/function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 from typing import List
 import os
 import importlib
 from . import types as t
 from .template import convert_template, extract_variables
-from .dialog import query
+from .dialog import query, improve
 from .function_name import generate_unique_function_name
 from .code_generator import implement_body
 from .prompt import make_coding_prompt
 from .path import add_to_sys_path
 from .example import ExampleType, check_examples
 from .logging_config import setup_logger
-from .llm import get_history, clear_history
 from .types.converter import convert_type
 
 
 logger = setup_logger(__name__)
 
 # Default path
 module_path = os.path.join(os.getcwd(), "askit")
 
 
+class Response:
+    def __init__(self, answer, answer_type, completion, reason, errors, messages):
+        self.answer = answer
+        self.answer_type = answer_type
+        self.completion = completion
+        self.reason = reason
+        self.errors = errors
+        self.messages = messages
+
+    def improve(self, feedback: str):
+        answer, reason, errors, completion, _ = improve(
+            self.answer, self.answer_type, self.messages, feedback
+        )
+        return Response(
+            answer, self.answer_type, completion, reason, errors, self.messages
+        )
+
+
 class Function:
     def __init__(
         self,
         return_type,
         param_types,
         template: str,
         training_examples: ExampleType = [],
@@ -45,33 +62,37 @@
         check_examples(return_type, self.variables, training_examples)
         self.training_examples = training_examples
         self._reason = ""
         self._errors: List[str] = []
         self._completion = None
         self._recompilation_count = 0
         self._validator = None
-        self._history = []
 
     def set_validator(self, validator):
         self._validator = validator
 
     def __call__(self, *args, **kwargs):
+        response = self.ask(*args, **kwargs)
+        self._reason = response.reason
+        self._errors = response.errors
+        self._completion = response.completion
+        return response.answer
+
+    def ask(self, *args, **kwargs):
         converted_template = convert_template(self.template)
         variableMap = {}
         self.check_args(args, kwargs, self.variables, variableMap)
-        clear_history()
-        result, self._reason, self._errors, self._completion = query(
+        answer, reason, _errors, completion, messages = query(
             converted_template,
             variableMap,
             self.return_type,
             self.training_examples,
             self._validator,
         )
-        self._history = get_history()
-        return result
+        return Response(answer, self.return_type, completion, reason, _errors, messages)
 
     @property
     def reason(self):
         return self._reason
 
     @property
     def errors(self):
@@ -81,18 +102,14 @@
     def completion(self):
         return self._completion
 
     @property
     def recompilation_count(self):
         return self._recompilation_count
 
-    @property
-    def history(self):
-        return self._history
-
     def check_args(self, args, kwargs, variables, variableMap):
         for var, arg in zip(variables, args):
             if var in kwargs:
                 raise ValueError(f"got multiple values for argument '{var}'")
             variableMap[var] = arg
         for variable in variables:
             if variable in variableMap:
```

### Comparing `pyaskit-1.4.1/pyaskit/function_name.py` & `pyaskit-1.4.2/pyaskit/function_name.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/llm_claude.py` & `pyaskit-1.4.2/pyaskit/llm_claude.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import anthropic
 from . import config
 
 
 def convert_role(role):
     if role == "system":
-        return "usr"
+        return "user"
     return role
 
 
 def convert_messages(messages):
     result = []
     for message in messages:
         role = convert_role(message["role"])
@@ -20,8 +20,8 @@
 def chat_with_retry(messages):
     messages = convert_messages(messages)
 
     response = anthropic.Anthropic().messages.create(
         model=config.get_model(), max_tokens=1024, messages=messages
     )
 
-    return response.content.text, response
+    return response.content[0].text, response
```

### Comparing `pyaskit-1.4.1/pyaskit/llm_cohere.py` & `pyaskit-1.4.2/pyaskit/llm_cohere.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/llm_gemini.py` & `pyaskit-1.4.2/pyaskit/llm_gemini.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/llm_llama.py` & `pyaskit-1.4.2/pyaskit/llm_llama.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/llm_openai.py` & `pyaskit-1.4.2/pyaskit/llm_openai.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/models.py` & `pyaskit-1.4.2/pyaskit/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -92,14 +92,20 @@
     {
         "model_name": "gpt-3.5-turbo-16k-0613",
         "input_tokens": 16385,
         "output_tokens": 4096,
         "api_name": "OpenAI API",
     },
     {
+        "model_name": "gemini-1.5-pro-latest",
+        "input_token": 1048576,
+        "output_token": 8192,
+        "api_name": "Gemini API",
+    },
+    {
         "model_name": "gemini-1.0-pro",
         "input_token": 30720,
         "output_token": 2048,
         "api_name": "Gemini API",
     },
     {
         "model_name": "gemini-1.0-pro-001",
@@ -160,14 +166,20 @@
     {
         "model_name": "claude-3-sonnet-20240229",
         "input_tokens": 200000,
         "output_tokens": 4096,
         "api_name": "Claude API",
     },
     {
+        "model_name": "claude-3-haiku-20240307",
+        "input_tokens": 200000,
+        "output_tokens": 4096,
+        "api_name": "Claude API",
+    },
+    {
         "model_name": "claude-2.1",
         "input_tokens": 200000,
         "output_tokens": 4096,
         "api_name": "Claude API",
     },
     {
         "model_name": "claude-2.0",
@@ -177,8 +189,26 @@
     },
     {
         "model_name": "claude-instant-1.2",
         "input_tokens": 100000,
         "output_tokens": 4096,
         "api_name": "Claude API",
     },
+    {
+        "model_name": "llama2-70b-4096",
+        "input_tokens": 4096,
+        "output_tokens": 4096,
+        "api_name": "groq API",
+    },
+    {
+        "model_name": "mixtral-8x7b-32768",
+        "input_tokens": 32768,
+        "output_tokens": 32768,
+        "api_name": "groq API",
+    },
+    {
+        "model_name": "gemma-7b-it",
+        "input_tokens": 8192,
+        "output_tokens": 8192,
+        "api_name": "groq API",
+    },
 ]
```

### Comparing `pyaskit-1.4.1/pyaskit/prompt.py` & `pyaskit-1.4.2/pyaskit/prompt.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/py_askit.py` & `pyaskit-1.4.2/pyaskit/py_askit.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/template.py` & `pyaskit-1.4.2/pyaskit/template.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/types/converter.py` & `pyaskit-1.4.2/pyaskit/types/converter.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/types/schema.py` & `pyaskit-1.4.2/pyaskit/types/schema.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/types/type_printer.py` & `pyaskit-1.4.2/pyaskit/types/type_printer.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit/types/types.py` & `pyaskit-1.4.2/pyaskit/types/types.py`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/pyaskit.egg-info/PKG-INFO` & `pyaskit-1.4.2/pyaskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaskit
-Version: 1.4.1
+Version: 1.4.2
 Summary: AskIt: Unified programming interface for programming with large language models (GPT-3.5, GPT-4, Gemini, Claude, COHERE, Llama 2)
 Home-page: https://github.com/katsumiok/pyaskit
 Author: Katsumi Okuda
 Author-email: okuda@csail.mit.edu
 License: MIT
 Description: <!-- {% raw %} -->
         # *AskIt* (pyaskit)
@@ -104,14 +104,15 @@
         
         Before using *AskIt*, you need to set your API key as an appropriate environment variable:
         
         - OpenAI API: `OPENAI_API_KEY`
         - Gemini API: `GOOGLE_API_KEY`
         - Claude API: `ANTHROPIC_API_KEY`
         - COHERE API: `CO_API_KEY`
+        - groq API: `GROQ_API_KEY`
         
         For example, to use OpenAI API, you need to set your OpenAI API key as an environment variable `OPENAI_API_KEY`:
         ```bash
         export OPENAI_API_KEY=<your OpenAI API key>
         ```
         `<your OpenAI API key>` is a string that looks like this: `sk-<your key>`.
          You can find your OpenAI API key in the [OpenAI dashboard](https://platform.openai.com/account/api-keys).
```

### Comparing `pyaskit-1.4.1/pyaskit.egg-info/SOURCES.txt` & `pyaskit-1.4.2/pyaskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyaskit-1.4.1/setup.py` & `pyaskit-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyaskit",
-    version="1.4.1",
+    version="1.4.2",
     packages=find_packages(),
     description="AskIt: Unified programming interface for programming with large language models (GPT-3.5, GPT-4, Gemini, Claude, COHERE, Llama 2)",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Katsumi Okuda",
     author_email="okuda@csail.mit.edu",
     url="https://github.com/katsumiok/pyaskit",
```

