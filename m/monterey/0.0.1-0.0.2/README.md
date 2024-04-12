# Comparing `tmp/monterey-0.0.1.tar.gz` & `tmp/monterey-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.1.tar", last modified: Fri Apr 12 05:07:25 2024, max compression
+gzip compressed data, was "monterey-0.0.2.tar", last modified: Fri Apr 12 05:08:23 2024, max compression
```

## Comparing `monterey-0.0.1.tar` & `monterey-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:07:25.526758 monterey-0.0.1/
--rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:07:25.526318 monterey-0.0.1/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:07:25.515887 monterey-0.0.1/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       20 2024-04-12 05:03:58.000000 monterey-0.0.1/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:07:25.525438 monterey-0.0.1/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.1/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.1/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     5305 2024-04-12 05:02:38.000000 monterey-0.0.1/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.1/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:07:25.525841 monterey-0.0.1/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:07:25.000000 monterey-0.0.1/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:07:25.000000 monterey-0.0.1/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:07:25.000000 monterey-0.0.1/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       46 2024-04-12 05:07:25.000000 monterey-0.0.1/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:07:25.000000 monterey-0.0.1/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:07:25.526867 monterey-0.0.1/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      568 2024-04-12 05:04:31.000000 monterey-0.0.1/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.081875 monterey-0.0.2/
+-rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:08:23.081269 monterey-0.0.2/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.073696 monterey-0.0.2/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.2/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.079479 monterey-0.0.2/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.2/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.2/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5305 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.2/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.080345 monterey-0.0.2/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       46 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:08:23.082053 monterey-0.0.2/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      568 2024-04-12 05:08:15.000000 monterey-0.0.2/setup.py
```

### Comparing `monterey-0.0.1/monterey/tools/cli.py` & `monterey-0.0.2/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/dialogs.py` & `monterey-0.0.2/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/frontend.py` & `monterey-0.0.2/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/inputs.py` & `monterey-0.0.2/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/live_table.py` & `monterey-0.0.2/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/loaders.py` & `monterey-0.0.2/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/logger.py` & `monterey-0.0.2/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/preconditions.py` & `monterey-0.0.2/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/progress_bar.py` & `monterey-0.0.2/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/text.py` & `monterey-0.0.2/monterey/tools/text.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/monterey/tools/tools.py` & `monterey-0.0.2/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.1/setup.py` & `monterey-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.01",
+    version="0.0.02",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
```

