# Comparing `tmp/readwrite-0.6.0.tar.gz` & `tmp/readwrite-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readwrite-0.6.0.tar", last modified: Sun Mar 17 16:34:04 2024, max compression
+gzip compressed data, was "readwrite-0.7.0.tar", last modified: Fri Apr 12 12:46:17 2024, max compression
```

## Comparing `readwrite-0.6.0.tar` & `readwrite-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.465014 readwrite-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-17 16:34:04.465014 readwrite-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-03-17 16:34:00.000000 readwrite-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.457014 readwrite-0.6.0/readwrite/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.461014 readwrite-0.6.0/readwrite/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/cli/fast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/cli/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.461014 readwrite-0.6.0/readwrite/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/text.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/toml.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/handlers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-17 16:34:00.000000 readwrite-0.6.0/readwrite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.465014 readwrite-0.6.0/readwrite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-17 16:34:04.000000 readwrite-0.6.0/readwrite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 16:34:04.465014 readwrite-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-17 16:34:00.000000 readwrite-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:04.465014 readwrite-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/test_interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-17 16:34:00.000000 readwrite-0.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.479549 readwrite-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 12:46:17.479549 readwrite-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-12 12:46:13.000000 readwrite-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.475549 readwrite-0.7.0/readwrite/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.475549 readwrite-0.7.0/readwrite/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/cli/fast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/cli/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.479549 readwrite-0.7.0/readwrite/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/toml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/handlers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-12 12:46:13.000000 readwrite-0.7.0/readwrite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.479549 readwrite-0.7.0/readwrite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 12:46:17.000000 readwrite-0.7.0/readwrite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:46:17.479549 readwrite-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-12 12:46:13.000000 readwrite-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:17.479549 readwrite-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/test_interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-12 12:46:13.000000 readwrite-0.7.0/tests/test_utils.py
```

### Comparing `readwrite-0.6.0/PKG-INFO` & `readwrite-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readwrite
-Version: 0.6.0
+Version: 0.7.0
 Summary: readwrite - Quickly read/write file in common formats
 Home-page: https://github.com/crunchdao/readwrite
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `readwrite-0.6.0/README.md` & `readwrite-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/__init__.py` & `readwrite-0.7.0/readwrite/__init__.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/cli/fast.py` & `readwrite-0.7.0/readwrite/cli/fast.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/cli/manual.py` & `readwrite-0.7.0/readwrite/cli/manual.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/handlers/base.py` & `readwrite-0.7.0/readwrite/handlers/base.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/handlers/csv.py` & `readwrite-0.7.0/readwrite/handlers/excel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-from .base import Handler, Param
+from .base import Handler
 
 
-class CsvHandler(Handler):
+class ExcelHandler(Handler):
 
     def __init__(self):
         super().__init__(
-            "csv",
-            ["csv"]
+            "excel",
+            ["xlsx"]
         )
 
     def read(self, path: str, **kwargs):
         import pandas
 
-        return pandas.read_csv(path, **kwargs)
+        return pandas.read_excel(path, **kwargs)
 
     def read_params(self):
         return {
-            "index_col": Param(
-                int,
-                help="Column to use as row label, denoted by column index.",
-            )
+            "sheet_name": str,
+            "engine": str,
         }
 
     def write(self, x, path, **kwargs):
         import pandas
 
         if not isinstance(x, pandas.DataFrame):
             raise ValueError("value must be a dataframe")
 
-        x.to_csv(path, **kwargs)
+        x.to_excel(path, **kwargs)
 
     def write_params(self):
         return {
-            "index": Param(
-                bool,
-                help="Write row names (index)."
-            ),
+            "index": bool,
+            "sheet_name": str,
         }
```

### Comparing `readwrite-0.6.0/readwrite/handlers/parquet.py` & `readwrite-0.7.0/readwrite/handlers/parquet.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/handlers/pickle.py` & `readwrite-0.7.0/readwrite/handlers/pickle.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/interactive.py` & `readwrite-0.7.0/readwrite/interactive.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/registry.py` & `readwrite-0.7.0/readwrite/registry.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite/utils.py` & `readwrite-0.7.0/readwrite/utils.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/readwrite.egg-info/PKG-INFO` & `readwrite-0.7.0/readwrite.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readwrite
-Version: 0.6.0
+Version: 0.7.0
 Summary: readwrite - Quickly read/write file in common formats
 Home-page: https://github.com/crunchdao/readwrite
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `readwrite-0.6.0/readwrite.egg-info/SOURCES.txt` & `readwrite-0.7.0/readwrite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/setup.py` & `readwrite-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/tests/test_handlers.py` & `readwrite-0.7.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/tests/test_interactive.py` & `readwrite-0.7.0/tests/test_interactive.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/tests/test_module.py` & `readwrite-0.7.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/tests/test_registry.py` & `readwrite-0.7.0/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `readwrite-0.6.0/tests/test_utils.py` & `readwrite-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

