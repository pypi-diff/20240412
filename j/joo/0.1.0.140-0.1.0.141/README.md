# Comparing `tmp/joo-0.1.0.140.tar.gz` & `tmp/joo-0.1.0.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joo-0.1.0.140.tar", last modified: Fri Apr 12 07:24:29 2024, max compression
+gzip compressed data, was "joo-0.1.0.141.tar", last modified: Fri Apr 12 07:27:10 2024, max compression
```

## Comparing `joo-0.1.0.140.tar` & `joo-0.1.0.141.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.048524 joo-0.1.0.140/
--rw-rw-rw-   0        0        0      625 2024-04-12 07:24:29.045528 joo-0.1.0.140/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-12 07:24:25.000000 joo-0.1.0.140/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:28.948236 joo-0.1.0.140/lib/
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:28.985097 joo-0.1.0.140/lib/joo/
--rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.140/lib/joo/LICENSE
--rw-rw-rw-   0        0        0     6197 2024-04-12 05:15:52.000000 joo-0.1.0.140/lib/joo/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-12 07:24:25.000000 joo-0.1.0.140/lib/joo/__version__.py
--rw-rw-rw-   0        0        0     2780 2024-04-12 03:38:16.000000 joo-0.1.0.140/lib/joo/cli.py
--rw-rw-rw-   0        0        0    12338 2024-04-11 09:21:46.000000 joo-0.1.0.140/lib/joo/datetimeutil.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.042107 joo-0.1.0.140/lib/joo/dc/
--rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.140/lib/joo/dc/__init__.py
--rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.140/lib/joo/dc/http.py
--rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.140/lib/joo/dc/selenium.py
--rw-rw-rw-   0        0        0     5119 2024-04-12 05:42:04.000000 joo-0.1.0.140/lib/joo/httpapi.py
--rw-rw-rw-   0        0        0    11864 2024-04-12 04:32:41.000000 joo-0.1.0.140/lib/joo/logging.py
--rw-rw-rw-   0        0        0    15809 2024-04-12 05:34:00.000000 joo-0.1.0.140/lib/joo/sysutil.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.031591 joo-0.1.0.140/lib/joo.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 07:24:29.048524 joo-0.1.0.140/setup.cfg
--rw-rw-rw-   0        0        0     1424 2024-04-12 07:24:25.000000 joo-0.1.0.140/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:27:10.482814 joo-0.1.0.141/
+-rw-rw-rw-   0        0        0      625 2024-04-12 07:27:10.480816 joo-0.1.0.141/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-12 07:27:06.000000 joo-0.1.0.141/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 07:27:10.376004 joo-0.1.0.141/lib/
+drwxrwxrwx   0        0        0        0 2024-04-12 07:27:10.440070 joo-0.1.0.141/lib/joo/
+-rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.141/lib/joo/LICENSE
+-rw-rw-rw-   0        0        0     6197 2024-04-12 05:15:52.000000 joo-0.1.0.141/lib/joo/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-12 07:27:06.000000 joo-0.1.0.141/lib/joo/__version__.py
+-rw-rw-rw-   0        0        0     2780 2024-04-12 03:38:16.000000 joo-0.1.0.141/lib/joo/cli.py
+-rw-rw-rw-   0        0        0    12338 2024-04-11 09:21:46.000000 joo-0.1.0.141/lib/joo/datetimeutil.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:27:10.476826 joo-0.1.0.141/lib/joo/dc/
+-rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.141/lib/joo/dc/__init__.py
+-rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.141/lib/joo/dc/http.py
+-rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.141/lib/joo/dc/selenium.py
+-rw-rw-rw-   0        0        0     5119 2024-04-12 05:42:04.000000 joo-0.1.0.141/lib/joo/httpapi.py
+-rw-rw-rw-   0        0        0    11864 2024-04-12 04:32:41.000000 joo-0.1.0.141/lib/joo/logging.py
+-rw-rw-rw-   0        0        0    15809 2024-04-12 05:34:00.000000 joo-0.1.0.141/lib/joo/sysutil.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:27:10.464099 joo-0.1.0.141/lib/joo.egg-info/
+-rw-rw-rw-   0        0        0      625 2024-04-12 07:27:08.000000 joo-0.1.0.141/lib/joo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-04-12 07:27:09.000000 joo-0.1.0.141/lib/joo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:27:08.000000 joo-0.1.0.141/lib/joo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-12 07:27:08.000000 joo-0.1.0.141/lib/joo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:27:10.483812 joo-0.1.0.141/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2024-04-12 07:27:06.000000 joo-0.1.0.141/setup.py
```

### Comparing `joo-0.1.0.140/PKG-INFO` & `joo-0.1.0.141/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.140
+Version: 0.1.0.141
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.140/lib/joo/LICENSE` & `joo-0.1.0.141/lib/joo/LICENSE`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/__init__.py` & `joo-0.1.0.141/lib/joo/__init__.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/__version__.py` & `joo-0.1.0.141/lib/joo/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 __VERSION__ = {
     "name": "joo",
     "description": "joo library",
     "version": "0.1.0",
-    "build": 140,
+    "build": 141,
     "license": "MIT License",
     "author": "Wooloo Studio",
     "author_email": "max.wu@wooloostudio.com",
     "url": "https://github.com/metatutu/joo",
     "project_urls": {
         "Documentation": "https://github.com/metatutu/joo",
         "Source Code": "https://github.com/metatutu/joo",
```

### Comparing `joo-0.1.0.140/lib/joo/cli.py` & `joo-0.1.0.141/lib/joo/cli.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/datetimeutil.py` & `joo-0.1.0.141/lib/joo/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/dc/__init__.py` & `joo-0.1.0.141/lib/joo/dc/__init__.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/dc/http.py` & `joo-0.1.0.141/lib/joo/dc/http.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/dc/selenium.py` & `joo-0.1.0.141/lib/joo/dc/selenium.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/httpapi.py` & `joo-0.1.0.141/lib/joo/httpapi.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/logging.py` & `joo-0.1.0.141/lib/joo/logging.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo/sysutil.py` & `joo-0.1.0.141/lib/joo/sysutil.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.140/lib/joo.egg-info/PKG-INFO` & `joo-0.1.0.141/lib/joo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.140
+Version: 0.1.0.141
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.140/setup.py` & `joo-0.1.0.141/setup.py`

 * *Files identical despite different names*

