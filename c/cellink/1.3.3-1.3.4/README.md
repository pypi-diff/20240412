# Comparing `tmp/cellink-1.3.3.tar.gz` & `tmp/cellink-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellink-1.3.3.tar", last modified: Thu Nov 30 03:15:48 2023, max compression
+gzip compressed data, was "cellink-1.3.4.tar", last modified: Fri Apr 12 04:39:20 2024, max compression
```

## Comparing `cellink-1.3.3.tar` & `cellink-1.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2023-11-30 03:15:48.238165 cellink-1.3.3/
--rw-rw-r--   0 zhai      (1000) zhai      (1000)      329 2023-11-30 03:15:48.238165 cellink-1.3.3/PKG-INFO
-drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2023-11-30 03:15:48.238165 cellink-1.3.3/cellink/
--rw-rw-r--   0 zhai      (1000) zhai      (1000)       18 2023-10-23 02:28:37.000000 cellink-1.3.3/cellink/__init__.py
-drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2023-11-30 03:15:48.238165 cellink-1.3.3/cellink/lib/
--rw-rw-r--   0 zhai      (1000) zhai      (1000)      372 2023-11-27 01:47:14.000000 cellink-1.3.3/cellink/lib/__init__.py
--rw-rw-r--   0 zhai      (1000) zhai      (1000)     1048 2023-10-23 02:28:37.000000 cellink-1.3.3/cellink/lib/graph.py
--rw-rw-r--   0 zhai      (1000) zhai      (1000)    22612 2023-11-27 09:33:04.000000 cellink-1.3.3/cellink/lib/node.py
--rw-rw-r--   0 zhai      (1000) zhai      (1000)     2882 2023-10-23 02:28:37.000000 cellink-1.3.3/cellink/lib/registry.py
-drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2023-11-30 03:15:48.238165 cellink-1.3.3/cellink.egg-info/
--rw-rw-r--   0 zhai      (1000) zhai      (1000)      329 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/PKG-INFO
--rw-rw-r--   0 zhai      (1000) zhai      (1000)      311 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/SOURCES.txt
--rw-rw-r--   0 zhai      (1000) zhai      (1000)        1 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/dependency_links.txt
--rw-rw-r--   0 zhai      (1000) zhai      (1000)        1 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/not-zip-safe
--rw-rw-r--   0 zhai      (1000) zhai      (1000)        9 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/requires.txt
--rw-rw-r--   0 zhai      (1000) zhai      (1000)        8 2023-11-30 03:15:48.000000 cellink-1.3.3/cellink.egg-info/top_level.txt
--rw-rw-r--   0 zhai      (1000) zhai      (1000)       38 2023-11-30 03:15:48.238165 cellink-1.3.3/setup.cfg
--rw-rw-r--   0 zhai      (1000) zhai      (1000)     1217 2023-11-30 03:15:46.000000 cellink-1.3.3/setup.py
+drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2024-04-12 04:39:20.315137 cellink-1.3.4/
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)      329 2024-04-12 04:39:20.315137 cellink-1.3.4/PKG-INFO
+drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2024-04-12 04:39:20.315137 cellink-1.3.4/cellink/
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)       18 2023-10-23 02:28:37.000000 cellink-1.3.4/cellink/__init__.py
+drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2024-04-12 04:39:20.315137 cellink-1.3.4/cellink/lib/
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)      372 2023-11-27 01:47:14.000000 cellink-1.3.4/cellink/lib/__init__.py
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)     1048 2023-10-23 02:28:37.000000 cellink-1.3.4/cellink/lib/graph.py
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)    22773 2024-04-12 04:33:19.000000 cellink-1.3.4/cellink/lib/node.py
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)     2882 2023-10-23 02:28:37.000000 cellink-1.3.4/cellink/lib/registry.py
+drwxrwxr-x   0 zhai      (1000) zhai      (1000)        0 2024-04-12 04:39:20.315137 cellink-1.3.4/cellink.egg-info/
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)      329 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/PKG-INFO
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)      311 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)        1 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)        1 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/not-zip-safe
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)        9 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/requires.txt
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)        8 2024-04-12 04:39:20.000000 cellink-1.3.4/cellink.egg-info/top_level.txt
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)       38 2024-04-12 04:39:20.315137 cellink-1.3.4/setup.cfg
+-rw-rw-r--   0 zhai      (1000) zhai      (1000)     1217 2024-04-12 04:38:48.000000 cellink-1.3.4/setup.py
```

### Comparing `cellink-1.3.3/cellink/lib/graph.py` & `cellink-1.3.4/cellink/lib/graph.py`

 * *Files identical despite different names*

### Comparing `cellink-1.3.3/cellink/lib/node.py` & `cellink-1.3.4/cellink/lib/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,17 +310,19 @@
         if target_node and str(source_node) == str(target_node):
             return source_node
 
         # keep scanning upwards
         elif source_node._run_backward():
             reached_node = None
             for parent in source_node._parents:
-                source_node = self._backward_from_node(parent, target_node)
-                if source_node:
-                    reached_node = source_node
+                # backward is executed only if the node is executed and successful
+                if parent._forward_state == ForwardState.success:
+                    source_node = self._backward_from_node(parent, target_node)
+                    if source_node:
+                        reached_node = source_node
             return reached_node
         return None
 
     def retr(self, node_name:str=None):
         """
         reach node in a bottom-up manner by executing series of backward() methods
```

### Comparing `cellink-1.3.3/cellink/lib/registry.py` & `cellink-1.3.4/cellink/lib/registry.py`

 * *Files identical despite different names*

### Comparing `cellink-1.3.3/setup.py` & `cellink-1.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from setuptools import setup
 from numpy.distutils.core import setup
 from numpy.distutils.misc_util import Configuration
 from os.path import join
 
-str_version = '1.3.3'
+str_version = '1.3.4'
 
 def configuration(parent_package='', top_path=''):
     # this will automatically build the scattering extensions, using the
     # setup.py files located in their subdirectories
     config = Configuration(None, parent_package, top_path)
 
     pkglist = setuptools.find_packages()
```

