# Comparing `tmp/aptll-2.2.5.tar.gz` & `tmp/aptll-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aptll-2.2.5.tar", last modified: Sat Mar 23 11:15:05 2024, max compression
+gzip compressed data, was "aptll-2.2.6.tar", last modified: Fri Apr 12 14:04:56 2024, max compression
```

## Comparing `aptll-2.2.5.tar` & `aptll-2.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:15:05.719619 aptll-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-23 11:14:55.000000 aptll-2.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-23 11:15:05.719619 aptll-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-23 11:14:55.000000 aptll-2.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:15:05.719619 aptll-2.2.5/apt/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-23 11:14:55.000000 aptll-2.2.5/apt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-23 11:14:55.000000 aptll-2.2.5/apt/aptll.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 11:15:05.719619 aptll-2.2.5/aptll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-23 11:15:05.000000 aptll-2.2.5/aptll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-23 11:15:05.000000 aptll-2.2.5/aptll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 11:15:05.000000 aptll-2.2.5/aptll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-23 11:15:05.000000 aptll-2.2.5/aptll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-23 11:15:05.000000 aptll-2.2.5/aptll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-23 11:14:55.000000 aptll-2.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 11:15:05.719619 aptll-2.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:56.119173 aptll-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 14:04:48.000000 aptll-2.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-12 14:04:56.119173 aptll-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-12 14:04:48.000000 aptll-2.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:56.115173 aptll-2.2.6/apt/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 14:04:48.000000 aptll-2.2.6/apt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-12 14:04:48.000000 aptll-2.2.6/apt/aptll.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:56.115173 aptll-2.2.6/aptll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-12 14:04:56.000000 aptll-2.2.6/aptll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 14:04:56.000000 aptll-2.2.6/aptll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:04:56.000000 aptll-2.2.6/aptll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 14:04:56.000000 aptll-2.2.6/aptll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 14:04:56.000000 aptll-2.2.6/aptll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-12 14:04:48.000000 aptll-2.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:04:56.119173 aptll-2.2.6/setup.cfg
```

### Comparing `aptll-2.2.5/LICENSE` & `aptll-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aptll-2.2.5/apt/aptll.py` & `aptll-2.2.6/apt/aptll.py`

 * *Files identical despite different names*

### Comparing `aptll-2.2.5/pyproject.toml` & `aptll-2.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["apt"]
 
 [project]
 name = "aptll"
-version = "2.2.5"
+version = "2.2.6"
 dependencies = [
   "aplustools", 
 ]
 requires-python = ">=3.9"
 authors = [
   {name = "Cariel Becker", email = "cariel.becker@gmx.de"},
 ]
```

