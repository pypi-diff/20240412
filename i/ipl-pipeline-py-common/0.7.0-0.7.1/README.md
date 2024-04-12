# Comparing `tmp/ipl_pipeline_py_common-0.7.0.tar.gz` & `tmp/ipl_pipeline_py_common-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipl_pipeline_py_common-0.7.0.tar", max compression
+gzip compressed data, was "ipl_pipeline_py_common-0.7.1.tar", max compression
```

## Comparing `ipl_pipeline_py_common-0.7.0.tar` & `ipl_pipeline_py_common-0.7.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      635 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/README.md
--rw-r--r--   0        0        0     1336 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/StartupCommon.py
--rw-r--r--   0        0        0       71 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/urn.py
--rw-r--r--   0        0        0      113 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/__init__.py
--rw-r--r--   0        0        0     2949 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/dBCommonConnector.py
--rw-r--r--   0        0        0       45 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/exceptions.py
--rw-r--r--   0        0        0       31 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/models/__init__.py
--rw-r--r--   0        0        0      376 2024-04-11 23:30:29.248806 ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/models/base.py
--rw-r--r--   0        0        0      156 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/__init__.py
--rw-r--r--   0        0        0      166 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceRequest.py
--rw-r--r--   0        0        0     1001 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceResponse.py
--rw-r--r--   0        0        0       58 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pipeline/__init__.py
--rw-r--r--   0        0        0      551 2024-04-11 23:30:29.252806 ipl_pipeline_py_common-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      635 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/README.md
+-rw-r--r--   0        0        0     1336 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/CommonFunctions/StartupCommon.py
+-rw-r--r--   0        0        0       71 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/CommonFunctions/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/CommonFunctions/urn.py
+-rw-r--r--   0        0        0      113 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/__init__.py
+-rw-r--r--   0        0        0     2968 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/dBCommonConnector.py
+-rw-r--r--   0        0        0       45 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/exceptions.py
+-rw-r--r--   0        0        0       31 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/models/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/models/base.py
+-rw-r--r--   0        0        0      156 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/QueueModels/__init__.py
+-rw-r--r--   0        0        0      166 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/QueueModels/serviceRequest.py
+-rw-r--r--   0        0        0     1001 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/QueueModels/serviceResponse.py
+-rw-r--r--   0        0        0       58 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pipeline/__init__.py
+-rw-r--r--   0        0        0      551 2024-04-11 23:36:11.055762 ipl_pipeline_py_common-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1413 1970-01-01 00:00:00.000000 ipl_pipeline_py_common-0.7.1/PKG-INFO
```

### Comparing `ipl_pipeline_py_common-0.7.0/README.md` & `ipl_pipeline_py_common-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/StartupCommon.py` & `ipl_pipeline_py_common-0.7.1/pipeline/CommonFunctions/StartupCommon.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.7.0/pipeline/CommonFunctions/urn.py` & `ipl_pipeline_py_common-0.7.1/pipeline/CommonFunctions/urn.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.7.0/pipeline/DBCommon/dBCommonConnector.py` & `ipl_pipeline_py_common-0.7.1/pipeline/DBCommon/dBCommonConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import motor.motor_asyncio
 from redis import asyncio as aioredis
-from typing import Optional, Union
+from typing import Optional, Union, Dict
 import json
 
 from .exceptions import NoConnectionError
 
 
 class DBCommonConnector:
     def __init__(self, mongo_uri: str, db_name: str, redis_uri: str):
@@ -47,15 +47,15 @@
         async with self._redis_client.client() as conn:
             if expire and expire > 0:
                 ok = await conn.execute_command("SET", f"{key}", cache_str, "EX", f"{expire}")
             else:
                 ok = await conn.execute_command("SET", f"{key}", cache_str)
             return bool(ok)
 
-    async def _cache_get_key(self, key: str) -> Optional[Union[dict, list]]:
+    async def _cache_get_key(self, key: str) -> Optional[Union[Dict[str, object], list]]:
         """
         Retrieve value via key from Redis cache
         :param key: Key to retrieve data from
         :return: None or dict
         """
         if self._redis_client is None:
             raise NoConnectionError("Redis client not connected")
```

### Comparing `ipl_pipeline_py_common-0.7.0/pipeline/QueueModels/serviceResponse.py` & `ipl_pipeline_py_common-0.7.1/pipeline/QueueModels/serviceResponse.py`

 * *Files identical despite different names*

### Comparing `ipl_pipeline_py_common-0.7.0/pyproject.toml` & `ipl_pipeline_py_common-0.7.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipl-pipeline-py-common"
-version = "0.7.0"
+version = "0.7.1"
 description = "Common functions and modules for Python based IPL Pipeline Services"
 authors = ["Vincent Lee <vlee@vlee.me.uk>"]
 license = "All Rights Reserved"
 readme = "README.md"
 packages = [{include = "pipeline"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ipl_pipeline_py_common-0.7.0/PKG-INFO` & `ipl_pipeline_py_common-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipl-pipeline-py-common
-Version: 0.7.0
+Version: 0.7.1
 Summary: Common functions and modules for Python based IPL Pipeline Services
 License: All Rights Reserved
 Author: Vincent Lee
 Author-email: vlee@vlee.me.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```
