# Comparing `tmp/fixinventory-plugin-scarf-4.0.1.tar.gz` & `tmp/fixinventory-plugin-scarf-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-scarf-4.0.1.tar", last modified: Thu Mar 14 14:04:49 2024, max compression
+gzip compressed data, was "fixinventory-plugin-scarf-4.0.2.tar", last modified: Fri Apr 12 12:16:39 2024, max compression
```

## Comparing `fixinventory-plugin-scarf-4.0.1.tar` & `fixinventory-plugin-scarf-4.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:03.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 14:04:49.000000 fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:49.698184 fixinventory-plugin-scarf-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-14 14:01:51.000000 fixinventory-plugin-scarf-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:39.928294 fixinventory-plugin-scarf-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-12 12:16:39.928294 fixinventory-plugin-scarf-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:39.924294 fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:39.928294 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:14:54.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 12:16:39.000000 fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:16:39.928294 fixinventory-plugin-scarf-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:16:39.928294 fixinventory-plugin-scarf-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 12:13:48.000000 fixinventory-plugin-scarf-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-scarf-4.0.1/PKG-INFO` & `fixinventory-plugin-scarf-4.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-scarf
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Scarf Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/scarf
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
 Requires-Dist: requests
 
 # Fix 💜 Scarf
 Scarf Collector Plugin for Fix
 
 This collector plugin is used to collect data from Scarf. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `fixinventory-plugin-scarf-4.0.1/README.md` & `fixinventory-plugin-scarf-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/__init__.py` & `fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/resources.py` & `fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-scarf-4.0.1/fix_plugin_scarf/scarf.py` & `fixinventory-plugin-scarf-4.0.2/fix_plugin_scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/PKG-INFO` & `fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-scarf
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Scarf Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/scarf
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
 Requires-Dist: requests
 
 # Fix 💜 Scarf
 Scarf Collector Plugin for Fix
 
 This collector plugin is used to collect data from Scarf. It is used internally at Some Engineering to create metrics about image downloads.
```

### Comparing `fixinventory-plugin-scarf-4.0.1/fixinventory_plugin_scarf.egg-info/SOURCES.txt` & `fixinventory-plugin-scarf-4.0.2/fixinventory_plugin_scarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-scarf-4.0.1/pyproject.toml` & `fixinventory-plugin-scarf-4.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-scarf"
 description = "Fix Scarf Collector Plugin"
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
     "requests",
 ]
 
 [project.entry-points."fix.plugins"]
 scarf = "fix_plugin_scarf:ScarfCollectorPlugin"
 
 [project.urls]
```

