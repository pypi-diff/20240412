# Comparing `tmp/monterey-0.0.2.tar.gz` & `tmp/monterey-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.2.tar", last modified: Fri Apr 12 05:08:23 2024, max compression
+gzip compressed data, was "monterey-0.0.3.tar", last modified: Fri Apr 12 05:29:46 2024, max compression
```

## Comparing `monterey-0.0.2.tar` & `monterey-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.081875 monterey-0.0.2/
--rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:08:23.081269 monterey-0.0.2/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.073696 monterey-0.0.2/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.2/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.079479 monterey-0.0.2/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.2/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.2/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     5305 2024-04-12 05:02:38.000000 monterey-0.0.2/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.2/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:08:23.080345 monterey-0.0.2/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      463 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       46 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:08:23.000000 monterey-0.0.2/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:08:23.082053 monterey-0.0.2/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      568 2024-04-12 05:08:15.000000 monterey-0.0.2/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:29:46.882671 monterey-0.0.3/
+-rw-r--r--   0 hammad     (501) staff       (20)      471 2024-04-12 05:29:46.882096 monterey-0.0.3/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:29:46.870123 monterey-0.0.3/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.3/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:29:46.880478 monterey-0.0.3/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      255 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.3/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.3/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5305 2024-04-12 05:02:38.000000 monterey-0.0.3/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.3/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:29:46.881342 monterey-0.0.3/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      471 2024-04-12 05:29:46.000000 monterey-0.0.3/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:29:46.000000 monterey-0.0.3/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:29:46.000000 monterey-0.0.3/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       54 2024-04-12 05:29:46.000000 monterey-0.0.3/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:29:46.000000 monterey-0.0.3/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:29:46.882801 monterey-0.0.3/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      576 2024-04-12 05:29:38.000000 monterey-0.0.3/setup.py
```

### Comparing `monterey-0.0.2/monterey/tools/cli.py` & `monterey-0.0.3/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/dialogs.py` & `monterey-0.0.3/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/frontend.py` & `monterey-0.0.3/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/inputs.py` & `monterey-0.0.3/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/live_table.py` & `monterey-0.0.3/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/loaders.py` & `monterey-0.0.3/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/logger.py` & `monterey-0.0.3/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/preconditions.py` & `monterey-0.0.3/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/progress_bar.py` & `monterey-0.0.3/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/text.py` & `monterey-0.0.3/monterey/tools/text.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/monterey/tools/tools.py` & `monterey-0.0.3/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.2/setup.py` & `monterey-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.02",
+    version="0.0.03",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
@@ -18,10 +18,10 @@
     python_requires='>3.8',
     install_requires=[
 "art",
 "fire",
 "prompt_toolkit",
 "pathlib",
 "rich-cli",
-"rich",
+"rich>=13.7.1",
     ],
 )
```

