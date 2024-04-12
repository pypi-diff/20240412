# Comparing `tmp/ovld-0.3.2.tar.gz` & `tmp/ovld-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovld-0.3.2.tar", last modified: Mon Jun 21 23:00:08 2021, max compression
+gzip compressed data, was "ovld-0.3.3.tar", max compression
```

## Comparing `ovld-0.3.2.tar` & `ovld-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.2/LICENSE
--rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.2/README.md
--rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.2/ovld/__init__.py
--rw-r--r--   0        0        0    31667 2021-06-21 22:58:05.855902 ovld-0.3.2/ovld/core.py
--rw-r--r--   0        0        0     5006 2020-08-22 00:43:34.764268 ovld-0.3.2/ovld/mro.py
--rw-r--r--   0        0        0     3521 2020-11-29 23:41:24.318549 ovld-0.3.2/ovld/utils.py
--rw-r--r--   0        0        0       18 2021-06-21 22:59:59.760962 ovld-0.3.2/ovld/version.py
--rw-r--r--   0        0        0      748 2021-06-21 22:59:59.732804 ovld-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9622 2021-06-21 23:00:08.740478 ovld-0.3.2/setup.py
--rw-r--r--   0        0        0     9386 2021-06-21 23:00:08.741176 ovld-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2021-03-11 20:11:21.537259 ovld-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8758 2021-06-21 18:33:09.067471 ovld-0.3.3/README.md
+-rw-r--r--   0        0        0       85 2021-03-03 23:11:27.683713 ovld-0.3.3/ovld/__init__.py
+-rw-r--r--   0        0        0    32571 2024-04-11 02:33:40.735176 ovld-0.3.3/ovld/core.py
+-rw-r--r--   0        0        0     5006 2020-08-22 00:43:34.764268 ovld-0.3.3/ovld/mro.py
+-rw-r--r--   0        0        0     3521 2024-04-10 21:30:36.965589 ovld-0.3.3/ovld/utils.py
+-rw-r--r--   0        0        0       18 2024-04-12 15:14:21.206118 ovld-0.3.3/ovld/version.py
+-rw-r--r--   0        0        0      906 2024-04-12 15:14:21.182667 ovld-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9439 1970-01-01 00:00:00.000000 ovld-0.3.3/PKG-INFO
```

### Comparing `ovld-0.3.2/LICENSE` & `ovld-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovld-0.3.2/README.md` & `ovld-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ovld-0.3.2/ovld/core.py` & `ovld-0.3.3/ovld/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,27 @@
 import inspect
 import itertools
 import math
 import textwrap
 import typing
 from types import FunctionType
 
+try:
+    from types import UnionType
+except ImportError:  # pragma: no cover
+    UnionType = None
+
 from .mro import compose_mro
 from .utils import BOOTSTRAP, MISSING, keyword_decorator
 
 
+def is_type_of_type(t):
+    return getattr(t, "__origin__", None) is type
+
+
 class TypeMap(dict):
     """Represents a mapping from types to handlers.
 
     The mro of a type is considered when getting the handler, so setting the
     [object] key creates a default for all objects.
 
     typemap[some_type] returns a tuple of a handler and a "level" that
@@ -27,26 +36,30 @@
     def __init__(self):
         self.entries = {}
         self.types = set()
 
     def register(self, obj_t, handler):
         """Register a handler for the given object type."""
         self.clear()
-        self.types.add(obj_t)
+        if not is_type_of_type(obj_t):
+            self.types.add(obj_t)
         s = self.entries.setdefault(obj_t, set())
         s.add(handler)
 
     def __missing__(self, obj_t):
         """Get the handler for the given type.
 
         The result is cached so that the normal dict getitem will find it
         the next time getitem is called.
         """
         results = {}
-        mro = compose_mro(obj_t, self.types)
+        if is_type_of_type(obj_t):
+            mro = [type[t] for t in compose_mro(obj_t.__args__[0], self.types)]
+        else:
+            mro = compose_mro(obj_t, self.types)
         for lvl, cls in enumerate(reversed(mro)):
             handlers = self.entries.get(cls, None)
             if handlers:
                 results.update({h: lvl for h in handlers})
 
         if results:
             self[obj_t] = results
@@ -73,17 +86,22 @@
     less specific than [int, int], but it is neither less specific nor more
     specific than [object, int] (which means there is an ambiguity).
     """
 
     def __init__(self, key_error=KeyError):
         self.maps = {}
         self.empty = MISSING
-        self.transform = type
         self.key_error = key_error
 
+    def transform(self, obj):
+        if isinstance(obj, type):
+            return type[obj]
+        else:
+            return type(obj)
+
     def register(self, obj_t_tup, nargs, handler):
         """Register a handler for a tuple of argument types.
 
         Arguments:
             obj_t_tup: A tuple of argument types.
             nargs: A (amin, amax, varargs) tuple where amin is the minimum
                 number of arguments needed to match this tuple (if there are
@@ -322,14 +340,17 @@
                 self._dispatch = mixin._dispatch
         self.mixins += mixins
 
     def _sig_string(self, type_tuple):
         def clsname(cls):
             if cls is object:
                 return "*"
+            elif is_type_of_type(cls):
+                arg = clsname(cls.__args__[0])
+                return f"type[{arg}]"
             elif hasattr(cls, "__name__"):
                 return cls.__name__
             else:
                 return repr(cls)
 
         return ", ".join(map(clsname, type_tuple))
 
@@ -485,19 +506,23 @@
         return self
 
     def register(self, fn):
         """Register a function."""
 
         def _normalize_type(t, force_tuple=False):
             origin = getattr(t, "__origin__", None)
-            if origin is typing.Union:
+            if UnionType and isinstance(t, UnionType):
+                return _normalize_type(t.__args__)
+            elif origin is type:
+                return (t,) if force_tuple else t
+            elif origin is typing.Union:
                 return _normalize_type(t.__args__)
             elif origin is not None:
                 raise TypeError(
-                    "ovld does not accept generic types except Union or Optional"
+                    "ovld does not accept generic types except type, Union or Optional"
                 )
             elif isinstance(t, tuple):
                 return tuple(_normalize_type(t2) for t2 in t)
             elif force_tuple:
                 return (t,)
             else:
                 return t
@@ -919,15 +944,18 @@
         code_registry.update_cache_entry(self, self.code, new_code)
 
         self.code = new_code
 
 
 def rename_code(co, newname):  # pragma: no cover
     if hasattr(co, "replace"):
-        return co.replace(co_name=newname)
+        if hasattr(co, "co_qualname"):
+            return co.replace(co_name=newname, co_qualname=newname)
+        else:
+            return co.replace(co_name=newname)
     else:
         return type(co)(
             co.co_argcount,
             co.co_kwonlyargcount,
             co.co_nlocals,
             co.co_stacksize,
             co.co_flags,
```

### Comparing `ovld-0.3.2/ovld/mro.py` & `ovld-0.3.3/ovld/mro.py`

 * *Files identical despite different names*

### Comparing `ovld-0.3.2/ovld/utils.py` & `ovld-0.3.3/ovld/utils.py`

 * *Files identical despite different names*

### Comparing `ovld-0.3.2/pyproject.toml` & `ovld-0.3.3/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 [tool.poetry]
 name = "ovld"
-version = "0.3.2"
+version = "0.3.3"
 description = "Overloading Python functions"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/breuleux/ovld"
 repository = "https://github.com/breuleux/ovld"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-black = "^19.10b0"
-codefind = {version = "^0.1.0", python = "^3.8"}
+black = "^24.3.0"
+ruff = "^0.3.5"
+codefind = "^0.1.0"
 pytest = "^6.0.1"
-flake8 = "^3.8.3"
 pytest-cov = "^2.10.0"
-isort = "^5.4.2"
 
 [tool.black]
 line-length = 80
 
 [tool.isort]
 known_first_party = "ovld"
 known_third_party = ""
 multi_line_output = 3
 include_trailing_comma = true
 combine_as_imports = true
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry-core>=1.0.8"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 99
+
+[tool.ruff.lint]
+extend-select = ["I"]
+ignore = ["E241", "F722", "E501", "E203", "F811", "F821"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401", "F403"]
```

### Comparing `ovld-0.3.2/setup.py` & `ovld-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,331 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ovld
+Version: 0.3.3
+Summary: Overloading Python functions
+Home-page: https://github.com/breuleux/ovld
+License: MIT
+Author: Olivier Breuleux
+Author-email: breuleux@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/breuleux/ovld
+Description-Content-Type: text/markdown
 
-packages = \
-['ovld']
 
-package_data = \
-{'': ['*']}
+# Ovld
 
-setup_kwargs = {
-    'name': 'ovld',
-    'version': '0.3.2',
-    'description': 'Overloading Python functions',
-    'long_description': '\n# Ovld\n\nMultiple dispatch in Python, with some extra features.\n\nWith ovld, you can write a version of the same function for every type signature using annotations instead of writing an awkward sequence of `isinstance` statements. Unlike Python `singledispatch`, it works for multiple arguments.\n\nOther features of `ovld`:\n\n* Multiple dispatch for methods (with `metaclass=ovld.OvldMC`)\n* Create variants of functions\n* Built-in support for extensible, stateful recursion\n* Function wrappers\n* Function postprocessors\n* Nice stack traces\n\n## Example\n\nHere\'s a function that adds lists, tuples and dictionaries:\n\n```python\nfrom ovld import ovld\n\n@ovld\ndef add(x: list, y: list):\n    return [add(a, b) for a, b in zip(x, y)]\n\n@ovld\ndef add(x: tuple, y: tuple):\n    return tuple(add(a, b) for a, b in zip(x, y))\n\n@ovld\ndef add(x: dict, y: dict):\n    return {k: add(v, y[k]) for k, v in x.items()}\n\n@ovld\ndef add(x: object, y: object):\n    return x + y\n```\n\n## Bootstrapping and variants\n\nNow, there is another way to do this using ovld\'s *auto-bootstrapping*. Simply list `self` as the first argument to the function, and `self` will be bound to the function itself, so you can call `self(x, y)` for the recursion instead of `add(x, y)`:\n\n\n```python\n@ovld\ndef add(self, x: list, y: list):\n    return [self(a, b) for a, b in zip(x, y)]\n\n@ovld\ndef add(self, x: tuple, y: tuple):\n    return tuple(self(a, b) for a, b in zip(x, y))\n\n@ovld\ndef add(self, x: dict, y: dict):\n    return {k: self(v, y[k]) for k, v in x.items()}\n\n@ovld\ndef add(self, x: object, y: object):\n    return x + y\n```\n\nWhy is this useful, though? Observe:\n\n```python\n@add.variant\ndef mul(self, x: object, y: object):\n    return x * y\n\nassert add([1, 2], [3, 4]) == [4, 6]\nassert mul([1, 2], [3, 4]) == [3, 8]\n```\n\nA `variant` of a function is a copy which inherits all of the original\'s implementations but may define new ones. And because `self` is bound to the function that\'s called at the top level, the implementations for `list`, `tuple` and `dict` will bind `self` to `add` or `mul` depending on which one was called. You may also call `self.super(*args)` to invoke the parent implementation for that type.\n\n## State\n\nYou can pass `initial_state` to `@ovld` or `variant`. The initial state must be a function that takes no arguments. Its return value will be available in `self.state`. The state is initialized at the top level call, but recursive calls to `self` will preserve it.\n\nIn other words, you can do something like this:\n\n```python\n@add.variant(initial_state=lambda: 0)\ndef count(self, x, y):\n    self.state += 1\n    return (f"#{self.state}", x + y)\n\nassert count([1, 2, 3], [4, 5, 6]) == [("#1", 5), ("#2", 7), ("#3", 9)]\n```\n\nThe initial_state function can return any object and you can use the state to any purpose (e.g. cache or memoization).\n\n## Custom dispatch\n\nYou can define your own dispatching function. The dispatcher\'s first argument is always `self`.\n\n* `self.resolve(x, y)` to get the right function for the types of x and y\n* `self[type(x), type(y)]` will also return the right function for these types, but it works directly with the types.\n\nFor example, here is how you might define a function such that f(x) <=> f(x, x):\n\n```python\n@ovld.dispatch\ndef add_default(self, x, y=None):\n    if y is None:\n        y = x\n    return self.resolve(x, y)(x, y)\n\n@ovld\ndef add_default(x: int, y: int):\n    return x + y\n\n@ovld\ndef add_default(x: str, y: str):\n    return x + y\n\n@ovld\ndef add_default(xs: list, ys: list):\n    return [add_default(x, y) for x, y in zip(xs, ys)]\n\nassert add_default([1, 2, "alouette"]) == [2, 4, "alouettealouette"]\n```\n\nThere are other uses for this feature, e.g. memoization.\n\nThe normal functions may also have a `self`, which works the same as bootstrapping, and you can give an `initial_state` to `@ovld.dispatch` as well.\n\n## Postprocess\n\n`@ovld`, `@ovld.dispatch`, etc. take a `postprocess` argument which should be a function of one argument. That function will be called with the result of the call and must return the final result of the call.\n\nNote that intermediate, bootstrapped recursive calls (recursive calls using `self()`) will **not** be postprocessed (if you want to wrap these calls, you can do so otherwise, like defining a custom dispatch). Only the result of the top level call is postprocessed.\n\n## Methods\n\nUse the `OvldMC` metaclass to use multiple dispatch on methods. In this case there is no bootstrapping as described above and `self` is simply bound to the class instance.\n\n```python\nfrom ovld import OvldMC\n\nclass Cat(metaclass=OvldMC):\n    def interact(self, x: Mouse):\n        return "catch"\n\n    def interact(self, x: Food):\n        return "devour"\n\n    def interact(self, x: PricelessVase):\n        return "destroy"\n```\n\nSubclasses of `Cat` will inherit the overloaded `interact` and it may define additional overloaded methods which will only be valid for the subclass.\n\n**Note:** It is possible to use `ovld.dispatch` on methods, but in this case be aware that the first argument for the dispatch method will not be the usual `self` but an `OvldCall` object. The `self` can be retrived as `ovldcall.obj`. Here\'s an example to make it all clear:\n\n```python\nclass Stuff(metaclass=OvldMC):\n    def __init__(self, mul):\n        self.mul = mul\n\n    @ovld.dispatch\n    def calc(ovldcall, x):\n        # Wraps every call to self.calc, but we receive ovldcall instead of self\n        # ovldcall[type(x)] returns the right method to call\n        # ovldcall.obj is the self (the actual instance of Stuff)\n        return ovldcall[type(x)](x) * ovldcall.obj.mul\n\n    def calc(self, x: int):\n        return x + 1\n\n    def calc(self, xs: list):\n        return [self.calc(x) for x in xs]\n\nprint(Stuff(2).calc([1, 2, 3]))  # [4, 6, 8, 4, 6, 8]\n```\n\n### Mixins in subclasses\n\nThe `@extend_super` decorator on a method will combine the method with the definition on the superclass:\n\n```python\nfrom ovld import OvldMC, extend_super\n\nclass One(metaclass=OvldMC):\n    def f(self, x: int):\n        return "an integer"\n\nclass Two(One):\n    @extend_super\n    def f(self, x: str):\n        return "a string"\n\nassert Two().f(1) == "an integer"\nassert Two().f("s") == "a string"\n```\n\n## Ambiguous calls\n\nThe following definitions will cause a TypeError at runtime when called with two ints, because it is unclear which function is the right match:\n\n```python\n@ovld\ndef ambig(x: int, y: object):\n    print("io")\n\n@ovld\ndef ambig(x: object, y: int):\n    print("oi")\n\nambig(8, 8)  # ???\n```\n\nYou may define an additional function with signature (int, int) to disambiguate:\n\n```python\n@ovld\ndef ambig(x: int, y: int):\n    print("ii")\n```\n\n## Other features\n\n### meta\n\nTo test arbitrary conditions, you can use `meta`:\n\n```python\nfrom ovld import ovld, meta\n\n@meta\ndef StartsWithT(cls):\n    return cls.__name__.startswith("T")\n\n@ovld\ndef f(x: StartsWithT):\n    return "T"\n\nassert f(TypeError("xyz")) == "T"\n\n\n# Or: a useful example, since dataclasses have no common superclass:\n\nfrom dataclasses import dataclass, is_dataclass\n\n@dataclass\nclass Point:\n    x: int\n    y: int\n\n@ovld\ndef f(x: meta(is_dataclass)):\n    return "dataclass"\n\nassert f(Point(1, 2)) == "dataclass"\n```\n\n\n### deferred\n\nYou may define overloads for certain classes from external packages without\nhaving to import them:\n\n\n```python\nfrom ovld import ovld, deferred\n\n@ovld\ndef f(x: deferred("numpy.ndarray")):\n    return "ndarray"\n\n# numpy is not imported\nassert "numpy" not in sys.modules\n\n# But once we import it, the ovld works:\nimport numpy\nassert f(numpy.arange(10)) == "ndarray"\n```\n\n\n### Tracebacks\n\n`ovld` automagically renames functions so that the stack trace is more informative:\n\n```python\n@add.variant\ndef bad(self, x: object, y: object):\n    raise Exception("Bad.")\n\nbad([1], [2])\n\n"""\n  File "/Users/breuleuo/code/ovld/ovld/core.py", line 148, in bad.entry\n    res = ovc(*args, **kwargs)\n  File "/Users/breuleuo/code/ovld/ovld/core.py", line 182, in bad.dispatch\n    return method(self.bind_to, *args, **kwargs)\n  File "example.py", line 6, in bad[list, list]\n    return [self(a, b) for a, b in zip(x, y)]\n  File "example.py", line 6, in <listcomp>\n    return [self(a, b) for a, b in zip(x, y)]\n  File "/Users/breuleuo/code/ovld/ovld/core.py", line 182, in bad.dispatch\n    return method(self.bind_to, *args, **kwargs)\n  File "example.py", line 26, in bad[*, *]\n    raise Exception("Bad.")\n  Exception: Bad.\n"""\n```\n\nThe functions on the stack have names like `bad.entry`, `bad.dispatch`, `bad[list, list]` and `bad[*, *]` (`*` stands for `object`), which lets you better understand what happened just from the stack trace.\n\nThis also means profilers will be able to differentiate between these paths and between variants, even if they share code paths.\n',
-    'author': 'Olivier Breuleux',
-    'author_email': 'breuleux@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/breuleux/ovld',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.6,<4.0',
-}
+Multiple dispatch in Python, with some extra features.
 
+With ovld, you can write a version of the same function for every type signature using annotations instead of writing an awkward sequence of `isinstance` statements. Unlike Python `singledispatch`, it works for multiple arguments.
+
+Other features of `ovld`:
+
+* Multiple dispatch for methods (with `metaclass=ovld.OvldMC`)
+* Create variants of functions
+* Built-in support for extensible, stateful recursion
+* Function wrappers
+* Function postprocessors
+* Nice stack traces
+
+## Example
+
+Here's a function that adds lists, tuples and dictionaries:
+
+```python
+from ovld import ovld
+
+@ovld
+def add(x: list, y: list):
+    return [add(a, b) for a, b in zip(x, y)]
+
+@ovld
+def add(x: tuple, y: tuple):
+    return tuple(add(a, b) for a, b in zip(x, y))
+
+@ovld
+def add(x: dict, y: dict):
+    return {k: add(v, y[k]) for k, v in x.items()}
+
+@ovld
+def add(x: object, y: object):
+    return x + y
+```
+
+## Bootstrapping and variants
+
+Now, there is another way to do this using ovld's *auto-bootstrapping*. Simply list `self` as the first argument to the function, and `self` will be bound to the function itself, so you can call `self(x, y)` for the recursion instead of `add(x, y)`:
+
+
+```python
+@ovld
+def add(self, x: list, y: list):
+    return [self(a, b) for a, b in zip(x, y)]
+
+@ovld
+def add(self, x: tuple, y: tuple):
+    return tuple(self(a, b) for a, b in zip(x, y))
+
+@ovld
+def add(self, x: dict, y: dict):
+    return {k: self(v, y[k]) for k, v in x.items()}
+
+@ovld
+def add(self, x: object, y: object):
+    return x + y
+```
+
+Why is this useful, though? Observe:
+
+```python
+@add.variant
+def mul(self, x: object, y: object):
+    return x * y
+
+assert add([1, 2], [3, 4]) == [4, 6]
+assert mul([1, 2], [3, 4]) == [3, 8]
+```
+
+A `variant` of a function is a copy which inherits all of the original's implementations but may define new ones. And because `self` is bound to the function that's called at the top level, the implementations for `list`, `tuple` and `dict` will bind `self` to `add` or `mul` depending on which one was called. You may also call `self.super(*args)` to invoke the parent implementation for that type.
+
+## State
+
+You can pass `initial_state` to `@ovld` or `variant`. The initial state must be a function that takes no arguments. Its return value will be available in `self.state`. The state is initialized at the top level call, but recursive calls to `self` will preserve it.
+
+In other words, you can do something like this:
+
+```python
+@add.variant(initial_state=lambda: 0)
+def count(self, x, y):
+    self.state += 1
+    return (f"#{self.state}", x + y)
+
+assert count([1, 2, 3], [4, 5, 6]) == [("#1", 5), ("#2", 7), ("#3", 9)]
+```
+
+The initial_state function can return any object and you can use the state to any purpose (e.g. cache or memoization).
+
+## Custom dispatch
+
+You can define your own dispatching function. The dispatcher's first argument is always `self`.
+
+* `self.resolve(x, y)` to get the right function for the types of x and y
+* `self[type(x), type(y)]` will also return the right function for these types, but it works directly with the types.
+
+For example, here is how you might define a function such that f(x) <=> f(x, x):
+
+```python
+@ovld.dispatch
+def add_default(self, x, y=None):
+    if y is None:
+        y = x
+    return self.resolve(x, y)(x, y)
+
+@ovld
+def add_default(x: int, y: int):
+    return x + y
+
+@ovld
+def add_default(x: str, y: str):
+    return x + y
+
+@ovld
+def add_default(xs: list, ys: list):
+    return [add_default(x, y) for x, y in zip(xs, ys)]
+
+assert add_default([1, 2, "alouette"]) == [2, 4, "alouettealouette"]
+```
+
+There are other uses for this feature, e.g. memoization.
+
+The normal functions may also have a `self`, which works the same as bootstrapping, and you can give an `initial_state` to `@ovld.dispatch` as well.
+
+## Postprocess
+
+`@ovld`, `@ovld.dispatch`, etc. take a `postprocess` argument which should be a function of one argument. That function will be called with the result of the call and must return the final result of the call.
+
+Note that intermediate, bootstrapped recursive calls (recursive calls using `self()`) will **not** be postprocessed (if you want to wrap these calls, you can do so otherwise, like defining a custom dispatch). Only the result of the top level call is postprocessed.
+
+## Methods
+
+Use the `OvldMC` metaclass to use multiple dispatch on methods. In this case there is no bootstrapping as described above and `self` is simply bound to the class instance.
+
+```python
+from ovld import OvldMC
+
+class Cat(metaclass=OvldMC):
+    def interact(self, x: Mouse):
+        return "catch"
+
+    def interact(self, x: Food):
+        return "devour"
+
+    def interact(self, x: PricelessVase):
+        return "destroy"
+```
+
+Subclasses of `Cat` will inherit the overloaded `interact` and it may define additional overloaded methods which will only be valid for the subclass.
+
+**Note:** It is possible to use `ovld.dispatch` on methods, but in this case be aware that the first argument for the dispatch method will not be the usual `self` but an `OvldCall` object. The `self` can be retrived as `ovldcall.obj`. Here's an example to make it all clear:
+
+```python
+class Stuff(metaclass=OvldMC):
+    def __init__(self, mul):
+        self.mul = mul
+
+    @ovld.dispatch
+    def calc(ovldcall, x):
+        # Wraps every call to self.calc, but we receive ovldcall instead of self
+        # ovldcall[type(x)] returns the right method to call
+        # ovldcall.obj is the self (the actual instance of Stuff)
+        return ovldcall[type(x)](x) * ovldcall.obj.mul
+
+    def calc(self, x: int):
+        return x + 1
+
+    def calc(self, xs: list):
+        return [self.calc(x) for x in xs]
+
+print(Stuff(2).calc([1, 2, 3]))  # [4, 6, 8, 4, 6, 8]
+```
+
+### Mixins in subclasses
+
+The `@extend_super` decorator on a method will combine the method with the definition on the superclass:
+
+```python
+from ovld import OvldMC, extend_super
+
+class One(metaclass=OvldMC):
+    def f(self, x: int):
+        return "an integer"
+
+class Two(One):
+    @extend_super
+    def f(self, x: str):
+        return "a string"
+
+assert Two().f(1) == "an integer"
+assert Two().f("s") == "a string"
+```
+
+## Ambiguous calls
+
+The following definitions will cause a TypeError at runtime when called with two ints, because it is unclear which function is the right match:
+
+```python
+@ovld
+def ambig(x: int, y: object):
+    print("io")
+
+@ovld
+def ambig(x: object, y: int):
+    print("oi")
+
+ambig(8, 8)  # ???
+```
+
+You may define an additional function with signature (int, int) to disambiguate:
+
+```python
+@ovld
+def ambig(x: int, y: int):
+    print("ii")
+```
+
+## Other features
+
+### meta
+
+To test arbitrary conditions, you can use `meta`:
+
+```python
+from ovld import ovld, meta
+
+@meta
+def StartsWithT(cls):
+    return cls.__name__.startswith("T")
+
+@ovld
+def f(x: StartsWithT):
+    return "T"
+
+assert f(TypeError("xyz")) == "T"
+
+
+# Or: a useful example, since dataclasses have no common superclass:
+
+from dataclasses import dataclass, is_dataclass
+
+@dataclass
+class Point:
+    x: int
+    y: int
+
+@ovld
+def f(x: meta(is_dataclass)):
+    return "dataclass"
+
+assert f(Point(1, 2)) == "dataclass"
+```
+
+
+### deferred
+
+You may define overloads for certain classes from external packages without
+having to import them:
+
+
+```python
+from ovld import ovld, deferred
+
+@ovld
+def f(x: deferred("numpy.ndarray")):
+    return "ndarray"
+
+# numpy is not imported
+assert "numpy" not in sys.modules
+
+# But once we import it, the ovld works:
+import numpy
+assert f(numpy.arange(10)) == "ndarray"
+```
+
+
+### Tracebacks
+
+`ovld` automagically renames functions so that the stack trace is more informative:
+
+```python
+@add.variant
+def bad(self, x: object, y: object):
+    raise Exception("Bad.")
+
+bad([1], [2])
+
+"""
+  File "/Users/breuleuo/code/ovld/ovld/core.py", line 148, in bad.entry
+    res = ovc(*args, **kwargs)
+  File "/Users/breuleuo/code/ovld/ovld/core.py", line 182, in bad.dispatch
+    return method(self.bind_to, *args, **kwargs)
+  File "example.py", line 6, in bad[list, list]
+    return [self(a, b) for a, b in zip(x, y)]
+  File "example.py", line 6, in <listcomp>
+    return [self(a, b) for a, b in zip(x, y)]
+  File "/Users/breuleuo/code/ovld/ovld/core.py", line 182, in bad.dispatch
+    return method(self.bind_to, *args, **kwargs)
+  File "example.py", line 26, in bad[*, *]
+    raise Exception("Bad.")
+  Exception: Bad.
+"""
+```
+
+The functions on the stack have names like `bad.entry`, `bad.dispatch`, `bad[list, list]` and `bad[*, *]` (`*` stands for `object`), which lets you better understand what happened just from the stack trace.
+
+This also means profilers will be able to differentiate between these paths and between variants, even if they share code paths.
 
-setup(**setup_kwargs)
```

