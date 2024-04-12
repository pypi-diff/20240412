# Comparing `tmp/firecrawl-py-0.0.2.tar.gz` & `tmp/firecrawl-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.2.tar", last modified: Fri Apr 12 00:59:13 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.3.tar", last modified: Fri Apr 12 01:00:52 2024, max compression
```

## Comparing `firecrawl-py-0.0.2.tar` & `firecrawl-py-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.086758 firecrawl-py-0.0.2/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:59:13.086627 firecrawl-py-0.0.2/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3318 2024-04-12 00:43:37.000000 firecrawl-py-0.0.2/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.085818 firecrawl-py-0.0.2/firecrawl/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       31 2024-04-12 00:47:28.000000 firecrawl-py-0.0.2/firecrawl/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3365 2024-04-12 00:57:26.000000 firecrawl-py-0.0.2/firecrawl/firecrawl.py
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.086431 firecrawl-py-0.0.2/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/top_level.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 00:59:13.086811 firecrawl-py-0.0.2/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 00:57:41.000000 firecrawl-py-0.0.2/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.241577 firecrawl-py-0.0.3/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:00:52.241478 firecrawl-py-0.0.3/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3318 2024-04-12 00:43:37.000000 firecrawl-py-0.0.3/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.240793 firecrawl-py-0.0.3/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       36 2024-04-12 01:00:36.000000 firecrawl-py-0.0.3/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3365 2024-04-12 00:57:26.000000 firecrawl-py-0.0.3/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 01:00:52.241333 firecrawl-py-0.0.3/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 01:00:52.000000 firecrawl-py-0.0.3/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 01:00:52.241618 firecrawl-py-0.0.3/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 01:00:45.000000 firecrawl-py-0.0.3/setup.py
```

### Comparing `firecrawl-py-0.0.2/README.md` & `firecrawl-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `firecrawl-py-0.0.2/firecrawl/firecrawl.py` & `firecrawl-py-0.0.3/firecrawl/firecrawl.py`

 * *Files identical despite different names*

