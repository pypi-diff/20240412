# Comparing `tmp/fastapi_htmx-0.4.1.tar.gz` & `tmp/fastapi_htmx-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_htmx-0.4.1.tar", max compression
+gzip compressed data, was "fastapi_htmx-0.4.2.tar", max compression
```

## Comparing `fastapi_htmx-0.4.1.tar` & `fastapi_htmx-0.4.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    13560 2024-01-21 22:13:22.867820 fastapi_htmx-0.4.1/README.md
--rw-r--r--   0        0        0      217 2024-01-12 22:34:14.120720 fastapi_htmx-0.4.1/fastapi_htmx/__init__.py
--rw-r--r--   0        0        0     7607 2024-01-12 23:24:48.161405 fastapi_htmx-0.4.1/fastapi_htmx/htmx.py
--rw-r--r--   0        0        0        0 2023-11-10 20:43:04.716939 fastapi_htmx-0.4.1/fastapi_htmx/py.typed
--rw-r--r--   0        0        0     2359 2024-01-21 22:14:18.206458 fastapi_htmx-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    15059 1970-01-01 00:00:00.000000 fastapi_htmx-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     7452 2023-11-10 20:43:04.716939 fastapi_htmx-0.4.2/LICENCE.md
+-rw-r--r--   0        0        0    13560 2024-04-12 06:53:01.178397 fastapi_htmx-0.4.2/README.md
+-rw-r--r--   0        0        0      217 2024-04-12 06:53:01.178397 fastapi_htmx-0.4.2/fastapi_htmx/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-12 06:53:01.178397 fastapi_htmx-0.4.2/fastapi_htmx/htmx.py
+-rw-r--r--   0        0        0        0 2023-11-10 20:43:04.716939 fastapi_htmx-0.4.2/fastapi_htmx/py.typed
+-rw-r--r--   0        0        0     2371 2024-04-12 06:58:07.034210 fastapi_htmx-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    15059 1970-01-01 00:00:00.000000 fastapi_htmx-0.4.2/PKG-INFO
```

### Comparing `fastapi_htmx-0.4.1/README.md` & `fastapi_htmx-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_htmx-0.4.1/fastapi_htmx/htmx.py` & `fastapi_htmx-0.4.2/fastapi_htmx/htmx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Extension for FastAPI to make HTMX easier to use."""
+
 import inspect
 import logging
 from collections.abc import Callable, Mapping
 from dataclasses import dataclass
 from functools import wraps
 from typing import Dict, Optional, Union
 
@@ -104,14 +105,15 @@
 
     Raises:
         MissingFullPageTemplateError: If a full page is required bu no template is specified.
         MissingHTMXInitError: FastAPI-HTMX needs to be initialized for templates to work.
 
     Returns:
         Callable: The decorated function.
+
     """  # noqa: D401
 
     def htmx_decorator(func):  # noqa: C901
         @wraps(func)
         async def wrapper(*args, request: Request, **kwargs) -> Callable:  # noqa: C901
             request_is_fullpage_request = _is_fullpage_request(request=request)
             # hint: use `HXRequest` instead of `Request` for typing when using `request.hx_request`
@@ -177,12 +179,13 @@
 def htmx_init(templates: TemplatePath, file_extension: str = "jinja2"):
     """Initialize the HTMX extension.
 
     Args:
         templates (TemplatePath): The configured template instance to use.
                                   Or multiple template collections distinguished by a key.
         file_extension: (str): The file extension to use for all templates. Can be individually overriden.
+
     """
     global templates_path
     templates_path = templates
     global templates_file_extension
     templates_file_extension = file_extension
```

### Comparing `fastapi_htmx-0.4.1/pyproject.toml` & `fastapi_htmx-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-htmx"
-version = "0.4.1"
+version = "0.4.2"
 description = "Extension for FastAPI to make HTMX easier to use."
 authors = ["maces <fastapi-htmx@mzip.de>"]
 license = "LGPL"
 readme = "README.md"
 homepage = "https://github.com/maces/fastapi-htmx"
 keywords = ["fastapi", "htmx", "html", "jinja2"]
 classifiers = [
@@ -36,25 +36,25 @@
 packages = [
     {include = "fastapi_htmx"},
     {include = "fastapi_htmx/py.typed"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-fastapi = ">=0.94,<0.110"
+fastapi = ">=0.94,<0.111"
 jinja2 = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
-ruff = ">=0.0.254,<0.1.14"
-black = "^23.1.0"
+ruff = ">=0.0.254,<0.3.6"
+black = ">=23.1,<25.0"
 mypy = "^1.1.1"
 pre-commit = "^3.1.1"
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
-httpx = ">=0.23.3,<0.27.0"
+pytest = ">=7.2.2,<9.0.0"
+pytest-cov = ">=4,<6"
+httpx = ">=0.23.3,<0.28.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `fastapi_htmx-0.4.1/PKG-INFO` & `fastapi_htmx-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-htmx
-Version: 0.4.1
+Version: 0.4.2
 Summary: Extension for FastAPI to make HTMX easier to use.
 Home-page: https://github.com/maces/fastapi-htmx
 License: LGPL
 Keywords: fastapi,htmx,html,jinja2
 Author: maces
 Author-email: fastapi-htmx@mzip.de
 Requires-Python: >=3.8,<4.0
@@ -27,15 +27,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: fastapi (>=0.94,<0.110)
+Requires-Dist: fastapi (>=0.94,<0.111)
 Requires-Dist: jinja2 (>=3.1,<4.0)
 Description-Content-Type: text/markdown
 
 # FastAPI-HTMX
 
 Extension for FastAPI to make HTMX easier to use.
```

