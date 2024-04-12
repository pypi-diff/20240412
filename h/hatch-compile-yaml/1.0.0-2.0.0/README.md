# Comparing `tmp/hatch_compile_yaml-1.0.0.tar.gz` & `tmp/hatch_compile_yaml-2.0.0.tar.gz`

## Comparing `hatch_compile_yaml-1.0.0.tar` & `hatch_compile_yaml-2.0.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/hatch_compile_yaml/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/hatch_compile_yaml/hooks.py
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/hatch_compile_yaml/plugin.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/.gitignore
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/README.rst
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 hatch_compile_yaml-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/hatch_compile_yaml/__init__.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/hatch_compile_yaml/convert.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/hatch_compile_yaml/hooks.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/hatch_compile_yaml/plugin.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/README.rst
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hatch_compile_yaml-2.0.0/PKG-INFO
```

### Comparing `hatch_compile_yaml-1.0.0/.gitignore` & `hatch_compile_yaml-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hatch_compile_yaml-1.0.0/README.rst` & `hatch_compile_yaml-2.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 
 Now you'll need to configure the build scripts you want to run.
 This is done by adding an array of scripts to the tool.hatch.build.hooks.build-scripts.scripts
 key in your pyproject.toml file. In practice this looks like:
 
 .. code-block:: toml
 
-   [tool.hatch.build.hooks.yaml-compile.options]
+   [tool.hatch.build.hooks.convert-data-file.options]
    pattern = "*.yaml"
-   remove_source_files = True
+   target_format = "msgpack"
+   remove_source_files = true
+
 
 Roadmap
 =======
 
 Reference the `open issues <https://gitlab.com/Akm0d/salt-agi/issues>`__ for a list of
 proposed features (and known issues).
```

### Comparing `hatch_compile_yaml-1.0.0/pyproject.toml` & `hatch_compile_yaml-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -95,14 +95,30 @@
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
 
+
+ignore = [
+  # Allow non-abstract empty methods in abstract base classes
+  "B027",
+  # Allow boolean positional values in function calls, like `dict.get(... True)`
+  "FBT003",
+  # Ignore checks for possible passwords
+  "S105", "S106", "S107",
+  # Ignore complexity
+  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  "ISC001",
+  "EM102",
+  "FBT001",
+  "FBT002",
+]
+
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["hatch_compile_yaml"]
```

### Comparing `hatch_compile_yaml-1.0.0/PKG-INFO` & `hatch_compile_yaml-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hatch-compile-yaml
-Version: 1.0.0
+Version: 2.0.0
 Summary: Compile yaml files to msgpack
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Hatch
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
@@ -69,17 +69,19 @@
 
 Now you'll need to configure the build scripts you want to run.
 This is done by adding an array of scripts to the tool.hatch.build.hooks.build-scripts.scripts
 key in your pyproject.toml file. In practice this looks like:
 
 .. code-block:: toml
 
-   [tool.hatch.build.hooks.yaml-compile.options]
+   [tool.hatch.build.hooks.convert-data-file.options]
    pattern = "*.yaml"
-   remove_source_files = True
+   target_format = "msgpack"
+   remove_source_files = true
+
 
 Roadmap
 =======
 
 Reference the `open issues <https://gitlab.com/Akm0d/salt-agi/issues>`__ for a list of
 proposed features (and known issues).
```

