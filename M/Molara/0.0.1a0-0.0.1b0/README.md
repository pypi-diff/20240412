# Comparing `tmp/Molara-0.0.1a0.tar.gz` & `tmp/Molara-0.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Molara-0.0.1a0.tar", last modified: Fri Apr 12 09:58:46 2024, max compression
+gzip compressed data, was "Molara-0.0.1b0.tar", last modified: Fri Apr 12 10:34:55 2024, max compression
```

## Comparing `Molara-0.0.1a0.tar` & `Molara-0.0.1b0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:58:46.806546 Molara-0.0.1a0/
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    35149 2023-09-07 16:46:05.000000 Molara-0.0.1a0/LICENSE
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    44132 2024-04-12 09:58:46.806170 Molara-0.0.1a0/PKG-INFO
--rw-r--r--   0 alexbonkowski   (501) staff       (20)     1645 2024-04-10 18:07:25.000000 Molara-0.0.1a0/README.md
--rw-r--r--   0 alexbonkowski   (501) staff       (20)     3353 2024-04-12 09:58:31.000000 Molara-0.0.1a0/pyproject.toml
--rw-r--r--   0 alexbonkowski   (501) staff       (20)       38 2024-04-12 09:58:46.806614 Molara-0.0.1a0/setup.cfg
--rw-r--r--   0 alexbonkowski   (501) staff       (20)      435 2024-04-12 09:56:04.000000 Molara-0.0.1a0/setup.py
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:58:46.800312 Molara-0.0.1a0/src/
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:58:46.804725 Molara-0.0.1a0/src/Molara.egg-info/
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    44132 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/PKG-INFO
--rw-r--r--   0 alexbonkowski   (501) staff       (20)      279 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/SOURCES.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)        1 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/dependency_links.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)       48 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/entry_points.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)      189 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/requires.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)        7 2024-04-12 09:58:46.000000 Molara-0.0.1a0/src/Molara.egg-info/top_level.txt
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:58:46.800191 Molara-0.0.1a0/src/molara/
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:58:46.801363 Molara-0.0.1a0/src/molara/Tools/
--rw-r--r--   0 alexbonkowski   (501) staff       (20)  1124658 2024-04-12 09:56:17.000000 Molara-0.0.1a0/src/molara/Tools/raycasting.c
+drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 10:34:55.324933 Molara-0.0.1b0/
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)    35149 2023-09-07 16:46:05.000000 Molara-0.0.1b0/LICENSE
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)    44132 2024-04-12 10:34:55.324534 Molara-0.0.1b0/PKG-INFO
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)     1645 2024-04-10 18:07:25.000000 Molara-0.0.1b0/README.md
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)     3278 2024-04-12 10:34:49.000000 Molara-0.0.1b0/pyproject.toml
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)       38 2024-04-12 10:34:55.325213 Molara-0.0.1b0/setup.cfg
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)      435 2024-04-12 09:56:04.000000 Molara-0.0.1b0/setup.py
+drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 10:34:55.313853 Molara-0.0.1b0/src/
+drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 10:34:55.322234 Molara-0.0.1b0/src/Molara.egg-info/
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)    44132 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/PKG-INFO
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)      325 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)        1 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)       48 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/entry_points.txt
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)      189 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/requires.txt
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)        7 2024-04-12 10:34:55.000000 Molara-0.0.1b0/src/Molara.egg-info/top_level.txt
+drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 10:34:55.321644 Molara-0.0.1b0/src/molara/
+drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 10:34:55.316478 Molara-0.0.1b0/src/molara/Tools/
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)  1124658 2024-04-12 09:56:17.000000 Molara-0.0.1b0/src/molara/Tools/raycasting.c
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)      114 2024-03-19 11:22:10.000000 Molara-0.0.1b0/src/molara/__init__.py
+-rw-r--r--   0 alexbonkowski   (501) staff       (20)     1008 2024-04-10 18:07:25.000000 Molara-0.0.1b0/src/molara/__main__.py
```

### Comparing `Molara-0.0.1a0/LICENSE` & `Molara-0.0.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `Molara-0.0.1a0/PKG-INFO` & `Molara-0.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Molara
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: A visualisation tool for chemical structures.
 Author: Michel Heinz, Gereon Feldmann
 Author-email: Adrian Usler <adrian.usler@rwth-aachen.de>, Alexander Bonkowski <alexander.bonkowski@rwth-aachen.de>
 Maintainer: Michel Heinz, Gereon Feldmann, Adrian Usler, Alexander Bonkowski
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `Molara-0.0.1a0/README.md` & `Molara-0.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `Molara-0.0.1a0/pyproject.toml` & `Molara-0.0.1b0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "cython", "numpy", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Molara"
-version = "0.0.1a"
+version = "0.0.1b"
 description = "A visualisation tool for chemical structures."
 authors = [
     {name = "Michel Heinz"},
     {name = "Gereon Feldmann"},
     {name = "Adrian Usler", email = "adrian.usler@rwth-aachen.de"},
     {name = "Alexander Bonkowski", email = "alexander.bonkowski@rwth-aachen.de"},
 ]
@@ -65,20 +65,17 @@
     "ase",
 ]
 
 [project.scripts]
 molara = "molara.__main__:main"
 
 [tool.setuptools]
+packages = ["molara"]
 package-dir = {"" = "src"}
 
-[tool.setuptools.packages.find]
-include = ["molara", "molara.*"]
-exclude = ["tests", "tests.*"]
-
 [tool.ruff]
 exclude = ["ui_*",]
 target-version = "py39"
 line-length = 120
 lint.select = ["ALL"]
 lint.ignore = [
   "ANN101", # Missing type annotation for `self` in method
```

### Comparing `Molara-0.0.1a0/src/Molara.egg-info/PKG-INFO` & `Molara-0.0.1b0/src/Molara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Molara
-Version: 0.0.1a0
+Version: 0.0.1b0
 Summary: A visualisation tool for chemical structures.
 Author: Michel Heinz, Gereon Feldmann
 Author-email: Adrian Usler <adrian.usler@rwth-aachen.de>, Alexander Bonkowski <alexander.bonkowski@rwth-aachen.de>
 Maintainer: Michel Heinz, Gereon Feldmann, Adrian Usler, Alexander Bonkowski
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `Molara-0.0.1a0/src/molara/Tools/raycasting.c` & `Molara-0.0.1b0/src/molara/Tools/raycasting.c`

 * *Files identical despite different names*

