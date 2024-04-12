# Comparing `tmp/vagrant-creator-0.0.2.tar.gz` & `tmp/vagrant-creator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vagrant-creator-0.0.2.tar", last modified: Fri Apr 12 07:24:52 2024, max compression
+gzip compressed data, was "vagrant-creator-0.0.3.tar", last modified: Fri Apr 12 07:43:52 2024, max compression
```

## Comparing `vagrant-creator-0.0.2.tar` & `vagrant-creator-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:52.461988 vagrant-creator-0.0.2/
--rw-rw-rw-   0        0        0     1478 2024-04-12 07:24:52.460985 vagrant-creator-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-04-12 06:24:23.000000 vagrant-creator-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 07:24:52.461988 vagrant-creator-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-04-12 07:24:22.000000 vagrant-creator-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:52.453809 vagrant-creator-0.0.2/vagrant_creator/
--rw-rw-rw-   0        0        0       49 2024-04-12 05:34:16.000000 vagrant-creator-0.0.2/vagrant_creator/__init__.py
--rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.2/vagrant_creator/vagrant_creator.py
-drwxrwxrwx   0        0        0        0 2024-04-12 07:24:52.459974 vagrant-creator-0.0.2/vagrant_creator.egg-info/
--rw-rw-rw-   0        0        0     1478 2024-04-12 07:24:52.000000 vagrant-creator-0.0.2/vagrant_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-04-12 07:24:52.000000 vagrant-creator-0.0.2/vagrant_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 07:24:52.000000 vagrant-creator-0.0.2/vagrant_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-12 07:24:52.000000 vagrant-creator-0.0.2/vagrant_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2024-04-12 07:24:52.000000 vagrant-creator-0.0.2/vagrant_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 07:43:52.278391 vagrant-creator-0.0.3/
+-rw-rw-rw-   0        0        0     1478 2024-04-12 07:43:52.277391 vagrant-creator-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2024-04-12 06:24:23.000000 vagrant-creator-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:43:52.278391 vagrant-creator-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-04-12 07:43:33.000000 vagrant-creator-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:43:52.269390 vagrant-creator-0.0.3/vagrant_creator/
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:39:23.000000 vagrant-creator-0.0.3/vagrant_creator/__init__.py
+-rw-rw-rw-   0        0        0     3450 2024-04-12 07:08:43.000000 vagrant-creator-0.0.3/vagrant_creator/vagrant_creator.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:43:52.276390 vagrant-creator-0.0.3/vagrant_creator.egg-info/
+-rw-rw-rw-   0        0        0     1478 2024-04-12 07:43:52.000000 vagrant-creator-0.0.3/vagrant_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-04-12 07:43:52.000000 vagrant-creator-0.0.3/vagrant_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:43:52.000000 vagrant-creator-0.0.3/vagrant_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2024-04-12 07:43:52.000000 vagrant-creator-0.0.3/vagrant_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2024-04-12 07:43:52.000000 vagrant-creator-0.0.3/vagrant_creator.egg-info/top_level.txt
```

### Comparing `vagrant-creator-0.0.2/PKG-INFO` & `vagrant-creator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagrant-creator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to generate Vagrant init files with custom configurations
 Home-page: https://github.com/ChandulaJ/vagrant-creator
 Author: Chandula Jayathilake
 Author-email: chandulaj3000@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vagrant-creator-0.0.2/README.md` & `vagrant-creator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vagrant-creator-0.0.2/setup.py` & `vagrant-creator-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name='vagrant-creator',
-    version='0.0.2',
+    version='0.0.3',
     author='Chandula Jayathilake',
     author_email='chandulaj3000@gmail.com',
     description='A tool to generate Vagrant init files with custom configurations',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ChandulaJ/vagrant-creator',
     license='MIT',
@@ -22,15 +22,15 @@
         'Topic :: Utilities',
     ],
     package_data={
         '': ['*.sh'],
     },
 entry_points={
     'console_scripts': [
-        'vagrant-creator=vagrant_creator:generate_vagrantfile',
+        'vagrant-creator = vagrant_creator.vagrant_creator:generate_vagrantfile'
 
     ],
 },
     include_package_data=True,
     install_requires=[],
 )
```

### Comparing `vagrant-creator-0.0.2/vagrant_creator/vagrant_creator.py` & `vagrant-creator-0.0.3/vagrant_creator/vagrant_creator.py`

 * *Files identical despite different names*

### Comparing `vagrant-creator-0.0.2/vagrant_creator.egg-info/PKG-INFO` & `vagrant-creator-0.0.3/vagrant_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vagrant-creator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to generate Vagrant init files with custom configurations
 Home-page: https://github.com/ChandulaJ/vagrant-creator
 Author: Chandula Jayathilake
 Author-email: chandulaj3000@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

