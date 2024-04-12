# Comparing `tmp/PyStorAI-0.2.5.tar.gz` & `tmp/PyStorAI-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyStorAI-0.2.5.tar", last modified: Fri Jan 19 21:10:58 2024, max compression
+gzip compressed data, was "PyStorAI-0.2.6.tar", last modified: Fri Apr 12 18:57:03 2024, max compression
```

## Comparing `PyStorAI-0.2.5.tar` & `PyStorAI-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 21:10:58.294494 PyStorAI-0.2.5/
--rw-r--r--   0 root         (0) root         (0)      687 2024-01-19 21:10:58.293494 PyStorAI-0.2.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 21:10:58.291494 PyStorAI-0.2.5/PyStorAI/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-19 21:10:32.000000 PyStorAI-0.2.5/PyStorAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9268 2024-01-19 21:10:28.000000 PyStorAI-0.2.5/PyStorAI/storyboard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-19 21:10:58.293494 PyStorAI-0.2.5/PyStorAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)      687 2024-01-19 21:10:58.000000 PyStorAI-0.2.5/PyStorAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      180 2024-01-19 21:10:58.000000 PyStorAI-0.2.5/PyStorAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-19 21:10:58.000000 PyStorAI-0.2.5/PyStorAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-19 21:10:58.000000 PyStorAI-0.2.5/PyStorAI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-19 21:10:58.294494 PyStorAI-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      933 2024-01-19 21:09:21.000000 PyStorAI-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.813655 PyStorAI-0.2.6/PyStorAI/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 18:54:20.000000 PyStorAI-0.2.6/PyStorAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6103 2024-04-12 18:54:59.000000 PyStorAI-0.2.6/PyStorAI/storyboard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:57:03.814655 PyStorAI-0.2.6/PyStorAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      687 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 18:57:03.000000 PyStorAI-0.2.6/PyStorAI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 18:57:03.815655 PyStorAI-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-12 18:53:55.000000 PyStorAI-0.2.6/setup.py
```

### Comparing `PyStorAI-0.2.5/PKG-INFO` & `PyStorAI-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.5
+Version: 0.2.6
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Your Name
 Author-email: your@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.5/PyStorAI.egg-info/PKG-INFO` & `PyStorAI-0.2.6/PyStorAI.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStorAI
-Version: 0.2.5
+Version: 0.2.6
 Summary: Effective Storyboard Visualisations for Artificial Intelligence.
 Home-page: https://github.com/VisualXAI/PyStorAI
 Author: Your Name
 Author-email: your@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PyStorAI-0.2.5/setup.py` & `PyStorAI-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyStorAI',
-    version='0.2.5',
+    version='0.2.6',
     packages=find_packages(),
     install_requires=[
         # List your dependencies here
     ],
     include_package_data=True,
     author='Your Name',
     author_email='your@email.com',
```

