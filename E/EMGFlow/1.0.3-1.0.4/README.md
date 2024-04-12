# Comparing `tmp/emgflow-1.0.3.tar.gz` & `tmp/emgflow-1.0.4.tar.gz`

## Comparing `emgflow-1.0.3.tar` & `emgflow-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.3/.gitignore
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 emgflow-1.0.3/README.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 emgflow-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 emgflow-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.4/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.4/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.4/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.4/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.4/.gitignore
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 emgflow-1.0.4/README.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 emgflow-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 emgflow-1.0.4/PKG-INFO
```

### Comparing `emgflow-1.0.3/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.4/src/EMGFlow/OutlierFinder.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.3/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.4/src/EMGFlow/PlotSignals.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.3/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.4/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.3/README.md` & `emgflow-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,11 +71,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.3},
+  version = {1.0.4},
   year = {2024}
 }
 ```
```

### Comparing `emgflow-1.0.3/pyproject.toml` & `emgflow-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.3"
+version = "1.0.4"
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "matplotlib",
     "opencv-python", 
     "tqdm",
     "webbrowser",
     "shiny",
 ]
 requires-python = ">=3.8"
 authors = [
-    {name = "Steven Livingstone"},
-    {name = "William Conley", email = "william@cconley.ca"}
+    {name = "William Conley", email = "william@cconley.ca"},
+    {name = "Steven Livingstone"}
 ]
 description = "A general EMG processing and feature extraction package."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
```

### Comparing `emgflow-1.0.3/PKG-INFO` & `emgflow-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: EMGFlow
-Version: 1.0.3
+Version: 1.0.4
 Summary: A general EMG processing and feature extraction package.
 Project-URL: Home, https://github.com/WiIIson/EMGFlow-Python-Package
 Author: Steven Livingstone
 Author-email: William Conley <william@cconley.ca>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -92,11 +92,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.3},
+  version = {1.0.4},
   year = {2024}
 }
 ```
```

