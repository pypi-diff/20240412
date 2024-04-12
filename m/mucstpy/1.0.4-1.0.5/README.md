# Comparing `tmp/mucstpy-1.0.4.tar.gz` & `tmp/mucstpy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mucstpy-1.0.4.tar", last modified: Fri Apr 12 03:20:31 2024, max compression
+gzip compressed data, was "mucstpy-1.0.5.tar", last modified: Fri Apr 12 03:35:23 2024, max compression
```

## Comparing `mucstpy-1.0.4.tar` & `mucstpy-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:20:31.639679 mucstpy-1.0.4/
--rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      556 2024-04-12 03:20:31.638680 mucstpy-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.4/README.md
--rw-rw-rw-   0        0        0      972 2024-04-12 03:16:39.000000 mucstpy-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 03:20:31.639679 mucstpy-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 03:20:31.617399 mucstpy-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 03:20:31.633168 mucstpy-1.0.4/src/mucstpy/
--rw-rw-rw-   0        0        0     5144 2024-04-12 03:16:51.000000 mucstpy-1.0.4/src/mucstpy/MuCST.py
--rw-rw-rw-   0        0        0      142 2024-04-12 03:16:39.000000 mucstpy-1.0.4/src/mucstpy/__init__.py
--rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.4/src/mucstpy/image_feature.py
--rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.4/src/mucstpy/loss.py
--rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.4/src/mucstpy/model.py
--rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.4/src/mucstpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:20:31.637678 mucstpy-1.0.4/src/mucstpy.egg-info/
--rw-rw-rw-   0        0        0      556 2024-04-12 03:20:31.000000 mucstpy-1.0.4/src/mucstpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-12 03:20:31.000000 mucstpy-1.0.4/src/mucstpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:20:31.000000 mucstpy-1.0.4/src/mucstpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-04-12 03:20:31.000000 mucstpy-1.0.4/src/mucstpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 03:20:31.000000 mucstpy-1.0.4/src/mucstpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.495657 mucstpy-1.0.5/
+-rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4330 2024-04-12 03:35:23.494657 mucstpy-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.5/README.md
+-rw-rw-rw-   0        0        0      849 2024-04-12 03:35:12.000000 mucstpy-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 03:35:23.495657 mucstpy-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.480657 mucstpy-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.488657 mucstpy-1.0.5/src/mucstpy/
+-rw-rw-rw-   0        0        0     5144 2024-04-12 03:16:51.000000 mucstpy-1.0.5/src/mucstpy/MuCST.py
+-rw-rw-rw-   0        0        0      142 2024-04-12 03:35:12.000000 mucstpy-1.0.5/src/mucstpy/__init__.py
+-rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.5/src/mucstpy/image_feature.py
+-rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.5/src/mucstpy/loss.py
+-rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.5/src/mucstpy/model.py
+-rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.5/src/mucstpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 03:35:23.493657 mucstpy-1.0.5/src/mucstpy.egg-info/
+-rw-rw-rw-   0        0        0     4330 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 03:35:23.000000 mucstpy-1.0.5/src/mucstpy.egg-info/top_level.txt
```

### Comparing `mucstpy-1.0.4/LICENSE` & `mucstpy-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/README.md` & `mucstpy-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/pyproject.toml` & `mucstpy-1.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #[build-system]
 #requires = ["setuptools", "wheel"]
 #build-backend = "setuptools.build_meta"
 
 [project]
 name = "mucstpy"
-version = "1.0.4"
+version = "1.0.5"
 
 dependencies=[
     "scanpy>=1.9.3",
     "numpy",
     "pandas",
     "anndata",
     "matplotlib",
@@ -18,18 +18,14 @@
     "tqdm",
     "leidenalg",
     "torch>=2.0",
     "torchvision",
     "pathlib",
     "torchvision",
 ]
-[tool.poetry.dependencies]
-torchtoolbox = {git = "https://github.com/bbchond/torch-toolbox.git", branch  = "master"}
-
-
 authors = [
   { name="Yu Wang", email="qq352542417@gmail.com" },
 ]
 description = "The initial package of MuCST"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mucstpy-1.0.4/src/mucstpy/MuCST.py` & `mucstpy-1.0.5/src/mucstpy/MuCST.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/src/mucstpy/image_feature.py` & `mucstpy-1.0.5/src/mucstpy/image_feature.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/src/mucstpy/loss.py` & `mucstpy-1.0.5/src/mucstpy/loss.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/src/mucstpy/model.py` & `mucstpy-1.0.5/src/mucstpy/model.py`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.4/src/mucstpy/utils.py` & `mucstpy-1.0.5/src/mucstpy/utils.py`

 * *Files identical despite different names*

