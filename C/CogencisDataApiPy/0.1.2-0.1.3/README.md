# Comparing `tmp/CogencisDataApiPy-0.1.2.tar.gz` & `tmp/CogencisDataApiPy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CogencisDataApiPy-0.1.2.tar", last modified: Fri Apr 12 13:46:16 2024, max compression
+gzip compressed data, was "CogencisDataApiPy-0.1.3.tar", last modified: Fri Apr 12 13:56:43 2024, max compression
```

## Comparing `CogencisDataApiPy-0.1.2.tar` & `CogencisDataApiPy-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.670655 CogencisDataApiPy-0.1.2/CogencisDataApiPy/
--rw-rw-rw-   0        0        0     2655 2024-04-12 12:58:13.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy/CogencisDataApiPy.py
--rw-rw-rw-   0        0        0       49 2024-04-12 13:44:32.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/
--rw-rw-rw-   0        0        0      570 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 13:46:16.000000 CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      570 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      121 2024-04-12 04:58:26.000000 CogencisDataApiPy-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 13:46:16.698307 CogencisDataApiPy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      632 2024-04-12 13:45:49.000000 CogencisDataApiPy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:56:43.065450 CogencisDataApiPy-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-12 13:56:43.055938 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/
+-rw-rw-rw-   0        0        0      570 2024-04-12 13:56:42.000000 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-12 13:56:42.000000 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:56:42.000000 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 13:56:42.000000 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:56:42.000000 CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      570 2024-04-12 13:56:43.065450 CogencisDataApiPy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      121 2024-04-12 04:58:26.000000 CogencisDataApiPy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:56:43.065450 CogencisDataApiPy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      632 2024-04-12 13:56:24.000000 CogencisDataApiPy-0.1.3/setup.py
```

### Comparing `CogencisDataApiPy-0.1.2/CogencisDataApiPy.egg-info/PKG-INFO` & `CogencisDataApiPy-0.1.3/CogencisDataApiPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CogencisDataApiPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `CogencisDataApiPy-0.1.2/PKG-INFO` & `CogencisDataApiPy-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CogencisDataApiPy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple interface to quickly to consume the Cogencis Data API in python environment. This package provides several functions for accessing historical market data and reference data
 Home-page: https://cogencis.com
 Author: Kannan M
 Author-email: kannan.m@cogencis.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

