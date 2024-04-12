# Comparing `tmp/Molara-0.0.1.tar.gz` & `tmp/Molara-0.0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Molara-0.0.1.tar", last modified: Fri Apr 12 09:31:45 2024, max compression
+gzip compressed data, was "Molara-0.0.1.7.tar", last modified: Fri Apr 12 16:29:43 2024, max compression
```

## Comparing `Molara-0.0.1.tar` & `Molara-0.0.1.7.tar`

### file list

```diff
@@ -1,14 +1,71 @@
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:31:45.539351 Molara-0.0.1/
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    35149 2023-09-07 16:46:05.000000 Molara-0.0.1/LICENSE
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    44130 2024-04-12 09:31:45.538955 Molara-0.0.1/PKG-INFO
--rw-r--r--   0 alexbonkowski   (501) staff       (20)     1645 2024-04-10 18:07:25.000000 Molara-0.0.1/README.md
--rw-r--r--   0 alexbonkowski   (501) staff       (20)     3352 2024-04-10 18:07:25.000000 Molara-0.0.1/pyproject.toml
--rw-r--r--   0 alexbonkowski   (501) staff       (20)       38 2024-04-12 09:31:45.539422 Molara-0.0.1/setup.cfg
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:31:45.534290 Molara-0.0.1/src/
-drwxr-xr-x   0 alexbonkowski   (501) staff       (20)        0 2024-04-12 09:31:45.537219 Molara-0.0.1/src/Molara.egg-info/
--rw-r--r--   0 alexbonkowski   (501) staff       (20)    44130 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/PKG-INFO
--rw-r--r--   0 alexbonkowski   (501) staff       (20)      238 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/SOURCES.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)        1 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/dependency_links.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)       48 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/entry_points.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)      189 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/requires.txt
--rw-r--r--   0 alexbonkowski   (501) staff       (20)        1 2024-04-12 09:31:45.000000 Molara-0.0.1/src/Molara.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.597966 Molara-0.0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 16:29:35.000000 Molara-0.0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 16:29:35.000000 Molara-0.0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44132 2024-04-12 16:29:43.597966 Molara-0.0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-12 16:29:35.000000 Molara-0.0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-12 16:29:35.000000 Molara-0.0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:29:43.597966 Molara-0.0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-12 16:29:35.000000 Molara-0.0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.581966 Molara-0.0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.597966 Molara-0.0.1.7/src/Molara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44132 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 16:29:43.000000 Molara-0.0.1.7/src/Molara.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.585966 Molara-0.0.1.7/src/molara/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.585966 Molara-0.0.1.7/src/molara/Eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Eval/aos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.585966 Molara-0.0.1.7/src/molara/Gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19184 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/crystal_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/measuring_tool_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22948 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/structure_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/supercell_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/trajectory_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18568 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_crystalstructure_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_measuring_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_supercell_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Gui/ui_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.589966 Molara-0.0.1.7/src/molara/Rendering/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/buffers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)   641086 2024-04-12 16:29:41.000000 Molara-0.0.1.7/src/molara/Rendering/cylinder.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/cylinder.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1288362 2024-04-12 16:29:41.000000 Molara-0.0.1.7/src/molara/Rendering/matrices.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/matrices.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)   536648 2024-04-12 16:29:41.000000 Molara-0.0.1.7/src/molara/Rendering/sphere.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Rendering/sphere.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.593966 Molara-0.0.1.7/src/molara/Structure/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37072 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/basisset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/crystals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9377 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/drawer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.593966 Molara-0.0.1.7/src/molara/Structure/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/io/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/io/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/io/importer_crystal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/molecules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/mos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Structure/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:29:43.597966 Molara-0.0.1.7/src/molara/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1015008 2024-04-12 16:29:42.000000 Molara-0.0.1.7/src/molara/Tools/mathtools.c
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Tools/mathtools.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1124656 2024-04-12 16:29:42.000000 Molara-0.0.1.7/src/molara/Tools/raycasting.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/Tools/raycasting.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-12 16:29:35.000000 Molara-0.0.1.7/src/molara/__main__.py
```

### Comparing `Molara-0.0.1/LICENSE` & `Molara-0.0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Molara-0.0.1/PKG-INFO` & `Molara-0.0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Molara
-Version: 0.0.1
+Version: 0.0.1.7
 Summary: A visualisation tool for chemical structures.
 Author: Michel Heinz, Gereon Feldmann
 Author-email: Adrian Usler <adrian.usler@rwth-aachen.de>, Alexander Bonkowski <alexander.bonkowski@rwth-aachen.de>
 Maintainer: Michel Heinz, Gereon Feldmann, Adrian Usler, Alexander Bonkowski
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `Molara-0.0.1/README.md` & `Molara-0.0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `Molara-0.0.1/pyproject.toml` & `Molara-0.0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 [build-system]
 requires = ["setuptools>=65.0.0", "cython", "numpy", "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools]
+package-dir = {"" = "src"}
+
+[tool.cibuildwheel.linux]
+skip = ["*musllinux*"]
+
 [project]
 name = "Molara"
-version = "0.0.1"
+version = "0.0.1.7"
 description = "A visualisation tool for chemical structures."
 authors = [
     {name = "Michel Heinz"},
     {name = "Gereon Feldmann"},
     {name = "Adrian Usler", email = "adrian.usler@rwth-aachen.de"},
     {name = "Alexander Bonkowski", email = "alexander.bonkowski@rwth-aachen.de"},
 ]
@@ -64,21 +70,14 @@
     "pymatgen",
     "ase",
 ]
 
 [project.scripts]
 molara = "molara.__main__:main"
 
-[tool.setuptools]
-package-dir = {"" = "src"}
-
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

### Comparing `Molara-0.0.1/src/Molara.egg-info/PKG-INFO` & `Molara-0.0.1.7/src/Molara.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Molara
-Version: 0.0.1
+Version: 0.0.1.7
 Summary: A visualisation tool for chemical structures.
 Author: Michel Heinz, Gereon Feldmann
 Author-email: Adrian Usler <adrian.usler@rwth-aachen.de>, Alexander Bonkowski <alexander.bonkowski@rwth-aachen.de>
 Maintainer: Michel Heinz, Gereon Feldmann, Adrian Usler, Alexander Bonkowski
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

