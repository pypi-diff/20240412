# Comparing `tmp/scikit-surgerycore-0.7.1.tar.gz` & `tmp/scikit-surgerycore-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-surgerycore-0.7.1.tar", last modified: Wed Feb 21 14:09:54 2024, max compression
+gzip compressed data, was "scikit-surgerycore-0.7.2.tar", last modified: Fri Apr 12 10:47:19 2024, max compression
```

## Comparing `scikit-surgerycore-0.7.1.tar` & `scikit-surgerycore-0.7.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-02-21 14:09:54.000000 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-21 14:09:54.000000 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 14:09:54.000000 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-21 14:09:54.000000 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-21 14:09:54.000000 scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/
--rwxr-xr-x   0 runner    (1001) docker     (127)      113 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/sksurgerycore/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/averagequaternions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/procrustes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/tracking_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/algorithms/vector_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/baseclasses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/baseclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/baseclasses/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/configuration/configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/io/load_mps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/transforms/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/transforms/transform_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.600318 scikit-surgerycore-0.7.1/sksurgerycore/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/utilities/file_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_averagequaternions.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_fre_from_fle.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_procrustes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_tracking_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/algorithms/test_tre_from_fle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:54.604318 scikit-surgerycore-0.7.1/tests/baseclasses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/baseclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/baseclasses/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/tests/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-02-21 14:09:42.000000 scikit-surgerycore-0.7.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-12 10:47:19.000000 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-12 10:47:19.000000 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 10:47:19.000000 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 10:47:19.000000 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 10:47:19.000000 scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.780149 scikit-surgerycore-0.7.2/sksurgerycore/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      113 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 10:47:19.788148 scikit-surgerycore-0.7.2/sksurgerycore/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.780149 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/averagequaternions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/tracking_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/algorithms/vector_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.780149 scikit-surgerycore-0.7.2/sksurgerycore/baseclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/baseclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/baseclasses/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.780149 scikit-surgerycore-0.7.2/sksurgerycore/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/configuration/configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.780149 scikit-surgerycore-0.7.2/sksurgerycore/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/io/load_mps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/sksurgerycore/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/transforms/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/transforms/transform_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/sksurgerycore/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/utilities/file_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_averagequaternions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_fre_from_fle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6127 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_procrustes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_tracking_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/algorithms/test_tre_from_fle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:19.784149 scikit-surgerycore-0.7.2/tests/baseclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/baseclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10779 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/baseclasses/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/tests/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 10:47:12.000000 scikit-surgerycore-0.7.2/versioneer.py
```

### Comparing `scikit-surgerycore-0.7.1/LICENSE` & `scikit-surgerycore-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/PKG-INFO` & `scikit-surgerycore-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgerycore
-Version: 0.7.1
+Version: 0.7.2
 Summary: scikit-surgerycore contains commonly used Image Guided Surgery algorithms and tools
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerycore
 Author: Steve Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Keywords: medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scikit-surgerycore-0.7.1/README.rst` & `scikit-surgerycore-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/PKG-INFO` & `scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgerycore
-Version: 0.7.1
+Version: 0.7.2
 Summary: scikit-surgerycore contains commonly used Image Guided Surgery algorithms and tools
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerycore
 Author: Steve Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Keywords: medical imaging
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `scikit-surgerycore-0.7.1/scikit_surgerycore.egg-info/SOURCES.txt` & `scikit-surgerycore-0.7.2/scikit_surgerycore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/setup.py` & `scikit-surgerycore-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/averagequaternions.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/averagequaternions.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/errors.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/errors.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/pivot.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/pivot.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/procrustes.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/procrustes.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/tracking_smoothing.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/tracking_smoothing.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/algorithms/vector_math.py` & `scikit-surgerycore-0.7.2/sksurgerycore/algorithms/vector_math.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/baseclasses/tracker.py` & `scikit-surgerycore-0.7.2/sksurgerycore/baseclasses/tracker.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/configuration/configuration_manager.py` & `scikit-surgerycore-0.7.2/sksurgerycore/configuration/configuration_manager.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/io/load_mps.py` & `scikit-surgerycore-0.7.2/sksurgerycore/io/load_mps.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/transforms/matrix.py` & `scikit-surgerycore-0.7.2/sksurgerycore/transforms/matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,26 +130,33 @@
     rot_tmp = np.matmul(rot_matrices[0], rot_matrices[1])
     rot_m = np.matmul(rot_tmp, rot_matrices[2])
 
     return rot_m
 
 
 def construct_rigid_transformation(rot_m, trans_v):
-    """Construct a 4x4 rigid-body transformation from a 3x3 rotation matrix and
+    """
+    Construct a 4x4 rigid-body transformation from a 3x3 rotation matrix and
     a 3x1 vector as translation
 
     :param rot_m: 3x3 rotation matrix, numpy array
     :param trans_v: 3x1 vector as translation, numpy array
     :returns: rigid_transformation -- 4x4 rigid transformation matrix,
     numpy array
     """
     rigid_transformation = np.identity(4)
 
     for i in range(3):
         for j in range(3):
             rigid_transformation[i][j] = rot_m[i][j]
 
-    rigid_transformation[0][3] = trans_v[0]
-    rigid_transformation[1][3] = trans_v[1]
-    rigid_transformation[2][3] = trans_v[2]
+    # While the specification is [3x1] which implies ndarray, the users
+    # may also pass in array (3,), ndarray (3, 1) or ndarray (1, 3).
+    # So, this will flatten all of them to the same array-like shape.
+    # In keeping with the rotation matrix, no range checking.
+    t_v = np.ravel(trans_v)
+
+    rigid_transformation[0][3] = t_v[0]
+    rigid_transformation[1][3] = t_v[1]
+    rigid_transformation[2][3] = t_v[2]
 
     return rigid_transformation
```

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/transforms/transform_manager.py` & `scikit-surgerycore-0.7.2/sksurgerycore/transforms/transform_manager.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/utilities/file_utilities.py` & `scikit-surgerycore-0.7.2/sksurgerycore/utilities/file_utilities.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate.py` & `scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate_file.py` & `scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate_file.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/sksurgerycore/utilities/validate_matrix.py` & `scikit-surgerycore-0.7.2/sksurgerycore/utilities/validate_matrix.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/algorithms/test_averagequaternions.py` & `scikit-surgerycore-0.7.2/tests/algorithms/test_averagequaternions.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/algorithms/test_fre_from_fle.py` & `scikit-surgerycore-0.7.2/tests/algorithms/test_fre_from_fle.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/algorithms/test_procrustes.py` & `scikit-surgerycore-0.7.2/tests/algorithms/test_procrustes.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/algorithms/test_tracking_smoothing.py` & `scikit-surgerycore-0.7.2/tests/algorithms/test_tracking_smoothing.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/algorithms/test_tre_from_fle.py` & `scikit-surgerycore-0.7.2/tests/algorithms/test_tre_from_fle.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/baseclasses/test_tracker.py` & `scikit-surgerycore-0.7.2/tests/baseclasses/test_tracker.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/tests/test_requirements.py` & `scikit-surgerycore-0.7.2/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycore-0.7.1/versioneer.py` & `scikit-surgerycore-0.7.2/versioneer.py`

 * *Files identical despite different names*

