# Comparing `tmp/neoval_py_utils-0.3.0.tar.gz` & `tmp/neoval_py_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neoval_py_utils-0.3.0.tar", max compression
+gzip compressed data, was "neoval_py_utils-0.3.1.tar", max compression
```

## Comparing `neoval_py_utils-0.3.0.tar` & `neoval_py_utils-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7738 2024-03-25 01:05:57.167953 neoval_py_utils-0.3.0/README.md
--rw-r--r--   0        0        0     2604 2024-03-25 01:05:58.119958 neoval_py_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       35 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/__init__.py
--rw-r--r--   0        0        0     6131 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/exporter.py
--rwxr-xr-x   0        0        0     3897 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb.py
--rwxr-xr-x   0        0        0      553 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb_build_event.py
--rwxr-xr-x   0        0        0    21187 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb_builder.py
--rw-r--r--   0        0        0     4191 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/template.py
--rw-r--r--   0        0        0     3045 2024-03-25 01:05:57.171953 neoval_py_utils-0.3.0/src/neoval_py_utils/utils.py
--rw-r--r--   0        0        0     8441 1970-01-01 00:00:00.000000 neoval_py_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6396 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/README.md
+-rw-r--r--   0        0        0     2818 2024-04-12 02:46:40.635305 neoval_py_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/__init__.py
+-rw-r--r--   0        0        0     6131 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/exporter.py
+-rwxr-xr-x   0        0        0     3869 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb.py
+-rw-r--r--   0        0        0      553 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_build_event.py
+-rwxr-xr-x   0        0        0    21941 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_builder.py
+-rw-r--r--   0        0        0     4191 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/template.py
+-rw-r--r--   0        0        0     3045 2024-04-12 02:46:39.723303 neoval_py_utils-0.3.1/src/neoval_py_utils/utils.py
+-rw-r--r--   0        0        0     7099 1970-01-01 00:00:00.000000 neoval_py_utils-0.3.1/PKG-INFO
```

### Comparing `neoval_py_utils-0.3.0/README.md` & `neoval_py_utils-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,47 @@
+Metadata-Version: 2.1
+Name: neoval-py-utils
+Version: 0.3.1
+Summary: 
+Author: Neoval
+Author-email: data@neoval.io
+Requires-Python: >=3.10,<=3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: duckdb (>=0.9.2,<0.10.0)
+Requires-Dist: google-cloud-bigquery
+Requires-Dist: google-cloud-storage
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: polars
+Requires-Dist: pyarrow
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Requires-Dist: taskipy (>=1.12.2,<2.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
+
 # neoval-py-utils
 
-Python Utilities
+neoval-py-utils is a python utilities package developed by [Neoval](https://neoval.io) to assist with the Extract, Load and Transform
+(ELT/ETL) of data from Google Cloud Platform (GCP) services.
+
+The main difference between this utilities package and [BigQuery provided APIs](https://cloud.google.com/bigquery/docs/samples/bigquery-list-rows-dataframe)
+is a faster export. Running a [BigQuery extract_job](https://cloud.google.com/python/docs/reference/bigquery/latest/google.cloud.bigquery.job.ExtractJob) 
+to a bucket and downloading it is faster and can be improved by increasing the machine's download speed. We also use of local caching so that the same query will not needless be repeatedly be executed / downloaded. 
+With this package the user can also create, databases that can be embedded to a machine for a website or application.
+
+Functionalities include:
+- exporter
+  - Exporting data from BigQuery(bq) to a pandas DataFrame, pyArrow Table or Google Cloud Storage (GCS).
+  - Can be a bq query or a bq table.
+- ipdb
+  - Building and preparing embedded in-process databases (IPDB) from BigQuery datasets.
+  - Supports SQLite and DuckDB and configured with a YAML file please see examples below.
+  - Supports templating for transformations post initial build.
 
 # Development
 
 All development must take place on a feature branch and a pull request is required; a user is not allowed to commit directly to `main`. The automated workflow in this repo (using `python-semantic-release`) requires the use of [angular style](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#commits) commit messages to update the package version and `CHANGELOG`. All commits must be formatted in this way before a user is able to merge a PR; a user who may want to develop without using this format for all commits can simply squash non-angular commit messages prior to merge. A PR may only be merged by the `rebase and merge` method. This is to ensure that only angular style commits end up on `main`.
 
 Upon merge to `main`, the `deploy` workflow will facilitate the following:
 
@@ -59,34 +96,43 @@
 
 # To export bigquery table to a parquet file in a gcp storage bucket. Returns a list of blobs.
 blobs = exporter.bq_to_gcs("my-dataset.my-table")
 ```
 ### Create In-process(Embedded) Databases #######
 
 ```shell
-# Pythong cli example to build in-process db
-poetry run python ipdb build <DBT_DATASET> <GCLOUD_PROJECT_ID> <DB_PATH> <CONFIG_PATH> --upload-bucket <UPLOAD_BUCKET> 
+# Python cli example to build in-process db
+poetry run ipdb build <DBT_DATASET> <GCLOUD_PROJECT_ID> <DB_PATH> <CONFIG_PATH> --upload-bucket <UPLOAD_BUCKET> 
 # If you would like to run it in locally in this repo, you can run
 # Upload bucket is optional, this will upload the in-process db to the specified bucket.
-poetry run python neoval_py_utils/ipdb.py build samples bigquery-public-data tests/artifacts/in_process_db tests/resources/good.config.yaml
+# Ensure your PYTHONPATH=./src
+poetry run ipdb build samples bigquery-public-data tests/artifacts/in_process_db tests/resources/good.config.yaml
 
+```
+Example of config.yaml
+```yaml
+sqlite:
+    -   name: shakespeare
+        primary_key: null
+duckdb:
+    -   name: shakespeare
+        primary_key: null
+        description: "Word counts from Shakespeare work - gcp public dataset"
+```
+
+```shell
 # To apply sql templates after the in-process db is built
-poetry run python ipdb prepare <DBT_DATASET> <GCLOUD_PROJECT_ID> <DB_PATH> <TEMPLATES_PATH>
+poetry run ipdb prepare <DBT_DATASET> <GCLOUD_PROJECT_ID> <DB_PATH> <TEMPLATES_PATH>
 # If you would like to run it in locally in this repo, you can run
-poetry run python neoval_py_utils/ipdb.py samples bigquery-public-data tests/artifacts/in_process_db tests/resources/templates
+poetry run ipdb prepare samples bigquery-public-data tests/artifacts/in_process_db tests/resources/templates
 # For more info you can run
-poetry run python neoval_py_utils/ipdb.py --help # which will return 
+poetry run ipdb --help # which will return 
                                                                                                                                      
- Usage: ipdb.py [OPTIONS] COMMAND [ARGS]...                                                                                                                                                               
-                                                                                                                                                                                                          
-╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --install-completion          Install completion for the current shell.                                                                                                                                │
-│ --show-completion             Show completion for the current shell, to copy it or customize the installation.                                                                                         │
-│ --help                        Show this message and exit.                                                                                                                                              │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
-╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ build                           Build the in process database(s).                                                                                                                                      │
-│ make-config                     Prints a default configuration to be used with the build command.                                                                                                      │
-│ prepare                         Run scripts to add views/virtual tables/etc. to the database(s).                                                                                                       │
-╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+ Usage: ipdb [OPTIONS] COMMAND [ARGS]...                                                                                                                                                               
+╭─ Commands ────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│ build                           Build the in process database(s).                                                 │
+│ make-config                     Prints a default configuration to be used with the build command.                 │
+│ prepare                         Run scripts to add views/virtual tables/etc. to the database(s).                  │
+╰───────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+
```

### Comparing `neoval_py_utils-0.3.0/pyproject.toml` & `neoval_py_utils-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 [tool.poetry]
 name = "neoval-py-utils"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Neoval <data@neoval.io>"]
 readme = "README.md"
+packages = [{include = "neoval_py_utils", from = "src"}]
+
+
+[tool.poetry.scripts]
+ipdb = "neoval_py_utils.ipdb:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<=3.12"
 google-cloud-storage = "*"
 google-cloud-bigquery = "*"
 polars = "*"
 pyarrow= "*"
@@ -21,24 +26,26 @@
 black = "*"
 ruff = "*"
 pytest = "*"
 pytest-xdist = "*"
 pytest-cov = "*"
 taskipy = "^1.12.2"
 python-semantic-release = "^8.7.0"
+pyright = "*"
+
 
 
 [tool.taskipy.tasks]
 format = "black ."
 lint = "ruff check --output-format grouped src/ tests/"
 test = "pytest tests/ -n auto"
-test-with-coverage = "pytest -n auto --cov=src --cov-fail-under=90 tests/"
+test-with-coverage = "pytest -n auto --cov=src/neoval_py_utils --cov-fail-under=90 tests/"
 
 [tool.pytest.ini_options]
-pythonpath = "src"
+pythonpath = "."
 addopts = [
     "--import-mode=importlib",
 ]
 
 [tool.ruff]
 line-length = 100
 
@@ -91,17 +98,17 @@
 autoescape = true
 
 [tool.semantic_release.commit_author]
 env = "GIT_COMMIT_AUTHOR"
 default = "semantic-release <semantic-release>"
 
 [tool.semantic_release.commit_parser_options]
-allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test"]
+allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test", "major"]
 minor_tags = ["feat"]
-patch_tags = ["fix", "perf"]
+patch_tags = ["build", "chore", "ci", "docs", "fix", "perf", "style", "refactor", "test"]
 
 [tool.semantic_release.remote]
 name = "origin"
 type = "github"
 ignore_token_for_push = false
 
 [tool.semantic_release.remote.token]
```

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/exporter.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/exporter.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,17 +108,17 @@
                     ]
                 )
             )
 
         if code == 1:
             raise typer.Exit(code=code)
 
-    except:  # noqa: E722
+    except Exception as e:
         traceback.print_exc()
-        raise typer.Exit(code=1)
+        raise e
 
 
 @app.command()
 def prepare(
     dataset: str, project: str, db_directory: Path, template_path: Path
 ) -> None:
     """Run scripts to add views/virtual tables/etc. to the database(s)."""
@@ -130,15 +130,15 @@
         )
 
         event: IPDBBuildEvent
         for event in events:
             print(event.type, event.data.get("database"), file=stderr)
             print(event.data.get("tables"), "\n", file=stderr)
 
-    except Exception:
+    except Exception as e:
         traceback.print_exc()
         typer.Exit(code=1)
-        raise typer.Exit(code=1)
+        raise e
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb_build_event.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_build_event.py`

 * *Files identical despite different names*

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/ipdb_builder.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/ipdb_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,44 +331,44 @@
                 )
             )
             + pk
             + "\n)"
         )
 
     @staticmethod
-    def _prepare_directory_and_pathname(s: str | Path, pathname: str) -> Path:
-        """Prepare pathnames for build method.
+    def _prepare_directory_and_pathname(path_ref: str | Path, pathname: str) -> Path:
+        """Prepare pathname for build method.
 
-        Ensure that `p` exists, and that the specified pathname within it
+        Ensure that `path_ref` exists, and that the specified pathname within it
         does not. If those files / folders exist, they are deleted - so that the
         returned `Path`s always reference files that don't exist on disk.
         """
-        p: Path = Path(s)
+        p: Path = Path(path_ref)
 
         if not p.exists():
             p.mkdir()
 
         pathname = p / pathname
         if pathname.exists():
             pathname.unlink()
 
         return pathname
 
     @staticmethod
-    def _prepare_pathnames(s: str | Path, pathname: str) -> Path:
+    def _verify_directory_and_pathname(path_ref: str | Path, pathname: str) -> Path:
         """Prepare pathnames for prepare method.
 
-        Ensure that `p` and the pathnames exist, otherwise raises an error.
+        Ensure that `path_ref` and the pathnames exist, otherwise raises an error.
         Opposite to the method above, this is used in the `prepare` method to ensure
         that the databases we want to operate on have already been created.
         """
-        p: Path = Path(s)
+        p: Path = Path(path_ref)
 
         if not p.exists():
-            raise ValueError(f"{s} directory does not exist.")
+            raise ValueError(f"{path_ref} directory does not exist.")
 
         pathname = p / pathname
         if not pathname.exists():
             raise FileNotFoundError(f"{pathname} does not exist.")
 
         return pathname
 
@@ -466,51 +466,60 @@
                 "name": name,
                 "create_table_statement": sqlite_create_table_statement,
             },
         )
 
     def _build_sqlite(self, sqlite_path: Path, metadata: list) -> None:
         sqlite_con: SQLiteConnection = sqlite3.connect(str(sqlite_path))
+        try:
+            sqlite3.register_adapter(dict, IPDBBuilder._composite_adapter)
+            sqlite3.register_adapter(list, IPDBBuilder._composite_adapter)
+
+            sqlite_con.execute("PRAGMA journal_mode = WAL;")
+            sqlite_con.execute("PRAGMA cache_size = -5000;")
+            sqlite_con.execute("PRAGMA synchronous = NORMAL")
 
-        sqlite3.register_adapter(dict, IPDBBuilder._composite_adapter)
-        sqlite3.register_adapter(list, IPDBBuilder._composite_adapter)
+            for table in metadata:
+                yield self._create_sqlite_table(table, sqlite_con)
 
-        sqlite_con.execute("PRAGMA journal_mode = WAL;")
-        sqlite_con.execute("PRAGMA cache_size = -5000;")
-        sqlite_con.execute("PRAGMA synchronous = NORMAL")
-
-        for table in metadata:
-            yield self._create_sqlite_table(table, sqlite_con)
-
-        sqlite_con.execute("VACUUM;")
-
-        sqlite_con.close()
+            sqlite_con.execute("VACUUM;")
+        finally:
+            sqlite_con.close()
 
     def _build_duckdb(self, duckdb_path: Path, metadata: list) -> None:
         duckdb_con: DuckDBPyConnection = duckdb.connect(str(duckdb_path))
+        try:
+            for table in metadata:
+                yield self._create_duckdb_table(table, duckdb_con)
 
-        for table in metadata:
-            yield self._create_duckdb_table(table, duckdb_con)
-
-        duckdb_con.close()
+        finally:
+            duckdb_con.close()
 
     def build(
         self,
-        directory: str | Path,  # The database directory (eg. `./artifacts`)
+        directory: str | Path,
         config: list[dict],
-        upload_bucket: Optional[
-            str
-        ] = None,  # The GCS bucket to upload the db files to (None)
+        upload_bucket: Optional[str] = None,
     ) -> None:
         (
             duckdb_metadata,
             sqlite_metadata,
         ) = self._merge_config_and_dataset_metadata(
             self.source_dataset_metadata, config
         )
+        """
+        Build the In-process duckdb and sqlite databases from a BQ dataset.
+
+        Args:
+            directory: Path to the directory where the database files will be stored
+            config: Configuration for the database.
+            upload_bucket: The GCS bucket to upload the db files to.
+        Yields:
+            _Event: IPDBBuildEvent indicating the progress or completion of the build process.
+        """
 
         yield _Event(
             _EventTypes.SOURCE_DATASET_METADATA_RETRIEVED,
             data={"metadata": None},
         )
 
         pathnames = []
@@ -566,52 +575,60 @@
         app/templates/duckdb/prepare.sql
         app/templates/duckdb/prepare/view1.sql
         app/templates/duckdb/prepare/view2.sql
         """
         env = Template(template_path)
 
         if os.path.exists(f"{template_path}/duckdb/prepare.sql"):
-            duckdb_path = self._prepare_pathnames(db_directory, "main.duck.db")
+            duckdb_path = self._verify_directory_and_pathname(
+                db_directory, "main.duck.db"
+            )
             duckdb_con: DuckDBPyConnection = duckdb.connect(str(duckdb_path))
             files = os.listdir(f"{template_path}/duckdb/prepare")
 
             duckdb_query = env.get("prepare.sql", "duckdb").render(files=files)
-            duckdb_con.execute(duckdb_query)
 
-            r = duckdb_con.execute(
-                "SELECT table_name, table_type FROM information_schema.tables"
-            )
+            try:
+                duckdb_con.execute(duckdb_query)
 
-            yield _Event(
-                _EventTypes.PREPARE_SCRIPTS_COMPLETE,
-                data={
-                    "database": "duckdb",
-                    "tables": yaml.safe_dump(r.arrow().to_pylist(), indent=4),
-                },
-            )
+                r = duckdb_con.execute(
+                    "SELECT table_name, table_type FROM information_schema.tables"
+                )
 
-            duckdb_con.close()
+                yield _Event(
+                    _EventTypes.PREPARE_SCRIPTS_COMPLETE,
+                    data={
+                        "database": "duckdb",
+                        "tables": yaml.safe_dump(r.arrow().to_pylist(), indent=4),
+                    },
+                )
 
-        if os.path.exists(f"{template_path}/sqlite/prepare.sql"):
-            sqlite_path = self._prepare_pathnames(db_directory, "main.sqlite.db")
-            sqlite_con: SQLiteConnection = sqlite3.connect(str(sqlite_path))
-            files = os.listdir(f"{template_path}/sqlite/prepare")
-            sqlite_query = env.get("prepare.sql", "sqlite").render(files=files)
+            finally:
+                duckdb_con.close()
 
-            sqlite_con.executescript(sqlite_query)
-            sqlite_con.commit()
-            r = sqlite_con.execute(
-                "SELECT type, tbl_name FROM sqlite_master WHERE type IN ('table', 'view')"
+        if os.path.exists(f"{template_path}/sqlite/prepare.sql"):
+            sqlite_path = self._verify_directory_and_pathname(
+                db_directory, "main.sqlite.db"
             )
-            rows = r.fetchall()
+            sqlite_con: SQLiteConnection = sqlite3.connect(str(sqlite_path))
+            try:
+                files = os.listdir(f"{template_path}/sqlite/prepare")
+                sqlite_query = env.get("prepare.sql", "sqlite").render(files=files)
 
-            data = [{"table_name": row[1], "table_type": row[0]} for row in rows]
+                sqlite_con.executescript(sqlite_query)
+                sqlite_con.commit()
+                r = sqlite_con.execute(
+                    "SELECT type, tbl_name FROM sqlite_master WHERE type IN ('table', 'view')"
+                )
+                rows = r.fetchall()
 
-            yield _Event(
-                _EventTypes.PREPARE_SCRIPTS_COMPLETE,
-                data={
-                    "database": "sqlite",
-                    "tables": yaml.safe_dump(data, indent=4),
-                },
-            )
+                data = [{"table_name": row[1], "table_type": row[0]} for row in rows]
 
-            sqlite_con.close()
+                yield _Event(
+                    _EventTypes.PREPARE_SCRIPTS_COMPLETE,
+                    data={
+                        "database": "sqlite",
+                        "tables": yaml.safe_dump(data, indent=4),
+                    },
+                )
+            finally:
+                sqlite_con.close()
```

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/template.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         `listify` (or the like), which is below.
 
         ```sql
         {% if values is populated %}
         ```
 
         Will evaluate to `True` where:
-        - `values` is a primative value, or
+        - `values` is a primitive value, or
         - `values` is an iterable with at least one item in it.
         """
         if isinstance(value, (float, int, str)):
             return True
 
         if isinstance(value, Iterable):
             return len(value) > 0
```

### Comparing `neoval_py_utils-0.3.0/src/neoval_py_utils/utils.py` & `neoval_py_utils-0.3.1/src/neoval_py_utils/utils.py`

 * *Files identical despite different names*

