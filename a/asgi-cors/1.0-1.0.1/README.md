# Comparing `tmp/asgi-cors-1.0.tar.gz` & `tmp/asgi-cors-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi-cors-1.0.tar", last modified: Mon Apr  8 16:18:32 2024, max compression
+gzip compressed data, was "asgi-cors-1.0.1.tar", last modified: Fri Apr 12 03:19:49 2024, max compression
```

## Comparing `asgi-cors-1.0.tar` & `asgi-cors-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:18:32.904999 asgi-cors-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 16:18:12.000000 asgi-cors-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-08 16:18:32.904999 asgi-cors-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-08 16:18:12.000000 asgi-cors-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:18:32.904999 asgi-cors-1.0/asgi_cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-08 16:18:32.000000 asgi-cors-1.0/asgi_cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 16:18:32.000000 asgi-cors-1.0/asgi_cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:18:32.000000 asgi-cors-1.0/asgi_cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:18:32.000000 asgi-cors-1.0/asgi_cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 16:18:32.000000 asgi-cors-1.0/asgi_cors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-08 16:18:12.000000 asgi-cors-1.0/asgi_cors.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 16:18:32.904999 asgi-cors-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-08 16:18:12.000000 asgi-cors-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:19:49.189041 asgi-cors-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 03:19:38.000000 asgi-cors-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-12 03:19:49.189041 asgi-cors-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-12 03:19:38.000000 asgi-cors-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:19:49.189041 asgi-cors-1.0.1/asgi_cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-12 03:19:49.000000 asgi-cors-1.0.1/asgi_cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 03:19:49.000000 asgi-cors-1.0.1/asgi_cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:19:49.000000 asgi-cors-1.0.1/asgi_cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 03:19:49.000000 asgi-cors-1.0.1/asgi_cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 03:19:49.000000 asgi-cors-1.0.1/asgi_cors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-12 03:19:38.000000 asgi-cors-1.0.1/asgi_cors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 03:19:49.189041 asgi-cors-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 03:19:38.000000 asgi-cors-1.0.1/setup.py
```

### Comparing `asgi-cors-1.0/LICENSE` & `asgi-cors-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi-cors-1.0/PKG-INFO` & `asgi-cors-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-cors
-Version: 1.0
+Version: 1.0.1
 Summary: ASGI middleware for applying CORS headers to an ASGI application
 Home-page: https://github.com/simonw/asgi-cors
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
```

### Comparing `asgi-cors-1.0/README.md` & `asgi-cors-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asgi-cors-1.0/asgi_cors.egg-info/PKG-INFO` & `asgi-cors-1.0.1/asgi_cors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-cors
-Version: 1.0
+Version: 1.0.1
 Summary: ASGI middleware for applying CORS headers to an ASGI application
 Home-page: https://github.com/simonw/asgi-cors
 Author: Simon Willison
 License: Apache License, Version 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: test
```

### Comparing `asgi-cors-1.0/asgi_cors.py` & `asgi-cors-1.0.1/asgi_cors.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,16 +61,16 @@
                     if access_control_allow_origin is not None:
                         # Construct a new event with new headers
                         new_headers = [
                             p
                             for p in original_headers
                             if p[0]
                             not in (
-                                b"access-control-allow-origin"
-                                b"access-control-allow-headers"
+                                b"access-control-allow-origin",
+                                b"access-control-allow-headers",
                                 b"access-control-allow-methods",
                                 b"access-control-max-age",
                             )
                         ]
                         if access_control_allow_origin:
                             new_headers.append(
                                 [
```

### Comparing `asgi-cors-1.0/setup.py` & `asgi-cors-1.0.1/setup.py`

 * *Files 1% similar despite different names*

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
```

