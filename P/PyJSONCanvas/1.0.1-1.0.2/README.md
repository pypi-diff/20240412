# Comparing `tmp/PyJSONCanvas-1.0.1.tar.gz` & `tmp/PyJSONCanvas-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyJSONCanvas-1.0.1.tar", last modified: Thu Mar 21 02:27:16 2024, max compression
+gzip compressed data, was "PyJSONCanvas-1.0.2.tar", last modified: Fri Apr 12 20:51:01 2024, max compression
```

## Comparing `PyJSONCanvas-1.0.1.tar` & `PyJSONCanvas-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-03-21 02:27:16.200963 PyJSONCanvas-1.0.1/
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2686 2024-03-21 02:27:16.200774 PyJSONCanvas-1.0.1/PKG-INFO
-drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-03-21 02:27:16.200588 PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2686 2024-03-21 02:27:16.000000 PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/PKG-INFO
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)      306 2024-03-21 02:27:16.000000 PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/SOURCES.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)        1 2024-03-21 02:27:16.000000 PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/dependency_links.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)       13 2024-03-21 02:27:16.000000 PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/top_level.txt
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2393 2024-03-21 02:15:12.000000 PyJSONCanvas-1.0.1/README.md
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)       38 2024-03-21 02:27:16.201011 PyJSONCanvas-1.0.1/setup.cfg
--rw-r--r--   0 chaitanyasharma   (501) staff       (20)      444 2024-03-21 02:27:04.000000 PyJSONCanvas-1.0.1/setup.py
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-12 20:51:01.904314 PyJSONCanvas-1.0.2/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2686 2024-04-12 20:51:01.904071 PyJSONCanvas-1.0.2/PKG-INFO
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-12 20:51:01.903812 PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2686 2024-04-12 20:51:01.000000 PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/PKG-INFO
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)      479 2024-04-12 20:51:01.000000 PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/SOURCES.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)        1 2024-04-12 20:51:01.000000 PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/dependency_links.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)       13 2024-04-12 20:51:01.000000 PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/top_level.txt
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2393 2024-03-21 02:15:12.000000 PyJSONCanvas-1.0.2/README.md
+drwxr-xr-x   0 chaitanyasharma   (501) staff       (20)        0 2024-04-12 20:51:01.902501 PyJSONCanvas-1.0.2/pyjsoncanvas/
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)      663 2024-03-20 23:46:20.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/__init__.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     1190 2024-03-21 01:47:58.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/encoder.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     2530 2024-03-20 23:37:57.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/exceptions.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     5942 2024-03-21 00:45:32.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/jsoncanvas.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     5766 2024-03-28 17:04:46.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/models.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)        0 2024-03-20 22:48:46.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/utils.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)     4448 2024-03-21 00:11:24.000000 PyJSONCanvas-1.0.2/pyjsoncanvas/validate.py
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)       38 2024-04-12 20:51:01.904378 PyJSONCanvas-1.0.2/setup.cfg
+-rw-r--r--   0 chaitanyasharma   (501) staff       (20)      442 2024-04-12 20:50:54.000000 PyJSONCanvas-1.0.2/setup.py
```

### Comparing `PyJSONCanvas-1.0.1/PKG-INFO` & `PyJSONCanvas-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJSONCanvas
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple library for working with JSON Canvas (previously known as Obsidian Canvas) files.
 Home-page: https://github.com/CheeksTheGeek/PyJSONCanvas
 Author: Chaitanya Sharma
 License: MIT
 Description-Content-Type: text/markdown
 
 # PyJSONCanvas
```

### Comparing `PyJSONCanvas-1.0.1/PyJSONCanvas.egg-info/PKG-INFO` & `PyJSONCanvas-1.0.2/PyJSONCanvas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJSONCanvas
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple library for working with JSON Canvas (previously known as Obsidian Canvas) files.
 Home-page: https://github.com/CheeksTheGeek/PyJSONCanvas
 Author: Chaitanya Sharma
 License: MIT
 Description-Content-Type: text/markdown
 
 # PyJSONCanvas
```

### Comparing `PyJSONCanvas-1.0.1/README.md` & `PyJSONCanvas-1.0.2/README.md`

 * *Files identical despite different names*

