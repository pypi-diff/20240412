# Comparing `tmp/datasette-cors-1.0.tar.gz` & `tmp/datasette-cors-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-cors-1.0.tar", last modified: Mon Apr  8 17:03:05 2024, max compression
+gzip compressed data, was "datasette-cors-1.0.1.tar", last modified: Fri Apr 12 03:22:35 2024, max compression
```

## Comparing `datasette-cors-1.0.tar` & `datasette-cors-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:05.414424 datasette-cors-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 17:02:55.000000 datasette-cors-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-08 17:03:05.414424 datasette-cors-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-08 17:02:55.000000 datasette-cors-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 17:03:05.414424 datasette-cors-1.0/datasette_cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-08 17:03:05.000000 datasette-cors-1.0/datasette_cors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-08 17:02:55.000000 datasette-cors-1.0/datasette_cors.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 17:03:05.414424 datasette-cors-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 17:02:55.000000 datasette-cors-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:22:35.327258 datasette-cors-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 03:22:29.000000 datasette-cors-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-12 03:22:35.327258 datasette-cors-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-12 03:22:29.000000 datasette-cors-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:22:35.327258 datasette-cors-1.0.1/datasette_cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 03:22:35.000000 datasette-cors-1.0.1/datasette_cors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 03:22:29.000000 datasette-cors-1.0.1/datasette_cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:22:35.327258 datasette-cors-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 03:22:29.000000 datasette-cors-1.0.1/setup.py
```

### Comparing `datasette-cors-1.0/LICENSE` & `datasette-cors-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-cors-1.0/PKG-INFO` & `datasette-cors-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: datasette-cors
-Version: 1.0
+Version: 1.0.1
 Summary: Datasette plugin for configuring CORS headers
 Home-page: https://github.com/simonw/datasette-cors
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asgi-cors>=1.0
+Requires-Dist: asgi-cors>=1.0.1
 Provides-Extra: test
 Requires-Dist: datasette; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: httpx; extra == "test"
 
 # datasette-cors
```

### Comparing `datasette-cors-1.0/README.md` & `datasette-cors-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `datasette-cors-1.0/datasette_cors.egg-info/PKG-INFO` & `datasette-cors-1.0.1/datasette_cors.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: datasette-cors
-Version: 1.0
+Version: 1.0.1
 Summary: Datasette plugin for configuring CORS headers
 Home-page: https://github.com/simonw/datasette-cors
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asgi-cors>=1.0
+Requires-Dist: asgi-cors>=1.0.1
 Provides-Extra: test
 Requires-Dist: datasette; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-asyncio; extra == "test"
 Requires-Dist: httpx; extra == "test"
 
 # datasette-cors
```

### Comparing `datasette-cors-1.0/datasette_cors.py` & `datasette-cors-1.0.1/datasette_cors.py`

 * *Files identical despite different names*

### Comparing `datasette-cors-1.0/setup.py` & `datasette-cors-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "1.0"
+VERSION = "1.0.1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -19,11 +19,11 @@
     long_description_content_type="text/markdown",
     author="Simon Willison",
     url="https://github.com/simonw/datasette-cors",
     license="Apache License, Version 2.0",
     version=VERSION,
     py_modules=["datasette_cors"],
     entry_points={"datasette": ["cors = datasette_cors"]},
-    install_requires=["asgi-cors>=1.0"],
+    install_requires=["asgi-cors>=1.0.1"],
     extras_require={"test": ["datasette", "pytest", "pytest-asyncio", "httpx"]},
     tests_require=["datasette-cors[test]"],
 )
```

