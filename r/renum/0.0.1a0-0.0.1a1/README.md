# Comparing `tmp/renum-0.0.1a0.tar.gz` & `tmp/renum-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renum-0.0.1a0.tar", last modified: Thu Apr 11 21:11:03 2024, max compression
+gzip compressed data, was "renum-0.0.1a1.tar", last modified: Thu Apr 11 22:58:54 2024, max compression
```

## Comparing `renum-0.0.1a0.tar` & `renum-0.0.1a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:11:03.818857 renum-0.0.1a0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:11:03.818857 renum-0.0.1a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:11:03.818857 renum-0.0.1a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-11 21:10:58.000000 renum-0.0.1a0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-11 21:10:58.000000 renum-0.0.1a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-11 21:10:58.000000 renum-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 21:10:58.000000 renum-0.0.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-11 21:11:03.818857 renum-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 21:10:58.000000 renum-0.0.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-11 21:10:58.000000 renum-0.0.1a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:11:03.818857 renum-0.0.1a0/renum/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-11 21:10:58.000000 renum-0.0.1a0/renum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-04-11 21:10:58.000000 renum-0.0.1a0/renum/renum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:11:03.818857 renum-0.0.1a0/renum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-11 21:11:03.000000 renum-0.0.1a0/renum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 21:11:03.000000 renum-0.0.1a0/renum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:11:03.000000 renum-0.0.1a0/renum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 21:11:03.000000 renum-0.0.1a0/renum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 21:11:03.000000 renum-0.0.1a0/renum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:11:03.818857 renum-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 21:10:58.000000 renum-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:58:54.947541 renum-0.0.1a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:58:54.943540 renum-0.0.1a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:58:54.943540 renum-0.0.1a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-11 22:58:50.000000 renum-0.0.1a1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-11 22:58:50.000000 renum-0.0.1a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-11 22:58:50.000000 renum-0.0.1a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-11 22:58:50.000000 renum-0.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-11 22:58:54.947541 renum-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-11 22:58:50.000000 renum-0.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-11 22:58:50.000000 renum-0.0.1a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:58:54.947541 renum-0.0.1a1/renum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-11 22:58:50.000000 renum-0.0.1a1/renum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-11 22:58:50.000000 renum-0.0.1a1/renum/renum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:58:54.947541 renum-0.0.1a1/renum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-11 22:58:54.000000 renum-0.0.1a1/renum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 22:58:54.000000 renum-0.0.1a1/renum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:58:54.000000 renum-0.0.1a1/renum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-11 22:58:54.000000 renum-0.0.1a1/renum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 22:58:54.000000 renum-0.0.1a1/renum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:58:54.947541 renum-0.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-11 22:58:50.000000 renum-0.0.1a1/setup.py
```

### Comparing `renum-0.0.1a0/.github/workflows/pythonpublish.yml` & `renum-0.0.1a1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/.gitignore` & `renum-0.0.1a1/.gitignore`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/.pre-commit-config.yaml` & `renum-0.0.1a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/LICENSE` & `renum-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/PKG-INFO` & `renum-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renum
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Easily build Enum-like regular expression patterns
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2024 - 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `renum-0.0.1a0/README.md` & `renum-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/pyproject.toml` & `renum-0.0.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `renum-0.0.1a0/renum/__init__.py` & `renum-0.0.1a1/renum/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 __all__ = ("renum",)
 
 if _sys.version_info < (3, 8):
     from importlib_metadata import metadata as _metadata
 else:
     from importlib.metadata import metadata as _metadata
 
-__copyright__ = "Copyright 2019-2023 Zephyrkul"
+__copyright__ = "Copyright 2024-2024 Zephyrkul"
 
 _meta = _metadata(__name__)
 __title__ = _meta["Name"]
 __author__ = _meta["Author"]
 __license__ = _meta["License"]
 __version__ = _meta["Version"]
```

### Comparing `renum-0.0.1a0/renum/renum.py` & `renum-0.0.1a1/renum/renum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from __future__ import annotations
 
 import re
 import sys
 from contextvars import ContextVar
 from enum import Enum
-from typing import TYPE_CHECKING, Any, ClassVar, Iterator, overload
+from typing import TYPE_CHECKING, Any, Iterator, overload
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
 __all__ = ("renum",)
 _matches: ContextVar[dict[renum, re.Match[str]]] = ContextVar("_match")
 
 
-class renum(str, Enum):
-    _pattern_: ClassVar[re.Pattern[str]]
+class renum(Enum):
+    if TYPE_CHECKING:
+        _pattern_: re.Pattern[str]
+        _value_: str
+
+        @property
+        def value(self) -> str: ...
 
     @staticmethod
     def _generate_next_value_(
         name: str, start: int, count: int, last_values: list[str]
     ) -> str:
         raise TypeError("enum.auto() used with renum")
 
     def __new__(cls, *values: Any) -> Self:
         value = str(*values)
-        member = str.__new__(cls, value)
+        member = object.__new__(cls)
         member._value_ = value
         return member
 
     def __init_subclass__(cls, flags: int | re.RegexFlag = 0, **kwargs: Any) -> None:
         super().__init_subclass__(**kwargs)
         cls._pattern_ = re.compile(
             r"|".join(rf"(?P<{member.name}>{member.value})" for member in cls),
             flags=flags,
         )
 
-    __str__ = str.__str__  # type: ignore
-    __format__ = str.__format__  # type: ignore
+    def __str__(self) -> str:
+        return self.value
+
+    __hash__ = object.__hash__
 
     @property
     def last_match(self) -> re.Match[str] | None:
         """
         The last re.Match that matched this renum member's pattern.
         """
         return _matches.get({}).get(self)
```

### Comparing `renum-0.0.1a0/renum.egg-info/PKG-INFO` & `renum-0.0.1a1/renum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renum
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Easily build Enum-like regular expression patterns
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2024 - 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

