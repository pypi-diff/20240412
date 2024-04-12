# Comparing `tmp/util_searchads360_hm-0.0.2.tar.gz` & `tmp/util_searchads360_hm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "util_searchads360_hm-0.0.2.tar", last modified: Fri Apr 12 13:37:38 2024, max compression
+gzip compressed data, was "util_searchads360_hm-0.0.3.tar", last modified: Fri Apr 12 13:56:39 2024, max compression
```

## Comparing `util_searchads360_hm-0.0.2.tar` & `util_searchads360_hm-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:37:38.206222 util_searchads360_hm-0.0.2/
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:37:38.206098 util_searchads360_hm-0.0.2/PKG-INFO
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:37:38.205213 util_searchads360_hm-0.0.2/interceptors/
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)      154 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.2/interceptors/__init__.py
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)     4614 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.2/interceptors/interceptor.py
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)     5980 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.2/interceptors/metadata_interceptor.py
--rw-r--r--   0 joefedorowicz   (501) staff       (20)       38 2024-04-12 13:37:38.206369 util_searchads360_hm-0.0.2/setup.cfg
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      929 2024-04-12 13:37:33.000000 util_searchads360_hm-0.0.2/setup.py
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:37:38.205924 util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:37:38.000000 util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/PKG-INFO
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      274 2024-04-12 13:37:38.000000 util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/SOURCES.txt
--rw-r--r--   0 joefedorowicz   (501) staff       (20)        1 2024-04-12 13:37:38.000000 util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/dependency_links.txt
--rw-r--r--   0 joefedorowicz   (501) staff       (20)       13 2024-04-12 13:37:38.000000 util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/top_level.txt
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.374749 util_searchads360_hm-0.0.3/
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:56:39.374631 util_searchads360_hm-0.0.3/PKG-INFO
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.373687 util_searchads360_hm-0.0.3/interceptors/
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)      154 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/__init__.py
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     4614 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/interceptor.py
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     5980 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/metadata_interceptor.py
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)       38 2024-04-12 13:56:39.374878 util_searchads360_hm-0.0.3/setup.cfg
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      929 2024-04-12 13:56:36.000000 util_searchads360_hm-0.0.3/setup.py
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.374448 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/PKG-INFO
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      274 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/SOURCES.txt
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)        1 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/dependency_links.txt
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)       13 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/top_level.txt
```

### Comparing `util_searchads360_hm-0.0.2/PKG-INFO` & `util_searchads360_hm-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: util_searchads360_hm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of the Search Ads 360 Utility Tool
 Home-page: https://developers.google.com/search-ads/reporting/client-libraries/client-libraries
 Author: Joe Fedorowicz
 Author-email: jfedorowicz@harmelin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `util_searchads360_hm-0.0.2/interceptors/interceptor.py` & `util_searchads360_hm-0.0.3/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `util_searchads360_hm-0.0.2/interceptors/metadata_interceptor.py` & `util_searchads360_hm-0.0.3/interceptors/metadata_interceptor.py`

 * *Files identical despite different names*

### Comparing `util_searchads360_hm-0.0.2/setup.py` & `util_searchads360_hm-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='util_searchads360_hm',
-    version='0.0.2',  # Update with your package version
+    version='0.0.3',  # Update with your package version
     description='A package of the Search Ads 360 Utility Tool',
     url='https://developers.google.com/search-ads/reporting/client-libraries/client-libraries',  # Update with your package URL
     author='Joe Fedorowicz',
     author_email='jfedorowicz@harmelin.com',
     license='MIT',  # Update with your package license
     packages=find_packages(),
     install_requires=[
```

### Comparing `util_searchads360_hm-0.0.2/util_searchads360_hm.egg-info/PKG-INFO` & `util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: util-searchads360-hm
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package of the Search Ads 360 Utility Tool
 Home-page: https://developers.google.com/search-ads/reporting/client-libraries/client-libraries
 Author: Joe Fedorowicz
 Author-email: jfedorowicz@harmelin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

