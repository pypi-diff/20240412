# Comparing `tmp/kodexa-7.0.8621391210.tar.gz` & `tmp/kodexa-7.0.8664569946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.8621391210.tar", max compression
+gzip compressed data, was "kodexa-7.0.8664569946.tar", max compression
```

## Comparing `kodexa-7.0.8621391210.tar` & `kodexa-7.0.8664569946.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-04-09 19:45:59.038848 kodexa-7.0.8621391210/LICENSE
--rw-r--r--   0        0        0     2178 2024-04-09 19:45:59.038848 kodexa-7.0.8621391210/README.md
--rw-r--r--   0        0        0      957 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-04-09 19:45:59.042848 kodexa-7.0.8621391210/kodexa/model/base.py
--rw-r--r--   0        0        0   115528 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/model.py
--rw-r--r--   0        0        0   174857 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/objects.py
--rw-r--r--   0        0        0    61967 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   213246 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    33933 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 19:45:59.046848 kodexa-7.0.8621391210/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1389 2024-04-09 19:46:15.122881 kodexa-7.0.8621391210/pyproject.toml
--rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8621391210/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-12 15:40:54.407065 kodexa-7.0.8664569946/LICENSE
+-rw-r--r--   0        0        0     2178 2024-04-12 15:40:54.407065 kodexa-7.0.8664569946/README.md
+-rw-r--r--   0        0        0      957 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/model/base.py
+-rw-r--r--   0        0        0   115528 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/model/model.py
+-rw-r--r--   0        0        0   174857 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-04-12 15:40:54.411065 kodexa-7.0.8664569946/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   213246 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    33933 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:40:54.415065 kodexa-7.0.8664569946/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1389 2024-04-12 15:41:09.731026 kodexa-7.0.8664569946/pyproject.toml
+-rw-r--r--   0        0        0     3493 1970-01-01 00:00:00.000000 kodexa-7.0.8664569946/PKG-INFO
```

### Comparing `kodexa-7.0.8621391210/LICENSE` & `kodexa-7.0.8664569946/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/README.md` & `kodexa-7.0.8664569946/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/__init__.py` & `kodexa-7.0.8664569946/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/assistant/assistant.py` & `kodexa-7.0.8664569946/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/connectors/connectors.py` & `kodexa-7.0.8664569946/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/model/__init__.py` & `kodexa-7.0.8664569946/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/model/base.py` & `kodexa-7.0.8664569946/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/model/model.py` & `kodexa-7.0.8664569946/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/model/objects.py` & `kodexa-7.0.8664569946/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/model/persistence.py` & `kodexa-7.0.8664569946/kodexa/model/persistence.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,17 @@
         disk_conn = sqlite3.connect(disk_db_path)
         disk_cursor = disk_conn.cursor()
 
         # Load the contents of the disk database into memory
         disk_cursor.execute("SELECT name, sql FROM sqlite_master WHERE type='table';")
         tables = disk_cursor.fetchall()
         for table_name, create_table_sql in tables:
+            if "sqlite" in table_name:
+                continue
+
             # Create the table structure in the in-memory database
             mem_cursor.execute(create_table_sql)
 
             # Populate the table with data from the disk database
             disk_cursor.execute(f"SELECT * FROM {table_name}")
             rows = disk_cursor.fetchall()
             for row in rows:
```

### Comparing `kodexa-7.0.8621391210/kodexa/pipeline/pipeline.py` & `kodexa-7.0.8664569946/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/platform/client.py` & `kodexa-7.0.8664569946/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/platform/interaction.py` & `kodexa-7.0.8664569946/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/platform/kodexa.py` & `kodexa-7.0.8664569946/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/ast.py` & `kodexa-7.0.8664569946/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/core.py` & `kodexa-7.0.8664569946/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/lexrules.py` & `kodexa-7.0.8664569946/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/lextab.py` & `kodexa-7.0.8664569946/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/parserules.py` & `kodexa-7.0.8664569946/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/selectors/parsetab.py` & `kodexa-7.0.8664569946/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/spatial/azure_models.py` & `kodexa-7.0.8664569946/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/spatial/bbox_common.py` & `kodexa-7.0.8664569946/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/spatial/table_form_common.py` & `kodexa-7.0.8664569946/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/steps/common.py` & `kodexa-7.0.8664569946/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/testing/test_components.py` & `kodexa-7.0.8664569946/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/kodexa/testing/test_utils.py` & `kodexa-7.0.8664569946/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.8621391210/pyproject.toml` & `kodexa-7.0.8664569946/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.08621391210"
+version = "7.0.08664569946"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.8621391210/PKG-INFO` & `kodexa-7.0.8664569946/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.8621391210
+Version: 7.0.8664569946
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

