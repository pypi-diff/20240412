# Comparing `tmp/util_searchads360_hm-0.0.3.tar.gz` & `tmp/util_searchads360_hm-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "util_searchads360_hm-0.0.3.tar", last modified: Fri Apr 12 13:56:39 2024, max compression
+gzip compressed data, was "util_searchads360_hm-0.0.4.tar", last modified: Fri Apr 12 14:30:16 2024, max compression
```

## Comparing `util_searchads360_hm-0.0.3.tar` & `util_searchads360_hm-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.374749 util_searchads360_hm-0.0.3/
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:56:39.374631 util_searchads360_hm-0.0.3/PKG-INFO
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.373687 util_searchads360_hm-0.0.3/interceptors/
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)      154 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/__init__.py
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)     4614 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/interceptor.py
--rw-rw-r--   0 joefedorowicz   (501) staff       (20)     5980 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.3/interceptors/metadata_interceptor.py
--rw-r--r--   0 joefedorowicz   (501) staff       (20)       38 2024-04-12 13:56:39.374878 util_searchads360_hm-0.0.3/setup.cfg
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      929 2024-04-12 13:56:36.000000 util_searchads360_hm-0.0.3/setup.py
-drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 13:56:39.374448 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/PKG-INFO
--rw-r--r--   0 joefedorowicz   (501) staff       (20)      274 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/SOURCES.txt
--rw-r--r--   0 joefedorowicz   (501) staff       (20)        1 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/dependency_links.txt
--rw-r--r--   0 joefedorowicz   (501) staff       (20)       13 2024-04-12 13:56:39.000000 util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/top_level.txt
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 14:30:16.353251 util_searchads360_hm-0.0.4/
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 14:30:16.353137 util_searchads360_hm-0.0.4/PKG-INFO
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     5584 2023-09-05 19:04:06.000000 util_searchads360_hm-0.0.4/client.py
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     1805 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.4/config.py
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 14:30:16.352279 util_searchads360_hm-0.0.4/interceptors/
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)      154 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.4/interceptors/__init__.py
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     4614 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.4/interceptors/interceptor.py
+-rw-rw-r--   0 joefedorowicz   (501) staff       (20)     5980 2022-12-05 19:13:24.000000 util_searchads360_hm-0.0.4/interceptors/metadata_interceptor.py
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)       38 2024-04-12 14:30:16.353379 util_searchads360_hm-0.0.4/setup.cfg
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      966 2024-04-12 14:30:08.000000 util_searchads360_hm-0.0.4/setup.py
+drwxr-xr-x   0 joefedorowicz   (501) staff       (20)        0 2024-04-12 14:30:16.352946 util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      704 2024-04-12 14:30:16.000000 util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/PKG-INFO
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)      294 2024-04-12 14:30:16.000000 util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/SOURCES.txt
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)        1 2024-04-12 14:30:16.000000 util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/dependency_links.txt
+-rw-r--r--   0 joefedorowicz   (501) staff       (20)       27 2024-04-12 14:30:16.000000 util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/top_level.txt
```

### Comparing `util_searchads360_hm-0.0.3/PKG-INFO` & `util_searchads360_hm-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: util_searchads360_hm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of the Search Ads 360 Utility Tool
 Home-page: https://developers.google.com/search-ads/reporting/client-libraries/client-libraries
 Author: Joe Fedorowicz
 Author-email: jfedorowicz@harmelin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `util_searchads360_hm-0.0.3/interceptors/interceptor.py` & `util_searchads360_hm-0.0.4/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `util_searchads360_hm-0.0.3/interceptors/metadata_interceptor.py` & `util_searchads360_hm-0.0.4/interceptors/metadata_interceptor.py`

 * *Files identical despite different names*

### Comparing `util_searchads360_hm-0.0.3/setup.py` & `util_searchads360_hm-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='util_searchads360_hm',
-    version='0.0.3',  # Update with your package version
+    version='0.0.4',  # Update with your package version
     description='A package of the Search Ads 360 Utility Tool',
     url='https://developers.google.com/search-ads/reporting/client-libraries/client-libraries',  # Update with your package URL
     author='Joe Fedorowicz',
     author_email='jfedorowicz@harmelin.com',
     license='MIT',  # Update with your package license
     packages=find_packages(),
+    py_modules=['client', 'config'],
     install_requires=[
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `util_searchads360_hm-0.0.3/util_searchads360_hm.egg-info/PKG-INFO` & `util_searchads360_hm-0.0.4/util_searchads360_hm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: util-searchads360-hm
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package of the Search Ads 360 Utility Tool
 Home-page: https://developers.google.com/search-ads/reporting/client-libraries/client-libraries
 Author: Joe Fedorowicz
 Author-email: jfedorowicz@harmelin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

