# Comparing `tmp/fixinventory-plugin-onelogin-4.0.1.tar.gz` & `tmp/fixinventory-plugin-onelogin-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-onelogin-4.0.1.tar", last modified: Thu Mar 14 14:04:58 2024, max compression
+gzip compressed data, was "fixinventory-plugin-onelogin-4.0.2.tar", last modified: Fri Apr 12 12:13:49 2024, max compression
```

## Comparing `fixinventory-plugin-onelogin-4.0.1.tar` & `fixinventory-plugin-onelogin-4.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:58.093339 fixinventory-plugin-onelogin-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-14 14:04:58.093339 fixinventory-plugin-onelogin-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:58.089339 fixinventory-plugin-onelogin-4.0.1/fix_plugin_onelogin/
--rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/fix_plugin_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/fix_plugin_onelogin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:58.093339 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:07.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-14 14:04:58.000000 fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:58.093339 fixinventory-plugin-onelogin-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:58.093339 fixinventory-plugin-onelogin-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-14 14:01:54.000000 fixinventory-plugin-onelogin-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6458 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:11:59.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 12:13:49.000000 fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:49.560401 fixinventory-plugin-onelogin-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:49.556401 fixinventory-plugin-onelogin-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-12 12:10:50.000000 fixinventory-plugin-onelogin-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-onelogin-4.0.1/PKG-INFO` & `fixinventory-plugin-onelogin-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
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
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory-plugin-onelogin-4.0.1/fix_plugin_onelogin/__init__.py` & `fixinventory-plugin-onelogin-4.0.2/fix_plugin_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-onelogin-4.0.1/fixinventory_plugin_onelogin.egg-info/PKG-INFO` & `fixinventory-plugin-onelogin-4.0.2/fixinventory_plugin_onelogin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-onelogin
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix OneLogin Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/onelogin
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
 Requires-Dist: onelogin==2.0.4
 
 # fix-plugin-onelogin
 OneLogin collector plugin for Fix
 
 This plugin collects OneLogin users as cloud resources and adds them to the Fix graph for use by other plugins.
```

### Comparing `fixinventory-plugin-onelogin-4.0.1/pyproject.toml` & `fixinventory-plugin-onelogin-4.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-onelogin"
 description = "Fix OneLogin Plugin"
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
     "onelogin==2.0.4",
 ]
 
 [project.entry-points."fix.plugins"]
 onelogin = "fix_plugin_onelogin:OneLoginPlugin"
 
 [project.urls]
```

