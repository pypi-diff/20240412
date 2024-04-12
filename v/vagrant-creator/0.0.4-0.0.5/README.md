# Comparing `tmp/vagrant-creator-0.0.4.tar.gz` & `tmp/vagrant-creator-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagrant-creator-0.0.4.tar", last modified: Fri Apr 12 08:55:16 2024, max compression
+gzip compressed data, was "vagrant-creator-0.0.5.tar", last modified: Fri Apr 12 15:53:18 2024, max compression
```

## Comparing `vagrant-creator-0.0.4.tar` & `vagrant-creator-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 08:55:16.027075 vagrant-creator-0.0.4/
--rw-rw-rw-   0        0        0     1464 2024-04-12 08:55:16.026075 vagrant-creator-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-04-12 08:52:32.000000 vagrant-creator-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 08:55:16.027075 vagrant-creator-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1104 2024-04-12 08:54:46.000000 vagrant-creator-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:55:16.020075 vagrant-creator-0.0.4/vagrant_creator/
--rw-rw-rw-   0        0        0        1 2024-04-12 07:39:23.000000 vagrant-creator-0.0.4/vagrant_creator/__init__.py
--rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.4/vagrant_creator/vagrant_creator.py
-drwxrwxrwx   0        0        0        0 2024-04-12 08:55:16.025074 vagrant-creator-0.0.4/vagrant_creator.egg-info/
--rw-rw-rw-   0        0        0     1464 2024-04-12 08:55:15.000000 vagrant-creator-0.0.4/vagrant_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-04-12 08:55:15.000000 vagrant-creator-0.0.4/vagrant_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 08:55:15.000000 vagrant-creator-0.0.4/vagrant_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-12 08:55:15.000000 vagrant-creator-0.0.4/vagrant_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 08:55:15.000000 vagrant-creator-0.0.4/vagrant_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.778756 vagrant-creator-0.0.5/
+-rw-rw-rw-   0        0        0     1636 2024-04-12 15:53:18.777742 vagrant-creator-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      975 2024-04-12 15:49:21.000000 vagrant-creator-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 15:53:18.778756 vagrant-creator-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-04-12 15:50:36.000000 vagrant-creator-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.772836 vagrant-creator-0.0.5/vagrant_creator/
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:39:23.000000 vagrant-creator-0.0.5/vagrant_creator/__init__.py
+-rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.5/vagrant_creator/vagrant_creator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 15:53:18.777742 vagrant-creator-0.0.5/vagrant_creator.egg-info/
+-rw-rw-rw-   0        0        0     1636 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 15:53:18.000000 vagrant-creator-0.0.5/vagrant_creator.egg-info/top_level.txt
```

### Comparing `vagrant-creator-0.0.4/PKG-INFO` & `vagrant-creator-0.0.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagrant-creator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to generate Vagrant init files with custom configurations
 Home-page: https://github.com/ChandulaJ/vagrant-creator
 Author: Chandula Jayathilake
 Author-email: chandulaj3000@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,7 +32,15 @@
 ## Installation
 
 To install `vagrant-creator`, you can use `pip`:
 
 ```bash
 pip install vagrant-creator
 ```
+
+## Usage
+
+To generate a vagrant file, enter the following command and follow the steps as prompted to customize the file as required:
+
+```bash
+vagrant-creator
+```
```

### Comparing `vagrant-creator-0.0.4/README.md` & `vagrant-creator-0.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,7 +15,15 @@
 ## Installation
 
 To install `vagrant-creator`, you can use `pip`:
 
 ```bash
 pip install vagrant-creator
 ```
+
+## Usage
+
+To generate a vagrant file, enter the following command and follow the steps as prompted to customize the file as required:
+
+```bash
+vagrant-creator
+```
```

### Comparing `vagrant-creator-0.0.4/setup.py` & `vagrant-creator-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name='vagrant-creator',
-    version='0.0.4',
+    version='0.0.5',
     author='Chandula Jayathilake',
     author_email='chandulaj3000@gmail.com',
     description='A tool to generate Vagrant init files with custom configurations',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ChandulaJ/vagrant-creator',
     license='MIT',
```

### Comparing `vagrant-creator-0.0.4/vagrant_creator/vagrant_creator.py` & `vagrant-creator-0.0.5/vagrant_creator/vagrant_creator.py`

 * *Files identical despite different names*

### Comparing `vagrant-creator-0.0.4/vagrant_creator.egg-info/PKG-INFO` & `vagrant-creator-0.0.5/vagrant_creator.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagrant-creator
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool to generate Vagrant init files with custom configurations
 Home-page: https://github.com/ChandulaJ/vagrant-creator
 Author: Chandula Jayathilake
 Author-email: chandulaj3000@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -32,7 +32,15 @@
 ## Installation
 
 To install `vagrant-creator`, you can use `pip`:
 
 ```bash
 pip install vagrant-creator
 ```
+
+## Usage
+
+To generate a vagrant file, enter the following command and follow the steps as prompted to customize the file as required:
+
+```bash
+vagrant-creator
+```
```

