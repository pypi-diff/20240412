# Comparing `tmp/jaraco.collections-5.0.0.tar.gz` & `tmp/jaraco.collections-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.collections-5.0.0.tar", last modified: Sat Dec  9 16:03:04 2023, max compression
+gzip compressed data, was "jaraco.collections-5.0.1.tar", last modified: Fri Apr 12 13:59:59 2024, max compression
```

## Comparing `jaraco.collections-5.0.0.tar` & `jaraco.collections-5.0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.323346 jaraco.collections-5.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.323346 jaraco.collections-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.323346 jaraco.collections-5.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.319346 jaraco.collections-5.0.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/jaraco/collections/
--rw-r--r--   0 runner    (1001) docker     (127)    25661 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/jaraco/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/jaraco/collections/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/jaraco.collections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2023-12-09 16:03:04.000000 jaraco.collections-5.0.0/jaraco.collections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-12-09 16:03:04.000000 jaraco.collections-5.0.0/jaraco.collections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-09 16:03:04.000000 jaraco.collections-5.0.0/jaraco.collections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-09 16:03:04.000000 jaraco.collections-5.0.0/jaraco.collections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-09 16:03:04.000000 jaraco.collections-5.0.0/jaraco.collections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-09 16:03:04.327346 jaraco.collections-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2023-12-09 16:02:39.000000 jaraco.collections-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.294414 jaraco.collections-5.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.294414 jaraco.collections-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.294414 jaraco.collections-5.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.290414 jaraco.collections-5.0.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/jaraco/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/jaraco/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/jaraco/collections/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/jaraco.collections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-12 13:59:59.000000 jaraco.collections-5.0.1/jaraco.collections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-12 13:59:59.000000 jaraco.collections-5.0.1/jaraco.collections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:59:59.000000 jaraco.collections-5.0.1/jaraco.collections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 13:59:59.000000 jaraco.collections-5.0.1/jaraco.collections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 13:59:59.000000 jaraco.collections-5.0.1/jaraco.collections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:59:59.298414 jaraco.collections-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-12 13:59:44.000000 jaraco.collections-5.0.1/tox.ini
```

### Comparing `jaraco.collections-5.0.0/.github/workflows/main.yml` & `jaraco.collections-5.0.1/.github/workflows/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 name: tests
 
-on: [push, pull_request]
+on:
+  merge_group:
+  push:
+    branches-ignore:
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
+  pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
   FORCE_COLOR: 1
@@ -18,28 +27,30 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
@@ -52,15 +63,17 @@
       - name: Run
         run: tox
 
   collateral:
     strategy:
       fail-fast: false
       matrix:
-        job: [diffcov, docs]
+        job:
+        - diffcov
+        - docs
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Setup Python
         uses: actions/setup-python@v4
```

### Comparing `jaraco.collections-5.0.0/LICENSE` & `jaraco.collections-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.collections-5.0.0/NEWS.rst` & `jaraco.collections-5.0.1/NEWS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.0.1
+======
+
+Bugfixes
+--------
+
+- Delinting and package refresh.
+
+
 v5.0.0
 ======
 
 Features
 --------
 
 - Moved collections into a package and declared as typed.
```

### Comparing `jaraco.collections-5.0.0/PKG-INFO` & `jaraco.collections-5.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 5.0.0
+Version: 5.0.1
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: jaraco.text
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.collections.svg
@@ -39,22 +37,18 @@
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.collections
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.collections?utm_source=pypi-jaraco.collections&utm_medium=readme
 
 Models and classes to supplement the stdlib 'collections' module.
```

### Comparing `jaraco.collections-5.0.0/README.rst` & `jaraco.collections-5.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,18 @@
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.collections
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.collections?utm_source=pypi-jaraco.collections&utm_medium=readme
 
 Models and classes to supplement the stdlib 'collections' module.
```

### Comparing `jaraco.collections-5.0.0/docs/conf.py` & `jaraco.collections-5.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-5.0.0/jaraco/collections/__init__.py` & `jaraco.collections-5.0.1/jaraco/collections/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import re
-import operator
+from __future__ import annotations
+
 import collections.abc
-import itertools
 import copy
 import functools
+import itertools
+import operator
 import random
+import re
 from collections.abc import Container, Iterable, Mapping
-from typing import Callable, Union
+from typing import Any, Callable, Union
 
 import jaraco.text
 
-
 _Matchable = Union[Callable, Container, Iterable, re.Pattern]
 
 
 def _dispatch(obj: _Matchable) -> Callable:
     # can't rely on singledispatch for Union[Container, Iterable]
     # due to ambiguity
     # (https://peps.python.org/pep-0443/#abstract-base-classes).
@@ -195,15 +196,20 @@
 
     >>> r = RangeMap.left({1: 'a', 4: 'b', 7: RangeMap.undefined_value})
     >>> r[1], r[2], r[3], r[4], r[5], r[6]
     ('a', 'a', 'a', 'b', 'b', 'b')
 
     """
 
-    def __init__(self, source, sort_params={}, key_match_comparator=operator.le):
+    def __init__(
+        self,
+        source,
+        sort_params: Mapping[str, Any] = {},
+        key_match_comparator=operator.le,
+    ):
         dict.__init__(self, source)
         self.sort_params = sort_params
         self.match = key_match_comparator
 
     @classmethod
     def left(cls, source):
         return cls(
@@ -287,58 +293,58 @@
     """
 
     @staticmethod
     def transform_key(key):  # pragma: nocover
         return key
 
     def __init__(self, *args, **kargs):
-        super(KeyTransformingDict, self).__init__()
+        super().__init__()
         # build a dictionary using the default constructs
         d = dict(*args, **kargs)
         # build this dictionary using transformed keys.
         for item in d.items():
             self.__setitem__(*item)
 
     def __setitem__(self, key, val):
         key = self.transform_key(key)
-        super(KeyTransformingDict, self).__setitem__(key, val)
+        super().__setitem__(key, val)
 
     def __getitem__(self, key):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).__getitem__(key)
+        return super().__getitem__(key)
 
     def __contains__(self, key):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).__contains__(key)
+        return super().__contains__(key)
 
     def __delitem__(self, key):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).__delitem__(key)
+        return super().__delitem__(key)
 
     def get(self, key, *args, **kwargs):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).get(key, *args, **kwargs)
+        return super().get(key, *args, **kwargs)
 
     def setdefault(self, key, *args, **kwargs):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).setdefault(key, *args, **kwargs)
+        return super().setdefault(key, *args, **kwargs)
 
     def pop(self, key, *args, **kwargs):
         key = self.transform_key(key)
-        return super(KeyTransformingDict, self).pop(key, *args, **kwargs)
+        return super().pop(key, *args, **kwargs)
 
     def matching_key_for(self, key):
         """
         Given a key, return the actual key stored in self that matches.
         Raise KeyError if the key isn't found.
         """
         try:
             return next(e_key for e_key in self.keys() if e_key == key)
-        except StopIteration:
-            raise KeyError(key)
+        except StopIteration as err:
+            raise KeyError(key) from err
 
 
 class FoldedCaseKeyedDict(KeyTransformingDict):
     """
     A case-insensitive dictionary (keys are compared as insensitive
     if they are strings).
 
@@ -479,15 +485,15 @@
     'missing item'
     >>> i.foo
     'missing item'
     """
 
     def __getattr__(self, key):
         try:
-            return getattr(super(ItemsAsAttributes, self), key)
+            return getattr(super(), key)
         except AttributeError as e:
             # attempt to get the value from the mapping (return self[key])
             #  but be careful not to lose the original exception context.
             noval = object()
 
             def _safe_getitem(cont, key, missing_result):
                 try:
@@ -673,41 +679,41 @@
     >>> len(m)
     0
     >>> 'a' in m
     False
     """
 
     def __init__(self, *args, **kwargs):
-        super(BijectiveMap, self).__init__()
+        super().__init__()
         self.update(*args, **kwargs)
 
     def __setitem__(self, item, value):
         if item == value:
             raise ValueError("Key cannot map to itself")
         overlap = (
             item in self
             and self[item] != value
             or value in self
             and self[value] != item
         )
         if overlap:
             raise ValueError("Key/Value pairs may not overlap")
-        super(BijectiveMap, self).__setitem__(item, value)
-        super(BijectiveMap, self).__setitem__(value, item)
+        super().__setitem__(item, value)
+        super().__setitem__(value, item)
 
     def __delitem__(self, item):
         self.pop(item)
 
     def __len__(self):
-        return super(BijectiveMap, self).__len__() // 2
+        return super().__len__() // 2
 
     def pop(self, key, *args, **kwargs):
         mirror = self[key]
-        super(BijectiveMap, self).__delitem__(mirror)
-        return super(BijectiveMap, self).pop(key, *args, **kwargs)
+        super().__delitem__(mirror)
+        return super().pop(key, *args, **kwargs)
 
     def update(self, *args, **kwargs):
         # build a dictionary using the default constructs
         d = dict(*args, **kwargs)
         # build this dictionary using transformed keys.
         for item in d.items():
             self.__setitem__(*item)
@@ -765,15 +771,15 @@
     >>> a.copy() is not a
     True
     """
 
     __slots__ = ['__data']
 
     def __new__(cls, *args, **kwargs):
-        self = super(FrozenDict, cls).__new__(cls)
+        self = super().__new__(cls)
         self.__data = dict(*args, **kwargs)
         return self
 
     # Container
     def __contains__(self, key):
         return key in self.__data
 
@@ -840,15 +846,15 @@
     """
 
     def __init__(self, names, codes=None):
         if isinstance(names, str):
             names = names.split()
         if codes is None:
             codes = itertools.count()
-        super(Enumeration, self).__init__(zip(names, codes))
+        super().__init__(zip(names, codes))
 
     @property
     def names(self):
         return (key for key in self if isinstance(key, str))
 
     @property
     def codes(self):
```

### Comparing `jaraco.collections-5.0.0/jaraco.collections.egg-info/PKG-INFO` & `jaraco.collections-5.0.1/jaraco.collections.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 5.0.0
+Version: 5.0.1
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: jaraco.text
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
-Requires-Dist: pytest-black>=0.3.7; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
-Requires-Dist: pytest-mypy>=0.9.1; platform_python_implementation != "PyPy" and extra == "testing"
+Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
-Requires-Dist: pytest-ruff; extra == "testing"
+Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
-Requires-Dist: sphinx<7.2.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
 Requires-Dist: jaraco.tidelift>=1.4; extra == "docs"
 
 .. image:: https://img.shields.io/pypi/v/jaraco.collections.svg
@@ -39,22 +37,18 @@
    :target: https://github.com/jaraco/jaraco.collections/actions?query=workflow%3A%22tests%22
    :alt: tests
 
 .. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
     :target: https://github.com/astral-sh/ruff
     :alt: Ruff
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
 .. image:: https://readthedocs.org/projects/jaracocollections/badge/?version=latest
    :target: https://jaracocollections.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/skeleton-2023-informational
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
    :target: https://blog.jaraco.com/skeleton
 
 .. image:: https://tidelift.com/badges/package/pypi/jaraco.collections
    :target: https://tidelift.com/subscription/pkg/pypi-jaraco.collections?utm_source=pypi-jaraco.collections&utm_medium=readme
 
 Models and classes to supplement the stdlib 'collections' module.
```

### Comparing `jaraco.collections-5.0.0/jaraco.collections.egg-info/SOURCES.txt` & `jaraco.collections-5.0.1/jaraco.collections.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 LICENSE
 NEWS.rst
 README.rst
 SECURITY.md
 mypy.ini
 pyproject.toml
 pytest.ini
+ruff.toml
 setup.cfg
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
```

### Comparing `jaraco.collections-5.0.0/setup.cfg` & `jaraco.collections-5.0.1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -9,41 +9,29 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 	jaraco.text
 
-[options.packages.find]
-exclude = 
-	build*
-	dist*
-	docs*
-	tests*
-
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
-	pytest-black >= 0.3.7; \
-	python_implementation != "PyPy"
 	pytest-cov
-	pytest-mypy >= 0.9.1; \
-	python_implementation != "PyPy"
+	pytest-mypy
 	pytest-enabler >= 2.2
-	pytest-ruff
+	pytest-ruff >= 0.2.1
 docs = 
 	sphinx >= 3.5
-	sphinx < 7.2.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 	
 	jaraco.tidelift >= 1.4
```

### Comparing `jaraco.collections-5.0.0/tests/test_collections.py` & `jaraco.collections-5.0.1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-5.0.0/tox.ini` & `jaraco.collections-5.0.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 usedevelop = True
 extras =
 	testing
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
```

