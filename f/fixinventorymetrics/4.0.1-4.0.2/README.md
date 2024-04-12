# Comparing `tmp/fixinventorymetrics-4.0.1.tar.gz` & `tmp/fixinventorymetrics-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorymetrics-4.0.1.tar", last modified: Thu Mar 14 14:04:43 2024, max compression
+gzip compressed data, was "fixinventorymetrics-4.0.2.tar", last modified: Fri Apr 12 12:13:45 2024, max compression
```

## Comparing `fixinventorymetrics-4.0.1.tar` & `fixinventorymetrics-4.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:43.860572 fixinventorymetrics-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-03-14 14:04:43.860572 fixinventorymetrics-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:43.860572 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 14:02:59.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-14 14:04:43.000000 fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:43.856572 fixinventorymetrics-4.0.1/fixmetrics/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/default_metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/fixmetrics/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-14 14:04:43.860572 fixinventorymetrics-4.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 14:04:43.860572 fixinventorymetrics-4.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-14 14:01:53.000000 fixinventorymetrics-4.0.1/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:11:58.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 12:13:45.000000 fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/fixmetrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7679 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/default_metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/fixmetrics/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:45.240135 fixinventorymetrics-4.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 12:10:51.000000 fixinventorymetrics-4.0.2/test/test_args.py
```

### Comparing `fixinventorymetrics-4.0.1/PKG-INFO` & `fixinventorymetrics-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventorymetrics
-Version: 4.0.1
+Version: 4.0.2
 Summary: Exports Fix Inventory metrics in Prometheus format.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixmetrics
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
 
 # `fixmetrics`
 Fix Prometheus exporter
 
 
 ## Table of contents
```

### Comparing `fixinventorymetrics-4.0.1/README.md` & `fixinventorymetrics-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/fixinventorymetrics.egg-info/PKG-INFO` & `fixinventorymetrics-4.0.2/fixinventorymetrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: fixinventorymetrics
-Version: 4.0.1
+Version: 4.0.2
 Summary: Exports Fix Inventory metrics in Prometheus format.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/fixmetrics
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
 
 # `fixmetrics`
 Fix Prometheus exporter
 
 
 ## Table of contents
```

### Comparing `fixinventorymetrics-4.0.1/fixmetrics/__main__.py` & `fixinventorymetrics-4.0.2/fixmetrics/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/fixmetrics/config.py` & `fixinventorymetrics-4.0.2/fixmetrics/config.py`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/fixmetrics/default_metrics.yaml` & `fixinventorymetrics-4.0.2/fixmetrics/default_metrics.yaml`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/fixmetrics/metrics.py` & `fixinventorymetrics-4.0.2/fixmetrics/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/fixmetrics/search.py` & `fixinventorymetrics-4.0.2/fixmetrics/search.py`

 * *Files identical despite different names*

### Comparing `fixinventorymetrics-4.0.1/pyproject.toml` & `fixinventorymetrics-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "fixinventorymetrics"
-version = "4.0.1"
+version = "4.0.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Exports Fix Inventory metrics in Prometheus format."
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
 
 dependencies = [
-    "fixinventorylib==4.0.1"
+    "fixinventorylib==4.0.2"
 ]
 
 [pyproject.optional-dependencies]
 test = ["pytest"]
 
 [project.scripts]
 fixmetrics = "fixmetrics.__main__:main"
```

### Comparing `fixinventorymetrics-4.0.1/test/test_args.py` & `fixinventorymetrics-4.0.2/test/test_args.py`

 * *Files identical despite different names*

