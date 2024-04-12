# Comparing `tmp/mucstpy-1.0.5.tar.gz` & `tmp/mucstpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mucstpy-1.0.5.tar", last modified: Fri Apr 12 03:35:23 2024, max compression
+gzip compressed data, was "mucstpy-1.0.6.tar", last modified: Fri Apr 12 03:38:17 2024, max compression
```

## Comparing `mucstpy-1.0.5.tar` & `mucstpy-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.495657 mucstpy-1.0.5/
--rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     4330 2024-04-12 03:35:23.494657 mucstpy-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.5/README.md
--rw-rw-rw-   0        0        0      849 2024-04-12 03:35:12.000000 mucstpy-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 03:35:23.495657 mucstpy-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.480657 mucstpy-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.488657 mucstpy-1.0.5/src/mucstpy/
--rw-rw-rw-   0        0        0     5144 2024-04-12 03:16:51.000000 mucstpy-1.0.5/src/mucstpy/MuCST.py
--rw-rw-rw-   0        0        0      142 2024-04-12 03:35:12.000000 mucstpy-1.0.5/src/mucstpy/__init__.py
--rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.5/src/mucstpy/image_feature.py
--rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.5/src/mucstpy/loss.py
--rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.5/src/mucstpy/model.py
--rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.5/src/mucstpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.493657 mucstpy-1.0.5/src/mucstpy.egg-info/
--rw-rw-rw-   0        0        0     4330 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 03:38:17.068548 mucstpy-1.0.6/
+-rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4350 2024-04-12 03:38:17.067548 mucstpy-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.6/README.md
+-rw-rw-rw-   0        0        0      860 2024-04-12 03:37:39.000000 mucstpy-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 03:38:17.068548 mucstpy-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 03:38:17.045409 mucstpy-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 03:38:17.062546 mucstpy-1.0.6/src/mucstpy/
+-rw-rw-rw-   0        0        0     5144 2024-04-12 03:16:51.000000 mucstpy-1.0.6/src/mucstpy/MuCST.py
+-rw-rw-rw-   0        0        0      142 2024-04-12 03:38:07.000000 mucstpy-1.0.6/src/mucstpy/__init__.py
+-rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.6/src/mucstpy/image_feature.py
+-rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.6/src/mucstpy/loss.py
+-rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.6/src/mucstpy/model.py
+-rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.6/src/mucstpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:38:17.066548 mucstpy-1.0.6/src/mucstpy.egg-info/
+-rw-rw-rw-   0        0        0     4350 2024-04-12 03:38:17.000000 mucstpy-1.0.6/src/mucstpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-12 03:38:17.000000 mucstpy-1.0.6/src/mucstpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 03:38:17.000000 mucstpy-1.0.6/src/mucstpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-04-12 03:38:17.000000 mucstpy-1.0.6/src/mucstpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 03:38:17.000000 mucstpy-1.0.6/src/mucstpy.egg-info/top_level.txt
```

### Comparing `mucstpy-1.0.5/LICENSE` & `mucstpy-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/PKG-INFO` & `mucstpy-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mucstpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: The initial package of MuCST
 Author-email: Yu Wang <qq352542417@gmail.com>
 Project-URL: Homepage, https://github.com/xkmaxidian/MuCST
 Project-URL: Issues, https://github.com/xkmaxidian/MuCST/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,15 @@
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: leidenalg
 Requires-Dist: torch>=2.0
 Requires-Dist: torchvision
 Requires-Dist: pathlib
 Requires-Dist: torchvision
+Requires-Dist: POT
 
 # MuCST v1.0
 
 ## MuCST: restoring and integrating heterogeneous morphology images and spatial transcriptomics data with contrastive learning
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10627683.svg)](https://doi.org/10.5281/zenodo.10627683)
```

### Comparing `mucstpy-1.0.5/README.md` & `mucstpy-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/pyproject.toml` & `mucstpy-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #[build-system]
 #requires = ["setuptools", "wheel"]
 #build-backend = "setuptools.build_meta"
 
 [project]
 name = "mucstpy"
-version = "1.0.5"
+version = "1.0.6"
 
 dependencies=[
     "scanpy>=1.9.3",
     "numpy",
     "pandas",
     "anndata",
     "matplotlib",
@@ -17,14 +17,15 @@
     "psutil",
     "tqdm",
     "leidenalg",
     "torch>=2.0",
     "torchvision",
     "pathlib",
     "torchvision",
+    "POT"
 ]
 authors = [
   { name="Yu Wang", email="qq352542417@gmail.com" },
 ]
 description = "The initial package of MuCST"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `mucstpy-1.0.5/src/mucstpy/MuCST.py` & `mucstpy-1.0.6/src/mucstpy/MuCST.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/src/mucstpy/image_feature.py` & `mucstpy-1.0.6/src/mucstpy/image_feature.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/src/mucstpy/loss.py` & `mucstpy-1.0.6/src/mucstpy/loss.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/src/mucstpy/model.py` & `mucstpy-1.0.6/src/mucstpy/model.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/src/mucstpy/utils.py` & `mucstpy-1.0.6/src/mucstpy/utils.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.5/src/mucstpy.egg-info/PKG-INFO` & `mucstpy-1.0.6/src/mucstpy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mucstpy
-Version: 1.0.5
+Version: 1.0.6
 Summary: The initial package of MuCST
 Author-email: Yu Wang <qq352542417@gmail.com>
 Project-URL: Homepage, https://github.com/xkmaxidian/MuCST
 Project-URL: Issues, https://github.com/xkmaxidian/MuCST/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,14 +21,15 @@
 Requires-Dist: psutil
 Requires-Dist: tqdm
 Requires-Dist: leidenalg
 Requires-Dist: torch>=2.0
 Requires-Dist: torchvision
 Requires-Dist: pathlib
 Requires-Dist: torchvision
+Requires-Dist: POT
 
 # MuCST v1.0
 
 ## MuCST: restoring and integrating heterogeneous morphology images and spatial transcriptomics data with contrastive learning
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10627683.svg)](https://doi.org/10.5281/zenodo.10627683)
```

