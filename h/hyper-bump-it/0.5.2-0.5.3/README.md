# Comparing `tmp/hyper-bump-it-0.5.2.tar.gz` & `tmp/hyper_bump_it-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-bump-it-0.5.2.tar", last modified: Sat Sep  9 20:28:25 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hyper-bump-it-0.5.2.tar` & `hyper_bump_it-0.5.3.tar`

### file list

```diff
@@ -1,53 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.772659 hyper-bump-it-0.5.2/hyper_bump_it/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.772659 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/by.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9817 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/to.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17041 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/planned_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/vcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/hyper_bump_it/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-09 20:28:25.772659 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-09 20:28:25.000000 hyper-bump-it-0.5.2/hyper_bump_it.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-09 20:28:25.776659 hyper-bump-it-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-09-09 20:28:07.000000 hyper-bump-it-0.5.2/setup.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/py.typed
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/compat.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/core.py
+-rw-r--r--   0        0        0    17042 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/error.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/execution_plan.py
+-rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/files.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/planned_changes.py
+-rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/ui.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/vcs.py
+-rw-r--r--   0        0        0     5232 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/version.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/__init__.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/by.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/common.py
+-rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/init.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/to.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
+-rw-r--r--   0        0        0     9818 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
+-rw-r--r--   0        0        0    12454 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/__init__.py
+-rw-r--r--   0        0        0     6624 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/application.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/cli.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/core.py
+-rw-r--r--   0        0        0    10505 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/file.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/LICENSE
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/README.md
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 hyper_bump_it-0.5.3/PKG-INFO
```

### Comparing `hyper-bump-it-0.5.2/LICENSE` & `hyper_bump_it-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/PKG-INFO` & `hyper_bump_it-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hyper-bump-it
-Version: 0.5.2
+Version: 0.5.3
 Summary: A version bumping tool
-Author-email: Patrick Lannigan <p.lannigan@gmail.com>
-License: MIT
 Project-URL: homepage, https://github.com/plannigan/hyper-bump-it
 Project-URL: changelog, https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/plannigan/hyper-bump-it/issues
 Project-URL: documentation, https://plannigan.github.io/hyper-bump-it
-Keywords: version,bump,command line
+Author-email: Patrick Lannigan <p.lannigan@gmail.com>
+License: MIT
+License-File: LICENSE
+Keywords: bump,command line,version
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <4.0,>=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: GitPython<4,>=3.1.35
-Requires-Dist: tomlkit<1.0,>=0.11.6
-Requires-Dist: typer<1.0,>=0.9.0
+Requires-Dist: gitpython<4,>=3.1.35
 Requires-Dist: pydantic<3,>=2.1.0
 Requires-Dist: rich<14,>=12.6.0
-Requires-Dist: typing-extensions<5,>=4.4.0; python_version < "3.11"
+Requires-Dist: tomlkit<1.0,>=0.11.6
+Requires-Dist: typer<1.0,>=0.9.0
+Requires-Dist: typing-extensions<5,>=4.4.0; python_version < '3.11'
+Description-Content-Type: text/markdown
 
 [![CI pipeline status](https://github.com/plannigan/hyper-bump-it/actions/workflows/main.yml/badge.svg?branch=main)][ci]
 [![PyPI](https://img.shields.io/pypi/v/hyper-bump-it)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
```

### Comparing `hyper-bump-it-0.5.2/README.md` & `hyper_bump_it-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/by.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Bump version by part command.
 """
+
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
 
 from .. import core
 from ..config import BumpByArgs, BumpPart, GitAction, config_for_bump_by
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/common.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Common command line functionality.
 """
+
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Any, Iterator, NoReturn, Optional, Protocol, overload
 
 import typer
 from rich.align import AlignMethod
 
@@ -19,16 +20,15 @@
 ERROR_PANEL_TILE_ALIGN_: AlignMethod = "left"
 EXAMPLE_FILE_GLOB = "version.txt"
 
 
 class OptionFactory(Protocol):
     def __call__(  # type: ignore[misc]
         self, panel_name: str = ..., show_default: bool = ...
-    ) -> Any:
-        ...
+    ) -> Any: ...
 
 
 def _create_option_factory(description: str, *param_decls: str) -> OptionFactory:
     def _create_option(  # type: ignore[misc]
         panel_name: str = OVERRIDE_PANEL_NAME, show_default: bool = False
     ) -> Any:
         return typer.Option(
@@ -42,15 +42,15 @@
 
 
 CONFIG_FILE = typer.Option(
     help="Path to dedicated configuration file to use instead of normal file discovery",
     show_default=False,
 )
 CONFIG_FILE_DEFAULT: Optional[Path] = None
-PROJECT_ROOT = typer.Option(  # type: ignore[call-overload]
+PROJECT_ROOT = typer.Option(
     help="Path to directory containing the project",
     show_default="Use current directory",
 )
 PROJECT_ROOT_DEFAULT = Path.cwd()
 DRY_RUN = typer.Option(
     "--no",
     "-n",
@@ -140,18 +140,16 @@
         border_style="red",
         title="Error",
     )
     raise typer.Exit(exit_code)
 
 
 @overload
-def resolve(path: Path) -> Path:
-    ...
+def resolve(path: Path) -> Path: ...
 
 
 @overload
-def resolve(path: Optional[Path]) -> Optional[Path]:
-    ...
+def resolve(path: Optional[Path]) -> Optional[Path]: ...
 
 
 def resolve(path: Optional[Path]) -> Optional[Path]:
     return None if path is None else path.resolve()
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/init.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Initialize configuration command.
 """
+
 from pathlib import Path
 from typing import Annotated, Mapping
 
 import tomlkit
 import typer
 from pydantic import ValidationError
 from rich.text import Text
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Validate a file definition to see if it could be used for a specific project.
 """
+
 from dataclasses import dataclass
 from enum import Enum, auto
 from pathlib import Path
 from typing import Optional
 
 from rich.text import Text
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Go through a series of prompts to construct a custom files configuration.
 """
+
 from enum import Enum
 from typing import Optional
 
 from rich.text import Text
 
 from ... import ui
 from ...config import DEFAULT_SEARCH_PATTERN, FileDefinition
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Go through a series of prompts to construct a custom Git integration configuration.
 """
+
 from enum import Enum
 from typing import Optional, TypeVar, Union
 
 from pydantic import ValidationError
 from rich.text import Text
 
 from ... import ui
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Go through a series of prompts to construct a custom configuration.
 """
+
 from enum import Enum
 from pathlib import Path
 from typing import Set
 
 from rich.text import Text
 
 from ... import ui
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/cli/to.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/cli/to.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Bump to version command.
 """
+
 from pathlib import Path
 from typing import Annotated, Optional
 
 import typer
 
 from .. import core
 from ..config import BumpToArgs, GitAction, config_for_bump_to
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/compat.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Consolidate Python version compatibility code.
 """
+
 import sys
 
 # flake8: noqa: F401
 
 if sys.version_info < (3, 10):
     from typing_extensions import TypeAlias as TypeAlias  # this supports python < 3.10
 else:
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/__init__.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/application.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Program configuration
 """
+
 from dataclasses import astuple, dataclass
 from pathlib import Path
 from typing import Callable, Optional, Union, cast
 
 from ..error import KeystoneFileGlobError
 from ..version import Version
 from . import file, keystone_parser
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/cli.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/cli.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/core.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/core.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/file.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,33 @@
     ) -> "GitActions":
         validate_git_action_combination(
             commit=self.commit, branch=self.branch, tag=self.tag
         )
         return self
 
 
+def _check_branches(
+    value: Optional[object], handler: ValidatorFunctionWrapHandler
+) -> frozenset[str]:
+    if isinstance(value, list):
+        value = frozenset(value)
+    return cast(frozenset[str], handler(value))
+
+
+PossiblyListBranches = Annotated[frozenset[str], WrapValidator(_check_branches)]
+
+
 class Git(HyperBaseMode):
     remote: str = DEFAULT_REMOTE
     commit_format_pattern: str = DEFAULT_COMMIT_FORMAT_PATTERN
     branch_format_pattern: str = DEFAULT_BRANCH_FORMAT_PATTERN
     tag_name_format_pattern: str = DEFAULT_TAG_NAME_FORMAT_PATTERN
     tag_message_format_pattern: str = DEFAULT_TAG_MESSAGE_FORMAT_PATTERN
-    allowed_initial_branches: frozenset[str] = DEFAULT_ALLOWED_INITIAL_BRANCHES
-    extend_allowed_initial_branches: frozenset[str] = frozenset()
+    allowed_initial_branches: PossiblyListBranches = DEFAULT_ALLOWED_INITIAL_BRANCHES
+    extend_allowed_initial_branches: PossiblyListBranches = frozenset()
     actions: GitActions = GitActions()
 
 
 class File(HyperBaseMode):
     file_glob: str  # relative to project root directory
     keystone: bool = False
     search_format_pattern: str = DEFAULT_SEARCH_PATTERN
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Use format patterns to produce regular expression matching patterns to determine the current
 version from a keystone file.
 """
+
 from pathlib import Path
 from re import Match
 from typing import Optional
 
 from ..error import IncompleteKeystoneVersionError, VersionNotFound
 from ..format_pattern import create_matching_pattern, keys
 from ..version import Version
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/core.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/core.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/error.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Errors raised by the library.
 """
+
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable, Collection, Literal, TypeVar, Union
 
 from pydantic import ValidationError
 from rich.text import Text
 
 from . import ui
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/execution_plan.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/execution_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Structured plan of what operations will be performed.
 
 The plan is created before performing any operations so that the user can confirm the changes
 to be made before files are edited.
 """
+
 from typing import Optional, Protocol, TypeVar
 
 from git import Repo
 from rich.text import Text
 
 from . import files, ui, vcs
 from .compat import LiteralString
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/files.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/files.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Convert a search pattern into a regex pattern.
 """
+
 import re
 from re import Pattern
 from string import Formatter, Template
 from typing import Optional
 
 from ..error import FormatKeyError, FormatPatternError, TodayFormatKeyError
 from . import keys
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Central place for performing text formatting.
 """
+
 from datetime import date
 from enum import Enum, auto
 from string import Formatter
 from typing import Optional
 
 from ..error import FormatKeyError, FormatPatternError
 from ..version import Version
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/planned_changes.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/planned_changes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Low level primitives for file interactions.
 """
+
 import difflib
 from dataclasses import InitVar, dataclass, field
 from functools import cached_property
 from pathlib import Path
 from typing import Optional
 
 _LINE_FEED = b"\n"[0]
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/ui.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Display interface for working with rich.
 """
+
 from collections.abc import Iterable, Mapping
 from enum import Enum
 from typing import Optional, TypeVar, Union, cast, overload
 
 from rich import prompt
 from rich.align import AlignMethod
 from rich.console import Console, RichCast
@@ -68,21 +69,19 @@
 ) -> None:
     _CONSOLE.print(
         Panel(message, title=title, title_align=title_align, border_style=border_style)
     )
 
 
 @overload
-def ask(message: TextType, *, default: str = ...) -> str:
-    ...
+def ask(message: TextType, *, default: str = ...) -> str: ...
 
 
 @overload
-def ask(message: TextType, *, default: None) -> Optional[str]:
-    ...
+def ask(message: TextType, *, default: None) -> Optional[str]: ...
 
 
 def ask(message: TextType, *, default: Optional[str] = None) -> Optional[str]:
     return prompt.Prompt.ask(
         message, default=default, show_default=False, console=_CONSOLE
     )
 
@@ -98,23 +97,21 @@
 T = TypeVar("T")
 _NOT_GIVEN = _Sentinel.A
 
 
 @overload
 def choice(
     message: Text, *, choices: list[str], default: str = ..., show_choices: bool = False
-) -> str:
-    ...
+) -> str: ...
 
 
 @overload
 def choice(
     message: Text, *, choices: list[str], default: None, show_choices: bool = False
-) -> Optional[str]:
-    ...
+) -> Optional[str]: ...
 
 
 def choice(
     message: Text,
     *,
     choices: list[str],
     default: Union[Optional[str], _Sentinel] = _NOT_GIVEN,
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/vcs.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/vcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Operation on git repositories.
 """
+
 from dataclasses import dataclass
 from pathlib import Path
 
 from git import InvalidGitRepositoryError, Repo
 
 from .config import Git, GitAction, GitActions
 from .error import (
@@ -129,16 +130,18 @@
 
 def create_tag(repo: Repo, tag_name: str, tag_message: str) -> None:
     repo.create_tag(tag_name, message=tag_message)
 
 
 def push_changes(repo: Repo, operation_info: GitOperationsInfo) -> None:
     to_push = [
-        operation_info.branch_name
-        if operation_info.actions.branch == GitAction.CreateAndPush
-        else repo.active_branch.name
+        (
+            operation_info.branch_name
+            if operation_info.actions.branch == GitAction.CreateAndPush
+            else repo.active_branch.name
+        )
     ]
     if operation_info.actions.tag == GitAction.CreateAndPush:
         to_push.append(operation_info.tag_name)
 
     remote = repo.remotes[operation_info.remote]
     remote.push(to_push, atomic=True)
```

### Comparing `hyper-bump-it-0.5.2/hyper_bump_it/_hyper_bump_it/version.py` & `hyper_bump_it-0.5.3/hyper_bump_it/_hyper_bump_it/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Semantic version parsing and data structure.
 """
+
 import re
 from dataclasses import dataclass
 from functools import cached_property, total_ordering
 from typing import Union
 
 from .compat import TypeAlias
```

### Comparing `hyper-bump-it-0.5.2/pyproject.toml` & `hyper_bump_it-0.5.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+[build-system]
+requires = ["hatchling==1.22.5"]
+build-backend = "hatchling.build"
+
+
 [project]
 name = "hyper-bump-it"
-version = "0.5.2"
+version = "0.5.3"
 description = "A version bumping tool"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 license = {text = "MIT"}
 dependencies = [
     "GitPython>=3.1.35,<4",
     "tomlkit>=0.11.6,<1.0",
@@ -14,14 +19,15 @@
     "typing-extensions>=4.4.0,<5; python_version < '3.11'",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
 ]
 keywords = [
     "version",
     "bump",
     "command line"
@@ -35,23 +41,89 @@
 changelog = "https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md"
 issues = "https://github.com/plannigan/hyper-bump-it/issues"
 documentation = "https://plannigan.github.io/hyper-bump-it"
 
 [project.scripts]
 hyper-bump-it = "hyper_bump_it._hyper_bump_it.cli:app"
 
-[build-system]
-requires = ["setuptools >= 61.0.0"]
-build-backend = "setuptools.build_meta"
+[tool.hatch.build.targets.sdist]
+include = [
+    "/hyper_bump_it",
+]
 
-[tool.setuptools.packages.find]
-exclude = ["*.tests", "*.tests.*", "tests.*", "tests"]
+# environment management & scripts
+[tool.hatch.envs.default]
+description = "Test and lint the project code"
+dependencies = [
+    "bandit==1.7.8",
+    "black==24.3.0",
+    "coverage==7.4.4",
+    "flake8==7.0.0",
+    "isort==5.13.2",
+    "mypy==1.9.0",
+    "pytest==8.1.1",
+    "pytest-cov==5.0.0",
+    "pytest-freezer==0.4.8",
+    "pytest-mock==3.14.0",
+    "pdbpp==0.10.3",
+]
+[tool.hatch.envs.default.scripts]
+test-no-cov = "pytest --no-cov {args}"
+test = "pytest --cov-report html {args}"
+test-ci = "pytest {args}"
+typing = "mypy"
+_fmt = [
+    "black --quiet .",
+    "isort .",
+]
+black-check = "black --check --diff ."
+isort-check = "isort --check-only ."
+flake8-check = "flake8"
+bandit-ci = "bandit --ini .bandit -r ."
+bandit-check = "bandit-ci --quiet"
+check-strict = [
+    "black-check",
+    "isort-check",
+    "typing",
+    "test",
+    "flake8-check",
+    "bandit-check",
+]
+check = [
+    "_fmt",
+    "typing",
+    "test",
+    "flake8-check",
+    "bandit-check",
+]
+test-docs-examples = [
+    "./docker/validate_docs.sh"
+]
+
+[tool.hatch.envs.bump]
+description = "Release a new version"
+detached = true
+dependencies = [
+    "hyper-bump-it==0.5.2"
+]
+[tool.hatch.envs.bump.scripts]
+it = "hyper-bump-it {args}"
+
+[tool.hatch.envs.docs]
+description = "Generate documentation for the project"
+dependencies = [
+    "mike==2.0.0",
+    "markdown-include==0.8.1",
+    "mkdocs==1.5.3",
+    "mkdocs-material==9.5.17",
+]
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build --strict"
+serve = "mkdocs serve --dev-addr=0.0.0.0:8000"
 
-[tool.setuptools.package-data]
-hyper_bump_it = ["py.typed"]
 
 # type checking
 [tool.mypy]
 files = "hyper_bump_it"
 show_error_codes = true
 warn_unused_configs = true
 pretty = true
@@ -71,16 +143,17 @@
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 
 # testing
 [tool.pytest.ini_options]
-addopts = "--verbose --cov=hyper_bump_it --cov-report xml:/tmp/coverage.xml --cov-report term-missing:skip-covered"
+addopts = "--cov=hyper_bump_it --cov-report xml:/tmp/coverage.xml --cov-report term-missing:skip-covered"
 testpaths = ["tests"]
+verbosity_assertions = 2
 
 [tool.coverage.run]
 branch = true
 data_file = "/tmp/hyper_bump_it_coverage"
 
 [tool.coverage.report]
 fail_under = 90
```

