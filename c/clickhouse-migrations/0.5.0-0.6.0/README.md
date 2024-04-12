# Comparing `tmp/clickhouse-migrations-0.5.0.tar.gz` & `tmp/clickhouse-migrations-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-migrations-0.5.0.tar", last modified: Thu Jan  4 22:11:03 2024, max compression
+gzip compressed data, was "clickhouse-migrations-0.6.0.tar", last modified: Fri Apr 12 08:32:33 2024, max compression
```

## Comparing `clickhouse-migrations-0.5.0.tar` & `clickhouse-migrations-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 22:11:03.274600 clickhouse-migrations-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-01-04 22:11:03.274600 clickhouse-migrations-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 22:11:03.274600 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-04 22:11:03.000000 clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 22:11:03.274600 clickhouse-migrations-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 22:11:03.270600 clickhouse-migrations-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 22:11:03.274600 clickhouse-migrations-0.5.0/src/clickhouse_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/clickhouse_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/migrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-04 22:10:43.000000 clickhouse-migrations-0.5.0/src/clickhouse_migrations/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:32:33.048935 clickhouse-migrations-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-12 08:32:33.048935 clickhouse-migrations-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:32:33.048935 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 08:32:33.000000 clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:32:33.052935 clickhouse-migrations-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:32:33.044935 clickhouse-migrations-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:32:33.048935 clickhouse-migrations-0.6.0/src/clickhouse_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/clickhouse_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/migrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 08:32:19.000000 clickhouse-migrations-0.6.0/src/clickhouse_migrations/types.py
```

### Comparing `clickhouse-migrations-0.5.0/LICENSE` & `clickhouse-migrations-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/PKG-INFO` & `clickhouse-migrations-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-migrations
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple file-based migrations for clickhouse
 Author-email: Aleh Strakachuk <zifter.ai+clickhouse.migrations@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zifter/clickhouse-migrations
 Project-URL: Source, https://github.com/zifter/clickhouse-migrations
 Project-URL: Tracker, https://github.com/zifter/clickhouse-migrations/issues
 Keywords: clickhouse,migrations
```

### Comparing `clickhouse-migrations-0.5.0/README.md` & `clickhouse-migrations-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/PKG-INFO` & `clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-migrations
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple file-based migrations for clickhouse
 Author-email: Aleh Strakachuk <zifter.ai+clickhouse.migrations@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/zifter/clickhouse-migrations
 Project-URL: Source, https://github.com/zifter/clickhouse-migrations
 Project-URL: Tracker, https://github.com/zifter/clickhouse-migrations/issues
 Keywords: clickhouse,migrations
```

### Comparing `clickhouse-migrations-0.5.0/clickhouse_migrations.egg-info/SOURCES.txt` & `clickhouse-migrations-0.6.0/clickhouse_migrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/pyproject.toml` & `clickhouse-migrations-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/src/clickhouse_migrations/clickhouse_cluster.py` & `clickhouse-migrations-0.6.0/src/clickhouse_migrations/clickhouse_cluster.py`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/src/clickhouse_migrations/cmd.py` & `clickhouse-migrations-0.6.0/src/clickhouse_migrations/cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,26 +87,33 @@
     )
     parser.add_argument(
         "--dry-run",
         default=os.environ.get("DRY_RUN", "0"),
         type=bool,
         help="Dry run mode",
     )
+    parser.add_argument(
+        "--secure",
+        default=os.environ.get("SECURE", "0"),
+        type=bool,
+        help="Secure connection",
+    )
 
     return parser.parse_args(args)
 
 
 def migrate(ctx) -> int:
     logging.basicConfig(level=ctx.log_level, style="{", format="{levelname}:{message}")
 
     cluster = ClickhouseCluster(
         ctx.db_host,
         db_port=ctx.db_port,
         db_user=ctx.db_user,
         db_password=ctx.db_password,
+        secure=ctx.secure,
     )
     cluster.migrate(
         db_name=ctx.db_name,
         migration_path=ctx.migrations_dir,
         cluster_name=ctx.cluster_name,
         multi_statement=ctx.multi_statement,
         dryrun=ctx.dry_run,
```

### Comparing `clickhouse-migrations-0.5.0/src/clickhouse_migrations/migrator.py` & `clickhouse-migrations-0.6.0/src/clickhouse_migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `clickhouse-migrations-0.5.0/src/clickhouse_migrations/types.py` & `clickhouse-migrations-0.6.0/src/clickhouse_migrations/types.py`

 * *Files identical despite different names*

