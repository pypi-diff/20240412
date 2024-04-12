# Comparing `tmp/fixinventory-plugin-github-4.0.1.tar.gz` & `tmp/fixinventory-plugin-github-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-github-4.0.1.tar", last modified: Thu Mar 14 14:04:48 2024, max compression
+gzip compressed data, was "fixinventory-plugin-github-4.0.2.tar", last modified: Fri Apr 12 12:14:44 2024, max compression
```

## Comparing `fixinventory-plugin-github-4.0.1.tar` & `fixinventory-plugin-github-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:48.961336 fixinventory-plugin-github-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-14 14:04:48.961336 fixinventory-plugin-github-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:48.961336 fixinventory-plugin-github-4.0.1/fix_plugin_github/
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/fix_plugin_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/fix_plugin_github/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/fix_plugin_github/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:48.961336 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:02.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:04:48.000000 fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:48.965336 fixinventory-plugin-github-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:48.961336 fixinventory-plugin-github-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-14 14:01:54.000000 fixinventory-plugin-github-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/fix_plugin_github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/fix_plugin_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/fix_plugin_github/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24265 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/fix_plugin_github/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:58.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:44.000000 fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:44.174199 fixinventory-plugin-github-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-12 12:11:52.000000 fixinventory-plugin-github-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-github-4.0.1/PKG-INFO` & `fixinventory-plugin-github-4.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-github
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Github Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/github
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
 Requires-Dist: PyGithub
 
 # fix-plugin-github (WIP)
 GitHub Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-github-4.0.1/fix_plugin_github/__init__.py` & `fixinventory-plugin-github-4.0.2/fix_plugin_github/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-github-4.0.1/fix_plugin_github/config.py` & `fixinventory-plugin-github-4.0.2/fix_plugin_github/config.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-github-4.0.1/fix_plugin_github/resources.py` & `fixinventory-plugin-github-4.0.2/fix_plugin_github/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-github-4.0.1/fixinventory_plugin_github.egg-info/PKG-INFO` & `fixinventory-plugin-github-4.0.2/fixinventory_plugin_github.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-github
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Github Collector Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/github
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
 Requires-Dist: PyGithub
 
 # fix-plugin-github (WIP)
 GitHub Collector Plugin for Fix
 
 ## License
 See [LICENSE](../../LICENSE) for details.
```

### Comparing `fixinventory-plugin-github-4.0.1/pyproject.toml` & `fixinventory-plugin-github-4.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-github"
 description = "Fix Github Collector Plugin"
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
     "PyGithub",
 ]
 
 [project.entry-points."fix.plugins"]
 github = "fix_plugin_github:GithubCollectorPlugin"
 
 [project.urls]
```

