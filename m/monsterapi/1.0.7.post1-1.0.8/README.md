# Comparing `tmp/monsterapi-1.0.7.post1.tar.gz` & `tmp/monsterapi-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monsterapi-1.0.7.post1.tar", last modified: Tue Mar 19 16:00:20 2024, max compression
+gzip compressed data, was "monsterapi-1.0.8.tar", last modified: Fri Apr 12 19:53:51 2024, max compression
```

## Comparing `monsterapi-1.0.7.post1.tar` & `monsterapi-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:20.443327 monsterapi-1.0.7.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-03-19 16:00:20.443327 monsterapi-1.0.7.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:20.439327 monsterapi-1.0.7.post1/monsterapi/
--rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/InputDataModels.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:20.439327 monsterapi-1.0.7.post1/monsterapi/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/benchmark/LLMBenchMark.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18554 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/deployDataModels.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/nextGenLLMClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/monsterapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:20.443327 monsterapi-1.0.7.post1/monsterapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-03-19 16:00:20.000000 monsterapi-1.0.7.post1/monsterapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-19 16:00:20.000000 monsterapi-1.0.7.post1/monsterapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 16:00:20.000000 monsterapi-1.0.7.post1/monsterapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-19 16:00:20.000000 monsterapi-1.0.7.post1/monsterapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 16:00:20.000000 monsterapi-1.0.7.post1/monsterapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 16:00:20.443327 monsterapi-1.0.7.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 16:00:20.439327 monsterapi-1.0.7.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/tests/test_client_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/tests/test_client_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-19 16:00:03.000000 monsterapi-1.0.7.post1/tests/test_next_gen_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:51.425781 monsterapi-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 19:53:41.000000 monsterapi-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-12 19:53:51.425781 monsterapi-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-12 19:53:41.000000 monsterapi-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:51.421781 monsterapi-1.0.8/monsterapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/Dreambooth_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14891 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/InputDataModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/LLM_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/Whisper_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:51.421781 monsterapi-1.0.8/monsterapi/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/benchmark/LLMBenchMark.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/deployDataModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/nextGenLLMClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-12 19:53:41.000000 monsterapi-1.0.8/monsterapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:51.425781 monsterapi-1.0.8/monsterapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-12 19:53:51.000000 monsterapi-1.0.8/monsterapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-12 19:53:51.000000 monsterapi-1.0.8/monsterapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:53:51.000000 monsterapi-1.0.8/monsterapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 19:53:51.000000 monsterapi-1.0.8/monsterapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 19:53:51.000000 monsterapi-1.0.8/monsterapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:53:51.425781 monsterapi-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-12 19:53:41.000000 monsterapi-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:53:51.425781 monsterapi-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-04-12 19:53:41.000000 monsterapi-1.0.8/tests/test_client_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-12 19:53:41.000000 monsterapi-1.0.8/tests/test_client_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-12 19:53:41.000000 monsterapi-1.0.8/tests/test_next_gen_llm.py
```

### Comparing `monsterapi-1.0.7.post1/LICENSE` & `monsterapi-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/PKG-INFO` & `monsterapi-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monsterapi
-Version: 1.0.7.post1
+Version: 1.0.8
 Summary: A Python client for Monster API v2
 Home-page: https://github.com/qblocks/monsterapiclient
 Author: Ramachandra Vikas Chamarthi
 Author-email: vikas@qblocks.cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `monsterapi-1.0.7.post1/README.md` & `monsterapi-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/monsterapi/InputDataModels.py` & `monsterapi-1.0.8/monsterapi/InputDataModels.py`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/monsterapi/benchmark/LLMBenchMark.py` & `monsterapi-1.0.8/monsterapi/benchmark/LLMBenchMark.py`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/monsterapi/client.py` & `monsterapi-1.0.8/monsterapi/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,19 @@
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 from typing import Optional, Literal, Union, List, Dict, Iterable
 from pydantic import BaseModel, Field
 from functools import wraps
 
 from monsterapi.InputDataModels import LLMInputModel1, LLMInputModel2, SDInputModel, MODELS_TO_DATAMODEL, FileField
-from monsterapi.deployDataModels import LLMServingParams, CustomImageParams, DEPLOY_SERVICES
+from monsterapi.deployDataModels import LLMServingParams, CustomImageParams, DEPLOY_SERVICES, FINETUNE_SERVICES
+from monsterapi.LLM_config import LLMServiceParams as LLMServiceParamsFinetuning
+from monsterapi.Dreambooth_config import DreamboothServiceParams as DreamboothServiceParamsFinetuning
+from monsterapi.Whisper_config import WhisperServiceParams as WhisperServiceParamsFinetuning
+from monsterapi.Dreambooth_config import DreamboothDeploymentConfig
 
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 # Use LOGGING_LEVEL environment variable to set logging level
 # Default logging level is INFO
 level = os.environ.get('LOGGING_LEVEL', 'INFO')
@@ -404,37 +408,55 @@
         if "deploy" in model:
             return self.get_response_sync_api(model, data)
         else:
             response = self.get_response(model, data)
             process_id = response['process_id']
             return self.wait_and_get_result(process_id, timeout=timeout)
 
-    
     def deploy(self, service: Literal["llm", "custom_image"], params: dict):
+        return self.__launch_job("deploy", service, params)
+    
+    def finetune(self, service: Literal["llm", "speech2text/whisper", "text2image/sdxl-dreambooth"], params: dict):
+        return self.__launch_job("finetune", service, params)
+
+    def __launch_job(self, service_type: Literal["finetune", "deploy"], service, params: dict ):
         """
         Deploy a LLM model on monsterapi all you need is basemodel path and lora adapter path if needed and GPU VRam requirement. 
 
         Parameters:
         -----------
             service: str Service to deploy currently only 'llm' is implemented.
             params: dict deployLLMInputDataModel see monsterapi/deployDataModels.py for more details
 
         Returns:
 
         """
-        if service not in DEPLOY_SERVICES:
-            raise ValueError(f"Invalid service: {service}!")
-
-        # Validate data payload with pydantic model
-        if service == "llm":
-            LLMServingParams(**params)
-        elif service == "custom_image":
-            CustomImageParams(**params)
+        if service_type == "finetune":
+            if service == "llm":
+                LLMServiceParamsFinetuning(**params)
+            elif service == "speech2text/whisper":
+                WhisperServiceParamsFinetuning(**params)
+            elif service == "text2image/sdxl-dreambooth":
+                DreamboothServiceParamsFinetuning(**params)
+            else:
+                raise ValueError(f"Invalid service: {service}!")         
+        elif service_type == "deploy":
+            # Validate deploy payloads
+            if service == "llm":
+                LLMServingParams(**params)
+            elif service == "custom_image":
+                CustomImageParams(**params)
+            elif service == "sdxl-dreambooth":
+                DreamboothDeploymentConfig(**params)
+            else:
+                raise ValueError(f"Invalid service: {service}!")        
+        else:
+            raise ValueError(f"Invalid service_type: {service_type}")
 
-        url = f"{self.base_url}/deploy/{service}"
+        url = f"{self.base_url}/{service_type}/{service}"
         response = requests.post(
             url,
             headers=self.headers,
             json=params
         )
         
         try:
@@ -527,7 +549,9 @@
             # Construct a new error message containing the original message and the JSON response.
             new_error_message = f"{str(e)} - Response: {response_content}"
             
             # Raise the new error
             raise requests.HTTPError(new_error_message, response=response)
        
         return response.json()
+
+
```

### Comparing `monsterapi-1.0.7.post1/monsterapi/deployDataModels.py` & `monsterapi-1.0.8/monsterapi/deployDataModels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pydantic import BaseModel, Field, validator
 from typing import Optional, Literal, List
 import uuid
 
 
+FINETUNE_SERVICES = ["llm", "speech2text/whisper", "text2image/sdxl-dreambooth"]
 
 class LLMServingParams(BaseModel):
     basemodel_path: str = Field(..., description="Path to the base model can be a huggingface model or a custom model link", examples=["meta-llama/Llama-2-7b-hf"])
     loramodel_path: Optional[str] = Field(None, description="Path to the LoRA model can be a huggingface model or a custom model link", examples=["qblocks/OpenPlatypus_LLAMA2_7b"])
     prompt_template: str = Field("{prompt}{completion}", description="Template for the prompt",examples = ["{prompt}{completion}"])
     per_gpu_vram: Literal[8, 16, 24, 48, 80] = Field(..., description="GPU VRAM to be used", examples = [24])
     gpu_count: Literal[1, 2, 4, 8] = Field(..., description="Number of GPUs to be used", examples = [1])
```

### Comparing `monsterapi-1.0.7.post1/monsterapi/nextGenLLMClient.py` & `monsterapi-1.0.8/monsterapi/nextGenLLMClient.py`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/monsterapi.egg-info/PKG-INFO` & `monsterapi-1.0.8/monsterapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monsterapi
-Version: 1.0.7.post1
+Version: 1.0.8
 Summary: A Python client for Monster API v2
 Home-page: https://github.com/qblocks/monsterapiclient
 Author: Ramachandra Vikas Chamarthi
 Author-email: vikas@qblocks.cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `monsterapi-1.0.7.post1/setup.py` & `monsterapi-1.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="monsterapi",
-    version="1.0.7.post1",
+    version="1.0.8",
     author="Ramachandra Vikas Chamarthi",
     author_email="vikas@qblocks.cloud",
     description="A Python client for Monster API v2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/qblocks/monsterapiclient",
     packages=find_packages(),
```

### Comparing `monsterapi-1.0.7.post1/tests/test_client_functional.py` & `monsterapi-1.0.8/tests/test_client_functional.py`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/tests/test_client_mock.py` & `monsterapi-1.0.8/tests/test_client_mock.py`

 * *Files identical despite different names*

### Comparing `monsterapi-1.0.7.post1/tests/test_next_gen_llm.py` & `monsterapi-1.0.8/tests/test_next_gen_llm.py`

 * *Files identical despite different names*

