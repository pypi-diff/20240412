# Comparing `tmp/fasted-0.2404.1.tar.gz` & `tmp/fasted-0.2404.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasted-0.2404.1.tar", max compression
+gzip compressed data, was "fasted-0.2404.2.tar", max compression
```

## Comparing `fasted-0.2404.1.tar` & `fasted-0.2404.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-04-08 06:59:48.497295 fasted-0.2404.1/LICENSE
--rw-r--r--   0        0        0     4028 2024-04-08 06:59:48.497295 fasted-0.2404.1/README.md
--rw-r--r--   0        0        0      103 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/__init__.py
--rw-r--r--   0        0        0     1211 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/idmemo.py
--rw-r--r--   0        0        0        0 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/py.typed
--rw-r--r--   0        0        0     7118 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/selfdependent.py
--rw-r--r--   0        0        0      586 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/typing.py
--rw-r--r--   0        0        0     1114 2024-04-08 06:59:48.501295 fasted-0.2404.1/fasted/utils.py
--rw-r--r--   0        0        0     1431 2024-04-08 06:59:48.501295 fasted-0.2404.1/pyproject.toml
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 fasted-0.2404.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-12 20:29:09.906325 fasted-0.2404.2/LICENSE
+-rw-r--r--   0        0        0     4036 2024-04-12 20:29:09.906325 fasted-0.2404.2/README.md
+-rw-r--r--   0        0        0      103 2024-04-12 20:29:09.906325 fasted-0.2404.2/fasted/__init__.py
+-rw-r--r--   0        0        0     1211 2024-04-12 20:29:09.906325 fasted-0.2404.2/fasted/idmemo.py
+-rw-r--r--   0        0        0        0 2024-04-12 20:29:09.906325 fasted-0.2404.2/fasted/py.typed
+-rw-r--r--   0        0        0     7139 2024-04-12 20:29:09.910325 fasted-0.2404.2/fasted/selfdependent.py
+-rw-r--r--   0        0        0      586 2024-04-12 20:29:09.910325 fasted-0.2404.2/fasted/typing.py
+-rw-r--r--   0        0        0     1114 2024-04-12 20:29:09.910325 fasted-0.2404.2/fasted/utils.py
+-rw-r--r--   0        0        0     1431 2024-04-12 20:29:09.910325 fasted-0.2404.2/pyproject.toml
+-rw-r--r--   0        0        0     4557 1970-01-01 00:00:00.000000 fasted-0.2404.2/PKG-INFO
```

### Comparing `fasted-0.2404.1/LICENSE` & `fasted-0.2404.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fasted-0.2404.1/README.md` & `fasted-0.2404.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 - **Decorated** instance **methods will behave as expected** if called directly.
 
 Example use:
 
 ```python
 from typing import Annotated
 
-from fastapi import FastAPI, Depends
+from fastapi import Depends, FastAPI
 from fasted import selfdependent
 
 
 def double() -> "Multiplier":
     # Dependency that returns a Multiplier with base = 2.
     return Multiplier(2)
 
@@ -53,15 +53,15 @@
 
     @selfdependent()
     def multiply(self, mul: float) -> float:
         # `__init__()` will be used as the dependency to create `self`, so the route
         # where this method is used will have a `base` and a `mul` query parameter.
         return self.base * mul
 
-    @selfdependent(double)
+    @selfdependent(factory=double)
     async def double(self, mul: float) -> float:
         # `double()` will be used as the dependency to create `self`, so the route
         # where this method is used will only have a `mul` query parameter.
         return self.base * mul
 
 
 app = FastAPI()
```

### Comparing `fasted-0.2404.1/fasted/idmemo.py` & `fasted-0.2404.2/fasted/idmemo.py`

 * *Files identical despite different names*

### Comparing `fasted-0.2404.1/fasted/selfdependent.py` & `fasted-0.2404.2/fasted/selfdependent.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,25 +183,28 @@
         )
 
         return self._memo.store(hcurrent, result)
 
 
 @overload
 def selfdependent(
+    *,
     factory: None = None,
 ) -> Callable[[BoundMethod[TOwner, TParams, TResult]], BoundMethod[TOwner, TParams, TResult]]: ...
 
 
 @overload
 def selfdependent(
+    *,
     factory: Dependency[TOwner],
 ) -> Callable[[BoundMethod[TOwner, TParams, TResult]], BoundMethod[TOwner, TParams, TResult]]: ...
 
 
 def selfdependent(
+    *,
     factory: Dependency[TOwner] | None = None,
 ) -> Callable[[BoundMethod[TOwner, TParams, TResult]], BoundMethod[TOwner, TParams, TResult]]:
     """
     Decorator that converts an instance method into a FastAPI dependency using a `SelfDependent` descriptor.
 
     Arguments:
         factory: An optional factory (and FastAPI dependency) that can be wrapped in `Depends()`
```

### Comparing `fasted-0.2404.1/fasted/typing.py` & `fasted-0.2404.2/fasted/typing.py`

 * *Files identical despite different names*

### Comparing `fasted-0.2404.1/fasted/utils.py` & `fasted-0.2404.2/fasted/utils.py`

 * *Files identical despite different names*

### Comparing `fasted-0.2404.1/pyproject.toml` & `fasted-0.2404.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fasted"
-version = "0.2404.1"
+version = "0.2404.2"
 description = "FastAPI dependencies and utilities."
 authors = ["Peter Volf <do.volfp@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fasted-0.2404.1/PKG-INFO` & `fasted-0.2404.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasted
-Version: 0.2404.1
+Version: 0.2404.2
 Summary: FastAPI dependencies and utilities.
 License: MIT
 Author: Peter Volf
 Author-email: do.volfp@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,15 +50,15 @@
 - **Decorated** instance **methods will behave as expected** if called directly.
 
 Example use:
 
 ```python
 from typing import Annotated
 
-from fastapi import FastAPI, Depends
+from fastapi import Depends, FastAPI
 from fasted import selfdependent
 
 
 def double() -> "Multiplier":
     # Dependency that returns a Multiplier with base = 2.
     return Multiplier(2)
 
@@ -69,15 +69,15 @@
 
     @selfdependent()
     def multiply(self, mul: float) -> float:
         # `__init__()` will be used as the dependency to create `self`, so the route
         # where this method is used will have a `base` and a `mul` query parameter.
         return self.base * mul
 
-    @selfdependent(double)
+    @selfdependent(factory=double)
     async def double(self, mul: float) -> float:
         # `double()` will be used as the dependency to create `self`, so the route
         # where this method is used will only have a `mul` query parameter.
         return self.base * mul
 
 
 app = FastAPI()
```

