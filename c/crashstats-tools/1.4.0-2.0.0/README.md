# Comparing `tmp/crashstats-tools-1.4.0.tar.gz` & `tmp/crashstats_tools-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crashstats-tools-1.4.0.tar", last modified: Fri Nov 18 22:23:00 2022, max compression
+gzip compressed data, was "crashstats_tools-2.tar", last modified: Fri Apr 12 19:06:50 2024, max compression
```

## Comparing `crashstats-tools-1.4.0.tar` & `crashstats_tools-2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2019-04-02 20:07:00.000000 crashstats-tools-1.4.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2908 2022-11-18 22:21:06.000000 crashstats-tools-1.4.0/HISTORY.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2018-06-14 23:11:50.000000 crashstats-tools-1.4.0/LICENSE
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      243 2020-05-21 20:24:16.000000 crashstats-tools-1.4.0/MANIFEST.in
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      805 2022-11-09 22:20:37.000000 crashstats-tools-1.4.0/Makefile
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     9175 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8250 2022-11-18 21:49:06.000000 crashstats-tools-1.4.0/README.rst
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      174 2022-11-18 22:09:50.000000 crashstats-tools-1.4.0/requirements-dev.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       99 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/setup.cfg
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     2230 2022-11-18 22:22:13.000000 crashstats-tools-1.4.0/setup.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/src/
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/src/crashstats_tools/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      296 2022-11-18 22:21:06.000000 crashstats-tools-1.4.0/src/crashstats_tools/__init__.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     8817 2022-11-18 21:59:19.000000 crashstats-tools-1.4.0/src/crashstats_tools/cmd_fetch_data.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     5175 2022-11-18 21:59:19.000000 crashstats-tools-1.4.0/src/crashstats_tools/cmd_reprocess.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     9861 2022-11-18 21:12:21.000000 crashstats-tools-1.4.0/src/crashstats_tools/cmd_supersearch.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)    13262 2022-11-18 21:31:32.000000 crashstats-tools-1.4.0/src/crashstats_tools/cmd_supersearchfacet.py
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     9964 2022-11-18 21:12:21.000000 crashstats-tools-1.4.0/src/crashstats_tools/utils.py
-drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2022-11-18 22:23:00.623597 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/
--rw-rw-r--   0 willkg    (1000) willkg    (1000)     9175 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/PKG-INFO
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      609 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      260 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/entry_points.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       35 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/requires.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)       17 2022-11-18 22:23:00.000000 crashstats-tools-1.4.0/src/crashstats_tools.egg-info/top_level.txt
--rw-rw-r--   0 willkg    (1000) willkg    (1000)      433 2022-11-09 22:24:55.000000 crashstats-tools-1.4.0/tox.ini
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-12 19:06:50.173867 crashstats_tools-2/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      691 2019-04-02 20:07:00.000000 crashstats_tools-2/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     3669 2024-04-12 19:05:59.000000 crashstats_tools-2/HISTORY.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    15977 2018-06-14 23:11:50.000000 crashstats_tools-2/LICENSE
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      243 2020-05-21 20:24:16.000000 crashstats_tools-2/MANIFEST.in
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      650 2023-12-27 23:31:14.000000 crashstats_tools-2/Makefile
+-rw-r--r--   0 willkg    (1000) willkg    (1000)    24590 2024-04-12 19:06:50.173867 crashstats_tools-2/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    22804 2024-04-12 18:18:52.000000 crashstats_tools-2/README.rst
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     2562 2024-04-12 19:05:59.000000 crashstats_tools-2/pyproject.toml
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       38 2024-04-12 19:06:50.173867 crashstats_tools-2/setup.cfg
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-12 19:06:50.173867 crashstats_tools-2/src/
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-12 19:06:50.173867 crashstats_tools-2/src/crashstats_tools/
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      415 2023-12-27 23:31:14.000000 crashstats_tools-2/src/crashstats_tools/__init__.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8564 2024-04-12 18:18:52.000000 crashstats_tools-2/src/crashstats_tools/cmd_fetch_data.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     5869 2024-04-12 15:47:25.000000 crashstats_tools-2/src/crashstats_tools/cmd_reprocess.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     8913 2024-04-12 18:18:52.000000 crashstats_tools-2/src/crashstats_tools/cmd_supersearch.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    18016 2024-04-12 18:43:45.000000 crashstats_tools-2/src/crashstats_tools/cmd_supersearchfacet.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)     5718 2024-04-12 18:18:52.000000 crashstats_tools-2/src/crashstats_tools/libcrashstats.py
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)    13628 2024-04-12 18:33:03.000000 crashstats_tools-2/src/crashstats_tools/utils.py
+drwxrwxr-x   0 willkg    (1000) willkg    (1000)        0 2024-04-12 19:06:50.173867 crashstats_tools-2/src/crashstats_tools.egg-info/
+-rw-r--r--   0 willkg    (1000) willkg    (1000)    24590 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      614 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)        1 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      264 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)      185 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/requires.txt
+-rw-rw-r--   0 willkg    (1000) willkg    (1000)       17 2024-04-12 19:06:50.000000 crashstats_tools-2/src/crashstats_tools.egg-info/top_level.txt
```

### Comparing `crashstats-tools-1.4.0/CODE_OF_CONDUCT.md` & `crashstats_tools-2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `crashstats-tools-1.4.0/HISTORY.rst` & `crashstats_tools-2/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 =======
 History
 =======
 
+2.0.0 (April 12th, 2024)
+========================
+
+Changes:
+
+* Radically improve README documentation.
+* Add estimates to reprocess command. (#80)
+* Add support for "csv" format for supersearch and supersearchfacet. (#88)
+* Drop support for Python 3.7. (#90)
+* Add support for Python 3.12. (#91)
+* Add "raw" format for better debugging.
+* Add ``_histogram`` support. (#98)
+* Add ``--denote-weekends`` to supersearchfacet. (#54)
+* Implement parallelization for fetch-data. (#106)
+* Implement ``--leftover-count`` and ``--no-leftover-count`` for supersearchfacet. (#109)
+* Fix user-agent to reflect crashstats-tools version. (#121)
+* Add support for nested aggs and cardinality. (#102, #103)
+* Move functions for Crash Stats API to libcrashstats library. (#67)
+
+
 1.4.0 (November 18th, 2022)
 ===========================
 
 Changes:
 
 * Fix supersearch to kick up a usage error when you use columns that don't
   exist or that you don't have access to. (#61)
```

### Comparing `crashstats-tools-1.4.0/LICENSE` & `crashstats_tools-2/LICENSE`

 * *Files identical despite different names*

### Comparing `crashstats-tools-1.4.0/Makefile` & `crashstats_tools-2/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 .PHONY: clean
 clean:  ## Clean build artifacts
 	rm -rf build dist src/${PROJECT}.egg-info .tox .pytest_cache/
 	rm -rf docs/_build/*
 	find src tests/ -name __pycache__ | xargs rm -rf
 	find src tests/ -name '*.pyc' | xargs rm -rf
 
+.PHONY: format
+format:  ## Format files
+	tox exec -e py38-lint -- ruff format
+
 .PHONY: lint
-lint:  ## Lint and black reformat files
-	black --target-version=py37 --line-length=88 setup.py src tests
-	tox -e py37-lint
+lint:  ## Lint files
+	tox -e py38-lint
 
 .PHONY: test
 test:  ## Run tests
 	tox
 
-.PHONY: checkrot
-checkrot:  ## Check package rot for dev dependencies
-	python -m venv ./tmpvenv/
-	./tmpvenv/bin/pip install -U pip
-	./tmpvenv/bin/pip install -r requirements-dev.txt
-	./tmpvenv/bin/pip list -o
-	rm -rf ./tmpvenv/
+.PHONY: docs
+docs:  ## Update README with fresh cog output
+	cog -r README.rst
```

### Comparing `crashstats-tools-1.4.0/setup.py` & `crashstats_tools-2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,110 @@
-#!/usr/bin/env python
-
-# This Source Code Form is subject to the terms of the Mozilla Public
-# License, v. 2.0. If a copy of the MPL was not distributed with this
-# file, You can obtain one at http://mozilla.org/MPL/2.0/.
-
-import codecs
-import os
-import re
-
-from setuptools import find_packages, setup
-
-
-def get_long_desc():
-    return codecs.open("README.rst", encoding="utf-8").read()
-
-
-def get_version():
-    fn = os.path.join("src", "crashstats_tools", "__init__.py")
-    vsre = r"""^__version__ = ['"]([^'"]*)['"]"""
-    version_file = codecs.open(fn, mode="r", encoding="utf-8").read()
-    return re.search(vsre, version_file, re.M).group(1)
-
-
-INSTALL_REQUIRES = ["click", "more_itertools", "requests", "rich"]
-EXTRAS_REQUIRE = {}
-
-
-setup(
-    name="crashstats-tools",
-    version=get_version(),
-    description="Tools for working with Crash Stats (https://crash-stats.mozilla.org/)",
-    long_description=get_long_desc(),
-    maintainer="Will Kahn-Greene",
-    maintainer_email="willkg@mozilla.com",
-    url="https://github.com/willkg/crashstats-tools",
-    license="Mozilla Public License v2",
-    include_package_data=True,
-    packages=find_packages(where="src"),
-    package_dir={"": "src"},
-    install_requires=INSTALL_REQUIRES,
-    extras_require=EXTRAS_REQUIRE,
-    python_requires=">=3.7",
-    entry_points="""
-        [console_scripts]
-        fetch-data=crashstats_tools.cmd_fetch_data:fetch_data
-        reprocess=crashstats_tools.cmd_reprocess:reprocess
-        supersearch=crashstats_tools.cmd_supersearch:supersearch
-        supersearchfacet=crashstats_tools.cmd_supersearchfacet:supersearchfacet
-    """,
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-)
+[project]
+name = "crashstats-tools"
+description = "Tools for working with Crash Stats (https://crash-stats.mozilla.org/)"
+version = "2.0.0"
+readme = "README.rst"
+keywords = ["socorro"]
+authors = [{name = "Will Kahn-Greene"}]
+license = {text = "MPLv2"}
+requires-python = ">=3.8"
+dependencies = [
+    "click",
+    "more_itertools",
+    "requests",
+    "rich",
+    "tomli>=1.1.0; python_version < '3.11'",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
+    "Natural Language :: English",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+]
+urls.Homepage = "https://github.com/willkg/crashstats-tools"
+urls.Source = "https://github.com/willkg/crashstats-tools"
+urls.Issues = "https://github.com/willkg/crashstats-tools"
+
+[project.scripts]
+fetch-data = "crashstats_tools.cmd_fetch_data:fetch_data"
+reprocess = "crashstats_tools.cmd_reprocess:reprocess"
+supersearch = "crashstats_tools.cmd_supersearch:supersearch_cli"
+supersearchfacet = "crashstats_tools.cmd_supersearchfacet:supersearchfacet"
+
+[project.optional-dependencies]
+dev = [
+    "build",
+    "check-manifest",
+    "cogapp",
+    "freezegun",
+    "pytest",
+    "responses",
+    "ruff",
+    "setuptools",
+    "tox",
+    "tox-gh-actions",
+    "twine",
+    "wheel",
+]
+
+
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
+
+
+[tool.ruff]
+target-version = "py38"
+src = ["src"]
+line-length = 88
+
+[tool.ruff.lint]
+# Enable pycodestyle (E), pyflakes (F), and bugbear (B) rules
+select = ["E", "F", "B"]
+
+# Ignore line-length violations; ruff format does its best and we can rely on
+# that
+ignore = ["E501"]
+
+[tool.ruff.lint.flake8-quotes]
+docstring-quotes = "double"
+
+
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+isolated_build = True
+envlist =
+    py38
+    py38-lint
+    py39
+    py310
+    py311
+    py312
+
+[gh-actions]
+python =
+    3.8: py38
+    3.9: py39
+    3.10: py310
+    3.11: py311
+    3.12: py312
+
+[testenv]
+extras = dev
+commands = pytest {posargs}
+
+[testenv:py38-lint]
+basepython = python3.8
+changedir = {toxinidir}
+commands =
+    ruff format --check src tests
+    ruff check src tests
+"""
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools/cmd_fetch_data.py` & `crashstats_tools-2/src/crashstats_tools/cmd_fetch_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,133 +1,128 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+from functools import partial
 import json
+from multiprocessing import Pool
 import os
 import sys
 
 import click
 from rich.console import Console
 
-from crashstats_tools.utils import DEFAULT_HOST, http_get, JsonDTEncoder, parse_crashid
+from crashstats_tools.libcrashstats import (
+    get_crash_annotations,
+    get_dump,
+    get_processed_crash,
+)
+from crashstats_tools.utils import (
+    DEFAULT_HOST,
+    JsonDTEncoder,
+    parse_crash_id,
+)
 
 
 def create_dir_if_needed(d):
     if not os.path.exists(d):
         os.makedirs(d)
 
 
 def fetch_crash(
-    console,
+    crash_id,
     host,
+    api_token,
     fetchraw,
     fetchdumps,
     fetchprocessed,
     outputdir,
-    api_token,
-    crash_id,
+    color,
     overwrite,
 ):
     """Fetch crash data and save to correct place on the file system
 
     https://antenna.readthedocs.io/en/latest/overview.html#aws-s3-file-hierarchy
 
     """
+    if not color:
+        console = Console(color_system=None)
+    else:
+        console = Console()
+
+    try:
+        crash_id = parse_crash_id(crash_id).strip()
+    except ValueError:
+        console.print(f"[yellow]{crash_id}: not a valid crash id[/yellow]")
+        return
+
     if fetchraw:
         # Fetch raw crash metadata to OUTPUTDIR/raw_crash/DATE/CRASHID
         fn = os.path.join(outputdir, "raw_crash", "20" + crash_id[-6:], crash_id)
         if os.path.exists(fn) and not overwrite:
-            console.print(
-                f"[bold green]Fetching raw {crash_id}[/bold green] ... already exists"
-            )
+            console.print(f"{crash_id}: fetching raw crash -- already exists")
         else:
-            console.print(f"[bold green]Fetching raw {crash_id}[/bold green]")
-            resp = http_get(
-                url=host + "/api/RawCrash/",
-                params={"crash_id": crash_id, "format": "meta"},
-                api_token=api_token,
-            )
+            console.print(f"{crash_id}: fetching raw crash")
+            raw_crash = get_crash_annotations(crash_id, host=host, api_token=api_token)
 
             # Save raw crash to file system
-            raw_crash = resp.json()
             create_dir_if_needed(os.path.dirname(fn))
             with open(fn, "w") as fp:
                 json.dump(raw_crash, fp, cls=JsonDTEncoder, indent=2, sort_keys=True)
 
         if fetchdumps:
             # Save dump_names to file system
             dump_names = raw_crash.get("metadata", {}).get("dump_checksums", {}).keys()
             fn = os.path.join(outputdir, "dump_names", crash_id)
             create_dir_if_needed(os.path.dirname(fn))
             with open(fn, "w") as fp:
                 json.dump(list(dump_names), fp)
 
             # Fetch dumps
             for dump_name in dump_names:
-
                 # We store "upload_file_minidump" as "dump", so we need to use that
                 # name when requesting from the RawCrash api
                 file_name = dump_name
                 if file_name == "upload_file_minidump":
                     file_name = "dump"
 
                 fn = os.path.join(outputdir, dump_name, crash_id)
                 if os.path.exists(fn) and not overwrite:
                     console.print(
-                        f"[bold green]Fetching dump {crash_id}/{dump_name}[/bold green] ... "
-                        + "already exists"
+                        f"{crash_id}: fetching dump: {dump_name} -- already exists"
                     )
                 else:
-                    console.print(
-                        f"[bold green]Fetching dump {crash_id}/{dump_name}[/bold green]"
+                    console.print(f"{crash_id}: fetching dump: {dump_name}")
+                    dump_content = get_dump(
+                        crash_id, dump_name=file_name, api_token=api_token, host=host
                     )
-                    resp = http_get(
-                        url=host + "/api/RawCrash/",
-                        params={
-                            "crash_id": crash_id,
-                            "format": "raw",
-                            "name": file_name,
-                        },
-                        api_token=api_token,
-                    )
-
-                    if resp.status_code != 200:
-                        raise Exception(
-                            f"Something unexpected happened. status_code {resp.status_code}, "
-                            + f"content {resp.content}"
-                        )
-
                     create_dir_if_needed(os.path.dirname(fn))
                     with open(fn, "wb") as fp:
-                        fp.write(resp.content)
+                        fp.write(dump_content)
 
     if fetchprocessed:
         # Fetch processed crash data
         fn = os.path.join(outputdir, "processed_crash", crash_id)
         if os.path.exists(fn) and not overwrite:
-            console.print(
-                f"[bold green]Fetching processed {crash_id}[/bold green] ... "
-                + "already exists"
-            )
+            console.print(f"{crash_id}: fetching processed crash -- already exists")
         else:
-            console.print(f"[bold green]Fetching processed {crash_id}[/bold green]")
-            resp = http_get(
-                host + "/api/ProcessedCrash/",
-                params={"crash_id": crash_id, "format": "meta"},
-                api_token=api_token,
+            console.print(f"{crash_id}: fetching processed crash")
+            processed_crash = get_processed_crash(
+                crash_id, api_token=api_token, host=host
             )
 
             # Save processed crash to file system
             create_dir_if_needed(os.path.dirname(fn))
             with open(fn, "w") as fp:
-                json.dump(resp.json(), fp, cls=JsonDTEncoder, indent=2, sort_keys=True)
+                json.dump(
+                    processed_crash, fp, cls=JsonDTEncoder, indent=2, sort_keys=True
+                )
 
 
-@click.command()
+@click.command(context_settings={"show_default": True})
 @click.option(
     "--host",
     default=DEFAULT_HOST,
     help="host to pull crash data from; this needs to match CRASHSTATS_API_TOKEN value",
 )
 @click.option(
     "--overwrite/--no-overwrite",
@@ -149,68 +144,75 @@
 @click.option(
     "--processed/--no-processed",
     "fetchprocessed",
     default=False,
     help="whether or not to save processed crash data",
 )
 @click.option(
+    "--workers",
+    default=1,
+    type=click.IntRange(1, 10, clamp=True),
+    help="how many workers to use to download data; requires CRASHSTATS_API_TOKEN",
+)
+@click.option(
     "--color/--no-color",
     default=True,
     help=(
         "whether or not to colorize output; note that color is shut off "
         "when stdout is not an interactive terminal automatically"
     ),
 )
 @click.argument("outputdir")
-@click.argument("crashids", nargs=-1)
+@click.argument("crash_ids", nargs=-1)
 @click.pass_context
 def fetch_data(
     ctx,
     host,
     overwrite,
     fetchraw,
     fetchdumps,
     fetchprocessed,
+    workers,
     color,
     outputdir,
-    crashids,
+    crash_ids,
 ):
     """
     Fetches crash data from Crash Stats (https://crash-stats.mozilla.org/) system.
 
     Given one or more crash ids via command line or stdin (one per line), fetches
     crash data and puts it in specified directory.
 
     Crash data is split up into directories: raw_crash/, dump_names/,
     processed_crash/, and directories with the same name as the dump type.
 
     https://antenna.readthedocs.io/en/latest/overview.html#aws-s3-file-hierarchy
 
-    This requires an API token in order to download dumps, personally identifiable
-    information, and security-sensitive data. It also reduces rate-limiting.  Set
-    the CRASHSTATS_API_TOKEN environment variable to your API token value:
+    This requires an API token in order to download dumps and protected data.
+    Using an API token also reduces rate-limiting. Set the CRASHSTATS_API_TOKEN
+    environment variable to your API token value:
 
     CRASHSTATS_API_TOKEN=xyz fetch-data crashdata ...
 
     To create an API token for Crash Stats, visit:
 
     https://crash-stats.mozilla.org/api/tokens/
 
     Remember to abide by the data access policy when using data from Crash Stats!
     The policy is specified here:
 
-    https://crash-stats.mozilla.org/documentation/memory_dump_access/
+    https://crash-stats.mozilla.org/documentation/protected_data_access/
     """
-    host = host.rstrip("/")
-
     if not color:
         console = Console(color_system=None)
     else:
         console = Console()
 
+    host = host.rstrip("/")
+
     if fetchdumps and not fetchraw:
         raise click.BadOptionUsage(
             "fetchdumps",
             "You cannot fetch dumps without also fetching the raw crash.",
             ctx=ctx,
         )
 
@@ -218,54 +220,57 @@
     if os.path.exists(outputdir) and not os.path.isdir(outputdir):
         raise click.ClickException(f"{outputdir} is not a directory.")
 
     # Sort out API token existence
     api_token = os.environ.get("CRASHSTATS_API_TOKEN")
     if api_token:
         masked_token = api_token[:4] + ("x" * (len(api_token) - 4))
-        console.print(f"Using api token: {masked_token}")
+        console.print(f"Using API token: {masked_token}")
     else:
         console.print(
-            "[yellow]No api token provided. Set CRASHSTATS_API_TOKEN in the "
+            "[yellow]No API token provided. Set CRASHSTATS_API_TOKEN in the "
             + "environment.[/yellow]"
         )
-        console.print(
-            "[yellow]Skipping dumps and personally identifiable "
-            + "information.[/yellow]"
-        )
+        console.print("[yellow]Skipping dumps and protected data.[/yellow]")
+
+    if workers > 1:
+        if not api_token:
+            raise click.BadOptionUsage(
+                "workers",
+                "You must specify a CRASHSTATS_API_TOKEN in order to set workers > 1.",
+                ctx=ctx,
+            )
+        console.print(f"Using {workers} workers.")
 
     if fetchdumps and not api_token:
         raise click.BadOptionUsage(
             "fetchdumps",
             "You cannot fetch dumps without providing an API token.",
             ctx=ctx,
         )
 
-    if not crashids and not sys.stdin.isatty():
-        crashids = list(click.get_text_stream("stdin").readlines())
+    if not crash_ids and not sys.stdin.isatty():
+        crash_ids = list(click.get_text_stream("stdin").readlines())
 
-    for crashid in crashids:
-        crashid = crashid.strip()
+    fetch_crash_partial = partial(
+        fetch_crash,
+        host=host,
+        api_token=api_token,
+        fetchraw=fetchraw,
+        fetchdumps=fetchdumps,
+        fetchprocessed=fetchprocessed,
+        color=color,
+        outputdir=outputdir,
+        overwrite=overwrite,
+    )
+
+    if workers > 1:
+        with Pool(workers) as p:
+            p.map(fetch_crash_partial, crash_ids)
 
-        try:
-            crashid = parse_crashid(crashid).strip()
-        except ValueError:
-            console.print(f"[yellow]Crash id not recognized: {crashid}[/yellow]")
-            continue
-
-        console.print(f"[bold green]Working on {crashid}...[/bold green]")
-        fetch_crash(
-            console=console,
-            host=host,
-            fetchraw=fetchraw,
-            fetchdumps=fetchdumps,
-            fetchprocessed=fetchprocessed,
-            outputdir=outputdir,
-            api_token=api_token,
-            crash_id=crashid,
-            overwrite=overwrite,
-        )
-    console.print("[bold green]Done![/bold green]")
+    else:
+        for crash_id in crash_ids:
+            fetch_crash_partial(crash_id)
 
 
 if __name__ == "__main__":
     fetch_data()
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools/cmd_reprocess.py` & `crashstats_tools-2/src/crashstats_tools/cmd_reprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+from datetime import timedelta
 import os
 import sys
 import time
 
 import click
 from rich.console import Console
 from more_itertools import chunked
 
-from crashstats_tools.utils import DEFAULT_HOST, http_post, parse_crashid
+from crashstats_tools.utils import (
+    DEFAULT_HOST,
+    http_post,
+    parse_crash_id,
+)
 
 
 CHUNK_SIZE = 50
 SLEEP_DEFAULT = 1
 
 
-@click.command()
+@click.command(context_settings={"show_default": True})
 @click.option(
     "--host",
     default=DEFAULT_HOST,
     show_default=True,
     help="host for system to reprocess in",
 )
 @click.option(
@@ -82,33 +87,33 @@
     else:
         console = Console()
         error_console = Console(stderr=True)
 
     api_token = os.environ.get("CRASHSTATS_API_TOKEN")
     if not api_token:
         error_console.print(
-            "[yellow]No api token provided. Set CRASHSTATS_API_TOKEN in the "
+            "[yellow]No API token provided. Set CRASHSTATS_API_TOKEN in the "
             + "environment.[/yellow]"
         )
         ctx.exit(1)
 
     masked_token = api_token[:4] + ("x" * (len(api_token) - 4))
-    console.print(f"Using api token: {masked_token}")
+    console.print(f"Using API token: {masked_token}")
 
     url = host.rstrip("/") + "/api/Reprocessing/"
     console.print(f"[bold green]Sending reprocessing requests to: {url}[/bold green]")
 
     if not crashids and not sys.stdin.isatty():
         crashids = list(click.get_text_stream("stdin").readlines())
 
     to_process = []
     for crashid in crashids:
         crashid = crashid.strip()
         try:
-            crashid = parse_crashid(crashid).strip()
+            crashid = parse_crash_id(crashid).strip()
         except ValueError:
             console.print(f"[yellow]Crash id not recognized: {crashid}[/yellow]")
             continue
 
         to_process.append(crashid)
 
     if not to_process:
@@ -116,45 +121,62 @@
             message="No crashids specified.",
             ctx=ctx,
             param="crashids",
             param_hint="crashids",
         )
 
     console.print(
-        f"[bold green]Reprocessing {len(to_process)} crashes sleeping {sleep} "
+        f"[bold green]Reprocessing {len(to_process):,} crashes sleeping {sleep} "
         + "seconds between groups...[/bold green]"
     )
+    estimate = timedelta(seconds=int(len(to_process) / CHUNK_SIZE * (sleep + 0.5)))
+    console.print(f"[bold green]Rough estimate: {estimate}")
 
     if len(to_process) > 10000 and not allow_many:
         console.print(
             "[yellow]You are trying to reprocess more than 10,000 crash reports "
             + "at once.[/yellow]"
         )
         console.print(
             "[yellow]Please let us know on #crashreporting on Matrix before you "
             + "do this.[/yellow]"
         )
         console.print("")
         console.print("[yellow]Use --allow-many argument to reprocess.[/yellow]")
         ctx.exit(1)
 
+    start_time = time.time()
+
     groups = list(chunked(to_process, CHUNK_SIZE))
     for i, group in enumerate(groups):
         if i > 0:
             # NOTE(willkg): We sleep here because the webapp has a bunch of rate
             # limiting and we don't want to trigger that. It'd be nice if we didn't
             # have to do this.
             time.sleep(sleep)
 
         last_crashid = group[-1]
         this_group = i + 1
         total_groups = len(groups)
+
+        # Calculate a running estimate, but only after 5 groups when it starts
+        # to stabilize
+        if i < 5:
+            estimate = ""
+        else:
+            seconds_per_group = int((time.time() - start_time) / (this_group + 1))
+            estimate = str(
+                timedelta(seconds=seconds_per_group * (len(groups) - this_group + 1))
+            )
+
         console.print(
-            f"Processing group ending with {last_crashid} ... "
-            + f"({this_group}/{total_groups})"
+            (
+                f"Processing group ending with {last_crashid} ... "
+                + f"({this_group}/{total_groups}) {estimate}"
+            ).strip()
         )
 
         if ruleset:
             group = [f"{crashid}:{ruleset}" for crashid in group]
 
         resp = http_post(url, data={"crash_ids": group}, api_token=api_token)
         if resp.status_code != 200:
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools/cmd_supersearch.py` & `crashstats_tools-2/src/crashstats_tools/cmd_supersearch.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,85 +7,28 @@
 import os
 from urllib.parse import urlparse, parse_qs
 
 import click
 from rich.console import Console
 from rich.table import Table
 
+from crashstats_tools.libcrashstats import supersearch
 from crashstats_tools.utils import (
-    escape_whitespace,
+    ConsoleLogger,
     DEFAULT_HOST,
-    http_get,
+    escape_whitespace,
     INFINITY,
     MissingField,
     parse_args,
+    tableize_csv,
     tableize_markdown,
     tableize_tab,
 )
 
 
-MAX_PAGE = 1000
-
-
-def fetch_supersearch(
-    console, host, params, num_results, api_token=None, verbose=False
-):
-    """Generator that returns Super Search results
-
-    :arg str host: the host to query
-    :arg dict params: dict of super search parameters to base the query on
-    :arg varies num: number of results to get or INFINITY
-    :arg str api_token: the API token to use or None
-    :arg bool verbose: whether or not to print verbose things
-
-    :returns: generator of crash ids
-
-    """
-    url = host + "/api/SuperSearch/"
-
-    # Set up first page
-    params["_results_offset"] = 0
-    params["_results_number"] = min(MAX_PAGE, num_results)
-
-    # Fetch pages of crash ids until we've gotten as many as we want or there
-    # aren't any more to get
-    crashids_count = 0
-    while True:
-        if verbose:
-            console.print(url, params)
-
-        resp = http_get(url=url, params=params, api_token=api_token)
-        hits = resp.json()["hits"]
-
-        for hit in hits:
-            crashids_count += 1
-            yield hit
-
-            # If we've gotten as many crashids as we need, we return
-            if crashids_count >= num_results:
-                return
-
-        # If there are no more crash ids to get, we return
-        total = resp.json()["total"]
-        if not hits or crashids_count >= total:
-            return
-
-        # Get the next page, but only as many results as we need
-        params["_results_offset"] += MAX_PAGE
-        params["_results_number"] = min(
-            # MAX_PAGE is the maximum we can request
-            MAX_PAGE,
-            # The number of results Super Search can return to us that is
-            # hasn't returned so far
-            total - crashids_count,
-            # The numver of results we want that we haven't gotten, yet
-            num_results - crashids_count,
-        )
-
-
 def extract_supersearch_params(url):
     """Parses out params from the query string and drops any aggs-related ones."""
     parsed = urlparse(url)
     params = parse_qs(parsed.query)
 
     # Remove any aggs
     aggs_keys = ("_facets", "_aggs", "_histogram", "_cardinality")
@@ -93,15 +36,20 @@
         if key.startswith(aggs_keys):
             del params[key]
 
     return params
 
 
 @click.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
+    name="supersearch",
+    context_settings={
+        "show_default": True,
+        "allow_extra_args": True,
+        "ignore_unknown_options": True,
+    },
 )
 @click.option(
     "--host",
     default=DEFAULT_HOST,
     show_default=True,
     help="host for system to fetch crashids from",
 )
@@ -120,82 +68,90 @@
     help="whether or not to show table headers",
 )
 @click.option(
     "--format",
     "format_type",
     default="tab",
     show_default=True,
-    type=click.Choice(["table", "tab", "json", "markdown"], case_sensitive=False),
+    type=click.Choice(
+        ["table", "tab", "csv", "json", "markdown"], case_sensitive=False
+    ),
     help="format to print output",
 )
 @click.option(
     "--verbose/--no-verbose", default=False, help="whether to print debugging output"
 )
 @click.option(
     "--color/--no-color",
     default=True,
     help=(
         "whether or not to colorize output; note that color is shut off "
         "when stdout is not an interactive terminal automatically"
     ),
 )
 @click.pass_context
-def supersearch(ctx, host, supersearch_url, num, headers, format_type, verbose, color):
+def supersearch_cli(
+    ctx, host, supersearch_url, num, headers, format_type, verbose, color
+):
     """
-    Fetches data from Crash Stats using Super Search
+    Performs a basic search on Crash Stats using the Super Search API and
+    outputs the results.
+
+    A basic search uses filters and can span multiple pages of results. A basic
+    search cannot include facets, aggregations, histograms, or cardinalities.
+    For those, use supersearchfacet.
 
     There are two ways to run this:
 
     First, you can specify Super Search API fields to generate the query.
 
     For example:
 
-    $ supersearch --product=Firefox --num=100 --date='>=2019-07-31'
+    $ supersearch --product=Firefox --num=10
 
-    Second, you can pass in a url from a Super Search on Crash Stats. This command
-    will then pull out the parameters. You can override those parameters with
-    command line arguments.
+    Second, you can pass in a url from a Super Search on Crash Stats. This
+    command will then pull out the filter parameters. You can override those
+    parameters with command line arguments.
 
-    $ supersearch --supersearch-url='longurlhere' --num=100
+    $ supersearch --supersearch-url='https://crash-stats.mozilla.org/search/...'
 
-    Make sure to use single quotes when specifying values so that your shell doesn't
-    expand variables.
+    Make sure to use single quotes when specifying values so that your shell
+    doesn't expand variables or parse escape sequences.
 
-    Returned fields are tab-delimited. You can specify them using the Super Search
-    field "_columns".
+    You can specify returned fields using the Super Search field "_columns".
 
     For example:
 
-    $ supersearch --_columns=uuid --_columns=product --_columns=build_id --_columns=version
+    \b
+    $ supersearch --_columns=uuid --_columns=product --_columns=build_id
 
-    Results are tab-delimited. Tabs and newlines in output is escaped.
-
-    This doesn't support any of the aggregations at this time.
+    Results are tab-delimited by default. You can specify other output formats
+    using "--format". Tabs and newlines in output are escaped.
 
     For list of available fields and Super Search API documentation, see:
 
     https://crash-stats.mozilla.org/documentation/supersearch/
 
     https://crash-stats.mozilla.org/documentation/supersearch/api/
 
-    This requires an API token in order to download search and download personally
-    identifiable information and security-sensitive data. It also reduces
-    rate-limiting. Set the CRASHSTATS_API_TOKEN environment variable to your API
-    token value:
+    This requires an API token in order to search and get results for protected
+    data fields. Using an API token also reduces rate-limiting. Set the
+    CRASHSTATS_API_TOKEN environment variable to your API token value:
 
     CRASHSTATS_API_TOKEN=xyz supersearch ...
 
     To create an API token for Crash Stats, visit:
 
     https://crash-stats.mozilla.org/api/tokens/
 
     Remember to abide by the data access policy when using data from Crash Stats!
     The policy is specified here:
 
-    https://crash-stats.mozilla.org/documentation/memory_dump_access/
+    https://crash-stats.mozilla.org/documentation/protected_data_access/
+
     """
     host = host.rstrip("/")
 
     if not color:
         console = Console(color_system=None)
     else:
         console = Console()
@@ -226,87 +182,94 @@
     num_results = num
     if num_results == "all":
         num_results = INFINITY
 
     else:
         try:
             num_results = int(num_results)
-        except ValueError:
+        except ValueError as exc:
             raise click.BadOptionUsage(
                 "num", 'num needs to be an integer or "all"', ctx=ctx
-            )
+            ) from exc
 
     if verbose:
         console.print(f"Params: {params}")
 
     # Sort out API token existence
     api_token = os.environ.get("CRASHSTATS_API_TOKEN")
     if verbose:
         if api_token:
             masked_token = api_token[:4] + ("x" * (len(api_token) - 4))
-            console.print(f"Using api token: {masked_token}")
+            console.print(f"Using API token: {masked_token}")
         else:
             console.print(
-                "[yellow]No api token provided. Set CRASHSTATS_API_TOKEN in the "
+                "[yellow]No API token provided. Set CRASHSTATS_API_TOKEN in the "
                 + "environment.[/yellow]"
             )
-            console.print(
-                "[yellow]Skipping dumps and personally identifiable "
-                + "information.[/yellow]"
-            )
+            console.print("[yellow]Skipping dumps and protected data.[/yellow]")
 
-    hits = fetch_supersearch(
-        console=console,
-        host=host,
+    hits_generator = supersearch(
         params=params,
         num_results=num_results,
+        host=host,
         api_token=api_token,
-        verbose=verbose,
+        logger=ConsoleLogger(console) if verbose else None,
     )
 
     if format_type == "table":
         table = Table(show_edge=False, show_header=headers)
         for column in params["_columns"]:
             table.add_column(column, justify="left")
 
-        for hit_i, hit in enumerate(hits):
+        for hit_i, hit in enumerate(hits_generator):
             if hit_i == 0:
                 for field in params["_columns"]:
                     if field not in hit:
                         raise click.UsageError(f"{field}: no data")
 
             table.add_row(
                 *[escape_whitespace(hit[field]) for field in params["_columns"]]
             )
 
         console.print(table)
 
     elif format_type == "tab":
         try:
             for line in tableize_tab(
-                params["_columns"], data=hits, show_headers=headers
+                params["_columns"], data=hits_generator, show_headers=headers
+            ):
+                # NOTE(willkg): we don't use console.print here because rich will do fancy
+                # things like wrapping and fixing tabs we don't want that
+                click.echo(line)
+        except MissingField as exc:
+            raise click.UsageError(f"{exc.args[0]}: no data") from exc
+
+    elif format_type == "csv":
+        try:
+            for line in tableize_csv(
+                params["_columns"], data=hits_generator, show_headers=headers
             ):
                 # NOTE(willkg): we don't use console.print here because rich will do fancy
                 # things like wrapping and fixing tabs we don't want that
                 click.echo(line)
         except MissingField as exc:
-            raise click.UsageError(f"{exc.args[0]}: no data")
+            raise click.UsageError(f"{exc.args[0]}: no data") from exc
 
     elif format_type == "markdown":
         try:
-            for line in tableize_markdown(params["_columns"], data=hits):
+            for line in tableize_markdown(params["_columns"], data=hits_generator):
                 # NOTE(willkg): we don't use console.print here because rich will do fancy
                 # things like wrapping and fixing tabs we don't want that
                 click.echo(line)
         except MissingField as exc:
-            raise click.UsageError(f"{exc.args[0]}: no data")
+            raise click.UsageError(f"{exc.args[0]}: no data") from exc
 
     elif format_type == "json":
         records = []
-        for hit_i, hit in enumerate(hits):
+        for hit_i, hit in enumerate(hits_generator):
             if hit_i == 0:
                 for field in params["_columns"]:
                     if field not in hit:
                         raise click.UsageError(f"{field}: no data")
 
             records.append(
                 {
@@ -314,8 +277,8 @@
                     for field in params["_columns"]
                 }
             )
         console.print_json(json.dumps(records))
 
 
 if __name__ == "__main__":
-    supersearch()
+    supersearch_cli()
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools/cmd_supersearchfacet.py` & `crashstats_tools-2/src/crashstats_tools/cmd_supersearchfacet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,232 +1,387 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import datetime
-import functools
 import json
 import logging
 import os
 from urllib.parse import urlparse, parse_qs
 
 import click
 from rich.console import Console
 from rich.table import Table
+from rich import box
 
+from crashstats_tools.libcrashstats import supersearch_facet
 from crashstats_tools.utils import (
+    ConsoleLogger,
     DEFAULT_HOST,
-    http_get,
     parse_args,
     parse_relative_date,
+    sanitize_text,
+    tableize_csv,
     tableize_markdown,
     tableize_tab,
+    thing_to_key,
 )
 
 
-@functools.total_ordering
-class AlwaysFirst:
-    def __eq__(self, other):
-        # Two AlwaysFirst instances are always equal
-        return type(other) == type(self)
+def extract_supersearch_params(url):
+    """Parses out params from the query string and drops any search-related ones.
 
-    def __lt__(self, other):
-        # This is always less than other
-        return True
+    :arg url: a url string
 
+    :returns: dict of params from url minus params specific to supersearch
+        results
 
-def thing_to_key(item):
-    if isinstance(item, (list, tuple)):
-        item = item[0]
-    if item == "--":
-        return AlwaysFirst()
-    return item
+    """
+    parsed = urlparse(url)
+    params = parse_qs(parsed.query)
 
+    # Remove search things
+    aggs_keys = ("_columns", "_results_number", "_results_offset")
+    for key in list(params.keys()):
+        if key.startswith(aggs_keys):
+            del params[key]
 
-def now():
-    return datetime.datetime.now()
+    return params
 
 
-def generate_periods(period, start_date, end_date):
-    start_point = datetime.datetime.strptime(start_date, "%Y-%m-%d")
-    end_point = datetime.datetime.strptime(end_date, "%Y-%m-%d")
+def convert_histogram_data(facet_name, facet_data):
+    """Converts histogram facet data into records
 
-    if period == "daily":
-        delta = datetime.timedelta(days=1)
+    :arg facet_name: the facet name
+    :arg facet_data: the facet results from the response payload
 
-    elif period == "hourly":
-        delta = datetime.timedelta(hours=1)
+    :returns: a map of facet_name -> list of record dicts
 
-    elif period == "weekly":
-        delta = datetime.timedelta(days=7)
+    """
+    # Map of field_name -> (map of date -> (map of term -> count))
+    facet_tables = {}
+    for row in facet_data:
+        row_term = row["term"]
+        if row_term.endswith("T00:00:00+00:00"):
+            # Convert timestamps that are just a date at midnight to just the
+            # date portion
+            row_term = row_term[:10]
+        total = row["count"]
+        records = {}
+        for field_name, field_data in row["facets"].items():
+            if field_name.startswith("cardinality"):
+                records = {"value": field_data["value"]}
+            else:
+                records = {item["term"]: item["count"] for item in field_data}
+                records["total"] = total
+            facet_tables.setdefault(field_name, {})[row_term] = records
 
-    while start_point <= end_point:
-        next_end_point = start_point + delta
-        yield start_point.strftime("%Y-%m-%d %H:%M:%S"), next_end_point.strftime(
-            "%Y-%m-%d %H:%M:%S"
-        )
-        start_point = next_end_point
+    # Normalize the data--make sure table rows have all the values
+    for field_data in facet_tables.values():
+        terms = set()
+        for date_data in field_data.values():
+            terms = terms | set(date_data.keys())
+
+        for date_data in field_data.values():
+            missing_terms = terms - set(date_data.keys())
+            for missing_term in missing_terms:
+                date_data[missing_term] = 0
+
+    # Now convert it to map of field_name -> records
+    result = {}
+    for field_name, field_data in facet_tables.items():
+        keys = list(field_data.values())[0].keys()
+        headers = [facet_name] + sorted(keys, key=thing_to_key)
+
+        records = []
+        for row_key, row_data in sorted(field_data.items()):
+            row = {facet_name: row_key}
+            row.update(
+                {column: sanitize_text(row_data[column]) for column in headers[1:]}
+            )
+            records.append(row)
+        result[field_name] = records
 
+    return result
 
-def fetch_supersearch_facets(console, host, params, api_token=None, verbose=False):
-    """Generator that returns Super Search results
 
-    :arg str host: the host to query
-    :arg dict params: dict of super search parameters to base the query on
-    :arg str api_token: the API token to use or None
-    :arg bool verbose: whether or not to print verbose things
+def flatten_facets(facet_data):
+    """Flattens facet value data.
 
-    :returns: dict with "total" and "facets" keys
+    :arg facet_data: map of key -> term_counts
+
+    :returns: map of key -> list of record dicts
 
     """
-    url = host + "/api/SuperSearch/"
+    if not facet_data:
+        return {}
 
-    params["_results_number"] = 0
+    flattened_facet_data = {}
+    for key, term_counts in facet_data.items():
+        if key.startswith("cardinality"):
+            # term_counts here is something like: {"value": 6}
+            #
+            # convert to [{key: "value", "value": 6}]
+            flattened_facet_data[key] = [{key: "value", "value": term_counts["value"]}]
 
-    if verbose:
-        console.print(f"{url} {params}")
+        elif key.startswith("histogram"):
+            flattened_facet_data[key] = convert_histogram_data(key, term_counts)
 
-    resp = http_get(url=url, params=params, api_token=api_token)
-    data = resp.json()
-    return {
-        "total": data["total"],
-        "facets": data["facets"],
-    }
+        else:
+            for term_count_item in term_counts:
+                term = term_count_item["term"]
+                count = term_count_item["count"]
+
+                if "facets" in term_count_item:
+                    term_counts_dict = flatten_facets(term_count_item["facets"])
+                    for term_key, term_data in term_counts_dict.items():
+                        new_key = f"{key} / {term_key}"
+                        for item in term_data:
+                            new_data = {
+                                new_key: f"{term} / {item[term_key]}",
+                            }
+                            # cardinality has "value", while facets have
+                            # "count" so we need to handle both here
+                            new_data["count"] = item.get("count", item.get("value"))
+                            flattened_facet_data.setdefault(new_key, []).append(
+                                new_data
+                            )
+
+                else:
+                    new_data = {key: term, "count": count}
+                    flattened_facet_data.setdefault(key, []).append(new_data)
 
+    return flattened_facet_data
 
-def extract_supersearch_params(url):
-    """Parses out params from the query string and drops any search-related ones."""
-    parsed = urlparse(url)
-    params = parse_qs(parsed.query)
 
-    # Remove search things
-    aggs_keys = ("_columns", "_results_number", "_results_offset")
-    for key in list(params.keys()):
-        if key.startswith(aggs_keys):
-            del params[key]
+def generate_facet_tables(leftover_count, facet_name, facet_data, total):
+    """
+    :returns: a map of facet_name -> {headers: headers, records: records}
 
-    return params
+    """
+    records = []
+    count_sum = 0
+    for term, count in sorted(facet_data.items(), key=lambda x: x[1], reverse=True):
+        records.append({facet_name: sanitize_text(term), "count": count})
+        count_sum += count
+
+    if not facet_name.startswith("cardinality"):
+        if leftover_count:
+            records.append({facet_name: "--", "count": total - count_sum})
+        records.append({facet_name: "total", "count": total})
+
+    return {facet_name: records}
+
+
+DATE_TEMPLATES = [
+    "%Y-%m-%d",
+    "%Y-%m-%dT%H:%M:%S+%z",
+]
+
+
+def is_weekend(value):
+    """Denotes whether this date is a weekend.
+
+    :arg value: a string value representing a date/datetime
+
+    :returns: whether or not this is a weekend
+
+    """
+    for template in DATE_TEMPLATES:
+        try:
+            dt = datetime.datetime.strptime(value, template)
+            return dt.weekday() in [5, 6]
+        except ValueError:
+            continue
+    return False
+
+
+def fix_value(value, denote_weekends=False):
+    """Sanitizes text and adds ``**`` if it's a weekend if specified
+
+    :arg value: the text to operate on
+    :arg denote_weekends: whether or not to denote weekend if the item is a
+        date/datetime and it's a weekend
+
+    :returns: the final value
+
+    """
+    value = sanitize_text(str(value))
+    if denote_weekends and isinstance(value, str) and is_weekend(value):
+        return f"{value} **"
+
+    return value
 
 
 @click.command(
-    context_settings={"allow_extra_args": True, "ignore_unknown_options": True}
+    context_settings={
+        "show_default": True,
+        "allow_extra_args": True,
+        "ignore_unknown_options": True,
+    }
 )
 @click.option(
     "--host", default=DEFAULT_HOST, help="host for system to fetch facets from"
 )
 @click.option("--supersearch-url", default="", help="Super Search url to base query on")
 @click.option(
     "--start-date", default="", help="start date for range; YYYY-MM-DD format"
 )
 @click.option(
     "--end-date",
-    default=None,
+    default="today",
     show_default=True,
-    help="end date for range; YYYY-MM-DD format; defaults to today",
+    help="end date for range; YYYY-MM-DD format",
 )
 @click.option(
     "--relative-range", default="7d", help="relative range ending on end-date"
 )
 @click.option(
-    "--period",
-    default="none",
-    show_default=True,
-    type=click.Choice(["none", "daily", "hourly", "weekly"], case_sensitive=False),
-    help="period to facet on to get count/period",
-)
-@click.option(
     "--format",
     "format_type",
     default="table",
     show_default=True,
-    type=click.Choice(["table", "tab", "markdown", "json"], case_sensitive=False),
+    type=click.Choice(
+        ["table", "tab", "csv", "markdown", "json", "raw"], case_sensitive=False
+    ),
     help="format to print output",
 )
 @click.option(
     "--verbose/--no-verbose", default=False, help="whether to print debugging output"
 )
 @click.option(
     "--color/--no-color",
     default=True,
     help=(
         "whether or not to colorize output; note that color is shut off "
-        "when stdout is not an interactive terminal automatically"
+        + "when stdout is not an interactive terminal automatically"
+    ),
+)
+@click.option(
+    "--denote-weekends/--no-denote-weekends",
+    default=False,
+    help=(
+        "This will add a * for values that are datestamps and on a Saturday or Sunday."
+    ),
+)
+@click.option(
+    "--leftover-count/--no-leftover-count",
+    default=False,
+    help=(
+        "Calculates the leftover that is the difference between the total "
+        + "minus the sum of all term counts"
     ),
 )
 @click.pass_context
 def supersearchfacet(
     ctx,
     host,
     supersearch_url,
     end_date,
     start_date,
     relative_range,
-    period,
     format_type,
     verbose,
     color,
+    denote_weekends,
+    leftover_count,
 ):
     """Fetches facet data from Crash Stats using Super Search
 
     There are two ways to run this:
 
     First, you can specify Super Search API fields to generate the query.
 
     For example:
 
     $ supersearchfacet --product=Firefox --_facets=version
 
-    Second, you can pass in a url from a Super Search on Crash Stats. This command
-    will then pull out the parameters. You can override those parameters with
-    command line arguments.
+    Second, you can pass in a url from a Super Search on Crash Stats. This
+    command will then pull out the parameters. You can override those
+    parameters with command line arguments.
+
+    \b
+    $ supersearchfacet --_facets=version \\
+        --supersearch-url='https://crash-stats.mozilla.org/search/...'
+
+    Make sure to use single quotes when specifying values so that your shell
+    doesn't expand variables.
+
+    You can get a facet of a field using ``_facets``.
+
+    For example, this filters on Firefox and returns a facet on version
+    for the last 7 days (the default time range).
+
+    $ supersearchfacet --product=Firefox --_facets=version
+
+    You can get cardinality (number of possible values), too. For example, this
+    shows the number of different versions for Firefox crash reports in the
+    last 7 days.
 
-    $ supersearchfacet --supersearch-url='longurlhere' --_facets=version
+    $ supersearchfacet --product=Firefox --_facets=_cardinality.version
 
-    Make sure to use single quotes when specifying values so that your shell doesn't
-    expand variables.
+    You can perform histograms. For example, this shows you counts for products
+    per day for the last week:
 
-    You can only specify one facet using "--_facets". If you don't specify one,
-    it defaults to "signature".
+    $ supersearchfacet --_histogram.date=product --relative-range=1w
 
-    By default, returned data is a tab-delimited table. Tabs and newlines in
-    output is escaped. Use "--format" to specify a different output format.
+    You can get a cardinality for the data for a field. For example,
+    this tells you how many build ids there were for Firefox 124:
+
+    $ supersearchfacet --product=Firefox --version=124.0 \
+        --_facets=_cardinality.build_id
+
+    You can do nested aggregations. For example, this shows the count
+    of crash reports by product by release channel:
+
+    $ supersearchfacet --_aggs.product=release_channel
+
+    This shows count of crash reports by product, version, cardinality of
+    install_time:
+
+    $ supersearchfacet --_aggs.product.version=_cardinality.install_time
+
+    Make sure to specify at least one of ``_facets``, ``_aggs``,
+    ``_histogram``, or ``_cardinality``.
+
+    By default, returned data is in a table. Tabs and newlines in output is
+    escaped. Use ``--format`` to specify a different output format.
 
     For list of available fields and Super Search API documentation, see:
 
     https://crash-stats.mozilla.org/documentation/supersearch/
 
     https://crash-stats.mozilla.org/documentation/supersearch/api/
 
-    This generates a table values and counts. If you want values and counts
-    over a series of days, use "--period=daily".
-
-    This requires an API token in order to download search and download personally
-    identifiable information and security-sensitive data. It also reduces
-    rate-limiting.  Set the CRASHSTATS_API_TOKEN environment variable to your API
-    token value:
+    This requires an API token in order to search and get results for protected
+    data fields. Using an API token also reduces rate-limiting. Set the
+    CRASHSTATS_API_TOKEN environment variable to your API token value:
 
     CRASHSTATS_API_TOKEN=xyz supersearchfacet ...
 
     To create an API token for Crash Stats, visit:
 
     https://crash-stats.mozilla.org/api/tokens/
 
     Remember to abide by the data access policy when using data from Crash Stats!
     The policy is specified here:
 
-    https://crash-stats.mozilla.org/documentation/memory_dump_access/
+    https://crash-stats.mozilla.org/documentation/protected_data_access/
+
     """
     host = host.rstrip("/")
 
     if not color:
-        console = Console(color_system=None)
+        console = Console(color_system=None, tab_size=None)
+        console_err = Console(color_system=None, tab_size=None, stderr=True)
     else:
-        console = Console()
+        console = Console(tab_size=None)
+        console_err = Console(tab_size=None, stderr=True)
 
-    if end_date is None:
+    if end_date == "today":
         end_date = datetime.datetime.now().strftime("%Y-%m-%d")
 
     # Require at least one facet specified.
     parsed_args = parse_args(ctx.args)
 
     if verbose:
         # Set logging to DEBUG because this picks up debug logging from
@@ -238,196 +393,167 @@
         params = extract_supersearch_params(supersearch_url)
     else:
         params = {}
 
     params.update(parsed_args)
 
     if "_facets" not in params:
-        params["_facets"] = ["signature"]
-
-    if len(params["_facets"]) > 1:
-        raise click.UsageError("One '_facets' must be specified.")
-        ctx.exit(1)
+        params["_facets"] = []
 
     # Sort out API token existence
     api_token = os.environ.get("CRASHSTATS_API_TOKEN")
     if verbose:
         if api_token:
             masked_token = api_token[:4] + ("x" * (len(api_token) - 4))
-            console.print(f"Using api token: {masked_token}")
+            console.print(f"Using API token: {masked_token}")
         else:
             console.print(
-                "[yellow]No api token provided. Set CRASHSTATS_API_TOKEN in the "
+                "[yellow]No API token provided. Set CRASHSTATS_API_TOKEN in the "
                 + "environment.[/yellow]"
             )
-            console.print(
-                "[yellow]Skipping dumps and personally identifiable "
-                + "information.[/yellow]"
-            )
+            console.print("[yellow]Skipping dumps and protected data.[/yellow]")
 
     if "date" not in params and not start_date:
         try:
             range_timedelta = parse_relative_date(relative_range)
-        except ValueError as ve:
-            raise click.UsageError(ve.msg)
+        except ValueError as vexc:
+            raise click.UsageError(vexc.msg) from vexc
 
         start_date = (
             datetime.datetime.strptime(end_date, "%Y-%m-%d") - range_timedelta
         ).strftime("%Y-%m-%d")
 
-    # If there's no count/period or the user used a supersearch-url that
-    # specifies a date, then we can do a single facet and print the data out
-    # and we're done
-    if period == "none" or "date" in params:
-        if "date" not in params:
-            params.update({"date": [">=%s" % start_date, "<%s" % end_date]})
+    if "date" not in params:
+        params.update({"date": [">=%s" % start_date, "<%s" % end_date]})
 
-        if verbose:
-            console.print(f"Params: {params}")
-
-        facet_data = fetch_supersearch_facets(
-            console=console,
-            host=host,
-            params=params,
-            api_token=api_token,
-            verbose=verbose,
-        )
-
-        facet_name = params["_facets"][0]
-
-        remaining = facet_data["total"]
-        facets = facet_data["facets"]
-
-        if facet_name not in facets:
-            raise click.UsageError(f"{facet_name}: no data")
-
-        headers = [facet_name, "count"]
-        facet_item_data = facets[facet_name]
-        records = [
-            {facet_name: item["term"], "count": item["count"]}
-            for item in sorted(facet_item_data, key=lambda x: x["count"], reverse=True)
-        ]
-        remaining -= sum([item["count"] for item in facet_item_data])
-
-        if remaining:
-            records.append({facet_name: "--", "count": remaining})
-
-        if format_type == "table":
-            table = Table(show_edge=False)
-            for column in headers:
-                table.add_column(column, justify="left")
-
-            for item in records:
-                table.add_row(*[str(item[field]) for field in headers])
-            console.print(table)
-
-        elif format_type == "tab":
-            # NOTE(willkg): We need to use click.echo because console.print
-            # does rich fancy-stuff with the output
-            for line in tableize_tab(headers=headers, data=records):
-                click.echo(line)
-
-        elif format_type == "markdown":
-            for line in tableize_markdown(headers=headers, data=records):
-                click.echo(line)
+    if verbose:
+        console.print(f"Params: {params}")
 
-        elif format_type == "json":
-            console.print_json(json.dumps(records))
+    facet_data_payload = supersearch_facet(
+        params=params,
+        api_token=api_token,
+        host=host,
+        logger=ConsoleLogger(console) if verbose else None,
+    )
+    if (
+        "signature" not in params["_facets"]
+        and "signature" in facet_data_payload["facets"]
+    ):
+        # The Super Search API adds a "signature" facet by default if no other
+        # "_facets" are specified even when you don't want it--this removes it
+        del facet_data_payload["facets"]["signature"]
 
+    if format_type == "raw":
+        console.print_json(json.dumps(facet_data_payload))
         return
 
-    # If it is in count/period mode, then we have to do one facet for each
-    # period and compose the results.
-
-    # Figure out what facet we're doing
-    facet_name = params["_facets"][0]
+    total = facet_data_payload["total"]
+    facets = facet_data_payload["facets"]
 
-    # Map of facet_name -> (map of date -> (map of value -> count))
-    facet_tables = {facet_name: {}}
+    flattened_facets = flatten_facets(facets)
 
-    # FIXME(willkg): for "period=weekly", does it make sense to anchor it on
-    # beginning of the week? (sunday or monday)
+    # Add leftover and total records
+    for facet_name, records in flattened_facets.items():
+        if not facet_name.startswith(("histogram", "cardinality")):
+            if leftover_count:
+                record_sum = sum(rec["count"] for rec in records)
+                records.append({facet_name: "--", "count": total - record_sum})
+
+            records.append({facet_name: "total", "count": total})
+
+        elif facet_name.startswith("histogram"):
+            if leftover_count:
+                for _, rows in records.items():
+                    for row in rows:
+                        count = 0
+                        for key, val in row.items():
+                            if key == facet_name:
+                                continue
+                            elif key == "total":
+                                count -= int(val)
+                            else:
+                                count += int(val)
+                        row["--"] = str(count)
 
-    for day_start, day_end in generate_periods(period, start_date, end_date):
-        params.update({"date": [">=%s" % day_start, "<%s" % day_end]})
+    if format_type == "json":
+        console.print_json(json.dumps(flattened_facets))
+        return
 
-        if verbose:
-            console.print(f"Params: {params}")
+    # We want to print a blank line between things, so we print a blank line
+    # before any thing that's not the first thing
+    first_thing = True
+    for facet_name, records in flattened_facets.items():
+        if not first_thing:
+            console.print()
 
-        facet_data = fetch_supersearch_facets(
+        print_table(
             console=console,
-            host=host,
-            params=params,
-            api_token=api_token,
-            verbose=verbose,
+            format_type=format_type,
+            denote_weekends=denote_weekends,
+            facet_name=[facet_name],
+            records=records,
         )
+        first_thing = False
 
-        remaining = facet_data["total"]
-        facets = facet_data["facets"]
-
-        for item in facets.get(facet_name, []):
-            count = item["count"]
-            facet_tables[facet_name].setdefault(day_start, {})[item["term"]] = count
-            remaining -= count
-        facet_tables[facet_name].setdefault(day_start, {})["--"] = remaining
-
-    # Normalize the data--make sure table rows have all the values
-    values = set()
-
-    table = facet_tables[facet_name]
-    for date, value_counts in table.items():
-        values = values | set(value_counts.keys())
-
-    for date, value_counts in table.items():
-        missing_values = values - set(value_counts.keys())
-        for missing_value in missing_values:
-            value_counts[missing_value] = 0
+    if first_thing:
+        # This is weird--it means we didn't print any tables, so something is
+        # wrong.
+        console_err.print("No output--something went wrong.")
+        console_err.print(f"Host: {host}")
+        if api_token:
+            masked_token = api_token[:4] + ("x" * (len(api_token) - 4))
+            console_err.print(f"Using API token: {masked_token}")
+        else:
+            console_err.print("Not using API token.")
+        console_err.print(f"Params sent: {params}")
+        console_err.print(f"Output returned: {facet_data_payload}")
+        ctx.exit(1)
 
-    table = facet_tables[facet_name]
 
-    if not table:
-        raise click.UsageError(f"{facet_name}: no data")
+def print_table(console, format_type, denote_weekends, facet_name, records):
+    if isinstance(records, dict):
+        for sub_facet_name, sub_records in records.items():
+            print_table(
+                console=console,
+                format_type=format_type,
+                denote_weekends=denote_weekends,
+                facet_name=facet_name + [sub_facet_name],
+                records=sub_records,
+            )
+        return
 
-    some_date = list(table.keys())[0]
-    headers = ["date"] + sorted(table[some_date].keys(), key=thing_to_key)
-    records = []
-    for date, value_counts in table.items():
-        records.append(
-            {
-                field_name: val
-                for field_name, val in zip(
-                    headers,
-                    [date]
-                    + [
-                        item[1]
-                        for item in sorted(value_counts.items(), key=thing_to_key)
-                    ],
-                )
-            }
-        )
+    # Grab the first record keys, take out the facet_name, sort, and then
+    # add the facet_name first
+    headers = list(records[0].keys())
+    headers.remove(facet_name[0])
+    headers = [facet_name[0]] + sorted(headers, key=thing_to_key)
+
+    records = [
+        {key: fix_value(val, denote_weekends) for key, val in record.items()}
+        for record in records
+    ]
 
+    console.print(".".join(facet_name))
     if format_type == "table":
-        table = Table(show_edge=False)
+        table = Table(show_edge=False, box=box.MARKDOWN)
         for column in headers:
             table.add_column(column, justify="left")
-        for item in records:
-            table.add_row(*[str(item[field]) for field in headers])
+
+        for record in records:
+            table.add_row(*[record[header] for header in headers])
         console.print(table)
 
+    elif format_type == "csv":
+        for line in tableize_csv(headers=headers, data=records):
+            console.file.write(line + "\n")
+
     elif format_type == "tab":
-        # NOTE(willkg): We need to use click.echo because console.print
-        # does rich fancy-stuff with the output
         for line in tableize_tab(headers=headers, data=records):
-            click.echo(line)
+            console.file.write(line + "\n")
 
     elif format_type == "markdown":
-        # NOTE(willkg): We need to use click.echo because console.print
-        # does rich fancy-stuff with the output
         for line in tableize_markdown(headers=headers, data=records):
-            click.echo(line)
-
-    elif format_type == "json":
-        console.print_json(json.dumps(records))
+            console.file.write(line + "\n")
 
 
 if __name__ == "__main__":
     supersearchfacet()
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools/utils.py` & `crashstats_tools-2/src/crashstats_tools/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,104 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+import csv
 import datetime
 from functools import total_ordering
+import inspect
+import io
 import json
+import os
 import re
+import string
 from typing import Any, Dict, Generator, Iterable, List
 from urllib.parse import urlparse
 
 import requests
-from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
+from requests.adapters import HTTPAdapter, Retry
+from rich.console import Console
+
+from crashstats_tools import __version__
 
 
 DEFAULT_HOST = "https://crash-stats.mozilla.org"
 
 
 WHITESPACE_TO_ESCAPE = [("\t", "\\t"), ("\r", "\\r"), ("\n", "\\n")]
 
 
+def dbg(*args):
+    """Utility for printing debug output when debugging.
+
+    Prints the filename and line number and then a stringified list of the
+    args.
+
+    """
+    console = Console(stderr=True, tab_size=None)
+    callframe = inspect.currentframe().f_back
+    fn = callframe.f_code.co_filename.split(os.sep)[-1]
+    lineno = callframe.f_lineno
+    str_args = ", ".join(f"{arg!r}" for arg in args)
+    console.print(f"dbg: [yellow]{fn}:{lineno}[/yellow] {str_args}")
+
+
+class ConsoleLogger:
+    """Logs to a click console."""
+
+    def __init__(self, console):
+        self.console = console
+
+    def log(self, level, msg, *args, **kwargs):
+        # NOTE(willkg): kwargs are currently ignored
+        self.console.print(msg % args)
+
+    def debug(self, msg, *args, **kwargs):
+        self.log(10, msg, *args, **kwargs)
+
+    def info(self, msg, *args, **kwargs):
+        self.log(20, msg, *args, **kwargs)
+
+    def warning(self, msg, *args, **kwargs):
+        self.log(30, msg, *args, **kwargs)
+
+    def error(self, msg, *args, **kwargs):
+        self.log(40, msg, *args, **kwargs)
+
+    def exception(self, msg, *args, **kwargs):
+        # NOTE(willkg): exception doesn't add exception information--currently,
+        # it's just an alias for error
+        self.log(40, msg, *args, **kwargs)
+
+    def critical(self, msg, *args, **kwargs):
+        self.log(50, msg, *args, **kwargs)
+
+
 def escape_whitespace(text):
     """Escapes whitespace characters."""
     text = text or ""
     for s, replace in WHITESPACE_TO_ESCAPE:
         text = text.replace(s, replace)
     return text
 
 
 def escape_pipes(text):
+    """Escape pipe characters."""
     text = text or ""
     return text.replace("|", "\\|")
 
 
+def sanitize_text(item):
+    """Sanitizes text dropping all non-printable characters."""
+    if not isinstance(item, str):
+        return item
+    text = "".join([c for c in item if c in string.printable])
+    return text
+
+
 class JsonDTEncoder(json.JSONEncoder):
     """JSON encoder that handles datetimes
 
     >>> json.dumps(some_data, cls=JsonDTEncoder)
     ...
 
     """
@@ -104,15 +166,15 @@
         backoff_factor=backoff_factor,
         status_forcelist=list(status_forcelist),
     )
 
     session = requests.Session()
 
     # Set the User-Agent header so we can distinguish our stuff from other stuff
-    session.headers.update({"User-Agent": "crashstats-tools/1.0"})
+    session.headers.update({"User-Agent": f"crashstats-tools/{__version__}"})
 
     adapter = HTTPAdapterWithTimeout(
         max_retries=retries, default_timeout=default_timeout
     )
     session.mount("http://", adapter)
     session.mount("https://", adapter)
 
@@ -213,16 +275,42 @@
         raise ValueError("This Infinity does not support right-hand-side")
 
 
 # For our purposes, there is only one infinity
 INFINITY = Infinity()
 
 
+@total_ordering
+class AlwaysFirst:
+    """This item is always first."""
+
+    def __eq__(self, other):
+        # Two AlwaysFirst instances are always equal
+        return type(other) == type(self)
+
+    def __lt__(self, other):
+        # This is always less than other
+        return True
+
+
+@total_ordering
+class AlwaysLast:
+    """This item is always last."""
+
+    def __eq__(self, other):
+        # Two AlwaysLast instances are always equal
+        return type(other) == type(self)
+
+    def __lt__(self, other):
+        # This is always greater than other
+        return False
+
+
 class InvalidArg(Exception):
-    pass
+    """Denotes an invalid command line argument."""
 
 
 def parse_args(args):
     """Convert command line arguments to supersearch arguments."""
     params = {}
 
     while args:
@@ -272,26 +360,26 @@
 
     :returns: True if it's valid, False if not
 
     """
     return bool(CRASH_ID_RE.match(crash_id))
 
 
-def parse_crashid(item):
-    """Returns a crashid from a number of formats.
+def parse_crash_id(item):
+    """Returns a crash id from a number of formats.
 
     This handles the following three forms of crashids:
 
     * CRASHID
     * bp-CRASHID
     * http[s]://HOST[:PORT]/report/index/CRASHID
 
     :arg str item: the thing to parse a crash id from
 
-    :returns: crashid as str or None
+    :returns: crash id as str or None
 
     :raises ValueError: if the crash id isn't recognized
 
     """
     if is_crash_id_valid(item):
         return item
 
@@ -306,15 +394,44 @@
             if is_crash_id_valid(crash_id):
                 return crash_id
 
     raise ValueError(f"Not a valid crash id: {item}")
 
 
 class MissingField(Exception):
-    pass
+    """Denotes a missing field."""
+
+
+def tableize_csv(
+    headers: List[str], data: Iterable[Dict[str, Any]], show_headers: bool = True
+) -> Generator[str, None, None]:
+    """Generate output for a table in csv.
+
+    :param headers: headers of the table
+    :param data: rows of the table
+
+    :returns: generator of strings
+
+    """
+    buffer = io.StringIO()
+    csvwriter = csv.writer(buffer)
+    for item_i, item in enumerate(data):
+        if item_i == 0:
+            for field in headers:
+                if field not in item:
+                    raise MissingField(field)
+            if show_headers:
+                csvwriter.writerow([escape_whitespace(str(item)) for item in headers])
+
+        row = [escape_whitespace(str(item.get(field, ""))) for field in headers]
+        if row:
+            csvwriter.writerow(row)
+
+    for line in buffer.getvalue().splitlines():
+        yield line
 
 
 def tableize_tab(
     headers: List[str], data: Iterable[Dict[str, Any]], show_headers: bool = True
 ) -> Generator[str, None, None]:
     """Generate output for a table using tab delimiters.
 
@@ -374,7 +491,27 @@
         raise ValueError(f"'{text}' is not a valid relative date.")
 
     count = int(parsed.group(1))
     unit = parsed.group(2)
 
     unit_to_arg = {"h": "hours", "d": "days", "w": "weeks"}
     return datetime.timedelta(**{unit_to_arg[unit]: count})
+
+
+def thing_to_key(item):
+    """Returns a sorting key for the item
+
+    This causes "--" to always be first and "total" to always
+    be last.
+
+    For lists/tuples, this picks the first item.
+
+    :returns: a key
+
+    """
+    if isinstance(item, (list, tuple)):
+        item = item[0]
+    if item == "--":
+        return AlwaysFirst()
+    if item == "total":
+        return AlwaysLast()
+    return item
```

### Comparing `crashstats-tools-1.4.0/src/crashstats_tools.egg-info/SOURCES.txt` & `crashstats_tools-2/src/crashstats_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 CODE_OF_CONDUCT.md
 HISTORY.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
-requirements-dev.txt
-setup.cfg
-setup.py
-tox.ini
+pyproject.toml
 src/crashstats_tools/__init__.py
 src/crashstats_tools/cmd_fetch_data.py
 src/crashstats_tools/cmd_reprocess.py
 src/crashstats_tools/cmd_supersearch.py
 src/crashstats_tools/cmd_supersearchfacet.py
+src/crashstats_tools/libcrashstats.py
 src/crashstats_tools/utils.py
 src/crashstats_tools.egg-info/PKG-INFO
 src/crashstats_tools.egg-info/SOURCES.txt
 src/crashstats_tools.egg-info/dependency_links.txt
 src/crashstats_tools.egg-info/entry_points.txt
 src/crashstats_tools.egg-info/requires.txt
 src/crashstats_tools.egg-info/top_level.txt
```

