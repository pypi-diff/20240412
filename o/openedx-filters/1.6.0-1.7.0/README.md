# Comparing `tmp/openedx-filters-1.6.0.tar.gz` & `tmp/openedx-filters-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-filters-1.6.0.tar", last modified: Thu Aug 24 15:01:01 2023, max compression
+gzip compressed data, was "openedx-filters-1.7.0.tar", last modified: Thu Apr 11 22:26:31 2024, max compression
```

## Comparing `openedx-filters-1.6.0.tar` & `openedx-filters-1.7.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (998)     4212 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (998)    35139 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (998)      178 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (998)     6154 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)     5471 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.475371 openedx-filters-1.6.0/openedx_filters/
--rw-r--r--   0 runner    (1001) docker     (998)      103 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (998)     1083 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (998)     2765 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/openedx_filters/learning/
--rw-r--r--   0 runner    (1001) docker     (998)      168 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (998)    24828 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/learning/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/openedx_filters/learning/tests/
--rw-r--r--   0 runner    (1001) docker     (998)       75 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/learning/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (998)    21051 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/learning/tests/test_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/openedx_filters/tests/
--rw-r--r--   0 runner    (1001) docker     (998)       78 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (998)      746 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (998)      942 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (998)    17309 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (998)     8532 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/tooling.py
--rw-r--r--   0 runner    (1001) docker     (998)     1022 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/openedx_filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.475371 openedx-filters-1.6.0/openedx_filters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (998)     6154 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)      801 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (998)        7 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (998)       16 2023-08-24 15:01:01.000000 openedx-filters-1.6.0/openedx_filters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (998)       75 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (998)      268 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (998)     2846 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-24 15:01:01.479371 openedx-filters-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (998)      180 2023-08-24 15:00:57.000000 openedx-filters-1.6.0/tests/test_openedx_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24828 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/learning/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/learning/tests/test_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17309 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/openedx_filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/openedx_filters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 22:26:31.000000 openedx-filters-1.7.0/openedx_filters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 22:26:31.906100 openedx-filters-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-11 22:26:28.000000 openedx-filters-1.7.0/setup.py
```

### Comparing `openedx-filters-1.6.0/CHANGELOG.rst` & `openedx-filters-1.7.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
 
+[1.7.0] - 2024-04-11
+--------------------
+
+Added
+~~~~~
+
+* Add Python 3.11 support.
+
 [1.6.0] - 2023-08-18
 --------------------
 
 Added
 ~~~~~
 
 * CourseRunAPIRenderStarted filter added which can be used to modify the courserun data for B2C dashboard rendering process.
```

### Comparing `openedx-filters-1.6.0/LICENSE.txt` & `openedx-filters-1.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/PKG-INFO` & `openedx-filters-1.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-filters
-Version: 1.6.0
+Version: 1.7.0
 Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
 Home-page: https://github.com/openedx/openedx-filters
 Author: eduNEXT
 Author-email: technical@edunext.co
 License: AGPL 3.0
 Keywords: Python openedx
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
+Requires-Dist: django
 
 Open edX Filters
 ################
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge| |status-badge|
 
@@ -30,68 +31,22 @@
 Purpose
 *******
 
 This repository implements the necessary tooling and
 definitions used by the Hooks Extension Framework to
 manage the filters execution and extra tools.
 
-Getting Started
-***************
 
-Developing
-==========
+Getting Started with Development
+********************************
 
-One Time Setup
---------------
-.. code-block::
-
-  # Clone the repository
-  git clone git@github.com:openedx/openedx-filters.git
-  cd openedx-filters
-
-  # Set up a virtualenv using virtualenvwrapper with the same name as the repo and activate it
-  mkvirtualenv -p python3.8 openedx-filters
-
-Every time you develop something in this repo
----------------------------------------------
-.. code-block::
-
-  # Activate the virtualenv
-  workon openedx-filters
-
-  # Grab the latest code
-  git checkout main
-  git pull
-
-  # Install/update the dev requirements
-  make requirements
-
-  # Run the tests and quality checks (to verify the status before you make any changes)
-  make validate
-
-  # Make a new branch for your changes
-  git checkout -b <your_github_username>/<short_description>
-
-  # Using your favorite editor, edit the code to make your change.
-  vim …
-
-  # Run your new tests
-  pytest ./path/to/new/tests
-
-  # Run all the tests and quality checks
-  make validate
-
-  # Commit all your changes
-  git commit …
-  git push
-
-  # Open a PR and ask for review.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
 Deploying
-=========
+*********
 
 The Open edX Filters component is a Python library which doesn't
 need independent deployment. Therefore, its setup is reasonably
 straightforward. First, it needs to be added to your service
 requirements, and then it will be installed alongside requirements
 of the service.
 
@@ -101,15 +56,15 @@
 
 Getting Help
 ************
 
 Documentation
 =============
 
-See the `Open edX Hooks Extension Framework guide <https://github.com/openedx/edx-platform/blob/master/docs/guides/hooks/index.rst>`_ in edx-platform.
+See `documentation on Read the Docs <https://docs.openedx.org/projects/openedx-filters/en/latest/>`_.
 
 More Help
 =========
 
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the
 community.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openedx-filters-1.6.0/README.rst` & `openedx-filters-1.7.0/openedx_filters.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: openedx-filters
+Version: 1.7.0
+Summary: Open edX Filters from Hooks Extensions Framework (OEP-50).
+Home-page: https://github.com/openedx/openedx-filters
+Author: eduNEXT
+Author-email: technical@edunext.co
+License: AGPL 3.0
+Keywords: Python openedx
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+Requires-Dist: django
+
 Open edX Filters
 ################
 
 |pypi-badge| |ci-badge| |codecov-badge| |doc-badge| |pyversions-badge|
 |license-badge| |status-badge|
 
 Open edX Filters from Hooks Extensions Framework (`OEP-50`_).
@@ -11,68 +31,22 @@
 Purpose
 *******
 
 This repository implements the necessary tooling and
 definitions used by the Hooks Extension Framework to
 manage the filters execution and extra tools.
 
-Getting Started
-***************
-
-Developing
-==========
-
-One Time Setup
---------------
-.. code-block::
-
-  # Clone the repository
-  git clone git@github.com:openedx/openedx-filters.git
-  cd openedx-filters
-
-  # Set up a virtualenv using virtualenvwrapper with the same name as the repo and activate it
-  mkvirtualenv -p python3.8 openedx-filters
-
-Every time you develop something in this repo
----------------------------------------------
-.. code-block::
-
-  # Activate the virtualenv
-  workon openedx-filters
-
-  # Grab the latest code
-  git checkout main
-  git pull
 
-  # Install/update the dev requirements
-  make requirements
+Getting Started with Development
+********************************
 
-  # Run the tests and quality checks (to verify the status before you make any changes)
-  make validate
-
-  # Make a new branch for your changes
-  git checkout -b <your_github_username>/<short_description>
-
-  # Using your favorite editor, edit the code to make your change.
-  vim …
-
-  # Run your new tests
-  pytest ./path/to/new/tests
-
-  # Run all the tests and quality checks
-  make validate
-
-  # Commit all your changes
-  git commit …
-  git push
-
-  # Open a PR and ask for review.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
 Deploying
-=========
+*********
 
 The Open edX Filters component is a Python library which doesn't
 need independent deployment. Therefore, its setup is reasonably
 straightforward. First, it needs to be added to your service
 requirements, and then it will be installed alongside requirements
 of the service.
 
@@ -82,15 +56,15 @@
 
 Getting Help
 ************
 
 Documentation
 =============
 
-See the `Open edX Hooks Extension Framework guide <https://github.com/openedx/edx-platform/blob/master/docs/guides/hooks/index.rst>`_ in edx-platform.
+See `documentation on Read the Docs <https://docs.openedx.org/projects/openedx-filters/en/latest/>`_.
 
 More Help
 =========
 
 If you're having trouble, we have discussion forums at
 https://discuss.openedx.org where you can connect with others in the
 community.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `openedx-filters-1.6.0/openedx_filters/exceptions.py` & `openedx-filters-1.7.0/openedx_filters/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/filters.py` & `openedx-filters-1.7.0/openedx_filters/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/learning/filters.py` & `openedx-filters-1.7.0/openedx_filters/learning/filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/learning/tests/test_filters.py` & `openedx-filters-1.7.0/openedx_filters/learning/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/tests/test_exceptions.py` & `openedx-filters-1.7.0/openedx_filters/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/tests/test_filters.py` & `openedx-filters-1.7.0/openedx_filters/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/tests/test_tooling.py` & `openedx-filters-1.7.0/openedx_filters/tests/test_tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/tooling.py` & `openedx-filters-1.7.0/openedx_filters/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters/utils.py` & `openedx-filters-1.7.0/openedx_filters/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-filters-1.6.0/openedx_filters.egg-info/SOURCES.txt` & `openedx-filters-1.7.0/openedx_filters.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 openedx_filters/learning/tests/__init__.py
 openedx_filters/learning/tests/test_filters.py
 openedx_filters/tests/__init__.py
 openedx_filters/tests/test_exceptions.py
 openedx_filters/tests/test_filters.py
 openedx_filters/tests/test_tooling.py
 requirements/base.in
-tests/test_openedx_filters.py
+requirements/constraints.txt
```

