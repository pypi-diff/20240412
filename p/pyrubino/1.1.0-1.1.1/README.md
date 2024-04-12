# Comparing `tmp/pyrubino-1.1.0.tar.gz` & `tmp/pyrubino-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubino-1.1.0.tar", last modified: Thu Apr 11 20:54:37 2024, max compression
+gzip compressed data, was "pyrubino-1.1.1.tar", last modified: Fri Apr 12 07:46:25 2024, max compression
```

## Comparing `pyrubino-1.1.0.tar` & `pyrubino-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.437857 pyrubino-1.1.0/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.1.0/LICENCE
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:54:37.437857 pyrubino-1.1.0/PKG-INFO
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.1.0/README.md
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.436858 pyrubino-1.1.0/pyrubino/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       22 2024-04-11 20:29:28.000000 pyrubino-1.1.0/pyrubino/ __init__.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     2481 2024-04-11 20:53:16.000000 pyrubino-1.1.0/pyrubino/rubino.py
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-11 20:54:37.437857 pyrubino-1.1.0/pyrubino.egg-info/
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/PKG-INFO
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/SOURCES.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/dependency_links.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-11 20:54:37.000000 pyrubino-1.1.0/pyrubino.egg-info/top_level.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-11 20:54:37.437857 pyrubino-1.1.0/setup.cfg
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-11 20:54:11.000000 pyrubino-1.1.0/setup.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:46:25.633978 pyrubino-1.1.1/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-11 20:41:50.000000 pyrubino-1.1.1/LICENCE
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 07:46:25.633978 pyrubino-1.1.1/PKG-INFO
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-11 20:41:30.000000 pyrubino-1.1.1/README.md
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:46:25.632978 pyrubino-1.1.1/pyrubino/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       22 2024-04-11 20:29:28.000000 pyrubino-1.1.1/pyrubino/ __init__.py
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     2481 2024-04-11 20:53:16.000000 pyrubino-1.1.1/pyrubino/rubino.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 07:46:25.633978 pyrubino-1.1.1/pyrubino.egg-info/
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      586 2024-04-12 07:46:25.000000 pyrubino-1.1.1/pyrubino.egg-info/PKG-INFO
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      195 2024-04-12 07:46:25.000000 pyrubino-1.1.1/pyrubino.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-12 07:46:25.000000 pyrubino-1.1.1/pyrubino.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        9 2024-04-12 07:46:25.000000 pyrubino-1.1.1/pyrubino.egg-info/top_level.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-12 07:46:25.633978 pyrubino-1.1.1/setup.cfg
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      562 2024-04-12 07:44:45.000000 pyrubino-1.1.1/setup.py
```

### Comparing `pyrubino-1.1.0/LICENCE` & `pyrubino-1.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `pyrubino-1.1.0/PKG-INFO` & `pyrubino-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.1.0
+Version: 1.1.1
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.1.0/pyrubino/rubino.py` & `pyrubino-1.1.1/pyrubino/rubino.py`

 * *Files identical despite different names*

### Comparing `pyrubino-1.1.0/pyrubino.egg-info/PKG-INFO` & `pyrubino-1.1.1/pyrubino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubino
-Version: 1.1.0
+Version: 1.1.1
 Summary: Luis Rubika libry
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrubino-1.1.0/setup.py` & `pyrubino-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='pyrubino',
-    version="1.1.0",
+    version="1.1.1",
     packages= ['pyrubino'],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika libry',
     long_description= open("README.md",'r').read(),
```

