# Comparing `tmp/ultra_logger-0.1.tar.gz` & `tmp/ultra_logger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultra_logger-0.1.tar", last modified: Thu Apr 11 16:06:25 2024, max compression
+gzip compressed data, was "ultra_logger-0.1.1.tar", last modified: Thu Apr 11 16:10:58 2024, max compression
```

## Comparing `ultra_logger-0.1.tar` & `ultra_logger-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 16:06:25.917877 ultra_logger-0.1/
--rw-rw-rw-   0        0        0     1462 2024-04-11 16:06:25.917877 ultra_logger-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3904 2024-04-11 13:48:05.000000 ultra_logger-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-11 16:06:25.919265 ultra_logger-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1510 2024-04-11 16:04:37.000000 ultra_logger-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:06:25.899328 ultra_logger-0.1/ultra_logger/
--rw-rw-rw-   0        0        0       28 2024-04-11 15:24:41.000000 ultra_logger-0.1/ultra_logger/__init__.py
--rw-rw-rw-   0        0        0     8077 2024-03-27 15:30:50.000000 ultra_logger-0.1/ultra_logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-11 16:06:25.916865 ultra_logger-0.1/ultra_logger.egg-info/
--rw-rw-rw-   0        0        0     1462 2024-04-11 16:06:25.000000 ultra_logger-0.1/ultra_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-11 16:06:25.000000 ultra_logger-0.1/ultra_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 16:06:25.000000 ultra_logger-0.1/ultra_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      517 2024-04-11 16:06:25.000000 ultra_logger-0.1/ultra_logger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 16:06:25.000000 ultra_logger-0.1/ultra_logger.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/
+-rw-rw-rw-   0        0        0     5306 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3904 2024-04-11 13:48:05.000000 ultra_logger-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-11 16:10:58.961427 ultra_logger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1550 2024-04-11 16:10:47.000000 ultra_logger-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.946976 ultra_logger-0.1.1/ultra_logger/
+-rw-rw-rw-   0        0        0       28 2024-04-11 15:24:41.000000 ultra_logger-0.1.1/ultra_logger/__init__.py
+-rw-rw-rw-   0        0        0     8077 2024-03-27 15:30:50.000000 ultra_logger-0.1.1/ultra_logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-11 16:10:58.960422 ultra_logger-0.1.1/ultra_logger.egg-info/
+-rw-rw-rw-   0        0        0     5306 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 16:10:58.000000 ultra_logger-0.1.1/ultra_logger.egg-info/top_level.txt
```

### Comparing `ultra_logger-0.1/README.md` & `ultra_logger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ultra_logger-0.1/setup.py` & `ultra_logger-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
 
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+    
+    
 setup(
     name='ultra_logger',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     author="Om Sing Chandel",
     author_email="omchandel1703@gmail.com",
-    description="Simplified and easy logger that aids while building projects",
-    long_description="This Python package provides a robust and customizable logger that simplifies the process of recording messages and events in your applications. It leverages the power of the `colorlog` library to enhance readability and debugging capabilities.",
+    description="This Python package provides a robust and customizable logger that simplifies the process of recording messages and events in your applications. It leverages the power of the `colorlog` library to enhance readability and debugging capabilities.",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'certifi==2024.2.2',
         'charset-normalizer==3.3.2',
         'colorama==0.4.6',
         'colorlog==6.8.2',
         'docutils==0.21.1',
```

### Comparing `ultra_logger-0.1/ultra_logger/logger.py` & `ultra_logger-0.1.1/ultra_logger/logger.py`

 * *Files identical despite different names*

### Comparing `ultra_logger-0.1/ultra_logger.egg-info/requires.txt` & `ultra_logger-0.1.1/ultra_logger.egg-info/requires.txt`

 * *Files identical despite different names*

