# Comparing `tmp/hatch_compile_yaml-2.0.1.tar.gz` & `tmp/hatch_compile_yaml-4.0.0.tar.gz`

## Comparing `hatch_compile_yaml-2.0.1.tar` & `hatch_compile_yaml-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/hatch_compile_yaml/convert.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/README.rst
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-2.0.1/hatch_compile_yaml/convert.py` & `hatch_compile_yaml-4.0.0/hatch_compile_yaml/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         raise ValueError(f"Unsupported file extension: {extension}")
 
 
 def convert_data_file(source_path: Path, target_format: str = "msgpack", remove_source_files: bool = True):
     target_format = FileFormat[target_format.upper()]
     source_format = resolve_file_format(source_path.suffix)
 
-    load_func, save_func = FORMAT_FUNCTIONS[source_format]
+    load_func, _ = FORMAT_FUNCTIONS[source_format]
+    _, save_func = FORMAT_FUNCTIONS[target_format]
 
     # Load the source data
     with source_path.open("rb") as f:
         data = load_func(f)
 
     # Convert and save the data to the target format
     target_path = source_path.with_suffix(f".{target_format.value}")
```

### Comparing `hatch_compile_yaml-2.0.1/hatch_compile_yaml/plugin.py` & `hatch_compile_yaml-4.0.0/hatch_compile_yaml/plugin.py`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-2.0.1/.gitignore` & `hatch_compile_yaml-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-2.0.1/README.rst` & `hatch_compile_yaml-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-2.0.1/pyproject.toml` & `hatch_compile_yaml-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-2.0.1/PKG-INFO` & `hatch_compile_yaml-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 2.0.1
+Version: 4.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

