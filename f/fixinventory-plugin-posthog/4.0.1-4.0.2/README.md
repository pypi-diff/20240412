# Comparing `tmp/fixinventory-plugin-posthog-4.0.1.tar.gz` & `tmp/fixinventory-plugin-posthog-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-posthog-4.0.1.tar", last modified: Thu Mar 14 14:04:50 2024, max compression
+gzip compressed data, was "fixinventory-plugin-posthog-4.0.2.tar", last modified: Fri Apr 12 12:15:48 2024, max compression
```

## Comparing `fixinventory-plugin-posthog-4.0.1.tar` & `fixinventory-plugin-posthog-4.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/posthog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:02.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 14:04:50.000000 fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:50.061968 fixinventory-plugin-posthog-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-14 14:01:53.000000 fixinventory-plugin-posthog-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:58.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 12:15:48.000000 fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:15:48.705687 fixinventory-plugin-posthog-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 12:12:46.000000 fixinventory-plugin-posthog-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-posthog-4.0.1/PKG-INFO` & `fixinventory-plugin-posthog-4.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-posthog
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Posthog Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/posthog
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
 
 # fix-plugin-posthog
 Posthog Collector Plugin for Fix
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about fix installations and usage.
```

### Comparing `fixinventory-plugin-posthog-4.0.1/README.md` & `fixinventory-plugin-posthog-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/__init__.py` & `fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/posthog.py` & `fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/posthog.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-posthog-4.0.1/fix_plugin_posthog/resources.py` & `fixinventory-plugin-posthog-4.0.2/fix_plugin_posthog/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/PKG-INFO` & `fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-posthog
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Posthog Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/posthog
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
 
 # fix-plugin-posthog
 Posthog Collector Plugin for Fix
 
 This collector plugin is used to collect data from Posthog. It is used internally at Some Engineering to create metrics about fix installations and usage.
```

### Comparing `fixinventory-plugin-posthog-4.0.1/fixinventory_plugin_posthog.egg-info/SOURCES.txt` & `fixinventory-plugin-posthog-4.0.2/fixinventory_plugin_posthog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-posthog-4.0.1/pyproject.toml` & `fixinventory-plugin-posthog-4.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-posthog"
 description = "Fix Posthog Collector Plugin"
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
 posthog = "fix_plugin_posthog:PosthogCollectorPlugin"
 
 [project.urls]
```

