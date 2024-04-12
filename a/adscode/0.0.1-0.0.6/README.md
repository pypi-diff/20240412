# Comparing `tmp/adscode-0.0.1.tar.gz` & `tmp/adscode-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adscode-0.0.1.tar", last modified: Fri Apr 12 18:21:49 2024, max compression
+gzip compressed data, was "dist\adscode-0.0.6.tar", last modified: Fri Apr 12 17:47:59 2024, max compression
```

## Comparing `adscode-0.0.1.tar` & `adscode-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:21:49.769721 adscode-0.0.1/
--rw-rw-rw-   0        0        0      488 2024-04-12 18:21:49.768149 adscode-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 18:21:49.725299 adscode-0.0.1/adscode/
--rw-rw-rw-   0        0        0       45 2024-04-12 17:45:38.000000 adscode-0.0.1/adscode/__init__.py
--rw-rw-rw-   0        0        0     3069 2024-04-12 17:45:16.000000 adscode-0.0.1/adscode/descriptive.py
--rw-rw-rw-   0        0        0     2874 2024-04-12 17:55:53.000000 adscode-0.0.1/adscode/imputation.py
--rw-rw-rw-   0        0        0     1981 2024-04-12 18:18:08.000000 adscode-0.0.1/adscode/outlier.py
--rw-rw-rw-   0        0        0    11221 2024-04-12 18:16:06.000000 adscode-0.0.1/adscode/performance.py
--rw-rw-rw-   0        0        0     1620 2024-04-10 15:22:10.000000 adscode-0.0.1/adscode/smote.py
--rw-rw-rw-   0        0        0     1560 2024-04-12 18:21:28.000000 adscode-0.0.1/adscode/timeseries.py
--rw-rw-rw-   0        0        0       84 2024-04-12 18:01:44.000000 adscode-0.0.1/adscode/url.py
--rw-rw-rw-   0        0        0     3952 2024-04-12 18:02:53.000000 adscode-0.0.1/adscode/visualization.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:21:49.765153 adscode-0.0.1/adscode.egg-info/
--rw-rw-rw-   0        0        0      488 2024-04-12 18:21:49.000000 adscode-0.0.1/adscode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2024-04-12 18:21:49.000000 adscode-0.0.1/adscode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:21:49.000000 adscode-0.0.1/adscode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 18:21:49.000000 adscode-0.0.1/adscode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 18:21:49.771247 adscode-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      614 2024-04-12 18:21:44.000000 adscode-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:47:59.346964 adscode-0.0.6/
+-rw-rw-rw-   0        0        0      488 2024-04-12 17:47:59.343964 adscode-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 17:47:59.265986 adscode-0.0.6/adscode/
+-rw-rw-rw-   0        0        0       45 2024-04-12 17:45:38.000000 adscode-0.0.6/adscode/__init__.py
+-rw-rw-rw-   0        0        0     3069 2024-04-12 17:45:16.000000 adscode-0.0.6/adscode/descriptive.py
+-rw-rw-rw-   0        0        0     1620 2024-04-10 15:22:10.000000 adscode-0.0.6/adscode/smote.py
+drwxrwxrwx   0        0        0        0 2024-04-12 17:47:59.337913 adscode-0.0.6/adscode.egg-info/
+-rw-rw-rw-   0        0        0      488 2024-04-12 17:47:58.000000 adscode-0.0.6/adscode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-12 17:47:59.000000 adscode-0.0.6/adscode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 17:47:58.000000 adscode-0.0.6/adscode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 17:47:58.000000 adscode-0.0.6/adscode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 17:47:59.347981 adscode-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-04-10 15:16:47.000000 adscode-0.0.6/setup.py
```

### Comparing `adscode-0.0.1/adscode/descriptive.py` & `adscode-0.0.6/adscode/descriptive.py`

 * *Files identical despite different names*

### Comparing `adscode-0.0.1/adscode/smote.py` & `adscode-0.0.6/adscode/smote.py`

 * *Files identical despite different names*

### Comparing `adscode-0.0.1/setup.py` & `adscode-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.1'
+VERSION = '0.0.6'
 DESCRIPTION = 'basic hello pkg'
 
 # Setting up
 setup(
     name="adscode",
     version=VERSION,
     author="Mathew Patil",
```

