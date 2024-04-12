# Comparing `tmp/firecrawl-py-0.0.1.tar.gz` & `tmp/firecrawl-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firecrawl-py-0.0.1.tar", last modified: Fri Apr 12 00:53:19 2024, max compression
+gzip compressed data, was "firecrawl-py-0.0.2.tar", last modified: Fri Apr 12 00:59:13 2024, max compression
```

## Comparing `firecrawl-py-0.0.1.tar` & `firecrawl-py-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:53:19.371695 firecrawl-py-0.0.1/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:53:19.371582 firecrawl-py-0.0.1/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3318 2024-04-12 00:43:37.000000 firecrawl-py-0.0.1/README.md
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:53:19.371144 firecrawl-py-0.0.1/firecrawl_py.egg-info/
--rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:53:19.000000 firecrawl-py-0.0.1/firecrawl_py.egg-info/PKG-INFO
--rw-r--r--   0 nicolascamara   (501) staff       (20)      240 2024-04-12 00:53:19.000000 firecrawl-py-0.0.1/firecrawl_py.egg-info/SOURCES.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 00:53:19.000000 firecrawl-py-0.0.1/firecrawl_py.egg-info/dependency_links.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 00:53:19.000000 firecrawl-py-0.0.1/firecrawl_py.egg-info/requires.txt
--rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 00:53:19.000000 firecrawl-py-0.0.1/firecrawl_py.egg-info/top_level.txt
-drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:53:19.371410 firecrawl-py-0.0.1/mendable/
--rw-r--r--   0 nicolascamara   (501) staff       (20)       31 2024-04-12 00:47:28.000000 firecrawl-py-0.0.1/mendable/__init__.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)     3362 2024-04-12 00:53:12.000000 firecrawl-py-0.0.1/mendable/firecrawl.py
--rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 00:53:19.371762 firecrawl-py-0.0.1/setup.cfg
--rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 00:48:20.000000 firecrawl-py-0.0.1/setup.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.086758 firecrawl-py-0.0.2/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:59:13.086627 firecrawl-py-0.0.2/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3318 2024-04-12 00:43:37.000000 firecrawl-py-0.0.2/README.md
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.085818 firecrawl-py-0.0.2/firecrawl/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       31 2024-04-12 00:47:28.000000 firecrawl-py-0.0.2/firecrawl/__init__.py
+-rw-r--r--   0 nicolascamara   (501) staff       (20)     3365 2024-04-12 00:57:26.000000 firecrawl-py-0.0.2/firecrawl/firecrawl.py
+drwxr-xr-x   0 nicolascamara   (501) staff       (20)        0 2024-04-12 00:59:13.086431 firecrawl-py-0.0.2/firecrawl_py.egg-info/
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      199 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/PKG-INFO
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      242 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        1 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)        9 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/requires.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       10 2024-04-12 00:59:13.000000 firecrawl-py-0.0.2/firecrawl_py.egg-info/top_level.txt
+-rw-r--r--   0 nicolascamara   (501) staff       (20)       38 2024-04-12 00:59:13.086811 firecrawl-py-0.0.2/setup.cfg
+-rw-r--r--   0 nicolascamara   (501) staff       (20)      349 2024-04-12 00:57:41.000000 firecrawl-py-0.0.2/setup.py
```

### Comparing `firecrawl-py-0.0.1/README.md` & `firecrawl-py-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `firecrawl-py-0.0.1/mendable/firecrawl.py` & `firecrawl-py-0.0.2/firecrawl/firecrawl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import requests
 
-class FireCrawl:
+class FirecrawlApp:
     def __init__(self, api_key=None):
         self.api_key = api_key or os.getenv('FIRECRAWL_API_KEY')
         if self.api_key is None:
             raise ValueError('No API key provided')
     
     def scrape_url(self, url, params):
         headers = {
```

