# Comparing `tmp/pytest-libfaketime-0.1.1.tar.gz` & `tmp/pytest-libfaketime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-libfaketime-0.1.1.tar", last modified: Wed Apr 25 12:29:12 2018, max compression
+gzip compressed data, was "dist/pytest-libfaketime-0.1.2.tar", last modified: Sat Dec 22 18:08:46 2018, max compression
```

## Comparing `pytest-libfaketime-0.1.1.tar` & `pytest-libfaketime-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 eloi      (1000) eloi      (1000)        0 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/
--rw-r--r--   0 eloi      (1000) eloi      (1000)       49 2018-01-25 13:35:21.000000 pytest-libfaketime-0.1.1/MANIFEST.in
--rw-r--r--   0 eloi      (1000) eloi      (1000)     1069 2018-01-25 13:35:21.000000 pytest-libfaketime-0.1.1/LICENSE
--rw-r--r--   0 eloi      (1000) eloi      (1000)       67 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/setup.cfg
--rw-r--r--   0 eloi      (1000) eloi      (1000)      381 2018-04-25 10:33:42.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.py
--rw-r--r--   0 eloi      (1000) eloi      (1000)     1648 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/PKG-INFO
-drwxr-xr-x   0 eloi      (1000) eloi      (1000)        0 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/
--rw-r--r--   0 eloi      (1000) eloi      (1000)       45 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/entry_points.txt
--rw-r--r--   0 eloi      (1000) eloi      (1000)       26 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/requires.txt
--rw-r--r--   0 eloi      (1000) eloi      (1000)        1 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/dependency_links.txt
--rw-r--r--   0 eloi      (1000) eloi      (1000)      324 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/SOURCES.txt
--rw-r--r--   0 eloi      (1000) eloi      (1000)     1648 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/PKG-INFO
--rw-r--r--   0 eloi      (1000) eloi      (1000)       19 2018-04-25 12:29:12.000000 pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/top_level.txt
--rw-r--r--   0 eloi      (1000) eloi      (1000)     1444 2018-04-25 12:15:01.000000 pytest-libfaketime-0.1.1/setup.py
--rw-r--r--   0 eloi      (1000) eloi      (1000)      518 2018-04-25 10:07:42.000000 pytest-libfaketime-0.1.1/README.md
+drwxr-xr-x   0 azmeuk    (1000) users      (100)        0 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/
+-rw-r--r--   0 azmeuk    (1000) users      (100)       49 2018-06-14 07:46:46.000000 pytest-libfaketime-0.1.2/MANIFEST.in
+drwxr-xr-x   0 azmeuk    (1000) users      (100)        0 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/
+-rw-r--r--   0 azmeuk    (1000) users      (100)       26 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/requires.txt
+-rw-r--r--   0 azmeuk    (1000) users      (100)       45 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/entry_points.txt
+-rw-r--r--   0 azmeuk    (1000) users      (100)        1 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/dependency_links.txt
+-rw-r--r--   0 azmeuk    (1000) users      (100)      324 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/SOURCES.txt
+-rw-r--r--   0 azmeuk    (1000) users      (100)     1624 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/PKG-INFO
+-rw-r--r--   0 azmeuk    (1000) users      (100)       19 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/top_level.txt
+-rw-r--r--   0 azmeuk    (1000) users      (100)       67 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/setup.cfg
+-rw-r--r--   0 azmeuk    (1000) users      (100)      381 2018-06-14 07:46:46.000000 pytest-libfaketime-0.1.2/pytest_libfaketime.py
+-rw-r--r--   0 azmeuk    (1000) users      (100)     1525 2018-12-22 18:02:29.000000 pytest-libfaketime-0.1.2/setup.py
+-rw-r--r--   0 azmeuk    (1000) users      (100)      386 2018-12-22 17:56:23.000000 pytest-libfaketime-0.1.2/README.md
+-rw-r--r--   0 azmeuk    (1000) users      (100)     1069 2017-09-04 21:22:08.000000 pytest-libfaketime-0.1.2/LICENSE
+-rw-r--r--   0 azmeuk    (1000) users      (100)     1624 2018-12-22 18:08:46.000000 pytest-libfaketime-0.1.2/PKG-INFO
```

### Comparing `pytest-libfaketime-0.1.1/LICENSE` & `pytest-libfaketime-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-libfaketime-0.1.1/PKG-INFO` & `pytest-libfaketime-0.1.2/pytest_libfaketime.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-libfaketime
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python-libfaketime plugin for pytest.
-Home-page: https://github.com/azmeuk/pytest-libfaketime
+Home-page: https://gitlab.com/yaal/pytest-libfaketime
 Author: Éloi Rivard
 Author-email: eloi@yaal.fr
-Maintainer: Éloi Rivard
-Maintainer-email: eloi@yaal.fr
+Maintainer: The Yaal Team
+Maintainer-email: contact@yaal.fr
 License: MIT
-Description: # pytest-libfaketime [![Build Status](https://travis-ci.org/azmeuk/pytest-libfaketime.svg?branch=master)](https://travis-ci.org/azmeuk/pytest-libfaketime) [![Latest Version](https://img.shields.io/pypi/v/pytest-libfaketime.svg)](https://pypi.python.org/pypi/pytest-libfaketime)
+Description: # pytest-libfaketime [![Latest Version](https://img.shields.io/pypi/v/pytest-libfaketime.svg)](https://pypi.python.org/pypi/pytest-libfaketime)
         [python-libfaketime](https://github.com/simon-weber/python-libfaketime) plugin for pytest, with support for [pytest-xdist](https://github.com/pytest-dev/pytest-xdist).
         
         # Installation
+        
         ```pip install pytest-libfaketime```
         
         # Tests
+        
         ```tox```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
```

### Comparing `pytest-libfaketime-0.1.1/pytest_libfaketime.egg-info/PKG-INFO` & `pytest-libfaketime-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-libfaketime
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python-libfaketime plugin for pytest.
-Home-page: https://github.com/azmeuk/pytest-libfaketime
+Home-page: https://gitlab.com/yaal/pytest-libfaketime
 Author: Éloi Rivard
 Author-email: eloi@yaal.fr
-Maintainer: Éloi Rivard
-Maintainer-email: eloi@yaal.fr
+Maintainer: The Yaal Team
+Maintainer-email: contact@yaal.fr
 License: MIT
-Description: # pytest-libfaketime [![Build Status](https://travis-ci.org/azmeuk/pytest-libfaketime.svg?branch=master)](https://travis-ci.org/azmeuk/pytest-libfaketime) [![Latest Version](https://img.shields.io/pypi/v/pytest-libfaketime.svg)](https://pypi.python.org/pypi/pytest-libfaketime)
+Description: # pytest-libfaketime [![Latest Version](https://img.shields.io/pypi/v/pytest-libfaketime.svg)](https://pypi.python.org/pypi/pytest-libfaketime)
         [python-libfaketime](https://github.com/simon-weber/python-libfaketime) plugin for pytest, with support for [pytest-xdist](https://github.com/pytest-dev/pytest-xdist).
         
         # Installation
+        
         ```pip install pytest-libfaketime```
         
         # Tests
+        
         ```tox```
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
```

### Comparing `pytest-libfaketime-0.1.1/setup.py` & `pytest-libfaketime-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+# coding: utf-8
 
-import io
 from setuptools import setup
 
 setup(
     name='pytest-libfaketime',
-    version='0.1.1',
+    version='0.1.2',
     author='Éloi Rivard',
     author_email='eloi@yaal.fr',
-    maintainer='Éloi Rivard',
-    maintainer_email='eloi@yaal.fr',
+    maintainer='The Yaal Team',
+    maintainer_email='contact@yaal.fr',
     license='MIT',
-    url='https://github.com/azmeuk/pytest-libfaketime',
+    url='https://gitlab.com/yaal/pytest-libfaketime',
     description='A python-libfaketime plugin for pytest.',
-    long_description=io.open('README.md').read(),
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
     py_modules=['pytest_libfaketime'],
     install_requires=[
         'libfaketime',
         'pytest>=3.0.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -28,14 +28,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
     ],
     entry_points={
         'pytest11': [
```

