# Comparing `tmp/hatch_compile_yaml-5.0.0.tar.gz` & `tmp/hatch_compile_yaml-6.0.0.tar.gz`

## Comparing `hatch_compile_yaml-5.0.0.tar` & `hatch_compile_yaml-6.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/convert.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/README.rst
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-6.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-5.0.0/hatch_compile_yaml/convert.py` & `hatch_compile_yaml-6.0.0/hatch_compile_yaml/convert.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,40 +18,33 @@
     ".yml": FileFormat.YAML,
     ".json": FileFormat.JSON,
     ".msgpack": FileFormat.MSGPACK,
 }
 
 
 # Define a dictionary that maps file formats to their respective load and save functions
-FORMAT_FUNCTIONS: dict[FileFormat, tuple[Callable, Callable]] = {
-    FileFormat.YAML: (
-        lambda f: yaml.safe_load(f.read().decode("utf-8")),
-        lambda data, f: f.write(yaml.safe_dump(data).encode("utf-8")),
-    ),
-    FileFormat.JSON: (
-        lambda f: json.loads(f.read().decode("utf-8")),
-        lambda data, f: f.write(json.dumps(data, indent=4).encode("utf-8")),
-    ),
-    FileFormat.MSGPACK: (
-        lambda f: msgpack.unpack(f, raw=False),
-        lambda data, f: msgpack.pack(data, f, use_bin_type=True),
-    ),
+
+FORMAT_FUNCTIONS = {
+    FileFormat.YAML: (lambda f: yaml.safe_load(f), lambda data, f: yaml.dump(data, f)),
+    FileFormat.JSON: (lambda f: json.load(f), lambda data, f: json.dump(data, f, indent=4)),
+    FileFormat.MSGPACK: (lambda f: msgpack.unpack(f, raw=False), lambda data, f: msgpack.pack(data, f))
 }
 
 
+
 def resolve_file_format(extension: str) -> FileFormat:
     if extension in EXTENSION_TO_FORMAT:
         return EXTENSION_TO_FORMAT[extension]
     else:
         raise ValueError(f"Unsupported file extension: {extension}")
 
 
-def convert_data_file(source_path: Path, target_path: Path, target_format: FileFormat, remove_source_files: bool = True):
-    # Retrieve the appropriate load and save functions
-    load_func, save_func = FORMAT_FUNCTIONS[target_format]
+def convert_data_file(source_path: Path, target_path: Path, target_format: str, remove_source_files: bool = True):
+    # Resolve format and get corresponding load and save functions
+    load_func, save_func = FORMAT_FUNCTIONS[FileFormat[target_format.upper()]]
 
     # Load the source data
     with source_path.open("rb") as f:
         data = load_func(f)
 
     # Convert and save the data to the target format
     with target_path.open("wb") as f:
```

### Comparing `hatch_compile_yaml-5.0.0/hatch_compile_yaml/plugin.py` & `hatch_compile_yaml-6.0.0/hatch_compile_yaml/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import re
 from pathlib import Path
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 
-from hatch_compile_yaml.convert import convert_data_file
-from hatch_compile_yaml.convert import FileFormat
+from hatch_compile_yaml.convert import FileFormat, convert_data_file
 
 DEFAULT_PATTERN = r".*\.(yaml|yml)$"
 
 class DataFileConverter(BuildHookInterface):
     PLUGIN_NAME = "convert-data-file"
 
     def initialize(self, version, build_data):
@@ -23,8 +22,8 @@
 
         for root, _, files in os.walk(self.root):
             for file in files:
                 file_path = Path(root) / file
                 if pattern_regex.match(file):
                     # Define the target path in the specified build output directory
                     target_path = output_dir / file_path.with_suffix(f".{target_format}").name
-                    convert_data_file(file_path, target_path, FileFormat[target_format.upper()], options.get("remove_source_files", True))
+                    convert_data_file(file_path, target_path, FileFormat[target_format.upper()], options.get("remove_source_files", True))
```

### Comparing `hatch_compile_yaml-5.0.0/.gitignore` & `hatch_compile_yaml-6.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-5.0.0/README.rst` & `hatch_compile_yaml-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-5.0.0/pyproject.toml` & `hatch_compile_yaml-6.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-5.0.0/PKG-INFO` & `hatch_compile_yaml-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 5.0.0
+Version: 6.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

