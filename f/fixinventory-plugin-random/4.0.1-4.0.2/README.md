# Comparing `tmp/fixinventory-plugin-random-4.0.1.tar.gz` & `tmp/fixinventory-plugin-random-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-random-4.0.1.tar", last modified: Thu Mar 14 14:08:09 2024, max compression
+gzip compressed data, was "fixinventory-plugin-random-4.0.2.tar", last modified: Fri Apr 12 12:13:48 2024, max compression
```

## Comparing `fixinventory-plugin-random-4.0.1.tar` & `fixinventory-plugin-random-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/fix_plugin_random/
--rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/fix_plugin_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/fix_plugin_random/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/fix_plugin_random/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:06:23.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:08:09.000000 fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:08:09.108714 fixinventory-plugin-random-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-14 14:05:17.000000 fixinventory-plugin-random-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/fix_plugin_random/
+-rw-r--r--   0 runner    (1001) docker     (127)    11001 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/fix_plugin_random/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:03.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:13:47.000000 fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:48.001354 fixinventory-plugin-random-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-12 12:10:58.000000 fixinventory-plugin-random-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-random-4.0.1/PKG-INFO` & `fixinventory-plugin-random-4.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory-plugin-random-4.0.1/README.md` & `fixinventory-plugin-random-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.1/fix_plugin_random/__init__.py` & `fixinventory-plugin-random-4.0.2/fix_plugin_random/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.1/fix_plugin_random/resources.py` & `fixinventory-plugin-random-4.0.2/fix_plugin_random/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-random-4.0.1/fixinventory_plugin_random.egg-info/PKG-INFO` & `fixinventory-plugin-random-4.0.2/fixinventory_plugin_random.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-random
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Random Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/random
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.1
+Requires-Dist: fixinventorylib==4.0.2
 
 # fix-plugin-random
 Random Cloud Collector for Fix
 
 Creates a plausible pseudo-random cloud based on a configurable seed.
 
 The base infrastructure stays the same, but the number of instances vary slightly from run to run so that metrics show some more interesting up/down lines.
```

### Comparing `fixinventory-plugin-random-4.0.1/pyproject.toml` & `fixinventory-plugin-random-4.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-random"
 description = "Fix Random Collector Plugin"
-version = "4.0.1"
+version = "4.0.2"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
     "Intended Audience :: System Administrators",
     "Intended Audience :: Information Technology",
     # License information
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     # Supported python versions
-    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.11",
     # Supported OS's
     "Operating System :: POSIX :: Linux",
     "Operating System :: Unix",
     # Extra metadata
     "Environment :: Console",
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.1",
+    "fixinventorylib==4.0.2",
 ]
 
 [project.entry-points."fix.plugins"]
 random = "fix_plugin_random:RandomCollectorPlugin"
 
 [project.urls]
 Documentation = "https://inventory.fix.security"
```

