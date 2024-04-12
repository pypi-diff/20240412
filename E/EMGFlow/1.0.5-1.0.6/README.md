# Comparing `tmp/emgflow-1.0.5.tar.gz` & `tmp/emgflow-1.0.6.tar.gz`

## Comparing `emgflow-1.0.5.tar` & `emgflow-1.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.5/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.5/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.5/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.5/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.5/.gitignore
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 emgflow-1.0.5/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 emgflow-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 emgflow-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.6/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.6/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.6/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.6/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.6/.gitignore
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 emgflow-1.0.6/README.md
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 emgflow-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 emgflow-1.0.6/PKG-INFO
```

### Comparing `emgflow-1.0.5/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.6/src/EMGFlow/OutlierFinder.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.5/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.6/src/EMGFlow/PlotSignals.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.5/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.6/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.5/README.md` & `emgflow-1.0.6/README.md`

 * *Files identical despite different names*

```diff
@@ -71,11 +71,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.5},
+  version = {1.0.6},
   year = {2024}
 }
 ```
```

### Comparing `emgflow-1.0.5/pyproject.toml` & `emgflow-1.0.6/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.5"
+version = "1.0.6"
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
-author = "William Conley and Steven Livingstone"
-author_email = "william@cconley.ca"
+authors = [
+    {name = "William Conley and Steven Livingstone", email = "william@cconley.ca"}
+]
 description = "A general EMG processing and feature extraction package."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `emgflow-1.0.5/PKG-INFO` & `emgflow-1.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: EMGFlow
-Version: 1.0.5
+Version: 1.0.6
 Summary: A general EMG processing and feature extraction package.
 Project-URL: Home, https://github.com/WiIIson/EMGFlow-Python-Package
+Author-email: William Conley and Steven Livingstone <william@cconley.ca>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: opencv-python
@@ -90,11 +91,11 @@
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {1.0.5},
+  version = {1.0.6},
   year = {2024}
 }
 ```
```

