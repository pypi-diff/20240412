# Comparing `tmp/ipl_pipeline_py_common-0.6.1.tar.gz` & `tmp/ipl_pipeline_py_common-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipl_pipeline_py_common-0.6.1.tar", max compression
+gzip compressed data, was "ipl_pipeline_py_common-0.7.0.tar", max compression
```

## Comparing `ipl_pipeline_py_common-0.6.1.tar` & `ipl_pipeline_py_common-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      635 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/README.md
--rw-r--r--   0        0        0     1336 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/CommonFunctions/StartupCommon.py
--rw-r--r--   0        0        0       71 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/CommonFunctions/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/CommonFunctions/urn.py
--rw-r--r--   0        0        0      113 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/__init__.py
--rw-r--r--   0        0        0     2856 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/dBCommonConnector.py
--rw-r--r--   0        0        0       45 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/models/__init__.py
--rw-r--r--   0        0        0      376 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/models/base.py
--rw-r--r--   0        0        0      156 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/QueueModels/__init__.py
--rw-r--r--   0        0        0      166 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/QueueModels/serviceRequest.py
--rw-r--r--   0        0        0      856 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/QueueModels/serviceResponse.py
--rw-r--r--   0        0        0       58 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pipeline/__init__.py
--rw-r--r--   0        0        0      551 2024-04-11 23:20:20.046983 ipl_pipeline_py_common-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      635 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/README.md
+-rw-r--r--   0        0        0     1336 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/StartupCommon.py
+-rw-r--r--   0        0        0       71 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/urn.py
+-rw-r--r--   0        0        0      113 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/__init__.py
+-rw-r--r--   0        0        0     2949 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/dBCommonConnector.py
+-rw-r--r--   0        0        0       45 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/models/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/models/base.py
+-rw-r--r--   0        0        0      156 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceRequest.py
+-rw-r--r--   0        0        0     1001 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceResponse.py
+-rw-r--r--   0        0        0       58 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/__init__.py
+-rw-r--r--   0        0        0      551 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.7.0/PKG-INFO
```

### Comparing `ipl_pipeline_py_common-0.6.1/README.md` & `ipl_pipeline_py_common-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.6.1/pipeline/CommonFunctions/StartupCommon.py` & `ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/StartupCommon.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.6.1/pipeline/CommonFunctions/urn.py` & `ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/urn.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.6.1/pipeline/DBCommon/dBCommonConnector.py` & `ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/dBCommonConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import motor.motor_asyncio
 from redis import asyncio as aioredis
 from typing import Optional, Union
-import msgpack
+import json
 
 from .exceptions import NoConnectionError
 
 
 class DBCommonConnector:
     def __init__(self, mongo_uri: str, db_name: str, redis_uri: str):
         """
@@ -37,33 +37,35 @@
         """
         Add Key:Value to Redis cache
         :param key: Key name
         :param value: Value Data dict
         :param expire: expiry time in seconds, default 1800s
         :return: if operation was successful
         """
+        cache_str = json.dumps(value)
         if self._redis_client is None:
             raise NoConnectionError("Redis client not connected")
         async with self._redis_client.client() as conn:
             if expire and expire > 0:
-                ok = await conn.execute_command("SET", f"{key}", value, "EX", f"{expire}")
+                ok = await conn.execute_command("SET", f"{key}", cache_str, "EX", f"{expire}")
             else:
-                ok = await conn.execute_command("SET", f"{key}", value)
+                ok = await conn.execute_command("SET", f"{key}", cache_str)
             return bool(ok)
 
     async def _cache_get_key(self, key: str) -> Optional[Union[dict, list]]:
         """
         Retrieve value via key from Redis cache
         :param key: Key to retrieve data from
         :return: None or dict
         """
         if self._redis_client is None:
             raise NoConnectionError("Redis client not connected")
         if data := await self._redis_client.get(f"{key}"):
-            return data
+            loaded_data = json.loads(data)
+            return loaded_data
         return None
 
     async def _cache_delete_key(self, key: str) -> bool:
         """
         Delete key from Redis Cache
         :param key: Key Name
         :return: if operation was successful
```

### Comparing `ipl_pipeline_py_common-0.6.1/pipeline/QueueModels/serviceResponse.py` & `ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceResponse.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 T = TypeVar("T", bound=BaseModel)
 
 
 class ServiceResponse(BaseModel, Generic[T]):
     response_node_id: Optional[str] = Field("unknown")
     response_node_version: Optional[str] = Field("unknown")
     request_error: bool = Field(False, description="Error in request")
+    server_error: bool = Field(False, description="Error in server")
+    response_code: Optional[int] = Field(None, description="Response Code")
     request_error_message: Optional[str] = Field(None, description="Error Message")
     response_data: Optional[T] = Field(None, description="Response Data")
 
     @model_validator(mode='after')
     def check_state(self):
         """
         Check if response data is None if request error is True
```

### Comparing `ipl_pipeline_py_common-0.6.1/pyproject.toml` & `ipl_pipeline_py_common-0.7.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipl-pipeline-py-common"
-version = "0.6.1"
+version = "0.7.0"
 description = "Common functions and modules for Python based IPL Pipeline Services"
 authors = ["Vincent Lee <vlee@vlee.me.uk>"]
 license = "All Rights Reserved"
 readme = "README.md"
 packages = [{include = "pipeline"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ipl_pipeline_py_common-0.6.1/PKG-INFO` & `ipl_pipeline_py_common-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipl-pipeline-py-common
-Version: 0.6.1
+Version: 0.7.0
 Summary: Common functions and modules for Python based IPL Pipeline Services
 License: All Rights Reserved
 Author: Vincent Lee
 Author-email: vlee@vlee.me.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

