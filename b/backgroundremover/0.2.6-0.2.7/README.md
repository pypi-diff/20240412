# Comparing `tmp/backgroundremover-0.2.6.tar.gz` & `tmp/backgroundremover-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backgroundremover-0.2.6.tar", last modified: Wed Dec  6 01:02:27 2023, max compression
+gzip compressed data, was "backgroundremover-0.2.7.tar", last modified: Fri Apr 12 18:43:02 2024, max compression
```

## Comparing `backgroundremover-0.2.6.tar` & `backgroundremover-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     6908 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6409 2023-11-12 00:46:28.000000 backgroundremover-0.2.6/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/backgroundremover/
--rw-rw-r--   0 john      (1000) john      (1000)      175 2023-12-06 01:02:04.000000 backgroundremover-0.2.6/backgroundremover/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6964 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/bg.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-07-01 21:34:29.000000 backgroundremover-0.2.6/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)    12566 2023-11-12 00:45:07.000000 backgroundremover-0.2.6/backgroundremover/utilities.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     6908 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      654 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       69 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2023-12-06 01:02:27.000000 backgroundremover-0.2.6/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      230 2023-07-01 21:34:32.000000 backgroundremover-0.2.6/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-07-01 21:34:32.000000 backgroundremover-0.2.6/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2023-12-06 01:02:27.373946 backgroundremover-0.2.6/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-12-06 01:02:04.000000 backgroundremover-0.2.6/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     6908 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6409 2023-11-12 00:46:28.000000 backgroundremover-0.2.7/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.911448 backgroundremover-0.2.7/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      175 2024-04-12 18:41:21.000000 backgroundremover-0.2.7/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7172 2023-12-06 01:26:54.000000 backgroundremover-0.2.7/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.915448 backgroundremover-0.2.7/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-07-01 21:34:29.000000 backgroundremover-0.2.7/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12566 2023-11-12 00:45:07.000000 backgroundremover-0.2.7/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-12 18:43:02.915448 backgroundremover-0.2.7/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     6908 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      654 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       69 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      358 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2024-04-12 18:43:02.000000 backgroundremover-0.2.7/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2023-07-01 21:34:32.000000 backgroundremover-0.2.7/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      358 2024-03-03 17:23:59.000000 backgroundremover-0.2.7/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2024-04-12 18:43:02.919448 backgroundremover-0.2.7/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1027 2024-04-12 18:41:32.000000 backgroundremover-0.2.7/setup.py
```

### Comparing `backgroundremover-0.2.6/LICENSE.txt` & `backgroundremover-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/PKG-INFO` & `backgroundremover-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.6
+Version: 0.2.7
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 Keywords: remove,background,u2net,remove background,background remover
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `backgroundremover-0.2.6/README.md` & `backgroundremover-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/bg.py` & `backgroundremover-0.2.7/backgroundremover/bg.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,24 @@
 import torch.nn.functional
 import torch.nn.functional
 from hsh.library.hash import Hasher
 from .u2net import detect, u2net
 from . import utilities
 
 # closes https://github.com/nadermx/backgroundremover/issues/18
-if torch.cuda.is_available():
-    DEVICE = torch.device('cuda:0')
-elif torch.backends.mps.is_available():
-    DEVICE = torch.device('mps')
-else:
+# closes https://github.com/nadermx/backgroundremover/issues/112
+try:
+    if torch.cuda.is_available():
+        DEVICE = torch.device('cuda:0')
+    elif torch.backends.mps.is_available():
+        DEVICE = torch.device('mps')
+    else:
+        DEVICE = torch.device('cpu')
+except Exception as e:
+    print(f"Using CPU.  Setting Cuda or MPS failed: {e}")
     DEVICE = torch.device('cpu')
 
 class Net(torch.nn.Module):
     def __init__(self, model_name):
         super(Net, self).__init__()
         hasher = Hasher()
         model = {
```

### Comparing `backgroundremover-0.2.6/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.7/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/cmd/server.py` & `backgroundremover-0.2.7/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.7/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.7/backgroundremover/u2net/detect.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.7/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover/utilities.py` & `backgroundremover-0.2.7/backgroundremover/utilities.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.7/backgroundremover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.6
+Version: 0.2.7
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 Keywords: remove,background,u2net,remove background,background remover
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `backgroundremover-0.2.6/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.7/backgroundremover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.6/setup.py` & `backgroundremover-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.6",
+    version="0.2.7",
     description="Background remover from image and video using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
```

