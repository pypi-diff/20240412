# Comparing `tmp/darepype-0.1.6.tar.gz` & `tmp/darepype-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/darepype-0.1.6.tar", last modified: Thu Jan 12 20:15:57 2023, max compression
+gzip compressed data, was "darepype-0.1.7.tar", last modified: Fri Apr 12 12:05:51 2024, max compression
```

## Comparing `darepype-0.1.6.tar` & `darepype-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/
--rw-r--r--   0 berthoud   (501) staff       (20)     1249 2023-01-12 20:15:57.000000 darepype-0.1.6/PKG-INFO
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype/
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype/drp/
--rw-r--r--   0 berthoud   (501) staff       (20)    35407 2022-09-08 16:00:03.000000 darepype-0.1.6/darepype/drp/dataparent.py
--rw-r--r--   0 berthoud   (501) staff       (20)     6554 2022-02-12 16:04:58.000000 darepype-0.1.6/darepype/drp/stepniparent.py
--rw-r--r--   0 berthoud   (501) staff       (20)     5726 2020-04-17 16:03:25.000000 darepype-0.1.6/darepype/drp/datatext.py
--rwxr-xr-x   0 berthoud   (501) staff       (20)    19714 2022-02-12 16:01:50.000000 darepype-0.1.6/darepype/drp/stepparent.py
--rw-r--r--   0 berthoud   (501) staff       (20)      403 2020-04-17 16:03:25.000000 darepype-0.1.6/darepype/drp/__init__.py
--rwxr-xr-x   0 berthoud   (501) staff       (20)    66540 2022-09-08 16:00:04.000000 darepype-0.1.6/darepype/drp/datafits.py
--rw-r--r--   0 berthoud   (501) staff       (20)     5372 2022-02-12 16:03:00.000000 darepype-0.1.6/darepype/drp/stepmoparent.py
--rwxr-xr-x   0 berthoud   (501) staff       (20)    30717 2022-02-11 16:59:56.000000 darepype-0.1.6/darepype/drp/pipeline.py
--rw-r--r--   0 berthoud   (501) staff       (20)     7974 2023-01-06 18:07:04.000000 darepype-0.1.6/darepype/drp/stepmiparent.py
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype/tools/
--rw-r--r--   0 berthoud   (501) staff       (20)     6922 2022-02-06 16:32:17.000000 darepype-0.1.6/darepype/tools/steplogsocket.py
--rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-02-13 16:09:20.000000 darepype-0.1.6/darepype/tools/__init__.py
--rw-r--r--   0 berthoud   (501) staff       (20)    13087 2022-09-08 21:06:46.000000 darepype-0.1.6/darepype/tools/steploadaux.py
--rwxr-xr-x   0 berthoud   (501) staff       (20)     3331 2022-02-06 16:32:17.000000 darepype-0.1.6/darepype/tools/steptemplate.py
--rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-02-27 21:28:06.000000 darepype-0.1.6/darepype/__init__.py
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype/utils/
--rw-r--r--   0 berthoud   (501) staff       (20)    10770 2022-10-13 00:19:13.000000 darepype-0.1.6/darepype/utils/stepdatagroup.py
--rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-04-17 16:03:25.000000 darepype-0.1.6/darepype/utils/__init__.py
--rwxr-xr-x   0 berthoud   (501) staff       (20)     6049 2020-04-17 16:03:25.000000 darepype-0.1.6/darepype/utils/stepsubpipe.py
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/bin/
--rwxr-xr-x   0 berthoud   (501) staff       (20)     7602 2022-02-06 16:32:17.000000 darepype-0.1.6/bin/darepyperun.py
--rw-r--r--   0 berthoud   (501) staff       (20)      788 2022-02-06 16:32:17.000000 darepype-0.1.6/README.md
--rw-r--r--   0 berthoud   (501) staff       (20)     1547 2023-01-12 20:12:50.000000 darepype-0.1.6/setup.py
--rw-r--r--   0 berthoud   (501) staff       (20)       38 2023-01-12 20:15:57.000000 darepype-0.1.6/setup.cfg
-drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/
--rw-r--r--   0 berthoud   (501) staff       (20)     1249 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/PKG-INFO
--rw-r--r--   0 berthoud   (501) staff       (20)      667 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/SOURCES.txt
--rw-r--r--   0 berthoud   (501) staff       (20)       10 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/requires.txt
--rw-r--r--   0 berthoud   (501) staff       (20)        9 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/top_level.txt
--rw-r--r--   0 berthoud   (501) staff       (20)        1 2023-01-12 20:15:57.000000 darepype-0.1.6/darepype.egg-info/dependency_links.txt
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.116631 darepype-0.1.7/
+-rw-r--r--   0 berthoud   (501) staff       (20)    35147 2020-02-13 16:09:20.000000 darepype-0.1.7/LICENSE
+-rw-r--r--   0 berthoud   (501) staff       (20)     1294 2024-04-12 12:05:51.116204 darepype-0.1.7/PKG-INFO
+-rw-r--r--   0 berthoud   (501) staff       (20)      788 2022-02-06 16:32:17.000000 darepype-0.1.7/README.md
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.091952 darepype-0.1.7/bin/
+-rwxr-xr-x   0 berthoud   (501) staff       (20)     7602 2022-02-06 16:32:17.000000 darepype-0.1.7/bin/darepyperun.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.092306 darepype-0.1.7/darepype/
+-rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-02-27 21:28:06.000000 darepype-0.1.7/darepype/__init__.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.109677 darepype-0.1.7/darepype/drp/
+-rw-r--r--   0 berthoud   (501) staff       (20)      403 2020-04-17 16:03:25.000000 darepype-0.1.7/darepype/drp/__init__.py
+-rwxr-xr-x   0 berthoud   (501) staff       (20)    66540 2022-09-08 16:00:04.000000 darepype-0.1.7/darepype/drp/datafits.py
+-rw-r--r--   0 berthoud   (501) staff       (20)    35407 2022-09-08 16:00:03.000000 darepype-0.1.7/darepype/drp/dataparent.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     5726 2020-04-17 16:03:25.000000 darepype-0.1.7/darepype/drp/datatext.py
+-rwxr-xr-x   0 berthoud   (501) staff       (20)    30717 2022-02-11 16:59:56.000000 darepype-0.1.7/darepype/drp/pipeline.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     7974 2023-01-06 18:07:04.000000 darepype-0.1.7/darepype/drp/stepmiparent.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     5372 2022-02-12 16:03:00.000000 darepype-0.1.7/darepype/drp/stepmoparent.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     6554 2022-02-12 16:04:58.000000 darepype-0.1.7/darepype/drp/stepniparent.py
+-rwxr-xr-x   0 berthoud   (501) staff       (20)    19714 2022-02-12 16:01:50.000000 darepype-0.1.7/darepype/drp/stepparent.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.111670 darepype-0.1.7/darepype/tools/
+-rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-02-13 16:09:20.000000 darepype-0.1.7/darepype/tools/__init__.py
+-rw-r--r--   0 berthoud   (501) staff       (20)    13079 2023-01-19 22:11:47.000000 darepype-0.1.7/darepype/tools/steploadaux.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     6922 2022-02-06 16:32:17.000000 darepype-0.1.7/darepype/tools/steplogsocket.py
+-rwxr-xr-x   0 berthoud   (501) staff       (20)     3331 2022-02-06 16:32:17.000000 darepype-0.1.7/darepype/tools/steptemplate.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.113465 darepype-0.1.7/darepype/utils/
+-rw-r--r--   0 berthoud   (501) staff       (20)        0 2020-04-17 16:03:25.000000 darepype-0.1.7/darepype/utils/__init__.py
+-rw-r--r--   0 berthoud   (501) staff       (20)    10770 2022-10-13 00:19:13.000000 darepype-0.1.7/darepype/utils/stepdatagroup.py
+-rwxr-xr-x   0 berthoud   (501) staff       (20)     6049 2020-04-17 16:03:25.000000 darepype-0.1.7/darepype/utils/stepsubpipe.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.115611 darepype-0.1.7/darepype.egg-info/
+-rw-r--r--   0 berthoud   (501) staff       (20)     1294 2024-04-12 12:05:50.000000 darepype-0.1.7/darepype.egg-info/PKG-INFO
+-rw-r--r--   0 berthoud   (501) staff       (20)      736 2024-04-12 12:05:50.000000 darepype-0.1.7/darepype.egg-info/SOURCES.txt
+-rw-r--r--   0 berthoud   (501) staff       (20)        1 2024-04-12 12:05:50.000000 darepype-0.1.7/darepype.egg-info/dependency_links.txt
+-rw-r--r--   0 berthoud   (501) staff       (20)       10 2024-04-12 12:05:50.000000 darepype-0.1.7/darepype.egg-info/requires.txt
+-rw-r--r--   0 berthoud   (501) staff       (20)        9 2024-04-12 12:05:50.000000 darepype-0.1.7/darepype.egg-info/top_level.txt
+-rw-r--r--   0 berthoud   (501) staff       (20)       38 2024-04-12 12:05:51.116708 darepype-0.1.7/setup.cfg
+-rw-r--r--   0 berthoud   (501) staff       (20)     1644 2024-04-12 12:05:36.000000 darepype-0.1.7/setup.py
+drwxr-xr-x   0 berthoud   (501) staff       (20)        0 2024-04-12 12:05:51.115089 darepype-0.1.7/tests/
+-rw-r--r--   0 berthoud   (501) staff       (20)     1748 2020-04-12 18:32:52.000000 darepype-0.1.7/tests/test_bin.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     5877 2022-02-20 00:16:38.000000 darepype-0.1.7/tests/test_objects.py
+-rw-r--r--   0 berthoud   (501) staff       (20)     3561 2020-04-17 16:03:25.000000 darepype-0.1.7/tests/test_piping.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `darepype-0.1.6/PKG-INFO` & `darepype-0.1.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: darepype
-Version: 0.1.6
+Version: 0.1.7
 Summary: DAta REduction PYPEline framework
 Home-page: https://github.com/berthoud/darepype
 Author: HAWC Team
 Author-email: marcberthoud@uchicago.edu
 License: GNU GPL v3+
-Description: # DarePype
-        DarePype (Data Reduction Pipeline in Python) is a python framework for developing data reduction pipelines.
-        
-        Read the documentation at [darepype.readthedocs.io](https://darepype.readthedocs.io).
-        
-        The core package for the framework is well developped and is used for the [HAWC instrument](https://www.sofia.usra.edu/science/instruments/hawc) pipeline and the [SEO telescope](https://stoneedgeobservatory.com/) pipeline at [github/yerkesobservatory/pipeline](https://github.com/yerkesobservatory/pipeline).
-        
-        ## Badges
-        [![Build Status](https://travis-ci.com/berthoud/darepype.svg?branch=master)](https://travis-ci.com/github/berthoud/darepype)
-        [![Documentation Status](https://readthedocs.org/projects/darepype/badge?version=latest)](https://darepype.readthedocs.io/en/latest/)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: configobj
+
+# DarePype
+DarePype (Data Reduction Pipeline in Python) is a python framework for developing data reduction pipelines.
+
+Read the documentation at [darepype.readthedocs.io](https://darepype.readthedocs.io).
+
+The core package for the framework is well developped and is used for the [HAWC instrument](https://www.sofia.usra.edu/science/instruments/hawc) pipeline and the [SEO telescope](https://stoneedgeobservatory.com/) pipeline at [github/yerkesobservatory/pipeline](https://github.com/yerkesobservatory/pipeline).
+
+## Badges
+[![Build Status](https://travis-ci.com/berthoud/darepype.svg?branch=master)](https://travis-ci.com/github/berthoud/darepype)
+[![Documentation Status](https://readthedocs.org/projects/darepype/badge?version=latest)](https://darepype.readthedocs.io/en/latest/)
```

### Comparing `darepype-0.1.6/darepype/drp/dataparent.py` & `darepype-0.1.7/darepype/drp/dataparent.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/stepniparent.py` & `darepype-0.1.7/darepype/drp/stepniparent.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/datatext.py` & `darepype-0.1.7/darepype/drp/datatext.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/stepparent.py` & `darepype-0.1.7/darepype/drp/stepparent.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/datafits.py` & `darepype-0.1.7/darepype/drp/datafits.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/stepmoparent.py` & `darepype-0.1.7/darepype/drp/stepmoparent.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/pipeline.py` & `darepype-0.1.7/darepype/drp/pipeline.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/drp/stepmiparent.py` & `darepype-0.1.7/darepype/drp/stepmiparent.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/tools/steplogsocket.py` & `darepype-0.1.7/darepype/tools/steplogsocket.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/tools/steploadaux.py` & `darepype-0.1.7/darepype/tools/steploadaux.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.paramlist.append([auxpar + 'file', '%sfolder/*.fits' % auxpar,
             'Filename for auxiliary file(s). Can contain * and ? ' +
             'wildcards to match multiple files to be selected using fitkeys ' +
             '(default = %sfolder/*.fits)' % auxpar])
         self.paramlist.append(['bkup'+auxpar, '',
             'Back up filename for auxiliary file(s). Can contain * and ? ' +
             'wildcards to match multiple files to be selected using fitkeys ' +
-            "(default = '' i.e. no backup folder)" % auxpar])
+            "(default = '' i.e. no backup folder)" ])
         self.paramlist.append([auxpar + 'fitkeys', [],
             'List of header keys that need to match auxiliary data file ' +
             '(default = []) - only used if multiple files ' +
             'match %sfile' % auxpar])
         if 'daterange' not in [ par[0] for par in self.paramlist] :
             self.paramlist.append(['daterange',1.0,
                 'If DATE-OBS is in fitkeys, files are matched within this many days.'])
```

### Comparing `darepype-0.1.6/darepype/tools/steptemplate.py` & `darepype-0.1.7/darepype/tools/steptemplate.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/utils/stepdatagroup.py` & `darepype-0.1.7/darepype/utils/stepdatagroup.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/darepype/utils/stepsubpipe.py` & `darepype-0.1.7/darepype/utils/stepsubpipe.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/bin/darepyperun.py` & `darepype-0.1.7/bin/darepyperun.py`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/README.md` & `darepype-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `darepype-0.1.6/setup.py` & `darepype-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 import glob
 import os
 from setuptools import setup
 
 # This call to setup() does all the work
 setup(
     name="darepype",
-    version="0.1.6",
+    version="0.1.7",
     description="DAta REduction PYPEline framework",
     long_description = open("README.md",'rb').read().decode().strip(),
     long_description_content_type="text/markdown",
     url="https://github.com/berthoud/darepype",
     author="HAWC Team",
     author_email="marcberthoud@uchicago.edu",
     license="GNU GPL v3+",
     scripts = glob.glob(os.path.join('bin','*')),
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     packages=["darepype","darepype.drp","darepype.tools","darepype.utils"],
     include_package_data=True,
     install_requires=["configobj"]
 )
 
 """ New Push to PIPY
@@ -34,19 +36,19 @@
       source bin/activate
       export PYTHONPATH=/Users/berthoud/instruments/software/DarePype
       cd ../DarePype/tests
       python -m unittest test_objects.py
       python -m unittest test_piping.py
       python -m unittest test_bin.py
     Updates
-    - Make new tag and push to github.
-    - Update version above
+    - Update version above and push to github
+    - Make new tag: git tag 0.1.7 and git push origin --tags
     Run / Install with:
         python setup.py build sdist --format=gztar
     CHECK IT:
         tar -tzf dist/*.tar.gz
         twine check dist/darepype-0.1.0.tar.gz
-        BTW: /opt/local/Library/Frameworks/Python.framework/Versions/2.7/bin/twine
+        BTW: install twine with macports
     Upload it:
         twine upload dist/*
 
 """
```

### Comparing `darepype-0.1.6/darepype.egg-info/PKG-INFO` & `darepype-0.1.7/darepype.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: darepype
-Version: 0.1.6
+Version: 0.1.7
 Summary: DAta REduction PYPEline framework
 Home-page: https://github.com/berthoud/darepype
 Author: HAWC Team
 Author-email: marcberthoud@uchicago.edu
 License: GNU GPL v3+
-Description: # DarePype
-        DarePype (Data Reduction Pipeline in Python) is a python framework for developing data reduction pipelines.
-        
-        Read the documentation at [darepype.readthedocs.io](https://darepype.readthedocs.io).
-        
-        The core package for the framework is well developped and is used for the [HAWC instrument](https://www.sofia.usra.edu/science/instruments/hawc) pipeline and the [SEO telescope](https://stoneedgeobservatory.com/) pipeline at [github/yerkesobservatory/pipeline](https://github.com/yerkesobservatory/pipeline).
-        
-        ## Badges
-        [![Build Status](https://travis-ci.com/berthoud/darepype.svg?branch=master)](https://travis-ci.com/github/berthoud/darepype)
-        [![Documentation Status](https://readthedocs.org/projects/darepype/badge?version=latest)](https://darepype.readthedocs.io/en/latest/)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: configobj
+
+# DarePype
+DarePype (Data Reduction Pipeline in Python) is a python framework for developing data reduction pipelines.
+
+Read the documentation at [darepype.readthedocs.io](https://darepype.readthedocs.io).
+
+The core package for the framework is well developped and is used for the [HAWC instrument](https://www.sofia.usra.edu/science/instruments/hawc) pipeline and the [SEO telescope](https://stoneedgeobservatory.com/) pipeline at [github/yerkesobservatory/pipeline](https://github.com/yerkesobservatory/pipeline).
+
+## Badges
+[![Build Status](https://travis-ci.com/berthoud/darepype.svg?branch=master)](https://travis-ci.com/github/berthoud/darepype)
+[![Documentation Status](https://readthedocs.org/projects/darepype/badge?version=latest)](https://darepype.readthedocs.io/en/latest/)
```

