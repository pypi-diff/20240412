# Comparing `tmp/monterey-0.0.6.tar.gz` & `tmp/monterey-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.6.tar", last modified: Fri Apr 12 05:41:14 2024, max compression
+gzip compressed data, was "monterey-0.0.7.tar", last modified: Fri Apr 12 05:46:44 2024, max compression
```

## Comparing `monterey-0.0.6.tar` & `monterey-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.918055 monterey-0.0.6/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:41:14.916849 monterey-0.0.6/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.894184 monterey-0.0.6/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.6/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.914396 monterey-0.0.6/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.6/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.6/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.6/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.6/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.6/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:41:14.915505 monterey-0.0.6/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:41:14.000000 monterey-0.0.6/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:41:14.918861 monterey-0.0.6/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 05:41:05.000000 monterey-0.0.6/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.360302 monterey-0.0.7/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:46:44.359538 monterey-0.0.7/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.348944 monterey-0.0.7/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.7/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.358337 monterey-0.0.7/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      296 2024-04-12 05:46:22.000000 monterey-0.0.7/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.7/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.7/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.7/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.7/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.358891 monterey-0.0.7/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:46:44.360451 monterey-0.0.7/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 05:46:37.000000 monterey-0.0.7/setup.py
```

### Comparing `monterey-0.0.6/monterey/tools/cli.py` & `monterey-0.0.7/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/dialogs.py` & `monterey-0.0.7/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/frontend.py` & `monterey-0.0.7/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/inputs.py` & `monterey-0.0.7/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/live_table.py` & `monterey-0.0.7/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/loaders.py` & `monterey-0.0.7/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/logger.py` & `monterey-0.0.7/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/preconditions.py` & `monterey-0.0.7/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/progress_bar.py` & `monterey-0.0.7/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/text.py` & `monterey-0.0.7/monterey/tools/text.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/monterey/tools/tools.py` & `monterey-0.0.7/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.6/setup.py` & `monterey-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.06",
+    version="0.0.07",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
```

