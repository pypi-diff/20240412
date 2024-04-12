# Comparing `tmp/freeze_dried_data-1.0.3.tar.gz` & `tmp/freeze_dried_data-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze_dried_data-1.0.3.tar", last modified: Sat Mar 11 03:16:15 2023, max compression
+gzip compressed data, was "freeze_dried_data-1.1.0.tar", last modified: Fri Apr 12 06:59:36 2024, max compression
```

## Comparing `freeze_dried_data-1.0.3.tar` & `freeze_dried_data-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2023-03-11 03:16:15.084296 freeze_dried_data-1.0.3/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2023-03-11 03:16:07.000000 freeze_dried_data-1.0.3/LICENSE
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      751 2023-03-11 03:16:15.084296 freeze_dried_data-1.0.3/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     2373 2023-03-11 03:16:07.000000 freeze_dried_data-1.0.3/README.md
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2023-03-11 03:16:15.084296 freeze_dried_data-1.0.3/freeze_dried_data/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2023-03-11 03:16:07.000000 freeze_dried_data-1.0.3/freeze_dried_data/__init__.py
--rw-rw-r--   0 tstand    (1000) tstand    (1000)     3575 2023-03-11 03:16:07.000000 freeze_dried_data-1.0.3/freeze_dried_data/freeze_dried_data.py
-drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2023-03-11 03:16:15.084296 freeze_dried_data-1.0.3/freeze_dried_data.egg-info/
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      751 2023-03-11 03:16:15.000000 freeze_dried_data-1.0.3/freeze_dried_data.egg-info/PKG-INFO
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      259 2023-03-11 03:16:15.000000 freeze_dried_data-1.0.3/freeze_dried_data.egg-info/SOURCES.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2023-03-11 03:16:15.000000 freeze_dried_data-1.0.3/freeze_dried_data.egg-info/dependency_links.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2023-03-11 03:16:15.000000 freeze_dried_data-1.0.3/freeze_dried_data.egg-info/top_level.txt
--rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2023-03-11 03:16:15.084296 freeze_dried_data-1.0.3/setup.cfg
--rw-rw-r--   0 tstand    (1000) tstand    (1000)      810 2023-03-11 03:16:07.000000 freeze_dried_data-1.0.3/setup.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     1072 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/LICENSE
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      825 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     3474 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/README.md
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/freeze_dried_data/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       33 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/__init__.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     6946 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/freeze_dried_data.py
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)     5277 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/freeze_dried_data/test_freeze_dried_data.py
+drwxrwxr-x   0 tstand    (1000) tstand    (1000)        0 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      825 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/PKG-INFO
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      303 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)        1 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       18 2024-04-12 06:59:36.000000 freeze_dried_data-1.1.0/freeze_dried_data.egg-info/top_level.txt
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)       38 2024-04-12 06:59:36.828151 freeze_dried_data-1.1.0/setup.cfg
+-rw-rw-r--   0 tstand    (1000) tstand    (1000)      910 2024-04-12 06:59:01.000000 freeze_dried_data-1.1.0/setup.py
```

### Comparing `freeze_dried_data-1.0.3/LICENSE` & `freeze_dried_data-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze_dried_data-1.0.3/setup.py` & `freeze_dried_data-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup
 
 setup(
     name='freeze_dried_data',
-    version='1.0.3',
+    version='1.1.0',
     description='A simple format for machine learning datasets',
     url='https://github.com/tstandley/freeze_dried_data',
-    author='trevor standley',
+    author='Trevor Standley',
     author_email='trevor.standley@gmail.com',
     license='MIT',
     packages=['freeze_dried_data'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

