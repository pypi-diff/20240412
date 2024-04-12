# Comparing `tmp/tcvectordb-1.3.0.tar.gz` & `tmp/tcvectordb-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcvectordb-1.3.0.tar", last modified: Mon Feb 26 02:50:02 2024, max compression
+gzip compressed data, was "tcvectordb-1.3.2.tar", last modified: Fri Apr 12 03:05:30 2024, max compression
```

## Comparing `tcvectordb-1.3.0.tar` & `tcvectordb-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,48 @@
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.701194 tcvectordb-1.3.0/
--rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-02-23 11:11:52.000000 tcvectordb-1.3.0/LICENSE
--rw-r--r--   0 wanglei    (501) staff       (20)      171 2024-02-26 02:50:02.701074 tcvectordb-1.3.0/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)      386 2024-02-23 11:11:57.000000 tcvectordb-1.3.0/README.md
--rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-02-26 02:50:02.701237 tcvectordb-1.3.0/setup.cfg
--rw-r--r--   0 wanglei    (501) staff       (20)      394 2024-02-23 11:12:30.000000 tcvectordb-1.3.0/setup.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.696743 tcvectordb-1.3.0/tcvectordb/
--rw-r--r--   0 wanglei    (501) staff       (20)     1266 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/__init__.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.698041 tcvectordb-1.3.0/tcvectordb/client/
--rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/client/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)     5660 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/client/httpclient.py
--rw-r--r--   0 wanglei    (501) staff       (20)     4865 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/client/stub.py
--rw-r--r--   0 wanglei    (501) staff       (20)      604 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/debug.py
--rw-r--r--   0 wanglei    (501) staff       (20)     1141 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/exceptions.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.700175 tcvectordb-1.3.0/tcvectordb/model/
--rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)     8970 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/ai_database.py
--rw-r--r--   0 wanglei    (501) staff       (20)    23771 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/collection.py
--rw-r--r--   0 wanglei    (501) staff       (20)    20546 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/collection_view.py
--rw-r--r--   0 wanglei    (501) staff       (20)    12881 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/database.py
--rw-r--r--   0 wanglei    (501) staff       (20)     2738 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/document.py
--rw-r--r--   0 wanglei    (501) staff       (20)    11436 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/document_set.py
--rw-r--r--   0 wanglei    (501) staff       (20)     1397 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/enum.py
--rw-r--r--   0 wanglei    (501) staff       (20)     5901 2024-02-23 11:12:40.000000 tcvectordb-1.3.0/tcvectordb/model/index.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.697515 tcvectordb-1.3.0/tcvectordb.egg-info/
--rw-r--r--   0 wanglei    (501) staff       (20)      171 2024-02-26 02:50:02.000000 tcvectordb-1.3.0/tcvectordb.egg-info/PKG-INFO
--rw-r--r--   0 wanglei    (501) staff       (20)      723 2024-02-26 02:50:02.000000 tcvectordb-1.3.0/tcvectordb.egg-info/SOURCES.txt
--rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-02-26 02:50:02.000000 tcvectordb-1.3.0/tcvectordb.egg-info/dependency_links.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       35 2024-02-26 02:50:02.000000 tcvectordb-1.3.0/tcvectordb.egg-info/requires.txt
--rw-r--r--   0 wanglei    (501) staff       (20)       17 2024-02-26 02:50:02.000000 tcvectordb-1.3.0/tcvectordb.egg-info/top_level.txt
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.700348 tcvectordb-1.3.0/tests/
--rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-02-23 11:12:44.000000 tcvectordb-1.3.0/tests/__init__.py
-drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-02-26 02:50:02.700820 tcvectordb-1.3.0/tests/model/
--rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-02-23 11:12:44.000000 tcvectordb-1.3.0/tests/model/__init__.py
--rw-r--r--   0 wanglei    (501) staff       (20)     2985 2024-02-23 11:12:44.000000 tcvectordb-1.3.0/tests/model/test_collection.py
--rw-r--r--   0 wanglei    (501) staff       (20)     1851 2024-02-23 11:12:44.000000 tcvectordb-1.3.0/tests/model/test_document.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.242679 tcvectordb-1.3.2/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:07:26.000000 tcvectordb-1.3.2/LICENSE
+-rw-r--r--   0 wanglei    (501) staff       (20)      171 2024-04-12 03:05:30.242550 tcvectordb-1.3.2/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)      386 2024-04-08 07:07:31.000000 tcvectordb-1.3.2/README.md
+-rw-r--r--   0 wanglei    (501) staff       (20)       38 2024-04-12 03:05:30.242734 tcvectordb-1.3.2/setup.cfg
+-rw-r--r--   0 wanglei    (501) staff       (20)      394 2024-04-12 03:05:03.000000 tcvectordb-1.3.2/setup.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.235628 tcvectordb-1.3.2/tcvectordb/
+-rw-r--r--   0 wanglei    (501) staff       (20)     1266 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/__init__.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.236623 tcvectordb-1.3.2/tcvectordb/asyncapi/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/__init__.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.236816 tcvectordb-1.3.2/tcvectordb/asyncapi/client/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/client/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     2172 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/client/stub.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.238414 tcvectordb-1.3.2/tcvectordb/asyncapi/model/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-12 03:02:20.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     3679 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/ai_database.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5196 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/collection.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     6056 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/collection_view.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     4185 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/database.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     2320 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/asyncapi/model/document_set.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.239124 tcvectordb-1.3.2/tcvectordb/client/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/client/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5660 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/client/httpclient.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     4865 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/client/stub.py
+-rw-r--r--   0 wanglei    (501) staff       (20)      604 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/debug.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     1141 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/exceptions.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.241411 tcvectordb-1.3.2/tcvectordb/model/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     8970 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/ai_database.py
+-rw-r--r--   0 wanglei    (501) staff       (20)    23771 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/collection.py
+-rw-r--r--   0 wanglei    (501) staff       (20)    20546 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/collection_view.py
+-rw-r--r--   0 wanglei    (501) staff       (20)    12341 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/database.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     2738 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/document.py
+-rw-r--r--   0 wanglei    (501) staff       (20)    11435 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/document_set.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     1397 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/enum.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     5901 2024-04-08 07:08:19.000000 tcvectordb-1.3.2/tcvectordb/model/index.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.236487 tcvectordb-1.3.2/tcvectordb.egg-info/
+-rw-r--r--   0 wanglei    (501) staff       (20)      171 2024-04-12 03:05:30.000000 tcvectordb-1.3.2/tcvectordb.egg-info/PKG-INFO
+-rw-r--r--   0 wanglei    (501) staff       (20)     1073 2024-04-12 03:05:30.000000 tcvectordb-1.3.2/tcvectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)        1 2024-04-12 03:05:30.000000 tcvectordb-1.3.2/tcvectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       35 2024-04-12 03:05:30.000000 tcvectordb-1.3.2/tcvectordb.egg-info/requires.txt
+-rw-r--r--   0 wanglei    (501) staff       (20)       17 2024-04-12 03:05:30.000000 tcvectordb-1.3.2/tcvectordb.egg-info/top_level.txt
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.241748 tcvectordb-1.3.2/tests/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:24.000000 tcvectordb-1.3.2/tests/__init__.py
+drwxr-xr-x   0 wanglei    (501) staff       (20)        0 2024-04-12 03:05:30.242206 tcvectordb-1.3.2/tests/model/
+-rw-r--r--   0 wanglei    (501) staff       (20)        0 2024-04-08 07:08:24.000000 tcvectordb-1.3.2/tests/model/__init__.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     2985 2024-04-08 07:08:24.000000 tcvectordb-1.3.2/tests/model/test_collection.py
+-rw-r--r--   0 wanglei    (501) staff       (20)     1851 2024-04-08 07:08:24.000000 tcvectordb-1.3.2/tests/model/test_document.py
```

### Comparing `tcvectordb-1.3.0/tcvectordb/__init__.py` & `tcvectordb-1.3.2/tcvectordb/__init__.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/client/httpclient.py` & `tcvectordb-1.3.2/tcvectordb/client/httpclient.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/client/stub.py` & `tcvectordb-1.3.2/tcvectordb/client/stub.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/debug.py` & `tcvectordb-1.3.2/tcvectordb/debug.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/exceptions.py` & `tcvectordb-1.3.2/tcvectordb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/ai_database.py` & `tcvectordb-1.3.2/tcvectordb/model/ai_database.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/collection.py` & `tcvectordb-1.3.2/tcvectordb/model/collection.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/collection_view.py` & `tcvectordb-1.3.2/tcvectordb/model/collection_view.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/database.py` & `tcvectordb-1.3.2/tcvectordb/model/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,35 @@
             'indexes': index.list()
         }
         self._conn.post('/collection/create', body, timeout)
 
         return Collection(self, name, shard, replicas, description, index, embedding=embedding,
                           read_consistency=self._read_consistency)
 
+    def _generate_collection(self, col):
+        index = Index()
+        for elem in col.get('indexes', []):
+            index.add(**elem)
+        ebd = Embedding()
+        if "embedding" in col:
+            ebd.set_fields(**col.get("embedding"))
+        collection = Collection(
+            self,
+            col['collection'],
+            shard=col['shardNum'],
+            replicas=col['replicaNum'],
+            description=col.get('description'),
+            index=index,
+            embedding=ebd,
+            create_time=col['createTime'],
+            read_consistency=self._read_consistency
+        )
+        collection.set_fields(**col)
+        return collection
+
     def list_collections(self, timeout: Optional[float] = None) -> List[Collection]:
         """Get collection list.
 
         :param timeout: An optional duration of time in seconds to allow for the request. When timeout
                         is set to None, will use the connect timeout.
         :type  timeout: float
 
@@ -178,36 +199,15 @@
             raise exceptions.ParamError(message='database not found')
         body = {
             'database': self.database_name
         }
         res = self._conn.post('/collection/list', body, timeout)
         collections = []
         for col in res.body['collections']:
-            index = Index()
-            for elem in col.get('indexes', []):
-                index.add(**elem)
-
-            ebd = Embedding()
-            if "embedding" in col:
-                ebd.set_fields(**col.get("embedding"))
-
-            collection = Collection(
-                self,
-                col['collection'],
-                shard=col['shardNum'],
-                replicas=col['replicaNum'],
-                description=col.get('description'),
-                index=index,
-                embedding=ebd,
-                create_time=col['createTime'],
-                read_consistency=self._read_consistency
-            )
-
-            collection.set_fields(**col)
-
+            collection = self._generate_collection(col)
             collections.append(collection)
 
         return collections
 
     def describe_collection(self, name: str, timeout: Optional[float] = None) -> Collection:
         """Get a collection details.
         :param name: The name of the collection.
@@ -230,36 +230,15 @@
             'collection': name,
         }
         res = self._conn.post('/collection/describe', body, timeout)
         if not res.body['collection']:
             raise exceptions.DescribeCollectionException(
                 code=-1, message=str(res.body))
         col = res.body['collection']
-        index = Index()
-        for elem in col.get('indexes', []):
-            index.add(**elem)
-
-        ebd = Embedding()
-        if "embedding" in col:
-            ebd.set_fields(**col.get("embedding"))
-
-        collection = Collection(
-            self,
-            col['collection'],
-            shard=col['shardNum'],
-            replicas=col['replicaNum'],
-            description=col.get('description'),
-            index=index,
-            embedding=ebd,
-            create_time=col['createTime'],
-            read_consistency=self._read_consistency
-        )
-        collection.set_fields(**col)
-
-        return collection
+        return self._generate_collection(col)
 
     def drop_collection(self, name: str, timeout: Optional[float] = None):
         """Delete a collection.
         :param name: The name of the collection.
         :type: str
 
         :param timeout: An optional duration of time in seconds to allow for the request. When timeout
```

### Comparing `tcvectordb-1.3.0/tcvectordb/model/document.py` & `tcvectordb-1.3.2/tcvectordb/model/document.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/document_set.py` & `tcvectordb-1.3.2/tcvectordb/model/document_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,14 @@
                 indexed_error_msg=info.get('indexedErrorMsg')
             )
             self.document_set_info = dsi
         if splitter_process is not None:
             self.splitter_process = splitter_process
         self._set_scalar_fields(data)
 
-
     def get_text(self) -> str:
         ds = self.collection_view.get_document_set(document_set_id=self.id)
         self.load_fields(vars(ds))
         return self.text
 
     def delete(self) -> Dict[str, Any]:
         return self.collection_view.delete(document_set_id=self.id)
```

### Comparing `tcvectordb-1.3.0/tcvectordb/model/enum.py` & `tcvectordb-1.3.2/tcvectordb/model/enum.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb/model/index.py` & `tcvectordb-1.3.2/tcvectordb/model/index.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tcvectordb.egg-info/SOURCES.txt` & `tcvectordb-1.3.2/tcvectordb.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 tcvectordb/debug.py
 tcvectordb/exceptions.py
 tcvectordb.egg-info/PKG-INFO
 tcvectordb.egg-info/SOURCES.txt
 tcvectordb.egg-info/dependency_links.txt
 tcvectordb.egg-info/requires.txt
 tcvectordb.egg-info/top_level.txt
+tcvectordb/asyncapi/__init__.py
+tcvectordb/asyncapi/client/__init__.py
+tcvectordb/asyncapi/client/stub.py
+tcvectordb/asyncapi/model/__init__.py
+tcvectordb/asyncapi/model/ai_database.py
+tcvectordb/asyncapi/model/collection.py
+tcvectordb/asyncapi/model/collection_view.py
+tcvectordb/asyncapi/model/database.py
+tcvectordb/asyncapi/model/document_set.py
 tcvectordb/client/__init__.py
 tcvectordb/client/httpclient.py
 tcvectordb/client/stub.py
 tcvectordb/model/__init__.py
 tcvectordb/model/ai_database.py
 tcvectordb/model/collection.py
 tcvectordb/model/collection_view.py
```

### Comparing `tcvectordb-1.3.0/tests/model/test_collection.py` & `tcvectordb-1.3.2/tests/model/test_collection.py`

 * *Files identical despite different names*

### Comparing `tcvectordb-1.3.0/tests/model/test_document.py` & `tcvectordb-1.3.2/tests/model/test_document.py`

 * *Files identical despite different names*

