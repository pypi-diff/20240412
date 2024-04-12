# Comparing `tmp/hatch_compile_yaml-7.0.0.tar.gz` & `tmp/hatch_compile_yaml-8.0.0.tar.gz`

## Comparing `hatch_compile_yaml-7.0.0.tar` & `hatch_compile_yaml-8.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/hatch_compile_yaml/convert.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/README.rst
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-8.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-7.0.0/hatch_compile_yaml/convert.py` & `hatch_compile_yaml-8.0.0/hatch_compile_yaml/convert.py`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-7.0.0/hatch_compile_yaml/plugin.py` & `hatch_compile_yaml-8.0.0/hatch_compile_yaml/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class DataFileConverter(BuildHookInterface):
     PLUGIN_NAME = "convert-data-file"
 
     def initialize(self, version, build_data):
         options = build_data.get("options", {})
         pattern = options.get("pattern", DEFAULT_PATTERN)
-        target_format = options.get("target_format", "msgpack")  # Default to msgpack
+        target_format = options.get("target_format", "MSGPACK")  # Default to msgpack
         pattern_regex = re.compile(pattern)
 
         # Determine the output directory from build_data or use 'dist' as default
         output_dir = Path(build_data.get("output_directory", "dist"))
 
         for root, _, files in os.walk(self.root):
             for file in files:
```

### Comparing `hatch_compile_yaml-7.0.0/.gitignore` & `hatch_compile_yaml-8.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-7.0.0/README.rst` & `hatch_compile_yaml-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-7.0.0/pyproject.toml` & `hatch_compile_yaml-8.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-7.0.0/PKG-INFO` & `hatch_compile_yaml-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 7.0.0
+Version: 8.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
```

