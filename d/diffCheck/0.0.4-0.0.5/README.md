# Comparing `tmp/diffCheck-0.0.4.tar.gz` & `tmp/diffCheck-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.4.tar", last modified: Fri Apr 12 13:41:26 2024, max compression
+gzip compressed data, was "diffCheck-0.0.5.tar", last modified: Fri Apr 12 13:57:07 2024, max compression
```

## Comparing `diffCheck-0.0.4.tar` & `diffCheck-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.776529 diffCheck-0.0.4/
--rw-rw-rw-   0        0        0      806 2024-04-12 13:41:26.776031 diffCheck-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.761529 diffCheck-0.0.4/diffCheck/
--rw-rw-rw-   0        0        0       21 2024-04-12 13:41:19.000000 diffCheck-0.0.4/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0     7680 2024-04-12 13:20:49.000000 diffCheck-0.0.4/diffCheck/df_joint_detector.py
--rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_transformations.py
--rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_util.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.774034 diffCheck-0.0.4/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 13:41:26.777033 diffCheck-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-12 13:41:21.000000 diffCheck-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.535807 diffCheck-0.0.5/
+-rw-rw-rw-   0        0        0      806 2024-04-12 13:57:07.534807 diffCheck-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.524805 diffCheck-0.0.5/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-12 13:57:00.000000 diffCheck-0.0.5/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7680 2024-04-12 13:20:49.000000 diffCheck-0.0.5/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.533804 diffCheck-0.0.5/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:57:07.535807 diffCheck-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      820 2024-04-12 13:56:54.000000 diffCheck-0.0.5/setup.py
```

### Comparing `diffCheck-0.0.4/PKG-INFO` & `diffCheck-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.4
+Version: 0.0.5
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.4/diffCheck/df_geometries.py` & `diffCheck-0.0.5/diffCheck/df_geometries.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.4/diffCheck/df_joint_detector.py` & `diffCheck-0.0.5/diffCheck/df_joint_detector.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.4/diffCheck/df_transformations.py` & `diffCheck-0.0.5/diffCheck/df_transformations.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.4/diffCheck/df_util.py` & `diffCheck-0.0.5/diffCheck/df_util.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.4/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.5/diffCheck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.4
+Version: 0.0.5
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.4/setup.py` & `diffCheck-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diffCheck',
-    version='0.0.4',
-    packages=find_packages(),
+    version='0.0.5',
+    packages=['diffCheck'],
+    install_requires=[
+        'numpy',
+        # other dependencies...
+    ],
     description='DiffCheck is a package to check the differences between two timber structures',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand',
     author_email='andrea.settimi@epfl.ch',
     url='https://github.com/diffCheckOrg/diffCheck',
     classifiers=[
```

