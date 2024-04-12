# Comparing `tmp/clustutils4r-0.0.8.tar.gz` & `tmp/clustutils4r-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustutils4r-0.0.8.tar", last modified: Sun Jul 16 08:29:46 2023, max compression
+gzip compressed data, was "clustutils4r-1.0.0.tar", last modified: Fri Apr 12 05:30:56 2024, max compression
```

## Comparing `clustutils4r-0.0.8.tar` & `clustutils4r-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-0.0.8/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5423 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4791 2023-07-16 08:28:10.000000 clustutils4r-0.0.8/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2023-07-16 08:29:32.000000 clustutils4r-0.0.8/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:29:24.000000 clustutils4r-0.0.8/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/clustutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-0.0.8/src/clustutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    28396 2023-07-16 08:18:23.000000 clustutils4r-0.0.8/src/clustutils4r/eval_clustering.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-16 08:29:46.615291 clustutils4r-0.0.8/src/clustutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5423 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      305 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       44 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2023-07-16 08:29:46.000000 clustutils4r-0.0.8/src/clustutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2023-07-13 07:56:53.000000 clustutils4r-1.0.0/LICENSE
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     5423 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     4791 2023-07-16 08:28:10.000000 clustutils4r-1.0.0/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      659 2024-04-12 05:30:33.000000 clustutils4r-1.0.0/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      978 2023-07-16 08:29:24.000000 clustutils4r-1.0.0/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/src/clustutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2023-07-13 05:33:28.000000 clustutils4r-1.0.0/src/clustutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    25864 2024-04-12 04:58:42.000000 clustutils4r-1.0.0/src/clustutils4r/eval_clustering.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2024-04-12 05:30:56.484463 clustutils4r-1.0.0/src/clustutils4r.egg-info/
+-rw-r--r--   0 rgura001 (52843) rgura001 (52843)     5423 2024-04-12 05:30:56.000000 clustutils4r-1.0.0/src/clustutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      266 2024-04-12 05:30:56.000000 clustutils4r-1.0.0/src/clustutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2024-04-12 05:30:56.000000 clustutils4r-1.0.0/src/clustutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       13 2024-04-12 05:30:56.000000 clustutils4r-1.0.0/src/clustutils4r.egg-info/top_level.txt
```

### Comparing `clustutils4r-0.0.8/LICENSE` & `clustutils4r-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.8/PKG-INFO` & `clustutils4r-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.8
+Version: 1.0.0
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clustutils4r-0.0.8/README.md` & `clustutils4r-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.8/pyproject.toml` & `clustutils4r-1.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clustutils4r"
-version = "0.0.8"
+version = "1.0.0"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn utilities for clustering."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers=[
```

### Comparing `clustutils4r-0.0.8/setup.py` & `clustutils4r-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `clustutils4r-0.0.8/src/clustutils4r.egg-info/PKG-INFO` & `clustutils4r-1.0.0/src/clustutils4r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clustutils4r
-Version: 0.0.8
+Version: 1.0.0
 Summary: Wrapper around some basic sklearn utilities for clustering.
 Home-page: https://github.com/rutujagurav/clustutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clustutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clustutils4r/issues
 Classifier: Programming Language :: Python :: 3
```

