# Comparing `tmp/variable_polyline_buffer-0.1.4.tar.gz` & `tmp/variable_polyline_buffer-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "variable_polyline_buffer-0.1.4.tar", last modified: Fri Apr 12 15:03:04 2024, max compression
+gzip compressed data, was "variable_polyline_buffer-0.1.5.tar", last modified: Fri Apr 12 15:04:13 2024, max compression
```

## Comparing `variable_polyline_buffer-0.1.4.tar` & `variable_polyline_buffer-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:03:04.761951 variable_polyline_buffer-0.1.4/
--rw-r--r--   0 stephan    (501) staff       (20)     1069 2024-04-12 14:13:03.000000 variable_polyline_buffer-0.1.4/LICENSE
--rw-r--r--   0 stephan    (501) staff       (20)     2264 2024-04-12 15:03:04.761721 variable_polyline_buffer-0.1.4/PKG-INFO
--rw-r--r--   0 stephan    (501) staff       (20)     1869 2024-04-12 14:55:37.000000 variable_polyline_buffer-0.1.4/README.md
--rw-r--r--   0 stephan    (501) staff       (20)       38 2024-04-12 15:03:04.761989 variable_polyline_buffer-0.1.4/setup.cfg
--rw-r--r--   0 stephan    (501) staff       (20)      592 2024-04-12 15:03:00.000000 variable_polyline_buffer-0.1.4/setup.py
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:03:04.760224 variable_polyline_buffer-0.1.4/src/
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:03:04.760851 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer/
--rw-r--r--   0 stephan    (501) staff       (20)       53 2024-04-12 13:54:44.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer/__init__.py
--rw-r--r--   0 stephan    (501) staff       (20)     3935 2024-04-12 13:52:24.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer/polyline_buffer.py
-drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:03:04.761559 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/
--rw-r--r--   0 stephan    (501) staff       (20)     2264 2024-04-12 15:03:04.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/PKG-INFO
--rw-r--r--   0 stephan    (501) staff       (20)      374 2024-04-12 15:03:04.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/SOURCES.txt
--rw-r--r--   0 stephan    (501) staff       (20)        1 2024-04-12 15:03:04.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/dependency_links.txt
--rw-r--r--   0 stephan    (501) staff       (20)        6 2024-04-12 15:03:04.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/requires.txt
--rw-r--r--   0 stephan    (501) staff       (20)       25 2024-04-12 15:03:04.000000 variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/top_level.txt
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:04:13.364326 variable_polyline_buffer-0.1.5/
+-rw-r--r--   0 stephan    (501) staff       (20)     1069 2024-04-12 14:13:03.000000 variable_polyline_buffer-0.1.5/LICENSE
+-rw-r--r--   0 stephan    (501) staff       (20)     2264 2024-04-12 15:04:13.364054 variable_polyline_buffer-0.1.5/PKG-INFO
+-rw-r--r--   0 stephan    (501) staff       (20)     1869 2024-04-12 14:55:37.000000 variable_polyline_buffer-0.1.5/README.md
+-rw-r--r--   0 stephan    (501) staff       (20)       38 2024-04-12 15:04:13.364364 variable_polyline_buffer-0.1.5/setup.cfg
+-rw-r--r--   0 stephan    (501) staff       (20)      592 2024-04-12 15:03:52.000000 variable_polyline_buffer-0.1.5/setup.py
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:04:13.362401 variable_polyline_buffer-0.1.5/src/
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:04:13.363055 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer/
+-rw-r--r--   0 stephan    (501) staff       (20)       54 2024-04-12 15:03:48.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer/__init__.py
+-rw-r--r--   0 stephan    (501) staff       (20)     3935 2024-04-12 13:52:24.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer/polyline_buffer.py
+drwxr-xr-x   0 stephan    (501) staff       (20)        0 2024-04-12 15:04:13.363804 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/
+-rw-r--r--   0 stephan    (501) staff       (20)     2264 2024-04-12 15:04:13.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/PKG-INFO
+-rw-r--r--   0 stephan    (501) staff       (20)      374 2024-04-12 15:04:13.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/SOURCES.txt
+-rw-r--r--   0 stephan    (501) staff       (20)        1 2024-04-12 15:04:13.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/dependency_links.txt
+-rw-r--r--   0 stephan    (501) staff       (20)        6 2024-04-12 15:04:13.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/requires.txt
+-rw-r--r--   0 stephan    (501) staff       (20)       25 2024-04-12 15:04:13.000000 variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/top_level.txt
```

### Comparing `variable_polyline_buffer-0.1.4/LICENSE` & `variable_polyline_buffer-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `variable_polyline_buffer-0.1.4/PKG-INFO` & `variable_polyline_buffer-0.1.5/src/variable_polyline_buffer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: variable_polyline_buffer
-Version: 0.1.4
+Name: variable-polyline-buffer
+Version: 0.1.5
 Summary: A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.
 Home-page: https://github.com/stephtr/variable-polyline-buffer
 Author: Stephan Troyer
 Author-email: stephantroyer@live.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `variable_polyline_buffer-0.1.4/README.md` & `variable_polyline_buffer-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `variable_polyline_buffer-0.1.4/setup.py` & `variable_polyline_buffer-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="variable_polyline_buffer",
-    version="0.1.4",
+    version="0.1.5",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     description="A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Stephan Troyer",
     author_email="stephantroyer@live.at",
```

### Comparing `variable_polyline_buffer-0.1.4/src/variable_polyline_buffer/polyline_buffer.py` & `variable_polyline_buffer-0.1.5/src/variable_polyline_buffer/polyline_buffer.py`

 * *Files identical despite different names*

### Comparing `variable_polyline_buffer-0.1.4/src/variable_polyline_buffer.egg-info/PKG-INFO` & `variable_polyline_buffer-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: variable-polyline-buffer
-Version: 0.1.4
+Name: variable_polyline_buffer
+Version: 0.1.5
 Summary: A function for calculating a buffer around a polyline, defining the contours of a line with variable thickness.
 Home-page: https://github.com/stephtr/variable-polyline-buffer
 Author: Stephan Troyer
 Author-email: stephantroyer@live.at
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

