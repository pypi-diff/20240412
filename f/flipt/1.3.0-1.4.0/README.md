# Comparing `tmp/flipt-1.3.0.tar.gz` & `tmp/flipt-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-1.3.0.tar", max compression
+gzip compressed data, was "flipt-1.4.0.tar", max compression
```

## Comparing `flipt-1.3.0.tar` & `flipt-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1197 2024-03-22 17:29:36.969731 flipt-1.3.0/README.md
--rw-r--r--   0        0        0      138 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/__init__.py
--rw-r--r--   0        0        0      625 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/async_client.py
--rw-r--r--   0        0        0      614 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/authentication/__init__.py
--rw-r--r--   0        0        0      744 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/evaluation/__init__.py
--rw-r--r--   0        0        0     2207 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/evaluation/async_evaluation_client.py
--rw-r--r--   0        0        0     2108 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/evaluation/models.py
--rw-r--r--   0        0        0     2143 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/evaluation/sync_evaluation_client.py
--rw-r--r--   0        0        0      368 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/exceptions.py
--rw-r--r--   0        0        0      252 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/flags/__init__.py
--rw-r--r--   0        0        0     1945 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/flags/async_flag_client.py
--rw-r--r--   0        0        0      701 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/flags/models.py
--rw-r--r--   0        0        0     1897 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/flags/sync_flag_client.py
--rw-r--r--   0        0        0      567 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/models.py
--rw-r--r--   0        0        0        0 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/py.typed
--rw-r--r--   0        0        0      590 2024-03-22 17:29:36.969731 flipt-1.3.0/flipt/sync_client.py
--rw-r--r--   0        0        0     1977 2024-03-22 17:29:36.969731 flipt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1684 1970-01-01 00:00:00.000000 flipt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1196 2024-04-12 00:32:10.026564 flipt-1.4.0/README.md
+-rw-r--r--   0        0        0      138 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/async_client.py
+-rw-r--r--   0        0        0      614 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/authentication/__init__.py
+-rw-r--r--   0        0        0      744 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/evaluation/__init__.py
+-rw-r--r--   0        0        0     2297 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/evaluation/async_evaluation_client.py
+-rw-r--r--   0        0        0     2108 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/evaluation/models.py
+-rw-r--r--   0        0        0     2233 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/evaluation/sync_evaluation_client.py
+-rw-r--r--   0        0        0      368 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/exceptions.py
+-rw-r--r--   0        0        0      252 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/flags/__init__.py
+-rw-r--r--   0        0        0     2035 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/flags/async_flag_client.py
+-rw-r--r--   0        0        0      701 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/flags/models.py
+-rw-r--r--   0        0        0     1987 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/flags/sync_flag_client.py
+-rw-r--r--   0        0        0      567 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/models.py
+-rw-r--r--   0        0        0        0 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/py.typed
+-rw-r--r--   0        0        0      655 2024-04-12 00:32:10.026564 flipt-1.4.0/flipt/sync_client.py
+-rw-r--r--   0        0        0     1981 2024-04-12 00:32:10.026564 flipt-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 flipt-1.4.0/PKG-INFO
```

### Comparing `flipt-1.3.0/README.md` & `flipt-1.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Flipt Python
 
 [![pypi](https://img.shields.io/pypi/v/flipt.svg)](https://pypi.org/project/flipt)
 
+
 This directory contains the Python source code for the Flipt [server-side](https://www.flipt.io/docs/integration/server/rest) client.
 
 ## Documentation
 
 API documentation is available at <https://www.flipt.io/docs/reference/overview>.
 
 ## Installation
@@ -34,14 +35,13 @@
 )
 
 print(variant_flag)
 ```
 
 There is a more detailed example in the [examples](./examples) directory.
 
-
 ## For developers
 
 After adding new code, please don't forget to add unit tests for new features.
-To format the code, check it with linters and run tests, use the `make check` command. 
+To format the code, check it with linters and run tests, use the `make check` command.
 
 Please keep the Python [PEP8](https://peps.python.org/pep-0008/) in mind while adding new code.
```

### Comparing `flipt-1.3.0/flipt/async_client.py` & `flipt-1.4.0/flipt/async_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from .flags import AsyncFlag
 
 
 class AsyncFliptClient:
     def __init__(
         self,
         url: str = "http://localhost:8080",
+        headers: dict[str, str] | None = None,
         timeout: int = 60,
         authentication: AuthenticationStrategy | None = None,
     ):
         self.httpx_client = httpx.AsyncClient(timeout=timeout)
 
-        self.evaluation = AsyncEvaluation(url, authentication, self.httpx_client)
-        self.flag = AsyncFlag(url, authentication, self.httpx_client)
+        self.evaluation = AsyncEvaluation(url, headers, authentication, self.httpx_client)
+        self.flag = AsyncFlag(url, headers, authentication, self.httpx_client)
 
     async def close(self) -> None:
         await self.httpx_client.aclose()
```

### Comparing `flipt-1.3.0/flipt/authentication/__init__.py` & `flipt-1.4.0/flipt/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `flipt-1.3.0/flipt/evaluation/__init__.py` & `flipt-1.4.0/flipt/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `flipt-1.3.0/flipt/evaluation/async_evaluation_client.py` & `flipt-1.4.0/flipt/evaluation/async_evaluation_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,23 @@
 )
 
 
 class AsyncEvaluation:
     def __init__(
         self,
         url: str,
+        headers: dict[str, str] | None = None,
         authentication: AuthenticationStrategy | None = None,
         httpx_client: httpx.AsyncClient | None = None,
     ):
         self.url = url
-        self.headers: dict[str, str] = {}
+
+        if headers is None:
+            headers = {}
+        self.headers = headers
 
         self._client = httpx_client or httpx.AsyncClient()
 
         if authentication:
             authentication.authenticate(self.headers)
 
     async def close(self) -> None:
```

### Comparing `flipt-1.3.0/flipt/evaluation/models.py` & `flipt-1.4.0/flipt/evaluation/models.py`

 * *Files identical despite different names*

### Comparing `flipt-1.3.0/flipt/evaluation/sync_evaluation_client.py` & `flipt-1.4.0/flipt/evaluation/sync_evaluation_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,23 @@
 )
 
 
 class Evaluation:
     def __init__(
         self,
         url: str,
+        headers: dict[str, str] | None = None,
         authentication: AuthenticationStrategy | None = None,
         httpx_client: httpx.Client | None = None,
     ):
         self.url = url
-        self.headers: dict[str, str] = {}
+
+        if headers is None:
+            headers = {}
+        self.headers = headers
 
         self._client = httpx_client or httpx.Client()
 
         if authentication:
             authentication.authenticate(self.headers)
 
     def close(self) -> None:
```

### Comparing `flipt-1.3.0/flipt/flags/async_flag_client.py` & `flipt-1.4.0/flipt/flags/async_flag_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 from .models import Flag, ListFlagsResponse
 
 
 class AsyncFlag:
     def __init__(
         self,
         url: str,
+        headers: dict[str, str] | None = None,
         authentication: AuthenticationStrategy | None = None,
         httpx_client: httpx.AsyncClient | None = None,
     ):
         self.url = url
-        self.headers: dict[str, str] = {}
+
+        if headers is None:
+            headers = {}
+        self.headers = headers
 
         self._client = httpx_client or httpx.AsyncClient()
 
         if authentication:
             authentication.authenticate(self.headers)
 
     async def close(self) -> None:
```

### Comparing `flipt-1.3.0/flipt/flags/models.py` & `flipt-1.4.0/flipt/flags/models.py`

 * *Files identical despite different names*

### Comparing `flipt-1.3.0/flipt/flags/sync_flag_client.py` & `flipt-1.4.0/flipt/flags/sync_flag_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 from .models import Flag, ListFlagsResponse
 
 
 class SyncFlag:
     def __init__(
         self,
         url: str,
+        headers: dict[str, str] | None = None,
         authentication: AuthenticationStrategy | None = None,
         httpx_client: httpx.Client | None = None,
     ):
         self.url = url
-        self.headers: dict[str, str] = {}
+
+        if headers is None:
+            headers = {}
+        self.headers = headers
 
         self._client = httpx_client or httpx.Client()
 
         if authentication:
             authentication.authenticate(self.headers)
 
     def close(self) -> None:
```

### Comparing `flipt-1.3.0/flipt/models.py` & `flipt-1.4.0/flipt/models.py`

 * *Files identical despite different names*

### Comparing `flipt-1.3.0/flipt/sync_client.py` & `flipt-1.4.0/flipt/sync_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from .flags import SyncFlag
 
 
 class FliptClient:
     def __init__(
         self,
         url: str = "http://localhost:8080",
+        headers: dict[str, str] | None = None,
         timeout: int = 60,
         authentication: AuthenticationStrategy | None = None,
     ):
         self.httpx_client = httpx.Client(timeout=timeout)
 
-        self.evaluation = Evaluation(url, authentication, self.httpx_client)
-        self.flag = SyncFlag(url, authentication, self.httpx_client)
+        self.evaluation = Evaluation(url, headers, authentication, self.httpx_client)
+        self.flag = SyncFlag(url, headers, authentication, self.httpx_client)
 
     def close(self) -> None:
         self.httpx_client.close()
```

### Comparing `flipt-1.3.0/pyproject.toml` & `flipt-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flipt"
-version = "1.3.0"
+version = "1.4.0"
 description = "Flipt Server SDK"
 authors = ["Flipt Devs <dev@flipt.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -12,15 +12,15 @@
 httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.12.1,<25.0.0"
 mypy = "^1.8.0"
 pytest = "^8.0.1"
 pytest-asyncio = "^0.23.5"
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-httpx = "^0.30.0"
 pytest-mock = "^3.12.0"
 ruff = ">=0.2.2,<0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
@@ -45,15 +45,15 @@
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 
 [tool.coverage.report]
 precision = 1
-fail_under = 95
+fail_under = 90
 exclude_also = [
     "raise NotImplementedError",
     "pragma: no cover",
     "if TYPE_CHECKING:",
     "def __repr__",
 ]
 show_missing = true
```

### Comparing `flipt-1.3.0/PKG-INFO` & `flipt-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipt
-Version: 1.3.0
+Version: 1.4.0
 Summary: Flipt Server SDK
 License: MIT
 Author: Flipt Devs
 Author-email: dev@flipt.io
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,15 @@
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Flipt Python
 
 [![pypi](https://img.shields.io/pypi/v/flipt.svg)](https://pypi.org/project/flipt)
 
+
 This directory contains the Python source code for the Flipt [server-side](https://www.flipt.io/docs/integration/server/rest) client.
 
 ## Documentation
 
 API documentation is available at <https://www.flipt.io/docs/reference/overview>.
 
 ## Installation
@@ -50,15 +51,14 @@
 )
 
 print(variant_flag)
 ```
 
 There is a more detailed example in the [examples](./examples) directory.
 
-
 ## For developers
 
 After adding new code, please don't forget to add unit tests for new features.
-To format the code, check it with linters and run tests, use the `make check` command. 
+To format the code, check it with linters and run tests, use the `make check` command.
 
 Please keep the Python [PEP8](https://peps.python.org/pep-0008/) in mind while adding new code.
```

