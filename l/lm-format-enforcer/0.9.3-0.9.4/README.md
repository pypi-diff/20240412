# Comparing `tmp/lm_format_enforcer-0.9.3.tar.gz` & `tmp/lm_format_enforcer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lm_format_enforcer-0.9.3.tar", max compression
+gzip compressed data, was "lm_format_enforcer-0.9.4.tar", max compression
```

## Comparing `lm_format_enforcer-0.9.3.tar` & `lm_format_enforcer-0.9.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1065 2024-03-13 20:42:48.052666 lm_format_enforcer-0.9.3/LICENSE
--rw-r--r--   0        0        0    12745 2024-03-13 20:42:48.052666 lm_format_enforcer-0.9.3/README.md
--rw-r--r--   0        0        0      850 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/__init__.py
--rw-r--r--   0        0        0     3893 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/analyzer.py
--rw-r--r--   0        0        0     6702 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/characterlevelparser.py
--rw-r--r--   0        0        0      341 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/consts.py
--rw-r--r--   0        0        0      104 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/external/__init__.py
--rw-r--r--   0        0        0    10566 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/external/jsonschemaobject.py
--rw-r--r--   0        0        0     7044 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/external/jsonschemaobjectutil.py
--rw-r--r--   0        0        0        0 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/__init__.py
--rw-r--r--   0        0        0     2798 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/exllamav2.py
--rw-r--r--   0        0        0     2820 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/haystackv1.py
--rw-r--r--   0        0        0     3518 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/haystackv2.py
--rw-r--r--   0        0        0     3572 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/llamacpp.py
--rw-r--r--   0        0        0     6769 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/transformers.py
--rw-r--r--   0        0        0     3538 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/trtllm.py
--rw-r--r--   0        0        0     2628 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/integrations/vllm.py
--rw-r--r--   0        0        0    29631 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/jsonschemaparser.py
--rw-r--r--   0        0        0     3875 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/regexparser.py
--rw-r--r--   0        0        0    10083 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/tokenenforcer.py
--rw-r--r--   0        0        0     6813 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/lmformatenforcer/tokenizerprefixtree.py
--rw-r--r--   0        0        0     2664 2024-03-13 20:42:48.056666 lm_format_enforcer-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    14078 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 19:53:10.248247 lm_format_enforcer-0.9.4/LICENSE
+-rw-r--r--   0        0        0    12745 2024-04-12 19:53:10.248247 lm_format_enforcer-0.9.4/README.md
+-rw-r--r--   0        0        0      850 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/__init__.py
+-rw-r--r--   0        0        0     3893 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/analyzer.py
+-rw-r--r--   0        0        0     6702 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/characterlevelparser.py
+-rw-r--r--   0        0        0      341 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/consts.py
+-rw-r--r--   0        0        0      104 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/external/__init__.py
+-rw-r--r--   0        0        0    10566 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/external/jsonschemaobject.py
+-rw-r--r--   0        0        0     7044 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/external/jsonschemaobjectutil.py
+-rw-r--r--   0        0        0        0 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/__init__.py
+-rw-r--r--   0        0        0     2798 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/exllamav2.py
+-rw-r--r--   0        0        0     2820 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/haystackv1.py
+-rw-r--r--   0        0        0     3518 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/haystackv2.py
+-rw-r--r--   0        0        0     3572 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/llamacpp.py
+-rw-r--r--   0        0        0     6769 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/transformers.py
+-rw-r--r--   0        0        0     3538 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/trtllm.py
+-rw-r--r--   0        0        0     2645 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/integrations/vllm.py
+-rw-r--r--   0        0        0    29631 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/jsonschemaparser.py
+-rw-r--r--   0        0        0     3875 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/regexparser.py
+-rw-r--r--   0        0        0    10083 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/tokenenforcer.py
+-rw-r--r--   0        0        0     6813 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/lmformatenforcer/tokenizerprefixtree.py
+-rw-r--r--   0        0        0     2664 2024-04-12 19:53:10.252246 lm_format_enforcer-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    14078 1970-01-01 00:00:00.000000 lm_format_enforcer-0.9.4/PKG-INFO
```

### Comparing `lm_format_enforcer-0.9.3/LICENSE` & `lm_format_enforcer-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/README.md` & `lm_format_enforcer-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/__init__.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/__init__.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/analyzer.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/analyzer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/characterlevelparser.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/characterlevelparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/external/jsonschemaobject.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/external/jsonschemaobject.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/external/jsonschemaobjectutil.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/external/jsonschemaobjectutil.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/exllamav2.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/exllamav2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/haystackv1.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/haystackv1.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/haystackv2.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/haystackv2.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/llamacpp.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/llamacpp.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/transformers.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/trtllm.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/trtllm.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/integrations/vllm.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/integrations/vllm.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,19 +27,20 @@
             # We create it here because full_like() also copies the device and dtype
             self.mask = torch.full_like(scores, -math.inf)
         self.mask[allowed_tokens] = 0
         scores = scores + self.mask
         return scores
 
 
-def build_vllm_token_enforcer_tokenizer_data(llm: Union[vllm.LLM, PreTrainedTokenizerBase]) -> TokenEnforcerTokenizerData:
-    tokenizer = llm.get_tokenizer() if isinstance(llm, vllm.LLM) else llm
-    # In some vLLM versions the tokenizer is wrapped in a TokenizerGroup
-    if tokenizer.__class__.__name__ == 'TokenizerGroup':
-        tokenizer = tokenizer.tokenizer  # noqa
+def build_vllm_token_enforcer_tokenizer_data(tokenizer: Union[vllm.LLM, PreTrainedTokenizerBase]) -> TokenEnforcerTokenizerData:
+    # There are many classes that can be passed here, this logic should work on all of them.
+    if hasattr(tokenizer, 'get_tokenizer'):
+        tokenizer = tokenizer.get_tokenizer()
+    if hasattr(tokenizer, 'tokenizer'):
+        tokenizer = tokenizer.tokenizer
     return build_token_enforcer_tokenizer_data(tokenizer)
 
 
 def build_vllm_logits_processor(llm: Union[vllm.LLM, PreTrainedTokenizerBase, TokenEnforcerTokenizerData], 
                                 character_level_parser: CharacterLevelParser, 
                                 analyze: bool=False) -> VLLMLogitsProcessor:
     """Build the logits processor function that llama.cpp will use to filter the tokens generated by the model. The result
```

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/jsonschemaparser.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/jsonschemaparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/regexparser.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/regexparser.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/tokenenforcer.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/tokenenforcer.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/lmformatenforcer/tokenizerprefixtree.py` & `lm_format_enforcer-0.9.4/lmformatenforcer/tokenizerprefixtree.py`

 * *Files identical despite different names*

### Comparing `lm_format_enforcer-0.9.3/pyproject.toml` & `lm_format_enforcer-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lm-format-enforcer"
-version = "0.9.3"
+version = "0.9.4"
 description = "Enforce the output format (JSON Schema, Regex etc) of a language model"
 authors = ["Noam Gat <noamgat@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noamgat/lm-format-enforcer"
 repository = "https://github.com/noamgat/lm-format-enforcer"
 documentation = "https://github.com/noamgat/lm-format-enforcer"
```

### Comparing `lm_format_enforcer-0.9.3/PKG-INFO` & `lm_format_enforcer-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lm-format-enforcer
-Version: 0.9.3
+Version: 0.9.4
 Summary: Enforce the output format (JSON Schema, Regex etc) of a language model
 Home-page: https://github.com/noamgat/lm-format-enforcer
 License: MIT
 Author: Noam Gat
 Author-email: noamgat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

