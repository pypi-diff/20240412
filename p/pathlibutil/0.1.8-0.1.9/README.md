# Comparing `tmp/pathlibutil-0.1.8.tar.gz` & `tmp/pathlibutil-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibutil-0.1.8.tar", max compression
+gzip compressed data, was "pathlibutil-0.1.9.tar", max compression
```

## Comparing `pathlibutil-0.1.8.tar` & `pathlibutil-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-01-27 17:10:50.840141 pathlibutil-0.1.8/LICENSE
--rw-r--r--   0        0        0     8115 2024-01-27 17:10:50.844141 pathlibutil-0.1.8/README.md
--rw-r--r--   0        0        0      242 2024-01-27 17:10:50.844141 pathlibutil-0.1.8/pathlibutil/__init__.py
--rw-r--r--   0        0        0      413 2024-01-27 17:10:50.844141 pathlibutil-0.1.8/pathlibutil/base.py
--rw-r--r--   0        0        0    16868 2024-01-27 17:10:50.844141 pathlibutil-0.1.8/pathlibutil/path.py
--rw-r--r--   0        0        0     9321 2024-01-27 17:10:50.844141 pathlibutil-0.1.8/pathlibutil/types.py
--rw-r--r--   0        0        0     1787 2024-01-27 17:11:00.424233 pathlibutil-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9074 1970-01-01 00:00:00.000000 pathlibutil-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/LICENSE
+-rw-r--r--   0        0        0     9675 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/README.md
+-rw-r--r--   0        0        0      242 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/pathlibutil/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/pathlibutil/base.py
+-rw-r--r--   0        0        0    19732 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/pathlibutil/path.py
+-rw-r--r--   0        0        0     9321 2024-04-12 19:40:08.276848 pathlibutil-0.1.9/pathlibutil/types.py
+-rw-r--r--   0        0        0     1810 2024-04-12 19:40:16.652834 pathlibutil-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0    10634 1970-01-01 00:00:00.000000 pathlibutil-0.1.9/PKG-INFO
```

### Comparing `pathlibutil-0.1.8/LICENSE` & `pathlibutil-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlibutil-0.1.8/README.md` & `pathlibutil-0.1.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 - `Path.move()` move a file or directory to a new path destination
 - `Path.make_archive()` creates and `Path.unpack_archive()` uncompresses an archive from a file or directory
 - `Path.archive_formats` to get all available archive formats
 - `Path.stat()` returns a `StatResult` object to get file or directory information containing
   - `TimeInt` objects for `atime`, `ctime`, `mtime` and `birthtime`
   - `ByteInt` object for `size`
 - `Path.relative_to()` to get relative path from a file or directory, `walk_up` to walk up the directory tree.
+- `Path.with_suffix()` to change the multiple suffixes of a file
+- `Path.cwd()` to get the current working directory or executable path when script is bundled, e.g. with `pyinstaller`
+- `Path.resolve()` to resolve a unc path to a mapped windows drive.
 
 ## Installation
 
 ```bash
 pip install pathlibutil
 ```
 
@@ -232,7 +235,44 @@
 
 archive = file.make_archive("README.foo.bar")
 
 backup = archive.move("./backup/")
 
 print(f"archive created: {archive.name} and moved to: {backup.parent}")
 ```
+
+## Example 6
+
+Access the current working directory with optional parameter `frozen` to determine
+different directories when script is bundled to an executable,
+e.g. with `pyinstaller`.
+> `Path.cwd()`
+
+```cmd
+>>> poetry run examples/example6.py -b
+Building frozen: K:/pathlibutil/examples/example6.exe
+Build succeeded: 0
+
+>>> poetry run examples/example6.py
+we are                          not frozen
+
+bundle dir is                   K:/pathlibutil/examples
+sys.argv[0] is                  K:/pathlibutil/examples/example6.py
+sys.executable is               K:/pathlibutil/.venv/Scripts/python.exe
+os.getcwd is                    K:/pathlibutil
+
+Path.cwd(frozen=True) is        K:/pathlibutil
+Path.cwd(frozen=False) is       K:/pathlibutil
+Path.cwd(frozen=_MEIPASS) is    K:/pathlibutil
+
+>>> examples/example6.exe
+we are                          ever so frozen
+
+bundle dir is                   C:/Users/CHRIST~1.DOE/AppData/Local/Temp/_MEI106042
+sys.argv[0] is                  examples/example6.exe
+sys.executable is               K:/pathlibutil/examples/example6.exe
+os.getcwd is                    K:/pathlibutil
+
+Path.cwd(frozen=True) is        K:/pathlibutil/examples
+Path.cwd(frozen=False) is       K:/pathlibutil
+Path.cwd(frozen=_MEIPASS) is    C:/Users/CHRIST~1.DOE/AppData/Local/Temp/_MEI106042
+```
```

### Comparing `pathlibutil-0.1.8/pathlibutil/path.py` & `pathlibutil-0.1.9/pathlibutil/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import errno
 import hashlib
 import itertools
 import os
+import re
 import shutil
-from typing import Callable, Dict, Generator, List, Set, Union
+import subprocess
+import sys
+from typing import Callable, Dict, Generator, List, Literal, Set, Union
 
 from pathlibutil.base import BasePath, _Path
 from pathlibutil.types import ByteInt, StatResult, _stat_result, byteint
 
 
 class Path(BasePath):
     """
@@ -471,14 +474,103 @@
         if relative.parts.count("..") > walk_up:
             raise ValueError(
                 f"'{relative}' is outside of the relative deepth of '{walk_up}'"
             )
 
         return relative
 
+    @classmethod
+    def cwd(cls, *, frozen: Literal[True, False, "_MEIPASS"] = False) -> _Path:
+        """
+        Return a `Path` object representing the current working directory.
+
+        The `frozen` parameter takes only effect when the script is bundled to a
+        executable, e.g. with `pyinstaller`.
+
+        - `False`: Returns the current working directory, this is the default.
+        - `True`: Returns the directory of the executable.
+        - `"_MEIPASS"`: Returns the directory of the bundled resources.
+        """
+        if getattr(sys, "frozen", False):
+            if frozen is True:
+                return cls(sys.executable).parent
+            elif isinstance(frozen, str):
+                return cls(getattr(sys, frozen))
+
+        return super().cwd()
+
+    @classmethod
+    def _net_use(cls) -> Dict[str, str]:
+        """
+        Return a dictionary of mapped network drives. Keys are UNC paths and values
+        are drive letters.
+        """
+
+        def run(cmd: str) -> str:
+            """execute `command` and return stdout with cp850 encoding."""
+            result = subprocess.run(
+                cmd,
+                capture_output=True,
+                shell=True,
+                encoding="cp850",
+            )
+
+            return result.stdout
+
+        try:
+            mapped_drives = re.finditer(
+                r"^OK\s+(?P<drive>[A-Z]):\s+(?P<unc>\S+)",
+                run("net use"),
+                re.IGNORECASE | re.MULTILINE,
+            )
+            return {
+                match.group("unc") + "\\": match.group("drive") + ":\\"
+                for match in mapped_drives
+            }
+        except Exception:
+            return {}
+
+    def _resolve_unc(self) -> _Path:
+        """
+        Resolve UNC paths to mapped network drives.
+        """
+        if not hasattr(self.__class__, "_netuse"):
+            self.__class__._netuse = self._net_use()
+
+        try:
+            drive = self._netuse[self.anchor]
+            return self.__class__(drive).joinpath(self.relative_to(self.anchor))
+        except KeyError:
+            return self
+
+    def resolve(self, strict: bool = False, unc: bool = True) -> _Path:
+        """
+        Make the path absolute, resolving all symlinks on the way and also normalizing
+        it.
+
+        If `strict` is `True`, a `FileNotFoundError` will be raised if the path does
+        not exist.
+
+        On Windows if `unc` is `False`, UNC paths will be resolved to mapped network
+        drives.
+
+        >>> Path("T:/file.txt").resolve()
+        Path("\\\\server\\temp\\file.txt")
+
+        >>> Path("//server/temp/file.txt").resolve(unc=False)
+        Path("T:\\file.txt")
+        """
+
+        p = super().resolve(strict)
+
+        if unc is True or os.name != "nt":
+            return p
+
+        return p._resolve_unc()
+
 
 class Register7zFormat(Path, archive="7z"):
     """
     Register 7z archive format using `__init_subclass__` hook.
 
     To register a new archive format just inherit a subclass from `Path` with an
     argument of `archive` specifying the suffix of the archive without any dots (eg.
```

### Comparing `pathlibutil-0.1.8/pathlibutil/types.py` & `pathlibutil-0.1.9/pathlibutil/types.py`

 * *Files identical despite different names*

### Comparing `pathlibutil-0.1.8/pyproject.toml` & `pathlibutil-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pathlibutil"
-version = "v0.1.8"
+version = "v0.1.9"
 description = "inherits from pathlib.Path with methods for hashing, copying, deleting and more"
 authors = ["Christoph Dörrer <d-chris@web.de>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
@@ -40,14 +40,15 @@
 black = "^23.12.1"
 docformatter = "^1.7.5"
 
 [tool.poetry.group.doc.dependencies]
 jinja2-pdoc = "^0.2.0"
 pdoc = "^14.3.0"
 click = "^8.1.7"
+pyinstaller = "^6.5.0"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [[tool.poetry.source]]
 name = "testpypi"
```

### Comparing `pathlibutil-0.1.8/PKG-INFO` & `pathlibutil-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathlibutil
-Version: 0.1.8
+Version: 0.1.9
 Summary: inherits from pathlib.Path with methods for hashing, copying, deleting and more
 Home-page: https://d-chris.github.io
 License: MIT
 Keywords: pathlib,hashlib,shutil
 Author: Christoph Dörrer
 Author-email: d-chris@web.de
 Requires-Python: >=3.8.1,<3.13
@@ -48,14 +48,17 @@
 - `Path.move()` move a file or directory to a new path destination
 - `Path.make_archive()` creates and `Path.unpack_archive()` uncompresses an archive from a file or directory
 - `Path.archive_formats` to get all available archive formats
 - `Path.stat()` returns a `StatResult` object to get file or directory information containing
   - `TimeInt` objects for `atime`, `ctime`, `mtime` and `birthtime`
   - `ByteInt` object for `size`
 - `Path.relative_to()` to get relative path from a file or directory, `walk_up` to walk up the directory tree.
+- `Path.with_suffix()` to change the multiple suffixes of a file
+- `Path.cwd()` to get the current working directory or executable path when script is bundled, e.g. with `pyinstaller`
+- `Path.resolve()` to resolve a unc path to a mapped windows drive.
 
 ## Installation
 
 ```bash
 pip install pathlibutil
 ```
 
@@ -257,7 +260,44 @@
 archive = file.make_archive("README.foo.bar")
 
 backup = archive.move("./backup/")
 
 print(f"archive created: {archive.name} and moved to: {backup.parent}")
 ```
 
+## Example 6
+
+Access the current working directory with optional parameter `frozen` to determine
+different directories when script is bundled to an executable,
+e.g. with `pyinstaller`.
+> `Path.cwd()`
+
+```cmd
+>>> poetry run examples/example6.py -b
+Building frozen: K:/pathlibutil/examples/example6.exe
+Build succeeded: 0
+
+>>> poetry run examples/example6.py
+we are                          not frozen
+
+bundle dir is                   K:/pathlibutil/examples
+sys.argv[0] is                  K:/pathlibutil/examples/example6.py
+sys.executable is               K:/pathlibutil/.venv/Scripts/python.exe
+os.getcwd is                    K:/pathlibutil
+
+Path.cwd(frozen=True) is        K:/pathlibutil
+Path.cwd(frozen=False) is       K:/pathlibutil
+Path.cwd(frozen=_MEIPASS) is    K:/pathlibutil
+
+>>> examples/example6.exe
+we are                          ever so frozen
+
+bundle dir is                   C:/Users/CHRIST~1.DOE/AppData/Local/Temp/_MEI106042
+sys.argv[0] is                  examples/example6.exe
+sys.executable is               K:/pathlibutil/examples/example6.exe
+os.getcwd is                    K:/pathlibutil
+
+Path.cwd(frozen=True) is        K:/pathlibutil/examples
+Path.cwd(frozen=False) is       K:/pathlibutil
+Path.cwd(frozen=_MEIPASS) is    C:/Users/CHRIST~1.DOE/AppData/Local/Temp/_MEI106042
+```
+
```

