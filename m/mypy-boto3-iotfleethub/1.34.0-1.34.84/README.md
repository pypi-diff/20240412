# Comparing `tmp/mypy-boto3-iotfleethub-1.34.0.tar.gz` & `tmp/mypy_boto3_iotfleethub-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleethub-1.34.0.tar", last modified: Wed Dec 13 21:22:54 2023, max compression
+gzip compressed data, was "mypy_boto3_iotfleethub-1.34.84.tar", last modified: Fri Apr 12 19:32:36 2024, max compression
```

## Comparing `mypy-boto3-iotfleethub-1.34.0.tar` & `mypy_boto3_iotfleethub-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:54.847245 mypy-boto3-iotfleethub-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2023-12-13 21:22:54.847245 mypy-boto3-iotfleethub-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:54.847245 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8677 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:54.847245 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 21:22:54.000000 mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:54.847245 mypy-boto3-iotfleethub-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2023-12-13 21:11:59.000000 mypy-boto3-iotfleethub-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.637305 mypy_boto3_iotfleethub-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-12 19:32:36.637305 mypy_boto3_iotfleethub-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.637305 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-12 19:32:07.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8834 2024-04-12 19:32:07.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-12 19:32:07.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2024-04-12 19:32:07.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.637305 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 19:32:36.000000 mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:36.637305 mypy_boto3_iotfleethub-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-12 19:32:06.000000 mypy_boto3_iotfleethub-1.34.84/setup.py
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/LICENSE` & `mypy_boto3_iotfleethub-1.34.84/LICENSE`

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

### Comparing `mypy-boto3-iotfleethub-1.34.0/PKG-INFO` & `mypy_boto3_iotfleethub-1.34.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.34.0
-Summary: Type annotations for boto3.IoTFleetHub 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.84
+Summary: Type annotations for boto3.IoTFleetHub 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
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
 
 <a id="mypy-boto3-iotfleethub"></a>
 
 # mypy-boto3-iotfleethub
 
 [![PyPI - mypy-boto3-iotfleethub](https://img.shields.io/pypi/v/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/README.md` & `mypy_boto3_iotfleethub-1.34.84/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__init__.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,8 @@
 """
 
 from .client import IoTFleetHubClient
 from .paginator import ListApplicationsPaginator
 
 Client = IoTFleetHubClient
 
-
 __all__ = ("Client", "IoTFleetHubClient", "ListApplicationsPaginator")
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__init__.pyi` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/__main__.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetHub 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.IoTFleetHub 1.34.84\n"
+        "Version:         1.34.84\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/client.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -28,36 +28,32 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("IoTFleetHubClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class IoTFleetHubClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/)
     """
 
     meta: ClientMeta
@@ -90,35 +86,34 @@
     def create_application(
         self,
         *,
         applicationName: str,
         roleArn: str,
         applicationDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
-        Creates a Fleet Hub for AWS IoT Device Management web application.
+        Creates a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#create_application)
         """
 
     def delete_application(self, *, applicationId: str, clientToken: str = ...) -> Dict[str, Any]:
         """
-        Deletes a Fleet Hub for AWS IoT Device Management web application.
+        Deletes a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#delete_application)
         """
 
     def describe_application(self, *, applicationId: str) -> DescribeApplicationResponseTypeDef:
         """
-        Gets information about a Fleet Hub for AWS IoT Device Management web
-        application.
+        Gets information about a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.describe_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#describe_application)
         """
 
     def generate_presigned_url(
         self,
@@ -132,15 +127,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#generate_presigned_url)
         """
 
     def list_applications(self, *, nextToken: str = ...) -> ListApplicationsResponseTypeDef:
         """
-        Gets a list of Fleet Hub for AWS IoT Device Management web applications for the
+        Gets a list of Fleet Hub for IoT Device Management web applications for the
         current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#list_applications)
         """
 
@@ -170,19 +165,18 @@
 
     def update_application(
         self,
         *,
         applicationId: str,
         applicationName: str = ...,
         applicationDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates information about a Fleet Hub for a AWS IoT Device Management web
-        application.
+        Updates information about a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#update_application)
         """
 
     def get_paginator(
         self, operation_name: Literal["list_applications"]
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/client.pyi` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,33 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("IoTFleetHubClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class IoTFleetHubClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/)
     """
 
     meta: ClientMeta
@@ -86,35 +89,34 @@
     def create_application(
         self,
         *,
         applicationName: str,
         roleArn: str,
         applicationDescription: str = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
-        Creates a Fleet Hub for AWS IoT Device Management web application.
+        Creates a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.create_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#create_application)
         """
 
     def delete_application(self, *, applicationId: str, clientToken: str = ...) -> Dict[str, Any]:
         """
-        Deletes a Fleet Hub for AWS IoT Device Management web application.
+        Deletes a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.delete_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#delete_application)
         """
 
     def describe_application(self, *, applicationId: str) -> DescribeApplicationResponseTypeDef:
         """
-        Gets information about a Fleet Hub for AWS IoT Device Management web
-        application.
+        Gets information about a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.describe_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#describe_application)
         """
 
     def generate_presigned_url(
         self,
@@ -128,15 +130,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#generate_presigned_url)
         """
 
     def list_applications(self, *, nextToken: str = ...) -> ListApplicationsResponseTypeDef:
         """
-        Gets a list of Fleet Hub for AWS IoT Device Management web applications for the
+        Gets a list of Fleet Hub for IoT Device Management web applications for the
         current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.list_applications)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#list_applications)
         """
 
@@ -166,19 +168,18 @@
 
     def update_application(
         self,
         *,
         applicationId: str,
         applicationName: str = ...,
         applicationDescription: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> Dict[str, Any]:
         """
-        Updates information about a Fleet Hub for a AWS IoT Device Management web
-        application.
+        Updates information about a Fleet Hub for IoT Device Management web application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.update_application)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/client/#update_application)
         """
 
     def get_paginator(
         self, operation_name: Literal["list_applications"]
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/literals.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ApplicationStateType",
     "ListApplicationsPaginatorName",
     "IoTFleetHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationStateType = Literal["ACTIVE", "CREATE_FAILED", "CREATING", "DELETE_FAILED", "DELETING"]
 ListApplicationsPaginatorName = Literal["list_applications"]
 IoTFleetHubServiceName = Literal["iotfleethub"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -56,14 +54,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -74,14 +73,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -99,14 +99,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -119,24 +120,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -197,15 +200,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -277,17 +279,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -377,19 +381,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/literals.pyi` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -72,14 +73,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -97,14 +99,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -117,24 +120,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -195,15 +200,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -275,17 +279,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -375,19 +381,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/paginator.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListApplicationsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListApplicationsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/paginator.pyi` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/type_defs.py` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -68,18 +67,18 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": NotRequired[str],
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub/type_defs.pyi` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,18 +67,18 @@
         "tags": NotRequired[Mapping[str, str]],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
         "clientToken": NotRequired[str],
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/PKG-INFO` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.34.0
-Summary: Type annotations for boto3.IoTFleetHub 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.84
+Summary: Type annotations for boto3.IoTFleetHub 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
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
 
 <a id="mypy-boto3-iotfleethub"></a>
 
 # mypy-boto3-iotfleethub
 
 [![PyPI - mypy-boto3-iotfleethub](https://img.shields.io/pypi/v/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleethub-1.34.0/mypy_boto3_iotfleethub.egg-info/SOURCES.txt` & `mypy_boto3_iotfleethub-1.34.84/mypy_boto3_iotfleethub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.34.0/setup.py` & `mypy_boto3_iotfleethub-1.34.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleethub",
-    version="1.34.0",
+    version="1.34.84",
     packages=["mypy_boto3_iotfleethub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.IoTFleetHub 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.IoTFleetHub 1.34.84 service generated with mypy-boto3-builder 7.23.2",
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
     keywords="boto3 iotfleethub type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_iotfleethub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

