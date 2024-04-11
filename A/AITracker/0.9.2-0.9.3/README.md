# Comparing `tmp/AITracker-0.9.2.tar.gz` & `tmp/AITracker-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AITracker-0.9.2.tar", last modified: Thu Apr 11 23:03:02 2024, max compression
+gzip compressed data, was "AITracker-0.9.3.tar", last modified: Thu Apr 11 23:08:23 2024, max compression
```

## Comparing `AITracker-0.9.2.tar` & `AITracker-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:03:02.715741 AITracker-0.9.2/
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:03:02.714640 AITracker-0.9.2/AITracker.egg-info/
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 23:03:02.000000 AITracker-0.9.2/AITracker.egg-info/PKG-INFO
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      382 2024-04-11 23:03:02.000000 AITracker-0.9.2/AITracker.egg-info/SOURCES.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)        1 2024-04-11 23:03:02.000000 AITracker-0.9.2/AITracker.egg-info/dependency_links.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      118 2024-04-11 23:03:02.000000 AITracker-0.9.2/AITracker.egg-info/requires.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)       10 2024-04-11 23:03:02.000000 AITracker-0.9.2/AITracker.egg-info/top_level.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)    35148 2024-04-08 01:15:01.000000 AITracker-0.9.2/LICENSE.txt
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 23:03:02.715192 AITracker-0.9.2/PKG-INFO
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      635 2024-04-11 17:38:51.000000 AITracker-0.9.2/README.md
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      937 2024-04-11 23:02:52.000000 AITracker-0.9.2/pyproject.toml
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 23:03:02.715872 AITracker-0.9.2/setup.cfg
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      187 2024-04-11 23:02:36.000000 AITracker-0.9.2/setup.py
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:03:02.704752 AITracker-0.9.2/src/
-drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:03:02.713794 AITracker-0.9.2/src/AITracker/
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     6952 2024-04-11 20:42:46.000000 AITracker-0.9.2/src/AITracker/AITrackerModel.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2404 2024-04-10 20:07:39.000000 AITracker-0.9.2/src/AITracker/AITrackerNetwork.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)     3823 2024-03-19 04:01:33.000000 AITracker-0.9.2/src/AITracker/DataValidation.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)    13617 2024-04-09 05:51:37.000000 AITracker-0.9.2/src/AITracker/UpdateH5.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 17:40:32.000000 AITracker-0.9.2/src/AITracker/__init__.py
--rw-r--r--   0 jacobhogrefe   (501) staff       (20)      115 2024-04-11 22:54:19.000000 AITracker-0.9.2/src/AITracker/setup.py
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:08:23.367911 AITracker-0.9.3/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)    35148 2024-04-08 01:15:01.000000 AITracker-0.9.3/LICENSE.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 23:08:23.367522 AITracker-0.9.3/PKG-INFO
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      635 2024-04-11 17:38:51.000000 AITracker-0.9.3/README.md
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      971 2024-04-11 23:08:12.000000 AITracker-0.9.3/pyproject.toml
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)       38 2024-04-11 23:08:23.368001 AITracker-0.9.3/setup.cfg
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      153 2024-04-11 23:07:56.000000 AITracker-0.9.3/setup.py
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:08:23.359492 AITracker-0.9.3/src/
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:08:23.364649 AITracker-0.9.3/src/AITracker/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     6952 2024-04-11 20:42:46.000000 AITracker-0.9.3/src/AITracker/AITrackerModel.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     2404 2024-04-10 20:07:39.000000 AITracker-0.9.3/src/AITracker/AITrackerNetwork.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     3823 2024-03-19 04:01:33.000000 AITracker-0.9.3/src/AITracker/DataValidation.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)    13617 2024-04-09 05:51:37.000000 AITracker-0.9.3/src/AITracker/UpdateH5.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 17:40:32.000000 AITracker-0.9.3/src/AITracker/__init__.py
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      115 2024-04-11 22:54:19.000000 AITracker-0.9.3/src/AITracker/setup.py
+drwxr-xr-x   0 jacobhogrefe   (501) staff       (20)        0 2024-04-11 23:08:23.367058 AITracker-0.9.3/src/AITracker.egg-info/
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)     1494 2024-04-11 23:08:23.000000 AITracker-0.9.3/src/AITracker.egg-info/PKG-INFO
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      402 2024-04-11 23:08:23.000000 AITracker-0.9.3/src/AITracker.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)        1 2024-04-11 23:08:23.000000 AITracker-0.9.3/src/AITracker.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)      118 2024-04-11 23:08:23.000000 AITracker-0.9.3/src/AITracker.egg-info/requires.txt
+-rw-r--r--   0 jacobhogrefe   (501) staff       (20)       10 2024-04-11 23:08:23.000000 AITracker-0.9.3/src/AITracker.egg-info/top_level.txt
```

### Comparing `AITracker-0.9.2/AITracker.egg-info/PKG-INFO` & `AITracker-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AITracker
-Version: 0.9.2
+Version: 0.9.3
 Summary: The AITracker neural network and it's implementation.
 Author: Jacob Hogrefe and Emilio Cruz
 Project-URL: Homepage, https://github.com/AITrackerDev/AITracker
 Project-URL: Issues, https://github.com/AITrackerDev/AITracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `AITracker-0.9.2/LICENSE.txt` & `AITracker-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.2/PKG-INFO` & `AITracker-0.9.3/src/AITracker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AITracker
-Version: 0.9.2
+Version: 0.9.3
 Summary: The AITracker neural network and it's implementation.
 Author: Jacob Hogrefe and Emilio Cruz
 Project-URL: Homepage, https://github.com/AITrackerDev/AITracker
 Project-URL: Issues, https://github.com/AITrackerDev/AITracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `AITracker-0.9.2/README.md` & `AITracker-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.2/pyproject.toml` & `AITracker-0.9.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AITracker"
-version = "0.9.2"
+version = "0.9.3"
 authors = [{ name = "Jacob Hogrefe and Emilio Cruz" }]
 description = "The AITracker neural network and it's implementation."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -27,8 +27,11 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/AITrackerDev/AITracker"
 Issues = "https://github.com/AITrackerDev/AITracker/issues"
 
 [tool.setuptools]
-package-data = {"AITracker" = ["*.model"]}
+include-package-data = true
+
+[tool.setuptools.packages.find]
+where = ["src"]
```

### Comparing `AITracker-0.9.2/src/AITracker/AITrackerModel.py` & `AITracker-0.9.3/src/AITracker/AITrackerModel.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.2/src/AITracker/AITrackerNetwork.py` & `AITracker-0.9.3/src/AITracker/AITrackerNetwork.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.2/src/AITracker/DataValidation.py` & `AITracker-0.9.3/src/AITracker/DataValidation.py`

 * *Files identical despite different names*

### Comparing `AITracker-0.9.2/src/AITracker/UpdateH5.py` & `AITracker-0.9.3/src/AITracker/UpdateH5.py`

 * *Files identical despite different names*

