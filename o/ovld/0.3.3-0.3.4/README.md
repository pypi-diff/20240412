# Comparing `tmp/ovld-0.3.3.tar.gz` & `tmp/ovld-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovld-0.3.3.tar", max compression
+gzip compressed data, was "ovld-0.3.4.tar", max compression
```

## Comparing `ovld-0.3.3.tar` & `ovld-0.3.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.3/LICENSE
--rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.3/README.md
--rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.3/ovld/__init__.py
--rw-r--r--   0        0        0    32571 2024-04-11 02:33:40.735176 ovld-0.3.3/ovld/core.py
--rw-r--r--   0        0        0     5006 2020-08-22 00:43:34.764268 ovld-0.3.3/ovld/mro.py
--rw-r--r--   0        0        0     3521 2024-04-10 21:30:36.965589 ovld-0.3.3/ovld/utils.py
--rw-r--r--   0        0        0       18 2024-04-12 15:14:21.206118 ovld-0.3.3/ovld/version.py
--rw-r--r--   0        0        0      906 2024-04-12 15:14:21.182667 ovld-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9439 1970-01-01 00:00:00.000000 ovld-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.4/LICENSE
+-rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.4/README.md
+-rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.4/ovld/__init__.py
+-rw-r--r--   0        0        0    33078 2024-04-12 18:44:42.542358 ovld-0.3.4/ovld/core.py
+-rw-r--r--   0        0        0     5006 2024-04-12 16:00:16.628660 ovld-0.3.4/ovld/mro.py
+-rw-r--r--   0        0        0     3861 2024-04-12 16:08:27.619178 ovld-0.3.4/ovld/utils.py
+-rw-r--r--   0        0        0       18 2024-04-12 18:59:54.328025 ovld-0.3.4/ovld/version.py
+-rw-r--r--   0        0        0      906 2024-04-12 18:59:54.304605 ovld-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9439 1970-01-01 00:00:00.000000 ovld-0.3.4/PKG-INFO
```

### Comparing `ovld-0.3.3/LICENSE` & `ovld-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovld-0.3.3/README.md` & `ovld-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ovld-0.3.3/ovld/core.py` & `ovld-0.3.4/ovld/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,26 @@
 import itertools
 import math
 import textwrap
 import typing
 from types import FunctionType
 
 try:
-    from types import UnionType
+    from types import GenericAlias, UnionType
 except ImportError:  # pragma: no cover
     UnionType = None
 
+    class GenericAliasMC(type):
+        def __instancecheck__(cls, obj):
+            return hasattr(obj, "__origin__")
+
+    class GenericAlias(metaclass=GenericAliasMC):
+        pass
+
+
 from .mro import compose_mro
 from .utils import BOOTSTRAP, MISSING, keyword_decorator
 
 
 def is_type_of_type(t):
     return getattr(t, "__origin__", None) is type
 
@@ -35,29 +43,36 @@
 
     def __init__(self):
         self.entries = {}
         self.types = set()
 
     def register(self, obj_t, handler):
         """Register a handler for the given object type."""
+        if isinstance(obj_t, str):
+            obj_t = eval(obj_t, getattr(handler[0], "__globals__", {}))
+
         self.clear()
-        if not is_type_of_type(obj_t):
+        if is_type_of_type(obj_t):
+            self.types.add(obj_t.__args__[0])
+        else:
             self.types.add(obj_t)
         s = self.entries.setdefault(obj_t, set())
         s.add(handler)
 
     def __missing__(self, obj_t):
         """Get the handler for the given type.
 
         The result is cached so that the normal dict getitem will find it
         the next time getitem is called.
         """
         results = {}
         if is_type_of_type(obj_t):
             mro = [type[t] for t in compose_mro(obj_t.__args__[0], self.types)]
+            mro.append(type)
+            mro.append(object)
         else:
             mro = compose_mro(obj_t, self.types)
         for lvl, cls in enumerate(reversed(mro)):
             handlers = self.entries.get(cls, None)
             if handlers:
                 results.update({h: lvl for h in handlers})
 
@@ -89,15 +104,17 @@
 
     def __init__(self, key_error=KeyError):
         self.maps = {}
         self.empty = MISSING
         self.key_error = key_error
 
     def transform(self, obj):
-        if isinstance(obj, type):
+        if isinstance(obj, GenericAlias):
+            return type[obj.__origin__]
+        elif isinstance(obj, type):
             return type[obj]
         else:
             return type(obj)
 
     def register(self, obj_t_tup, nargs, handler):
         """Register a handler for a tuple of argument types.
```

### Comparing `ovld-0.3.3/ovld/mro.py` & `ovld-0.3.4/ovld/mro.py`

 * *Files identical despite different names*

### Comparing `ovld-0.3.3/ovld/utils.py` & `ovld-0.3.4/ovld/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Miscellaneous utilities."""
 
 import functools
 import sys
+from dataclasses import dataclass
+from typing import Protocol, runtime_checkable
 
 
 class Named:
     """A named object.
 
     This class can be used to construct objects with a name that will be used
     for the string representation.
@@ -139,17 +141,28 @@
     @meta
     def check(cls):
         return all(hasattr(cls, a) for a in attrs)
 
     return check
 
 
+@runtime_checkable
+@dataclass
+class Dataclass(Protocol):
+    @classmethod
+    def __subclasshook__(cls, subclass):
+        return hasattr(subclass, "__dataclass_fields__") and hasattr(
+            subclass, "__dataclass_params__"
+        )
+
+
 __all__ = [
     "BOOTSTRAP",
     "MISSING",
+    "Dataclass",
     "Named",
     "deferred",
     "exactly",
     "has_attribute",
     "meta",
     "keyword_decorator",
     "strict_subclass",
```

### Comparing `ovld-0.3.3/pyproject.toml` & `ovld-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ovld"
-version = "0.3.3"
+version = "0.3.4"
 description = "Overloading Python functions"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/breuleux/ovld"
 repository = "https://github.com/breuleux/ovld"
```

### Comparing `ovld-0.3.3/PKG-INFO` & `ovld-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovld
-Version: 0.3.3
+Version: 0.3.4
 Summary: Overloading Python functions
 Home-page: https://github.com/breuleux/ovld
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

