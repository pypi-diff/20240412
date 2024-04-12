# Comparing `tmp/g2papi-1.0.1.tar.gz` & `tmp/g2papi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2papi-1.0.1.tar", last modified: Fri Apr 12 21:46:00 2024, max compression
+gzip compressed data, was "g2papi-1.0.2.tar", last modified: Fri Apr 12 21:48:02 2024, max compression
```

## Comparing `g2papi-1.0.1.tar` & `g2papi-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:46:00.465747 g2papi-1.0.1/
--rw-r--r--   0 jsafer     (503) staff       (20)     1072 2024-04-12 21:04:13.000000 g2papi-1.0.1/LICENSE
--rw-r--r--   0 jsafer     (503) staff       (20)      248 2024-04-12 21:46:00.465126 g2papi-1.0.1/PKG-INFO
--rw-r--r--   0 jsafer     (503) staff       (20)     3910 2024-04-12 21:04:13.000000 g2papi-1.0.1/README.md
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:46:00.460401 g2papi-1.0.1/g2papi/
--rw-r--r--   0 jsafer     (503) staff       (20)       85 2024-03-28 16:40:25.000000 g2papi-1.0.1/g2papi/__init__.py
--rw-r--r--   0 jsafer     (503) staff       (20)      844 2024-03-28 18:16:13.000000 g2papi-1.0.1/g2papi/api.py
--rw-r--r--   0 jsafer     (503) staff       (20)     1340 2024-03-28 18:00:11.000000 g2papi-1.0.1/g2papi/cli.py
-drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:46:00.464137 g2papi-1.0.1/g2papi.egg-info/
--rw-r--r--   0 jsafer     (503) staff       (20)      248 2024-04-12 21:45:59.000000 g2papi-1.0.1/g2papi.egg-info/PKG-INFO
--rw-r--r--   0 jsafer     (503) staff       (20)      255 2024-04-12 21:46:00.000000 g2papi-1.0.1/g2papi.egg-info/SOURCES.txt
--rw-r--r--   0 jsafer     (503) staff       (20)        1 2024-04-12 21:45:59.000000 g2papi-1.0.1/g2papi.egg-info/dependency_links.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       43 2024-04-12 21:46:00.000000 g2papi-1.0.1/g2papi.egg-info/entry_points.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       16 2024-04-12 21:46:00.000000 g2papi-1.0.1/g2papi.egg-info/requires.txt
--rw-r--r--   0 jsafer     (503) staff       (20)        7 2024-04-12 21:46:00.000000 g2papi-1.0.1/g2papi.egg-info/top_level.txt
--rw-r--r--   0 jsafer     (503) staff       (20)       38 2024-04-12 21:46:00.465965 g2papi-1.0.1/setup.cfg
--rw-r--r--   0 jsafer     (503) staff       (20)      575 2024-04-12 21:44:30.000000 g2papi-1.0.1/setup.py
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.166732 g2papi-1.0.2/
+-rw-r--r--   0 jsafer     (503) staff       (20)     1072 2024-04-12 21:04:13.000000 g2papi-1.0.2/LICENSE
+-rw-r--r--   0 jsafer     (503) staff       (20)     4191 2024-04-12 21:48:02.165767 g2papi-1.0.2/PKG-INFO
+-rw-r--r--   0 jsafer     (503) staff       (20)     3910 2024-04-12 21:04:13.000000 g2papi-1.0.2/README.md
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.158943 g2papi-1.0.2/g2papi/
+-rw-r--r--   0 jsafer     (503) staff       (20)       85 2024-03-28 16:40:25.000000 g2papi-1.0.2/g2papi/__init__.py
+-rw-r--r--   0 jsafer     (503) staff       (20)      844 2024-03-28 18:16:13.000000 g2papi-1.0.2/g2papi/api.py
+-rw-r--r--   0 jsafer     (503) staff       (20)     1340 2024-03-28 18:00:11.000000 g2papi-1.0.2/g2papi/cli.py
+drwxr-xr-x   0 jsafer     (503) staff       (20)        0 2024-04-12 21:48:02.164802 g2papi-1.0.2/g2papi.egg-info/
+-rw-r--r--   0 jsafer     (503) staff       (20)     4191 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/PKG-INFO
+-rw-r--r--   0 jsafer     (503) staff       (20)      255 2024-04-12 21:48:02.000000 g2papi-1.0.2/g2papi.egg-info/SOURCES.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)        1 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/dependency_links.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       43 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/entry_points.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       16 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/requires.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)        7 2024-04-12 21:48:01.000000 g2papi-1.0.2/g2papi.egg-info/top_level.txt
+-rw-r--r--   0 jsafer     (503) staff       (20)       38 2024-04-12 21:48:02.167212 g2papi-1.0.2/setup.cfg
+-rw-r--r--   0 jsafer     (503) staff       (20)      625 2024-04-12 21:47:47.000000 g2papi-1.0.2/setup.py
```

### Comparing `g2papi-1.0.1/LICENSE` & `g2papi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.1/README.md` & `g2papi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.1/g2papi/api.py` & `g2papi-1.0.2/g2papi/api.py`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.1/g2papi/cli.py` & `g2papi-1.0.2/g2papi/cli.py`

 * *Files identical despite different names*

### Comparing `g2papi-1.0.1/setup.py` & `g2papi-1.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='g2papi',
-    version='1.0.1',
+    version='1.0.2',
     author='Jordan Safer',
     author_email='genomics2proteins@gmail.com',
     description='A python client and CLI for easy access to G2P portal APIs',
-    #long_description=long_description,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas'
     ],
     entry_points={
         'console_scripts': [
```

