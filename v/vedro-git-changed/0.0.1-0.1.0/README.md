# Comparing `tmp/vedro-git-changed-0.0.1.tar.gz` & `tmp/vedro-git-changed-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-git-changed-0.0.1.tar", last modified: Wed Jan  3 12:19:30 2024, max compression
+gzip compressed data, was "vedro-git-changed-0.1.0.tar", last modified: Wed Jan  3 15:33:05 2024, max compression
```

## Comparing `vedro-git-changed-0.0.1.tar` & `vedro-git-changed-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 12:19:30.919441 vedro-git-changed-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-03 12:19:30.919441 vedro-git-changed-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-03 12:19:30.923441 vedro-git-changed-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 12:19:30.919441 vedro-git-changed-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/tests/test_git_changed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 12:19:30.919441 vedro-git-changed-0.0.1/vedro_git_changed/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/vedro_git_changed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-01-03 12:19:20.000000 vedro-git-changed-0.0.1/vedro_git_changed/_vedro_git_changed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 12:19:30.919441 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-01-03 12:19:30.000000 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-03 12:19:30.000000 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 12:19:30.000000 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-03 12:19:30.000000 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-03 12:19:30.000000 vedro-git-changed-0.0.1/vedro_git_changed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 15:33:05.120237 vedro-git-changed-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-03 15:33:05.120237 vedro-git-changed-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-03 15:33:05.120237 vedro-git-changed-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 15:33:05.116237 vedro-git-changed-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5548 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/tests/test_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 15:33:05.116237 vedro-git-changed-0.1.0/vedro_git_changed/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/vedro_git_changed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/vedro_git_changed/_git_changed_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-01-03 15:32:58.000000 vedro-git-changed-0.1.0/vedro_git_changed/_git_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 15:33:05.120237 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-01-03 15:33:05.000000 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-03 15:33:05.000000 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 15:33:05.000000 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-03 15:33:05.000000 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-03 15:33:05.000000 vedro-git-changed-0.1.0/vedro_git_changed.egg-info/top_level.txt
```

### Comparing `vedro-git-changed-0.0.1/LICENSE` & `vedro-git-changed-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-git-changed-0.0.1/PKG-INFO` & `vedro-git-changed-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vedro-git-changed
-Version: 0.0.1
-Summary: Runs only scenarios that have changed based on git diff against a specified branch
+Version: 0.1.0
+Summary: Vedro plugin that runs test scenarios which have changed relative to the specified git branch
 Home-page: https://github.com/vedro-universe/vedro-git-changed
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://github.com/vedro-universe/vedro-git-changed
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-git-changed
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,15 +24,15 @@
 # Vedro Git Changed
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-git-changed/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-git-changed)
 [![PyPI](https://img.shields.io/pypi/v/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-git-changed?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 
-[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios that have been changed relative to a specified git branch.
+[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios which have changed relative to the specified git branch.
 
 ## Installation
 
 <details open>
 <summary>Quick</summary>
 <p>
```

### Comparing `vedro-git-changed-0.0.1/README.md` & `vedro-git-changed-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Vedro Git Changed
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-git-changed/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-git-changed)
 [![PyPI](https://img.shields.io/pypi/v/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-git-changed?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 
-[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios that have been changed relative to a specified git branch.
+[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios which have changed relative to the specified git branch.
 
 ## Installation
 
 <details open>
 <summary>Quick</summary>
 <p>
```

### Comparing `vedro-git-changed-0.0.1/setup.cfg` & `vedro-git-changed-0.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.0.1
+current_version = 0.1.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `vedro-git-changed-0.0.1/setup.py` & `vedro-git-changed-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-git-changed",
-    version="0.0.1",
-    description="Runs only scenarios that have changed based on git diff against a specified branch",
+    version="0.1.0",
+    description=("Vedro plugin that runs test scenarios which have changed "
+                 "relative to the specified git branch"),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-git-changed",
     project_urls={
```

### Comparing `vedro-git-changed-0.0.1/vedro_git_changed.egg-info/PKG-INFO` & `vedro-git-changed-0.1.0/vedro_git_changed.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: vedro-git-changed
-Version: 0.0.1
-Summary: Runs only scenarios that have changed based on git diff against a specified branch
+Version: 0.1.0
+Summary: Vedro plugin that runs test scenarios which have changed relative to the specified git branch
 Home-page: https://github.com/vedro-universe/vedro-git-changed
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://github.com/vedro-universe/vedro-git-changed
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-git-changed
 Classifier: License :: OSI Approved :: Apache Software License
@@ -24,15 +24,15 @@
 # Vedro Git Changed
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-git-changed/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-git-changed)
 [![PyPI](https://img.shields.io/pypi/v/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-git-changed?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-git-changed.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-git-changed/)
 
-[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios that have been changed relative to a specified git branch.
+[vedro-git-changed](https://pypi.org/project/vedro-git-changed/) is a Vedro plugin that runs test scenarios which have changed relative to the specified git branch.
 
 ## Installation
 
 <details open>
 <summary>Quick</summary>
 <p>
```

