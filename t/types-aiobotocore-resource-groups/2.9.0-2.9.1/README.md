# Comparing `tmp/types-aiobotocore-resource-groups-2.9.0.tar.gz` & `tmp/types-aiobotocore-resource-groups-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-groups-2.9.0.tar", last modified: Wed Dec 13 20:00:18 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-groups-2.9.1.tar", last modified: Thu Jan 18 01:21:38 2024, max compression
```

## Comparing `types-aiobotocore-resource-groups-2.9.0.tar` & `types-aiobotocore-resource-groups-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.501241 types-aiobotocore-resource-groups-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2023-12-13 20:00:18.501241 types-aiobotocore-resource-groups-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12110 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:18.501241 types-aiobotocore-resource-groups-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.501241 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17013 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17009 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10009 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10007 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14309 2023-12-13 19:54:41.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:40.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:18.501241 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      965 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 20:00:18.000000 types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.013083 types-aiobotocore-resource-groups-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-01-18 01:21:38.013083 types-aiobotocore-resource-groups-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:38.013083 types-aiobotocore-resource-groups-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.013083 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17015 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17012 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14309 2024-01-18 01:16:17.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:16.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:38.013083 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13724 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:37.000000 types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/LICENSE` & `types-aiobotocore-resource-groups-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/PKG-INFO` & `types-aiobotocore-resource-groups-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-groups
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceGroups 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceGroups 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroups 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[aiobotocore.ResourceGroups 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/README.md` & `types-aiobotocore-resource-groups-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroups 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[aiobotocore.ResourceGroups 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/setup.py` & `types-aiobotocore-resource-groups-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-groups",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_resource_groups"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ResourceGroups 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ResourceGroups 2.9.1 service generated with"
+        " mypy-boto3-builder 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="aiobotocore resource-groups type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resource_groups": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__init__.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import ResourceGroupsClient
 from .paginator import ListGroupResourcesPaginator, ListGroupsPaginator, SearchResourcesPaginator
 
 Client = ResourceGroupsClient
 
-
 __all__ = (
     "Client",
     "ListGroupResourcesPaginator",
     "ListGroupsPaginator",
     "ResourceGroupsClient",
     "SearchResourcesPaginator",
 )
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__init__.pyi` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/__main__.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceGroups 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ResourceGroups 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.9.0")
+    print("2.9.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/client.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ResourceGroupsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -111,15 +110,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...,
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -208,15 +207,15 @@
     async def list_group_resources(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupResourcesOutputTypeDef:
         """
         Returns a list of ARNs of the resources that are members of a specified
         resource
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_group_resources)
@@ -224,15 +223,15 @@
         """
 
     async def list_groups(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupsOutputTypeDef:
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/client.pyi` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     async def create_group(
         self,
         *,
         Name: str,
         Description: str = ...,
         ResourceQuery: ResourceQueryTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...
+        Configuration: Sequence[GroupConfigurationItemTypeDef] = ...,
     ) -> CreateGroupOutputTypeDef:
         """
         Creates a resource group with the specified name and description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#create_group)
         """
@@ -204,15 +204,15 @@
     async def list_group_resources(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupResourcesOutputTypeDef:
         """
         Returns a list of ARNs of the resources that are members of a specified
         resource
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_group_resources)
@@ -220,15 +220,15 @@
         """
 
     async def list_groups(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListGroupsOutputTypeDef:
         """
         Returns a list of existing Resource Groups in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Client.list_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/client/#list_groups)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/literals.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GroupConfigurationStatusType",
     "GroupFilterNameType",
     "GroupLifecycleEventsDesiredStatusType",
     "GroupLifecycleEventsStatusType",
     "ListGroupResourcesPaginatorName",
     "ListGroupsPaginatorName",
@@ -35,15 +34,14 @@
     "ResourceGroupsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GroupConfigurationStatusType = Literal["UPDATE_COMPLETE", "UPDATE_FAILED", "UPDATING"]
 GroupFilterNameType = Literal["configuration-type", "resource-type"]
 GroupLifecycleEventsDesiredStatusType = Literal["ACTIVE", "INACTIVE"]
 GroupLifecycleEventsStatusType = Literal["ACTIVE", "ERROR", "INACTIVE", "IN_PROGRESS"]
 ListGroupResourcesPaginatorName = Literal["list_group_resources"]
 ListGroupsPaginatorName = Literal["list_groups"]
 QueryErrorCodeType = Literal[
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/literals.pyi` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/paginator.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     ResourceFilterTypeDef,
     ResourceQueryTypeDef,
     SearchResourcesOutputTypeDef,
 )
 
 __all__ = ("ListGroupResourcesPaginator", "ListGroupsPaginator", "SearchResourcesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -61,15 +60,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 
@@ -79,15 +78,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
         """
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/paginator.pyi` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         Group: str = ...,
         Filters: Sequence[ResourceFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupresourcespaginator)
         """
 
 class ListGroupsPaginator(AioPaginator):
@@ -75,15 +75,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[GroupFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/paginators/#listgroupspaginator)
         """
 
 class SearchResourcesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/type_defs.py` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountSettingsTypeDef",
     "ResourceQueryTypeDef",
     "GroupTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteGroupInputRequestTypeDef",
     "FailedResourceTypeDef",
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups/type_defs.pyi` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/PKG-INFO` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-groups
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ResourceGroups 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ResourceGroups 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-resource-groups"></a>
 
 # types-aiobotocore-resource-groups
 
 [![PyPI - types-aiobotocore-resource-groups](https://img.shields.io/pypi/v/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-groups.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-groups)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-groups)](https://pepy.tech/project/types-aiobotocore-resource-groups)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ResourceGroups 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
+[aiobotocore.ResourceGroups 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-resource-groups docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_groups/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-resource-groups-2.9.0/types_aiobotocore_resource_groups.egg-info/SOURCES.txt` & `types-aiobotocore-resource-groups-2.9.1/types_aiobotocore_resource_groups.egg-info/SOURCES.txt`

 * *Files identical despite different names*
