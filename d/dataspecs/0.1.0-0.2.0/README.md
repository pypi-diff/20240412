# Comparing `tmp/dataspecs-0.1.0.tar.gz` & `tmp/dataspecs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspecs-0.1.0.tar", max compression
+gzip compressed data, was "dataspecs-0.2.0.tar", max compression
```

## Comparing `dataspecs-0.1.0.tar` & `dataspecs-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2024-03-03 09:44:37.563845 dataspecs-0.1.0/LICENSE
--rw-r--r--   0        0        0      884 2024-03-03 09:44:37.563845 dataspecs-0.1.0/README.md
--rw-r--r--   0        0        0      358 2024-03-03 09:44:37.563845 dataspecs-0.1.0/dataspecs/__init__.py
--rw-r--r--   0        0        0     3606 2024-03-03 09:44:37.563845 dataspecs-0.1.0/dataspecs/api.py
--rw-r--r--   0        0        0        0 2024-03-03 09:44:37.563845 dataspecs-0.1.0/dataspecs/py.typed
--rw-r--r--   0        0        0     5067 2024-03-03 09:44:37.563845 dataspecs-0.1.0/dataspecs/specs.py
--rw-r--r--   0        0        0     2079 2024-03-03 09:44:37.567845 dataspecs-0.1.0/dataspecs/typing.py
--rw-r--r--   0        0        0      899 2024-03-03 09:44:37.567845 dataspecs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 dataspecs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-12 18:28:21.633624 dataspecs-0.2.0/LICENSE
+-rw-r--r--   0        0        0      876 2024-04-12 18:28:21.633624 dataspecs-0.2.0/README.md
+-rw-r--r--   0        0        0      358 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/__init__.py
+-rw-r--r--   0        0        0     5113 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/api.py
+-rw-r--r--   0        0        0        0 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/py.typed
+-rw-r--r--   0        0        0     5104 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/specs.py
+-rw-r--r--   0        0        0     2633 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/typing.py
+-rw-r--r--   0        0        0      891 2024-04-12 18:28:21.633624 dataspecs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.2.0/PKG-INFO
```

### Comparing `dataspecs-0.1.0/LICENSE` & `dataspecs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspecs-0.1.0/README.md` & `dataspecs-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 [![Release](https://img.shields.io/pypi/v/dataspecs?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dataspecs/)
 [![Python](https://img.shields.io/pypi/pyversions/dataspecs?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dataspecs/)
 [![Downloads](https://img.shields.io/pypi/dm/dataspecs?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/dataspecs)
 [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.10652375-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.10652375)
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
-Data specifications defined in data classes
+Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.1.0
+pip install dataspecs==0.2.0
 ```
```

### Comparing `dataspecs-0.1.0/dataspecs/specs.py` & `dataspecs-0.2.0/dataspecs/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from pathlib import PurePosixPath
 from re import Match, compile, escape, fullmatch
 from typing import Any, Optional, SupportsIndex, TypeVar, cast, overload
 
 
 # dependencies
 from typing_extensions import Self
-from .typing import StrPath, TagBase, is_strpath, is_tag
+from .typing import DataClass, StrPath, TagBase, is_strpath, is_tag
 
 
 # constants
-GLOB_PATTERN = compile(r"\\\*\\\*()|\\\*([^\\\*]|$)|\\\?()")
-GLOB_REPLS = r".*", r"[^/]*", r"[/_]"
+GLOB_PATTERN = compile(r"\\\*\\\*()|\\\*([^\\\*]|$)")
+GLOB_REPLS = r".*", r"[^/]*"
 ROOT_PATH = "/"
 
 
 # type hints
 TSpec = TypeVar("TSpec", bound="Spec")
 
 
@@ -49,16 +49,15 @@
         return super().__new__(cls, *segments)
 
     def match(self, path_pattern: StrPath, /) -> bool:
         """Check if the ID matches a path pattern.
 
         Unlike original ``PurePosixPath.match``, it always performs
         case-sensitive matching. It also accepts double-wildcards
-        (``**``) for recursively matching the path segments
-        and question mark (``?``) for matching ``/`` or ``_``.
+        (``**``) for recursively matching the path segments.
 
         Args:
             path_pattern: Path pattern for matching.
 
         Returns:
             ``True`` if the path pattern matches the ID.
             ``False`` otherwise.
@@ -69,45 +68,45 @@
             index = cast(int, match.lastindex)
             return GLOB_REPLS[index - 1] + match.group(index)
 
         regex = GLOB_PATTERN.sub(repl, escape(fspath(path_pattern)))
         return bool(fullmatch(regex, fspath(self)))
 
 
-ROOT = ID("/")
+ROOT = ID(ROOT_PATH)
 """Root ID."""
 
 
 @dataclass(frozen=True)
 class Spec:
     """Data specification (data spec).
 
     Args:
         id: ID of the data spec.
         tags: Tags of the data spec.
-        data: Data of the data spec.
-        type: Type hint of the data spec.
-        origin: Origin of the data spec.
+        type: Type hint for the data of the data spec.
+        data: Default or final data of the data spec.
+        origin: Original dataclass object of the data spec.
 
     """
 
     id: ID
     """ID of the data spec."""
 
     tags: tuple[TagBase, ...]
     """Tags of the data spec."""
 
-    data: Any
-    """Data of the data spec."""
+    type: Any
+    """Type hint for the data of the data spec."""
 
-    type: Any = field(default=Any, repr=False)
-    """Type hint of the data spec."""
+    data: Optional[Any] = None
+    """Default or final data of the data spec."""
 
-    origin: Any = field(default=None, repr=False)
-    """Origin of the data spec."""
+    origin: Optional[DataClass] = field(default=None, repr=False)
+    """Original dataclass object of the data spec."""
 
 
 class Specs(UserList[TSpec]):
     """Data specifications (data specs)."""
 
     @property
     def first(self) -> Optional[TSpec]:
```

### Comparing `dataspecs-0.1.0/dataspecs/typing.py` & `dataspecs-0.2.0/dataspecs/typing.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from dataclasses import Field, is_dataclass
 from enum import Enum
 from os import PathLike
 from typing import Annotated, Any, ClassVar, Protocol, Union
 
 
 # dependencies
-from typing_extensions import TypeGuard, get_args, get_origin
+from typing_extensions import TypeGuard, get_args, get_origin, get_type_hints
 
 
 # type hints
 StrPath = Union[str, PathLike[str]]
 
 
 class DataClass(Protocol):
@@ -21,15 +21,15 @@
 
     __dataclass_fields__: ClassVar[dict[str, Field[Any]]]
 
 
 class TagBase(Enum):
     """Base enum of tag for data specs.
 
-    Since ``TagBase`` itself cannot have any members,
+    Since ``TagBase`` itself does not have any members,
     users should create their own tags by inheriting it::
 
         from enum import auto
         from dataspecs import TagBase
 
         class Tag(TagBase):
             ATTR = auto()
@@ -52,16 +52,30 @@
 
 
 def get_dataclasses(obj: Any, /) -> tuple[DataClass, ...]:
     """Return dataclass objects that annotate a type hint."""
     return tuple(filter(is_dataclass, get_annotations(obj)))
 
 
-def get_subscriptions(obj: Any, /) -> tuple[Any, ...]:
-    """Return subscriptions of a type hint if they exist."""
+def get_final(obj: Any, /, type_only: bool = True) -> Any:
+    """Return the type hint with forward references resolved."""
+
+    class _:
+        __annotations__ = dict(obj=obj)
+
+    return get_type_hints(_, include_extras=not type_only)["obj"]
+
+
+def get_first(obj: Any, /) -> Any:
+    """Return the first type if a type hint is a union type."""
+    return get_args(obj)[0] if is_union(obj) else obj
+
+
+def get_subtypes(obj: Any, /) -> tuple[Any, ...]:
+    """Return subtypes of a type hint if they exist."""
     return get_args(get_annotated(obj))
 
 
 def get_tags(obj: Any, /) -> tuple[TagBase, ...]:
     """Return tags that annotate a type hint."""
     return tuple(filter(is_tag, get_annotations(obj)))
 
@@ -75,7 +89,12 @@
     """Check if an object is a string or a string path."""
     return isinstance(obj, (str, PathLike))
 
 
 def is_tag(obj: Any, /) -> TypeGuard[TagBase]:
     """Check if an object is a specification tag."""
     return isinstance(obj, TagBase)
+
+
+def is_union(obj: Any, /) -> bool:
+    """Check if a type hint is a union type."""
+    return get_origin(Union[obj]) is Union  # type: ignore
```

### Comparing `dataspecs-0.1.0/pyproject.toml` & `dataspecs-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "dataspecs"
-version = "0.1.0"
-description = "Data specifications defined in data classes"
+version = "0.2.0"
+description = "Data specifications by data classes"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 documentation = "https://astropenguin.github.io/dataspecs/"
 homepage = "https://github.com/astropenguin/dataspecs/"
 keywords = ["dataclasses", "specifications", "typing"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 typing-extensions = "^4.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^24.2"
+black = "^24.3"
 ipython = "^8.18"
 myst-parser = "^2.0"
-mypy = "^1.8"
-pydata-sphinx-theme = "^0.14"
+mypy = "^1.9"
+pydata-sphinx-theme = "^0.15"
 pyright = "^1.1"
 pytest = "^7.4"
 sphinx = "^7.2"
 
 [tool.mypy]
 strict = true
 disable_error_code = ["override", "unused-ignore"]
```

### Comparing `dataspecs-0.1.0/PKG-INFO` & `dataspecs-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dataspecs
-Version: 0.1.0
-Summary: Data specifications defined in data classes
+Version: 0.2.0
+Summary: Data specifications by data classes
 Home-page: https://github.com/astropenguin/dataspecs/
 License: MIT
 Keywords: dataclasses,specifications,typing
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 
 [![Release](https://img.shields.io/pypi/v/dataspecs?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dataspecs/)
 [![Python](https://img.shields.io/pypi/pyversions/dataspecs?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dataspecs/)
 [![Downloads](https://img.shields.io/pypi/dm/dataspecs?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/dataspecs)
 [![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.10652375-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.10652375)
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
-Data specifications defined in data classes
+Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.1.0
+pip install dataspecs==0.2.0
 ```
```

