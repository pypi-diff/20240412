# Comparing `tmp/mime-utils-0.1.0.tar.gz` & `tmp/mime-utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mime-utils-0.1.0.tar", last modified: Sun Mar 17 21:51:24 2024, max compression
+gzip compressed data, was "mime-utils-0.1.1.tar", last modified: Thu Apr 11 23:31:26 2024, max compression
```

## Comparing `mime-utils-0.1.0.tar` & `mime-utils-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-03-17 21:51:24.096371 mime-utils-0.1.0/
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1446 2024-03-17 21:51:24.096371 mime-utils-0.1.0/PKG-INFO
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)      488 2024-03-17 21:29:21.000000 mime-utils-0.1.0/README.md
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       38 2024-03-17 21:51:24.096371 mime-utils-0.1.0/setup.cfg
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1186 2024-03-17 21:50:40.000000 mime-utils-0.1.0/setup.py
-drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-03-17 21:51:24.092371 mime-utils-0.1.0/src/
-drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-03-17 21:51:24.096371 mime-utils-0.1.0/src/mime_utils/
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       63 2024-03-17 21:49:13.000000 mime-utils-0.1.0/src/mime_utils/__init__.py
-drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-03-17 21:51:24.096371 mime-utils-0.1.0/src/mime_utils.egg-info/
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1446 2024-03-17 21:51:24.000000 mime-utils-0.1.0/src/mime_utils.egg-info/PKG-INFO
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)      234 2024-03-17 21:51:24.000000 mime-utils-0.1.0/src/mime_utils.egg-info/SOURCES.txt
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)        1 2024-03-17 21:51:24.000000 mime-utils-0.1.0/src/mime_utils.egg-info/dependency_links.txt
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       89 2024-03-17 21:51:24.000000 mime-utils-0.1.0/src/mime_utils.egg-info/requires.txt
--rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       11 2024-03-17 21:51:24.000000 mime-utils-0.1.0/src/mime_utils.egg-info/top_level.txt
+drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-04-11 23:31:26.168766 mime-utils-0.1.1/
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1446 2024-04-11 23:31:26.168766 mime-utils-0.1.1/PKG-INFO
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)      488 2024-03-17 21:29:21.000000 mime-utils-0.1.1/README.md
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       38 2024-04-11 23:31:26.168766 mime-utils-0.1.1/setup.cfg
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1186 2024-04-11 23:31:14.000000 mime-utils-0.1.1/setup.py
+drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-04-11 23:31:26.164766 mime-utils-0.1.1/src/
+drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-04-11 23:31:26.168766 mime-utils-0.1.1/src/mime_utils/
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)        0 2024-04-11 23:17:52.000000 mime-utils-0.1.1/src/mime_utils/__init__.py
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     3554 2024-03-17 21:29:37.000000 mime-utils-0.1.1/src/mime_utils/oauth2user.py
+drwxr-xr-x   0 bjomal   (1681601562) domain users (1681600513)        0 2024-04-11 23:31:26.168766 mime-utils-0.1.1/src/mime_utils.egg-info/
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)     1446 2024-04-11 23:31:26.000000 mime-utils-0.1.1/src/mime_utils.egg-info/PKG-INFO
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)      263 2024-04-11 23:31:26.000000 mime-utils-0.1.1/src/mime_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)        1 2024-04-11 23:31:26.000000 mime-utils-0.1.1/src/mime_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       89 2024-04-11 23:31:26.000000 mime-utils-0.1.1/src/mime_utils.egg-info/requires.txt
+-rw-r--r--   0 bjomal   (1681601562) domain users (1681600513)       11 2024-04-11 23:31:26.000000 mime-utils-0.1.1/src/mime_utils.egg-info/top_level.txt
```

### Comparing `mime-utils-0.1.0/PKG-INFO` & `mime-utils-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mime-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Some reusable libraries
 Home-page: https://www.vegvesen.no
 Author: Bjørne Malmanger
 Author-email: bjorne.malmanger@vegvesen.no
 License: MIT
 Description: # Mime Utils
```

### Comparing `mime-utils-0.1.0/setup.py` & `mime-utils-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description: str = fh.read()
 
 setup(
     name='mime-utils',
-    version='0.1.0',
+    version='0.1.1',
     description='Some reusable libraries',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.vegvesen.no",
     author="Bjørne Malmanger",
     author_email="bjorne.malmanger@vegvesen.no",
     license="MIT",
```

### Comparing `mime-utils-0.1.0/src/mime_utils.egg-info/PKG-INFO` & `mime-utils-0.1.1/src/mime_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mime-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: Some reusable libraries
 Home-page: https://www.vegvesen.no
 Author: Bjørne Malmanger
 Author-email: bjorne.malmanger@vegvesen.no
 License: MIT
 Description: # Mime Utils
```

