# Comparing `tmp/sparecores-crawler-0.1.0.tar.gz` & `tmp/sparecores_crawler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparecores-crawler-0.1.0.tar", last modified: Fri Apr  5 21:46:46 2024, max compression
+gzip compressed data, was "sparecores_crawler-0.1.1.tar", last modified: Fri Apr 12 17:16:58 2024, max compression
```

## Comparing `sparecores-crawler-0.1.0.tar` & `sparecores_crawler-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.941177 sparecores-crawler-0.1.0/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores-crawler-0.1.0/LICENSE
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       18 2024-02-23 23:24:20.000000 sparecores-crawler-0.1.0/MANIFEST.in
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7235 2024-04-05 21:46:46.941177 sparecores-crawler-0.1.0/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/README.md
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3386 2024-04-05 21:44:17.000000 sparecores-crawler-0.1.0/pyproject.toml
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-04-05 21:46:46.941177 sparecores-crawler-0.1.0/setup.cfg
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.924510 sparecores-crawler-0.1.0/src/
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.934510 sparecores-crawler-0.1.0/src/sc_crawler/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores-crawler-0.1.0/src/sc_crawler/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    18160 2024-04-05 21:01:59.000000 sparecores-crawler-0.1.0/src/sc_crawler/cli.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/insert.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores-crawler-0.1.0/src/sc_crawler/logger.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2437 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/lookup.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19567 2024-04-04 22:44:04.000000 sparecores-crawler-0.1.0/src/sc_crawler/table_bases.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/table_fields.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17021 2024-04-04 22:44:21.000000 sparecores-crawler-0.1.0/src/sc_crawler/tables.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/tables_scd.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4836 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/utils.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.934510 sparecores-crawler-0.1.0/src/sc_crawler/vendors/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      108 2024-02-20 22:24:12.000000 sparecores-crawler-0.1.0/src/sc_crawler/vendors/__init__.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)    39071 2024-04-04 22:53:58.000000 sparecores-crawler-0.1.0/src/sc_crawler/vendors/aws.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      520 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/src/sc_crawler/vendors/gcp.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      824 2024-04-04 20:24:37.000000 sparecores-crawler-0.1.0/src/sc_crawler/vendors/vendors.py
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.937843 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7235 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/PKG-INFO
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      808 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/SOURCES.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/dependency_links.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/entry_points.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)      443 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/requires.txt
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-04-05 21:46:46.000000 sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/top_level.txt
-drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-05 21:46:46.937843 sparecores-crawler-0.1.0/tests/
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/tests/test_schemas.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores-crawler-0.1.0/tests/test_str_utils.py
--rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores-crawler-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    16726 2023-12-08 22:12:52.000000 sparecores_crawler-0.1.1/LICENSE
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       53 2024-04-12 16:09:18.000000 sparecores_crawler-0.1.1/MANIFEST.in
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7384 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5326 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/README.md
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3515 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/pyproject.toml
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       38 2024-04-12 17:16:58.198246 sparecores_crawler-0.1.1/setup.cfg
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.184913 sparecores_crawler-0.1.1/src/
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        0 2024-02-14 13:12:38.000000 sparecores_crawler-0.1.1/src/sc_crawler/__init__.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/alembic/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2977 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/env.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     5929 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    68592 2024-04-12 16:51:35.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3618 2024-04-12 15:45:00.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic.ini
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1185 2024-04-12 16:10:05.000000 sparecores_crawler-0.1.1/src/sc_crawler/alembic_helpers.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    22486 2024-04-12 16:49:26.000000 sparecores_crawler-0.1.1/src/sc_crawler/cli.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     6780 2024-04-10 22:14:16.000000 sparecores_crawler-0.1.1/src/sc_crawler/insert.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     8517 2024-04-04 14:01:05.000000 sparecores_crawler-0.1.1/src/sc_crawler/logger.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     3503 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/lookup.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2201 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    19543 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/table_bases.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4705 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/table_fields.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    17021 2024-04-12 15:16:24.000000 sparecores_crawler-0.1.1/src/sc_crawler/tables.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     2730 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/tables_scd.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     4836 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/utils.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.191579 sparecores_crawler-0.1.1/src/sc_crawler/vendors/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      116 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/__init__.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)    38933 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/aws.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      520 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/gcp.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     9834 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/hcloud.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1298 2024-04-12 15:19:56.000000 sparecores_crawler-0.1.1/src/sc_crawler/vendors/vendors.py
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.194913 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     7384 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/PKG-INFO
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1042 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/SOURCES.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)        1 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/dependency_links.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       50 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/entry_points.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)      495 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/requires.txt
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)       11 2024-04-12 17:16:58.000000 sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/top_level.txt
+drwxr-xr-x   0 daroczig  (1000) daroczig  (1000)        0 2024-04-12 17:16:58.194913 sparecores_crawler-0.1.1/tests/
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1391 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/tests/test_schemas.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1316 2024-04-04 14:00:10.000000 sparecores_crawler-0.1.1/tests/test_str_utils.py
+-rw-r--r--   0 daroczig  (1000) daroczig  (1000)     1216 2024-03-25 14:01:48.000000 sparecores_crawler-0.1.1/tests/test_utils.py
```

### Comparing `sparecores-crawler-0.1.0/LICENSE` & `sparecores_crawler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/PKG-INFO` & `sparecores_crawler-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alembic
 Requires-Dist: cachier
 Requires-Dist: pydantic
 Requires-Dist: pydantic_extra_types
 Requires-Dist: rich
 Requires-Dist: sqlmodel
 Requires-Dist: typer
 Provides-Extra: mkdocs
@@ -33,16 +34,19 @@
 Requires-Dist: griffe; extra == "mkdocs"
 Requires-Dist: griffe-inherited-docstrings; extra == "mkdocs"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: sparecores-crawler[mkdocs]; extra == "testing"
 Provides-Extra: aws
 Requires-Dist: boto3; extra == "aws"
+Provides-Extra: hcloud
+Requires-Dist: hcloud; extra == "hcloud"
 Provides-Extra: vendors
 Requires-Dist: sparecores-crawler[aws]; extra == "vendors"
+Requires-Dist: sparecores-crawler[hcloud]; extra == "vendors"
 Provides-Extra: all
 Requires-Dist: sparecores-crawler[testing]; extra == "all"
 Requires-Dist: sparecores-crawler[vendors]; extra == "all"
 
 ## Spare Cores Crawler
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-crawler/tests.yaml)](https://github.com/SpareCores/sc-crawler/actions/workflows/tests.yaml)
```

### Comparing `sparecores-crawler-0.1.0/README.md` & `sparecores_crawler-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/pyproject.toml` & `sparecores_crawler-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sparecores-crawler"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">= 3.7"
 dependencies = [
+  "alembic",
   "cachier",
   "pydantic",
   "pydantic_extra_types",
   "rich",
   "sqlmodel",
   "typer",
 ]
@@ -43,20 +44,24 @@
   "mkdocs-material[imaging]==9.5.13", "mkdocs-material-extensions",
   "mkdocs-autorefs", "mkdocs-gen-files", "mkdocs-literate-nav", "mkdocs-section-index",
   "mkdocstrings[python]>=0.18",
   "griffe", "griffe-inherited-docstrings",
 ]
 testing = ["pytest", "sparecores-crawler[mkdocs]"]
 aws = ["boto3"]
-vendors = ["sparecores-crawler[aws]"]
+hcloud = ["hcloud"]
+vendors = ["sparecores-crawler[aws]", "sparecores-crawler[hcloud]"]
 all = ["sparecores-crawler[testing]", "sparecores-crawler[vendors]"]
 
 [project.scripts]
 sc-crawler = "sc_crawler.cli:cli"
 
+[tool.setuptools]
+include-package-data = true  # see MANIFEST.in
+
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
```

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/cli.py` & `sparecores_crawler-0.1.1/src/sc_crawler/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 Check `sc-crawler --help` for more details."""
 
 import logging
 from datetime import datetime, timedelta
 from enum import Enum
 from json import dumps, loads
 from pathlib import Path
-from typing import List
+from types import SimpleNamespace
+from typing import List, Optional
 
 import typer
+from alembic import command
 from cachier import set_default_params
 from rich.console import Console
 from rich.live import Live
 from rich.panel import Panel
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
@@ -23,14 +25,15 @@
 )
 from rich.table import Table
 from rich.text import Text
 from sqlmodel import Session, create_engine, select
 from typing_extensions import Annotated
 
 from . import vendors as vendors_module
+from .alembic_helpers import alembic_cfg, get_revision
 from .insert import insert_items
 from .logger import ProgressPanel, ScRichHandler, VendorProgressTracker, logger
 from .lookup import compliance_frameworks, countries
 from .table_fields import Status
 from .tables import Vendor, tables
 from .tables_scd import tables_scd
 from .utils import HashLevels, get_row_by_pk, hash_database, table_name_to_model
@@ -60,47 +63,160 @@
 supported_records = [r[10:] for r in dir(Vendor) if r.startswith("inventory_")]
 Records = Enum("RECORDS", {k: k for k in supported_records})
 
 table_names = [t.get_table_name() for t in tables]
 Tables = Enum("TABLES", {k: k for k in table_names})
 
 
-@cli.command()
-def schema(
+alembic_app = typer.Typer()
+cli.add_typer(
+    alembic_app, name="schemas", help="Database migration utilities using Alembic."
+)
+
+options = SimpleNamespace(
+    connection_string=Annotated[
+        str, typer.Option(help="Database URL with SQLAlchemy dialect.")
+    ],
+    revision=Annotated[
+        str,
+        typer.Option(
+            help="Target revision passed to Alembic. Use 'heads' to get to the most recent version."
+        ),
+    ],
+    scd=Annotated[
+        bool,
+        typer.Option(help="Migrate the SCD tables instead of the standard tables."),
+    ],
+    sql=Annotated[
+        bool,
+        typer.Option(help="Dry-run, printing the SQL commands instead of running."),
+    ],
+)
+
+
+@alembic_app.command()
+def create(
+    connection_string: Annotated[
+        Optional[str], typer.Option(help="Database URL with SQLAlchemy dialect.")
+    ] = None,
     dialect: Annotated[
-        Engines,
+        Optional[Engines],
         typer.Option(
             help="SQLAlchemy dialect to use for generating CREATE TABLE statements."
         ),
-    ],
+    ] = None,
     scd: Annotated[
         bool, typer.Option(help="If SCD Type 2 tables should be also created.")
     ] = False,
 ):
     """
     Print the database schema in a SQL dialect.
+
+    Either `connection_string` or `dialect` is to be provided to decide
+    what SQL dialect to use to generate the CREATE TABLE (and related)
+    SQL statements.
     """
-    url = engine_to_dialect[dialect.value]
+    if connection_string is None and dialect is None:
+        print("Either connection_string or dialect parameters needs to be provided!")
+        raise typer.Exit(code=1)
+    if dialect:
+        url = engine_to_dialect[dialect.value]
+    else:
+        url = connection_string
 
     def metadata_dump(sql, *_args, **_kwargs):
         typer.echo(str(sql.compile(dialect=engine.dialect)) + ";")
 
     engine = create_engine(url, strategy="mock", executor=metadata_dump)
     for table in tables:
         table.__table__.create(engine)
     if scd:
         for table in tables_scd:
             table.__table__.create(engine)
 
 
+@alembic_app.command()
+def current(
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
+    scd: options.scd = False,
+):
+    """
+    Show current database revision.
+    """
+    engine = create_engine(connection_string)
+    with engine.begin() as connection:
+        command.current(alembic_cfg(connection, scd))
+
+
+@alembic_app.command()
+def upgrade(
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
+    revision: options.revision = "heads",
+    scd: options.scd = False,
+    sql: options.sql = False,
+):
+    """
+    Upgrade the database schema to a given (default: most recent) revision.
+    """
+    engine = create_engine(connection_string)
+    with engine.begin() as connection:
+        command.upgrade(alembic_cfg(connection, scd), revision, sql)
+
+
+@alembic_app.command()
+def downgrade(
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
+    revision: options.revision = "-1",
+    scd: options.scd = False,
+    sql: options.sql = False,
+):
+    """
+    Downgrade the database schema to a given (default: previous) revision.
+    """
+    engine = create_engine(connection_string)
+    with engine.begin() as connection:
+        command.downgrade(alembic_cfg(connection, scd), revision, sql)
+
+
+@alembic_app.command()
+def stamp(
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
+    revision: options.revision = "heads",
+    scd: options.scd = False,
+    sql: options.sql = False,
+):
+    """
+    Set the migration revision mark in he database to a specified revision. Set to "heads" if the database schema is up-to-date.
+    """
+    engine = create_engine(connection_string)
+    with engine.begin() as connection:
+        command.stamp(alembic_cfg(connection, scd), revision, sql)
+
+
+@alembic_app.command()
+def autogenerate(
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
+    message: Annotated[
+        str,
+        typer.Option(help="Revision message, e.g. SC Crawler version number."),
+    ] = "empty message",
+):
+    """
+    Autogenerate a migrations script based on the current state of a database.
+    """
+    engine = create_engine(connection_string)
+    with engine.begin() as connection:
+        command.revision(
+            alembic_cfg(connection=connection), autogenerate=True, message=message
+        )
+
+
 @cli.command(name="hash")
 def hash_command(
-    connection_string: Annotated[
-        str, typer.Option(help="Database URL with SQLAlchemy dialect.")
-    ] = "sqlite:///sc-data-all.db",
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
 ):
     """Print the hash of the content of a database."""
     print(hash_database(connection_string))
 
 
 @cli.command()
 def copy(
@@ -113,21 +229,21 @@
     target: Annotated[
         str,
         typer.Option(
             help="Database URL (SQLAlchemy connection string) that is to be populated with the content of `source`."
         ),
     ],
 ):
-    """Copy the content of a database to a blank database."""
+    """Copy the standard SC Crawler tables of a database into a blank database."""
 
     source_engine = create_engine(source)
     target_engine = create_engine(target)
 
     for table in tables:
-        table.__table__.create(target_engine, checkfirst=True)
+        table.__table__.create(target_engine)
 
     progress = Progress(
         TimeElapsedColumn(),
         TextColumn("{task.description}"),
         BarColumn(),
         MofNCompleteColumn(),
     )
@@ -139,14 +255,16 @@
         Session(target_engine) as target_session,
     ):
         for table in tables:
             rows = source_session.exec(statement=select(table))
             items = [row.model_dump() for row in rows]
             insert_items(table, items, session=target_session, progress=progress)
         target_session.commit()
+    with target_engine.begin() as connection:
+        command.stamp(alembic_cfg(connection), "heads")
 
 
 @cli.command()
 def sync(
     source: Annotated[
         str,
         typer.Option(
@@ -193,14 +311,29 @@
 
     The records marked for syncing are written to the `target` database's
     standard or SCD tables. When updating the SCD tables, the hashing still
     happens on the standard tables/views, which are probably based on the
     most recent records of the SCD tables.
     """
 
+    source_engine = create_engine(source)
+    target_engine = create_engine(target)
+
+    # compare source and target database revisions, halt if not matching
+    with source_engine.connect() as connection:
+        current_rev = get_revision(connection)
+    with target_engine.begin() as connection:
+        target_rev = get_revision(connection)
+    if current_rev != target_rev:
+        print(
+            "Database revisions do NOT match, so not risking the sync. "
+            "Upgrade the database(s) before trying again!"
+        )
+        raise typer.Exit(code=1)
+
     ps = Progress(
         TimeElapsedColumn(),
         TextColumn("{task.description}"),
         BarColumn(),
         MofNCompleteColumn(),
     )
     pt = Progress(
@@ -245,16 +378,15 @@
     g = Table.grid(padding=1)
     g.add_row(
         Panel(ps, title="Comparing source database with target"),
         Panel(pt, title="Comparing target database with source"),
     )
     with Live(g):
         # compare new records with old
-        engine = create_engine(source)
-        with Session(engine) as session:
+        with Session(source_engine) as session:
             tables_task_id = ps.add_task("Comparing tables", total=len(source_hash))
             for table_name, items in source_hash.items():
                 table_task_id = ps.add_task(table_name, total=len(items))
                 model = table_name_to_model(table_name)
                 for pks_json, item in items.items():
                     action = None
                     try:
@@ -267,16 +399,15 @@
                         # source database and store as JSON for future update
                         obj = get_row_by_pk(session, model, loads(pks_json))
                         actions[action][table_name].append(obj.model_dump())
                     ps.update(table_task_id, advance=1)
                 ps.update(tables_task_id, advance=1)
 
         # compare old records with new
-        engine = create_engine(target)
-        with Session(engine) as session:
+        with Session(target_engine) as session:
             tables_task_id = pt.add_task("Comparing tables", total=len(target_hash))
             for table_name, items in target_hash.items():
                 table_task_id = pt.add_task(table_name, total=len(items))
                 model = table_name_to_model(table_name)
                 for key, _ in items.items():
                     if key not in source_hash[table_name]:
                         # check if the row was already set to INACTIVE
@@ -328,16 +459,15 @@
         progress = Progress(
             TimeElapsedColumn(),
             TextColumn("{task.description}"),
             BarColumn(),
             MofNCompleteColumn(),
         )
         panel = Panel(progress, title="Updating target", expand=False)
-        engine = create_engine(target)
-        with Live(panel), Session(engine) as session:
+        with Live(panel), Session(target_engine) as session:
             for table_name, _ in source_hash.items():
                 model = table_name_to_model(table_name)
                 if scd:
                     model = model.get_scd()
                 items = (
                     actions["new"][table_name]
                     + actions["update"][table_name]
@@ -347,17 +477,15 @@
                     insert_items(model, items, session=session, progress=progress)
                     logger.info("Updated %d %s(s) rows" % (len(items), table_name))
             session.commit()
 
 
 @cli.command()
 def pull(
-    connection_string: Annotated[
-        str, typer.Option(help="Database URL with SQLAlchemy dialect.")
-    ] = "sqlite:///sc-data-all.db",
+    connection_string: options.connection_string = "sqlite:///sc-data-all.db",
     include_vendor: Annotated[
         List[Vendors],
         typer.Option(help="Enabled data sources. Can be specified multiple times."),
     ] = [v.vendor_id for v in supported_vendors],
     exclude_vendor: Annotated[
         List[Vendors],
         typer.Option(help="Disabled data sources. Can be specified multiple times."),
@@ -419,18 +547,14 @@
             and vendor.vendor_id not in [ev.value for ev in exclude_vendor]
         )
     ]
 
     # filter reocrds
     records = [r for r in include_records if r not in exclude_records]
 
-    engine = create_engine(connection_string, json_serializer=custom_serializer)
-    for table in tables:
-        table.__table__.create(engine, checkfirst=True)
-
     pbars = ProgressPanel()
     with Live(pbars.panels):
         # show CLI arguments in the Metadata panel
         pbars.metadata.append(Text("Data sources: ", style="bold"))
         pbars.metadata.append(Text(", ".join([x.vendor_id for x in vendors]) + " "))
         pbars.metadata.append(Text("Updating records: ", style="bold"))
         pbars.metadata.append(Text(", ".join([x.value for x in records]) + "\n"))
@@ -440,14 +564,19 @@
         if cache:
             pbars.metadata.append(Text("Enabled (" + str(cache_ttl) + "m)"))
         else:
             pbars.metadata.append(Text("Disabled"))
         pbars.metadata.append(Text(" Time: ", style="bold"))
         pbars.metadata.append(Text(str(datetime.now())))
 
+        # alembic upgrade to ensure using the most recent version of the schemas
+        engine = create_engine(connection_string, json_serializer=custom_serializer)
+        with engine.begin() as connection:
+            command.upgrade(alembic_cfg(connection, force_logging=False), "heads")
+
         with Session(engine) as session:
             # add/merge static objects to database
             for compliance_framework in compliance_frameworks.values():
                 session.merge(compliance_framework)
             logger.info("%d Compliance Frameworks synced." % len(compliance_frameworks))
             for country in countries.values():
                 session.merge(country)
```

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/insert.py` & `sparecores_crawler-0.1.1/src/sc_crawler/insert.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/logger.py` & `sparecores_crawler-0.1.1/src/sc_crawler/logger.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/str_utils.py` & `sparecores_crawler-0.1.1/src/sc_crawler/str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/table_bases.py` & `sparecores_crawler-0.1.1/src/sc_crawler/table_bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
 class HasDescription(ScModel):
     description: Optional[str] = Field(description="Short description.")
 
 
 class HasVendorPKFK(ScModel):
     vendor_id: str = Field(
-        foreign_key="vendor",
+        foreign_key="vendor.vendor_id",
         primary_key=True,
         description="Reference to the Vendor.",
     )
 
 
 class HasDatacenterPK(ScModel):
     datacenter_id: str = Field(
@@ -337,15 +337,15 @@
     )
     homepage: Optional[str] = Field(
         default=None,
         description="Public homepage of the Vendor.",
     )
 
     country_id: str = Field(
-        foreign_key="country",
+        foreign_key="country.country_id",
         description="Reference to the Country, where the Vendor's main headquarter is located.",
     )
     state: Optional[str] = Field(
         default=None,
         description="Optional state/administrative area of the Vendor's location within the Country.",
     )
     city: Optional[str] = Field(
@@ -369,15 +369,15 @@
 
 class VendorBase(MetaColumns, VendorFields):
     pass
 
 
 class VendorComplianceLinkFields(HasVendorPKFK):
     compliance_framework_id: str = Field(
-        foreign_key="compliance_framework",
+        foreign_key="compliance_framework.compliance_framework_id",
         primary_key=True,
         description="Reference to the Compliance Framework.",
     )
     comment: Optional[str] = Field(
         default=None,
         description="Optional references, such as dates, URLs, and additional information/evidence.",
     )
@@ -390,15 +390,15 @@
 class DatacenterFields(HasName, HasDatacenterIdPK, HasVendorPKFK):
     aliases: List[str] = Field(
         default=[],
         sa_type=JSON,
         description="List of other commonly used names for the same Datacenter.",
     )
     country_id: str = Field(
-        foreign_key="country",
+        foreign_key="country.country_id",
         description="Reference to the Country, where the Datacenter is located.",
     )
     state: Optional[str] = Field(
         default=None,
         description="Optional state/administrative area of the Datacenter's location within the Country.",
     )
     city: Optional[str] = Field(
@@ -446,32 +446,28 @@
     )
 
 
 class StorageBase(MetaColumns, StorageFields):
     pass
 
 
-class ServerFields(HasServerIdPK, HasVendorPKFK):
-    name: str = Field(
-        default=None,
-        description="Human-friendly name or short description.",
-    )
+class ServerFields(HasDescription, HasName, HasServerIdPK, HasVendorPKFK):
     vcpus: int = Field(
         default=None,
         description="Default number of virtual CPUs (vCPU) of the server.",
     )
     hypervisor: Optional[str] = Field(
         default=None,
         description="Hypervisor of the virtual server, e.g. Xen, KVM, Nitro or Dedicated.",
     )
     cpu_allocation: CpuAllocation = Field(
         default=None,
         description="Allocation of CPU(s) to the server, e.g. shared, burstable or dedicated.",
     )
-    cpu_cores: int = Field(
+    cpu_cores: Optional[int] = Field(
         default=None,
         description=(
             "Default number of CPU cores of the server. "
             "Equals to vCPUs when HyperThreading is disabled."
         ),
     )
     cpu_speed: Optional[float] = Field(
@@ -515,15 +511,15 @@
     )
     gpu_memory_total: Optional[int] = Field(
         default=None,
         description="Overall memory (MiB) allocated to all the GPU accelerator(s).",
     )
     gpu_manufacturer: Optional[str] = Field(
         default=None,
-        description="The manufacturer of the primary GPU accelerator, e.g. Nvidia or AMD",
+        description="The manufacturer of the primary GPU accelerator, e.g. Nvidia or AMD.",
     )
     gpu_model: Optional[str] = Field(
         default=None,
         description="The model number of the primary GPU accelerator.",
     )
     gpus: List[Gpu] = Field(
         default=[],
```

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/table_fields.py` & `sparecores_crawler-0.1.1/src/sc_crawler/table_fields.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/tables.py` & `sparecores_crawler-0.1.1/src/sc_crawler/tables.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/tables_scd.py` & `sparecores_crawler-0.1.1/src/sc_crawler/tables_scd.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/utils.py` & `sparecores_crawler-0.1.1/src/sc_crawler/utils.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/vendors/aws.py` & `sparecores_crawler-0.1.1/src/sc_crawler/vendors/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List, Optional, Tuple
 
 import boto3
 from botocore.exceptions import ClientError
 from cachier import cachier, set_default_params
 
 from ..logger import logger
+from ..lookup import map_compliance_frameworks_to_vendor
 from ..str_utils import extract_last_number
 from ..table_fields import (
     Allocation,
     CpuAllocation,
     Disk,
     Gpu,
     PriceTier,
@@ -364,24 +365,17 @@
 
 # ##############################################################################
 # Public methods to fetch data
 
 
 def inventory_compliance_frameworks(vendor):
     """Manual list of compliance frameworks known for AWS."""
-    compliance_frameworks = ["hipaa", "soc2t2"]
-    items = []
-    for compliance_framework in compliance_frameworks:
-        items.append(
-            {
-                "vendor_id": vendor.vendor_id,
-                "compliance_framework_id": compliance_framework,
-            }
-        )
-    return items
+    return map_compliance_frameworks_to_vendor(
+        vendor.vendor_id, ["hipaa", "soc2t2", "iso27001"]
+    )
 
 
 def inventory_datacenters(vendor):
     """List all available AWS datacenters via `boto3` calls.
 
     Some data sources are not available from APIs, and were collected manually:
```

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/vendors/gcp.py` & `sparecores_crawler-0.1.1/src/sc_crawler/vendors/gcp.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/src/sc_crawler/vendors/vendors.py` & `sparecores_crawler-0.1.1/src/sc_crawler/vendors/vendors.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from ..lookup import countries
 from ..tables import Vendor
 
 aws = Vendor(
     vendor_id="aws",
     name="Amazon Web Services",
+    # TODO host on cdn.sparecores.com
+    logo="https://upload.wikimedia.org/wikipedia/commons/9/93/Amazon_Web_Services_Logo.svg",
     homepage="https://aws.amazon.com",
     country=countries["US"],
     state="Washington",
     city="Seattle",
     address_line="410 Terry Ave N",
     zip_code="98109",
     founding_year=2002,
@@ -26,7 +28,21 @@
     city="Mountain View",
     address_line="1600 Amphitheatre Pkwy",
     zip_code="94043",
     founding_year=2008,
     status_page="https://status.cloud.google.com/",
 )
 """Google Cloud Platform."""
+
+hcloud = Vendor(
+    vendor_id="hcloud",
+    name="Hetzner Cloud",
+    homepage="https://www.hetzner.com/cloud/",
+    country=countries["DE"],
+    state="Bavaria",
+    city="Gunzenhausen",
+    address_line="Industriestr. 25",
+    zip_code="91710",
+    founding_year=1997,
+    status_page="https://status.hetzner.com/",
+)
+"""Hetzner Cloud."""
```

### Comparing `sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/PKG-INFO` & `sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: sparecores-crawler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pull and standardize data on cloud compute resources.
 Author: Attila Nagy, Gergely Daroczi, Balazs Hodobay
 Maintainer-email: Spare Cores team <pkg@sparecores.com>
 Project-URL: repository, https://github.com/SpareCores/sc-crawler
 Project-URL: issues, https://github.com/SpareCores/sc-crawler/issues
 Project-URL: documentation, https://sparecores.github.io/sc-crawler/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alembic
 Requires-Dist: cachier
 Requires-Dist: pydantic
 Requires-Dist: pydantic_extra_types
 Requires-Dist: rich
 Requires-Dist: sqlmodel
 Requires-Dist: typer
 Provides-Extra: mkdocs
@@ -33,16 +34,19 @@
 Requires-Dist: griffe; extra == "mkdocs"
 Requires-Dist: griffe-inherited-docstrings; extra == "mkdocs"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: sparecores-crawler[mkdocs]; extra == "testing"
 Provides-Extra: aws
 Requires-Dist: boto3; extra == "aws"
+Provides-Extra: hcloud
+Requires-Dist: hcloud; extra == "hcloud"
 Provides-Extra: vendors
 Requires-Dist: sparecores-crawler[aws]; extra == "vendors"
+Requires-Dist: sparecores-crawler[hcloud]; extra == "vendors"
 Provides-Extra: all
 Requires-Dist: sparecores-crawler[testing]; extra == "all"
 Requires-Dist: sparecores-crawler[vendors]; extra == "all"
 
 ## Spare Cores Crawler
 
 [![Build](https://img.shields.io/github/actions/workflow/status/SpareCores/sc-crawler/tests.yaml)](https://github.com/SpareCores/sc-crawler/actions/workflows/tests.yaml)
```

### Comparing `sparecores-crawler-0.1.0/src/sparecores_crawler.egg-info/SOURCES.txt` & `sparecores_crawler-0.1.1/src/sparecores_crawler.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/sc_crawler/__init__.py
+src/sc_crawler/alembic.ini
+src/sc_crawler/alembic_helpers.py
 src/sc_crawler/cli.py
 src/sc_crawler/insert.py
 src/sc_crawler/logger.py
 src/sc_crawler/lookup.py
 src/sc_crawler/str_utils.py
 src/sc_crawler/table_bases.py
 src/sc_crawler/table_fields.py
 src/sc_crawler/tables.py
 src/sc_crawler/tables_scd.py
 src/sc_crawler/utils.py
+src/sc_crawler/alembic/env.py
+src/sc_crawler/alembic/versions/4691089690c2_v0_1_1.py
+src/sc_crawler/alembic/versions/98894dffd37c_v0_1_0.py
 src/sc_crawler/vendors/__init__.py
 src/sc_crawler/vendors/aws.py
 src/sc_crawler/vendors/gcp.py
+src/sc_crawler/vendors/hcloud.py
 src/sc_crawler/vendors/vendors.py
 src/sparecores_crawler.egg-info/PKG-INFO
 src/sparecores_crawler.egg-info/SOURCES.txt
 src/sparecores_crawler.egg-info/dependency_links.txt
 src/sparecores_crawler.egg-info/entry_points.txt
 src/sparecores_crawler.egg-info/requires.txt
 src/sparecores_crawler.egg-info/top_level.txt
```

### Comparing `sparecores-crawler-0.1.0/tests/test_schemas.py` & `sparecores_crawler-0.1.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/tests/test_str_utils.py` & `sparecores_crawler-0.1.1/tests/test_str_utils.py`

 * *Files identical despite different names*

### Comparing `sparecores-crawler-0.1.0/tests/test_utils.py` & `sparecores_crawler-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

