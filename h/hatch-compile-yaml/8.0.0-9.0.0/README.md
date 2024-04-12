# Comparing `tmp/hatch_compile_yaml-8.0.0.tar.gz` & `tmp/hatch_compile_yaml-9.0.0.tar.gz`

## Comparing `hatch_compile_yaml-8.0.0.tar` & `hatch_compile_yaml-9.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/convert.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/README.rst
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-9.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-8.0.0/hatch_compile_yaml/convert.py` & `hatch_compile_yaml-9.0.0/hatch_compile_yaml/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 def resolve_file_format(extension: str) -> FileFormat:
     if extension in EXTENSION_TO_FORMAT:
         return EXTENSION_TO_FORMAT[extension]
     else:
         raise ValueError(f"Unsupported file extension: {extension}")
 
 
-def convert_data_file(source_path: Path, target_path: Path, target_format: FileFormat, remove_source_files: bool = True):
+def convert_data_file(source_path: Path, target_path: Path, target_format: str, remove_source_files: bool = True):
     # Resolve format and get corresponding load and save functions
-    load_func, save_func = FORMAT_FUNCTIONS[FileFormat[target_format]]
+    load_func, save_func = FORMAT_FUNCTIONS[FileFormat[target_format.upper()]]
 
     # Load the source data
     with source_path.open("rb") as f:
         data = load_func(f)
 
     # Convert and save the data to the target format
     with target_path.open("wb") as f:
```

### Comparing `hatch_compile_yaml-8.0.0/hatch_compile_yaml/plugin.py` & `hatch_compile_yaml-9.0.0/hatch_compile_yaml/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 class DataFileConverter(BuildHookInterface):
     PLUGIN_NAME = "convert-data-file"
 
     def initialize(self, version, build_data):
         options = build_data.get("options", {})
         pattern = options.get("pattern", DEFAULT_PATTERN)
-        target_format = options.get("target_format", "MSGPACK")  # Default to msgpack
+        target_format = options.get("target_format", "msgpack")  # Default to msgpack
         pattern_regex = re.compile(pattern)
 
         # Determine the output directory from build_data or use 'dist' as default
         output_dir = Path(build_data.get("output_directory", "dist"))
 
         for root, _, files in os.walk(self.root):
             for file in files:
                 file_path = Path(root) / file
                 if pattern_regex.match(file):
                     # Define the target path in the specified build output directory
-                    target_path = output_dir / file_path.with_suffix(f".{target_format}").name
-                    convert_data_file(file_path, target_path, FileFormat[target_format.upper()], options.get("remove_source_files", True))
+                    target_path = output_dir / file_path.with_suffix(f".{target_format.lower()}").name
+                    convert_data_file(file_path, target_path, **options)
```

### Comparing `hatch_compile_yaml-8.0.0/.gitignore` & `hatch_compile_yaml-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-8.0.0/README.rst` & `hatch_compile_yaml-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-8.0.0/pyproject.toml` & `hatch_compile_yaml-9.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-8.0.0/PKG-INFO` & `hatch_compile_yaml-9.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 8.0.0
+Version: 9.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

