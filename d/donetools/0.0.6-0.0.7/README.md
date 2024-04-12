# Comparing `tmp/donetools-0.0.6.tar.gz` & `tmp/donetools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donetools-0.0.6.tar", last modified: Thu Apr 11 08:57:16 2024, max compression
+gzip compressed data, was "donetools-0.0.7.tar", last modified: Thu Apr 11 12:41:41 2024, max compression
```

## Comparing `donetools-0.0.6.tar` & `donetools-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 08:57:16.352984 donetools-0.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/donetools/
--rw-r--r--   0 root         (0) root         (0)       54 2024-04-08 07:14:03.000000 donetools-0.0.6/donetools/__init__.py
--rw-r--r--   0 root         (0) root         (0)      684 2024-04-10 15:11:13.000000 donetools-0.0.6/donetools/info.py
--rw-r--r--   0 root         (0) root         (0)     2258 2024-04-11 08:56:20.000000 donetools-0.0.6/donetools/path.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 08:57:16.352984 donetools-0.0.6/donetools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      212 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 08:57:16.000000 donetools-0.0.6/donetools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      457 2024-04-11 08:56:40.000000 donetools-0.0.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 08:57:16.352984 donetools-0.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:41:41.171385 donetools-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1068 2024-04-08 07:07:04.000000 donetools-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 12:41:41.171385 donetools-0.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:41:41.171385 donetools-0.0.7/donetools/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-04-11 08:58:54.000000 donetools-0.0.7/donetools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      684 2024-04-10 15:11:13.000000 donetools-0.0.7/donetools/info.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-04-11 12:41:16.000000 donetools-0.0.7/donetools/path.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 12:41:41.171385 donetools-0.0.7/donetools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-11 12:41:41.000000 donetools-0.0.7/donetools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      212 2024-04-11 12:41:41.000000 donetools-0.0.7/donetools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 12:41:41.000000 donetools-0.0.7/donetools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-11 12:41:41.000000 donetools-0.0.7/donetools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-11 12:41:36.000000 donetools-0.0.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 12:41:41.171385 donetools-0.0.7/setup.cfg
```

### Comparing `donetools-0.0.6/LICENSE` & `donetools-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `donetools-0.0.6/donetools/info.py` & `donetools-0.0.7/donetools/info.py`

 * *Files identical despite different names*

### Comparing `donetools-0.0.6/donetools/path.py` & `donetools-0.0.7/donetools/path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import os
 import shutil
 
 from donetools import info
 
+def dir(path: str) -> str:
+    """Ensure the tail separator exists in a directory path."""
+    return path if isDir(path) else path + os.sep
+
 def isDir(path: str) -> bool:
     """Test whether a path is intended to represent a directory."""
     return path.endswith(os.sep)
 
 def isFile(path: str) -> bool:
     """Test whether a path is intended to represent a file."""
     return not path.endswith(os.sep)
 
 def abs(path: str) -> str:
     """Absolutize path without normalizing it."""
     return os.path.join(os.getcwd(), path)
 
 def rel(path: str, start=os.curdir) -> str:
     """Return a relative path from a `start` directory without normalizing the output."""
-    relpath = os.path.relpath(path, start=start)
-    return relpath + os.sep if isDir(path) and isFile(relpath) else relpath
+    return dir(os.path.relpath(path, start)) if isDir(path) else os.path.relpath(path, start)
 
 def existDir(path: str) -> bool:
     """Test whether a path points to an existing directory."""
     return os.path.isdir(path)
 
 def existFile(path: str) -> bool:
     """Test whether a path points to an existing file."""
```

