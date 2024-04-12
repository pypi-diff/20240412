# Comparing `tmp/pg_logidater-0.3.1.tar.gz` & `tmp/pg_logidater-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_logidater-0.3.1.tar", max compression
+gzip compressed data, was "pg_logidater-0.3.2.tar", max compression
```

## Comparing `pg_logidater-0.3.1.tar` & `pg_logidater-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.3.1/LICENSE
--rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.3.1/README.md
--rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.3.1/pg_logidater/__init__.py
--rw-r--r--   0        0        0    10163 2024-04-10 18:12:32.925105 pg_logidater-0.3.1/pg_logidater/cli.py
--rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.3.1/pg_logidater/exceptions.py
--rw-r--r--   0        0        0     2220 2024-04-10 18:12:39.811524 pg_logidater-0.3.1/pg_logidater/master.py
--rw-r--r--   0        0        0     1553 2024-04-10 18:12:44.616579 pg_logidater-0.3.1/pg_logidater/replica.py
--rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.3.1/pg_logidater/sqlqueries.py
--rw-r--r--   0        0        0     5611 2024-04-10 18:12:50.406016 pg_logidater-0.3.1/pg_logidater/tartget.py
--rw-r--r--   0        0        0     8987 2024-04-10 18:14:01.144134 pg_logidater-0.3.1/pg_logidater/utils.py
--rw-r--r--   0        0        0      873 2024-04-10 18:35:51.151852 pg_logidater-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pg_logidater-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-05 12:39:35.484273 pg_logidater-0.3.2/LICENSE
+-rw-r--r--   0        0        0      802 2024-04-05 19:02:12.042024 pg_logidater-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-29 08:12:18.901186 pg_logidater-0.3.2/pg_logidater/__init__.py
+-rw-r--r--   0        0        0    10163 2024-04-10 18:12:32.925105 pg_logidater-0.3.2/pg_logidater/cli.py
+-rw-r--r--   0        0        0     1326 2024-04-10 07:00:49.766735 pg_logidater-0.3.2/pg_logidater/exceptions.py
+-rw-r--r--   0        0        0     2220 2024-04-10 18:12:39.811524 pg_logidater-0.3.2/pg_logidater/master.py
+-rw-r--r--   0        0        0     1553 2024-04-10 18:12:44.616579 pg_logidater-0.3.2/pg_logidater/replica.py
+-rw-r--r--   0        0        0     2813 2024-04-10 07:23:02.468326 pg_logidater-0.3.2/pg_logidater/sqlqueries.py
+-rw-r--r--   0        0        0     5570 2024-04-11 19:15:49.271005 pg_logidater-0.3.2/pg_logidater/tartget.py
+-rw-r--r--   0        0        0     8987 2024-04-11 19:26:26.238111 pg_logidater-0.3.2/pg_logidater/utils.py
+-rw-r--r--   0        0        0      871 2024-04-12 06:27:17.544337 pg_logidater-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pg_logidater-0.3.2/PKG-INFO
```

### Comparing `pg_logidater-0.3.1/LICENSE` & `pg_logidater-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/README.md` & `pg_logidater-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/cli.py` & `pg_logidater-0.3.2/pg_logidater/cli.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/exceptions.py` & `pg_logidater-0.3.2/pg_logidater/exceptions.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/master.py` & `pg_logidater-0.3.2/pg_logidater/master.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/replica.py` & `pg_logidater-0.3.2/pg_logidater/replica.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/sqlqueries.py` & `pg_logidater-0.3.2/pg_logidater/sqlqueries.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pg_logidater/tartget.py` & `pg_logidater-0.3.2/pg_logidater/tartget.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from subprocess import Popen, PIPE
 from os import path
 from shutil import disk_usage
 from pg_logidater.exceptions import (
     DatabaseExists,
     DiskSpaceTooLow
 )
-from pycotore.progress import ProgressBar
 from threading import Event
+from pycotore import ProgressBar
 
 PG_DUMP_DB = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -U {user} {db}"
 PG_DUMP_SEQ = "/usr/bin/pg_dump --no-publications --no-subscriptions -h {host} -d {db} -U {user} -t {seq_name}"
 PG_DUMP_ROLES = "/usr/bin/pg_dumpall --roles-only -h {host} -U repmgr"
 PSQL_SQL_RESTORE = "/usr/bin/psql -f {file} -d {db}"
 PSQL_SQL_PIPE_RESTORE = "/usr/bin/psql -d {db}"
 
@@ -88,29 +88,28 @@
     event.set()
 
 
 def db_sync_progress_bar(psql: SqlConn, total: float, event: Event, db: str, update_interval: float) -> None:
     _logger.debug("Startign progress bar function")
     bar = ProgressBar()
     suffix = f"{db} sync in progress"
-    bar.set_suffix(suffix)
-    bar.set_total(total)
+    bar.suffix = suffix
+    bar.total = total
     event.wait(timeout=10)
     _logger.debug("Continue progrss function")
     event.clear()
     while True:
         if event.is_set():
             break
         synced_size = psql.get_db_size(db)
-        bar.update_progress(synced_size)
+        bar.progress = synced_size
         bar.draw()
         event.wait(update_interval)
-    bar.update_progress(total)
+    bar.update_progress = total
     bar.draw()
-    bar.flush_line()
 
 
 def create_subscriber(sub_target: str, database: str, slot_name: str, repl_position: str) -> None:
     psql = SqlConn("/tmp", user="postgres", db=database)
     _logger.info(f"Creating subsriber to {sub_target}")
     sub_id = psql.create_subscriber(
         name=slot_name,
```

### Comparing `pg_logidater-0.3.1/pg_logidater/utils.py` & `pg_logidater-0.3.2/pg_logidater/utils.py`

 * *Files identical despite different names*

### Comparing `pg_logidater-0.3.1/pyproject.toml` & `pg_logidater-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "pg-logidater"
 readme = "README.md"
 authors = ["Arunas Grigalionis <arunas.grigalionis@gmail.com>"]
 description = "Postgresql logical replication setup utility"
-version = "0.0.0a7"
+version = "0.3.1"
 license = "GPL-3.0-only"
 homepage = "https://github.com/niekosau"
 repository = "https://github.com/niekosau/pg-logidater"
 keywords = ["postgres"]
 
 [tool.poetry.scripts]
 pg-logidater = 'pg_logidater.cli:main'
 
 [tool.poetry.dependencies]
 python = "~3.9"
 psycopg2-binary = "^2.9.9"
 paramiko = "^3.4.0"
-pycotore = "^0.1.0"
+pycotore = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 tox = "^4.14.2"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 wheel = "^0.43.0"
```

### Comparing `pg_logidater-0.3.1/PKG-INFO` & `pg_logidater-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pg-logidater
-Version: 0.3.1
+Version: 0.3.2
 Summary: Postgresql logical replication setup utility
 Home-page: https://github.com/niekosau
 License: GPL-3.0-only
 Keywords: postgres
 Author: Arunas Grigalionis
 Author-email: arunas.grigalionis@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: paramiko (>=3.4.0,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
-Requires-Dist: pycotore (>=0.1.0,<0.2.0)
+Requires-Dist: pycotore (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/niekosau/pg-logidater
 Description-Content-Type: text/markdown
 
 pg-logidater
 ============
 > [!CAUTION]
 > Use with yout own risk, not batletested
```

