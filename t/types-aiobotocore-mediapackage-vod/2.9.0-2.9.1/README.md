# Comparing `tmp/types-aiobotocore-mediapackage-vod-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediapackage-vod-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediapackage-vod-2.9.0.tar", last modified: Wed Dec 13 19:59:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediapackage-vod-2.9.1.tar", last modified: Thu Jan 18 01:21:15 2024, max compression
```

## Comparing `types-aiobotocore-mediapackage-vod-2.9.0.tar` & `types-aiobotocore-mediapackage-vod-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.857456 types-aiobotocore-mediapackage-vod-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2023-12-13 19:59:53.857456 types-aiobotocore-mediapackage-vod-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12199 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:53.857456 types-aiobotocore-mediapackage-vod-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.857456 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16827 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21697 2023-12-13 19:50:16.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21696 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:15.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:53.857456 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 19:59:53.000000 types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.725183 types-aiobotocore-mediapackage-vod-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-01-18 01:21:15.725183 types-aiobotocore-mediapackage-vod-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12199 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:15.725183 types-aiobotocore-mediapackage-vod-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.725183 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16833 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16830 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21696 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21696 2024-01-18 01:11:59.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:58.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:15.725183 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13817 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:15.000000 types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/LICENSE` & `types-aiobotocore-mediapackage-vod-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/PKG-INFO` & `types-aiobotocore-mediapackage-vod-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage-vod
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaPackageVod 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaPackageVod 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/
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
 
 <a id="types-aiobotocore-mediapackage-vod"></a>
 
 # types-aiobotocore-mediapackage-vod
 
 [![PyPI - types-aiobotocore-mediapackage-vod](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage-vod)](https://pepy.tech/project/types-aiobotocore-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackageVod 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[aiobotocore.MediaPackageVod 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [types-aiobotocore-mediapackage-vod docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/README.md` & `types-aiobotocore-mediapackage-vod-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage-vod)](https://pepy.tech/project/types-aiobotocore-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackageVod 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[aiobotocore.MediaPackageVod 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [types-aiobotocore-mediapackage-vod docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/setup.py` & `types-aiobotocore-mediapackage-vod-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediapackage-vod",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediapackage_vod"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaPackageVod 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaPackageVod 2.9.1 service generated with"
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
     keywords="aiobotocore mediapackage-vod type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediapackage_vod": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__init__.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListAssetsPaginator,
     ListPackagingConfigurationsPaginator,
     ListPackagingGroupsPaginator,
 )
 
 Client = MediaPackageVodClient
 
-
 __all__ = (
     "Client",
     "ListAssetsPaginator",
     "ListPackagingConfigurationsPaginator",
     "ListPackagingGroupsPaginator",
     "MediaPackageVodClient",
 )
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__init__.pyi` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/__main__.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaPackageVod 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaPackageVod 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod\nOther"
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

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/client.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaPackageVodClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,15 +123,15 @@
         self,
         *,
         Id: str,
         PackagingGroupId: str,
         SourceArn: str,
         SourceRoleArn: str,
         ResourceId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAssetResponseTypeDef:
         """
         Creates a new MediaPackage VOD Asset resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_asset)
         """
@@ -142,30 +141,30 @@
         *,
         Id: str,
         PackagingGroupId: str,
         CmafPackage: CmafPackageTypeDef = ...,
         DashPackage: DashPackageTypeDef = ...,
         HlsPackage: HlsPackageTypeDef = ...,
         MssPackage: MssPackageTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_configuration)
         """
 
     async def create_packaging_group(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         EgressAccessLogs: EgressAccessLogsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePackagingGroupResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingGroup resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_group)
         """
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/client.pyi` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self,
         *,
         Id: str,
         PackagingGroupId: str,
         SourceArn: str,
         SourceRoleArn: str,
         ResourceId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAssetResponseTypeDef:
         """
         Creates a new MediaPackage VOD Asset resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_asset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_asset)
         """
@@ -138,30 +138,30 @@
         *,
         Id: str,
         PackagingGroupId: str,
         CmafPackage: CmafPackageTypeDef = ...,
         DashPackage: DashPackageTypeDef = ...,
         HlsPackage: HlsPackageTypeDef = ...,
         MssPackage: MssPackageTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePackagingConfigurationResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingConfiguration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_configuration)
         """
 
     async def create_packaging_group(
         self,
         *,
         Id: str,
         Authorization: AuthorizationTypeDef = ...,
         EgressAccessLogs: EgressAccessLogsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreatePackagingGroupResponseTypeDef:
         """
         Creates a new MediaPackage VOD PackagingGroup resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client.create_packaging_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/client/#create_packaging_group)
         """
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/literals.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/literals.py`

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
     "AdMarkersType",
     "EncryptionMethodType",
     "ListAssetsPaginatorName",
     "ListPackagingConfigurationsPaginatorName",
     "ListPackagingGroupsPaginatorName",
     "ManifestLayoutType",
@@ -37,15 +36,14 @@
     "MediaPackageVodServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdMarkersType = Literal["NONE", "PASSTHROUGH", "SCTE35_ENHANCED"]
 EncryptionMethodType = Literal["AES_128", "SAMPLE_AES"]
 ListAssetsPaginatorName = Literal["list_assets"]
 ListPackagingConfigurationsPaginatorName = Literal["list_packaging_configurations"]
 ListPackagingGroupsPaginatorName = Literal["list_packaging_groups"]
 ManifestLayoutType = Literal["COMPACT", "FULL"]
 PeriodTriggersElementType = Literal["ADS"]
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/literals.pyi` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/paginator.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 __all__ = (
     "ListAssetsPaginator",
     "ListPackagingConfigurationsPaginator",
     "ListPackagingGroupsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/paginator.pyi` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/type_defs.py` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssetShallowTypeDef",
     "AuthorizationTypeDef",
     "EgressAccessLogsTypeDef",
     "ResponseMetadataTypeDef",
     "CreateAssetRequestRequestTypeDef",
     "EgressEndpointTypeDef",
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod/type_defs.pyi` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediapackage-vod
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaPackageVod 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaPackageVod 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/
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
 
 <a id="types-aiobotocore-mediapackage-vod"></a>
 
 # types-aiobotocore-mediapackage-vod
 
 [![PyPI - types-aiobotocore-mediapackage-vod](https://img.shields.io/pypi/v/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediapackage-vod.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediapackage-vod)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediapackage-vod)](https://pepy.tech/project/types-aiobotocore-mediapackage-vod)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaPackageVod 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
+[aiobotocore.MediaPackageVod 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
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
 [types-aiobotocore-mediapackage-vod docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediapackage_vod/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediapackage-vod-2.9.0/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt` & `types-aiobotocore-mediapackage-vod-2.9.1/types_aiobotocore_mediapackage_vod.egg-info/SOURCES.txt`

 * *Files identical despite different names*
