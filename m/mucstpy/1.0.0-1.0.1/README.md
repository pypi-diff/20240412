# Comparing `tmp/mucstpy-1.0.0.tar.gz` & `tmp/mucstpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mucstpy-1.0.0.tar", last modified: Thu Apr 11 19:46:46 2024, max compression
+gzip compressed data, was "mucstpy-1.0.1.tar", last modified: Thu Apr 11 20:42:04 2024, max compression
```

## Comparing `mucstpy-1.0.0.tar` & `mucstpy-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 19:46:46.923534 mucstpy-1.0.0/
--rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4474 2024-04-11 19:46:46.922535 mucstpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3567 2024-04-11 19:41:33.000000 mucstpy-1.0.0/README.md
--rw-rw-rw-   0        0        0      877 2024-04-11 19:45:29.000000 mucstpy-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 19:46:46.923534 mucstpy-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 19:46:46.910793 mucstpy-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 19:46:46.916932 mucstpy-1.0.0/src/mucstpy/
--rw-rw-rw-   0        0        0     5199 2024-04-11 19:32:18.000000 mucstpy-1.0.0/src/mucstpy/MuCST.py
--rw-rw-rw-   0        0        0      140 2024-04-11 19:27:17.000000 mucstpy-1.0.0/src/mucstpy/__init__.py
--rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.0/src/mucstpy/image_feature.py
--rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.0/src/mucstpy/loss.py
--rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.0/src/mucstpy/model.py
--rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.0/src/mucstpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 19:46:46.921159 mucstpy-1.0.0/src/mucstpy.egg-info/
--rw-rw-rw-   0        0        0     4474 2024-04-11 19:46:46.000000 mucstpy-1.0.0/src/mucstpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-11 19:46:46.000000 mucstpy-1.0.0/src/mucstpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 19:46:46.000000 mucstpy-1.0.0/src/mucstpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2024-04-11 19:46:46.000000 mucstpy-1.0.0/src/mucstpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-11 19:46:46.000000 mucstpy-1.0.0/src/mucstpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 20:42:04.535642 mucstpy-1.0.1/
+-rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      556 2024-04-11 20:42:04.535642 mucstpy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3567 2024-04-11 19:41:33.000000 mucstpy-1.0.1/README.md
+-rw-rw-rw-   0        0        0      958 2024-04-11 20:39:36.000000 mucstpy-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:42:04.536641 mucstpy-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 20:42:04.524498 mucstpy-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 20:42:04.530481 mucstpy-1.0.1/src/mucstpy/
+-rw-rw-rw-   0        0        0     5199 2024-04-11 19:32:18.000000 mucstpy-1.0.1/src/mucstpy/MuCST.py
+-rw-rw-rw-   0        0        0      142 2024-04-11 20:35:41.000000 mucstpy-1.0.1/src/mucstpy/__init__.py
+-rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.1/src/mucstpy/image_feature.py
+-rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.1/src/mucstpy/loss.py
+-rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.1/src/mucstpy/model.py
+-rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.1/src/mucstpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:42:04.534470 mucstpy-1.0.1/src/mucstpy.egg-info/
+-rw-rw-rw-   0        0        0      556 2024-04-11 20:42:04.000000 mucstpy-1.0.1/src/mucstpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-11 20:42:04.000000 mucstpy-1.0.1/src/mucstpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:42:04.000000 mucstpy-1.0.1/src/mucstpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-04-11 20:42:04.000000 mucstpy-1.0.1/src/mucstpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-11 20:42:04.000000 mucstpy-1.0.1/src/mucstpy.egg-info/top_level.txt
```

### Comparing `mucstpy-1.0.0/LICENSE` & `mucstpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.0/PKG-INFO` & `mucstpy-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: mucstpy
-Version: 1.0.0
-Summary: The initial package of MuCST
-Author-email: Yu Wang <qq352542417@gmail.com>
-Project-URL: Homepage, https://github.com/xkmaxidian/MuCST
-Project-URL: Issues, https://github.com/xkmaxidian/MuCST/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scanpy>=1.9.3
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: anndata
-Requires-Dist: matplotlib
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: psutil
-Requires-Dist: tqdm
-Requires-Dist: leidenalg
-Requires-Dist: torch>=2.0
-Requires-Dist: torchvision
-Requires-Dist: pathlib
-Requires-Dist: torchvision
-Requires-Dist: torchtoolbox
-Requires-Dist: POT
-
 # MuCST v1.0
 
 ## MuCST: restoring and integrating heterogeneous morphology images and spatial transcriptomics data with contrastive learning
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10627683.svg)](https://doi.org/10.5281/zenodo.10627683)
 
 ###  Yu Wang, Xiaoke Ma
```

### Comparing `mucstpy-1.0.0/pyproject.toml` & `mucstpy-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #[build-system]
 #requires = ["setuptools", "wheel"]
 #build-backend = "setuptools.build_meta"
 [project]
 name = "mucstpy"
-version = "1.0.0"
+version = "1.0.1"
 dependencies=[
     "scanpy>=1.9.3",
     "numpy",
     "pandas",
     "anndata",
     "matplotlib",
     "scipy",
@@ -15,17 +15,19 @@
     "psutil",
     "tqdm",
     "leidenalg",
     "torch>=2.0",
     "torchvision",
     "pathlib",
     "torchvision",
-    "torchtoolbox",
-    "POT"
 ]
+[tool.poetry.source]
+torchtoolbox = {url = "https://github.com/bbchond/torch-toolbox.git", rev = "master"}
+
+
 authors = [
   { name="Yu Wang", email="qq352542417@gmail.com" },
 ]
 description = "The initial package of MuCST"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mucstpy-1.0.0/src/mucstpy/MuCST.py` & `mucstpy-1.0.1/src/mucstpy/MuCST.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.0/src/mucstpy/image_feature.py` & `mucstpy-1.0.1/src/mucstpy/image_feature.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.0/src/mucstpy/loss.py` & `mucstpy-1.0.1/src/mucstpy/loss.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.0/src/mucstpy/model.py` & `mucstpy-1.0.1/src/mucstpy/model.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.0/src/mucstpy/utils.py` & `mucstpy-1.0.1/src/mucstpy/utils.py`

 * *Files identical despite different names*

