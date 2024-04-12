# Comparing `tmp/CropwiseWorker-0.1.tar.gz` & `tmp/CropwiseWorker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CropwiseWorker-0.1.tar", last modified: Fri Apr 12 11:08:14 2024, max compression
+gzip compressed data, was "CropwiseWorker-0.1.1.tar", last modified: Fri Apr 12 12:22:28 2024, max compression
```

## Comparing `CropwiseWorker-0.1.tar` & `CropwiseWorker-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 molevarkhip   (501) staff       (20)        0 2024-04-12 11:08:14.070579 CropwiseWorker-0.1/
-drwxr-xr-x   0 molevarkhip   (501) staff       (20)        0 2024-04-12 11:08:14.068649 CropwiseWorker-0.1/CropwiseWorker.egg-info/
--rw-r--r--   0 molevarkhip   (501) staff       (20)     1713 2024-04-12 11:08:13.000000 CropwiseWorker-0.1/CropwiseWorker.egg-info/PKG-INFO
--rw-r--r--   0 molevarkhip   (501) staff       (20)      207 2024-04-12 11:08:14.000000 CropwiseWorker-0.1/CropwiseWorker.egg-info/SOURCES.txt
--rw-r--r--   0 molevarkhip   (501) staff       (20)        1 2024-04-12 11:08:13.000000 CropwiseWorker-0.1/CropwiseWorker.egg-info/dependency_links.txt
--rw-r--r--   0 molevarkhip   (501) staff       (20)       16 2024-04-12 11:08:13.000000 CropwiseWorker-0.1/CropwiseWorker.egg-info/requires.txt
--rw-r--r--   0 molevarkhip   (501) staff       (20)        1 2024-04-12 11:08:13.000000 CropwiseWorker-0.1/CropwiseWorker.egg-info/top_level.txt
--rw-r--r--   0 molevarkhip   (501) staff       (20)     1713 2024-04-12 11:08:14.069896 CropwiseWorker-0.1/PKG-INFO
--rw-r--r--   0 molevarkhip   (501) staff       (20)      981 2024-04-12 10:56:15.000000 CropwiseWorker-0.1/README.md
--rw-r--r--   0 molevarkhip   (501) staff       (20)       38 2024-04-12 11:08:14.070720 CropwiseWorker-0.1/setup.cfg
--rw-r--r--   0 molevarkhip   (501) staff       (20)      990 2024-04-12 11:07:56.000000 CropwiseWorker-0.1/setup.py
+drwxr-xr-x   0 molevarkhip   (501) staff       (20)        0 2024-04-12 12:22:28.611175 CropwiseWorker-0.1.1/
+drwxr-xr-x   0 molevarkhip   (501) staff       (20)        0 2024-04-12 12:22:28.608584 CropwiseWorker-0.1.1/CropwiseWorker/
+-rw-r--r--   0 molevarkhip   (501) staff       (20)       93 2024-04-12 12:11:13.000000 CropwiseWorker-0.1.1/CropwiseWorker/__init__.py
+-rwx------   0 molevarkhip   (501) staff       (20)     7753 2024-04-12 10:43:12.000000 CropwiseWorker-0.1.1/CropwiseWorker/cropwiseworker.py
+drwxr-xr-x   0 molevarkhip   (501) staff       (20)        0 2024-04-12 12:22:28.610164 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/
+-rw-r--r--   0 molevarkhip   (501) staff       (20)     1637 2024-04-12 12:22:28.000000 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/PKG-INFO
+-rw-r--r--   0 molevarkhip   (501) staff       (20)      267 2024-04-12 12:22:28.000000 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/SOURCES.txt
+-rw-r--r--   0 molevarkhip   (501) staff       (20)        1 2024-04-12 12:22:28.000000 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/dependency_links.txt
+-rw-r--r--   0 molevarkhip   (501) staff       (20)       16 2024-04-12 12:22:28.000000 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/requires.txt
+-rw-r--r--   0 molevarkhip   (501) staff       (20)       15 2024-04-12 12:22:28.000000 CropwiseWorker-0.1.1/CropwiseWorker.egg-info/top_level.txt
+-rw-r--r--   0 molevarkhip   (501) staff       (20)     1637 2024-04-12 12:22:28.610769 CropwiseWorker-0.1.1/PKG-INFO
+-rw-r--r--   0 molevarkhip   (501) staff       (20)      981 2024-04-12 10:56:15.000000 CropwiseWorker-0.1.1/README.md
+-rw-r--r--   0 molevarkhip   (501) staff       (20)       38 2024-04-12 12:22:28.611300 CropwiseWorker-0.1.1/setup.cfg
+-rw-r--r--   0 molevarkhip   (501) staff       (20)      856 2024-04-12 12:20:32.000000 CropwiseWorker-0.1.1/setup.py
```

### Comparing `CropwiseWorker-0.1/CropwiseWorker.egg-info/PKG-INFO` & `CropwiseWorker-0.1.1/CropwiseWorker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: CropwiseWorker
-Version: 0.1
+Version: 0.1.1
 Summary: Модуль реализует функции для работы с API цифровой платформы управления агропредприятием Cropwise Operations.
 Author: Molev Arkhip
 Author-email: jobarkhip@gmail.com
-License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas
 
 
 # CropwiseWorker
```

### Comparing `CropwiseWorker-0.1/PKG-INFO` & `CropwiseWorker-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: CropwiseWorker
-Version: 0.1
+Version: 0.1.1
 Summary: Модуль реализует функции для работы с API цифровой платформы управления агропредприятием Cropwise Operations.
 Author: Molev Arkhip
 Author-email: jobarkhip@gmail.com
-License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: Russian
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: pandas
 
 
 # CropwiseWorker
```

### Comparing `CropwiseWorker-0.1/README.md` & `CropwiseWorker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `CropwiseWorker-0.1/setup.py` & `CropwiseWorker-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CropwiseWorker',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
-    author='Molev Arkhip',
-    author_email='jobarkhip@gmail.com',
-    description='Модуль реализует функции для работы с API цифровой платформы управления агропредприятием Cropwise Operations.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',  # Указываем формат описания
     install_requires=[
         'requests',
         'pandas'
     ],
-    license='Apache License 2.0',
+    author='Molev Arkhip',
+    author_email='jobarkhip@gmail.com',
+    description='Модуль реализует функции для работы с API цифровой платформы управления агропредприятием Cropwise Operations.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: Russian',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
     ],
     python_requires='>=3.6',
 )
-
```

