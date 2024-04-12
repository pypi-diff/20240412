# Comparing `tmp/imy-0.2.2.tar.gz` & `tmp/imy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.2.2.tar", max compression
+gzip compressed data, was "imy-0.2.3.tar", max compression
```

## Comparing `imy-0.2.2.tar` & `imy-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.2/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.2/imy/__init__.py
--rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.2/imy/assets.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.2/imy/async_utils.py
--rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.2/imy/config.py
--rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.2/imy/docstrings/__init__.py
--rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.2/imy/docstrings/models.py
--rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.2/imy/docstrings/parsers.py
--rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.2/imy/inject.py
--rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.2/imy/logs.py
--rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.2/imy/package_metadata.py
--rw-r--r--   0        0        0      754 2024-04-10 14:11:15.450664 imy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.3/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-08 18:10:47.446922 imy-0.2.3/imy/__init__.py
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.3/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.3/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.3/imy/config.py
+-rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.3/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.3/imy/docstrings/models.py
+-rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.3/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8572 2024-04-10 14:07:52.133967 imy-0.2.3/imy/inject.py
+-rw-r--r--   0        0        0    13613 2024-04-10 14:10:43.230681 imy-0.2.3/imy/logs.py
+-rw-r--r--   0        0        0     2167 2024-04-11 21:48:52.558560 imy-0.2.3/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-12 07:06:15.658576 imy-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.3/PKG-INFO
```

### Comparing `imy-0.2.2/LICENSE` & `imy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/assets.py` & `imy-0.2.3/imy/assets.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/async_utils.py` & `imy-0.2.3/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/config.py` & `imy-0.2.3/imy/config.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/docstrings/models.py` & `imy-0.2.3/imy/docstrings/models.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/docstrings/parsers.py` & `imy-0.2.3/imy/docstrings/parsers.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/inject.py` & `imy-0.2.3/imy/inject.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/logs.py` & `imy-0.2.3/imy/logs.py`

 * *Files identical despite different names*

### Comparing `imy-0.2.2/imy/package_metadata.py` & `imy-0.2.3/imy/package_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 """
 Utilities for getting metadata about your own package.
 """
 
 import importlib.metadata
 import inspect
+import sys
 from pathlib import Path
 
 
 def _get_root_directory(caller: inspect.FrameInfo) -> Path:
     """
     Return the root directory of the calling module, accounting for submodules.
 
     For example, if the calling module is `foo.bar.baz`, and `foo` is located
     at `/home/user/foo`, this function will return `/home/user/foo`.
     """
-    caller_dir = Path(caller.filename).resolve().parent
+    caller_path = Path(caller.filename).absolute()
+
+    # `__init__` files aren't their own submodules, so treat them as their
+    # parent
+    if caller_path.name == "__init__.py":
+        caller_path = caller_path.parent
 
     # How deep is this submodule?
-    depth = caller.frame.f_globals["__name__"].count(".")
+    depth: int = caller.frame.f_globals["__name__"].count(".")
 
     for _ in range(depth):
-        caller_dir = caller_dir.parent
+        caller_path = caller_path.parent
 
-    return caller_dir
+    return caller_path
 
 
 def get_package_version(own_package_pypi_name: str) -> str:
     """
     Determine the version of **the calling package**. `own_package_pypi_name` is
     the name of the package, as you would type to install it from pypi.
 
@@ -41,15 +47,15 @@
         pass
 
     # While the approach above is clean, it fails during development. In that
     # case, read the version from the `pyproject.toml` file.
     import tomllib
 
     caller_frame = inspect.stack()[1]
-    toml_path = _get_root_directory(caller_frame) / "pyproject.toml"
+    toml_path = _get_root_directory(caller_frame).parent / "pyproject.toml"
 
     try:
         with open(toml_path, "rb") as f:
             toml_contents = tomllib.load(f)
 
     except FileNotFoundError:
         raise RuntimeError(f"Cannot find `pyproject.toml` at `{toml_path}`") from None
```

### Comparing `imy-0.2.2/pyproject.toml` & `imy-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.2.2"
+version = "0.2.3"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.2.2/PKG-INFO` & `imy-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

