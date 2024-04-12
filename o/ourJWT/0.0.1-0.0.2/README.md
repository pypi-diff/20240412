# Comparing `tmp/ourJWT-0.0.1.tar.gz` & `tmp/ourJWT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ourJWT-0.0.1.tar", last modified: Fri Apr 12 14:00:12 2024, max compression
+gzip compressed data, was "ourJWT-0.0.2.tar", last modified: Fri Apr 12 19:09:42 2024, max compression
```

## Comparing `ourJWT-0.0.1.tar` & `ourJWT-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-12 14:00:12.013117 ourJWT-0.0.1/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-12 14:00:12.013117 ourJWT-0.0.1/PKG-INFO
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-12 14:00:12.013117 ourJWT-0.0.1/ourJWT/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     2467 2024-04-12 11:29:42.000000 ourJWT-0.0.1/ourJWT/OUR_class.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      374 2024-04-08 12:48:41.000000 ourJWT-0.0.1/ourJWT/OUR_exception.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-12 12:30:21.000000 ourJWT-0.0.1/ourJWT/__init__.py
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)     1077 2024-04-12 12:50:04.000000 ourJWT-0.0.1/ourJWT/decorators.py
-drwxr-xr-x   0 gd-harco (102195) 2022_lyon  (4222)        0 2024-04-12 14:00:12.013117 ourJWT-0.0.1/ourJWT.egg-info/
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      258 2024-04-12 14:00:12.000000 ourJWT-0.0.1/ourJWT.egg-info/PKG-INFO
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      241 2024-04-12 14:00:12.000000 ourJWT-0.0.1/ourJWT.egg-info/SOURCES.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        1 2024-04-12 14:00:12.000000 ourJWT-0.0.1/ourJWT.egg-info/dependency_links.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      134 2024-04-12 14:00:12.000000 ourJWT-0.0.1/ourJWT.egg-info/requires.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)        7 2024-04-12 14:00:12.000000 ourJWT-0.0.1/ourJWT.egg-info/top_level.txt
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)       38 2024-04-12 14:00:12.013117 ourJWT-0.0.1/setup.cfg
--rw-r--r--   0 gd-harco (102195) 2022_lyon  (4222)      599 2024-04-12 12:56:31.000000 ourJWT-0.0.1/setup.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 19:09:42.148186 ourJWT-0.0.2/PKG-INFO
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/ourJWT/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     2467 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/OUR_class.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      374 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/OUR_exception.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      150 2024-04-12 19:04:02.000000 ourJWT-0.0.2/ourJWT/__init__.py
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)     1077 2024-04-12 19:02:23.000000 ourJWT-0.0.2/ourJWT/decorators.py
+drwxr-xr-x   0 gd-harco  (1000) gd-harco  (1000)        0 2024-04-12 19:09:42.148186 ourJWT-0.0.2/ourJWT.egg-info/
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      258 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/PKG-INFO
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      241 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/SOURCES.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        1 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/dependency_links.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      134 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/requires.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)        7 2024-04-12 19:09:42.000000 ourJWT-0.0.2/ourJWT.egg-info/top_level.txt
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)       38 2024-04-12 19:09:42.148186 ourJWT-0.0.2/setup.cfg
+-rw-r--r--   0 gd-harco  (1000) gd-harco  (1000)      599 2024-04-12 19:04:07.000000 ourJWT-0.0.2/setup.py
```

### Comparing `ourJWT-0.0.1/ourJWT/OUR_class.py` & `ourJWT-0.0.2/ourJWT/OUR_class.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.0.1/ourJWT/decorators.py` & `ourJWT-0.0.2/ourJWT/decorators.py`

 * *Files identical despite different names*

### Comparing `ourJWT-0.0.1/setup.py` & `ourJWT-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     include_package_data=True,
     name='ourJWT',
-    version='0.0.1',
+    version='0.0.2',
     description='repackaging of pyJWT package, adding fonction required for our_transcendence',
     author="gd-harco",
     author_email="gd-harco@student.42lyon.fr",
     py_modules=['ourJWT'],
     packages=find_packages(),
     install_requires=[
         'asgiref==3.8.1',
```

