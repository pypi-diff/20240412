# Comparing `tmp/SAMMEC2-0.0.4.tar.gz` & `tmp/SAMMEC2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMMEC2-0.0.4.tar", last modified: Thu Apr 11 14:36:26 2024, max compression
+gzip compressed data, was "SAMMEC2-0.0.5.tar", last modified: Fri Apr 12 10:49:10 2024, max compression
```

## Comparing `SAMMEC2-0.0.4.tar` & `SAMMEC2-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.463595 SAMMEC2-0.0.4/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:36:26.463145 SAMMEC2-0.0.4/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.4/README
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.458122 SAMMEC2-0.0.4/SAMMEC2/
--rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.4/SAMMEC2/SAMMEC2.py
--rw-r--r--   0 bso2     (1724916894) 285334988       22 2024-04-11 14:36:10.000000 SAMMEC2-0.0.4/SAMMEC2/__init__.py
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-11 14:36:26.462775 SAMMEC2-0.0.4/SAMMEC2.egg-info/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988      178 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/SOURCES.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/dependency_links.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-11 14:36:26.000000 SAMMEC2-0.0.4/SAMMEC2.egg-info/top_level.txt
--rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-11 14:36:26.463679 SAMMEC2-0.0.4/setup.cfg
--rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-11 14:36:10.000000 SAMMEC2-0.0.4/setup.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-12 10:49:10.159307 SAMMEC2-0.0.5/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-12 10:49:10.158517 SAMMEC2-0.0.5/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.5/README
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-12 10:49:10.154439 SAMMEC2-0.0.5/SAMMEC2/
+-rw-r--r--   0 bso2     (1724916894) 285334988     5981 2024-04-12 10:44:38.000000 SAMMEC2-0.0.5/SAMMEC2/GA.py
+-rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.5/SAMMEC2/SAMMEC2.py
+-rw-r--r--   0 bso2     (1724916894) 285334988       40 2024-04-12 10:44:38.000000 SAMMEC2-0.0.5/SAMMEC2/__init__.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-12 10:49:10.157718 SAMMEC2-0.0.5/SAMMEC2.egg-info/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-12 10:49:09.000000 SAMMEC2-0.0.5/SAMMEC2.egg-info/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988      192 2024-04-12 10:49:09.000000 SAMMEC2-0.0.5/SAMMEC2.egg-info/SOURCES.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-12 10:49:09.000000 SAMMEC2-0.0.5/SAMMEC2.egg-info/dependency_links.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-12 10:49:09.000000 SAMMEC2-0.0.5/SAMMEC2.egg-info/top_level.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-12 10:49:10.159468 SAMMEC2-0.0.5/setup.cfg
+-rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-12 10:48:43.000000 SAMMEC2-0.0.5/setup.py
```

### Comparing `SAMMEC2-0.0.4/SAMMEC2/SAMMEC2.py` & `SAMMEC2-0.0.5/SAMMEC2/SAMMEC2.py`

 * *Files identical despite different names*

### Comparing `SAMMEC2-0.0.4/setup.py` & `SAMMEC2-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SAMMEC2", # Replace with your own PyPI username(id)
-    version="0.0.4",
+    version="0.0.5",
     author="Banghee So",
     author_email="bso@towson.edu",
     description="SAMMEC2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bheeso/SAMME.C2",
     packages=setuptools.find_packages(),
```

