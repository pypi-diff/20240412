# Comparing `tmp/vellox-0.1.0.tar.gz` & `tmp/vellox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellox-0.1.0.tar", max compression
+gzip compressed data, was "vellox-0.1.1.tar", max compression
```

## Comparing `vellox-0.1.0.tar` & `vellox-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-04-12 11:55:05.542267 vellox-0.1.0/LICENSE
--rw-r--r--   0        0        0      978 2024-04-12 11:55:05.542267 vellox-0.1.0/README.md
--rw-r--r--   0        0        0      898 2024-04-12 11:55:05.542267 vellox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/__init__.py
--rw-r--r--   0        0        0     2691 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/adapter.py
--rw-r--r--   0        0        0      440 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/exceptions.py
--rw-r--r--   0        0        0      100 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/handlers/__init__.py
--rw-r--r--   0        0        0     2385 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/handlers/gcp.py
--rw-r--r--   0        0        0     1050 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/handlers/utils.py
--rw-r--r--   0        0        0      148 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/protocols/__init__.py
--rw-r--r--   0        0        0     4234 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/protocols/http.py
--rw-r--r--   0        0        0     7801 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/protocols/lifespan.py
--rw-r--r--   0        0        0        0 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/py.typed
--rw-r--r--   0        0        0     1274 2024-04-12 11:55:05.542267 vellox-0.1.0/vellox/types.py
--rw-r--r--   0        0        0     1838 1970-01-01 00:00:00.000000 vellox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-12 12:33:23.078842 vellox-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1209 2024-04-12 12:33:23.078842 vellox-0.1.1/README.md
+-rw-r--r--   0        0        0      928 2024-04-12 12:33:23.078842 vellox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-12 12:33:23.078842 vellox-0.1.1/vellox/__init__.py
+-rw-r--r--   0        0        0     2691 2024-04-12 12:33:23.078842 vellox-0.1.1/vellox/adapter.py
+-rw-r--r--   0        0        0      440 2024-04-12 12:33:23.078842 vellox-0.1.1/vellox/exceptions.py
+-rw-r--r--   0        0        0      100 2024-04-12 12:33:23.078842 vellox-0.1.1/vellox/handlers/__init__.py
+-rw-r--r--   0        0        0     2385 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/handlers/gcp.py
+-rw-r--r--   0        0        0     1050 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/handlers/utils.py
+-rw-r--r--   0        0        0      148 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/protocols/__init__.py
+-rw-r--r--   0        0        0     4234 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/protocols/http.py
+-rw-r--r--   0        0        0     7801 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/protocols/lifespan.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/py.typed
+-rw-r--r--   0        0        0     1298 2024-04-12 12:33:23.082843 vellox-0.1.1/vellox/types.py
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 vellox-0.1.1/PKG-INFO
```

### Comparing `vellox-0.1.0/LICENSE` & `vellox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/README.md` & `vellox-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Vellox
 
+<a href="https://pypi.org/project/vellox">
+    <img src="https://badge.fury.io/py/vellox.svg" alt="Package version">
+</a>
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/vellox.svg?style=flat-square">
+
 Vellox is an adapter for running [ASGI](https://asgi.readthedocs.io/en/latest) applications in GCP Cloud Functions.
 
 ## Requirements
 
 Python 3.8+
 
 ## Example
```

### Comparing `vellox-0.1.0/pyproject.toml` & `vellox-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vellox"
-version = "0.1.0"
+version = "0.1.1"
 description = "GCP Cloud Functions support for ASGI applications"
 authors = ["junah201 <junah.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://vellox.junah.dev"
 repository = "https://github.com/junah201/vellox"
 documentation = "https://vellox.junah.dev"
@@ -19,15 +19,16 @@
     "Programming Language :: Python :: 3.12",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 
-Flask = ">=2.0.2"
+Flask = "==2.2.5"
+typing_extensions = "==4.7.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `vellox-0.1.0/vellox/adapter.py` & `vellox-0.1.1/vellox/adapter.py`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/vellox/handlers/gcp.py` & `vellox-0.1.1/vellox/handlers/gcp.py`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/vellox/handlers/utils.py` & `vellox-0.1.1/vellox/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/vellox/protocols/http.py` & `vellox-0.1.1/vellox/protocols/http.py`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/vellox/protocols/lifespan.py` & `vellox-0.1.1/vellox/protocols/lifespan.py`

 * *Files identical despite different names*

### Comparing `vellox-0.1.0/vellox/types.py` & `vellox-0.1.1/vellox/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     Union,
     Sequence,
     MutableMapping,
     Awaitable,
     Callable,
     Literal,
     Protocol,
-    TypedDict,
-    TypeAlias,
+    TypedDict
 )
+from typing_extensions import TypeAlias
 
 import flask
 
 
 QueryParams: TypeAlias = MutableMapping[str, Union[str, Sequence[str]]]
 
 Headers: TypeAlias = List[List[bytes]]
```

### Comparing `vellox-0.1.0/PKG-INFO` & `vellox-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellox
-Version: 0.1.0
+Version: 0.1.1
 Summary: GCP Cloud Functions support for ASGI applications
 Home-page: https://vellox.junah.dev
 License: MIT
 Author: junah201
 Author-email: junah.dev@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,21 +12,27 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Flask (>=2.0.2)
+Requires-Dist: Flask (==2.2.5)
+Requires-Dist: typing_extensions (==4.7.1)
 Project-URL: Documentation, https://vellox.junah.dev
 Project-URL: Repository, https://github.com/junah201/vellox
 Description-Content-Type: text/markdown
 
 # Vellox
 
+<a href="https://pypi.org/project/vellox">
+    <img src="https://badge.fury.io/py/vellox.svg" alt="Package version">
+</a>
+<img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/vellox.svg?style=flat-square">
+
 Vellox is an adapter for running [ASGI](https://asgi.readthedocs.io/en/latest) applications in GCP Cloud Functions.
 
 ## Requirements
 
 Python 3.8+
 
 ## Example
```

