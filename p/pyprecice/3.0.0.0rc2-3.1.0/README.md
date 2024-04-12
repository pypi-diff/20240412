# Comparing `tmp/pyprecice-3.0.0.0rc2.tar.gz` & `tmp/pyprecice-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprecice-3.0.0.0rc2.tar", last modified: Mon Feb  5 12:17:12 2024, max compression
+gzip compressed data, was "pyprecice-3.1.0.tar", last modified: Fri Apr 12 14:12:17 2024, max compression
```

## Comparing `pyprecice-3.0.0.0rc2.tar` & `pyprecice-3.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:17:12.198701 pyprecice-3.0.0.0rc2/cyprecice/
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/cyprecice/Participant.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/cyprecice/cyprecice.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    39060 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/cyprecice/cyprecice.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:17:12.198701 pyprecice-3.0.0.0rc2/precice/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/precice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/precice/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/pyprecice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14326 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 12:17:12.000000 pyprecice-3.0.0.0rc2/pyprecice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 12:17:12.202701 pyprecice-3.0.0.0rc2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    27245 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/test/test_bindings_module.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-02-05 12:16:57.000000 pyprecice-3.0.0.0rc2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.870955 pyprecice-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-12 14:12:05.000000 pyprecice-3.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 14:12:05.000000 pyprecice-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 14:12:05.000000 pyprecice-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-04-12 14:12:17.870955 pyprecice-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-04-12 14:12:05.000000 pyprecice-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.870955 pyprecice-3.1.0/cyprecice/
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-12 14:12:05.000000 pyprecice-3.1.0/cyprecice/Participant.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-12 14:12:05.000000 pyprecice-3.1.0/cyprecice/cyprecice.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    39060 2024-04-12 14:12:05.000000 pyprecice-3.1.0/cyprecice/cyprecice.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.870955 pyprecice-3.1.0/precice/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-12 14:12:05.000000 pyprecice-3.1.0/precice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 14:12:17.870955 pyprecice-3.1.0/precice/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.870955 pyprecice-3.1.0/pyprecice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 14:12:17.000000 pyprecice-3.1.0/pyprecice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 14:12:05.000000 pyprecice-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 14:12:17.870955 pyprecice-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5920 2024-04-12 14:12:05.000000 pyprecice-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.870955 pyprecice-3.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    27245 2024-04-12 14:12:05.000000 pyprecice-3.1.0/test/test_bindings_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 14:12:05.000000 pyprecice-3.1.0/versioneer.py
```

### Comparing `pyprecice-3.0.0.0rc2/CHANGELOG.md` & `pyprecice-3.1.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog of Python language bindings for preCICE
 
 All notable changes to this project will be documented in this file.
 
-## 3.0.0.0rc2
+## v3.1.0
+
+* Change versioning scheme https://github.com/precice/python-bindings/pull/199
+
+## 3.0.0.0
 
 * Add Cython as build time dependency https://github.com/precice/python-bindings/pull/177
 * Update CMake configuration flags for preCICE source installation in Actions. https://github.com/precice/python-bindings/commit/23a840144c2647d6cf09c0ed87be3b768a22feb7
 * Remove API functions `has_mesh` and `has_data` and rename `get_mesh_vertices_and_ids` to `get_mesh_vertices_and_coordinates`. https://github.com/precice/python-bindings/commit/cd446d2807b841d81a4cf5c9dd6656ab43c278c3
 * Update API according to preCICE v3.0.0 https://github.com/precice/python-bindings/pull/179
 
 ## 2.5.0.4
```

### Comparing `pyprecice-3.0.0.0rc2/LICENSE.txt` & `pyprecice-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/PKG-INFO` & `pyprecice-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprecice
-Version: 3.0.0.0rc2
+Version: 3.1.0
 Summary: Python language bindings for the preCICE coupling library
 Home-page: https://github.com/precice/python-bindings
 Author: the preCICE developers
 Author-email: info@precice.org
 License: LGPL-3.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # Python language bindings for the C++ library preCICE
 
 ⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
-This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
+This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first two digits of the version number of the bindings indicate the major and minor version of the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v3.1.0` and `v3.1.1` of the bindings represent versions `0` and `1` of the bindings that are compatible with preCICE `v3.1.x`. Note that this versioning scheme was introduced from bindings `v3.1.0`, which is different than the [old versioning scheme](#old-versioning-scheme).
 
 ## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
 ## Required dependencies
 
@@ -330,14 +330,18 @@
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
+## Old versioning scheme
+
+Bindings versions up to `v3.0.0.0` have four digits, where the first three digits are the supported preCICE version, and the fourth digit is the bindings version. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`. We dropped the third digit of the preCICE version as bugfix releases are always compatible and do not impact the bindings. The new three digit format is now consistent with other preCICE bindings.
+
 ## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
```

### Comparing `pyprecice-3.0.0.0rc2/README.md` & `pyprecice-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python language bindings for the C++ library preCICE
 
 ⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
-This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
+This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first two digits of the version number of the bindings indicate the major and minor version of the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v3.1.0` and `v3.1.1` of the bindings represent versions `0` and `1` of the bindings that are compatible with preCICE `v3.1.x`. Note that this versioning scheme was introduced from bindings `v3.1.0`, which is different than the [old versioning scheme](#old-versioning-scheme).
 
 ## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
 ## Required dependencies
 
@@ -315,14 +315,18 @@
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
+## Old versioning scheme
+
+Bindings versions up to `v3.0.0.0` have four digits, where the first three digits are the supported preCICE version, and the fourth digit is the bindings version. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`. We dropped the third digit of the preCICE version as bugfix releases are always compatible and do not impact the bindings. The new three digit format is now consistent with other preCICE bindings.
+
 ## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
```

### Comparing `pyprecice-3.0.0.0rc2/cyprecice/Participant.pxd` & `pyprecice-3.1.0/cyprecice/Participant.pxd`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/cyprecice/cyprecice.pxd` & `pyprecice-3.1.0/cyprecice/cyprecice.pxd`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/cyprecice/cyprecice.pyx` & `pyprecice-3.1.0/cyprecice/cyprecice.pyx`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/pyprecice.egg-info/PKG-INFO` & `pyprecice-3.1.0/pyprecice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprecice
-Version: 3.0.0.0rc2
+Version: 3.1.0
 Summary: Python language bindings for the preCICE coupling library
 Home-page: https://github.com/precice/python-bindings
 Author: the preCICE developers
 Author-email: info@precice.org
 License: LGPL-3.0
 Requires-Python: >=3
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # Python language bindings for the C++ library preCICE
 
 ⚠️ The latest version of the documentation for the python bindings can be found on [precice.org](https://precice.org/installation-bindings-python.html). The information from this `README` is currently under revision and will be moved ⚠️
 
 [![Upload Python Package](https://github.com/precice/python-bindings/workflows/Upload%20Python%20Package/badge.svg?branch=master)](https://pypi.org/project/pyprecice/)
 
-This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first three digits of the version number of the bindings indicate the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`.
+This package provides python language bindings for the C++ library [preCICE](https://github.com/precice/precice). Note that the first two digits of the version number of the bindings indicate the major and minor version of the preCICE version that the bindings support. The last digit represents the version of the bindings. Example: `v3.1.0` and `v3.1.1` of the bindings represent versions `0` and `1` of the bindings that are compatible with preCICE `v3.1.x`. Note that this versioning scheme was introduced from bindings `v3.1.0`, which is different than the [old versioning scheme](#old-versioning-scheme).
 
 ## User documentation
 
 Please refer to [the preCICE documentation](https://www.precice.org/installation-bindings-python.html) for information on how to install and use the python bindings. Information below is intended for advanced users and developers.
 
 ## Required dependencies
 
@@ -330,14 +330,18 @@
 
 make sure that you are using an up-to-date version of NumPy. You can update NumPy with
 
 ```bash
 pip3 install numpy --upgrade
 ```
 
+## Old versioning scheme
+
+Bindings versions up to `v3.0.0.0` have four digits, where the first three digits are the supported preCICE version, and the fourth digit is the bindings version. Example: `v2.0.0.1` and `v2.0.0.2` of the bindings represent versions `1` and `2` of the bindings that are compatible with preCICE `v2.0.0`. We dropped the third digit of the preCICE version as bugfix releases are always compatible and do not impact the bindings. The new three digit format is now consistent with other preCICE bindings.
+
 ## Contributors
 
 * [Benjamin Rodenberg](https://github.com/BenjaminRodenberg)
 * [Ishaan Desai](https://github.com/IshaanDesai)
 * [Saumitra Vinay Joshi](https://github.com/saumiJ) contributed first working prototype in [`3db9c9` on `precice/precice`](https://github.com/precice/precice/commit/3db9c95e527db1e1cacb2fd116a5ce13ee877513)
 * [Frédéric Simonis](https://github.com/fsimonis)
 * [Florian Lindner](https://github.com/floli)
```

### Comparing `pyprecice-3.0.0.0rc2/setup.py` & `pyprecice-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/test/test_bindings_module.py` & `pyprecice-3.1.0/test/test_bindings_module.py`

 * *Files identical despite different names*

### Comparing `pyprecice-3.0.0.0rc2/versioneer.py` & `pyprecice-3.1.0/versioneer.py`

 * *Files identical despite different names*

