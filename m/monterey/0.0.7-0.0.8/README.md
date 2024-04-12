# Comparing `tmp/monterey-0.0.7.tar.gz` & `tmp/monterey-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monterey-0.0.7.tar", last modified: Fri Apr 12 05:46:44 2024, max compression
+gzip compressed data, was "monterey-0.0.8.tar", last modified: Fri Apr 12 06:14:27 2024, max compression
```

## Comparing `monterey-0.0.7.tar` & `monterey-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.360302 monterey-0.0.7/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:46:44.359538 monterey-0.0.7/PKG-INFO
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.348944 monterey-0.0.7/monterey/
--rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.7/monterey/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.358337 monterey-0.0.7/monterey/tools/
--rw-r--r--   0 hammad     (501) staff       (20)      296 2024-04-12 05:46:22.000000 monterey-0.0.7/monterey/tools/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/cli.py
--rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/dialogs.py
--rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/frontend.py
--rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/live_table.py
--rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/loaders.py
--rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.7/monterey/tools/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.7/monterey/tools/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.7/monterey/tools/progress_bar.py
--rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.7/monterey/tools/text.py
--rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.7/monterey/tools/tools.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 05:46:44.358891 monterey-0.0.7/monterey.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      443 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      505 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 05:46:44.000000 monterey-0.0.7/monterey.egg-info/top_level.txt
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 05:46:44.360451 monterey-0.0.7/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      560 2024-04-12 05:46:37.000000 monterey-0.0.7/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.939892 monterey-0.0.8/
+-rw-r--r--   0 hammad     (501) staff       (20)      466 2024-04-12 06:14:27.938239 monterey-0.0.8/PKG-INFO
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.923566 monterey-0.0.8/monterey/
+-rw-r--r--   0 hammad     (501) staff       (20)       51 2024-04-12 05:08:11.000000 monterey-0.0.8/monterey/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.936668 monterey-0.0.8/monterey/tools/
+-rw-r--r--   0 hammad     (501) staff       (20)      327 2024-04-12 06:14:20.000000 monterey-0.0.8/monterey/tools/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4942 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/cli.py
+-rw-r--r--   0 hammad     (501) staff       (20)     5625 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/dialogs.py
+-rw-r--r--   0 hammad     (501) staff       (20)    13289 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/frontend.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3583 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     1619 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/live_table.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2967 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/loaders.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6617 2024-04-12 05:03:16.000000 monterey-0.0.8/monterey/tools/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     4077 2024-04-12 05:03:49.000000 monterey-0.0.8/monterey/tools/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)     2461 2024-04-12 05:02:38.000000 monterey-0.0.8/monterey/tools/progress_bar.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3829 2024-04-12 06:13:31.000000 monterey-0.0.8/monterey/tools/tailwind.py
+-rw-r--r--   0 hammad     (501) staff       (20)     7323 2024-04-12 05:40:58.000000 monterey-0.0.8/monterey/tools/text.py
+-rw-r--r--   0 hammad     (501) staff       (20)      953 2024-04-12 05:03:36.000000 monterey-0.0.8/monterey/tools/tools.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-12 06:14:27.937435 monterey-0.0.8/monterey.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      466 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      532 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       49 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        9 2024-04-12 06:14:27.000000 monterey-0.0.8/monterey.egg-info/top_level.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-12 06:14:27.940185 monterey-0.0.8/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      571 2024-04-12 06:13:48.000000 monterey-0.0.8/setup.py
```

### Comparing `monterey-0.0.7/monterey/tools/cli.py` & `monterey-0.0.8/monterey/tools/cli.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/dialogs.py` & `monterey-0.0.8/monterey/tools/dialogs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/frontend.py` & `monterey-0.0.8/monterey/tools/frontend.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/inputs.py` & `monterey-0.0.8/monterey/tools/inputs.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/live_table.py` & `monterey-0.0.8/monterey/tools/live_table.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/loaders.py` & `monterey-0.0.8/monterey/tools/loaders.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/logger.py` & `monterey-0.0.8/monterey/tools/logger.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/preconditions.py` & `monterey-0.0.8/monterey/tools/preconditions.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/progress_bar.py` & `monterey-0.0.8/monterey/tools/progress_bar.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/text.py` & `monterey-0.0.8/monterey/tools/text.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/monterey/tools/tools.py` & `monterey-0.0.8/monterey/tools/tools.py`

 * *Files identical despite different names*

### Comparing `monterey-0.0.7/setup.py` & `monterey-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="monterey",
-    version="0.0.07",
+    version="0.0.08",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="monterey tools",
     long_description="""
 Monterey Tools
     """,
     packages=setuptools.find_packages(),
@@ -15,12 +15,13 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>3.8',
     install_requires=[
 "art",
 "fire",
+'Ipython',
 "prompt_toolkit",
 "pathlib",
 "rich-cli",
     ],
 )
```

