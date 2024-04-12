# Comparing `tmp/bin_package_manager-2.2.4.tar.gz` & `tmp/bin_package_manager-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bin_package_manager-2.2.4.tar", max compression
+gzip compressed data, was "bin_package_manager-2.2.5.tar", max compression
```

## Comparing `bin_package_manager-2.2.4.tar` & `bin_package_manager-2.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.4/LICENSE
--rw-r--r--   0        0        0     3822 2024-04-08 16:38:00.593122 bin_package_manager-2.2.4/README.md
--rw-r--r--   0        0        0      184 2024-03-25 08:16:31.955639 bin_package_manager-2.2.4/bpm/__init__.py
--rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.4/bpm/__main__.py
--rw-r--r--   0        0        0     4031 2024-04-08 16:23:47.314764 bin_package_manager-2.2.4/bpm/cli.py
--rw-r--r--   0        0        0     6855 2024-04-08 16:26:54.032376 bin_package_manager-2.2.4/bpm/command.py
--rw-r--r--   0        0        0    17653 2024-04-08 17:12:36.984564 bin_package_manager-2.2.4/bpm/install/__init__.py
--rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.4/bpm/lib/windowspathadder.py
--rw-r--r--   0        0        0    11303 2024-04-08 17:12:41.197879 bin_package_manager-2.2.4/bpm/search.py
--rw-r--r--   0        0        0     4410 2024-03-06 14:53:06.937647 bin_package_manager-2.2.4/bpm/storage.py
--rw-r--r--   0        0        0     3882 2024-03-25 08:19:26.282328 bin_package_manager-2.2.4/bpm/utils/__init__.py
--rw-r--r--   0        0        0      545 2024-04-08 17:12:31.247925 bin_package_manager-2.2.4/bpm/utils/constants.py
--rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.4/bpm/utils/exceptions.py
--rw-r--r--   0        0        0     1026 2024-04-08 17:12:45.534529 bin_package_manager-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     4728 1970-01-01 00:00:00.000000 bin_package_manager-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-02-03 15:14:27.236806 bin_package_manager-2.2.5/LICENSE
+-rw-r--r--   0        0        0     3907 2024-04-12 17:44:29.537756 bin_package_manager-2.2.5/README.md
+-rw-r--r--   0        0        0      211 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/__init__.py
+-rw-r--r--   0        0        0       61 2024-02-14 06:21:44.497403 bin_package_manager-2.2.5/bpm/__main__.py
+-rw-r--r--   0        0        0     4119 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/cli.py
+-rw-r--r--   0        0        0     6946 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/command.py
+-rw-r--r--   0        0        0    17654 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/install/__init__.py
+-rw-r--r--   0        0        0     4103 2024-02-19 11:56:44.850635 bin_package_manager-2.2.5/bpm/lib/windowspathadder.py
+-rw-r--r--   0        0        0    12254 2024-04-12 17:42:26.398806 bin_package_manager-2.2.5/bpm/search.py
+-rw-r--r--   0        0        0     4449 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/storage.py
+-rw-r--r--   0        0        0     3913 2024-04-12 17:41:05.452840 bin_package_manager-2.2.5/bpm/utils/__init__.py
+-rw-r--r--   0        0        0      526 2024-04-12 12:39:24.674496 bin_package_manager-2.2.5/bpm/utils/constants.py
+-rw-r--r--   0        0        0      988 2024-02-21 10:21:37.512797 bin_package_manager-2.2.5/bpm/utils/exceptions.py
+-rw-r--r--   0        0        0     1003 2024-04-12 17:43:02.785161 bin_package_manager-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4819 1970-01-01 00:00:00.000000 bin_package_manager-2.2.5/PKG-INFO
```

### Comparing `bin_package_manager-2.2.4/LICENSE` & `bin_package_manager-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.4/README.md` & `bin_package_manager-2.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # bin package manager
 
 English | [简体中文](./docs/README.zh-CN.md)
 
 Bin package manager (BPM) is a Github release-based package manager that allows users to install and manage binaries from any Github release.
 
-BPM is currently supported on Linux and Windows, python >= 3.10.
+BPM is currently supported on Linux and Windows, python >= 3.9.
 
 > [!CAUTION]
 > Risk Warning: BPM on Linux may damage your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
 
 ## Why use it?
 
 In non-rolling release Linux distributions, the version of softwares in official source are often too low to use some new features.
@@ -65,15 +65,15 @@
 ## Usage
 
 - Install: `bpm i <package>`
 - Run `bpm -h` and `bpm i -h` for more help.
 
 ```
 ❯ bpm i -h
-usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--sort [SORT]] packages [packages ...]
+usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--filter [FILTER ...]] [--sort [SORT]] packages [packages ...]
 
 positional arguments:
   packages              Package name or github url to install
 
 options:
   -h, --help            show this help message and exit
   -b [BIN_NAME], --bin-name [BIN_NAME]
@@ -81,14 +81,16 @@
   -l [Archive], --local [Archive]
                         install from local archive.
   -q, --quiet           not ask, install the best match repo.
   --one-bin             install given binary only. Use package name as binary name by default.
   --prefer-gnu          bpm prefers musl target by default, you can change this default option.
   -n, --dry-run         print the install position, but not install actually.
   -i, --interactive     select asset interactively.
+  --filter [FILTER ...]
+                        filter assets
   --sort [SORT]         sort param in github api, use `best-match` by default. The value could be `stars`, `forks`, `help-wanted-
                         issues`, `updated`.
 ```
 
 ## How it works
 
 ### Linux
```

### Comparing `bin_package_manager-2.2.4/bpm/cli.py` & `bin_package_manager-2.2.5/bpm/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
 install_parser.add_argument(
     "-i",
     "--interactive",
     action="store_true",
     help="select asset interactively.",
 )
 install_parser.add_argument(
+    "--filter",
+    nargs="*",
+    help="filter assets",
+)
+install_parser.add_argument(
     "--sort",
     nargs="?",
     type=lambda value: value_in(
         value, ["stars", "forks", "help-wanted-issues", "updated"]
     ),
     help="sort param in github api, use `best-match` by default. The value could be `stars`, `forks`, `help-wanted-issues`, `updated`.",
 )
```

### Comparing `bin_package_manager-2.2.4/bpm/command.py` & `bin_package_manager-2.2.5/bpm/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging as log
+from copy import copy
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from urllib.parse import urlparse
 
-from simpleufcs import UFCS
-
 from .install import auto_install, download_and_extract, extract, remove
 from .search import RepoHandler
 from .storage import repo_group
 from .utils import check_root, error_exit, set_dry_run, trace
 from .utils.constants import BIN_PATH, WINDOWS
 from .utils.exceptions import RepoNotFoundError
 
@@ -61,23 +60,25 @@
         try:
             if is_url:
                 repo = (
                     RepoHandler(
                         real_name,
                         prefer_gnu=args.prefer_gnu,
                         one_bin=args.one_bin,
+                        asset_filter=args.filter,
                     )
                     .set_by_url(package)
                     .with_bin_name(args.bin_name)
                 )
             else:
                 repo = RepoHandler(
                     package,
                     prefer_gnu=args.prefer_gnu,
                     one_bin=args.one_bin,
+                    asset_filter=args.filter,
                 ).with_bin_name(args.bin_name)
                 if not args.local:
                     repo.ask(quiet=args.quiet, sort=args.sort)
             if not args.local:
                 repo.get_asset(interactive=args.interactive)
         except Exception as e:
             log.error(f"Failed on searching `{package}`: {e}")
@@ -85,20 +86,18 @@
             exit(1)
 
         # install
         try:
             download_and_install(args, repo)
             log.info(f"Successfully installed `{repo.name}`.")
             if WINDOWS:
-                bins = (
-                    UFCS(repo.file_list)
-                    .filter(lambda x: x.endswith(".lnk"))
-                    .map(lambda x: Path(x).stem)
-                    .map(lambda x: f"`{x}`")
-                )
+                bins = copy(repo.file_list)
+                bins = filter(lambda x: x.endswith(".lnk"), bins)
+                bins = map(lambda x: Path(x).stem, bins)
+                bins = map(lambda x: f"`{x}`", bins)
                 log.info(
                     f"You can press `Win+r`, enter {', '.join(bins)} to start software, or execute in cmd."
                 )
             if not args.dry_run:
                 repo_group.insert_repo(repo)
         except Exception as e:
             log.error(f"Failed to install `{repo.name}`: {e}")
@@ -140,15 +139,16 @@
 def cli_update(args):
     check_root()
     failed = []
 
     def update(repo: RepoHandler):
         try:
             log.info(f"Updating `{repo.name}`...")
-            if result := repo.update_asset():
+            result = repo.update_asset()
+            if result:
                 log.info(
                     f"`{repo.name}` has an update: {result[0]} -> {result[1]}. Updating..."
                 )
                 download_and_install(args, repo, rename=False)
                 log.info(f"`{repo.name}` updated successfully.")
             else:
                 log.info(f"`{repo.name}` is the newest.")
```

### Comparing `bin_package_manager-2.2.4/bpm/install/__init__.py` & `bin_package_manager-2.2.5/bpm/install/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import platform
 import shutil
 import tarfile
 import zipfile
 from contextlib import suppress
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Optional
+from typing import Optional, Union
 
 import requests
 import tqdm
 
 import bpm.utils as utils
 
 from ..search import RepoHandler
@@ -63,16 +63,16 @@
     shutil.copy2(_from, _to)
     log.info(f"{_from} -> {_to}")
     record()
     mode and _to.chmod(mode)
 
 
 def merge_dir(
-    _from: Path | str,
-    _to: Path | str,
+    _from: Union[Path, str],
+    _to: Union[Path, str],
     rename: bool = True,
     recorder: Optional[list[str]] = None,
 ):
     """
     Install one dir and all files to another.
 
     `rename`: Whether the overlap files to be renamed to `*.old`. If rename, the previous `*.old` file will be replaced.
@@ -158,35 +158,36 @@
         if not Path(member).resolve().is_relative_to(root_dir):
             return False
     return True
 
 
 def extract(buffer: io.BytesIO, to_dir: Path) -> Path:
     """
-    extract tar | zip | 7z to dir.
+    extract tar / zip / 7z to dir.
 
     `Returns`: the "main" path of extracted files.
     """
     try:
         with tarfile.open(fileobj=buffer, mode="r") as file:
             if not check_if_tar_safe(file):
                 raise TarPathTraversalException
             file.extractall(path=to_dir)
     except tarfile.ReadError:
+        buffer.seek(0)
         try:
             with zipfile.ZipFile(buffer, "r") as file:
                 file.extractall(path=to_dir)
         except zipfile.BadZipFile:
+            buffer.seek(0)
             try:
                 import py7zr
             except ImportError:
                 utils.error_exit("cannot extract 7z file without py7zr module.")
 
-            with py7zr.SevenZipFile(buffer, "r") as file:
-                file.extractall(path=to_dir)
+            py7zr.SevenZipFile(buffer, "r").extractall(path=to_dir)
 
     temp = list(to_dir.glob("*"))
     if len(temp) == 1 and temp[0].is_dir():
         return temp[0]
     return to_dir
 
 
@@ -302,33 +303,33 @@
         first_layer.remove(bin)
         install_bin(bin)
         if one_bin:
             return
 
     for file in first_layer:
         # 2. merge all files to coordinate position
-        match file.name:
-            case "lib":
-                merge_dir(file, pkgdst / "lib", rename=rename, recorder=recorder)
-            case "include":
-                merge_dir(file, pkgdst / "include", rename=rename, recorder=recorder)
-            case "share":
-                merge_dir(file, pkgdst / "share", rename=rename, recorder=recorder)
-            case "bin":
-                merge_dir(file, pkgdst / "bin", rename=rename, recorder=recorder)
-            case "man":
-                merge_dir(file, pkgdst / "share/man", rename=rename, recorder=recorder)
-            # 3. deal with other circumstance.
-            case name:
-                if name.startswith("complet"):
-                    install_completions(file)
-                elif name == bin_name and file.is_file():
-                    install_bin(file)
-                else:
-                    log.debug(f"cannot match {name}.")
+        if file.name == "lib":
+            merge_dir(file, pkgdst / "lib", rename=rename, recorder=recorder)
+        elif file.name == "include":
+            merge_dir(file, pkgdst / "include", rename=rename, recorder=recorder)
+        elif file.name == "share":
+            merge_dir(file, pkgdst / "share", rename=rename, recorder=recorder)
+        elif file.name == "bin":
+            merge_dir(file, pkgdst / "bin", rename=rename, recorder=recorder)
+        elif file.name == "man":
+            merge_dir(file, pkgdst / "share/man", rename=rename, recorder=recorder)
+        # 3. deal with other circumstance.
+        else:
+            name = file.name
+            if name.startswith("complet"):
+                install_completions(file)
+            elif name == bin_name and file.is_file():
+                install_bin(file)
+            else:
+                log.debug(f"cannot match {name}.")
 
     # check binary
     if not any(map(lambda x: x.startswith("/usr/bin"), recorder)):
         log.warning("No binary file found, please check the release package.")
 
 
 def install_on_windows(
@@ -415,23 +416,22 @@
     pkgsrc: Path,
     rename: bool = True,
 ):
     """
     Install by different platforms.
     """
 
-    match platform.system():
-        case "Linux":
-            install_on_linux(
-                pkgsrc, repo.bin_name, repo.one_bin, rename, repo.installed_files
-            )
-        case "Windows":
-            install_on_windows(repo, pkgsrc)
-        case _:
-            raise NotImplementedError(f"{platform.system()} is not supported now.")
+    if platform.system() == "Linux":
+        install_on_linux(
+            pkgsrc, repo.bin_name, repo.one_bin, rename, repo.installed_files
+        )
+    elif platform.system() == "Windows":
+        install_on_windows(repo, pkgsrc)
+    else:
+        raise NotImplementedError(f"{platform.system()} is not supported now.")
 
 
 import unittest  # noqa: E402
 
 
 class Test(unittest.TestCase):
     def test_rename_old_and_rev(self):
```

### Comparing `bin_package_manager-2.2.4/bpm/lib/windowspathadder.py` & `bin_package_manager-2.2.5/bpm/lib/windowspathadder.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.4/bpm/search.py` & `bin_package_manager-2.2.5/bpm/search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,46 @@
+# ruff: noqa: E731
+
+import functools
 import logging as log
 import platform
 import posixpath
 import sys
 from enum import Enum
 from functools import reduce
 from pprint import pprint
-from typing import Optional
+from typing import Optional, Union
 from urllib.parse import urljoin, urlparse
 
 import requests
 
-from .utils import select_interactive
+from .utils import multi_in, select_interactive
 from .utils.constants import INFO_BASE_STRING, OPTION_REPO_NUM, WINDOWS
 from .utils.exceptions import AssetNotFoundError, InvalidAssetError, RepoNotFoundError
 
 
 class Combination(Enum):
     """
     Enum for the different ways of combining the select_list and prompt.
     """
 
     ALL = 0
     ANY = 1
 
 
+class MatchPos(Enum):
+    """
+    Enum for the str matching position
+    """
+
+    ALL = 0
+    BEGIN = 1
+    END = 2
+
+
 def select_list(
     select_list: list[str],
     prompts: list[str],
     combination: Combination = Combination.ALL,
     case_sensitive=False,
 ) -> list[str]:
     """
@@ -40,60 +53,82 @@
     ['12', '13']
     >>> select_list(["12", "13", "23", "34"], ["1", "2"], Combination.ANY)
     ['12', '13', '23']
     >>> select_list(["12", "13", "23", "34", "21"], ["1", "2"], Combination.ALL)
     ['12', '21']
     """
     comb_func = any if combination == Combination.ANY else all
-    is_valid = lambda s: comb_func(  # noqa: E731
+    is_valid = lambda s: comb_func(
         map(
             (lambda x: x in s)
             if case_sensitive
             else (lambda x: x.lower() in s.lower()),
             prompts,
         )
     )
     return list(filter(is_valid, select_list)) or select_list
 
 
 def sort_list(
     sort_list: list[str],
     prompts: list[str],
-    combination: Combination = Combination.ALL,
+    combination=Combination.ALL,
+    match_pos=MatchPos.ALL,
     case_sensitive=False,
 ) -> list[str]:
     """
     Sort items from the given list and return.
 
     :param combination: ALL => every prompt should in the word, ANY => one or more prompt in the word.
 
 
     >>> sort_list(["12", "13", "23"], ["2"])
     ['12', '23', '13']
     """
     comb_func = any if combination == Combination.ANY else all
-    is_valid = lambda s: comb_func(  # noqa: E731
+    if match_pos == MatchPos.ALL:
+        match_func = lambda a, b: a not in b
+    elif match_pos == MatchPos.BEGIN:
+        match_func = lambda a, b: not b.beginswith(a)
+    elif match_pos == MatchPos.END:
+        match_func = lambda a, b: not b.endswith(a)
+
+    is_valid = lambda s: comb_func(
         map(
-            (lambda x: x not in s)
+            (lambda x: match_func(x, s))
             if case_sensitive
-            else (lambda x: x.lower() not in s.lower()),
+            else (lambda x: match_func(x.lower(), s.lower())),
             prompts,
         )
     )
     return sorted(sort_list, key=is_valid)
 
 
+@functools.lru_cache()
+def platform_map() -> list:
+    return [platform.system()]
+
+
+@functools.lru_cache()
+def architecture_map():
+    if platform.machine() == "AMD64":
+        return ["x86_64", "amd64"]
+    else:
+        return [platform.machine()]
+
+
 class RepoHandler:
     def __init__(self, name: str, **kwargs):
         self.name = name
         self.bin_name = name
         self.site = "github"
         self.repo_name = None
         self.repo_owner = None
         self.asset = None
+        self.asset_filter = []
         self.version = None
         self.installed_files: list[str] = []
         self.prefer_gnu: bool = False
         self.no_pre: bool = False
         self.one_bin: bool = False
 
         self.set(**kwargs)
@@ -107,20 +142,32 @@
 
     def __lt__(self, other: "RepoHandler"):
         return self.name < other.name
 
     def __eq__(self, __value: object) -> bool:
         return self.name == __value.name
 
+    def __getstate__(self):
+        state = self.__dict__.copy()
+        return state
+
+    def __setstate__(self, state):
+        """
+        Add backward Compatibility
+        """
+        self.__dict__.update(state)
+        if "asset_filter" not in state:
+            self.asset_filter = []
+
     def set(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
         return self
 
-    def with_bin_name(self, bin_name: str | None):
+    def with_bin_name(self, bin_name: Union[str, None]):
         if WINDOWS:
             self.bin_name = bin_name.rstrip(".exe") + ".exe" if bin_name else "*.exe"
         else:
             self.bin_name = bin_name or self.name
         return self
 
     @property
@@ -129,19 +176,18 @@
             return None
         return urljoin(
             f"https://{self.site}.com/", posixpath.join(self.repo_owner, self.repo_name)
         )
 
     @property
     def api_base(self):
-        match self.site:
-            case "github":
-                return "https://api.github.com"
-            case _:
-                raise NotImplementedError
+        if self.site == "github":
+            return "https://api.github.com"
+        else:
+            raise NotImplementedError
 
     @property
     def file_list(self) -> list[str]:
         """
         Get the "IndexSet" of `installed_files`.
         """
         # same as `unique` function, keep them
@@ -272,48 +318,48 @@
         assets: list[str] = [x["browser_download_url"] for x in r[0]["assets"]]
 
         if interactive:
             self.asset = select_interactive(assets)
             log.info(f"selected asset: {self.asset}")
             return self
 
+        # asset filter
+        if self.asset_filter:
+            assets = list(filter(lambda a: multi_in(self.asset_filter, a), assets))
+
         # select
         # 1. platform
-        pltfm = (
-            [platform.system().lower(), "win"]
-            if WINDOWS and "win" not in self.name.lower()
-            else [platform.system().lower()]
-        )
-        assets = select_list(assets, pltfm, Combination.ANY)
+        log.debug(f"platform filter: {platform_map()}")
+        assets = select_list(assets, platform_map(), Combination.ANY)
+        log.debug(f"platform selected assets: {assets}")
+
         # 2. architecture
-        arch = (
-            [platform.machine().lower()]
-            if platform.machine().lower() != "amd64"
-            else ["amd64", "x86_64"]
-        )
-        assets = select_list(assets, arch, Combination.ANY)
+        log.debug(f"architecture filter: {architecture_map()}")
+        assets = select_list(assets, architecture_map(), Combination.ANY)
+
         # 3. musl or gnu
         if not self.prefer_gnu:
             assets = sort_list(assets, ["musl"])
+
         # 4. tar, zip, 7z, other
-        assets = sorted(assets, key=lambda x: not x.endswith(".7z"))
+        assets = sort_list(assets, [".7z"], match_pos=MatchPos.END)
         if WINDOWS:
-            assets = sorted(assets, key=lambda x: ".tar." not in x)
-            assets = sorted(assets, key=lambda x: not x.endswith(".zip"))
+            assets = sort_list(assets, [".tar."])
+            assets = sort_list(assets, [".zip"], match_pos=MatchPos.END)
         else:
-            assets = sorted(assets, key=lambda x: not x.endswith(".zip"))
-            assets = sorted(assets, key=lambda x: ".tar." not in x)
+            assets = sort_list(assets, [".zip"], match_pos=MatchPos.END)
+            assets = sort_list(assets, [".tar."])
 
         if not assets:
             raise InvalidAssetError
         self.asset = assets[0]
         log.info(f"selected asset: {self.asset}")
         return self
 
-    def update_asset(self) -> Optional[tuple[str, str] | tuple[None, None]]:
+    def update_asset(self) -> Optional[Union[tuple[str, str], tuple[None, None]]]:
         """
         update assets list. If a repo was installed locally, it will always return (None, None).
 
         `Returns`: `None` if has no update, `(old_version, new_version)` if has update.
         """
         old_version = self.version
         if not old_version:
```

### Comparing `bin_package_manager-2.2.4/bpm/storage.py` & `bin_package_manager-2.2.5/bpm/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import bisect
 import logging as log
 import pickle
 from contextlib import suppress
 from pathlib import Path
 from pprint import pprint
 from tempfile import TemporaryDirectory
-from typing import Optional
+from typing import Optional, Union
 
 from .search import RepoHandler
 from .utils.constants import DATABASE_PATH, INFO_BASE_STRING, WINDOWS
 from .utils.exceptions import RepoNotFoundError
 
 
 class RepoGroup:
@@ -29,27 +29,29 @@
         self.db_path.write_bytes(pickle.dumps(self.repos))
 
     def info_repos(self):
         print(INFO_BASE_STRING.format("Name", "Url", "Version"))
         for repo in self.repos:
             print(repo)
 
-    def find_repo(self, repo: str | RepoHandler) -> tuple[int, Optional[RepoHandler]]:
+    def find_repo(
+        self, repo: Union[str, RepoHandler]
+    ) -> tuple[int, Optional[RepoHandler]]:
         """
         Find a repo.
         return the index and the object of repo.
         """
         if isinstance(repo, str):
             repo = RepoHandler(repo)
         index = bisect.bisect_left(self.repos, repo)
         if index != len(self.repos) and self.repos[index] == repo:
             return (index, self.repos[index])
         return (-1, None)
 
-    def info_one_repo(self, repo: str | RepoHandler) -> RepoHandler:
+    def info_one_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
         """
         Print ALL messages about one repo.
         If not found, raise exception `RepoNotFoundError`.
         """
         _, result = self.find_repo(repo)
         if result:
             pprint(vars(result))
@@ -61,15 +63,15 @@
         """
         Insert repo to RepoGroup, and save.
         """
         index = bisect.bisect_left(self.repos, repo)
         self.repos.insert(index, repo)
         self.save()
 
-    def remove_repo(self, repo: str | RepoHandler) -> RepoHandler:
+    def remove_repo(self, repo: Union[str, RepoHandler]) -> RepoHandler:
         """
         Remove repo and save.
         """
         index, result = self.find_repo(repo)
         if result:
             self.repos.pop(index)
             self.save()
```

### Comparing `bin_package_manager-2.2.4/bpm/utils/__init__.py` & `bin_package_manager-2.2.5/bpm/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging as log
 import os
 import posixpath
 import sys
 import tempfile
 import traceback
 from pathlib import Path, WindowsPath
+from typing import Union
 
 from ..lib.windowspathadder import add_windows_path
 from .constants import BIN_PATH, LINUX, WINDOWS
 
 TEST = False
 
 
@@ -52,15 +53,15 @@
     """
     Trace back only in debug mode.
     """
     if log.getLogger().isEnabledFor(log.DEBUG):
         traceback.print_exc()
 
 
-def multi_in(parts: list | str, total: str):
+def multi_in(parts: list, total: str):
     """
     return any strings in the list is a part of one string.
     """
     if isinstance(parts, str):
         parts = [parts]
     return any(x in total for x in parts)
 
@@ -89,28 +90,28 @@
                 f"Invalid choice. Please enter a number between 1 and {len(options)}."
             )
         except KeyboardInterrupt:
             print("Interrupted by user.")
             exit(0)
 
 
-def windows_path_to_windows_bash(p: WindowsPath | str) -> str:
+def windows_path_to_windows_bash(p: Union[WindowsPath, str]) -> str:
     """
     convert a windows path to posix path string. example:
 
     >>> windows_path_to_windows_bash("C:\\Users\\lxl\\bpm\\bin")
     "/c/Users/lxl/bpm/bin"
     """
     p = WindowsPath(p)
     return posixpath.join(
         "/", p.drive.rstrip(":").lower(), p.relative_to(p.anchor).as_posix()
     )
 
 
-def windows_path_to_wsl(p: WindowsPath | str) -> str:
+def windows_path_to_wsl(p: Union[WindowsPath, str]) -> str:
     """
     convert a windows path to wsl path string. example:
 
     >>> windows_path_to_wsl("C:\\Users\\lxl\\bpm\\bin")
     "/mnt/c/Users/lxl/bpm/bin"
     """
```

### Comparing `bin_package_manager-2.2.4/bpm/utils/exceptions.py` & `bin_package_manager-2.2.5/bpm/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `bin_package_manager-2.2.4/pyproject.toml` & `bin_package_manager-2.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bin-package-manager"
-version = "2.2.4"
+version = "2.2.5"
 description = "Bin package manager, a package manager based on Github release"
 authors = ["lxl66566 <lxl66566@gmail.com>"]
 license = "MIT"
 readme = ["README.md"]
 keywords = ["binary", "packaging", "release"]
 repository = "https://github.com/lxl66566/bpm"
 homepage = "https://github.com/lxl66566/bpm"
@@ -12,20 +12,19 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 packages = [{ include = "bpm" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 py7zr = { version = "^0.20.8", markers = "sys_platform == 'win32'" }
 requests = "^2.31.0"
 tqdm = "^4.66.2"
 pylnk3 = { version = "^0.4.2", markers = "sys_platform == 'win32'" }
-simpleufcs = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 bpm = 'bpm.cli:main'
```

### Comparing `bin_package_manager-2.2.4/PKG-INFO` & `bin_package_manager-2.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: bin-package-manager
-Version: 2.2.4
+Version: 2.2.5
 Summary: Bin package manager, a package manager based on Github release
 Home-page: https://github.com/lxl66566/bpm
 License: MIT
 Keywords: binary,packaging,release
 Author: lxl66566
 Author-email: lxl66566@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: py7zr (>=0.20.8,<0.21.0) ; sys_platform == "win32"
 Requires-Dist: pylnk3 (>=0.4.2,<0.5.0) ; sys_platform == "win32"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: simpleufcs (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/lxl66566/bpm
 Description-Content-Type: text/markdown
 
 # bin package manager
 
 English | [简体中文](./docs/README.zh-CN.md)
 
 Bin package manager (BPM) is a Github release-based package manager that allows users to install and manage binaries from any Github release.
 
-BPM is currently supported on Linux and Windows, python >= 3.10.
+BPM is currently supported on Linux and Windows, python >= 3.9.
 
 > [!CAUTION]
 > Risk Warning: BPM on Linux may damage your computer. By using BPM to install software, you accept this risk and trust third-party Github release packagers.
 
 ## Why use it?
 
 In non-rolling release Linux distributions, the version of softwares in official source are often too low to use some new features.
@@ -88,15 +88,15 @@
 ## Usage
 
 - Install: `bpm i <package>`
 - Run `bpm -h` and `bpm i -h` for more help.
 
 ```
 ❯ bpm i -h
-usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--sort [SORT]] packages [packages ...]
+usage: bpm install [-h] [-b [BIN_NAME]] [-l [Archive]] [-q] [--one-bin] [--prefer-gnu] [-n] [-i] [--filter [FILTER ...]] [--sort [SORT]] packages [packages ...]
 
 positional arguments:
   packages              Package name or github url to install
 
 options:
   -h, --help            show this help message and exit
   -b [BIN_NAME], --bin-name [BIN_NAME]
@@ -104,14 +104,16 @@
   -l [Archive], --local [Archive]
                         install from local archive.
   -q, --quiet           not ask, install the best match repo.
   --one-bin             install given binary only. Use package name as binary name by default.
   --prefer-gnu          bpm prefers musl target by default, you can change this default option.
   -n, --dry-run         print the install position, but not install actually.
   -i, --interactive     select asset interactively.
+  --filter [FILTER ...]
+                        filter assets
   --sort [SORT]         sort param in github api, use `best-match` by default. The value could be `stars`, `forks`, `help-wanted-
                         issues`, `updated`.
 ```
 
 ## How it works
 
 ### Linux
```

