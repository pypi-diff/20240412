# Comparing `tmp/mewtools-0.1.8.tar.gz` & `tmp/mewtools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mewtools-0.1.8.tar", last modified: Fri Mar 15 11:01:00 2024, max compression
+gzip compressed data, was "mewtools-0.1.9.tar", last modified: Fri Apr 12 13:23:12 2024, max compression
```

## Comparing `mewtools-0.1.8.tar` & `mewtools-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-03-15 11:01:00.346418 mewtools-0.1.8/
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1060 2024-03-15 08:08:57.000000 mewtools-0.1.8/LICENSE
--rw-r--r--   0 sensei.qm   (501) staff       (20)       26 2024-03-15 08:08:57.000000 mewtools-0.1.8/MANIFEST.in
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1490 2024-03-15 11:01:00.346196 mewtools-0.1.8/PKG-INFO
--rw-r--r--   0 sensei.qm   (501) staff       (20)      167 2024-03-15 09:21:36.000000 mewtools-0.1.8/README.md
-drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-03-15 11:01:00.341659 mewtools-0.1.8/mewtools/
--rw-r--r--   0 sensei.qm   (501) staff       (20)       51 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/__init__.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)      352 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/__version__.py
-drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-03-15 11:01:00.344227 mewtools-0.1.8/mewtools/mydatetime/
--rw-r--r--   0 sensei.qm   (501) staff       (20)     2940 2024-03-15 10:01:30.000000 mewtools-0.1.8/mewtools/mydatetime/__init__.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     5673 2024-03-15 10:01:28.000000 mewtools-0.1.8/mewtools/mydatetime/core.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     4182 2024-03-15 10:01:45.000000 mewtools-0.1.8/mewtools/mydatetime/extract_.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     9304 2024-03-15 10:01:45.000000 mewtools-0.1.8/mewtools/mydatetime/extract_prep.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)      366 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/mydatetime/month_pair.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     5013 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/mydatetime/timezone.py
-drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-03-15 11:01:00.345527 mewtools-0.1.8/mewtools/wordpress/
--rw-r--r--   0 sensei.qm   (501) staff       (20)        0 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/wordpress/__init__.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1145 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/wordpress/category.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1973 2024-03-15 10:01:45.000000 mewtools-0.1.8/mewtools/wordpress/core.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)      538 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/wordpress/custom.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     3430 2024-03-15 08:08:57.000000 mewtools-0.1.8/mewtools/wordpress/files.py
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1779 2024-03-15 10:01:45.000000 mewtools-0.1.8/mewtools/wordpress/posts.py
-drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-03-15 11:01:00.345885 mewtools-0.1.8/mewtools.egg-info/
--rw-r--r--   0 sensei.qm   (501) staff       (20)     1490 2024-03-15 11:01:00.000000 mewtools-0.1.8/mewtools.egg-info/PKG-INFO
--rw-r--r--   0 sensei.qm   (501) staff       (20)      610 2024-03-15 11:01:00.000000 mewtools-0.1.8/mewtools.egg-info/SOURCES.txt
--rw-r--r--   0 sensei.qm   (501) staff       (20)        1 2024-03-15 11:01:00.000000 mewtools-0.1.8/mewtools.egg-info/dependency_links.txt
--rw-r--r--   0 sensei.qm   (501) staff       (20)      482 2024-03-15 11:01:00.000000 mewtools-0.1.8/mewtools.egg-info/requires.txt
--rw-r--r--   0 sensei.qm   (501) staff       (20)        9 2024-03-15 11:01:00.000000 mewtools-0.1.8/mewtools.egg-info/top_level.txt
--rw-r--r--   0 sensei.qm   (501) staff       (20)       38 2024-03-15 11:01:00.346457 mewtools-0.1.8/setup.cfg
--rw-r--r--   0 sensei.qm   (501) staff       (20)     4116 2024-03-15 11:00:55.000000 mewtools-0.1.8/setup.py
+drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-04-12 13:23:12.655151 mewtools-0.1.9/
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     1060 2024-03-15 08:08:57.000000 mewtools-0.1.9/LICENSE
+-rw-r--r--   0 sensei.qm   (501) staff       (20)       26 2024-03-15 08:08:57.000000 mewtools-0.1.9/MANIFEST.in
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      588 2024-04-12 13:23:12.654985 mewtools-0.1.9/PKG-INFO
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      167 2024-03-15 09:21:36.000000 mewtools-0.1.9/README.md
+drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-04-12 13:23:12.650158 mewtools-0.1.9/mewtools/
+-rw-r--r--   0 sensei.qm   (501) staff       (20)       51 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/__init__.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      352 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/__version__.py
+drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-04-12 13:23:12.652732 mewtools-0.1.9/mewtools/mydatetime/
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     2940 2024-03-15 10:01:30.000000 mewtools-0.1.9/mewtools/mydatetime/__init__.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     5673 2024-03-15 10:01:28.000000 mewtools-0.1.9/mewtools/mydatetime/core.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     4182 2024-03-15 10:01:45.000000 mewtools-0.1.9/mewtools/mydatetime/extract_.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     9304 2024-03-15 10:01:45.000000 mewtools-0.1.9/mewtools/mydatetime/extract_prep.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      366 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/mydatetime/month_pair.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     5013 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/mydatetime/timezone.py
+drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-04-12 13:23:12.654618 mewtools-0.1.9/mewtools/wordpress/
+-rw-r--r--   0 sensei.qm   (501) staff       (20)        0 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/wordpress/__init__.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     1145 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/wordpress/category.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     1973 2024-03-15 10:01:45.000000 mewtools-0.1.9/mewtools/wordpress/core.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      538 2024-03-15 08:08:57.000000 mewtools-0.1.9/mewtools/wordpress/custom.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     3333 2024-04-12 13:11:13.000000 mewtools-0.1.9/mewtools/wordpress/files.py
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     1779 2024-03-15 10:01:45.000000 mewtools-0.1.9/mewtools/wordpress/posts.py
+drwxr-xr-x   0 sensei.qm   (501) staff       (20)        0 2024-04-12 13:23:12.651209 mewtools-0.1.9/mewtools.egg-info/
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      588 2024-04-12 13:23:12.000000 mewtools-0.1.9/mewtools.egg-info/PKG-INFO
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      610 2024-04-12 13:23:12.000000 mewtools-0.1.9/mewtools.egg-info/SOURCES.txt
+-rw-r--r--   0 sensei.qm   (501) staff       (20)        1 2024-04-12 13:23:12.000000 mewtools-0.1.9/mewtools.egg-info/dependency_links.txt
+-rw-r--r--   0 sensei.qm   (501) staff       (20)      482 2024-04-12 13:23:12.000000 mewtools-0.1.9/mewtools.egg-info/requires.txt
+-rw-r--r--   0 sensei.qm   (501) staff       (20)        9 2024-04-12 13:23:12.000000 mewtools-0.1.9/mewtools.egg-info/top_level.txt
+-rw-r--r--   0 sensei.qm   (501) staff       (20)       38 2024-04-12 13:23:12.655193 mewtools-0.1.9/setup.cfg
+-rw-r--r--   0 sensei.qm   (501) staff       (20)     4116 2024-04-12 13:11:45.000000 mewtools-0.1.9/setup.py
```

### Comparing `mewtools-0.1.8/LICENSE` & `mewtools-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/mydatetime/__init__.py` & `mewtools-0.1.9/mewtools/mydatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/mydatetime/core.py` & `mewtools-0.1.9/mewtools/mydatetime/core.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/mydatetime/extract_.py` & `mewtools-0.1.9/mewtools/mydatetime/extract_.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/mydatetime/extract_prep.py` & `mewtools-0.1.9/mewtools/mydatetime/extract_prep.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/mydatetime/timezone.py` & `mewtools-0.1.9/mewtools/mydatetime/timezone.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/wordpress/category.py` & `mewtools-0.1.9/mewtools/wordpress/category.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/wordpress/core.py` & `mewtools-0.1.9/mewtools/wordpress/core.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/wordpress/custom.py` & `mewtools-0.1.9/mewtools/wordpress/custom.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools/wordpress/posts.py` & `mewtools-0.1.9/mewtools/wordpress/posts.py`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/mewtools.egg-info/SOURCES.txt` & `mewtools-0.1.9/mewtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mewtools-0.1.8/setup.py` & `mewtools-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Package meta-data.
 NAME = "mewtools"
 DESCRIPTION = "My python library package with some scraper tool and data tool"
 URL = "https://github.com/sizzlingbun/mewtools"
 EMAIL = "me@example.com"
 AUTHOR = "Andrew"
 REQUIRES_PYTHON = ">=3.10.0"
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "addict==2.4.0",
     "carehttp>=0.3.11",
     "certifi==2022.5.18.1",
     "charset-normalizer==2.0.12",
```

