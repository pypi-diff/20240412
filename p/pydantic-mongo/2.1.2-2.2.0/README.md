# Comparing `tmp/pydantic-mongo-2.1.2.tar.gz` & `tmp/pydantic-mongo-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-mongo-2.1.2.tar", last modified: Wed Mar  6 20:45:55 2024, max compression
+gzip compressed data, was "pydantic-mongo-2.2.0.tar", last modified: Thu Apr 11 22:54:04 2024, max compression
```

## Comparing `pydantic-mongo-2.1.2.tar` & `pydantic-mongo-2.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/pydantic_mongo/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/abstract_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pydantic_mongo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-03-06 20:45:55.000000 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-06 20:45:55.000000 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 20:45:55.000000 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-06 20:45:55.000000 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-06 20:45:55.000000 pydantic-mongo-2.1.2/pydantic_mongo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 20:45:55.692107 pydantic-mongo-2.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/test/test_enhance_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/test/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/test/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     7580 2024-03-06 20:45:48.000000 pydantic-mongo-2.1.2/test/test_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/pydantic_mongo/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/abstract_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pydantic_mongo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 22:54:04.000000 pydantic-mongo-2.2.0/pydantic_mongo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:54:04.614344 pydantic-mongo-2.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_enhance_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-11 22:53:58.000000 pydantic-mongo-2.2.0/test/test_repository.py
```

### Comparing `pydantic-mongo-2.1.2/LICENSE.md` & `pydantic-mongo-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/PKG-INFO` & `pydantic-mongo-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo
-Version: 2.1.2
+Version: 2.2.0
 Summary: Document object mapper for pydantic and pymongo
 Home-page: https://github.com/jefersondaniel/pydantic-mongo
 Author: Jeferson Daniel
 Author-email: jeferson.daniel412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydantic-mongo-2.1.2/README.md` & `pydantic-mongo-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/pydantic_mongo/abstract_repository.py` & `pydantic-mongo-2.2.0/pydantic_mongo/abstract_repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,17 @@
             for mongo_id, document in zip(mongo_ids, documents_to_update)
         ]
         self.get_collection().bulk_write(bulk_operations)
 
     def delete(self, model: T):
         return self.get_collection().delete_one({"_id": model.id})
 
+    def delete_by_id(self, _id: Any):
+        return self.get_collection().delete_one({"_id": _id})
+
     def find_one_by_id(self, _id: Any) -> Optional[T]:
         """
         Find entity by id
 
         Note: The id should be of the same type as the id field in the document class, ie. ObjectId
         """
         return self.find_one_by({"id": _id})
```

### Comparing `pydantic-mongo-2.1.2/pydantic_mongo/fields.py` & `pydantic-mongo-2.2.0/pydantic_mongo/fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/pydantic_mongo/pagination.py` & `pydantic-mongo-2.2.0/pydantic_mongo/pagination.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/pydantic_mongo.egg-info/PKG-INFO` & `pydantic-mongo-2.2.0/pydantic_mongo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo
-Version: 2.1.2
+Version: 2.2.0
 Summary: Document object mapper for pydantic and pymongo
 Home-page: https://github.com/jefersondaniel/pydantic-mongo
 Author: Jeferson Daniel
 Author-email: jeferson.daniel412@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydantic-mongo-2.1.2/pydantic_mongo.egg-info/SOURCES.txt` & `pydantic-mongo-2.2.0/pydantic_mongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/setup.py` & `pydantic-mongo-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/test/test_enhance_meta.py` & `pydantic-mongo-2.2.0/test/test_enhance_meta.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/test/test_fields.py` & `pydantic-mongo-2.2.0/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/test/test_pagination.py` & `pydantic-mongo-2.2.0/test/test_pagination.py`

 * *Files identical despite different names*

### Comparing `pydantic-mongo-2.1.2/test/test_repository.py` & `pydantic-mongo-2.2.0/test/test_repository.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,28 @@
         result = spam_repository.find_one_by_id(spam.id)
         assert result is not None
 
         spam_repository.delete(spam)
         result = spam_repository.find_one_by_id(spam.id)
         assert result is None
 
+    def test_delete_by_id(self, database):
+        spam_repository = SpamRepository(database=database)
+        foo = Foo(count=1, size=1.0)
+        bar = Bar()
+        spam = Spam(foo=foo, bars=[bar])
+        spam_repository.save(spam)
+
+        result = spam_repository.find_one_by_id(spam.id)
+        assert result is not None
+
+        spam_repository.delete_by_id(spam.id)
+        result = spam_repository.find_one_by_id(spam.id)
+        assert result is None
+
     def test_find_by_id(self, database):
         spam_id = ObjectId("611827f2878b88b49ebb69fc")
         database.spams.insert_one(
             {
                 "_id": spam_id,
                 "foo": {"count": 2, "size": 1.0},
                 "bars": [{"apple": "x", "banana": "y"}],
```

