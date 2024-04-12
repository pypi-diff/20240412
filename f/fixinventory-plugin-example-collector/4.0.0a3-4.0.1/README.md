# Comparing `tmp/fixinventory-plugin-example-collector-4.0.0a3.tar.gz` & `tmp/fixinventory-plugin-example-collector-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-example-collector-4.0.0a3.tar", last modified: Wed Feb 28 15:44:00 2024, max compression
+gzip compressed data, was "fixinventory-plugin-example-collector-4.0.1.tar", last modified: Thu Mar 14 14:05:03 2024, max compression
```

## Comparing `fixinventory-plugin-example-collector-4.0.0a3.tar` & `fixinventory-plugin-example-collector-4.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:44:00.805566 fixinventory-plugin-example-collector-4.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-28 15:44:00.805566 fixinventory-plugin-example-collector-4.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:44:00.801566 fixinventory-plugin-example-collector-4.0.0a3/fix_plugin_example_collector/
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/fix_plugin_example_collector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:44:00.805566 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:42:18.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-28 15:44:00.000000 fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-28 15:44:00.805566 fixinventory-plugin-example-collector-4.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:44:00.805566 fixinventory-plugin-example-collector-4.0.0a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-28 15:41:12.000000 fixinventory-plugin-example-collector-4.0.0a3/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/fix_plugin_example_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/fix_plugin_example_collector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:12.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-14 14:05:03.000000 fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:03.990848 fixinventory-plugin-example-collector-4.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-14 14:01:55.000000 fixinventory-plugin-example-collector-4.0.1/test/test_config.py
```

### Comparing `fixinventory-plugin-example-collector-4.0.0a3/PKG-INFO` & `fixinventory-plugin-example-collector-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-example-collector
-Version: 4.0.0a3
+Version: 4.0.1
 Summary: Fix Example Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,14 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.0a3
+Requires-Dist: fixinventorylib==4.0.1
 
 # fix-plugin-example-collector
 Example Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-example-collector-4.0.0a3/fix_plugin_example_collector/__init__.py` & `fixinventory-plugin-example-collector-4.0.1/fix_plugin_example_collector/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/PKG-INFO` & `fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-example-collector
-Version: 4.0.0a3
+Version: 4.0.1
 Summary: Fix Example Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/example_collector
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,14 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.0a3
+Requires-Dist: fixinventorylib==4.0.1
 
 # fix-plugin-example-collector
 Example Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-example-collector-4.0.0a3/fixinventory_plugin_example_collector.egg-info/SOURCES.txt` & `fixinventory-plugin-example-collector-4.0.1/fixinventory_plugin_example_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-example-collector-4.0.0a3/pyproject.toml` & `fixinventory-plugin-example-collector-4.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-example-collector"
 description = "Fix Example Collector Plugin"
-version = "4.0.0a3"
+version = "4.0.1"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.0a3",
+    "fixinventorylib==4.0.1",
 ]
 
 [project.entry-points."fix.plugins"]
 example_collector = "fix_plugin_example_collector:ExampleCollectorPlugin"
 
 [project.urls]
 Documentation = "https://inventory.fix.security"
```

