# Comparing `tmp/hatch_compile_yaml-4.0.0.tar.gz` & `tmp/hatch_compile_yaml-5.0.0.tar.gz`

## Comparing `hatch_compile_yaml-4.0.0.tar` & `hatch_compile_yaml-5.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/convert.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/README.rst
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-4.0.0/hatch_compile_yaml/convert.py` & `hatch_compile_yaml-5.0.0/hatch_compile_yaml/convert.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,26 +41,22 @@
 def resolve_file_format(extension: str) -> FileFormat:
     if extension in EXTENSION_TO_FORMAT:
         return EXTENSION_TO_FORMAT[extension]
     else:
         raise ValueError(f"Unsupported file extension: {extension}")
 
 
-def convert_data_file(source_path: Path, target_format: str = "msgpack", remove_source_files: bool = True):
-    target_format = FileFormat[target_format.upper()]
-    source_format = resolve_file_format(source_path.suffix)
-
-    load_func, _ = FORMAT_FUNCTIONS[source_format]
-    _, save_func = FORMAT_FUNCTIONS[target_format]
+def convert_data_file(source_path: Path, target_path: Path, target_format: FileFormat, remove_source_files: bool = True):
+    # Retrieve the appropriate load and save functions
+    load_func, save_func = FORMAT_FUNCTIONS[target_format]
 
     # Load the source data
     with source_path.open("rb") as f:
         data = load_func(f)
 
     # Convert and save the data to the target format
-    target_path = source_path.with_suffix(f".{target_format.value}")
     with target_path.open("wb") as f:
         save_func(data, f)
 
     # Optionally remove the source file
     if remove_source_files:
         source_path.unlink()
```

### Comparing `hatch_compile_yaml-4.0.0/.gitignore` & `hatch_compile_yaml-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-4.0.0/README.rst` & `hatch_compile_yaml-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-4.0.0/pyproject.toml` & `hatch_compile_yaml-5.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-4.0.0/PKG-INFO` & `hatch_compile_yaml-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 4.0.0
+Version: 5.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

