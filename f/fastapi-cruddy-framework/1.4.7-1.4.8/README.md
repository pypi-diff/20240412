# Comparing `tmp/fastapi_cruddy_framework-1.4.7.tar.gz` & `tmp/fastapi_cruddy_framework-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-1.4.7.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-1.4.8.tar", max compression
```

## Comparing `fastapi_cruddy_framework-1.4.7.tar` & `fastapi_cruddy_framework-1.4.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.7/LICENSE
--rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.7/README.md
--rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    44639 2024-04-12 16:37:02.252154 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/graphql.py
--rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/pubsub.py
--rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/test_helpers.py
--rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/websocket_manager.py
--rw-r--r--   0        0        0     2252 2024-04-12 16:37:41.085216 fastapi_cruddy_framework-1.4.7/pyproject.toml
--rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-03 18:31:12.339513 fastapi_cruddy_framework-1.4.8/LICENSE
+-rw-r--r--   0        0        0    54838 2024-04-03 17:29:13.060260 fastapi_cruddy_framework-1.4.8/README.md
+-rw-r--r--   0        0        0     2483 2024-03-20 18:15:08.576001 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     6747 2024-01-06 16:48:05.591411 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    44781 2024-04-12 17:41:34.217544 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0    15521 2024-04-03 20:42:09.978482 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/graphql.py
+-rw-r--r--   0        0        0       46 2023-03-03 18:31:12.343965 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0     3575 2024-01-06 19:00:34.485202 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/pubsub.py
+-rw-r--r--   0        0        0    36269 2024-03-29 20:29:49.898024 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    31716 2024-04-10 18:04:33.796733 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2375 2023-10-24 11:53:06.377545 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     5687 2024-04-03 17:41:13.269559 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0    11050 2023-12-12 17:22:31.207802 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/test_helpers.py
+-rw-r--r--   0        0        0     8260 2024-04-10 15:33:48.817894 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0    16184 2024-01-30 17:02:35.391956 fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/websocket_manager.py
+-rw-r--r--   0        0        0     2252 2024-04-12 17:42:31.230211 fastapi_cruddy_framework-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0    56415 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-1.4.8/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-1.4.7/LICENSE` & `fastapi_cruddy_framework-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/README.md` & `fastapi_cruddy_framework-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -724,15 +724,19 @@
                     must_be if shim_where is None else {"*and": [must_be, shim_where]}
                 )
                 query_conf["where"] = shim_where
                 return
 
             _repo_lifecycle_before = _shimmed_repo_lifecycle_before
         else:
-            where = must_be if where is None else {"*and": [must_be, where]}
+            context_data[DATA_KEY]["where"] = (
+                must_be
+                if context_data[DATA_KEY]["where"] is None
+                else {"*and": [must_be, context_data[DATA_KEY]["where"]]}
+            )
 
         # Collect the bulk data transfer object from the query
         result: BulkDTO = await config.foreign_resource.repository.get_all(
             page=1,
             limit=1,
             columns=columns,
             sort=None,
```

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/graphql.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/graphql.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/pubsub.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/pubsub.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/test_helpers.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/util.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/util.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/fastapi_cruddy_framework/websocket_manager.py` & `fastapi_cruddy_framework-1.4.8/fastapi_cruddy_framework/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-1.4.7/pyproject.toml` & `fastapi_cruddy_framework-1.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "1.4.7"
+version = "1.4.8"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-1.4.7/PKG-INFO` & `fastapi_cruddy_framework-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 1.4.7
+Version: 1.4.8
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.7 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 1.4.8 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

