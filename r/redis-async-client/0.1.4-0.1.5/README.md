# Comparing `tmp/redis_async_client-0.1.4.tar.gz` & `tmp/redis_async_client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_async_client-0.1.4.tar", max compression
+gzip compressed data, was "redis_async_client-0.1.5.tar", max compression
```

## Comparing `redis_async_client-0.1.4.tar` & `redis_async_client-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1098 2024-04-06 08:45:54.633004 redis_async_client-0.1.4/README.md
--rw-r--r--   0        0        0     2223 2024-04-06 08:38:23.651775 redis_async_client-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      653 2024-04-06 08:04:14.972887 redis_async_client-0.1.4/src/redis_async_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.4/src/redis_async_client/core/__init__.py
--rw-r--r--   0        0        0     3869 2024-04-06 08:03:13.985441 redis_async_client-0.1.4/src/redis_async_client/core/_base.py
--rw-r--r--   0        0        0       54 2024-04-06 08:00:40.522853 redis_async_client-0.1.4/src/redis_async_client/core/_constants.py
--rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.4/src/redis_async_client/core/_logger.py
--rw-r--r--   0        0        0       87 2024-04-06 07:58:23.004145 redis_async_client-0.1.4/src/redis_async_client/core/_types.py
--rw-r--r--   0        0        0     3290 2024-04-06 08:04:13.056904 redis_async_client-0.1.4/src/redis_async_client/core/async_client.py
--rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.4/src/redis_async_client/core/exc.py
--rw-r--r--   0        0        0      760 2024-04-06 08:03:13.477445 redis_async_client-0.1.4/src/redis_async_client/core/settings.py
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 redis_async_client-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-06 08:45:54.633004 redis_async_client-0.1.5/README.md
+-rw-r--r--   0        0        0     2223 2024-04-12 06:45:10.017904 redis_async_client-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      653 2024-04-06 08:04:14.972887 redis_async_client-0.1.5/src/redis_async_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.5/src/redis_async_client/core/__init__.py
+-rw-r--r--   0        0        0     4761 2024-04-12 06:37:50.653257 redis_async_client-0.1.5/src/redis_async_client/core/_base.py
+-rw-r--r--   0        0        0       54 2024-04-06 08:00:40.522853 redis_async_client-0.1.5/src/redis_async_client/core/_constants.py
+-rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.5/src/redis_async_client/core/_logger.py
+-rw-r--r--   0        0        0       87 2024-04-06 07:58:23.004145 redis_async_client-0.1.5/src/redis_async_client/core/_types.py
+-rw-r--r--   0        0        0     3819 2024-04-12 06:45:11.025896 redis_async_client-0.1.5/src/redis_async_client/core/async_client.py
+-rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.5/src/redis_async_client/core/exc.py
+-rw-r--r--   0        0        0      760 2024-04-06 08:03:13.477445 redis_async_client-0.1.5/src/redis_async_client/core/settings.py
+-rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 redis_async_client-0.1.5/PKG-INFO
```

### Comparing `redis_async_client-0.1.4/README.md` & `redis_async_client-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.4/pyproject.toml` & `redis_async_client-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-async-client"
-version = "0.1.4"
+version = "0.1.5"
 description = "Redis async client."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Deskent/redis_async_client"
 homepage = "https://pypi.org/project/redis-async-client/"
```

### Comparing `redis_async_client-0.1.4/src/redis_async_client/__init__.py` & `redis_async_client-0.1.5/src/redis_async_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.4/src/redis_async_client/core/_base.py` & `redis_async_client-0.1.5/src/redis_async_client/core/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,19 +130,51 @@
         old_data: str = await self.client.get(self.key)
         if not old_data:
             old_data: list = []
         else:
             old_data: list = json.loads(old_data)
         if not isinstance(old_data, list):
             raise RedisAsyncClientException(
-                f'Data for update must be list, got {type(old_data)}'
+                f'Existing data must be list, got {type(old_data)}'
             )
 
         old_data.append(self._data)
         new_data: str = json.dumps(old_data)
         await self.client.set(
             name=self.key,
             value=new_data,
             ex=self.timeout_sec,
         )
 
+        return old_data
+
+
+class ExtendOperator(SaveOperator):
+    """Extend list with data."""
+
+    async def _execute(self) -> list:
+        """Append data to list"""
+
+        if not isinstance(self._data, list):
+            raise RedisAsyncClientException(
+                f'Data must be list, got {type(self._data)}'
+            )
+
+        old_data: str = await self.client.get(self.key)
+        if not old_data:
+            old_data: list = []
+        else:
+            old_data: list = json.loads(old_data)
+        if not isinstance(old_data, list):
+            raise RedisAsyncClientException(
+                f'Existing data must be list, got {type(old_data)}'
+            )
+
+        old_data.extend(self._data)
+        new_data: str = json.dumps(old_data)
+        await self.client.set(
+            name=self.key,
+            value=new_data,
+            ex=self.timeout_sec,
+        )
+
         return old_data
```

### Comparing `redis_async_client-0.1.4/src/redis_async_client/core/async_client.py` & `redis_async_client-0.1.5/src/redis_async_client/core/async_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Any
 
 from ._base import (
     AppendOperator,
     DeleteOperator,
+    ExtendOperator,
     LoadOperator,
     RedisBase,
     SaveOperator,
     UpdateOperator,
 )
 from ._constants import STORE_TIME_SEC
 from ._logger import logger
@@ -124,14 +125,36 @@
         logger.debug(
             f'Key [{key}]: Timeout: {timeout_sec}. '
             f'Data appended. Now: {len(appended)}'
         )
 
         return appended
 
+    async def extend(
+        self,
+        key: str,
+        data: list,
+        timeout_sec: int = STORE_TIME_SEC,
+    ) -> list:
+        """Extend list with data."""
+
+        extended: list = await ExtendOperator(
+            client=self.client,
+            key=key,
+            data=data,
+            timeout_sec=timeout_sec,
+        ).run()
+
+        logger.debug(
+            f'Key [{key}]: Timeout: {timeout_sec}. '
+            f'Data extended. Now: {len(extended)}'
+        )
+
+        return extended
+
     async def extract(self, key: str) -> JSON:
         """Load data from Redis and delete its key."""
 
         data: JSON = await self.load(key)
         await self.delete(key)
 
         return data
```

### Comparing `redis_async_client-0.1.4/src/redis_async_client/core/settings.py` & `redis_async_client-0.1.5/src/redis_async_client/core/settings.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.4/PKG-INFO` & `redis_async_client-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-async-client
-Version: 0.1.4
+Version: 0.1.5
 Summary: Redis async client.
 Home-page: https://pypi.org/project/redis-async-client/
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: redis-async-client Version: 0.1.4 Summary: Redis
+Metadata-Version: 2.1 Name: redis-async-client Version: 0.1.5 Summary: Redis
 async client. Home-page: https://pypi.org/project/redis-async-client/ License:
 MIT Author: deskent Author-email: battenetciz@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: redis (>=5.0.3,<6.0.0)
 Project-URL: Repository, https://github.com/Deskent/redis_async_client
```

