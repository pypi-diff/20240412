# Comparing `tmp/xblock_qualtrics_survey-1.4.0.tar.gz` & `tmp/xblock_qualtrics_survey-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock_qualtrics_survey-1.4.0.tar", last modified: Mon Nov  6 15:34:52 2023, max compression
+gzip compressed data, was "xblock_qualtrics_survey-1.4.1.tar", last modified: Fri Apr 12 14:13:24 2024, max compression
```

## Comparing `xblock_qualtrics_survey-1.4.0.tar` & `xblock_qualtrics_survey-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.542482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.542482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/scenario.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.542482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/public/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/public/view.css
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/public/view.js
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/public/view.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.542482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/scenarios/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/scenarios/qualtrics-survey-single-simple.xml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.542482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/templates/view.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/test_workbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/qualtricssurvey/xblocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2023-11-06 15:34:47.000000 xblock_qualtrics_survey-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 15:34:52.546482 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-06 15:34:52.000000 xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.906344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.906344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.906344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/public/view.css
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/public/view.js
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/public/view.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/scenarios/qualtrics-survey-single-simple.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/templates/view.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/test_workbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/qualtricssurvey/xblocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-12 14:13:20.000000 xblock_qualtrics_survey-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:13:24.910344 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 14:13:24.000000 xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/top_level.txt
```

### Comparing `xblock_qualtrics_survey-1.4.0/LICENSE` & `xblock_qualtrics_survey-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/PKG-INFO` & `xblock_qualtrics_survey-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock_qualtrics_survey
-Version: 1.4.0
+Version: 1.4.1
 Summary: XBlock for linking to a Qualtrics survey
 Home-page: https://github.com/Stanford-Online/xblock-qualtrics-survey
 Author: David Adams
 Author-email: dcadams@stanford.edu
 License: AGPL-3.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `xblock_qualtrics_survey-1.4.0/README.rst` & `xblock_qualtrics_survey-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/fragment.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/fragment.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Note: We should resume test coverage for all lines in this file once
 split into its own library.
 """
 
 
 from django.template.context import Context
 from xblock.core import XBlock
-from xblock.fragment import Fragment
+from web_fragments.fragment import Fragment
 
 
 class XBlockFragmentBuilderMixin:
     """
     Create a default XBlock fragment builder
     """
     static_css = [
```

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/mixins/scenario.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/mixins/scenario.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/models.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/models.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/public/view.js` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/public/view.js`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/scenarios/qualtrics-survey-multiple-custom.xml`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/test_display.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/tests/test_workbench.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/tests/test_workbench.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/qualtricssurvey/views.py` & `xblock_qualtrics_survey-1.4.1/qualtricssurvey/views.py`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/requirements/constraints.txt` & `xblock_qualtrics_survey-1.4.1/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock_qualtrics_survey-1.4.0/setup.py` & `xblock_qualtrics_survey-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import re
 from os import path
 
 from setuptools import find_packages, setup
 
 
-version = '1.4.0'
+version = '1.4.1'
 description = __doc__.strip().split('\n')[0]
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.rst')) as file_in:
     long_description = file_in.read()
 
 
 def load_requirements(*requirements_paths):
```

### Comparing `xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/PKG-INFO` & `xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xblock-qualtrics-survey
-Version: 1.4.0
+Name: xblock_qualtrics_survey
+Version: 1.4.1
 Summary: XBlock for linking to a Qualtrics survey
 Home-page: https://github.com/Stanford-Online/xblock-qualtrics-survey
 Author: David Adams
 Author-email: dcadams@stanford.edu
 License: AGPL-3.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `xblock_qualtrics_survey-1.4.0/xblock_qualtrics_survey.egg-info/SOURCES.txt` & `xblock_qualtrics_survey-1.4.1/xblock_qualtrics_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

