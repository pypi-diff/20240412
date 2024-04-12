# Comparing `tmp/fixinventoryshell-4.0.1.tar.gz` & `tmp/fixinventoryshell-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventoryshell-4.0.1.tar", last modified: Thu Mar 14 14:05:46 2024, max compression
+gzip compressed data, was "fixinventoryshell-4.0.2.tar", last modified: Fri Apr 12 12:14:48 2024, max compression
```

## Comparing `fixinventoryshell-4.0.1.tar` & `fixinventoryshell-4.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:03:02.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-14 14:05:46.000000 fixinventoryshell-4.0.1/fixinventoryshell.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/fixshell/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/authorized_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38726 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/promptsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/protected_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/fixshell/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:05:46.113203 fixinventoryshell-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/test/test_promptsession.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-14 14:01:55.000000 fixinventoryshell-4.0.1/test/test_protected_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:12:00.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 12:14:48.000000 fixinventoryshell-4.0.2/fixinventoryshell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/fixshell/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/authorized_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38726 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/protected_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/fixshell/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:14:48.809072 fixinventoryshell-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14172 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/test/test_promptsession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-12 12:10:51.000000 fixinventoryshell-4.0.2/test/test_protected_files.py
```

### Comparing `fixinventoryshell-4.0.1/PKG-INFO` & `fixinventoryshell-4.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: fixinventoryshell
-Version: 4.0.1
+Version: 4.0.2
 Summary: Commandline interpreter to interact with Fix Inventory.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixshell
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
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
 Requires-Dist: prompt-toolkit
 Requires-Dist: rich
 Requires-Dist: fixinventoryclient
 Requires-Dist: aiohttp[speedups]
 
 # `resh`
 Fix Shell
```

### Comparing `fixinventoryshell-4.0.1/README.md` & `fixinventoryshell-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixinventoryshell.egg-info/PKG-INFO` & `fixinventoryshell-4.0.2/fixinventoryshell.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: fixinventoryshell
-Version: 4.0.1
+Version: 4.0.2
 Summary: Commandline interpreter to interact with Fix Inventory.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixshell
 Keywords: cloud security
 Classifier: Development Status :: 5 - Production/Stable
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
 Requires-Dist: prompt-toolkit
 Requires-Dist: rich
 Requires-Dist: fixinventoryclient
 Requires-Dist: aiohttp[speedups]
 
 # `resh`
 Fix Shell
```

### Comparing `fixinventoryshell-4.0.1/fixinventoryshell.egg-info/SOURCES.txt` & `fixinventoryshell-4.0.2/fixinventoryshell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixshell/__main__.py` & `fixinventoryshell-4.0.2/fixshell/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixshell/authorized_client.py` & `fixinventoryshell-4.0.2/fixshell/authorized_client.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixshell/promptsession.py` & `fixinventoryshell-4.0.2/fixshell/promptsession.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixshell/protected_files.py` & `fixinventoryshell-4.0.2/fixshell/protected_files.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/fixshell/shell.py` & `fixinventoryshell-4.0.2/fixshell/shell.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/pyproject.toml` & `fixinventoryshell-4.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [project]
 name = "fixinventoryshell"
-version = "4.0.1"
+version = "4.0.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Commandline interpreter to interact with Fix Inventory."
 license = { text="AGPLv3" }
-requires-python = ">=3.9"
+requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 5 - Production/Stable",
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
 keywords = ["cloud security"]
 
 dependencies = [
-    "fixinventorylib==4.0.1",
+    "fixinventorylib==4.0.2",
     "prompt-toolkit",
     "rich",
     "fixinventoryclient",
     "aiohttp[speedups]",
 ]
 
 [project.scripts]
```

### Comparing `fixinventoryshell-4.0.1/test/test_promptsession.py` & `fixinventoryshell-4.0.2/test/test_promptsession.py`

 * *Files identical despite different names*

### Comparing `fixinventoryshell-4.0.1/test/test_protected_files.py` & `fixinventoryshell-4.0.2/test/test_protected_files.py`

 * *Files identical despite different names*

