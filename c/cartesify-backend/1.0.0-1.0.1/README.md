# Comparing `tmp/cartesify_backend-1.0.0.tar.gz` & `tmp/cartesify_backend-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartesify_backend-1.0.0.tar", last modified: Wed Apr 10 22:02:54 2024, max compression
+gzip compressed data, was "cartesify_backend-1.0.1.tar", last modified: Fri Apr 12 14:29:27 2024, max compression
```

## Comparing `cartesify_backend-1.0.0.tar` & `cartesify_backend-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-10 22:02:54.083948 cartesify_backend-1.0.0/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1081 2024-03-26 23:02:44.000000 cartesify_backend-1.0.0/LICENSE
--rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-04-10 22:02:54.083948 cartesify_backend-1.0.0/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)       19 2024-03-26 23:03:22.000000 cartesify_backend-1.0.0/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-10 22:02:54.079948 cartesify_backend-1.0.0/cartesify_backend/
--rw-rw-r--   0 diego     (1000) diego     (1000)     1876 2024-04-10 22:02:18.000000 cartesify_backend-1.0.0/cartesify_backend/App.py
--rw-rw-r--   0 diego     (1000) diego     (1000)       97 2024-03-31 20:29:13.000000 cartesify_backend-1.0.0/cartesify_backend/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     1898 2024-04-10 22:02:18.000000 cartesify_backend-1.0.0/cartesify_backend/appfactory.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     5585 2024-04-10 22:00:56.000000 cartesify_backend-1.0.0/cartesify_backend/cartesifybackend.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-10 22:02:54.079948 cartesify_backend-1.0.0/cartesify_backend.egg-info/
--rw-rw-r--   0 diego     (1000) diego     (1000)      281 2024-04-10 22:02:53.000000 cartesify_backend-1.0.0/cartesify_backend.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      355 2024-04-10 22:02:53.000000 cartesify_backend-1.0.0/cartesify_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-10 22:02:53.000000 cartesify_backend-1.0.0/cartesify_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       15 2024-04-10 22:02:53.000000 cartesify_backend-1.0.0/cartesify_backend.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       18 2024-04-10 22:02:53.000000 cartesify_backend-1.0.0/cartesify_backend.egg-info/top_level.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-10 22:02:54.083948 cartesify_backend-1.0.0/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      477 2024-04-10 22:02:46.000000 cartesify_backend-1.0.0/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-12 14:29:27.974148 cartesify_backend-1.0.1/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1081 2024-03-26 23:02:44.000000 cartesify_backend-1.0.1/LICENSE
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1768 2024-04-12 14:29:27.974148 cartesify_backend-1.0.1/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1506 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/README.md
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-12 14:29:27.970148 cartesify_backend-1.0.1/cartesify_backend/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1876 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/cartesify_backend/App.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)       97 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/cartesify_backend/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1898 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/cartesify_backend/appfactory.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     5585 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/cartesify_backend/cartesifybackend.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-04-12 14:29:27.974148 cartesify_backend-1.0.1/cartesify_backend.egg-info/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1768 2024-04-12 14:29:27.000000 cartesify_backend-1.0.1/cartesify_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      355 2024-04-12 14:29:27.000000 cartesify_backend-1.0.1/cartesify_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-04-12 14:29:27.000000 cartesify_backend-1.0.1/cartesify_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       15 2024-04-12 14:29:27.000000 cartesify_backend-1.0.1/cartesify_backend.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       18 2024-04-12 14:29:27.000000 cartesify_backend-1.0.1/cartesify_backend.egg-info/top_level.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-04-12 14:29:27.974148 cartesify_backend-1.0.1/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      477 2024-04-12 14:28:38.000000 cartesify_backend-1.0.1/setup.py
```

### Comparing `cartesify_backend-1.0.0/LICENSE` & `cartesify_backend-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cartesify_backend-1.0.0/cartesify_backend/App.py` & `cartesify_backend-1.0.1/cartesify_backend/App.py`

 * *Files identical despite different names*

### Comparing `cartesify_backend-1.0.0/cartesify_backend/appfactory.py` & `cartesify_backend-1.0.1/cartesify_backend/appfactory.py`

 * *Files identical despite different names*

### Comparing `cartesify_backend-1.0.0/cartesify_backend/cartesifybackend.py` & `cartesify_backend-1.0.1/cartesify_backend/cartesifybackend.py`

 * *Files identical despite different names*

