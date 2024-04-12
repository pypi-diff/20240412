# Comparing `tmp/tulona-0.3.3.tar.gz` & `tmp/tulona-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.3.3.tar", last modified: Thu Apr 11 07:14:51 2024, max compression
+gzip compressed data, was "tulona-0.4.0.tar", last modified: Fri Apr 12 06:52:13 2024, max compression
```

## Comparing `tulona-0.3.3.tar` & `tulona-0.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.898353 tulona-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-11 07:14:47.000000 tulona-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-11 07:14:51.898353 tulona-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-11 07:14:47.000000 tulona-0.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.890353 tulona-0.3.3/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.890353 tulona-0.3.3/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.894353 tulona-0.3.3/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.894353 tulona-0.3.3/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.894353 tulona-0.3.3/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7863 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.894353 tulona-0.3.3/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.894353 tulona-0.3.3/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15829 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.898353 tulona-0.3.3/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 07:14:47.000000 tulona-0.3.3/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:14:51.898353 tulona-0.3.3/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-11 07:14:51.000000 tulona-0.3.3/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-11 07:14:47.000000 tulona-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:14:51.898353 tulona-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-12 06:52:03.000000 tulona-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-12 06:52:13.308987 tulona-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-12 06:52:03.000000 tulona-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.300987 tulona-0.4.0/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.300987 tulona-0.4.0/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.304987 tulona-0.4.0/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15885 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 06:52:03.000000 tulona-0.4.0/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:52:13.308987 tulona-0.4.0/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 06:52:13.000000 tulona-0.4.0/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-12 06:52:03.000000 tulona-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:52:13.308987 tulona-0.4.0/setup.cfg
```

### Comparing `tulona-0.3.3/LICENSE` & `tulona-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/PKG-INFO` & `tulona-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.3.3
+Version: 0.4.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -96,15 +96,15 @@
 
 This is how a `tulona-project.yml` file looks like:
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
-  config-version: 1
+  config_version: 1
 
   outdir: output # the folder comparison result is written into
 
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgres
@@ -120,14 +120,23 @@
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:  # optional
         - phone_number
       compare_column: Employee_ID  # conditional optional
 
+  # List of lists
+  # The inner lists have datasources that need to be used for tasks like comparison
+  # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
+  # Outer list is a list of those combinations.
+  # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
+  source_map:
+    - - employee_postgres
+      - employee_mysql
+
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
@@ -138,14 +147,18 @@
 
     ``tulona ping --datasources employee_postgres``
 
   * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
+  * To ping all the datasources, just skip the `--datasources` parameter:
+
+    ``tulona ping``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
@@ -168,14 +181,26 @@
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+
+From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
+For example this command:
+
+``tulona compare --datasources employee_postgres,employee_mysql``
+
+will become this:
+
+``tulona compare``
+
+Please look at the sample project config from above to understand how to use `source_map` property.
+
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
 
 ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
```

### Comparing `tulona-0.3.3/README.rst` & `tulona-0.4.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 This is how a `tulona-project.yml` file looks like:
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
-  config-version: 1
+  config_version: 1
 
   outdir: output # the folder comparison result is written into
 
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgres
@@ -88,14 +88,23 @@
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:  # optional
         - phone_number
       compare_column: Employee_ID  # conditional optional
 
+  # List of lists
+  # The inner lists have datasources that need to be used for tasks like comparison
+  # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
+  # Outer list is a list of those combinations.
+  # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
+  source_map:
+    - - employee_postgres
+      - employee_mysql
+
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
@@ -106,14 +115,18 @@
 
     ``tulona ping --datasources employee_postgres``
 
   * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
+  * To ping all the datasources, just skip the `--datasources` parameter:
+
+    ``tulona ping``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
@@ -136,14 +149,26 @@
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+
+From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
+For example this command:
+
+``tulona compare --datasources employee_postgres,employee_mysql``
+
+will become this:
+
+``tulona compare``
+
+Please look at the sample project config from above to understand how to use `source_map` property.
+
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
 
 ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
```

### Comparing `tulona-0.3.3/core/tulona/adapter/connection.py` & `tulona-0.4.0/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/adapter/mssql.py` & `tulona-0.4.0/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/adapter/mysql.py` & `tulona-0.4.0/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/adapter/postgres.py` & `tulona-0.4.0/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/adapter/snowflake.py` & `tulona-0.4.0/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/cli/base.py` & `tulona-0.4.0/core/tulona/cli/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,30 +41,28 @@
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 def ping(ctx, **kwargs):
     """Test connectivity to datasources"""
 
-    if not kwargs["datasources"]:
-        raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: ping"
-        )
-
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
 
-    datasource_list = kwargs["datasources"].split(",")
+    if kwargs["datasources"]:
+        datasource_list = kwargs["datasources"].split(",")
+    else:
+        datasource_list = list(ctx.obj["project"]["datasources"].keys())
 
     task = PingTask(
         profile=ctx.obj["profile"],
         project=ctx.obj["project"],
         datasources=datasource_list,
     )
     task.execute()
@@ -77,99 +75,115 @@
 @p.outdir
 @p.verbose
 @p.datasources
 @p.compare
 def profile(ctx, **kwargs):
     """Profile data sources to collect metadata [row count, column min/max/mean etc.]"""
 
-    if not kwargs["datasources"]:
-        raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: profile"
-        )
-
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
-    datasource_list = kwargs["datasources"].split(",")
-
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
-    outfile_fqn = get_outfile_fqn(
-        outdir=ctx.obj["project"]["outdir"],
-        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-        infix="profiling",
-    )
 
-    task = ProfileTask(
-        profile=ctx.obj["profile"],
-        project=ctx.obj["project"],
-        runtime=ctx.obj["runtime"],
-        datasources=datasource_list,
-        outfile_fqn=outfile_fqn,
-        compare=kwargs["compare"],
-    )
-    task.execute()
+    source_maps = []
+    if kwargs["datasources"]:
+        source_maps.append(kwargs["datasources"].split(","))
+    elif "source_map" in ctx.obj["project"]:
+        source_maps = ctx.obj["project"]["source_map"]
+    else:
+        raise TulonaMissingArgumentError(
+            "Either --datasources command line argument or source_map (tulona-project.yml)"
+            " must be provided with command: profile"
+            " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+            " for more information on source_map"
+        )
+
+    for datasource_list in source_maps:
+        outfile_fqn = get_outfile_fqn(
+            outdir=ctx.obj["project"]["outdir"],
+            ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+            infix="profiling",
+        )
+
+        task = ProfileTask(
+            profile=ctx.obj["profile"],
+            project=ctx.obj["project"],
+            runtime=ctx.obj["runtime"],
+            datasources=datasource_list,
+            outfile_fqn=outfile_fqn,
+            compare=kwargs["compare"],
+        )
+        task.execute()
 
 
 # command: tulona compare-data
 @cli.command("compare-data")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
 @p.sample_count
 def compare_data(ctx, **kwargs):
     """Compares two data entities"""
 
-    if not kwargs["datasources"]:
-        raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: compare-data"
-        )
-
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
-    datasource_list = kwargs["datasources"].split(",")
-
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
-    outfile_fqn = get_outfile_fqn(
-        outdir=ctx.obj["project"]["outdir"],
-        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-        infix="data_comparison",
-    )
 
-    task = CompareDataTask(
-        profile=ctx.obj["profile"],
-        project=ctx.obj["project"],
-        runtime=ctx.obj["runtime"],
-        datasources=datasource_list,
-        outfile_fqn=outfile_fqn,
-        sample_count=kwargs["sample_count"],
-    )
-    task.execute()
+    source_maps = []
+    if kwargs["datasources"]:
+        source_maps.append(kwargs["datasources"].split(","))
+    elif "source_map" in ctx.obj["project"]:
+        source_maps = ctx.obj["project"]["source_map"]
+    else:
+        raise TulonaMissingArgumentError(
+            "Either --datasources command line argument or source_map (tulona-project.yml)"
+            " must be provided with command: compare-data"
+            " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+            " for more information on source_map"
+        )
+
+    for datasource_list in source_maps:
+        outfile_fqn = get_outfile_fqn(
+            outdir=ctx.obj["project"]["outdir"],
+            ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+            infix="data_comparison",
+        )
+
+        task = CompareDataTask(
+            profile=ctx.obj["profile"],
+            project=ctx.obj["project"],
+            runtime=ctx.obj["runtime"],
+            datasources=datasource_list,
+            outfile_fqn=outfile_fqn,
+            sample_count=kwargs["sample_count"],
+        )
+        task.execute()
 
 
 # command: tulona compare-column
 @cli.command("compare-column")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
@@ -179,49 +193,57 @@
     """
     Column name must be specified for task: compare-column
     by specifying 'compare_column' property in
     all the datasource[project] configs
     (check sample tulona-project.yml file for example)
     """
 
-    if not kwargs["datasources"]:
-        raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: compare-column"
-        )
-
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
-    datasource_list = kwargs["datasources"].split(",")
-
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
-    outfile_fqn = get_outfile_fqn(
-        outdir=ctx.obj["project"]["outdir"],
-        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-        infix="column_comparison",
-    )
 
-    task = CompareColumnTask(
-        profile=ctx.obj["profile"],
-        project=ctx.obj["project"],
-        runtime=ctx.obj["runtime"],
-        datasources=datasource_list,
-        outfile_fqn=outfile_fqn,
-    )
-    task.execute()
+    source_maps = []
+    if kwargs["datasources"]:
+        source_maps.append(kwargs["datasources"].split(","))
+    elif "source_map" in ctx.obj["project"]:
+        source_maps = ctx.obj["project"]["source_map"]
+    else:
+        raise TulonaMissingArgumentError(
+            "Either --datasources command line argument or source_map (tulona-project.yml)"
+            " must be provided with command: compare-column"
+            " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+            " for more information on source_map"
+        )
+
+    for datasource_list in source_maps:
+        outfile_fqn = get_outfile_fqn(
+            outdir=ctx.obj["project"]["outdir"],
+            ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+            infix="column_comparison",
+        )
+
+        task = CompareColumnTask(
+            profile=ctx.obj["profile"],
+            project=ctx.obj["project"],
+            runtime=ctx.obj["runtime"],
+            datasources=datasource_list,
+            outfile_fqn=outfile_fqn,
+        )
+        task.execute()
 
 
 # command: tulona compare
 @cli.command("compare")
 @click.pass_context
 # @p.exec_engine
 @p.outdir
@@ -229,47 +251,55 @@
 @p.datasources
 @p.sample_count
 def compare(ctx, **kwargs):
     """
     Compare everything(profiles, rows and columns) for the given datasoures
     """
 
-    if not kwargs["datasources"]:
-        raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: compare-column"
-        )
-
     if kwargs["verbose"]:
         logging.getLogger("tulona").setLevel(logging.DEBUG)
 
     prof = Profile()
     proj = Project()
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
     ctx.obj["runtime"] = RunConfig(options=kwargs, project=ctx.obj["project"])
 
-    datasource_list = kwargs["datasources"].split(",")
-
     # Override config outdir if provided in command line
     if kwargs["outdir"]:
         ctx.obj["project"]["outdir"] = kwargs["outdir"]
-    outfile_fqn = get_outfile_fqn(
-        outdir=ctx.obj["project"]["outdir"],
-        ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
-        infix="comparison",
-    )
 
-    task = CompareTask(
-        profile=ctx.obj["profile"],
-        project=ctx.obj["project"],
-        runtime=ctx.obj["runtime"],
-        datasources=datasource_list,
-        outfile_fqn=outfile_fqn,
-        sample_count=kwargs["sample_count"],
-    )
-    task.execute()
+    source_maps = []
+    if kwargs["datasources"]:
+        source_maps.append(kwargs["datasources"].split(","))
+    elif "source_map" in ctx.obj["project"]:
+        source_maps = ctx.obj["project"]["source_map"]
+    else:
+        raise TulonaMissingArgumentError(
+            "Either --datasources command line argument or source_map (tulona-project.yml)"
+            " must be provided with command: compare"
+            " Check https://github.com/mrinalsardar/tulona/tree/main?tab=readme-ov-file#project-config-file"
+            " for more information on source_map"
+        )
+
+    for datasource_list in source_maps:
+        outfile_fqn = get_outfile_fqn(
+            outdir=ctx.obj["project"]["outdir"],
+            ds_list=[ds.split(":")[0].replace("_", "") for ds in datasource_list],
+            infix="comparison",
+        )
+
+        task = CompareTask(
+            profile=ctx.obj["profile"],
+            project=ctx.obj["project"],
+            runtime=ctx.obj["runtime"],
+            datasources=datasource_list,
+            outfile_fqn=outfile_fqn,
+            sample_count=kwargs["sample_count"],
+        )
+        task.execute()
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `tulona-0.3.3/core/tulona/cli/params.py` & `tulona-0.4.0/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/config/profile.py` & `tulona-0.4.0/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/config/project.py` & `tulona-0.4.0/core/tulona/config/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 import logging
 from pathlib import Path
+from typing import Dict, List
+
+from pydantic import BaseModel
 
 from tulona.exceptions import TulonaInvalidProjectConfigError, TulonaProjectException
 from tulona.util.filesystem import path_exists
 from tulona.util.yaml_parser import read_yaml
 
 log = logging.getLogger(__name__)
 
 PROJECT_FILE_NAME = "tulona-project.yml"
 
 
+# TODO: Add datasource model to validation
+class ProjectModel(BaseModel):
+    version: str
+    name: str
+    config_version: int = 1
+    engine: str = "pandas"
+    outdir: str = "output"
+    datasources: Dict
+    source_map: List[List] = list()
+
+
 class Project:
     @property
     def get_project_root(self):
         return Path().absolute()
 
     @property
     def project_conf_path(self) -> str:
         return Path(self.get_project_root, PROJECT_FILE_NAME)
 
-    def validate_project_config(self, project_dict_raw: dict) -> bool:
-        # TODO: implement validations for project config
-        valid = True
-
-        if not valid:
-            raise TulonaInvalidProjectConfigError("Project config is not valid")
+    def validate_project_config(self, project_dict_raw: Dict) -> bool:
+        try:
+            _ = ProjectModel(**project_dict_raw)
+        except TulonaInvalidProjectConfigError as exc:
+            raise TulonaInvalidProjectConfigError(exc)
 
     def load_project_config(self) -> None:
         project_file_uri = self.project_conf_path
         log.debug(f"Attempting to load project config from {project_file_uri}")
 
         if not path_exists(project_file_uri):
             raise TulonaProjectException(
```

### Comparing `tulona-0.3.3/core/tulona/exceptions.py` & `tulona-0.4.0/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/task/base.py` & `tulona-0.4.0/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/task/compare.py` & `tulona-0.4.0/core/tulona/task/compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,17 @@
                 setattr(self, field.name, field.default)
 
     def execute(self):
         log.info("------------------------ Starting task: compare-data")
         start_time = time.time()
 
         if len(self.datasources) != 2:
-            raise ValueError("Comparison needs two data sources.")
+            raise ValueError("Data comparison needs two data sources.")
+
+        log.info(f"Comparing {self.datasources}")
 
         # TODO: Add support of composite primary key
         # TODO: Add support for different names of primary keys in different tables
         # Check if primary key[s] is[are] specified for row comparison
         primary_keys = set()
         ds_names = []
         ds_name_compressed_list = []
```

### Comparing `tulona-0.3.3/core/tulona/task/helper.py` & `tulona-0.4.0/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/task/profile.py` & `tulona-0.4.0/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/task/scan.py` & `tulona-0.4.0/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/database.py` & `tulona-0.4.0/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/dataframe.py` & `tulona-0.4.0/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/excel.py` & `tulona-0.4.0/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/filesystem.py` & `tulona-0.4.0/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/profiles.py` & `tulona-0.4.0/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona/util/sql.py` & `tulona-0.4.0/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/core/tulona.egg-info/PKG-INFO` & `tulona-0.4.0/core/tulona.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.3.3
+Version: 0.4.0
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -96,15 +96,15 @@
 
 This is how a `tulona-project.yml` file looks like:
 
 .. code-block:: yaml
 
   version: '2.0'
   name: integration_project
-  config-version: 1
+  config_version: 1
 
   outdir: output # the folder comparison result is written into
 
   datasources:
     employee_postgres:
       connection_profile: pgdb
       database: postgres
@@ -120,14 +120,23 @@
       schema: db
       table: employee
       primary_key: employee_id
       exclude_columns:  # optional
         - phone_number
       compare_column: Employee_ID  # conditional optional
 
+  # List of lists
+  # The inner lists have datasources that need to be used for tasks like comparison
+  # For example employee_postgres vs employee_mysql. So a [employee_postgres, employee_mysql]
+  # Outer list is a list of those combinations.
+  # So like: [[employee_postgres, employee_mysql], [datasource3, datasource4]]
+  source_map:
+    - - employee_postgres
+      - employee_mysql
+
 
 Features
 --------
 Executing `tulona` or `tulona -h` or `tulona --help` returns available commands.
 All commands take one mandatory parameter, `--datasources`, a comma separated list of names of datasources from project config file (`tulona-project.yml`).
 
 Tulona has following commands available:
@@ -138,14 +147,18 @@
 
     ``tulona ping --datasources employee_postgres``
 
   * More than one datasources can be passed to the `--datasources` parameter separated by commas:
 
     ``tulona ping --datasources employee_postgres,employee_mysql``
 
+  * To ping all the datasources, just skip the `--datasources` parameter:
+
+    ``tulona ping``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
 
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
@@ -168,14 +181,26 @@
 
     ``tulona compare-column --datasources employee_postgres,employee_mysql``
 
 * **compare**: To prepare a comparison report for evrything together. To executed this command just swap the command from any of the above commands with `compare`. It will prepare comparison of everything and write them into different sheets of a single excel file. Sample command:
 
   ``tulona compare --datasources employee_postgres,employee_mysql``
 
+
+From `tulona v0.4.0` a new project config property has been introduced: `source_map`. If this config is set, in the project config file (tulona-project.yml), then `--datasources` parameter can be skipped with commands.
+For example this command:
+
+``tulona compare --datasources employee_postgres,employee_mysql``
+
+will become this:
+
+``tulona compare``
+
+Please look at the sample project config from above to understand how to use `source_map` property.
+
 For debug level log, add `-v` or `--verbose` flag along with any command. For example:
 
 ``tulona ping -v --datasources employee_postgres``
 
 To know more about any specific command, execute `tulona <command> -h`.
```

### Comparing `tulona-0.3.3/core/tulona.egg-info/SOURCES.txt` & `tulona-0.4.0/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.3.3/pyproject.toml` & `tulona-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.3.3"
+version = "0.4.0"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -110,27 +110,27 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.3.3"
+current_version = "0.4.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
-commit = true
+commit = false
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 
 [[tool.bumpversion.files]]
```

