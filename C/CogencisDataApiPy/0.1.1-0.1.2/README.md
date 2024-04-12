# Comparing `tmp/CogencisDataApiPy-0.1.1.tar.gz` & `tmp/CogencisDataApiPy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CogencisDataApiPy-0.1.1.tar", last modified: Fri Apr 12 13:28:37 2024, max compression
+gzip compressed data, was "CogencisDataApiPy-0.1.2.tar", last modified: Fri Apr 12 13:46:16 2024, max compression
```

## Comparing `CogencisDataApiPy-0.1.1.tar` & `CogencisDataApiPy-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:28:37.876418 CogencisDataApiPy-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:28:37.845165 CogencisDataApiPy-0.1.1/CogencisDataApiPy/
--rw-rw-rw-   0        0        0     2655 2024-04-12 12:58:13.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy/CogencisDataApiPy.py
--rw-rw-rw-   0        0        0       42 2024-04-12 13:21:02.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:28:37.860794 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/
--rw-rw-rw-   0        0        0      570 2024-04-12 13:28:37.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-12 13:28:37.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:28:37.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 13:28:37.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 13:28:37.000000 CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      570 2024-04-12 13:28:37.876418 CogencisDataApiPy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-04-12 04:58:26.000000 CogencisDataApiPy-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 13:28:37.876418 CogencisDataApiPy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-04-12 13:28:18.000000 CogencisDataApiPy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.670655 CogencisDataApiPy-0.1.2/CogencisDataApiPy/
+-rw-rw-rw-   0        0        0     2655 2024-04-12 12:58:13.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy/CogencisDataApiPy.py
+-rw-rw-rw-   0        0        0       49 2024-04-12 13:44:32.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/
+-rw-rw-rw-   0        0        0      570 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      570 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-04-12 04:58:26.000000 CogencisDataApiPy-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-04-12 13:45:49.000000 CogencisDataApiPy-0.1.2/setup.py
```

### Comparing `CogencisDataApiPy-0.1.1/CogencisDataApiPy/CogencisDataApiPy.py` & `CogencisDataApiPy-0.1.2/CogencisDataApiPy/CogencisDataApiPy.py`

 * *Files identical despite different names*

### Comparing `CogencisDataApiPy-0.1.1/CogencisDataApiPy.egg-info/PKG-INFO` & `CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CogencisDataApiPy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `CogencisDataApiPy-0.1.1/PKG-INFO` & `CogencisDataApiPy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CogencisDataApiPy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `CogencisDataApiPy-0.1.1/setup.py` & `CogencisDataApiPy-0.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='CogencisDataApiPy',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     install_requires=['requests', 'pandas'],  # Add any dependencies
     author='Kannan M',
     author_email='kannan.m@cogencis.com',
     description='Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

