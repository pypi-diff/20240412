# Comparing `tmp/trycast-1.1.0.tar.gz` & `tmp/trycast-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycast-1.1.0.tar", max compression
+gzip compressed data, was "trycast-1.2.0.tar", max compression
```

## Comparing `trycast-1.1.0.tar` & `trycast-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2022-05-10 05:54:03.409342 trycast-1.1.0/LICENSE.md
--rw-r--r--   0        0        0    21537 2023-11-12 02:50:48.559984 trycast-1.1.0/README.md
--rw-r--r--   0        0        0     2313 2023-11-12 11:31:48.395371 trycast-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    37161 2023-11-11 16:37:38.417287 trycast-1.1.0/trycast.py
--rw-r--r--   0        0        0    22818 1970-01-01 00:00:00.000000 trycast-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-10 05:54:03.409342 trycast-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0    23655 2024-04-12 20:43:20.404090 trycast-1.2.0/README.md
+-rw-r--r--   0        0        0     2487 2024-04-12 20:44:06.449996 trycast-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    42592 2024-04-12 20:33:54.044595 trycast-1.2.0/trycast.py
+-rw-r--r--   0        0        0    24880 1970-01-01 00:00:00.000000 trycast-1.2.0/PKG-INFO
```

### Comparing `trycast-1.1.0/LICENSE.md` & `trycast-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trycast-1.1.0/README.md` & `trycast-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <img src="https://raw.githubusercontent.com/davidfstr/trycast/main/README/trycast-logo.svg" title="trycast logo" align="right" />
 
 Trycast helps parses JSON-like values whose shape is defined by
 [typed dictionaries](https://www.python.org/dev/peps/pep-0589/#abstract)
 (TypedDicts) and other standard Python type hints.
 
-You can use either the `trycast()` or `isassignable()` functions below
+You can use the `trycast()`, `checkcast()`, or `isassignable()` functions below
 for parsing:
 
 
 ### trycast()
 
 Here is an example of parsing a `Point2D` object defined as a `TypedDict`
 using `trycast()`:
@@ -85,14 +85,48 @@
 > if shape is None:
 >     ...
 > ```
 > 
 > These limitations are in the process of being resolved by
 > [introducing TypeForm support to mypy](https://github.com/python/mypy/issues/9773).
 
+### checkcast()
+
+`checkcast()` is similar to `trycast()` but instead of returning `None` 
+when parsing fails it raises an exception explaining why and where the 
+parsing failed.
+
+Here is an example of parsing a `Circle` object using `checkcast()`:
+
+```python
+>>> from typing import Literal, TypedDict
+>>> from trycast import checkcast
+>>> 
+>>> class Point2D(TypedDict):
+...     x: float
+...     y: float
+... 
+>>> class Circle(TypedDict):
+...     type: Literal['circle']
+...     center: Point2D  # a nested TypedDict!
+...     radius: float
+... 
+>>> checkcast(Circle, {"type": "circle", "center": {"x": 1}, "radius": 10})
+Traceback (most recent call last):
+  ...
+trycast.ValidationError: Expected Circle but found {'type': 'circle', 'center': {'x': 1}, 'radius': 10}
+  At key 'center': Expected Point2D but found {'x': 1}
+    Required key 'y' is missing
+>>> 
+```
+
+`ValidationError` only spends time generating a message if you try to print it
+or stringify it, so can be cheaply caught if you only want to use it for
+control flow purposes.
+
 
 ### isassignable()
 
 Here is an example of parsing a `Shape` object defined as a union of
 `TypedDict`s using `isassignable()`:
 
 ```python
@@ -274,14 +308,16 @@
 * TypedDict
     * typing.TypedDict, typing_extensions.TypedDict
       ([PEP 589](https://peps.python.org/pep-0589/))
     * mypy_extensions.TypedDict (when strict=False)
     * –––
     * Required, NotRequired
       ([PEP 655](https://peps.python.org/pep-0655/))
+    * ReadOnly
+      ([PEP 705](https://peps.python.org/pep-0705/))
 * Tuples (Heterogeneous)
     * tuple[T1], tuple[T1, T2], tuple[T1, T2, T3], etc
     * Tuple[T1], Tuple[T1, T2], Tuple[T1, T2, T3], etc
 * Unions
     * Union[X, Y]
     * Optional[T]
     * X | Y
@@ -291,28 +327,30 @@
       ([PEP 586](https://peps.python.org/pep-0586/))
 * Callables
     * Callable
     * Callable[P, R] (where P=[Any]\*N and R=Any)
 * NewTypes (when strict=False)
 * Special Types
     * Any
+    * Never
     * NoReturn
 
 ### Type Checkers Supported
 
 Trycast does type check successfully with the following type checkers:
 
 * [Mypy]
 * [Pyright] / [Pylance]
 * [Pyre]
 * [Pytype]
 
 
 ## API Reference
 
+<a name="trycast-api"></a>
 ### trycast API
 
 ```
 def trycast(
     tp: TypeForm[T]† | TypeFormString[T]‡,
     value: object,
     /, failure: F = None,
@@ -339,46 +377,46 @@
 * Union[T1, T2, ...]
 * Literal[...]
 * T extends TypedDict
 
 Similar to isinstance(), this method considers every bool value to
 also be a valid int value, as consistent with Python typecheckers:
 
-> trycast(int, True) -> True
+> trycast(int, True) -> True  
 > isinstance(True, int) -> True
 
 Note that unlike isinstance(), this method considers every int value to
 also be a valid float or complex value, as consistent with Python typecheckers:
 
-> trycast(float, 1) -> 1
-> trycast(complex, 1) -> 1
-> isinstance(1, float) -> False
+> trycast(float, 1) -> 1  
+> trycast(complex, 1) -> 1  
+> isinstance(1, float) -> False  
 > isinstance(1, complex) -> False
 
 Note that unlike isinstance(), this method considers every float value to
 also be a valid complex value, as consistent with Python typecheckers:
 
-> trycast(complex, 1.0) -> 1
+> trycast(complex, 1.0) -> 1  
 > isinstance(1.0, complex) -> False
 
 Parameters:
 
 * **strict** -- 
-    * If strict=False then trycast will additionally accept
+    * If strict=False then this function will additionally accept
       mypy_extensions.TypedDict instances and Python 3.8 typing.TypedDict
       instances for the `tp` parameter. Normally these kinds of types are
-      rejected by trycast with a TypeNotSupportedError because these
+      rejected with a TypeNotSupportedError because these
       types do not preserve enough information at runtime to reliably
       determine which keys are required and which are potentially-missing.
-    * If strict=False then trycast will treat `NewType("Foo", T)`
-      the same as `T`. Normally NewTypes are rejected by trycast with a
+    * If strict=False then `NewType("Foo", T)` will be treated
+      the same as `T`. Normally NewTypes are rejected with a
       TypeNotSupportedError because values of NewTypes at runtime
       are indistinguishable from their wrapped supertype.
 * **eval** --
-  If eval=False then trycast will not attempt to resolve string
+  If eval=False then this function will not attempt to resolve string
   type references, which requires the use of the eval() function.
   Otherwise string type references will be accepted.
 
 Raises:
 
 * **TypeNotSupportedError** --
     * If strict=True and either mypy_extensions.TypedDict or a
@@ -396,79 +434,122 @@
 * † TypeForm[T] is a [type annotation object]. For example: `list[str]`
 
 * ‡ TypeFormString[T] is a stringified [type annotation object]. For example: `"list[str]"`
 
 [type annotation object]: https://github.com/python/mypy/issues/9773
 
 
+### checkcast API
+
+```
+def checkcast(
+    tp: TypeForm[T]† | TypeFormString[T]‡,
+    value: object,
+    /, *, strict: bool = True,
+    eval: bool = True
+) -> T: ...
+```
+
+If `value` is in the shape of `tp` (as accepted by a Python typechecker
+conforming to PEP 484 "Type Hints") then returns it, otherwise
+raises ValidationError.
+
+This method logically performs an operation similar to:
+
+```
+if isinstance(tp, value):
+    return value
+else:
+    raise ValidationError(tp, value)
+```
+
+except that it supports many more types than `isinstance`, including:
+
+* List[T]
+* Dict[K, V]
+* Optional[T]
+* Union[T1, T2, ...]
+* Literal[...]
+* T extends TypedDict
+
+See [trycast.trycast]\() for information about parameters,
+raised exceptions, and other details.
+
+Raises:
+
+* **ValidationError** -- If `value` is not in the shape of `tp`.
+* **TypeNotSupportedError**
+* **UnresolvedForwardRefError**
+* **UnresolvableTypeError**
+
+[trycast.trycast]: #trycast-api
+
+
 ### isassignable API
 
 ```
 def isassignable(
     value: object,
     tp: TypeForm[T]† | TypeFormString[T]‡,
-    *, eval: bool = True
+    /, *, eval: bool = True
 ) -> TypeGuard[T]: ...
 ```
 
 Returns whether `value` is in the shape of `tp`
 (as accepted by a Python typechecker conforming to PEP 484 "Type Hints").
 
 This method logically performs an operation similar to:
 
 ```
-return isinstance(tp, value)
+return isinstance(value, tp)
 ```
 
 except that it supports many more types than `isinstance`, including:
 
 * List[T]
 * Dict[K, V]
 * Optional[T]
 * Union[T1, T2, ...]
 * Literal[...]
 * T extends TypedDict
 
-Note that unlike isinstance(), this method does NOT consider bool values
-to be valid int values, as consistent with Python typecheckers:
-
-> isassignable(False, int) -> False
-> isinstance(False, int) -> True
-
-Note that unlike isinstance(), this method considers every int value to
-also be a valid float value, as consistent with Python typecheckers:
-
-> isassignable(1, float) -> True
-> isinstance(1, float) -> False
-
-Parameters:
-* **eval** --
-  If eval=False then isassignable will not attempt to resolve string
-  type references, which requires the use of the eval() function.
-  Otherwise string type references will be accepted.
+See [trycast.trycast]\(..., strict=True) for information about parameters,
+raised exceptions, and other details.
 
-Raises:
-* **TypeNotSupportedError** --
-    * If strict=True and either mypy_extensions.TypedDict or a
-      Python 3.8 typing.TypedDict is found within the `tp` argument.
-    * If strict=True and a NewType is found within the `tp` argument.
-    * If a TypeVar is found within the `tp` argument.
-    * If an unrecognized Generic type is found within the `tp` argument.
-* **UnresolvedForwardRefError** --
-  If `tp` is a type form which contains a ForwardRef.
-* **UnresolvableTypeError** --
-  If `tp` is a string that could not be resolved to a type.
+[trycast.trycast]: #trycast-api
 
 
 ## Changelog
 
 ### Future
 
 * See the [Roadmap](https://github.com/davidfstr/trycast/wiki/Roadmap).
 
+### v1.2.0
+
+* Add `checkcast()`, an alternative to `trycast()` which raises a
+  `ValidationError` upon failure instead of returning `None`.
+  ([#16](https://github.com/davidfstr/trycast/issues/16))
+* Add support for Python 3.13.
+    * Recognize `ReadOnly[]` from PEP 705.
+      ([#25](https://github.com/davidfstr/trycast/issues/25))
+* Add support for Python 3.12.
+    * Recognize `type` statements from PEP 695.
+      ([#29](https://github.com/davidfstr/trycast/issues/29))
+* Enhance support for Python 3.11:
+    * Recognize special `Never` values.
+      ([#26](https://github.com/davidfstr/trycast/issues/26))
+* Drop support for Python 3.7. ([#21](https://github.com/davidfstr/trycast/issues/21))
+* Enforce that calls to `trycast()` and `isassignable()` pass the
+  first 2 arguments in positional fashion and not in a named fashion:
+  ([#18](https://github.com/davidfstr/trycast/issues/18))
+  **(Breaking change)**
+    * Yes: `trycast(T, value)`, `isassignable(value, T)`
+    * No: `trycast(tp=T, value=value)`, `isassignable(value=value, tp=T)`
+
 ### v1.1.0
 
 * Fix `trycast()` to recognize TypedDicts with extra keys. ([#19](https://github.com/davidfstr/trycast/issues/19))
     * This new behavior helps recognize JSON structures with arbitrary additional keys
       and is consistent with how static typecheckers treat additional keys.
 * Fix magic wand in logo to look more like a magic wand. ([#20](https://github.com/davidfstr/trycast/issues/20))
```

### Comparing `trycast-1.1.0/pyproject.toml` & `trycast-1.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trycast"
-version = "1.1.0"  # publish: version
+version = "1.2.0"  # publish: version
 description = ""
 authors = ["David Foster <david@dafoster.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://dafoster.net/projects/trycast/"
 repository = "https://github.com/davidfstr/trycast"
 # TODO: Create a dedicated documentation site for the trycast project
@@ -12,40 +12,41 @@
 classifiers = [  # https://pypi.org/classifiers/
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development"
 ]
 
 [tool.poetry.urls]
 "Release notes" = "https://github.com/davidfstr/trycast#changelog"
 
 [tool.poetry.dependencies]
-# Python 3.7.4 is the minimum Python with typing.ForwardRef
-python = "^3.7.4"
+python = ">=3.8.1"
 
 [tool.poetry.dev-dependencies]
 mypy = "*"
 mypy_extensions = "*"
 pyright = "*"
 pyre-check = "*"
 pytype = { version = "==2022.3.21", python = ">=3.7.4,<3.10" }
 tox = "^3.23.1"
-black = "==22.3.0"
+black = "==24.3.0"
 isort = "^5.9.1"
-flake8 = "^3.9.2"
+flake8 = ">=6.0,<7.0"
 coverage = "*"
+# NOTE: Duplicated in: [tool.tox] > legacy_tox_ini > [testenv] > deps
+typing-extensions = ">=4.11.0rc1"  # for get_type_hints() that supports ReadOnly
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # Type Checker: Mypy
 # 
@@ -65,29 +66,35 @@
 #typeCheckingMode = "strict"  # TODO: try this
 
 # Formatter: Isort
 [tool.isort]
 profile = "black"
 atomic = true
 line_length = 88
-skip_glob = ["venv*", "test_data/forwardrefs_example_with_import_annotations.py", ".pytype"]
+skip_glob = [
+    ".pytype",
+    "test_data/forwardrefs_example*.py",
+    "test_data/type_statement_example.py",
+    "venv*",
+]
 
 # Formatter: Black
 [tool.black]
 line_length = 88
 
 # Tests
 [tool.tox]
 legacy_tox_ini = """
 
 [tox]
-envlist = py37,py38,py39,py310
+envlist = py38,py39,py310,py311,py312
 isolated_build = True
 
 [testenv]
 deps =
     mypy
     pytype == 2022.3.21 ; python_version < "3.10"
+    typing-extensions >= 4.11.0rc1
 commands =
     python3 -m unittest
 
 """
```

### Comparing `trycast-1.1.0/trycast.py` & `trycast-1.2.0/trycast.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     FrozenSet,
     List,
+    Literal,
     Mapping,
     MutableMapping,
     MutableSequence,
     NamedTuple,
     NewType,
     NoReturn,
     Optional,
@@ -33,44 +34,69 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 from typing import _eval_type as eval_type  # type: ignore[attr-defined]
 from typing import _type_repr as type_repr  # type: ignore[attr-defined]
-from typing import cast, overload
+from typing import cast, get_args, get_origin, overload
 
-try:
+# GenericAlias
+if sys.version_info >= (3, 9):
+    from types import GenericAlias
+else:
+
+    class GenericAlias(type):  # type: ignore[no-redef]
+        __origin__: object
+        __args__: Tuple[object, ...]
+
+        def __init__(self, origin: object, args: Tuple[object, ...]) -> None: ...
+
+        ...
+
+
+# UnionType
+if sys.version_info >= (3, 10):
     from types import UnionType  # type: ignore[attr-defined]
-except ImportError:
+else:
 
     class UnionType(type):  # type: ignore[no-redef]
         ...
 
 
+# Never
+if sys.version_info >= (3, 11):
+    from typing import Never
+else:
+
+    class Never(type):  # type: ignore[no-redef]
+        ...
+
+
+# TypeAliasType
+if sys.version_info >= (3, 12):
+    from typing import TypeAliasType  # type: ignore[21]  # pyre
+else:
+
+    class TypeAliasType(type):  # type: ignore[no-redef]
+        __type_params__: Tuple[object, ...]
+        __value__: object
+        ...
+
+
 # get_type_hints
 try:
-    # Python 3.7+
+    # If typing_extensions available,
+    # understands both typing.* and typing_extensions.* types
     from typing_extensions import get_type_hints  # type: ignore[attr-defined]
 except ImportError:
-    # Python 3.6
-    from typing import get_type_hints  # type: ignore[misc]  # incompatible import
-
-# Literal
-if sys.version_info >= (3, 8):
-    from typing import Literal  # Python 3.8+
-else:
-    try:
-        from typing_extensions import Literal  # Python 3.5+
-    except ImportError:
-        if not TYPE_CHECKING:
-
-            class Literal:
-                def __class_getitem__(cls, key):
-                    pass
+    # If typing_extensions not available
+    from typing import (  # type: ignore[misc, assignment]  # incompatible import
+        get_type_hints,
+    )
 
 
 # TypeGuard
 if sys.version_info >= (3, 10):
     from typing import TypeGuard  # Python 3.10+
 else:
     try:
@@ -81,36 +107,14 @@
         if not TYPE_CHECKING:
 
             class TypeGuard:
                 def __class_getitem__(cls, key):
                     return bool
 
 
-# get_origin, get_args
-if sys.version_info >= (3, 8):
-    from typing import get_args, get_origin  # Python 3.8+
-
-elif sys.version_info >= (3, 7):
-
-    def get_origin(tp: object) -> Optional[object]:
-        if isinstance(tp, _GenericAlias):  # type: ignore[16]  # pyre
-            return tp.__origin__  # type: ignore[reportGeneralTypeIssues]  # pyright
-        else:
-            return None
-
-    def get_args(tp: object) -> Tuple[object, ...]:
-        if isinstance(tp, _GenericAlias):  # type: ignore[16]  # pyre
-            return tp.__args__  # type: ignore[reportGeneralTypeIssues]  # pyright
-        else:
-            return ()
-
-else:  # pragma: no cover
-    raise ImportError("Expected Python 3.7 or later.")
-
-
 # _is_typed_dict
 _typed_dict_meta_list = []
 try:
     from typing import (  # type: ignore[attr-defined]  # isort: skip
         _TypedDictMeta as _TypingTypedDictMeta,  # type: ignore[reportGeneralTypeIssues]  # pyright
     )
 
@@ -141,15 +145,15 @@
 
 def _is_typed_dict(tp: object) -> bool:
     return isinstance(tp, _typed_dict_metas)
 
 
 # _is_newtype
 if NewType.__class__.__name__ == "function":  # type: ignore[reportGeneralTypeIssues]  # pyright
-    # Python 3.7 - 3.9
+    # Python 3.8 - 3.9
     def _is_newtype(tp: object) -> bool:
         return (
             hasattr(tp, "__class__")
             and tp.__class__.__name__ == "function"
             and hasattr(tp, "__qualname__")
             and tp.__qualname__.startswith("NewType.<locals>")  # type: ignore[attr-defined]
             and hasattr(tp, "__module__")
@@ -187,59 +191,29 @@
             # Don't auto-unwrap decorated functions
             follow_wrapped=False,
         )
 
 
 # _type_check
 if sys.version_info >= (3, 11):
-    import types
-    from typing import _GenericAlias  # type: ignore[attr-defined]  # noqa: F811
-    from typing import (  # type: ignore[attr-defined]
-        ClassVar,
-        Final,
-        Generic,
-        ParamSpec,
-        Protocol,
-        _SpecialForm,
-    )
-
-    # Workaround https://github.com/python/cpython/issues/92601
-    # by using Python 3.10's typing._type_check()
+    # NOTE: This function is derived from Python 3.12's typing._type_check
+    #       internal helper function. It is however more concerned with
+    #       rejecting known non-types (true negatives) than it is
+    #       avoiding rejecting actual types (false negatives).
+    #       See discussion at: https://github.com/python/cpython/issues/92601
     def _type_check(arg: object, msg: str):
-        """Check that the argument is a type, and return it (internal helper).
-
-        As a special case, accept None and return type(None) instead. Also wrap strings
-        into ForwardRef instances. Consider several corner cases, for example plain
-        special forms like Union are not valid, while Union[int, str] is OK, etc.
-        The msg argument is a human-readable error message, e.g::
+        """Returns the argument if it appears to be a type.
+        Raises TypeError if the argument is a known non-type.
 
-            "Union[arg, ...]: arg should be a type."
-
-        We append the repr() of the actual value (truncated to 100 chars).
+        As a special case, accepts None and returns type(None) instead.
+        Also wraps strings into ForwardRef instances.
         """
-        is_argument = True
-        module = None
-        is_class = False
-
-        invalid_generic_forms = (Generic, Protocol)  # type: tuple[object, ...]
-        if not is_class:
-            invalid_generic_forms += (ClassVar,)
-            if is_argument:
-                invalid_generic_forms += (Final,)
-
-        arg = _type_convert(arg, module=module)
-        if isinstance(arg, _GenericAlias) and arg.__origin__ in invalid_generic_forms:  # type: ignore[reportGeneralTypeIssues]  # pyright
-            raise TypeError(f"{arg} is not valid as type argument")
-        if arg in (Any, NoReturn, Final):
-            return arg
-        if isinstance(arg, _SpecialForm) or arg in (Generic, Protocol):
-            raise TypeError(f"Plain {arg} is not valid as type argument")
-        if isinstance(arg, (type, TypeVar, ForwardRef, types.UnionType, ParamSpec)):
-            return arg
-        if not callable(arg):
+        arg = _type_convert(arg, module=None)
+        # Recognize *common* non-types. (This check is not exhaustive.)
+        if isinstance(arg, (dict, list, int, tuple)):
             raise TypeError(f"{msg} Got {arg!r:.100}.")
         return arg
 
     # Python 3.10's typing._type_convert()
     def _type_convert(arg, module=None):
         """For converting None to type(None), and strings to ForwardRef."""
         if arg is None:
@@ -250,94 +224,107 @@
 
 else:
     from typing import _type_check  # type: ignore[attr-defined]
 
 
 __all__ = (
     "trycast",
+    "checkcast",
     "isassignable",
     # NOTE: May be part of the API in the future
     # "eval_type_str",
 )
 
 
 _T = TypeVar("_T")
 _F = TypeVar("_F")
 _SimpleTypeVar = TypeVar("_SimpleTypeVar")
 _SimpleTypeVarCo = TypeVar("_SimpleTypeVarCo", covariant=True)  # type: ignore[not-supported-yet]  # pytest
 
 _MISSING = object()
-_FAILURE = object()
 
 # ------------------------------------------------------------------------------
 # trycast
 
 # TODO: Once support for TypeForm is implemented in mypy,
 #       replace the   `(Type[T]) -> Optional[T]` overload
 #       and the       `(object) -> Optional[object]` overload with
 #       the following `(TypeForm[T]) -> Optional[T]` overload:
 #
 #       See: https://github.com/python/mypy/issues/9773
 # @overload
 # def trycast(tp: TypeForm[_T], value: object) -> Optional[_T]: ...
 
 
+# Overload: (tp: str, eval: Literal[False]) -> NoReturn
+
+
 @overload
 def trycast(  # type: ignore[43]  # pyre
-    tp: str, value: object, *, strict: bool = True, eval: Literal[False]
-) -> NoReturn:
-    ...  # pragma: no cover
+    tp: str, value: object, /, *, strict: bool = True, eval: Literal[False]
+) -> NoReturn: ...  # pragma: no cover
+
+
+# Overload Group: (tp: str|Type[_T]|object, value: object) -> ...
 
 
 @overload
-def trycast(tp: str, value: object, *, strict: bool = True, eval: bool = True) -> bool:  # type: ignore[43]  # pyre
+def trycast(tp: str, value: object, /, *, strict: bool = True, eval: bool = True) -> bool:  # type: ignore[43]  # pyre
     ...  # pragma: no cover
 
 
 @overload
 def trycast(  # type: ignore[43]  # pyre
-    tp: Type[_T], value: object, *, strict: bool = True, eval: bool = True
-) -> Optional[_T]:
-    ...  # pragma: no cover
+    tp: Type[_T], value: object, /, *, strict: bool = True, eval: bool = True
+) -> Optional[_T]: ...  # pragma: no cover
 
 
 @overload
 def trycast(  # type: ignore[43]  # pyre
-    tp: object, value: object, *, strict: bool = True, eval: bool = True
-) -> Optional[object]:
-    ...  # pragma: no cover
+    tp: object, value: object, /, *, strict: bool = True, eval: bool = True
+) -> Optional[object]: ...  # pragma: no cover
+
+
+# Overload Group: (tp: str|Type[_T]|object, value: object, failure: object) -> ...
 
 
 @overload
 def trycast(
     tp: str,
     value: object,
+    /,
     failure: object,
     *,
     strict: bool = True,
     eval: Literal[False],
-) -> NoReturn:
-    ...  # pragma: no cover
+) -> NoReturn: ...  # pragma: no cover
 
 
 @overload
 def trycast(
-    tp: Type[_T], value: object, failure: _F, *, strict: bool = True, eval: bool = True
-) -> Union[_T, _F]:
-    ...  # pragma: no cover
+    tp: Type[_T],
+    value: object,
+    /,
+    failure: _F,
+    *,
+    strict: bool = True,
+    eval: bool = True,
+) -> Union[_T, _F]: ...  # pragma: no cover
 
 
 @overload
 def trycast(
-    tp: object, value: object, failure: _F, *, strict: bool = True, eval: bool = True
-) -> Union[object, _F]:
-    ...  # pragma: no cover
+    tp: object, value: object, /, failure: _F, *, strict: bool = True, eval: bool = True
+) -> Union[object, _F]: ...  # pragma: no cover
+
 
+# Implementation
 
-def trycast(tp, value, failure=None, *, strict=True, eval=True):
+
+def trycast(tp, value, /, failure=None, *, strict=True, eval=True):
     """
     If `value` is in the shape of `tp` (as accepted by a Python typechecker
     conforming to PEP 484 "Type Hints") then returns it, otherwise returns
     `failure` (which is None by default).
 
     This method logically performs an operation similar to:
 
@@ -366,26 +353,26 @@
     Note that unlike isinstance(), this method considers every float value to
     also be a valid complex value, as consistent with Python typecheckers:
         > trycast(complex, 1.0) -> 1
         > isinstance(1.0, complex) -> False
 
     Parameters:
     * strict --
-        * If strict=False then trycast will additionally accept
+        * If strict=False then this function will additionally accept
           mypy_extensions.TypedDict instances and Python 3.8 typing.TypedDict
           instances for the `tp` parameter. Normally these kinds of types are
-          rejected by trycast with a TypeNotSupportedError because these
+          rejected with a TypeNotSupportedError because these
           types do not preserve enough information at runtime to reliably
           determine which keys are required and which are potentially-missing.
-        * If strict=False then trycast will treat `NewType("Foo", T)`
-          the same as `T`. Normally NewTypes are rejected by trycast with a
+        * If strict=False then `NewType("Foo", T)` will be treated
+          the same as `T`. Normally NewTypes are rejected with a
           TypeNotSupportedError because values of NewTypes at runtime
           are indistinguishable from their wrapped supertype.
     * eval --
-        If eval=False then trycast will not attempt to resolve string
+        If eval=False then this function will not attempt to resolve string
         type references, which requires the use of the eval() function.
         Otherwise string type references will be accepted.
 
     Raises:
     * TypeNotSupportedError --
         * If strict=True and either mypy_extensions.TypedDict or a
           Python 3.8 typing.TypedDict is found within the `tp` argument.
@@ -393,599 +380,757 @@
         * If a TypeVar is found within the `tp` argument.
         * If an unrecognized Generic type is found within the `tp` argument.
     * UnresolvedForwardRefError --
         If `tp` is a type form which contains a ForwardRef.
     * UnresolvableTypeError --
         If `tp` is a string that could not be resolved to a type.
     """
-    options = _TrycastOptions(strict, eval)
+    e = _checkcast_outer(tp, value, _TrycastOptions(strict, eval, funcname="trycast"))
+    if e is not None:
+        return failure  # type: ignore[bad-return-type]  # pytype
+    else:
+        return value  # type: ignore[bad-return-type]  # pytype
+
+
+# ------------------------------------------------------------------------------
+# checkcast
+
+# TODO: Once support for TypeForm is implemented in mypy,
+#       replace the   `(Type[T]) -> Optional[T]` overload
+#       and the       `(object) -> Optional[object]` overload with
+#       the following `(TypeForm[T]) -> Optional[T]` overload:
+#
+#       See: https://github.com/python/mypy/issues/9773
+# @overload
+# def checkcast(tp: TypeForm[_T], value: object) -> Optional[_T]: ...
+
+
+# Overload: (tp: str, eval: Literal[False]) -> NoReturn
+
+
+@overload
+def checkcast(  # type: ignore[43]  # pyre
+    tp: str,
+    value: object,
+    /,
+    *,
+    strict: bool = True,
+    eval: Literal[False],
+    _funcname: str = "checkcast",
+) -> NoReturn: ...  # pragma: no cover
+
+
+# Overload Group: (tp: str|Type[_T]|object, value: object) -> ...
+
+
+@overload
+def checkcast(tp: str, value: object, /, *, strict: bool = True, eval: bool = True, _funcname: str = "checkcast") -> bool:  # type: ignore[43]  # pyre
+    ...  # pragma: no cover
+
+
+@overload
+def checkcast(  # type: ignore[43]  # pyre
+    tp: Type[_T],
+    value: object,
+    /,
+    *,
+    strict: bool = True,
+    eval: bool = True,
+    _funcname: str = "checkcast",
+) -> Optional[_T]: ...  # pragma: no cover
+
+
+@overload
+def checkcast(  # type: ignore[43]  # pyre
+    tp: object,
+    value: object,
+    /,
+    *,
+    strict: bool = True,
+    eval: bool = True,
+    _funcname: str = "checkcast",
+) -> Optional[object]: ...  # pragma: no cover
+
+
+# Implementation
+
+
+def checkcast(tp, value, /, *, strict=True, eval=True, _funcname="checkcast"):
+    """
+    If `value` is in the shape of `tp` (as accepted by a Python typechecker
+    conforming to PEP 484 "Type Hints") then returns it, otherwise
+    raises ValidationError
+
+    This method logically performs an operation similar to:
+
+        if isinstance(tp, value):
+            return value
+        else:
+            raise ValidationError(tp, value)
+
+    except that it supports many more types than `isinstance`, including:
+        * List[T]
+        * Dict[K, V]
+        * Optional[T]
+        * Union[T1, T2, ...]
+        * Literal[...]
+        * T extends TypedDict
+
+    See trycast.trycast() for information about parameters,
+    raised exceptions, and other details.
+
+    Raises:
+    * ValidationError -- If `value` is not in the shape of `tp`.
+    * TypeNotSupportedError
+    * UnresolvedForwardRefError
+    * UnresolvableTypeError
+    """
+    e = _checkcast_outer(tp, value, _TrycastOptions(strict, eval, _funcname))
+    if e is not None:
+        raise e
+    else:
+        return value  # type: ignore[bad-return-type]  # pytype
+
+
+class _TrycastOptions(NamedTuple):
+    strict: bool
+    eval: bool
+    funcname: str
+
+
+def _checkcast_outer(
+    tp: object, value: object, options: _TrycastOptions
+) -> "Optional[ValidationError]":
     if isinstance(tp, str):
-        if eval:  # == options.eval (for pytype)
+        if options.eval:  # == options.eval (for pytype)
             tp = eval_type_str(tp)  # does use eval()
         else:
             raise UnresolvableTypeError(
                 f"Could not resolve type {tp!r}: "
                 f"Type appears to be a string reference "
-                f"and trycast() was called with eval=False, "
+                f"and {options.funcname}() was called with eval=False, "
                 f"disabling eval of string type references."
             )
     else:
         try:
-            tp = _type_check(tp, "trycast() requires a type as its first argument.")
+            # TODO: Eliminate format operation done by f-string
+            #       from the hot path of _checkcast_outer()
+            tp = _type_check(  # type: ignore[16]  # pyre
+                tp,
+                f"{options.funcname}() requires a type as its first argument.",
+            )
         except TypeError:
             if isinstance(tp, tuple) and len(tp) >= 1 and isinstance(tp[0], type):
                 raise TypeError(
-                    "trycast does not support checking against a tuple of types. "
+                    f"{options.funcname} does not support checking against a tuple of types. "
                     "Try checking against a Union[T1, T2, ...] instead."
                 )
             else:
                 raise
     try:
-        return _trycast_inner(tp, value, failure, options)  # type: ignore[bad-return-type]  # pytype
+        return _checkcast_inner(tp, value, options)  # type: ignore[bad-return-type]  # pytype
     except UnresolvedForwardRefError:
         if options.eval:
             advise = (
                 "Try altering the first type argument to be a string "
                 "reference (surrounded with quotes) instead."
             )
         else:
             advise = (
-                "trycast() cannot resolve string type references "
+                f"{options.funcname}() cannot resolve string type references "
                 "because it was called with eval=False."
             )
         raise UnresolvedForwardRefError(
-            f"trycast does not support checking against type form {tp!r} "
+            f"{options.funcname} does not support checking against type form {tp!r} "
             "which contains a string-based forward reference. "
             f"{advise}"
         )
 
 
-class _TrycastOptions(NamedTuple):
-    strict: bool
-    eval: bool
-
-
-# TODO: Use this signature for _trycast_inner once support for TypeForm is
-#       implemented in mypy. See: https://github.com/python/mypy/issues/9773
-# @overload
-# def _trycast_inner(tp: TypeForm[_T], value: object, failure: _F) -> Union[_T, _F]: ...
-
-
-@overload
-def _trycast_inner(
-    tp: Type[_T], value: object, failure: _F, options: _TrycastOptions
-) -> Union[_T, _F]:
-    ...  # pragma: no cover
-
-
-@overload
-def _trycast_inner(
-    tp: object, value: object, failure: _F, options: _TrycastOptions
-) -> Union[object, _F]:
-    ...  # pragma: no cover
-
-
-def _trycast_inner(tp, value, failure, options):
+def _checkcast_inner(
+    tp: object, value: object, options: _TrycastOptions
+) -> "Optional[ValidationError]":
     """
     Raises:
     * TypeNotSupportedError
     * UnresolvedForwardRefError
     """
     if tp is int:
         # Also accept bools as valid int values
         if isinstance(value, int):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+            return None
         else:
-            return failure
+            return ValidationError(tp, value)
 
     if tp is float:
         # Also accept ints and bools as valid float values
         if isinstance(value, float) or isinstance(value, int):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+            return None
         else:
-            return failure
+            return ValidationError(tp, value)
 
     if tp is complex:
         # Also accept floats, ints, and bools as valid complex values
         if (
             isinstance(value, complex)
             or isinstance(value, float)
             or isinstance(value, int)
         ):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+            return None
         else:
-            return failure
+            return ValidationError(tp, value)
 
     type_origin = get_origin(tp)
 
     if type_origin is list or type_origin is List:  # List, List[T]
-        return _trycast_listlike(tp, value, failure, list, options)
+        return _checkcast_listlike(tp, value, list, options)
 
     if type_origin is set or type_origin is Set:  # Set, Set[T]
-        return _trycast_listlike(tp, value, failure, set, options)
+        return _checkcast_listlike(tp, value, set, options)
 
     if type_origin is frozenset or type_origin is FrozenSet:  # FrozenSet, FrozenSet[T]
-        return _trycast_listlike(
-            tp, value, failure, frozenset, options, covariant_t=True
-        )
+        return _checkcast_listlike(tp, value, frozenset, options, covariant_t=True)
 
     if type_origin is tuple or type_origin is Tuple:
         if isinstance(value, tuple):
             type_args = get_args(tp)
 
             if len(type_args) == 0 or (
                 len(type_args) == 2 and type_args[1] is Ellipsis
             ):  # Tuple, Tuple[T, ...]
 
-                return _trycast_listlike(
+                return _checkcast_listlike(
                     tp,
                     value,
-                    failure,
                     tuple,
                     options,
                     covariant_t=True,
                     t_ellipsis=True,
                 )
             else:  # Tuple[Ts]
                 if len(value) != len(type_args):
-                    return failure
+                    return ValidationError(tp, value)
 
-                for (T, t) in zip(type_args, value):
-                    if _trycast_inner(T, t, _FAILURE, options) is _FAILURE:
-                        return failure
+                for i, T, t in zip(range(len(type_args)), type_args, value):
+                    e = _checkcast_inner(T, t, options)
+                    if e is not None:
+                        return ValidationError(
+                            tp,
+                            value,
+                            _causes=[e._with_prefix(_LazyStr(lambda: f"At index {i}"))],
+                        )
 
-                return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+                return None
         else:
-            return failure
+            return ValidationError(tp, value)
 
     if type_origin is Sequence or type_origin is CSequence:  # Sequence, Sequence[T]
-        return _trycast_listlike(
-            tp, value, failure, CSequence, options, covariant_t=True
-        )
+        return _checkcast_listlike(tp, value, CSequence, options, covariant_t=True)
 
     if (
         type_origin is MutableSequence or type_origin is CMutableSequence
     ):  # MutableSequence, MutableSequence[T]
-        return _trycast_listlike(tp, value, failure, CMutableSequence, options)
+        return _checkcast_listlike(tp, value, CMutableSequence, options)
 
     if type_origin is dict or type_origin is Dict:  # Dict, Dict[K, V]
-        return _trycast_dictlike(tp, value, failure, dict, options)
+        return _checkcast_dictlike(tp, value, dict, options)
 
     if type_origin is Mapping or type_origin is CMapping:  # Mapping, Mapping[K, V]
-        return _trycast_dictlike(
-            tp, value, failure, CMapping, options, covariant_v=True
-        )
+        return _checkcast_dictlike(tp, value, CMapping, options, covariant_v=True)
 
     if (
         type_origin is MutableMapping or type_origin is CMutableMapping
     ):  # MutableMapping, MutableMapping[K, V]
-        return _trycast_dictlike(tp, value, failure, CMutableMapping, options)
+        return _checkcast_dictlike(tp, value, CMutableMapping, options)
 
-    if type_origin is Union or type_origin is UnionType:  # Union[T1, T2, ...]
+    if (
+        type_origin is Union or type_origin is UnionType
+    ):  # Union[T1, T2, ...], Optional[T]
+        causes = []
         for T in get_args(tp):
-            if _trycast_inner(T, value, _FAILURE, options) is not _FAILURE:  # type: ignore[wrong-arg-types]  # pytype
-                if isinstance(tp, type):
-                    return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-                else:
-                    return value
-        return failure
+            e = _checkcast_inner(T, value, options)
+            if e is not None:
+                causes.append(e)
+            else:
+                return None
+        return ValidationError(tp, value, _causes=causes)
 
     if type_origin is Literal:  # Literal[...]
         for literal in get_args(tp):
             if value == literal:
-                if isinstance(tp, type):
-                    return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-                else:
-                    return value
-        return failure
+                return None
+        return ValidationError(tp, value)
 
     if type_origin is CCallable:
         callable_args = get_args(tp)
         if callable_args == ():
             # Callable
             if callable(value):
-                return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+                return None
             else:
-                return failure
+                return ValidationError(tp, value)
         else:
-            if len(callable_args) != 2 or (
-                callable_args[0] is not Ellipsis
-                and not isinstance(callable_args[0], list)
-            ):
-                # Python 3.7
-                callable_args = (
-                    list(callable_args[: len(callable_args) - 1]),
-                    callable_args[len(callable_args) - 1],
-                )
-
             assert len(callable_args) == 2
             (param_types, return_type) = callable_args
 
             if return_type is not Any:
                 # Callable[..., T]
                 raise TypeNotSupportedError(
-                    f"trycast cannot reliably determine whether value is "
+                    f"{options.funcname} cannot reliably determine whether value is "
                     f"a {type_repr(tp)} because "
                     f"callables at runtime do not always have a "
                     f"declared return type. "
-                    f"Consider using trycast(Callable, value) instead."
+                    f"Consider using {options.funcname}(Callable, value) instead."
                 )
 
             if param_types is Ellipsis:
                 # Callable[..., Any]
-                return _trycast_inner(Callable, value, failure, options)
+                return _checkcast_inner(Callable, value, options)
 
             assert isinstance(param_types, list)
             for param_type in param_types:
                 if param_type is not Any:
                     raise TypeNotSupportedError(
-                        f"trycast cannot reliably determine whether value is "
+                        f"{options.funcname} cannot reliably determine whether value is "
                         f"a {type_repr(tp)} because "
                         f"callables at runtime do not always have "
                         f"declared parameter types. "
-                        f"Consider using trycast("
+                        f"Consider using {options.funcname}("
                         f"Callable[{','.join('Any' * len(param_types))}, Any], value) "
                         f"instead."
                     )
 
             # Callable[[Any * N], Any]
             if callable(value):
                 try:
                     sig = _inspect_signature(value)
                 except TypeError:
                     # Not a callable
-                    return failure
-                except ValueError:
+                    return ValidationError(tp, value)
+                except ValueError as f:
                     # Unable to introspect signature for value.
                     # It might be a built-in function that lacks signature support.
                     # Assume conservatively that value does NOT match the requested type.
-                    return failure
+                    e = ValidationError(tp, value)
+                    e.__cause__ = f
+                    return e
                 else:
-                    sig_min_param_count = 0
-                    sig_max_param_count = 0
+                    sig_min_param_count = 0  # type: float
+                    sig_max_param_count = 0  # type: float
                     for expected_param in sig.parameters.values():
                         if (
                             expected_param.kind == Parameter.POSITIONAL_ONLY
                             or expected_param.kind == Parameter.POSITIONAL_OR_KEYWORD
                         ):
                             if expected_param.default is Parameter.empty:
                                 sig_min_param_count += 1
                             sig_max_param_count += 1
                         elif expected_param.kind == Parameter.VAR_POSITIONAL:
                             sig_max_param_count = math.inf
 
                     if sig_min_param_count <= len(param_types) <= sig_max_param_count:
-                        return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
+                        return None
                     else:
-                        return failure
+                        return ValidationError(tp, value)
             else:
-                return failure
+                return ValidationError(tp, value)
+
+    if isinstance(type_origin, TypeAliasType):  # type: ignore[16]  # pyre
+        if len(type_origin.__type_params__) > 0:
+            substitutions = dict(
+                zip(
+                    type_origin.__type_params__,
+                    get_args(tp) + ((Any,) * len(type_origin.__type_params__)),
+                )
+            )  # type: Dict[object, object]
+            new_tp = _substitute(tp.__value__, substitutions)  # type: ignore[attr-defined]  # mypy
+        else:
+            new_tp = tp.__value__  # type: ignore[attr-defined]  # mypy
+        return _checkcast_inner(new_tp, value, options)  # type: ignore[16]  # pyre
 
-    if isinstance(tp, _GenericAlias):
+    if isinstance(tp, _GenericAlias):  # type: ignore[16]  # pyre
         raise TypeNotSupportedError(
-            f"trycast does not know how to recognize generic type "
+            f"{options.funcname} does not know how to recognize generic type "
             f"{type_repr(type_origin)}."
         )
 
     if _is_typed_dict(tp):  # T extends TypedDict
         if isinstance(value, Mapping):
             if options.eval:
                 resolved_annotations = get_type_hints(  # does use eval()
-                    tp
+                    tp  # type: ignore[arg-type]  # mypy
                 )  # resolve ForwardRefs in tp.__annotations__
             else:
                 resolved_annotations = tp.__annotations__  # type: ignore[attribute-error]  # pytype
 
             try:
                 # {typing in Python 3.9+, typing_extensions}.TypedDict
-                required_keys = tp.__required_keys__  # type: ignore[attribute-error]  # pytype
+                required_keys = tp.__required_keys__  # type: ignore[attr-defined, attribute-error]  # mypy, pytype
             except AttributeError:
                 # {typing in Python 3.8, mypy_extensions}.TypedDict
                 if options.strict:
                     if sys.version_info[:2] >= (3, 9):
                         advise = "Suggest use a typing.TypedDict instead."
                     else:
                         advise = "Suggest use a typing_extensions.TypedDict instead."
-                    advise2 = "Or use trycast(..., strict=False)."
+                    advise2 = f"Or use {options.funcname}(..., strict=False)."
                     raise TypeNotSupportedError(
-                        f"trycast cannot determine which keys are required "
+                        f"{options.funcname} cannot determine which keys are required "
                         f"and which are potentially-missing for the "
                         f"specified kind of TypedDict. {advise} {advise2}"
                     )
                 else:
-                    if tp.__total__:  # type: ignore[attribute-error]  # pytype
+                    if tp.__total__:  # type: ignore[attr-defined, attribute-error]  # mypy, pytype
                         required_keys = resolved_annotations.keys()
                     else:
                         required_keys = frozenset()
 
-            for (k, v) in value.items():  # type: ignore[attribute-error]  # pytype
+            for k, v in value.items():  # type: ignore[attribute-error]  # pytype
                 V = resolved_annotations.get(k, _MISSING)
-                if (
-                    V is not _MISSING
-                    and _trycast_inner(V, v, _FAILURE, options) is _FAILURE
-                ):
-                    return failure
+                if V is not _MISSING:
+                    e = _checkcast_inner(V, v, options)
+                    if e is not None:
+                        return ValidationError(
+                            tp,
+                            value,
+                            _causes=[e._with_prefix(_LazyStr(lambda: f"At key {k!r}"))],
+                        )
 
             for k in required_keys:
                 if k not in value:  # type: ignore[unsupported-operands]  # pytype
-                    return failure
-            if isinstance(tp, type):
-                return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-            else:
-                return value
+                    return ValidationError(
+                        tp,
+                        value,
+                        _causes=[
+                            ValidationError._from_message(
+                                _LazyStr(lambda: f"Required key {k!r} is missing")
+                            )
+                        ],
+                    )
+            return None
         else:
-            return failure
+            return ValidationError(tp, value)
 
     if _is_newtype(tp):
         if options.strict:
-            supertype_repr = type_repr(tp.__supertype__)  # type: ignore[attribute-error]  # pytype
+            supertype_repr = type_repr(tp.__supertype__)  # type: ignore[attr-defined, attribute-error]  # mypy, pytype
+            tp_name_repr = repr(tp.__name__)  # type: ignore[attr-defined]  # mypy
             raise TypeNotSupportedError(
-                f"trycast cannot reliably determine whether value is "
-                f"a NewType({tp.__name__!r}, {supertype_repr}) because "
+                f"{options.funcname} cannot reliably determine whether value is "
+                f"a NewType({tp_name_repr}, {supertype_repr}) because "
                 f"NewType wrappers are erased at runtime "
                 f"and are indistinguishable from their supertype. "
-                f"Consider using trycast(..., strict=False) to treat "
-                f"NewType({tp.__name__!r}, {supertype_repr}) "
+                f"Consider using {options.funcname}(..., strict=False) to treat "
+                f"NewType({tp_name_repr}, {supertype_repr}) "
                 f"like {supertype_repr}."
             )
         else:
-            supertype = tp.__supertype__  # type: ignore[attribute-error]  # pytype
-            return _trycast_inner(supertype, value, failure, options)
+            supertype = tp.__supertype__  # type: ignore[attr-defined, attribute-error]  # mypy, pytype
+            return _checkcast_inner(supertype, value, options)
 
     if isinstance(tp, TypeVar):  # type: ignore[wrong-arg-types]  # pytype
         raise TypeNotSupportedError(
-            "trycast cannot reliably determine whether value matches a TypeVar."
+            f"{options.funcname} cannot reliably determine whether value matches a TypeVar."
         )
 
     if tp is Any:
-        if isinstance(tp, type):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-        else:
-            return value
+        return None
+
+    if tp is Never or tp is NoReturn:
+        return ValidationError(tp, value)
 
-    if tp is NoReturn:
-        return failure
+    if isinstance(tp, TypeAliasType):  # type: ignore[16]  # pyre
+        if len(tp.__type_params__) > 0:  # type: ignore[16]  # pyre
+            substitutions = dict(
+                zip(tp.__type_params__, ((Any,) * len(tp.__type_params__)))
+            )
+            new_tp = _substitute(tp.__value__, substitutions)
+        else:
+            new_tp = tp.__value__
+        return _checkcast_inner(new_tp, value, options)  # type: ignore[16]  # pyre
 
     if isinstance(tp, ForwardRef):
         raise UnresolvedForwardRefError()
 
-    if isinstance(value, tp):  # type: ignore[wrong-arg-types]  # pytype
-        return value
+    if isinstance(value, tp):  # type: ignore[arg-type, wrong-arg-types]  # mypy, pytype
+        return None
     else:
-        return failure
+        return ValidationError(tp, value)
 
 
 class TypeNotSupportedError(TypeError):
     pass
 
 
 class UnresolvedForwardRefError(TypeError):
     pass
 
 
-@overload
-def _trycast_listlike(
-    tp: Type[_T],
-    value: object,
-    failure: _F,
-    listlike_type: Type,
-    options: _TrycastOptions,
-    *,
-    covariant_t: bool = False,
-    t_ellipsis: bool = False,
-) -> Union[_T, _F]:
-    ...  # pragma: no cover
+def _substitute(tp: object, substitutions: Dict[object, object]) -> object:
+    if isinstance(tp, GenericAlias):  # ex: tuple[T1, T2]
+        return GenericAlias(  # type: ignore[reportCallIssue]  # pyright
+            tp.__origin__, tuple([_substitute(a, substitutions) for a in tp.__args__])
+        )
+    if isinstance(tp, TypeVar):  # type: ignore[wrong-arg-types]  # pytype
+        return substitutions.get(tp, tp)
+    return tp
 
 
-@overload
-def _trycast_listlike(
+def _checkcast_listlike(
     tp: object,
     value: object,
-    failure: _F,
     listlike_type: Type,
     options: _TrycastOptions,
     *,
     covariant_t: bool = False,
     t_ellipsis: bool = False,
-) -> Union[object, _F]:
-    ...  # pragma: no cover
-
-
-def _trycast_listlike(
-    tp, value, failure, listlike_type, options, *, covariant_t=False, t_ellipsis=False
-):
+) -> "Optional[ValidationError]":
     if isinstance(value, listlike_type):
         T_ = get_args(tp)
 
         if len(T_) == 0:  # Python 3.9+
             (T,) = (_SimpleTypeVarCo if covariant_t else _SimpleTypeVar,)
 
         else:
             if t_ellipsis:
                 if len(T_) == 2 and T_[1] is Ellipsis:
                     (T, _) = T_
                 else:
-                    return failure
+                    return ValidationError(tp, value)
             else:
                 (T,) = T_
 
         if _is_simple_typevar(T, covariant=covariant_t):
             pass
         else:
-            for x in value:  # type: ignore[attribute-error]  # pytype
-                if _trycast_inner(T, x, _FAILURE, options) is _FAILURE:
-                    return failure
+            for i, x in enumerate(value):  # type: ignore[attribute-error]  # pytype
+                e = _checkcast_inner(T, x, options)
+                if e is not None:
+                    return ValidationError(
+                        tp,
+                        value,
+                        _causes=[e._with_prefix(_LazyStr(lambda: f"At index {i}"))],
+                    )
 
-        if isinstance(tp, type):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-        else:
-            return value
+        return None
     else:
-        return failure
-
-
-@overload
-def _trycast_dictlike(
-    tp: Type[_T],
-    value: object,
-    failure: _F,
-    dictlike_type: Type,
-    options: _TrycastOptions,
-    *,
-    covariant_v: bool = False,
-) -> Union[_T, _F]:
-    ...  # pragma: no cover
+        return ValidationError(tp, value)
 
 
-@overload
-def _trycast_dictlike(
+def _checkcast_dictlike(
     tp: object,
     value: object,
-    failure: _F,
     dictlike_type: Type,
     options: _TrycastOptions,
     *,
     covariant_v: bool = False,
-) -> Union[object, _F]:
-    ...  # pragma: no cover
-
-
-def _trycast_dictlike(tp, value, failure, dictlike_type, options, *, covariant_v=False):
+) -> "Optional[ValidationError]":
     if isinstance(value, dictlike_type):
         K_V = get_args(tp)
 
         if len(K_V) == 0:  # Python 3.9+
             (K, V) = (
                 _SimpleTypeVar,
                 _SimpleTypeVarCo if covariant_v else _SimpleTypeVar,
             )
         else:
             (K, V) = K_V
 
         if _is_simple_typevar(K) and _is_simple_typevar(V, covariant=covariant_v):
             pass
         else:
-            for (k, v) in value.items():  # type: ignore[attribute-error]  # pytype
-                if (
-                    _trycast_inner(K, k, _FAILURE, options) is _FAILURE
-                    or _trycast_inner(V, v, _FAILURE, options) is _FAILURE
-                ):
-                    return failure
-        if isinstance(tp, type):
-            return cast(_T, value)  # type: ignore[reportGeneralTypeIssues]  # pyright
-        else:
-            return value
+            for k, v in value.items():  # type: ignore[attribute-error]  # pytype
+                e = _checkcast_inner(K, k, options)
+                if e is not None:
+                    return ValidationError(
+                        tp,
+                        value,
+                        _causes=[e._with_prefix(_LazyStr(lambda: f"Key {k!r}"))],
+                    )
+                e = _checkcast_inner(V, v, options)
+                if e is not None:
+                    return ValidationError(
+                        tp,
+                        value,
+                        _causes=[e._with_prefix(_LazyStr(lambda: f"At key {k!r}"))],
+                    )
+        return None
     else:
-        return failure
+        return ValidationError(tp, value)
 
 
 def _is_simple_typevar(T: object, covariant: bool = False) -> bool:
     return (
         isinstance(T, TypeVar)  # type: ignore[wrong-arg-types]  # pytype
         and T.__constraints__ == ()  # type: ignore[attribute-error]  # pytype
         and T.__covariant__ == covariant  # type: ignore[attribute-error]  # pytype
         and T.__contravariant__ is False  # type: ignore[attribute-error]  # pytype
         and T.__constraints__ == ()  # type: ignore[attribute-error]  # pytype
     )
 
 
 # ------------------------------------------------------------------------------
+# ValidationError
+
+
+if sys.version_info >= (3, 11):
+    from typing import Self as _SelfValidationError
+else:
+    _SelfValidationError = TypeVar("_SelfValidationError", bound="ValidationError")
+
+
+class ValidationError(ValueError):
+    # === Init ===
+
+    def __init__(
+        self,
+        tp: object,
+        value: object,
+        /,
+        # NOTE: Inner type and structure for representing "cause" information
+        #       is private and may change in the future.
+        _causes: "Optional[Sequence[ValidationError]]" = None,
+        *,
+        _message: "Optional[_LazyStr]" = None,
+    ) -> None:
+        """
+        Creates a ValidationError related to the specified value not matching
+        the expected specified type.
+
+        Parameters (positional-only):
+        * tp -- the expected type of the specified value.
+        * value -- a value.
+        """
+        if _causes is None:
+            _causes = []
+        if _message is None:
+            _message = _LazyStr(
+                lambda: f"Expected {format_type_str(tp)} but found {value!r}"
+            )
+        super().__init__(_message)
+        self._tp = tp
+        self._value = value
+        self._causes = _causes
+        self._prefix = None  # type: Optional[_LazyStr]
+
+    # Private factory method
+    @staticmethod
+    def _from_message(message: "_LazyStr") -> "ValidationError":
+        return ValidationError(None, None, _message=message)
+
+    # Private builder method
+    def _with_prefix(
+        self: _SelfValidationError, prefix: "_LazyStr", /  # type: ignore[11]  # pyre  # noqa: W504
+    ) -> _SelfValidationError:
+        self._prefix = prefix
+        return self
+
+    # === __str__ ===
+
+    def __str__(self) -> str:
+        """
+        Returns a human-readable explanation of this ValidationError.
+
+        The specific format of this explanation may change in the future.
+        """
+        parts = []  # type: List[str]
+        self._format_to(parts)
+        return "".join(parts)
+
+    def _format_to(self, parts: List[str], indent: int = 0) -> None:
+        for i in range(indent):
+            parts.append("  ")
+        if self._prefix is not None:
+            parts.append(str(self._prefix))  # NOTE: May be a _LazyStr
+            parts.append(": ")
+        parts.append(super().__str__())
+        if len(self._causes) > 0:
+            for c in self._causes:  # type: ignore[16]  # pyre
+                parts.append("\n")
+                c._format_to(parts, indent=indent + 1)
+
+
+class _LazyStr(str):
+    def __init__(self, value_func: Callable[[], str], /) -> None:
+        self._value_func = value_func
+        self._value = None  # type: Optional[str]
+
+    def __str__(self) -> str:
+        if self._value is None:
+            self._value = self._value_func()
+        return self._value
+
+
+# ------------------------------------------------------------------------------
 # isassignable
 
 # TODO: Once support for TypeForm is implemented in mypy,
 #       replace the   `(Type[T]) -> TypeGuard[T]` overload
 #       and the       `(object) -> bool` overload with
 #       the following `(TypeForm[T]) -> TypeGuard[T]` overload:
 #
 #       See: https://github.com/python/mypy/issues/9773
 # @overload
 # def isassignable(value: object, tp: TypeForm[_T]) -> TypeGuard[_T]: ...
 
 
 @overload
-def isassignable(value: object, tp: str, *, eval: Literal[False]) -> NoReturn:
-    ...  # pragma: no cover
+def isassignable(
+    value: object, tp: str, /, *, eval: Literal[False]
+) -> NoReturn: ...  # pragma: no cover
 
 
 @overload
-def isassignable(value: object, tp: str, *, eval: bool = True) -> bool:
-    ...  # pragma: no cover
+def isassignable(
+    value: object, tp: str, /, *, eval: bool = True
+) -> bool: ...  # pragma: no cover
 
 
 @overload
-def isassignable(value: object, tp: Type[_T], *, eval: bool = True) -> TypeGuard[_T]:  # type: ignore[invalid-annotation]  # pytype
+def isassignable(value: object, tp: Type[_T], /, *, eval: bool = True) -> TypeGuard[_T]:  # type: ignore[invalid-annotation]  # pytype
     ...  # pragma: no cover
 
 
 @overload
-def isassignable(value: object, tp: object, *, eval: bool = True) -> bool:
-    ...  # pragma: no cover
+def isassignable(
+    value: object, tp: object, /, *, eval: bool = True
+) -> bool: ...  # pragma: no cover
 
 
-def isassignable(value, tp, *, eval=True):
+def isassignable(value, tp, /, *, eval=True):
     """
     Returns whether `value` is in the shape of `tp`
     (as accepted by a Python typechecker conforming to PEP 484 "Type Hints").
 
     This method logically performs an operation similar to:
 
-        return isinstance(tp, value)
+        return isinstance(value, tp)
 
     except that it supports many more types than `isinstance`, including:
         * List[T]
         * Dict[K, V]
         * Optional[T]
         * Union[T1, T2, ...]
         * Literal[...]
         * T extends TypedDict
 
-    Note that unlike isinstance(), this method does NOT consider bool values
-    to be valid int values, as consistent with Python typecheckers:
-        > isassignable(False, int) -> False
-        > isinstance(False, int) -> True
-
-    Note that unlike isinstance(), this method considers every int value to
-    also be a valid float value, as consistent with Python typecheckers:
-        > isassignable(1, float) -> True
-        > isinstance(1, float) -> False
-
-    Parameters:
-    * eval --
-        If eval=False then isassignable will not attempt to resolve string
-        type references, which requires the use of the eval() function.
-        Otherwise string type references will be accepted.
-
-    Raises:
-    * TypeNotSupportedError --
-        * If strict=True and either mypy_extensions.TypedDict or a
-          Python 3.8 typing.TypedDict is found within the `tp` argument.
-        * If strict=True and a NewType is found within the `tp` argument.
-        * If a TypeVar is found within the `tp` argument.
-        * If an unrecognized Generic type is found within the `tp` argument.
-    * UnresolvedForwardRefError --
-        If `tp` is a type form which contains a ForwardRef.
-    * UnresolvableTypeError --
-        If `tp` is a string that could not be resolved to a type.
+    See trycast.trycast(..., strict=True) for information about parameters,
+    raised exceptions, and other details.
     """
+    e = _checkcast_outer(
+        tp, value, _TrycastOptions(strict=True, eval=eval, funcname="isassignable")
+    )
+    result = e is None
     if isinstance(tp, type):
         return cast(  # type: ignore[invalid-annotation]  # pytype
             TypeGuard[_T],  # type: ignore[not-indexable]  # pytype
-            (
-                trycast(tp, value, _isassignable_failure, strict=True, eval=eval)
-                is not _isassignable_failure
-            ),
+            result,
         )
     else:
-        return (
-            trycast(tp, value, _isassignable_failure, strict=True, eval=eval)
-            is not _isassignable_failure
-        )
-
-
-_isassignable_failure = object()
+        return result  # type: ignore[bad-return-type]  # pytype
 
 
 # ------------------------------------------------------------------------------
 # eval_type_str
 
 _IMPORTABLE_TYPE_EXPRESSION_RE = re.compile(r"^((?:[a-zA-Z0-9_]+\.)+)(.*)$")
 _UNIMPORTABLE_TYPE_EXPRESSION_RE = re.compile(r"^[a-zA-Z0-9_]+(\[.*\])?$")
@@ -999,15 +1144,15 @@
 
 # TODO: Use this signature for _eval_type once support for TypeForm is
 #       implemented in mypy. See: https://github.com/python/mypy/issues/9773
 # def _eval_type(tp: str) -> TypeForm: ...
 
 
 @functools.lru_cache()
-def eval_type_str(tp: str) -> object:
+def eval_type_str(tp: str, /) -> object:
     """
     Resolves a string-reference to a type that can be imported,
     such as `'typing.List'`.
 
     This function does internally cache lookups that have been made in
     the past to improve performance. If you need to clear this cache
     you can call:
@@ -1083,7 +1228,39 @@
 
 
 class UnresolvableTypeError(TypeError):
     pass
 
 
 # ------------------------------------------------------------------------------
+# format_type_str
+
+
+def format_type_str(tp: object, /) -> str:
+    """
+    Formats a type annotation object as a string similar to how it would
+    appear in source code.
+    """
+    if tp is Ellipsis:
+        return "..."
+
+    tp_origin = get_origin(tp)
+    if tp_origin is not None:
+        tp_args = get_args(tp)
+        if tp_args != ():
+            if tp_origin is UnionType:
+                return " | ".join([format_type_str(x) for x in tp_args])
+            return (
+                format_type_str(tp_origin)
+                + "["
+                + ", ".join([format_type_str(x) for x in tp_args])
+                + "]"
+            )
+        tp_name = getattr(tp_origin, "__name__", None)
+    else:
+        tp_name = getattr(tp, "__name__", None)
+    if tp_name is not None:
+        return tp_name
+    return repr(tp)
+
+
+# ------------------------------------------------------------------------------
```

### Comparing `trycast-1.1.0/PKG-INFO` & `trycast-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: trycast
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Home-page: https://dafoster.net/projects/trycast/
 License: MIT
 Author: David Foster
 Author-email: david@dafoster.net
-Requires-Python: >=3.7.4,<4.0.0
+Requires-Python: >=3.8.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Project-URL: Documentation, https://dafoster.net/projects/trycast/
 Project-URL: Repository, https://github.com/davidfstr/trycast
 Project-URL: Release notes, https://github.com/davidfstr/trycast#changelog
 Description-Content-Type: text/markdown
@@ -33,15 +32,15 @@
 
 <img src="https://raw.githubusercontent.com/davidfstr/trycast/main/README/trycast-logo.svg" title="trycast logo" align="right" />
 
 Trycast helps parses JSON-like values whose shape is defined by
 [typed dictionaries](https://www.python.org/dev/peps/pep-0589/#abstract)
 (TypedDicts) and other standard Python type hints.
 
-You can use either the `trycast()` or `isassignable()` functions below
+You can use the `trycast()`, `checkcast()`, or `isassignable()` functions below
 for parsing:
 
 
 ### trycast()
 
 Here is an example of parsing a `Point2D` object defined as a `TypedDict`
 using `trycast()`:
@@ -116,14 +115,48 @@
 > if shape is None:
 >     ...
 > ```
 > 
 > These limitations are in the process of being resolved by
 > [introducing TypeForm support to mypy](https://github.com/python/mypy/issues/9773).
 
+### checkcast()
+
+`checkcast()` is similar to `trycast()` but instead of returning `None` 
+when parsing fails it raises an exception explaining why and where the 
+parsing failed.
+
+Here is an example of parsing a `Circle` object using `checkcast()`:
+
+```python
+>>> from typing import Literal, TypedDict
+>>> from trycast import checkcast
+>>> 
+>>> class Point2D(TypedDict):
+...     x: float
+...     y: float
+... 
+>>> class Circle(TypedDict):
+...     type: Literal['circle']
+...     center: Point2D  # a nested TypedDict!
+...     radius: float
+... 
+>>> checkcast(Circle, {"type": "circle", "center": {"x": 1}, "radius": 10})
+Traceback (most recent call last):
+  ...
+trycast.ValidationError: Expected Circle but found {'type': 'circle', 'center': {'x': 1}, 'radius': 10}
+  At key 'center': Expected Point2D but found {'x': 1}
+    Required key 'y' is missing
+>>> 
+```
+
+`ValidationError` only spends time generating a message if you try to print it
+or stringify it, so can be cheaply caught if you only want to use it for
+control flow purposes.
+
 
 ### isassignable()
 
 Here is an example of parsing a `Shape` object defined as a union of
 `TypedDict`s using `isassignable()`:
 
 ```python
@@ -305,14 +338,16 @@
 * TypedDict
     * typing.TypedDict, typing_extensions.TypedDict
       ([PEP 589](https://peps.python.org/pep-0589/))
     * mypy_extensions.TypedDict (when strict=False)
     * –––
     * Required, NotRequired
       ([PEP 655](https://peps.python.org/pep-0655/))
+    * ReadOnly
+      ([PEP 705](https://peps.python.org/pep-0705/))
 * Tuples (Heterogeneous)
     * tuple[T1], tuple[T1, T2], tuple[T1, T2, T3], etc
     * Tuple[T1], Tuple[T1, T2], Tuple[T1, T2, T3], etc
 * Unions
     * Union[X, Y]
     * Optional[T]
     * X | Y
@@ -322,28 +357,30 @@
       ([PEP 586](https://peps.python.org/pep-0586/))
 * Callables
     * Callable
     * Callable[P, R] (where P=[Any]\*N and R=Any)
 * NewTypes (when strict=False)
 * Special Types
     * Any
+    * Never
     * NoReturn
 
 ### Type Checkers Supported
 
 Trycast does type check successfully with the following type checkers:
 
 * [Mypy]
 * [Pyright] / [Pylance]
 * [Pyre]
 * [Pytype]
 
 
 ## API Reference
 
+<a name="trycast-api"></a>
 ### trycast API
 
 ```
 def trycast(
     tp: TypeForm[T]† | TypeFormString[T]‡,
     value: object,
     /, failure: F = None,
@@ -370,46 +407,46 @@
 * Union[T1, T2, ...]
 * Literal[...]
 * T extends TypedDict
 
 Similar to isinstance(), this method considers every bool value to
 also be a valid int value, as consistent with Python typecheckers:
 
-> trycast(int, True) -> True
+> trycast(int, True) -> True  
 > isinstance(True, int) -> True
 
 Note that unlike isinstance(), this method considers every int value to
 also be a valid float or complex value, as consistent with Python typecheckers:
 
-> trycast(float, 1) -> 1
-> trycast(complex, 1) -> 1
-> isinstance(1, float) -> False
+> trycast(float, 1) -> 1  
+> trycast(complex, 1) -> 1  
+> isinstance(1, float) -> False  
 > isinstance(1, complex) -> False
 
 Note that unlike isinstance(), this method considers every float value to
 also be a valid complex value, as consistent with Python typecheckers:
 
-> trycast(complex, 1.0) -> 1
+> trycast(complex, 1.0) -> 1  
 > isinstance(1.0, complex) -> False
 
 Parameters:
 
 * **strict** -- 
-    * If strict=False then trycast will additionally accept
+    * If strict=False then this function will additionally accept
       mypy_extensions.TypedDict instances and Python 3.8 typing.TypedDict
       instances for the `tp` parameter. Normally these kinds of types are
-      rejected by trycast with a TypeNotSupportedError because these
+      rejected with a TypeNotSupportedError because these
       types do not preserve enough information at runtime to reliably
       determine which keys are required and which are potentially-missing.
-    * If strict=False then trycast will treat `NewType("Foo", T)`
-      the same as `T`. Normally NewTypes are rejected by trycast with a
+    * If strict=False then `NewType("Foo", T)` will be treated
+      the same as `T`. Normally NewTypes are rejected with a
       TypeNotSupportedError because values of NewTypes at runtime
       are indistinguishable from their wrapped supertype.
 * **eval** --
-  If eval=False then trycast will not attempt to resolve string
+  If eval=False then this function will not attempt to resolve string
   type references, which requires the use of the eval() function.
   Otherwise string type references will be accepted.
 
 Raises:
 
 * **TypeNotSupportedError** --
     * If strict=True and either mypy_extensions.TypedDict or a
@@ -427,79 +464,122 @@
 * † TypeForm[T] is a [type annotation object]. For example: `list[str]`
 
 * ‡ TypeFormString[T] is a stringified [type annotation object]. For example: `"list[str]"`
 
 [type annotation object]: https://github.com/python/mypy/issues/9773
 
 
+### checkcast API
+
+```
+def checkcast(
+    tp: TypeForm[T]† | TypeFormString[T]‡,
+    value: object,
+    /, *, strict: bool = True,
+    eval: bool = True
+) -> T: ...
+```
+
+If `value` is in the shape of `tp` (as accepted by a Python typechecker
+conforming to PEP 484 "Type Hints") then returns it, otherwise
+raises ValidationError.
+
+This method logically performs an operation similar to:
+
+```
+if isinstance(tp, value):
+    return value
+else:
+    raise ValidationError(tp, value)
+```
+
+except that it supports many more types than `isinstance`, including:
+
+* List[T]
+* Dict[K, V]
+* Optional[T]
+* Union[T1, T2, ...]
+* Literal[...]
+* T extends TypedDict
+
+See [trycast.trycast]\() for information about parameters,
+raised exceptions, and other details.
+
+Raises:
+
+* **ValidationError** -- If `value` is not in the shape of `tp`.
+* **TypeNotSupportedError**
+* **UnresolvedForwardRefError**
+* **UnresolvableTypeError**
+
+[trycast.trycast]: #trycast-api
+
+
 ### isassignable API
 
 ```
 def isassignable(
     value: object,
     tp: TypeForm[T]† | TypeFormString[T]‡,
-    *, eval: bool = True
+    /, *, eval: bool = True
 ) -> TypeGuard[T]: ...
 ```
 
 Returns whether `value` is in the shape of `tp`
 (as accepted by a Python typechecker conforming to PEP 484 "Type Hints").
 
 This method logically performs an operation similar to:
 
 ```
-return isinstance(tp, value)
+return isinstance(value, tp)
 ```
 
 except that it supports many more types than `isinstance`, including:
 
 * List[T]
 * Dict[K, V]
 * Optional[T]
 * Union[T1, T2, ...]
 * Literal[...]
 * T extends TypedDict
 
-Note that unlike isinstance(), this method does NOT consider bool values
-to be valid int values, as consistent with Python typecheckers:
-
-> isassignable(False, int) -> False
-> isinstance(False, int) -> True
-
-Note that unlike isinstance(), this method considers every int value to
-also be a valid float value, as consistent with Python typecheckers:
-
-> isassignable(1, float) -> True
-> isinstance(1, float) -> False
-
-Parameters:
-* **eval** --
-  If eval=False then isassignable will not attempt to resolve string
-  type references, which requires the use of the eval() function.
-  Otherwise string type references will be accepted.
+See [trycast.trycast]\(..., strict=True) for information about parameters,
+raised exceptions, and other details.
 
-Raises:
-* **TypeNotSupportedError** --
-    * If strict=True and either mypy_extensions.TypedDict or a
-      Python 3.8 typing.TypedDict is found within the `tp` argument.
-    * If strict=True and a NewType is found within the `tp` argument.
-    * If a TypeVar is found within the `tp` argument.
-    * If an unrecognized Generic type is found within the `tp` argument.
-* **UnresolvedForwardRefError** --
-  If `tp` is a type form which contains a ForwardRef.
-* **UnresolvableTypeError** --
-  If `tp` is a string that could not be resolved to a type.
+[trycast.trycast]: #trycast-api
 
 
 ## Changelog
 
 ### Future
 
 * See the [Roadmap](https://github.com/davidfstr/trycast/wiki/Roadmap).
 
+### v1.2.0
+
+* Add `checkcast()`, an alternative to `trycast()` which raises a
+  `ValidationError` upon failure instead of returning `None`.
+  ([#16](https://github.com/davidfstr/trycast/issues/16))
+* Add support for Python 3.13.
+    * Recognize `ReadOnly[]` from PEP 705.
+      ([#25](https://github.com/davidfstr/trycast/issues/25))
+* Add support for Python 3.12.
+    * Recognize `type` statements from PEP 695.
+      ([#29](https://github.com/davidfstr/trycast/issues/29))
+* Enhance support for Python 3.11:
+    * Recognize special `Never` values.
+      ([#26](https://github.com/davidfstr/trycast/issues/26))
+* Drop support for Python 3.7. ([#21](https://github.com/davidfstr/trycast/issues/21))
+* Enforce that calls to `trycast()` and `isassignable()` pass the
+  first 2 arguments in positional fashion and not in a named fashion:
+  ([#18](https://github.com/davidfstr/trycast/issues/18))
+  **(Breaking change)**
+    * Yes: `trycast(T, value)`, `isassignable(value, T)`
+    * No: `trycast(tp=T, value=value)`, `isassignable(value=value, tp=T)`
+
 ### v1.1.0
 
 * Fix `trycast()` to recognize TypedDicts with extra keys. ([#19](https://github.com/davidfstr/trycast/issues/19))
     * This new behavior helps recognize JSON structures with arbitrary additional keys
       and is consistent with how static typecheckers treat additional keys.
 * Fix magic wand in logo to look more like a magic wand. ([#20](https://github.com/davidfstr/trycast/issues/20))
```

