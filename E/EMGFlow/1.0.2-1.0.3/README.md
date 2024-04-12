# Comparing `tmp/emgflow-1.0.2.tar.gz` & `tmp/emgflow-1.0.3.tar.gz`

## Comparing `emgflow-1.0.2.tar` & `emgflow-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.2/src/EMGFlow/OutlierFinder.py
--rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 emgflow-1.0.2/src/EMGFlow/PlotSignals.py
--rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.2/src/EMGFlow/SignalFilterer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.2/src/EMGFlow/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.2/.gitignore
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 emgflow-1.0.2/README.md
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 emgflow-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 emgflow-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/OutlierFinder.py
+-rw-r--r--   0        0        0     8818 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/PlotSignals.py
+-rw-r--r--   0        0        0    49356 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/SignalFilterer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 emgflow-1.0.3/src/EMGFlow/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 emgflow-1.0.3/.gitignore
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 emgflow-1.0.3/README.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 emgflow-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 emgflow-1.0.3/PKG-INFO
```

### Comparing `emgflow-1.0.2/src/EMGFlow/OutlierFinder.py` & `emgflow-1.0.3/src/EMGFlow/OutlierFinder.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.2/src/EMGFlow/PlotSignals.py` & `emgflow-1.0.3/src/EMGFlow/PlotSignals.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 import re
 import matplotlib.pyplot as plt
 import random
 import webbrowser
 from tqdm import tqdm
 
 from shiny import App, render, ui
-import nest_asyncio
-nest_asyncio.apply()
 
 from SignalFilterer import ConvertMapFiles, MapFilesFuse, EMG2PSD
 
 #
 # =============================================================================
 #
```

### Comparing `emgflow-1.0.2/src/EMGFlow/SignalFilterer.py` & `emgflow-1.0.3/src/EMGFlow/SignalFilterer.py`

 * *Files identical despite different names*

### Comparing `emgflow-1.0.2/README.md` & `emgflow-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,23 +52,30 @@
 ```
 
 Once installed, the package can be loaded as follows:
 ```python
 import EMGFlow
 ```
 
+EMGFlow's functions are divided into 3 different modules, which can be imported with shorthands as follows:
+```python
+import EMGFlow.SignalFilterer as ESIG
+import EMGFlow.OutlierFinder as EOLF
+import EMGFlow.PlotSignals as EPLT
+```
+
 ---
 
 ## Citations
 
 This package can be cited as follows:
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {0.0.1},
+  version = {1.0.3},
   year = {2024}
 }
 ```
```

### Comparing `emgflow-1.0.2/pyproject.toml` & `emgflow-1.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "EMGFlow"
-version = "1.0.2"
+version = "1.0.3"
 dependencies = [
     "pandas",
     "numpy",
     "scipy",
     "matplotlib",
     "opencv-python", 
     "tqdm",
     "webbrowser",
     "shiny",
-    "nest-asyncio"
 ]
 requires-python = ">=3.8"
 authors = [
-    { name="William Conley", email="william@cconley.ca" },
-    { name="Steven Livingstone" },
+    {name = "Steven Livingstone"},
+    {name = "William Conley", email = "william@cconley.ca"}
 ]
 description = "A general EMG processing and feature extraction package."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
-]
+]
+
+[project.urls]
+Home = "https://github.com/WiIIson/EMGFlow-Python-Package"
```

### Comparing `emgflow-1.0.2/PKG-INFO` & `emgflow-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: EMGFlow
-Version: 1.0.2
+Version: 1.0.3
 Summary: A general EMG processing and feature extraction package.
+Project-URL: Home, https://github.com/WiIIson/EMGFlow-Python-Package
 Author: Steven Livingstone
 Author-email: William Conley <william@cconley.ca>
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: matplotlib
-Requires-Dist: nest-asyncio
 Requires-Dist: numpy
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: shiny
 Requires-Dist: tqdm
 Requires-Dist: webbrowser
@@ -73,23 +73,30 @@
 ```
 
 Once installed, the package can be loaded as follows:
 ```python
 import EMGFlow
 ```
 
+EMGFlow's functions are divided into 3 different modules, which can be imported with shorthands as follows:
+```python
+import EMGFlow.SignalFilterer as ESIG
+import EMGFlow.OutlierFinder as EOLF
+import EMGFlow.PlotSignals as EPLT
+```
+
 ---
 
 ## Citations
 
 This package can be cited as follows:
 
 ```bibtex
 @software{Conley_EMGFlow_2024,
   author = {Conley {\tt william@cconley.ca}, William and Livingstone, Steven R},
   month = {03},
   title = {{EMGFlow Package}},
   url = {https://github.com/WiIIson/EMGFlow-Python-Package},
-  version = {0.0.1},
+  version = {1.0.3},
   year = {2024}
 }
 ```
```

