# Comparing `tmp/fixinventory-plugin-slack-4.0.1.tar.gz` & `tmp/fixinventory-plugin-slack-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-slack-4.0.1.tar", last modified: Thu Mar 14 14:04:52 2024, max compression
+gzip compressed data, was "fixinventory-plugin-slack-4.0.2.tar", last modified: Fri Apr 12 12:17:55 2024, max compression
```

## Comparing `fixinventory-plugin-slack-4.0.1.tar` & `fixinventory-plugin-slack-4.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/fix_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/fix_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/fix_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/fix_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:02.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-14 14:04:52.000000 fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:52.594977 fixinventory-plugin-slack-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-14 14:01:53.000000 fixinventory-plugin-slack-4.0.1/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.833978 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:06.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/test/test_config.py
```

### Comparing `fixinventory-plugin-slack-4.0.1/PKG-INFO` & `fixinventory-plugin-slack-4.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
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
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory-plugin-slack-4.0.1/fix_plugin_slack/__init__.py` & `fixinventory-plugin-slack-4.0.2/fix_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-slack-4.0.1/fix_plugin_slack/resources.py` & `fixinventory-plugin-slack-4.0.2/fix_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-slack-4.0.1/fixinventory_plugin_slack.egg-info/PKG-INFO` & `fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.1
+Version: 4.0.2
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
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
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory-plugin-slack-4.0.1/pyproject.toml` & `fixinventory-plugin-slack-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventory-plugin-slack"
 description = "Fix Slack Plugin"
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
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."fix.plugins"]
 slack_bot = "fix_plugin_slack:SlackBotPlugin"
 slack_collector = "fix_plugin_slack:SlackCollectorPlugin"
```

