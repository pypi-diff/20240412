# Comparing `tmp/liminal_sdk_python-2024.4.0.tar.gz` & `tmp/liminal_sdk_python-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.4.0.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.4.3.tar", max compression
```

## Comparing `liminal_sdk_python-2024.4.0.tar` & `liminal_sdk_python-2024.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/LICENSE
--rw-r--r--   0        0        0    13136 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/README.md
--rw-r--r--   0        0        0       82 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/__init__.py
--rw-r--r--   0        0        0      524 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2961 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      873 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0     8731 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/client.py
--rw-r--r--   0        0        0      165 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/const.py
--rw-r--r--   0        0        0       45 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2352 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0     5463 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3264 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0     2372 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2162 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      400 2024-04-03 01:59:47.512432 liminal_sdk_python-2024.4.0/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      382 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/model.py
--rw-r--r--   0        0        0      109 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/liminal/helpers/typing.py
--rw-r--r--   0        0        0    13516 2024-04-03 01:59:47.516432 liminal_sdk_python-2024.4.0/pyproject.toml
--rw-r--r--   0        0        0    14258 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/LICENSE
+-rw-r--r--   0        0        0    13136 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/README.md
+-rw-r--r--   0        0        0       82 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      873 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0     8731 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2284 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0     5463 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3264 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0     2372 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2162 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      400 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/model.py
+-rw-r--r--   0        0        0      109 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/liminal/helpers/typing.py
+-rw-r--r--   0        0        0     8522 2024-04-12 05:10:15.966537 liminal_sdk_python-2024.4.3/pyproject.toml
+-rw-r--r--   0        0        0    14258 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.4.3/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.4.0/LICENSE` & `liminal_sdk_python-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/README.md` & `liminal_sdk_python-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/auth/__init__.py` & `liminal_sdk_python-2024.4.3/liminal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.4.3/liminal/auth/microsoft/device_code_flow.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.4.3/liminal/auth/microsoft/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/client.py` & `liminal_sdk_python-2024.4.3/liminal/client.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/llm/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,14 @@
     """Define the enum for the model provider key."""
 
     ANTHROPIC = "anthropic"
     AWS_BEDROCK = "aws_bedrock"
     AWS_SAGEMAKER = "aws_sagemaker"
     AZURE_OPENAI = "azure_openai"
     COHERE = "cohere"
-    GOOGLE_GEMINI = "google_gemini"
-    GOOGLE_PALM = "google_palm"
     HUGGINGFACE = "huggingface"
     MISTRAL = "mistral"
     OLLAMA = "ollama"
     OPENAI = "openai"
 
 
 @dataclass(frozen=True, kw_only=True)
```

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/__init__.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/prompt/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/thread/__init__.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.4.3/liminal/endpoints/thread/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.4.0/PKG-INFO` & `liminal_sdk_python-2024.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.4.0
+Version: 2024.4.3
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

