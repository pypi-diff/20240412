# Comparing `tmp/motion-lake-client-0.0.4.tar.gz` & `tmp/motion_lake_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion-lake-client-0.0.4.tar", last modified: Mon Apr  8 18:10:37 2024, max compression
+gzip compressed data, was "motion_lake_client-0.0.5.tar", last modified: Fri Apr 12 17:44:19 2024, max compression
```

## Comparing `motion-lake-client-0.0.4.tar` & `motion_lake_client-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion-lake-client-0.0.4/LICENSE
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion-lake-client-0.0.4/README.md
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-08 18:10:02.000000 motion-lake-client-0.0.4/pyproject.toml
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/setup.cfg
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion-lake-client-0.0.4/setup.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.490542 motion-lake-client-0.0.4/src/
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/src/motion_lake_client/
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion-lake-client-0.0.4/src/motion_lake_client/__init__.py
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     8869 2024-04-08 18:10:02.000000 motion-lake-client-0.0.4/src/motion_lake_client/client.py
-drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-08 18:10:37.498542 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/
--rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/PKG-INFO
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/SOURCES.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/dependency_links.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/requires.txt
--rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-08 18:10:37.000000 motion-lake-client-0.0.4/src/motion_lake_client.egg-info/top_level.txt
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:44:19.893393 motion_lake_client-0.0.5/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      516 2024-04-05 16:21:57.000000 motion_lake_client-0.0.5/LICENSE
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-12 17:44:19.893393 motion_lake_client-0.0.5/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)     1842 2024-04-05 16:52:44.000000 motion_lake_client-0.0.5/README.md
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      744 2024-04-12 17:44:16.000000 motion_lake_client-0.0.5/pyproject.toml
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       38 2024-04-12 17:44:19.893393 motion_lake_client-0.0.5/setup.cfg
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       37 2024-04-05 16:27:42.000000 motion_lake_client-0.0.5/setup.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:44:19.889393 motion_lake_client-0.0.5/src/
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:44:19.889393 motion_lake_client-0.0.5/src/motion_lake_client/
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       22 2024-04-05 16:23:48.000000 motion_lake_client-0.0.5/src/motion_lake_client/__init__.py
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)    10394 2024-04-12 17:43:58.000000 motion_lake_client-0.0.5/src/motion_lake_client/client.py
+drwxrwxr-x   0 gaspard   (1000) gaspard   (1000)        0 2024-04-12 17:44:19.893393 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/
+-rw-r--r--   0 gaspard   (1000) gaspard   (1000)     3025 2024-04-12 17:44:19.000000 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/PKG-INFO
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)      338 2024-04-12 17:44:19.000000 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        1 2024-04-12 17:44:19.000000 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)        9 2024-04-12 17:44:19.000000 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/requires.txt
+-rw-rw-r--   0 gaspard   (1000) gaspard   (1000)       19 2024-04-12 17:44:19.000000 motion_lake_client-0.0.5/src/motion_lake_client.egg-info/top_level.txt
```

### Comparing `motion-lake-client-0.0.4/LICENSE` & `motion_lake_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `motion-lake-client-0.0.4/PKG-INFO` & `motion_lake_client-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

### Comparing `motion-lake-client-0.0.4/README.md` & `motion_lake_client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `motion-lake-client-0.0.4/pyproject.toml` & `motion_lake_client-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion-lake-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)"
 readme = "README.md"
 authors = [{ name = "Gaspard Merten", email = "gaspard.mp.work@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
```

### Comparing `motion-lake-client-0.0.4/src/motion_lake_client/client.py` & `motion_lake_client-0.0.5/src/motion_lake_client/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 import dataclasses
 from datetime import datetime
 from enum import Enum
 from typing import Protocol, Dict, Any, List
 
 import requests
 
-__all__ = ['Item', 'Collection', 'NetworkClient', 'RequestsClient', 'InnerClient', 'BaseClient']
+__all__ = [
+    "Item",
+    "Collection",
+    "NetworkClient",
+    "RequestsClient",
+    "InnerClient",
+    "BaseClient",
+    "ContentType",
+    "MAX_DATE",
+    "MIN_DATE",
+]
 
 # Hopefully, we have better storage systems in 2250...
 MAX_DATE = datetime(2250, 12, 31, 23, 59, 59, 999999)
 MIN_DATE = datetime(1971, 1, 1, 0, 0, 0, 0)
 
 
 @dataclasses.dataclass
 class Item:
     """
     A data item in the collection.
     """
+
     timestamp: datetime
     data: bytes
 
 
 @dataclasses.dataclass
 class Collection:
     """
     A summary of a collection. A collection is a group of items.
     """
+
     name: str
     min_timestamp: datetime
     max_timestamp: datetime
     count: int
 
 
 class ContentType(Enum):
@@ -41,19 +53,17 @@
 
 
 class NetworkClient(Protocol):
     """
     A network client to make requests to the storage server.
     """
 
-    def get(self, url: str, query_params: Dict[str, Any] = None) -> dict:
-        ...
+    def get(self, url: str, query_params: Dict[str, Any] = None) -> dict: ...
 
-    def post(self, url: str, body: dict) -> dict:
-        ...
+    def post(self, url: str, body: dict) -> dict: ...
 
 
 class RequestsClient(NetworkClient):
     """
     A network client using the requests library.
     """
 
@@ -94,33 +104,50 @@
         """
         Create a new collection with the given name.
         :param collection_name: The name of the collection to create
         :return: None
         """
         return self.network_client.post(f"/collection/", {"name": collection_name})
 
-    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: ContentType = None,
-              create_collection: bool = False) -> dict:
+    def store(
+        self,
+        collection_name: str,
+        data: bytes,
+        timestamp: int,
+        content_type: ContentType = None,
+        create_collection: bool = False,
+    ) -> dict:
         """
         Store the given data in the collection with the given name.
         :param collection_name: The name of the collection to store the data in
         :param data: The data to store
         :param timestamp: The timestamp to associate with the data
         :param content_type: The type of the data
         :param create_collection: Whether to create the collection if it does not exist
         :return: None
         """
         return self.network_client.post(
             f"/store/{collection_name}/",
-            {"data": data.hex(), "timestamp": timestamp, "content_type": content_type.value if content_type else None,
-             "create_collection": create_collection, }
+            {
+                "data": data.hex(),
+                "timestamp": timestamp,
+                "content_type": content_type.value if content_type else None,
+                "create_collection": create_collection,
+            },
         )
 
-    def query(self, collection_name: str, min_timestamp: int, max_timestamp: int, ascending: bool,
-              limit: int = None, offset: int = None) -> dict:
+    def query(
+        self,
+        collection_name: str,
+        min_timestamp: int,
+        max_timestamp: int,
+        ascending: bool,
+        limit: int = None,
+        offset: int = None,
+    ) -> dict:
         """
         Query the data in the collection with the given name.
         :param collection_name: The name of the collection to query
         :param min_timestamp: The minimum timestamp to filter the data
         :param max_timestamp: The maximum timestamp to filter the data
         :param ascending: Whether to sort the data in ascending order
         :param limit: The limit of the data to retrieve
@@ -130,102 +157,174 @@
         return self.network_client.get(
             f"/query/{collection_name}/",
             {
                 "min_timestamp": min_timestamp,
                 "max_timestamp": max_timestamp,
                 "ascending": ascending,
                 "limit": limit or 1,
-                "offset": offset or 0
-            }
+                "offset": offset or 0,
+            },
         )
 
     def get_collections(self) -> List[Collection]:
         """
         Get a list of all collections.
         :return: A list of collections
         """
         collections = self.network_client.get("/collections/")
         return [
             Collection(
                 name=collection["name"],
-                min_timestamp=datetime.fromisoformat(collection["min_timestamp"]) if collection[
-                    "min_timestamp"] else None,
-                max_timestamp=datetime.fromisoformat(collection["max_timestamp"]) if collection[
-                    "max_timestamp"] else None,
-                count=collection["count"]
+                min_timestamp=(
+                    datetime.fromisoformat(collection["min_timestamp"])
+                    if collection["min_timestamp"]
+                    else None
+                ),
+                max_timestamp=(
+                    datetime.fromisoformat(collection["max_timestamp"])
+                    if collection["max_timestamp"]
+                    else None
+                ),
+                count=collection["count"],
             )
             for collection in collections
         ]
 
+    def advanced_query(
+        self,
+        collection_name: str,
+        query: str,
+        min_timestamp: datetime,
+        max_timestamp: datetime,
+    ):
+        assert (
+            "[table]" in query
+        ), """Query must contain [table] placeholder (it will be replaced with a view on a 
+        table)"""
+
+        return self.network_client.post(
+            f"/advanced/{collection_name}/",
+            {
+                "query": query,
+                "min_timestamp": int(min_timestamp.timestamp() * 1000),
+                "max_timestamp": int(max_timestamp.timestamp() * 1000),
+            },
+        )
+
 
 class BaseClient:
-    def __init__(self, lake_url: str = 'http://localhost:8000'):
+    def __init__(self, lake_url: str = "http://localhost:8000"):
         """
         Initialize the client with the base URL of the storage server.
         :param lake_url: The base URL of the storage server
         """
         self.inner_client = InnerClient(RequestsClient(lake_url))
 
     @staticmethod
     def _parse_server_timestamp(timestamp: int) -> datetime:
         return datetime.fromtimestamp(timestamp)
 
     def _parse_results(self, results: List[dict]) -> List[Item]:
-        print([result["timestamp"] for result in results])
         return [
             Item(
                 timestamp=self._parse_server_timestamp(item["timestamp"]),
-                data=bytes.fromhex(item["data"])
+                data=bytes.fromhex(item["data"]),
             )
             for item in results
         ]
 
     def flush_buffer(self, collection_name: str) -> dict:
         return self.inner_client.flush_buffer(collection_name)
 
     def create_collection(self, collection_name: str) -> dict:
         return self.inner_client.create_collection(collection_name)
 
-    def store(self, collection_name: str, data: bytes, timestamp: int, content_type: str = None,
-              create_collection: bool = False) -> dict:
-        return self.inner_client.store(collection_name, data, timestamp, content_type, create_collection)
+    def store(
+        self,
+        collection_name: str,
+        data: bytes,
+        timestamp: int,
+        content_type: ContentType = None,
+        create_collection: bool = False,
+    ) -> dict:
+        return self.inner_client.store(
+            collection_name, data, timestamp, content_type, create_collection
+        )
 
-    def query(self, collection_name: str, min_datetime: datetime, max_datetime: datetime, ascending: bool,
-              limit: int = None, offset: int = 0) -> dict:
+    def query(
+        self,
+        collection_name: str,
+        min_datetime: datetime,
+        max_datetime: datetime,
+        ascending: bool,
+        limit: int = None,
+        offset: int = 0,
+    ) -> dict:
         min_datetime = min_datetime or MIN_DATE
         max_datetime = max_datetime or MAX_DATE
 
-        return self.inner_client.query(collection_name, int(min_datetime.timestamp() * 1000),
-                                       int(max_datetime.timestamp() * 1000),
-                                       ascending, limit, offset)
+        return self.inner_client.query(
+            collection_name,
+            int(min_datetime.timestamp() * 1000),
+            int(max_datetime.timestamp() * 1000),
+            ascending,
+            limit,
+            offset,
+        )
 
     def get_last_items(self, collection_name: str, limit: int) -> List[Item]:
         response = self.query(collection_name, MIN_DATE, datetime.now(), False, limit)
-        return self._parse_results(response['results'])
+        return self._parse_results(response["results"])
 
     def get_last_item(self, collection_name: str) -> Item:
         results = self.get_last_items(collection_name, 1)
         return (results or [None])[0]
 
     def get_first_items(self, collection_name: str, limit: int) -> List[Item]:
         response = self.query(collection_name, MIN_DATE, datetime.now(), True, limit)
-        return self._parse_results(response['results'])
+        return self._parse_results(response["results"])
 
     def get_first_item(self, collection_name: str) -> Item:
         items = self.get_first_items(collection_name, 1)
 
         return (items or [None])[0]
 
-    def get_items_between(self, collection_name: str, min_datetime: datetime, max_datetime: datetime,
-                          ascending: bool = True,
-                          limit: int = None, offset: int = None) -> List[Item]:
-        response = self.query(collection_name, min_datetime, max_datetime, ascending, limit, offset)
-        return self._parse_results(response['results'])
+    def get_items_between(
+        self,
+        collection_name: str,
+        min_datetime: datetime,
+        max_datetime: datetime,
+        ascending: bool = True,
+        limit: int = None,
+        offset: int = None,
+    ) -> List[Item]:
+        response = self.query(
+            collection_name, min_datetime, max_datetime, ascending, limit, offset
+        )
+        return self._parse_results(response["results"])
 
-    def get_items_before(self, collection_name: str, date: datetime, limit: int) -> List[Item]:
+    def get_items_before(
+        self, collection_name: str, date: datetime, limit: int
+    ) -> List[Item]:
         return self.get_items_between(collection_name, MIN_DATE, date, False, limit)
 
-    def get_items_after(self, collection_name: str, timestamp: datetime, limit: int) -> List[Item]:
+    def get_items_after(
+        self, collection_name: str, timestamp: datetime, limit: int
+    ) -> List[Item]:
         return self.get_items_between(collection_name, timestamp, MAX_DATE, True, limit)
 
     def get_collections(self) -> List[Collection]:
         return self.inner_client.get_collections()
+
+    def advanced_query(
+        self,
+        collection_name: str,
+        query: str,
+        min_timestamp: datetime,
+        max_timestamp: datetime,
+    ):
+        assert (
+            "[table]" in query
+        ), """Query must contain [table] placeholder (it will be replaced with a view on a table)"""
+        return self.inner_client.advanced_query(
+            collection_name, query, min_timestamp, max_timestamp
+        )
```

### Comparing `motion-lake-client-0.0.4/src/motion_lake_client.egg-info/PKG-INFO` & `motion_lake_client-0.0.5/src/motion_lake_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-lake-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Motion Lake Client, a client for the Motion Lake API (a Mobility Data Lake)
 Author-email: Gaspard Merten <gaspard.mp.work@gmail.com>
 License: All Rights Reserved
         
         Copyright (c) 2024 Gaspard Merten
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
```

