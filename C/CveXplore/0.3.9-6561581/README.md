# Comparing `tmp/CveXplore-0.3.9.tar.gz` & `tmp/CveXplore-6561581.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CveXplore-0.3.9.tar", last modified: Tue Oct 17 15:27:06 2023, max compression
+gzip compressed data, was "CveXplore-6561581.tar", last modified: Fri Apr 12 13:37:52 2024, max compression
```

## Comparing `CveXplore-0.3.9.tar` & `CveXplore-6561581.tar`

### file list

```diff
@@ -1,108 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.265117 CveXplore-0.3.9/CveXplore/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/.schema_version
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/api_base_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/connection/api_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/helpers/cve_search_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/api/nvd_nist/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/nvd_nist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/api/nvd_nist/nvd_nist_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.269117 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/find_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/mutex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/cli_cmds/stats_cmds/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/cpe_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/data_source_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/db_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/common/db_obj_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/connection/mongo_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.273117 CveXplore-0.3.9/CveXplore/database/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/cpe_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/cvesearch_mongo_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/generic_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/helpers/specific_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/database/maintenance/
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/DatabaseSchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/DownloadHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/IJSONHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/LogHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    52189 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/Sources_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/Toolkit.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/api_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/content_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/db_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5567 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/main_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/database/maintenance/worker_q.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/errors/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/errors/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13204 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.277118 CveXplore-0.3.9/CveXplore/objects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/capec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cpe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cves.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cvexplore_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/cwe.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-17 15:26:55.000000 CveXplore-0.3.9/CveXplore/objects/via4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 15:27:06.265117 CveXplore-0.3.9/CveXplore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-17 15:27:06.000000 CveXplore-0.3.9/CveXplore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35121 2023-10-17 15:26:55.000000 CveXplore-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-17 15:26:55.000000 CveXplore-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16347 2023-10-17 15:27:06.277118 CveXplore-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15684 2023-10-17 15:26:55.000000 CveXplore-0.3.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-17 15:26:55.000000 CveXplore-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 15:27:06.277118 CveXplore-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-10-17 15:26:55.000000 CveXplore-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.194304 CveXplore-6561581/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.170304 CveXplore-6561581/CveXplore/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/.schema_version
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 13:37:51.000000 CveXplore-6561581/CveXplore/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/alembic/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic/versions/53df0e286532_first_2_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic/versions/ecb1788b7e08_initial_full_model_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/api/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/api/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/api/connection/api_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/api/helpers/cve_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/cli_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/cli_cmds/capec_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/capec_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/capec_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/cli_cmds/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cli_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/cli_cmds/cpe_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cpe_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cpe_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.174304 CveXplore-6561581/CveXplore/cli_cmds/cve_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cve_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cve_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/cli_cmds/cwe_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cwe_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/cwe_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/cli_cmds/db_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/db_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/db_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/cli_cmds/find_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/find_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/find_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/cli_cmds/mutex_options/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/mutex_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/mutex_options/mutex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/cli_cmds/stats_cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/stats_cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/cli_cmds/stats_cmds/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/.env_example
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/.sources.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/cpe_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/data_source_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/db_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/common/db_obj_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/api_base_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.178304 CveXplore-6561581/CveXplore/core/database_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_actions/db_action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/database_indexer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_indexer/db_indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/database_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/api_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15750 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/content_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/download_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/ijson_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/main_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42306 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/sources_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_maintenance/update_base_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/database_migration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_migration/database_migrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/database_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/database_version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/database_version/db_version_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/general/datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/general/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.182304 CveXplore-6561581/CveXplore/core/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/core/logging/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/formatters/task_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/core/logging/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/handlers/cve_explore_rfh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/handlers/cve_explore_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/handlers/gelf_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/handlers/syslog_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/logging/logger_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/core/nvd_nist/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/nvd_nist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18644 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/nvd_nist/nvd_nist_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/core/worker_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/worker_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/core/worker_queue/worker_q.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/database/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/database/connection/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/base/db_connection_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/database_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/database/connection/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/dummy/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.186304 CveXplore-6561581/CveXplore/database/connection/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/mongodb/mongo_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.190304 CveXplore-6561581/CveXplore/database/connection/sqlbase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/sqlbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/sqlbase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/connection/sqlbase/sql_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.190304 CveXplore-6561581/CveXplore/database/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/cpe_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/cvesearch_mongo_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/generic_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/specific_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/database/helpers/specific_db.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.190304 CveXplore-6561581/CveXplore/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/errors/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/errors/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/errors/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/errors/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.190304 CveXplore-6561581/CveXplore/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/capec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/cpe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/cves.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/cvexplore_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/cwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 13:37:38.000000 CveXplore-6561581/CveXplore/objects/via4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:37:52.190304 CveXplore-6561581/CveXplore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 13:37:52.000000 CveXplore-6561581/CveXplore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-04-12 13:37:38.000000 CveXplore-6561581/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 13:37:38.000000 CveXplore-6561581/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-04-12 13:37:52.194304 CveXplore-6561581/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16296 2024-04-12 13:37:38.000000 CveXplore-6561581/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 13:37:38.000000 CveXplore-6561581/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:37:52.194304 CveXplore-6561581/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-12 13:37:38.000000 CveXplore-6561581/setup.py
```

### Comparing `CveXplore-0.3.9/CveXplore/LICENSE` & `CveXplore-6561581/CveXplore/LICENSE`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.9/CveXplore/api/api_base_class.py` & `CveXplore-6561581/CveXplore/core/api_base_class.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.9/CveXplore/api/connection/api_db.py` & `CveXplore-6561581/CveXplore/api/connection/api_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 API connection
 ==============
 """
+
 from CveXplore.api.helpers.cve_search_api import CveSearchApi
 from CveXplore.common.db_mapping import database_mapping
 
 
 class ApiDatabaseSource(object):
     """
     The ApiDatabaseSource mimics the behaviour of the MongoDBConnection.
@@ -25,15 +26,15 @@
         self.database_mapping = database_mapping
 
         self.baseurl = baseurl
 
         for each in self.database_mapping:
             setattr(
                 self,
-                "store_{}".format(each),
+                f"store_{each}",
                 ApiDatabaseCollection(
                     baseurl=baseurl,
                     api_path=api_path,
                     proxies=proxies,
                     user_agent=user_agent,
                     collname=each,
                 ),
```

### Comparing `CveXplore-0.3.9/CveXplore/api/helpers/cve_search_api.py` & `CveXplore-6561581/CveXplore/api/helpers/cve_search_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Cve Search API
 ==============
 """
+
 import pymongo
 
-from CveXplore.api.api_base_class import ApiBaseClass
+from CveXplore.core.api_base_class import ApiBaseClass
 
 
 class CveSearchApi(ApiBaseClass):
     """
     The CveSearchApi handles the different arguments in order to perform a query to a specific Cve Search api endpoint.
     It mimics the pymongo cursor's behaviour to provide an ambiguous way to talk to either an API or a mongodb.
     """
@@ -50,17 +51,15 @@
         self.__skip = skip
         self.__sort = sort
 
         self.data_queue = None
 
     def __repr__(self):
         """return a string representation of the obj GenericApi"""
-        return "<<CveSearchApi:({}, {})>>".format(
-            self.db_collection.address[0], self.db_collection.address[1]
-        )
+        return f"<<CveSearchApi:({self.db_collection.address[0]}, {self.db_collection.address[1]})>>"
 
     def query(self):
         """
         Endpoint for free query to cve search data
         """
 
         results = self.call(method="POST", resource="query", data=self.__data)
```

### Comparing `CveXplore-0.3.9/CveXplore/api/nvd_nist/nvd_nist_api.py` & `CveXplore-6561581/CveXplore/core/nvd_nist/nvd_nist_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,67 @@
 import asyncio
 import json
 import logging
 import math
 import random
 import time
+import uuid
 from collections import namedtuple
 from datetime import datetime, timedelta
 from json import JSONDecodeError
 from urllib.parse import urlencode
 
 import aiohttp as aiohttp
 import requests
 from aiohttp import ContentTypeError
 from aioretry import retry, RetryPolicyStrategy, RetryInfo
 from requests import Response
+from requests.adapters import HTTPAdapter, Retry
 
-from CveXplore.api.api_base_class import ApiBaseClass
 from CveXplore.common.config import Configuration
-from CveXplore.database.maintenance.LogHandler import UpdateHandler
+from CveXplore.core.api_base_class import ApiBaseClass
+from CveXplore.core.database_maintenance.update_base_class import UpdateBaseClass
+from CveXplore.core.logging.logger_class import AppLogger
 from CveXplore.errors.apis import (
     ApiErrorException,
     ApiDataError,
     ApiDataRetrievalFailed,
+    ApiMaxRetryError,
 )
 
-logging.setLoggerClass(UpdateHandler)
+logging.setLoggerClass(AppLogger)
 
 
-class NvdNistApi(ApiBaseClass):
+class NvdNistApi(ApiBaseClass, UpdateBaseClass):
     def __init__(
         self,
         baseurl: str = "https://services.nvd.nist.gov",
         api_path: str = "2.0",
+        proxies: dict = None,
         user_agent: str = "CveXplore",
     ):
-        super().__init__(baseurl, api_path=api_path, user_agent=user_agent)
-
-        self.config = Configuration()
+        ApiBaseClass.__init__(
+            self,
+            baseurl=baseurl,
+            api_path=api_path,
+            user_agent=user_agent,
+            proxies=proxies,
+        )
 
-        self.logger = logging.getLogger("NvdNistApi")
+        UpdateBaseClass.__init__(self, logger_name=__name__)
 
         if self.config.NVD_NIST_API_KEY is not None:
             self.api_key = self.config.NVD_NIST_API_KEY
             self.set_header_field("apiKey", self.api_key)
             self.api_key_limit = False
+            self.logger.info("NVD NIST API Key found!")
         else:
             self.logger.warning(
-                "Could not find a NIST API Key in the '~/.cvexplore/.env' file; "
+                "Could not find a NIST API Key in the environment variable 'NVD_NIST_API_KEY' "
+                "(e.g. from the '~/.cvexplore/.env' file); "
                 "you could request one at: https://nvd.nist.gov/developers/request-an-api-key"
             )
             self.api_key_limit = True
 
         self.filter_rejected = False
 
         if self.config.NVD_NIST_NO_REJECTED:
@@ -113,20 +124,29 @@
                     if return_response_object:
                         return r
                     if r.status_code >= 400:
                         the_response = json.loads(r.text)
                         raise requests.exceptions.ConnectionError(the_response)
                     else:
                         the_response = json.loads(r.text)
+                else:
+                    the_response = r
+
             except JSONDecodeError:
-                if r.headers["content-type"] == "text/plain":
-                    the_response = r.text
+                if "content-type" in r.headers:
+                    if r.headers["content-type"] == "text/plain":
+                        the_response = r.text
+                    else:
+                        the_response = r
                 else:
                     the_response = r
 
+            except Exception:
+                the_response = r
+
             return the_response
 
         except requests.exceptions.ConnectionError as err:
             raise requests.exceptions.ConnectionError(err)
         except Exception as err:
             raise Exception(err)
 
@@ -166,14 +186,53 @@
             )
 
         resource["lastModStartDate"] = last_mod_start_date.isoformat()
         resource["lastModEndDate"] = last_mod_end_date.isoformat()
 
         return resource
 
+    def get_session(
+        self,
+        retries: int = 10,
+        backoff_factor: float = 3,
+        backoff_max: float = 30,
+        status_forcelist: tuple = (403, 429, 500, 502, 503, 504),
+        session=None,
+    ) -> requests.Session:
+        """
+        Method for returning a session object per every requesting thread
+        """
+        session = session or requests.Session()
+        try:
+            retry = Retry(
+                total=retries,
+                read=retries,
+                connect=retries,
+                backoff_factor=backoff_factor,
+                backoff_max=backoff_max,
+                status_forcelist=status_forcelist,
+            )
+        except TypeError:
+            self.logger.info(
+                f"urllib3.util.retry did not support configurable backoff_max; "
+                f"falling back to default for urllib3 1.x compatibility"
+            )
+            retry = Retry(
+                total=retries,
+                read=retries,
+                connect=retries,
+                backoff_factor=backoff_factor,
+                status_forcelist=status_forcelist,
+            )
+        adapter = HTTPAdapter(max_retries=retry)
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+
+        return session
+
     def get_count(
         self,
         datasource: int = 1,
         last_mod_start_date: datetime = None,
         last_mod_end_date: datetime = None,
     ):
         resource = {"resultsPerPage": 1}
@@ -181,20 +240,25 @@
         if last_mod_start_date is not None and last_mod_end_date is not None:
             resource = self.check_date_range(
                 resource=resource,
                 last_mod_start_date=last_mod_start_date,
                 last_mod_end_date=last_mod_end_date,
             )
 
-        ret_data = self.call(self.methods.GET, resource=resource, data=datasource)
+        self.logger.debug(f"Getting count for datasource: {datasource}")
 
-        if not isinstance(ret_data, Response):
-            return ret_data["totalResults"]
-        else:
-            raise ApiDataRetrievalFailed
+        try:
+            ret_data = self.call(self.methods.GET, resource=resource, data=datasource)
+
+            if not isinstance(ret_data, Response):
+                return ret_data["totalResults"]
+            else:
+                raise ApiDataRetrievalFailed(resource)
+        except Exception:
+            raise ApiMaxRetryError
 
     def get_all_data(
         self,
         data_type: str,
         last_mod_start_date: datetime = None,
         last_mod_end_date: datetime = None,
     ):
@@ -206,19 +270,23 @@
                 resource=resource,
                 last_mod_start_date=last_mod_start_date,
                 last_mod_end_date=last_mod_end_date,
             )
         else:
             self.logger.debug(f"Getting all {data_type}s...")
 
-        data = self.get_count(
-            getattr(self.datasource, data_type.upper()),
-            last_mod_start_date=last_mod_start_date,
-            last_mod_end_date=last_mod_end_date,
-        )
+        try:
+            data = self.get_count(
+                getattr(self.datasource, data_type.upper()),
+                last_mod_start_date=last_mod_start_date,
+                last_mod_end_date=last_mod_end_date,
+            )
+        except ApiMaxRetryError:
+            # failed to get the count; set data to 0 and continue
+            data = 0
 
         if isinstance(data, int):
             for each_data in ApiData(
                 results_per_page=getattr(self.max_page_length, data_type.upper()),
                 start_index=0,
                 total_results=data,
                 api_handle=self,
@@ -252,48 +320,51 @@
 
 
 def retry_policy(info: RetryInfo) -> RetryPolicyStrategy:
     """
     - It will always retry until succeeded
     - If fails for the first time, it will retry immediately,
     - If it fails again,
-      aioretry will perform a 100ms delay before the second retry,
-      200ms delay before the 3rd retry,
-      the 4th retry immediately,
-      100ms delay before the 5th retry,
-      etc...
+
+    aioretry will perform a 100ms delay before the second retry,
+    200ms delay before the 3rd retry,
+    the 4th retry immediately,
+    100ms delay before the 5th retry,
+    etc...
     """
-    max_retries = 5
-    backoff_in_ms = 0.2 * 2**info.fails + random.uniform(0, 1) * 4
-    logger = logging.getLogger("RetryPolicy")
+    max_retries = 10
+    backoff_in_s = 0.6 * 2**info.fails + random.uniform(0, 1) * 4
+    logger = logging.getLogger(__name__)
 
     if info.fails != max_retries:
-        logger.debug(f"Current backoff: {backoff_in_ms}")
-
-        logger.debug(f"Retrying {info.fails + 1}/{max_retries}")
-
-        return False, backoff_in_ms
-
+        logger.debug(
+            f"Current backoff: {backoff_in_s}; Retrying {info.fails + 1}/{max_retries}"
+        )
+        return False, backoff_in_s
     else:
         return True, 0
 
 
 class ApiDataIterator(object):
     def __init__(self, api_data: ApiData):
-        self.logger = logging.getLogger("ApiDataIterator")
+        self.logger = logging.getLogger(__name__)
+        self.config = Configuration
 
         self._page_length = api_data.results_per_page
         self._total_results = api_data.total_results
         self._current_index = api_data.start_index
         self.api_data = api_data
 
-        self.sem_factor = 6
+        if self.config.DOWNLOAD_SEM_FACTOR != 0.0:
+            self.sem_factor = self.config.DOWNLOAD_SEM_FACTOR
+        else:
+            self.sem_factor = 6
 
-        if not self.api_data.api_handle.api_key_limit:
-            self.sem_factor = 0.6
+            if not self.api_data.api_handle.api_key_limit:
+                self.sem_factor = 0.6
 
         self.logger.debug(f"Using sem factor: {self.sem_factor}")
 
         self.first_iteration = True
 
         self.last_stop_time = 0
 
@@ -319,18 +390,28 @@
                     )
                     time.sleep(36 - sleep_time)
 
             self.logger.debug(f"Starting download run...")
 
             self.workload = []
 
-            if self.api_data.api_handle.api_key_limit:
-                batch_range = 5
+            if self.config.DOWNLOAD_BATCH_RANGE is None:
+                if self.api_data.api_handle.api_key_limit:
+                    batch_range = 5
+                else:
+                    batch_range = 45
             else:
-                batch_range = 45
+                try:
+                    batch_range = int(self.config.DOWNLOAD_BATCH_RANGE)
+                except ValueError:
+                    self.logger.error(
+                        f"Invalid value for DOWNLOAD_BATCH_RANGE, {self.config.DOWNLOAD_BATCH_RANGE} "
+                        f"cannot be converted into an integer..."
+                    )
+                    raise
 
             for i in range(batch_range):
                 if not self.first_iteration:
                     new_start_index = self._current_index + self._page_length
                 else:
                     new_start_index = self._current_index
                     self.first_iteration = False
@@ -363,17 +444,20 @@
         asyncio.set_event_loop(loop)
         results = loop.run_until_complete(self.fetch_all(loop))
 
         return results
 
     @retry(retry_policy)
     async def fetch(self, session: aiohttp.ClientSession, url: str):
+        request_id = uuid.uuid4()
         try:
-            async with session.get(url) as response:
-                self.logger.debug(f"Sending request to url: {url}")
+            async with session.get(
+                url, proxy=self.config.HTTP_PROXY_STRING
+            ) as response:
+                self.logger.debug(f"[{request_id}] Sending request to url: {url}")
                 if response.status == 200:
                     data = await response.json()
                     if "format" in data:
                         if data["format"] == "NVD_CPE":
                             if "products" not in data:
                                 self.logger.debug(
                                     f"Data received does not contain a products list; raise error to retry!"
@@ -404,16 +488,23 @@
                         self.logger.debug(f"Request forbidden by administrative rules")
                     raise ApiDataRetrievalFailed(url)
         except ApiDataError:
             raise
         except ContentTypeError:
             return ApiDataRetrievalFailed(url)
         finally:
-            self.logger.debug(f"Finished request to url: {url}")
-            time.sleep(self.sem_factor / 2)
+            random_sleep = round(
+                random.SystemRandom().uniform(
+                    self.config.DOWNLOAD_SLEEP_MIN, self.config.DOWNLOAD_SLEEP_MAX
+                ),
+                1,
+            )
+            self.logger.debug(f"[{request_id}] Sleeping for {random_sleep} secs...")
+            await asyncio.sleep(random_sleep)
+            self.logger.debug(f"[{request_id}] Finished request")
 
     async def fetch_all(self, loop):
         sem = asyncio.Semaphore(math.ceil(30 / self.sem_factor))
         async with sem:
             async with aiohttp.ClientSession(
                 loop=loop,
                 headers=self.api_data.api_handle.headers,
```

### Comparing `CveXplore-0.3.9/CveXplore/cli.py` & `CveXplore-6561581/CveXplore/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 
 import click
 import click_completion.core
 
 from CveXplore.cli_cmds.capec_cmds import commands as group6
-from CveXplore.cli_cmds.cwe_cmds import commands as group7
 from CveXplore.cli_cmds.cpe_cmds import commands as group5
 from CveXplore.cli_cmds.cve_cmds import commands as group2
+from CveXplore.cli_cmds.cwe_cmds import commands as group7
 from CveXplore.cli_cmds.db_cmds import commands as group4
 from CveXplore.cli_cmds.find_cmds import commands as group1
 from CveXplore.cli_cmds.stats_cmds import commands as group3
 from CveXplore.main import CveXplore
 
 click_completion.init()
 
@@ -25,14 +25,14 @@
     if version:
         click.echo(ctx.obj["data_source"].version)
         exit(0)
     if ctx.invoked_subcommand is None:
         click.echo(main.get_help(ctx))
 
 
-main.add_command(group1.search_cmd)
+main.add_command(group1.find_cmd)
 main.add_command(group2.cve_cmd)
 main.add_command(group3.stats_cmd)
 main.add_command(group4.db_cmd)
 main.add_command(group5.cpe_cmd)
 main.add_command(group6.capec_cmd)
 main.add_command(group7.cwe_cmd)
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/capec_cmds/commands.py` & `CveXplore-6561581/CveXplore/cli_cmds/cwe_cmds/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 import click
 
 from CveXplore.cli_cmds.cli_utils.utils import printer
 from CveXplore.cli_cmds.mutex_options.mutex import Mutex
 
 
-@click.group("capec", invoke_without_command=True, help="Query for capec specific data")
+@click.group("cwe", invoke_without_command=True, help="Query for cwe specific data")
 @click.pass_context
-def capec_cmd(ctx):
+def cwe_cmd(ctx):
     if ctx.invoked_subcommand is None:
-        click.echo(capec_cmd.get_help(ctx))
+        click.echo(cwe_cmd.get_help(ctx))
 
 
-@capec_cmd.group(
+@cwe_cmd.group(
     "search",
     invoke_without_command=True,
-    help="Search for capec entries by id",
+    help="Search for cwe entries by id",
 )
 @click.option(
     "-c",
-    "--capec",
-    help="Search for CAPEC's (could be multiple)",
+    "--cwe",
+    help="Search for CWE's (could be multiple)",
     multiple=True,
-    cls=Mutex,
-    not_required_if=["field_list"],
 )
 @click.option(
     "-f",
     "--field",
     help="Field to return (could be multiple)",
     multiple=True,
     cls=Mutex,
     not_required_if=["field_list"],
 )
 @click.option(
     "-fl",
     "--field_list",
     help="Return a field list for this collection",
-    multiple=True,
     is_flag=True,
     cls=Mutex,
-    not_required_if=["field", "capec"],
+    not_required_if=["field"],
 )
 @click.option(
     "-o",
     "--output",
     default="json",
     help="Set the desired output format (defaults to json)",
     type=click.Choice(["json", "csv", "xml", "html"], case_sensitive=False),
 )
 @click.pass_context
 def search_cmd(
     ctx,
-    capec,
+    cwe,
     field,
     field_list,
     output,
 ):
-    if capec:
-        ret_list = getattr(ctx.obj["data_source"], "capec").mget_by_id(*capec)
-    elif field_list:
-        ret_list = getattr(ctx.obj["data_source"], "capec").field_list()
+    if cwe and not field_list:
+        ret_list = getattr(ctx.obj["data_source"], "cwe").mget_by_id(*cwe)
+    elif cwe and field_list:
+        ret_list = getattr(ctx.obj["data_source"], "cwe").field_list(*cwe)
     else:
         click.echo(search_cmd.get_help(ctx))
         return
 
-    if isinstance(ret_list, list):
+    if isinstance(ret_list, list) and not field_list:
         result = [result.to_dict(*field) for result in ret_list]
-    elif isinstance(ret_list, set):
-        result = sorted([result for result in ret_list])
+    elif field_list:
+        result = [result for result in ret_list]
     else:
         result = []
 
     if ctx.invoked_subcommand is None:
         printer(input_data=result, output=output)
     else:
         ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/cli_utils/utils.py` & `CveXplore-6561581/CveXplore/cli_cmds/cli_utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         df = pd.DataFrame(input_list)
         output = df.to_html(index=False)
     elif format_type == "xml":
         if isinstance(input_list, list):
             count = 1
             temp_dict = defaultdict(dict)
             for each in input_list:
-                temp_dict["entry_{}".format(count)] = each
+                temp_dict[f"entry_{count}"] = each
                 count += 1
             output = dicttoxml(temp_dict, custom_root="CveXplore")
         elif isinstance(input_list, dict):
             output = dicttoxml(input_list, custom_root="CveXplore")
 
     return output
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/cpe_cmds/commands.py` & `CveXplore-6561581/CveXplore/cli_cmds/cpe_cmds/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,32 +46,31 @@
 )
 @click.option(
     "-c",
     "--cpe",
     help="Search for CPE's (could be multiple) by id",
     multiple=True,
     cls=Mutex,
-    not_required_if=["field_list", "name", "title", "vendor"],
+    not_required_if=["name", "title", "vendor"],
 )
 @click.option(
     "-f",
     "--field",
     help="Field to return (could be multiple)",
     multiple=True,
     cls=Mutex,
     not_required_if=["field_list", "name", "title", "vendor"],
 )
 @click.option(
     "-fl",
     "--field_list",
     help="Return a field list for this collection",
-    multiple=True,
     is_flag=True,
     cls=Mutex,
-    not_required_if=["field", "cpe", "name", "title", "vendor"],
+    not_required_if=["field", "name", "title", "vendor"],
 )
 @click.option(
     "-m",
     "--match",
     help="Use match for searching",
     cls=Mutex,
     not_required_if=["regex"],
@@ -80,21 +79,21 @@
     "-r",
     "--regex",
     help="Use regex for searching",
     cls=Mutex,
     not_required_if=["match"],
 )
 @click.option("-d", "--deprecated", is_flag=True, help="Filter deprecated cpe's")
-@click.option("-c", "--cve", is_flag=True, help="Add related CVE's")
+@click.option("-rc", "--related_cve", is_flag=True, help="Add related CVE's")
 @click.option(
     "-p",
     "--product_search",
     default=False,
     is_flag=True,
-    help="If adding CVE's search for vulnerable products and not for vulnerable configurations",
+    help="Let CveXplore search for vulnerable products and not for vulnerable configurations",
 )
 @click.option("-l", "--limit", default=10, help="Search limit")
 @click.option("-s", "--sort", is_flag=True, help="Sort DESCENDING")
 @click.option(
     "-o",
     "--output",
     default="json",
@@ -109,15 +108,15 @@
     vendor,
     cpe,
     field,
     field_list,
     match,
     regex,
     deprecated,
-    cve,
+    related_cve,
     product_search,
     limit,
     sort,
     output,
 ):
     if not name and not vendor and title:
         search_by = "title"
@@ -151,28 +150,28 @@
         else:
             ret_list = (
                 getattr(getattr(ctx.obj["data_source"], "cpe"), search_by)
                 .find(match)
                 .limit(limit)
                 .sort(search_by, sorting)
             )
-    elif cpe:
+    elif cpe and not field_list:
         ret_list = getattr(ctx.obj["data_source"], "cpe").mget_by_id(*cpe)
-    elif field_list:
-        ret_list = getattr(ctx.obj["data_source"], "cpe").field_list()
+    elif cpe and field_list:
+        ret_list = getattr(ctx.obj["data_source"], "cpe").field_list(*cpe)
     else:
         click.echo(search_cmd.get_help(ctx))
         return
 
-    if cve:
+    if related_cve:
         result = [result.to_cve_summary(product_search) for result in ret_list]
-    elif cpe:
+    elif cpe and not field_list:
         result = [result.to_dict(*field) for result in ret_list]
-    elif isinstance(ret_list, set):
-        result = sorted([result for result in ret_list])
+    elif field_list:
+        result = [result for result in ret_list]
     else:
         result = [result.to_dict() for result in ret_list]
 
     if ctx.invoked_subcommand is None:
         printer(input_data=result, output=output)
     else:
         ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/cve_cmds/commands.py` & `CveXplore-6561581/CveXplore/cli_cmds/cve_cmds/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,33 +17,30 @@
     help="Search for cve entries by id",
 )
 @click.option(
     "-c",
     "--cve",
     help="Search for CVE's (could be multiple)",
     multiple=True,
-    cls=Mutex,
-    not_required_if=["field_list"],
 )
 @click.option(
     "-f",
     "--field",
     help="Field to return (could be multiple)",
     multiple=True,
     cls=Mutex,
     not_required_if=["field_list"],
 )
 @click.option(
     "-fl",
     "--field_list",
     help="Return a field list for this collection",
-    multiple=True,
     is_flag=True,
     cls=Mutex,
-    not_required_if=["field", "cve"],
+    not_required_if=["field"],
 )
 @click.option(
     "-o",
     "--output",
     default="json",
     help="Set the desired output format (defaults to json)",
     type=click.Choice(["json", "csv", "xml", "html"], case_sensitive=False),
@@ -52,26 +49,26 @@
 def search_cmd(
     ctx,
     cve,
     field,
     field_list,
     output,
 ):
-    if cve:
+    if cve and not field_list:
         ret_list = getattr(ctx.obj["data_source"], "cves").mget_by_id(*cve)
-    elif field_list:
-        ret_list = getattr(ctx.obj["data_source"], "cves").field_list()
+    elif cve and field_list:
+        ret_list = getattr(ctx.obj["data_source"], "cves").field_list(*cve)
     else:
         click.echo(search_cmd.get_help(ctx))
         return
 
-    if isinstance(ret_list, list):
+    if isinstance(ret_list, list) and not field_list:
         result = [result.to_dict(*field) for result in ret_list]
-    elif isinstance(ret_list, set):
-        result = sorted([result for result in ret_list])
+    elif field_list:
+        result = [result for result in ret_list]
     else:
         result = []
 
     if ctx.invoked_subcommand is None:
         printer(input_data=result, output=output)
     else:
         ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/cwe_cmds/commands.py` & `CveXplore-6561581/CveXplore/cli_cmds/capec_cmds/commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,74 @@
 import click
 
 from CveXplore.cli_cmds.cli_utils.utils import printer
 from CveXplore.cli_cmds.mutex_options.mutex import Mutex
 
 
-@click.group("cwe", invoke_without_command=True, help="Query for cwe specific data")
+@click.group("capec", invoke_without_command=True, help="Query for capec specific data")
 @click.pass_context
-def cwe_cmd(ctx):
+def capec_cmd(ctx):
     if ctx.invoked_subcommand is None:
-        click.echo(cwe_cmd.get_help(ctx))
+        click.echo(capec_cmd.get_help(ctx))
 
 
-@cwe_cmd.group(
+@capec_cmd.group(
     "search",
     invoke_without_command=True,
-    help="Search for cwe entries by id",
+    help="Search for capec entries by id",
 )
 @click.option(
     "-c",
-    "--cwe",
-    help="Search for CWE's (could be multiple)",
+    "--capec",
+    help="Search for CAPEC's (could be multiple)",
     multiple=True,
-    cls=Mutex,
-    not_required_if=["field_list"],
 )
 @click.option(
     "-f",
     "--field",
     help="Field to return (could be multiple)",
     multiple=True,
     cls=Mutex,
     not_required_if=["field_list"],
 )
 @click.option(
     "-fl",
     "--field_list",
     help="Return a field list for this collection",
-    multiple=True,
     is_flag=True,
     cls=Mutex,
-    not_required_if=["field", "cwe"],
+    not_required_if=["field"],
 )
 @click.option(
     "-o",
     "--output",
     default="json",
     help="Set the desired output format (defaults to json)",
     type=click.Choice(["json", "csv", "xml", "html"], case_sensitive=False),
 )
 @click.pass_context
 def search_cmd(
     ctx,
-    cwe,
+    capec,
     field,
     field_list,
     output,
 ):
-    if cwe:
-        ret_list = getattr(ctx.obj["data_source"], "cwe").mget_by_id(*cwe)
-    elif field_list:
-        ret_list = getattr(ctx.obj["data_source"], "cwe").field_list()
+    if capec and not field_list:
+        ret_list = getattr(ctx.obj["data_source"], "capec").mget_by_id(*capec)
+    elif capec and field_list:
+        ret_list = getattr(ctx.obj["data_source"], "capec").field_list(*capec)
     else:
         click.echo(search_cmd.get_help(ctx))
         return
 
-    if isinstance(ret_list, list):
+    if isinstance(ret_list, list) and not field_list:
         result = [result.to_dict(*field) for result in ret_list]
-    elif isinstance(ret_list, set):
-        result = sorted([result for result in ret_list])
+    elif field_list:
+        result = [result for result in ret_list]
     else:
         result = []
 
     if ctx.invoked_subcommand is None:
         printer(input_data=result, output=output)
     else:
         ctx.obj["RESULT"] = result
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/db_cmds/commands.py` & `CveXplore-6561581/CveXplore/cli_cmds/db_cmds/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     if ctx.invoked_subcommand is None:
         click.echo(sources_cmd.get_help(ctx))
 
 
 @sources_cmd.group("show", invoke_without_command=True, help="Show sources")
 @click.pass_context
 def show_cmd(ctx):
-    config = Configuration()
+    config = Configuration
 
     if ctx.invoked_subcommand is None:
         printer(input_data=[config.SOURCES])
     else:
         printer(input_data=[config.SOURCES])
 
 
@@ -52,30 +52,29 @@
     "--key",
     help="Set the source key",
     type=click.Choice(["capec", "cpe", "cwe", "via4", "cves"], case_sensitive=False),
 )
 @click.option("-v", "--value", help="Set the source key value")
 @click.pass_context
 def set_cmd(ctx, key, value):
-    config = Configuration()
+    config = Configuration
 
     sources = config.SOURCES
 
     sources[key] = value
 
     with open(os.path.join(config.USER_HOME_DIR, ".sources.ini"), "w") as f:
         f.write(json.dumps(sources))
 
     printer(input_data=[{"SOURCES SET TO": sources}])
 
 
 @sources_cmd.group("reset", invoke_without_command=True, help="Set sources")
 @click.pass_context
 def reset_cmd(ctx):
-    config = Configuration()
+    config = Configuration
 
     sources = config.DEFAULT_SOURCES
 
-    with open(os.path.join(config.USER_HOME_DIR, ".sources.ini"), "w") as f:
-        f.write(json.dumps(sources))
+    ctx.obj["data_source"].database.reset_download_sources_to_default()
 
     printer(input_data=[{"SOURCES RESET TO": sources}])
```

### Comparing `CveXplore-0.3.9/CveXplore/cli_cmds/mutex_options/mutex.py` & `CveXplore-6561581/CveXplore/cli_cmds/mutex_options/mutex.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.9/CveXplore/database/connection/mongo_db.py` & `CveXplore-6561581/CveXplore/database/connection/mongodb/mongo_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,81 @@
 """
 Mongo DB connection
 ===================
 """
+
 import atexit
 
 from pymongo import MongoClient
 from pymongo.errors import ServerSelectionTimeoutError
 
+from CveXplore.database.connection.base.db_connection_base import DatabaseConnectionBase
 from CveXplore.database.helpers.cvesearch_mongo_database import CveSearchCollection
 from CveXplore.errors import DatabaseConnectionException
 
 
-class MongoDBConnection(object):
+class MongoDBConnection(DatabaseConnectionBase):
     """
     The MongoDBConnection class serves as a shell that functions as uniform way to connect to the mongodb backend.
-    By default it will try to establish a connection towards a mongodb running on localhost (default port 27017) and
+    By default, it will try to establish a connection towards a mongodb running on localhost (default port 27017) and
     database 'cvedb' (as per defaults of cve_search)
     """
 
     def __init__(
         self,
         host: str = "mongodb://127.0.0.1:27017",
         port: int = None,
         database: str = "cvedb",
-        **kwargs
+        **kwargs,
     ):
         """
         The `host` parameter can be a full `mongodb URI <http://dochub.mongodb.org/core/connections>`_, in addition to
         a simple hostname.
         """
+        super().__init__(logger_name=__name__)
 
         self.client = None
         self._dbclient = None
 
         self.client = MongoClient(host, port, connect=False, **kwargs)
 
         self._dbclient = self.client[database]
 
         try:
-            collections = self._dbclient.list_collection_names()
+            collections = self.dbclient.list_collection_names()
         except ServerSelectionTimeoutError as err:
             raise DatabaseConnectionException(
-                "Connection to the database failed: {}".format(err)
+                f"Connection to the database failed: {err}"
             )
 
         if len(collections) != 0:
             for each in collections:
                 self.__setattr__(
-                    "store_{}".format(each),
-                    CveSearchCollection(database=self._dbclient, name=each),
+                    f"store_{each}",
+                    CveSearchCollection(database=self.dbclient, name=each),
                 )
 
         atexit.register(self.disconnect)
 
-    def get_collections_details(self):
-        for each in self._dbclient.list_collections():
-            yield each
+    @property
+    def dbclient(self):
+        return self._dbclient
 
     def set_handlers_for_collections(self):
-        for each in self._dbclient.list_collection_names():
+        for each in self.dbclient.list_collection_names():
             if not hasattr(self, each):
                 setattr(
                     self,
-                    "store_{}".format(each),
-                    CveSearchCollection(database=self._dbclient, name=each),
+                    f"store_{each}",
+                    CveSearchCollection(database=self.dbclient, name=each),
                 )
 
-    @property
-    def get_collection_names(self):
-        return self._dbclient.list_collection_names()
-
     def disconnect(self):
         """
         Disconnect from mongodb
         """
         if self.client is not None:
             self.client.close()
 
     def __del__(self):
         """Called when the class is garbage collected."""
         self.disconnect()
-
-    def __repr__(self):
-        """String representation of object"""
-        return "<< MongoDBConnection:{} >>".format(self._dbclient.name)
```

### Comparing `CveXplore-0.3.9/CveXplore/database/helpers/cpe_conversion.py` & `CveXplore-6561581/CveXplore/database/helpers/cpe_conversion.py`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.9/CveXplore/database/helpers/cvesearch_mongo_database.py` & `CveXplore-6561581/CveXplore/database/helpers/cvesearch_mongo_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Mongodb specific
 ================
 """
+
 from pymongo.collection import Collection
 from pymongo.cursor import Cursor
 
 
 class CveSearchCollection(Collection):
     """
     The CveSearchCollection is a custom Collection based on the pymongo Collection class which has been altered to
@@ -17,15 +18,15 @@
         Get / create a custon cve-search Mongo collection.
         """
 
         super().__init__(database, name, **kwargs)
 
     def __repr__(self):
         """Return string representation of this class"""
-        return "<< CveSearchCollection:{} >>".format(self.name)
+        return f"<< CveSearchCollection:{self.name} >>"
 
     def find(self, *args, **kwargs):
         """
         Query the database as you would do so with a pymongo Collection.
         """
         return CveSearchCursor(self, *args, **kwargs)
 
@@ -92,8 +93,8 @@
         else:
             raise StopIteration
 
     __next__ = next
 
     def __repr__(self):
         """Return string representation of this class"""
-        return "<< CveSearchCursor:{} >>".format(self.collection)
+        return f"<< CveSearchCursor:{self.collection} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/database/helpers/generic_db.py` & `CveXplore-6561581/CveXplore/database/helpers/generic_db.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Generic database functions
 ==========================
 """
+
 import re
 from functools import reduce
 from typing import Union, Iterable
 
 from CveXplore.common.data_source_connection import DatasourceConnection
 from CveXplore.common.db_mapping import database_mapping
 from CveXplore.objects.cvexplore_object import CveXploreObject
@@ -33,55 +34,54 @@
                 "name",
                 "summary",
                 "prerequisites",
                 "solutions",
                 "loa",
                 "typical_severity",
             ],
-            "cpe": ["title", "cpeName", "vendor", "product"],
-            "cwe": ["name", "status", "Description"],
+            "cpe": ["title", "cpeName", "vendor", "product", "stem"],
+            "cwe": ["name", "status", "description"],
             "cves": [
                 "cvss",
                 "cvss3",
                 "summary",
                 "vendors",
                 "products",
                 "lastModified",
                 "modified",
                 "published",
                 "status",
                 "assigner",
                 "cwe",
+                "epss",
             ],
         }
 
         total_fields_list = (
-            self.__default_fields + self.__fields_mapping[self._collection]
+            self.__default_fields + self.__fields_mapping[self.collection]
         )
         for field in total_fields_list:
             setattr(
                 self,
                 field,
-                GenericDatabaseFieldsFunctions(
-                    field=field, collection=self._collection
-                ),
+                GenericDatabaseFieldsFunctions(field=field, collection=self.collection),
             )
 
     def get_by_id(self, doc_id: str):
         """
         Method to fetch a specific collection entry via it's id number
         """
 
         if not isinstance(doc_id, str):
             try:
                 doc_id = str(doc_id)
             except ValueError:
                 return "Provided value is not a string nor can it be cast to one"
 
-        return self._datasource_collection_connection.find_one({"id": doc_id})
+        return self.datasource_collection_connection.find_one({"id": doc_id})
 
     def mget_by_id(self, *doc_ids: str) -> Union[Iterable[CveXploreObject], Iterable]:
         """
         Method to fetch a specific collection entry via it's id number
         """
         ret_data = []
         for doc_id in doc_ids:
@@ -90,30 +90,59 @@
                 ret_data.append(data)
 
         if len(ret_data) >= 1:
             return sorted(ret_data, key=lambda x: x.id)
         else:
             return ret_data
 
-    def field_list(self) -> set:
+    def _field_list(self, doc_id: str) -> list:
         """
         Method to fetch all field names from a specific collection
         """
-        return reduce(
-            lambda all_keys, rec_keys: all_keys | set(rec_keys),
-            map(
-                lambda d: d.to_dict(),
-                [self._datasource_collection_connection.find_one()],
-            ),
-            set(),
+        return sorted(
+            list(
+                reduce(
+                    lambda all_keys, rec_keys: all_keys | set(rec_keys),
+                    map(
+                        lambda d: d.to_dict(),
+                        [
+                            self.datasource_collection_connection.find_one(
+                                {"id": doc_id}
+                            )
+                        ],
+                    ),
+                    set(),
+                )
+            )
         )
 
+    def field_list(self, *doc_ids: str) -> list:
+        """
+        Method to fetch all field names from a specific collection
+        """
+        ret_data = []
+        for doc_id in sorted(doc_ids):
+            data = self._field_list(doc_id=doc_id)
+            ret_data.append({doc_id: data, "field_count": len(data)})
+
+        return ret_data
+
+    def mapped_fields(self, collection: str) -> list:
+        ret_list = []
+        try:
+            ret_list.extend(self.__fields_mapping[collection])
+        except KeyError:
+            pass
+
+        ret_list.extend(self.__default_fields)
+        return sorted(ret_list)
+
     def __repr__(self):
         """String representation of object"""
-        return "<< GenericDatabaseFactory:{} >>".format(self._collection)
+        return f"<< {self.__class__.__name__}:{self.collection} >>"
 
 
 class GenericDatabaseFieldsFunctions(DatasourceConnection):
     """
     The GenericDatabaseFieldsFunctions handles the creation of general, field based, functions
     """
 
@@ -130,24 +159,24 @@
         Method for searching for a given value. The value shall be converted to a regex.
         """
 
         regex = re.compile(value, re.IGNORECASE)
 
         query = {self.__field: {"$regex": regex}}
 
-        return self._datasource_collection_connection.find(query)
+        return self.datasource_collection_connection.find(query)
 
     def find(self, value: str | dict = None):
         """
         Method to find a given value.
         """
 
         if value is not None:
             query = {self.__field: value}
         else:
             query = None
 
-        return self._datasource_collection_connection.find(query)
+        return self.datasource_collection_connection.find(query)
 
     def __repr__(self):
         """String representation of object"""
-        return "<< GenericDatabaseFieldsFunctions:{} >>".format(self._collection)
+        return f"<< GenericDatabaseFieldsFunctions:{self.collection} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/database/helpers/specific_db.py` & `CveXplore-6561581/CveXplore/database/helpers/specific_db.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Specific database functions
 ===========================
 """
+
 import re
-from typing import List, Union, Iterable
+from functools import reduce
+from typing import List
 
 from pymongo import DESCENDING
 
 from CveXplore.database.helpers.generic_db import GenericDatabaseFactory
 from CveXplore.errors.validation import CveNumberValidationError
 from CveXplore.objects.cvexplore_object import CveXploreObject
 
@@ -25,54 +27,77 @@
         self, vendor: str, limit: int = 0
     ) -> List[CveXploreObject] | None:
         """
         Function to return cves based on a given vendor. By default, to result is sorted descending on th cvss field.
         """
 
         the_result = list(
-            self._datasource_collection_connection.find({"vendors": vendor})
+            self.datasource_collection_connection.find({"vendors": vendor})
             .limit(limit)
             .sort("cvss", DESCENDING)
         )
 
         if len(the_result) != 0:
             return the_result
         else:
             return None
 
-    def get_by_id(self, doc_id: str):
-        """
-        Method to retrieve a single CVE from the database by its CVE ID number.
-        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
-        """
+    def __parse_cve_id(self, doc_id: str) -> str:
         # first try to match full cve number format
         reg_match = re.compile(r"[cC][vV][eE]-\d{4}-\d{4,10}")
         if reg_match.match(doc_id) is not None:
             doc_id = doc_id.upper()
         else:
             part_match = re.compile(r"\d{4}-\d{4,10}")
             if part_match.match(doc_id) is not None:
                 doc_id = f"CVE-{doc_id}"
             else:
                 raise CveNumberValidationError(
                     "Could not validate the CVE number. The number format should be either "
                     "CVE-2000-0001, cve-2000-0001 or 2000-0001."
                 )
+        return doc_id
+
+    def get_by_id(self, doc_id: str):
+        """
+        Method to retrieve a single CVE from the database by its CVE ID number.
+        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
+        """
+        doc_id = self.__parse_cve_id(doc_id)
 
         if not isinstance(doc_id, str):
             try:
                 doc_id = str(doc_id)
             except ValueError:
                 return "Provided value is not a string nor can it be cast to one"
 
-        return self._datasource_collection_connection.find_one({"id": doc_id})
+        return self.datasource_collection_connection.find_one({"id": doc_id})
+
+    def _field_list(self, doc_id: str) -> list:
+        """
+        Method to fetch all field names from a specific collection
+        """
+        doc_id = self.__parse_cve_id(doc_id)
 
-    def __repr__(self):
-        """String representation of object"""
-        return "<< CvesDatabaseFunctions:{} >>".format(self._collection)
+        return sorted(
+            list(
+                reduce(
+                    lambda all_keys, rec_keys: all_keys | set(rec_keys),
+                    map(
+                        lambda d: d.to_dict(),
+                        [
+                            self.datasource_collection_connection.find_one(
+                                {"id": doc_id}
+                            )
+                        ],
+                    ),
+                    set(),
+                )
+            )
+        )
 
 
 class CpeDatabaseFunctions(GenericDatabaseFactory):
     """
     The CpeDatabaseFunctions is a specific class that provides the cpe attribute of a CveXplore instance additional
     functions that only apply to the 'cpe' collection
     """
@@ -88,15 +113,15 @@
         returned.
         """
         regex = re.compile(value, re.IGNORECASE)
 
         query = {"$and": [{field: {"$regex": regex}}, {"deprecated": False}]}
 
         the_result = list(
-            self._datasource_collection_connection.find(query)
+            self.datasource_collection_connection.find(query)
             .limit(limit)
             .sort(field, sorting)
         )
 
         if len(the_result) != 0:
             return the_result
         else:
@@ -108,20 +133,36 @@
         """
         Function to find cpe based on value in string. Only active (deprecated == false) cpe records are
         returned.
         """
         query = {"$and": [{field: value}, {"deprecated": False}]}
 
         the_result = list(
-            self._datasource_collection_connection.find(query)
+            self.datasource_collection_connection.find(query)
             .limit(limit)
             .sort(field, sorting)
         )
 
         if len(the_result) != 0:
             return the_result
         else:
             return None
 
-    def __repr__(self):
-        """String representation of object"""
-        return "<< CpeDatabaseFunctions:{} >>".format(self._collection)
+
+class CapecDatabaseFunctions(GenericDatabaseFactory):
+    """
+    The CapecDatabaseFunctions is a specific class that provides the capec attribute of a CveXplore instance additional
+    functions that only apply to the 'capec' collection
+    """
+
+    def __init__(self, collection: str):
+        super().__init__(collection)
+
+
+class CWEDatabaseFunctions(GenericDatabaseFactory):
+    """
+    The CWEDatabaseFunctions is a specific class that provides the cwe attribute of a CveXplore instance additional
+    functions that only apply to the 'cwe' collection
+    """
+
+    def __init__(self, collection: str):
+        super().__init__(collection)
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/DatabaseSchemaChecker.py` & `CveXplore-6561581/CveXplore/core/database_version/db_version_checker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 import json
-import logging
 import os
 
-from CveXplore.database.connection.mongo_db import MongoDBConnection
-from CveXplore.errors import DatabaseSchemaError
+from CveXplore.core.database_maintenance.update_base_class import UpdateBaseClass
+from CveXplore.database.connection.base.db_connection_base import DatabaseConnectionBase
+from CveXplore.errors import DatabaseSchemaVersionError
 
 runPath = os.path.dirname(os.path.realpath(__file__))
 
 
-class SchemaChecker(object):
-    def __init__(self):
+class DatabaseVersionChecker(UpdateBaseClass):
+    def __init__(self, datasource: DatabaseConnectionBase):
+        super().__init__(logger_name=__name__)
+
         with open(os.path.join(runPath, "../../.schema_version")) as f:
             self.schema_version = json.loads(f.read())
 
-        database = MongoDBConnection(**json.loads(os.getenv("MONGODB_CON_DETAILS")))
-
-        self.dbh = database._dbclient["schema"]
+        database = datasource
 
-        self.logger = logging.getLogger("SchemaChecker")
+        self.dbh = database.dbclient["schema"]
 
     def validate_schema(self):
         try:
             if (
                 not self.schema_version["version"]
                 == list(self.dbh.find({}))[0]["version"]
             ):
                 if not self.schema_version["rebuild_needed"]:
-                    raise DatabaseSchemaError(
+                    raise DatabaseSchemaVersionError(
                         "Database is not on the latest schema version; please update the database!"
                     )
                 else:
-                    raise DatabaseSchemaError(
+                    raise DatabaseSchemaVersionError(
                         "Database schema is not up to date; please re-populate the database!"
                     )
             else:
                 return True
         except IndexError:
             # something went wrong fetching the result from the database; assume re-populate is needed
-            raise DatabaseSchemaError(
+            raise DatabaseSchemaVersionError(
                 "Database schema is not up to date; please re-populate the database!"
             )
 
-    def create_indexes(self):
-        # hack for db_updater.py to put this class in the posts variable and run the update method
+    def update(self):
         self.logger.info("Updating schema version")
-        self.update()
-        self.logger.info("Update schema version done!")
 
-    def update(self):
         try:
             current_record = list(self.dbh.find({}))
 
             if len(current_record) != 0:
                 current_record[0]["version"] = self.schema_version["version"]
                 current_record[0]["rebuild_needed"] = self.schema_version[
                     "rebuild_needed"
@@ -69,7 +65,9 @@
                 self.dbh.insert_one(current_record)
         except AttributeError:
             current_record = {
                 "version": self.schema_version["version"],
                 "rebuild_needed": self.schema_version["rebuild_needed"],
             }
             self.dbh.insert_one(current_record)
+
+        self.logger.info("Update schema version done!")
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/DownloadHandler.py` & `CveXplore-6561581/CveXplore/core/database_maintenance/download_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Download Handler
 ================
 """
+
 import datetime
 import gzip
-import json
 import logging
 import os
 import sys
 import tempfile
 import threading
 import time
 import zipfile
@@ -23,32 +23,42 @@
 from dateutil.parser import parse as parse_datetime
 from pymongo.errors import BulkWriteError, InvalidOperation
 from requests.adapters import HTTPAdapter
 from tqdm.contrib.concurrent import thread_map
 from urllib3 import Retry
 
 from CveXplore.common.config import Configuration
-from CveXplore.database.connection.mongo_db import MongoDBConnection
-from .LogHandler import UpdateHandler
-from .Toolkit import sanitize
-from .worker_q import WorkerQueue
+from CveXplore.core.general.utils import sanitize
+from CveXplore.core.worker_queue.worker_q import WorkerQueue
+from ..database_indexer.db_indexer import DatabaseIndexer
+from ..logging.handlers.cve_explore_rfh import CveExploreUpdateRfhHandler
+from ..logging.handlers.cve_explore_stream import CveExploreUpdateStreamHandler
+from ..logging.logger_class import AppLogger
+from ...database.connection.database_connection import DatabaseConnection
 
 thread_local = threading.local()
-logging.setLoggerClass(UpdateHandler)
+logging.setLoggerClass(AppLogger)
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 class DownloadHandler(ABC):
     """
     DownloadHandler is the base class for all downloads and subsequent processing of the downloaded content.
     Each download script has a derived class which handles specifics for that type of content / download.
     """
 
-    def __init__(self, feed_type: str, prefix: str = None):
+    def __init__(
+        self,
+        feed_type: str,
+        logger_name: str,
+        prefix: str = None,
+    ):
+        self.config = Configuration
+
         self._end = None
 
         self.feed_type = feed_type
 
         self.prefix = prefix
 
         self.queue = WorkerQueue(name=self.feed_type)
@@ -58,38 +68,80 @@
 
         self.progress_bar = None
 
         self.last_modified = None
 
         self.do_process = True
 
-        database = MongoDBConnection(**json.loads(os.getenv("MONGODB_CON_DETAILS")))
+        database = DatabaseConnection(
+            database_type=self.config.DATASOURCE_TYPE,
+            database_init_parameters=self.config.DATASOURCE_CONNECTION_DETAILS,
+        ).database_connection
+
+        self.database = database.dbclient
 
-        self.database = database._dbclient
+        self.database_indexer = DatabaseIndexer(datasource=database)
 
-        self.logger = logging.getLogger("DownloadHandler")
+        self.logger = logging.getLogger(logger_name)
+
+        if len(self.logger.handlers) == 1:
+            self.logger.removeHandler(self.logger.handlers[0])
+
+        self.logger.propagate = False
+
+        self.formatter = logging.Formatter(
+            "%(asctime)s - %(name)-8s - %(levelname)-8s - %(message)s"
+        )
 
-        self.config = Configuration()
+        crf = None
+
+        cli = CveExploreUpdateStreamHandler(stream=sys.stdout)
+        cli.setFormatter(self.formatter)
+        cli.setLevel(logging.INFO)
+
+        if self.config.LOGGING_TO_FILE:
+            crf = CveExploreUpdateRfhHandler(
+                filename=f"{self.config.LOGGING_FILE_PATH}/{self.config.LOGGING_UPDATE_FILE_NAME}",
+                maxBytes=self.config.LOGGING_MAX_FILE_SIZE,
+                backupCount=self.config.LOGGING_BACKLOG,
+            )
+            crf.setLevel(logging.DEBUG)
+            crf.setFormatter(self.formatter)
+
+        if len(self.logger.handlers) > 0:
+            for handler in self.logger.handlers:
+                # add the handlers to the logger
+                # makes sure no duplicate handlers are added
+                if not isinstance(
+                    handler, CveExploreUpdateRfhHandler
+                ) and not isinstance(handler, CveExploreUpdateStreamHandler):
+                    if crf is not None:
+                        self.logger.addHandler(crf)
+                    self.logger.addHandler(cli)
+        else:
+            if crf is not None:
+                self.logger.addHandler(crf)
+            self.logger.addHandler(cli)
 
     def __repr__(self):
         """return string representation of object"""
-        return "<< DownloadHandler:{} >>".format(self.feed_type)
+        return f"<< {self.__class__.__name__}:{self.feed_type} >>"
 
     def get_session(
         self,
-        retries: int = 1,
+        retries: int = 5,
         backoff_factor: float = 0.3,
         status_forcelist: tuple = (429, 500, 502, 503, 504),
         session=None,
     ) -> requests.Session:
         """
         Method for returning a session object per every requesting thread
         """
 
-        proxies = {"http": self.config.getProxy(), "https": self.config.getProxy()}
+        proxies = self.config.HTTP_PROXY_DICT
 
         if not hasattr(thread_local, "session"):
             session = session or requests.Session()
             retry = Retry(
                 total=retries,
                 read=retries,
                 connect=retries,
@@ -110,15 +162,24 @@
     def process_downloads(self, sites: list):
         """
         Method to download and process files
         """
 
         start_time = time.time()
 
-        thread_map(self.download_site, sites, desc="Downloading files")
+        self.logger.info(
+            f"Downloading files (max {self.config.MAX_DOWNLOAD_WORKERS} workers)"
+        )
+
+        thread_map(
+            self.download_site,
+            sites,
+            desc="Downloading files",
+            max_workers=self.config.MAX_DOWNLOAD_WORKERS,
+        )
 
         if self.do_process:
             thread_map(
                 self.file_to_queue,
                 self.file_queue.getall(),
                 desc="Processing downloaded files",
             )
@@ -132,32 +193,42 @@
                 self._db_bulk_writer, chunks, desc="Transferring queue to database"
             )
 
             # checking if last-modified was in the response headers and not set to default
             if "01-01-1970" != self.last_modified.strftime("%d-%m-%Y"):
                 self.setColUpdate(self.feed_type.lower(), self.last_modified)
 
-        self.logger.info(
-            "Duration: {}".format(timedelta(seconds=time.time() - start_time))
-        )
+        self.logger.info(f"Duration: {timedelta(seconds=time.time() - start_time)}")
 
     def chunk_list(self, lst: list, number: int) -> list:
         """
         Yield successive n-sized chunks from lst.
         """
         for i in range(0, len(lst), number):
             yield lst[i : i + number]
 
-    def _db_bulk_writer(self, batch: list):
+    def _db_bulk_writer(self, batch: list, initialization_run: bool = False):
         """
         Method to act as worker for writing queued entries into the database
         """
 
         try:
-            self.database[self.feed_type.lower()].bulk_write(batch, ordered=False)
+            if self.feed_type.lower() == "epss":
+                self.database["cves"].bulk_write(batch, ordered=False)
+            elif initialization_run and (
+                self.feed_type.lower() == "cves" or self.feed_type.lower() == "cpe"
+            ):
+                # cves or cpe process item could yield None; so filter None from batch list
+                self.database[self.feed_type.lower()].insert_many(
+                    [x for x in batch if x is not None], ordered=False
+                )
+            else:
+                self.database[self.feed_type.lower()].bulk_write(
+                    [x for x in batch if x is not None], ordered=False
+                )
         except BulkWriteError as err:
             self.logger.debug(f"Error during bulk write: {err}")
             pass
         except InvalidOperation as err:
             self.logger.debug(f"Got error during bulk update: {err}")
             pass
         except TypeError as err:
@@ -176,71 +247,121 @@
         if (
             content_type == "application/zip"
             or content_type == "application/x-zip"
             or content_type == "application/x-zip-compressed"
             or content_type == "application/zip-compressed"
         ):
             filename = os.path.join(wd, url.split("/")[-1][:-4])
-            self.logger.debug("Saving file to: {}".format(filename))
+            self.logger.debug(f"Saving file to: {filename}")
 
             with zipfile.ZipFile(BytesIO(response_content)) as zip_file:
                 zip_file.extractall(wd)
 
         elif (
             content_type == "application/x-gzip"
             or content_type == "application/gzip"
             or content_type == "application/x-gzip-compressed"
             or content_type == "application/gzip-compressed"
         ):
             filename = os.path.join(wd, url.split("/")[-1][:-3])
-            self.logger.debug("Saving file to: {}".format(filename))
+            self.logger.debug(f"Saving file to: {filename}")
 
             buf = BytesIO(response_content)
             with open(filename, "wb") as f:
                 f.write(gzip.GzipFile(fileobj=buf).read())
 
         elif (
             content_type == "application/json"
             or content_type == "application/xml"
             or content_type == "text/xml"
         ):
             filename = os.path.join(wd, url.split("/")[-1])
-            self.logger.debug("Saving file to: {}".format(filename))
+            self.logger.debug(f"Saving file to: {filename}")
 
             with open(filename, "wb") as output_file:
                 output_file.write(response_content)
 
         elif content_type == "application/local":
             filename = os.path.join(wd, url.split("/")[-1])
-            self.logger.debug("Saving file to: {}".format(filename))
+            self.logger.debug(f"Saving file to: {filename}")
 
             copy(url[7:], filename)
 
         else:
             self.logger.error(
-                "Unhandled Content-Type encountered: {} from url".format(
-                    content_type, url
-                )
+                f"Unhandled Content-Type encountered: {content_type} from url: {url}"
             )
             sys.exit(1)
 
         return wd, filename
 
+    def source_changed(self, url: str) -> bool:
+        """
+        Method to check whether the source file has changed since last update using HEAD instead of GET.
+        """
+
+        # Always assume a file has changed; only compare last-modified for HTTP resources
+        if url[:4] == "file":
+            return True
+        else:
+            i = self.getInfo(self.feed_type.lower())
+
+            if i is None:
+                self.logger.info(
+                    f"Cached last-modified for {self.feed_type}'s not found; should update"
+                )
+                return True
+            else:
+                self.logger.info(
+                    f"Comparing cached last-modified of {self.feed_type} ({i['lastModified']}) with URL {url}"
+                )
+                session = self.get_session()
+
+                try:
+                    with session.head(url) as response:
+                        try:
+                            self.last_modified = parse_datetime(
+                                response.headers["last-modified"], ignoretz=True
+                            )
+                            self.logger.debug(
+                                f"Last {self.feed_type} modified value: {self.last_modified} for URL: {url}"
+                            )
+                        except KeyError:
+                            self.logger.info(
+                                f"Did not receive last-modified header in the response; assuming {self.feed_type}'s have changed"
+                            )
+                            return True
+
+                        if self.last_modified == i["lastModified"]:
+                            self.logger.info(
+                                f"{self.feed_type}'s are not modified since the last update"
+                            )
+                            return False
+                        else:
+                            self.logger.info(
+                                f"{self.feed_type}'s last-modified changed ({self.last_modified}); should update"
+                            )
+                            return True
+
+                except Exception:
+                    self.logger.warning(
+                        f"Exception encountered during comparison; assuming {self.feed_type}'s have changed"
+                    )
+                    return True
+
     def download_site(self, url: str):
         if url[:4] == "file":
-            self.logger.info("Scheduling local hosted file: {}".format(url))
+            self.logger.info(f"Scheduling local hosted file: {url}")
 
             # local file do not get last_modified header; so completely ignoring last_modified check and always asume
             # local file == the last modified file and set to current time.
             self.last_modified = datetime.datetime.now()
 
             self.logger.debug(
-                "Last {} modified value: {} for URL: {}".format(
-                    self.feed_type, self.last_modified, url
-                )
+                f"Last {self.feed_type} modified value: {self.last_modified} for URL: {url}"
             )
 
             wd, filename = self.store_file(
                 response_content=b"local", content_type="application/local", url=url
             )
 
             if filename is not None:
@@ -248,54 +369,52 @@
             else:
                 self.logger.error(
                     "Unable to retrieve a filename; something went wrong when trying to save the file"
                 )
                 sys.exit(1)
 
         else:
-            self.logger.debug("Downloading from url: {}".format(url))
+            self.logger.debug(f"Downloading from url: {url}")
             session = self.get_session()
             try:
                 with session.get(url) as response:
                     try:
                         self.last_modified = parse_datetime(
                             response.headers["last-modified"], ignoretz=True
                         )
                     except KeyError:
                         self.logger.error(
-                            "Did not receive last-modified header in the response; setting to default "
-                            "(01-01-1970) and force update! Headers received: {}".format(
-                                response.headers
-                            )
+                            f"Did not receive last-modified header in the response; setting to default "
+                            f"(01-01-1970) and force update! Headers received: {response.headers}"
                         )
                         # setting to last_modified to default value
                         self.last_modified = parse_datetime("01-01-1970")
 
                     self.logger.debug(
-                        "Last {} modified value: {} for URL: {}".format(
-                            self.feed_type, self.last_modified, url
-                        )
+                        f"Last {self.feed_type} modified value: {self.last_modified} for URL: {url}"
                     )
 
-                    i = self.getInfo(self.feed_type.lower())
-
-                    if i is not None:
-                        if self.last_modified == i["lastModified"]:
-                            self.logger.info(
-                                "{}'s are not modified since the last update".format(
-                                    self.feed_type
+                    # epss releases on daily basis, if new cve's are inserted in the database
+                    # it might be missing epss info, so always run the epss update
+                    if self.feed_type.lower() != "epss":
+                        i = self.getInfo(self.feed_type.lower())
+
+                        if i is not None:
+                            if self.last_modified == i["lastModified"]:
+                                self.logger.info(
+                                    f"{self.feed_type}'s are not modified since the last update"
                                 )
-                            )
-                            self.file_queue.getall()
-                            self.do_process = False
+                                self.file_queue.getall()
+                                self.do_process = False
+
                     if self.do_process:
                         content_type = response.headers["content-type"]
 
                         self.logger.debug(
-                            "URL: {} fetched Content-Type: {}".format(url, content_type)
+                            f"URL: {url} fetched Content-Type: {content_type}"
                         )
 
                         wd, filename = self.store_file(
                             response_content=response.content,
                             content_type=content_type,
                             url=url,
                         )
@@ -305,22 +424,18 @@
                         else:
                             self.logger.error(
                                 "Unable to retrieve a filename; something went wrong when trying to save the file"
                             )
                             sys.exit(1)
             except Exception as err:
                 self.logger.info(
-                    "Exception encountered during download from: {}. Please check the logs for more information!".format(
-                        url
-                    )
+                    f"Exception encountered during download from: {url}. Please check the logs for more information!"
                 )
                 self.logger.error(
-                    "Exception encountered during the download from: {}. Error encountered: {}".format(
-                        url, err
-                    )
+                    f"Exception encountered during the download from: {url}. Error encountered: {err}"
                 )
                 self.do_process = False
 
     def dropCollection(self, col: str):
         return self.database[col].drop()
 
     def getTableNames(self):
@@ -331,15 +446,15 @@
             {"db": collection}, {"$set": {field: data}}, upsert=True
         )
 
     def delColInfo(self, collection: str):
         self.database["info"].delete_one({"db": collection})
 
     def getCPEVersionInformation(self, query: dict):
-        return sanitize(self.database["cpe"].find_one(query))
+        return sanitize(self.database["cpe"].find(query))
 
     def getInfo(self, collection: str):
         return sanitize(self.database["info"].find_one({"db": collection}))
 
     def setColUpdate(self, collection: str, date: datetime):
         self.database["info"].update_one(
             {"db": collection}, {"$set": {"lastModified": date}}, upsert=True
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/LogHandler.py` & `CveXplore-6561581/CveXplore/core/logging/logger_class.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,177 @@
-"""
-Log Handler
-===========
-"""
 import logging
-import platform
-from logging.config import dictConfig
+import os
 from logging.handlers import RotatingFileHandler
 
 import colors
 
 from CveXplore.common.config import Configuration
+from CveXplore.core.logging.formatters.task_formatter import TaskFormatter
+from CveXplore.core.logging.handlers.gelf_handler import GelfUDPHandler
+from CveXplore.core.logging.handlers.syslog_handler import FullSysLogHandler
+
+CRITICAL = 50
+FATAL = CRITICAL
+ERROR = 40
+WARNING = 30
+WARN = WARNING
+INFO = 20
+DEBUG = 10
+NOTSET = 0
+
+level_map = {
+    "debug": "magenta",
+    "info": "white",
+    "warning": "yellow",
+    "error": "red",
+    "critical": "red",
+}
+
+
+class AppLogger(logging.Logger):
+    def __init__(self, name, level=logging.NOTSET):
+        self.formatter = TaskFormatter(
+            "%(asctime)s - %(task_name)s - %(name)-8s - %(levelname)-8s - [%(task_id)s] %(message)s"
+        )
+        self.config = Configuration
 
+        root = logging.getLogger()
 
-class HostnameFilter(logging.Filter):
-    hostname = platform.node()
+        root.setLevel(logging.DEBUG)
 
-    def filter(self, record):
-        record.hostname = HostnameFilter.hostname
-        return True
-
-
-class HelperLogger(logging.Logger):
-    """
-    The HelperLogger is used by the application / gui as their logging class and *extends* the default python
-    logger.logging class.
-    """
-
-    config = Configuration()
-
-    logDict = {
-        "version": 1,
-        "formatters": {
-            "sysLogFormatter": {
-                "format": "%(asctime)s - %(name)-8s - %(levelname)-8s - %(message)s"
-            },
-            "simpleFormatter": {
-                "format": "%(asctime)s - %(name)-8s - %(levelname)-8s - %(message)s"
-            },
-        },
-        "handlers": {
-            "consoleHandler": {
-                "class": "logging.StreamHandler",
-                "level": "INFO",
-                "stream": "ext://sys.stdout",
-                "formatter": "simpleFormatter",
-            }
-        },
-        "root": {"level": "DEBUG", "handlers": ["consoleHandler"]},
-    }
-
-    dictConfig(logDict)
-
-    level_map = {
-        "debug": "magenta",
-        "info": "white",
-        "warning": "yellow",
-        "error": "red",
-        "critical": "red",
-    }
+        root_null_handler = logging.NullHandler()
+        root.handlers.clear()
+        root.addHandler(root_null_handler)
 
-    def __init__(self, name: str, level: int | str = logging.NOTSET):
         super().__init__(name, level)
 
-    def debug(self, msg: str, *args, **kwargs):
+        self.propagate = False
+
+        if self.config.LOGGING_FILE_PATH != "":
+            if not os.path.exists(self.config.LOGGING_FILE_PATH):
+                os.makedirs(self.config.LOGGING_FILE_PATH)
+
+            crf = RotatingFileHandler(
+                filename=f"{self.config.LOGGING_FILE_PATH}/{self.config.LOGGING_FILE_NAME}",
+                maxBytes=self.config.LOGGING_MAX_FILE_SIZE,
+                backupCount=self.config.LOGGING_BACKLOG,
+            )
+            crf.setLevel(self.config.LOGGING_LEVEL)
+            crf.setFormatter(self.formatter)
+            self.addHandler(crf)
+
+        if self.config.SYSLOG_ENABLE:
+            syslog_server = self.config.SYSLOG_SERVER
+            syslog_port = self.config.SYSLOG_PORT
+
+            if self.config.GELF_SYSLOG:
+                syslog = GelfUDPHandler(
+                    host=syslog_server,
+                    port=syslog_port,
+                    _application_name="CveXplore",
+                    include_extra_fields=True,
+                    debug=True,
+                    **(
+                        self.config.GELF_SYSLOG_ADDITIONAL_FIELDS
+                        if self.config.GELF_SYSLOG_ADDITIONAL_FIELDS is not None
+                        else {}
+                    ),
+                )
+            else:
+                syslog = FullSysLogHandler(
+                    address=(syslog_server, syslog_port),
+                    facility=FullSysLogHandler.LOG_LOCAL0,
+                    appname="CveXplore",
+                )
+
+            syslog.setFormatter(self.formatter)
+            syslog.setLevel(self.config.SYSLOG_LEVEL)
+            self.addHandler(syslog)
+
+    def debug(self, msg, *args, **kwargs):
         """
         Log ‘msg % args’ with severity ‘DEBUG’ and color *MAGENTA.
 
         To pass exception information, use the keyword argument exc_info with a true value, e.g.
 
-        .. code-block:: python
-
-            >>> logger.debug(“Houston, we have a thorny problem”)
+        logger.debug(“Houston, we have a %s”, “thorny problem”, exc_info=1)
 
+        :param msg: Message to log
+        :type msg: str
         """
 
-        msg = colors.color("{}".format(msg), fg=HelperLogger.level_map["debug"])
+        msg = colors.color("{}".format(msg), fg=level_map["debug"])
 
-        return super(HelperLogger, self).debug(msg, *args, **kwargs)
+        if self.isEnabledFor(DEBUG):
+            self._log(DEBUG, msg, args, **kwargs)
 
-    def info(self, msg: str, *args, **kwargs):
+    def info(self, msg, *args, **kwargs):
         """
         Log ‘msg % args’ with severity ‘INFO’ and color *WHITE*.
 
         To pass exception information, use the keyword argument exc_info with a true value, e.g.
 
-        .. code-block:: python
-
-            >>> logger.info(“Houston, we have an interesting problem”)
+        logger.info(“Houston, we have a %s”, “interesting problem”, exc_info=1)
 
+        :param msg: Message to log
+        :type msg: str
         """
 
-        msg = colors.color("{}".format(msg), fg=HelperLogger.level_map["info"])
+        msg = colors.color("{}".format(msg), fg=level_map["info"])
 
-        return super(HelperLogger, self).info(msg, *args, **kwargs)
+        if self.isEnabledFor(INFO):
+            self._log(INFO, msg, args, **kwargs)
 
-    def warning(self, msg: str, *args, **kwargs):
+    def warning(self, msg, *args, **kwargs):
         """
         Log ‘msg % args’ with severity ‘WARNING’ and color *YELLOW*.
 
         To pass exception information, use the keyword argument exc_info with a true value, e.g.
 
-        .. code-block:: python
-
-            >>> logger.warning(“Houston, we have a bit of a problem”)
+        logger.warning(“Houston, we have a %s”, “bit of a problem”, exc_info=1)
 
+        :param msg: Message to log
+        :type msg: str
         """
 
-        msg = colors.color("{}".format(msg), fg=HelperLogger.level_map["warning"])
+        msg = colors.color("{}".format(msg), fg=level_map["warning"])
 
-        return super(HelperLogger, self).warning(msg, *args, **kwargs)
+        if self.isEnabledFor(WARNING):
+            self._log(WARNING, msg, args, **kwargs)
 
-    def error(self, msg: str, *args, **kwargs):
+    def error(self, msg, *args, **kwargs):
         """
         Log ‘msg % args’ with severity ‘ERROR’ and color *RED*.
 
         Store logged message to the database for dashboard alerting.
 
         To pass exception information, use the keyword argument exc_info with a true value, e.g.
 
-        .. code-block:: python
-
-            >>> logger.error(“Houston, we have a major problem”)
+        logger.error(“Houston, we have a %s”, “major problem”, exc_info=1)
 
+        :param msg: Message to log
+        :type msg: str
         """
 
-        msg = colors.color("{}".format(msg), fg=HelperLogger.level_map["error"])
+        msg = colors.color("{}".format(msg), fg=level_map["error"])
 
-        return super(HelperLogger, self).error(msg, *args, **kwargs)
+        if self.isEnabledFor(ERROR):
+            self._log(ERROR, msg, args, **kwargs)
 
-    def critical(self, msg: str, *args, **kwargs):
+    def critical(self, msg, *args, **kwargs):
         """
         Log ‘msg % args’ with severity ‘CRITICAL’ and color *RED*.
 
         Store logged message to the database for dashboard alerting.
 
         To pass exception information, use the keyword argument exc_info with a true value, e.g.
 
-        .. code-block:: python
-
-            >>> logger.critical(“Houston, we have a hell of a problem”)
+        logger.critical(“Houston, we have a %s”, “hell of a problem”, exc_info=1)
 
+        :param msg: Message to log
+        :type msg: str
         """
 
-        msg = colors.color("{}".format(msg), fg=HelperLogger.level_map["critical"])
-
-        return super(HelperLogger, self).critical(msg, *args, **kwargs)
-
-
-class UpdateHandler(HelperLogger):
-    """
-    The UpdateHandler is used by the update process to provide written and visual feedback to the initiator of database
-    management tasks.
-    """
-
-    def __init__(self, name: str, level: int | str = logging.NOTSET):
-        super().__init__(name, level)
+        msg = colors.color("{}".format(msg), fg=level_map["critical"])
 
-        formatter = logging.Formatter(
-            "%(asctime)s - %(name)-8s - %(levelname)-8s - %(message)s"
-        )
-
-        if self.config.LOGGING_TO_FILE:
-            crf = RotatingFileHandler(
-                filename=self.config.getUpdateLogFile(),
-                maxBytes=self.config.getMaxLogSize(),
-                backupCount=self.config.getBacklog(),
-            )
-            crf.setLevel(logging.DEBUG)
-            crf.setFormatter(formatter)
-            self.addHandler(crf)
+        if self.isEnabledFor(CRITICAL):
+            self._log(CRITICAL, msg, args, **kwargs)
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/Sources_process.py` & `CveXplore-6561581/CveXplore/core/database_maintenance/sources_process.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,114 @@
 """
 Source processing classes
 =========================
 """
+
 import datetime
 import glob
 import hashlib
 import json
-import logging
-import os
 import shutil
 import time
-from collections import namedtuple
 from typing import Any, Tuple
 from xml.sax import make_parser
 
 from dateutil.parser import parse as parse_datetime
-from pymongo import TEXT, ASCENDING
 from tqdm import tqdm
 
-from CveXplore.common.config import Configuration
-from CveXplore.database.connection.mongo_db import MongoDBConnection
-from CveXplore.database.maintenance.Toolkit import sanitize
-from CveXplore.database.maintenance.api_handlers import NVDApiHandler
-from CveXplore.database.maintenance.content_handlers import CapecHandler, CWEHandler
-from CveXplore.database.maintenance.db_action import DatabaseAction
-from CveXplore.database.maintenance.file_handlers import XMLFileHandler, JSONFileHandler
-from CveXplore.errors.apis import ApiDataRetrievalFailed
+from CveXplore.core.database_actions.db_action import DatabaseAction
+from CveXplore.core.database_maintenance.api_handlers import NVDApiHandler
+from CveXplore.core.database_maintenance.content_handlers import (
+    CapecHandler,
+    CWEHandler,
+)
+from CveXplore.core.database_maintenance.file_handlers import (
+    XMLFileHandler,
+    JSONFileHandler,
+    CSVFileHandler,
+)
+from CveXplore.errors.apis import ApiDataRetrievalFailed, ApiMaxRetryError
 
 date = datetime.datetime.now()
 year = date.year + 1
 
 # default config
 defaultvalue = {"cwe": "Unknown"}
 
-cveStartYear = Configuration.getCVEStartYear()
-
 
 class CPEDownloads(NVDApiHandler):
     """
     Class processing CPE source files
     """
 
     def __init__(self):
         self.feed_type = "CPE"
 
-        super().__init__(self.feed_type)
-
-        self.logger = logging.getLogger("CPEDownloads")
+        super().__init__(feed_type=self.feed_type, logger_name=__name__)
 
     def file_to_queue(self, *args):
         pass
 
-    @staticmethod
-    def process_the_item(item: dict = None):
+    def parse_cpe_version(self, cpename: str):
+        cpe_list = self.split_cpe_name(cpename)
+        version_stem = cpe_list[5]
+
+        if cpe_list[6] != "*" and cpe_list[6] != "-":
+            return f"{version_stem}.{cpe_list[6]}"
+        else:
+            return version_stem
+
+    def process_the_item(self, item: dict = None):
         if item is None:
             return None
 
         item = item["cpe"]
 
+        # filter out deprecated CPE's if CPE_FILTER_DEPRECATED is set to True
+        if self.config.CPE_FILTER_DEPRECATED:
+            if item["deprecated"]:
+                return None
+
         if "cpeName" not in item:
             return None
 
         title = None
 
         if "titles" in item:
             for t in item["titles"]:
                 if t["lang"] == "en":
                     title = t["title"]
 
+        version = self.parse_cpe_version(cpename=item["cpeName"])
+
+        split_cpe_name = self.split_cpe_name(item["cpeName"])
         cpe = {
             "title": title,
             "cpeName": item["cpeName"],
-            "vendor": item["cpeName"].split(":")[3],
-            "product": item["cpeName"].split(":")[4],
+            "vendor": split_cpe_name[3],
+            "product": split_cpe_name[4],
+            "version": version,
+            "padded_version": self.padded_version(version),
+            "stem": self.stem(item["cpeName"]),
             "cpeNameId": item["cpeNameId"],
             "lastModified": parse_datetime(item["lastModified"], ignoretz=True),
             "created": parse_datetime(item["created"], ignoretz=True),
             "deprecated": item["deprecated"],
+            "deprecatedBy": item["deprecatedBy"] if item["deprecated"] else "",
         }
 
-        version_info = ""
-        if "versionStartExcluding" in item:
-            cpe["versionStartExcluding"] = item["versionStartExcluding"]
-            version_info += cpe["versionStartExcluding"] + "_VSE"
-        if "versionStartIncluding" in item:
-            cpe["versionStartIncluding"] = item["versionStartIncluding"]
-            version_info += cpe["versionStartIncluding"] + "_VSI"
-        if "versionEndExcluding" in item:
-            cpe["versionEndExcluding"] = item["versionEndExcluding"]
-            version_info += cpe["versionEndExcluding"] + "_VEE"
-        if "versionEndIncluding" in item:
-            cpe["versionEndIncluding"] = item["versionEndIncluding"]
-            version_info += cpe["versionEndIncluding"] + "_VEI"
-
         sha1_hash = hashlib.sha1(
-            cpe["cpeName"].encode("utf-8") + version_info.encode("utf-8")
+            cpe["cpeName"].encode("utf-8") + split_cpe_name[5].encode("utf-8")
         ).hexdigest()
 
         cpe["id"] = sha1_hash
 
         return cpe
 
-    def process_downloads(self, sites: list = None):
+    def process_downloads(self, sites: list | None = None):
         """
         Method to download and process files
         """
 
         self.logger.info("Starting download...")
 
         start_time = time.time()
@@ -114,17 +117,21 @@
 
         self.logger.debug(
             f"do_process = {self.do_process}; is_update = {self.is_update}"
         )
 
         if self.do_process:
             if not self.is_update:
-                total_results = self.api_handler.get_count(
-                    self.api_handler.datasource.CPE
-                )
+                try:
+                    total_results = self.api_handler.get_count(
+                        self.api_handler.datasource.CPE
+                    )
+                except ApiMaxRetryError:
+                    # failed to get the count; set total_results to 0 and continue
+                    total_results = 0
 
                 self.logger.info(f"Preparing to download {total_results} CPE entries")
 
                 with tqdm(
                     desc="Downloading and processing content",
                     total=total_results,
                     position=0,
@@ -132,48 +139,65 @@
                 ) as pbar:
                     for entry in self.api_handler.get_all_data(data_type="cpe"):
                         # do something here with the results...
                         for data_list in tqdm(
                             entry, desc=f"Processing batch", leave=False
                         ):
                             if not isinstance(data_list, ApiDataRetrievalFailed):
-                                processed_items = [
-                                    self.process_item(item)
-                                    for item in data_list["products"]
-                                ]
-                                self._db_bulk_writer(processed_items)
-                                pbar.update(len(data_list["products"]))
+                                if not isinstance(data_list, Exception):
+                                    processed_items = [
+                                        self.process_item(item)
+                                        for item in data_list["products"]
+                                    ]
+                                    self._db_bulk_writer(
+                                        processed_items, initialization_run=True
+                                    )
+                                    pbar.update(len(data_list["products"]))
+                                else:
+                                    self.logger.error(
+                                        f"Retrieval of api data resulted in an Exception: {data_list}..."
+                                    )
                             else:
                                 self.logger.error(
                                     f"Retrieval of api data on url: {data_list.args[0]} failed...."
                                 )
             else:
                 last_mod_start_date = self.database[self.feed_type.lower()].find_one(
                     {}, {"lastModified": 1}, sort=[("lastModified", -1)]
                 )
 
-                if "lastModified" in last_mod_start_date:
-                    last_mod_start_date = last_mod_start_date[
-                        "lastModified"
-                    ] + datetime.timedelta(
-                        0, 1
-                    )  # add one second to prevent false results...
+                if last_mod_start_date is not None:
+                    if "lastModified" in last_mod_start_date:
+                        last_mod_start_date = last_mod_start_date[
+                            "lastModified"
+                        ] + datetime.timedelta(
+                            0, 1
+                        )  # add one second to prevent false results...
+                    else:
+                        raise KeyError(
+                            "Missing field 'lastModified' from database query..."
+                        )
                 else:
-                    raise KeyError(
-                        "Missing field 'lastModified' from database query..."
+                    self.logger.warning(
+                        "No records found in the mongodb cpe collection.."
                     )
+                    return
 
-                # Get datetime from runtime
+                    # Get datetime from runtime
                 last_mod_end_date = datetime.datetime.now()
 
-                total_results = self.api_handler.get_count(
-                    self.api_handler.datasource.CPE,
-                    last_mod_start_date=last_mod_start_date,
-                    last_mod_end_date=last_mod_end_date,
-                )
+                try:
+                    total_results = self.api_handler.get_count(
+                        self.api_handler.datasource.CPE,
+                        last_mod_start_date=last_mod_start_date,
+                        last_mod_end_date=last_mod_end_date,
+                    )
+                except ApiMaxRetryError:
+                    # failed to get the count; set total_results to 0 and continue
+                    total_results = 0
 
                 self.logger.info(f"Preparing to download {total_results} CPE entries")
 
                 with tqdm(
                     desc="Downloading and processing content",
                     total=total_results,
                     position=0,
@@ -185,42 +209,47 @@
                         last_mod_end_date=last_mod_end_date,
                     ):
                         # do something here with the results...
                         for data_list in tqdm(
                             entry, desc=f"Processing batch", leave=False
                         ):
                             if not isinstance(data_list, ApiDataRetrievalFailed):
-                                processed_items = [
-                                    self.process_item(item)
-                                    for item in data_list["products"]
-                                ]
-                                self._db_bulk_writer(processed_items)
-                                pbar.update(len(data_list["products"]))
+                                if not isinstance(data_list, Exception):
+                                    processed_items = [
+                                        self.process_item(item)
+                                        for item in data_list["products"]
+                                    ]
+                                    self._db_bulk_writer(processed_items)
+                                    pbar.update(len(data_list["products"]))
+                                else:
+                                    self.logger.error(
+                                        f"Retrieval of api data resulted in an Exception: {data_list}..."
+                                    )
                             else:
                                 self.logger.error(
                                     f"Retrieval of api data on url: {data_list.args[0]} failed...."
                                 )
 
             # Set the last update time in the info collection
             self.setColUpdate(self.feed_type.lower(), self.last_modified)
 
         self.logger.info(
-            "Duration: {}".format(datetime.timedelta(seconds=time.time() - start_time))
+            f"Duration: {datetime.timedelta(seconds=time.time() - start_time)}"
         )
 
     def update(self, **kwargs):
         self.logger.info("CPE database update started")
 
+        self.process_downloads()
+
         # if collection is non-existent; assume it's not an update
         if self.feed_type.lower() not in self.getTableNames():
-            DatabaseIndexer().create_indexes(collection=self.feed_type.lower())
+            self.database_indexer.create_indexes(collection=self.feed_type.lower())
             self.is_update = False
 
-        self.process_downloads()
-
         self.logger.info("Finished CPE database update")
 
         return self.last_modified
 
     def populate(self, **kwargs):
         self.logger.info("CPE Database population started")
 
@@ -228,79 +257,124 @@
 
         self.queue.clear()
 
         self.delColInfo(self.feed_type.lower())
 
         self.dropCollection(self.feed_type.lower())
 
-        DatabaseIndexer().create_indexes(collection=self.feed_type.lower())
-
         self.process_downloads()
 
+        self.database_indexer.create_indexes(collection=self.feed_type.lower())
+
         self.logger.info("Finished CPE database population")
 
         return self.last_modified
 
 
 class CVEDownloads(NVDApiHandler):
     """
     Class processing CVE source files
     """
 
     def __init__(self):
         self.feed_type = "CVES"
 
-        super().__init__(self.feed_type)
-
-        self.logger = logging.getLogger("CVEDownloads")
+        super().__init__(feed_type=self.feed_type, logger_name=__name__)
 
-    @staticmethod
-    def get_cve_year_range():
-        """
-        Method to fetch the years where we need cve's for
-        """
-        for a_year in range(cveStartYear, year):
-            yield a_year
-
-    @staticmethod
-    def get_cpe_info(cpeuri: str):
+    def get_cpe_info(self, cpeuri: str):
         query = {}
-        version_info = ""
+
         if "versionStartExcluding" in cpeuri:
-            query["versionStartExcluding"] = cpeuri["versionStartExcluding"]
-            version_info += query["versionStartExcluding"] + "_VSE"
-        if "versionStartIncluding" in cpeuri:
-            query["versionStartIncluding"] = cpeuri["versionStartIncluding"]
-            version_info += query["versionStartIncluding"] + "_VSI"
-        if "versionEndExcluding" in cpeuri:
-            query["versionEndExcluding"] = cpeuri["versionEndExcluding"]
-            version_info += query["versionEndExcluding"] + "_VEE"
-        if "versionEndIncluding" in cpeuri:
-            query["versionEndIncluding"] = cpeuri["versionEndIncluding"]
-            version_info += query["versionEndIncluding"] + "_VEI"
+            if "versionEndExcluding" in cpeuri:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gt": self.padded_version(cpeuri["versionStartExcluding"]),
+                        "$lt": self.padded_version(cpeuri["versionEndExcluding"]),
+                    },
+                }
+            elif "versionEndIncluding" in cpeuri:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gt": self.padded_version(cpeuri["versionStartExcluding"]),
+                        "$lte": self.padded_version(cpeuri["versionEndIncluding"]),
+                    },
+                }
+            else:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gt": self.padded_version(cpeuri["versionStartExcluding"])
+                    },
+                }
+
+        elif "versionStartIncluding" in cpeuri:
+            if "versionEndExcluding" in cpeuri:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gte": self.padded_version(cpeuri["versionStartIncluding"]),
+                        "$lt": self.padded_version(cpeuri["versionEndExcluding"]),
+                    },
+                }
+            elif "versionEndIncluding" in cpeuri:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gte": self.padded_version(cpeuri["versionStartIncluding"]),
+                        "$lte": self.padded_version(cpeuri["versionEndIncluding"]),
+                    },
+                }
+            else:
+                query = {
+                    "deprecated": False,
+                    "stem": self.stem(cpeuri["criteria"]),
+                    "padded_version": {
+                        "$gte": self.padded_version(cpeuri["versionStartIncluding"])
+                    },
+                }
+
+        elif "versionEndExcluding" in cpeuri:
+            query = {
+                "deprecated": False,
+                "stem": self.stem(cpeuri["criteria"]),
+                "padded_version": {
+                    "$lt": self.padded_version(cpeuri["versionEndExcluding"])
+                },
+            }
+
+        elif "versionEndIncluding" in cpeuri:
+            query = {
+                "deprecated": False,
+                "stem": self.stem(cpeuri["criteria"]),
+                "padded_version": {
+                    "$lte": self.padded_version(cpeuri["versionEndIncluding"])
+                },
+            }
 
-        return query, version_info
+        return query
 
     @staticmethod
     def add_if_missing(cve: dict, key: str, value: Any):
         if value not in cve[key]:
             cve[key].append(value)
         return cve
 
-    @staticmethod
-    def get_vendor_product(cpeUri: str):
-        vendor = cpeUri.split(":")[3]
-        product = cpeUri.split(":")[4]
+    def get_vendor_product(self, cpeUri: str):
+        split_cpe_uri = self.split_cpe_name(cpeUri)
+        vendor = split_cpe_uri[3]
+        product = split_cpe_uri[4]
         return vendor, product
 
-    @staticmethod
-    def stem(cpeUri: str):
-        cpeArr = cpeUri.split(":")
-        return ":".join(cpeArr[:5])
-
     def file_to_queue(self, *args):
         pass
 
     def process_the_item(self, item: dict = None):
         if item is None:
             return None
 
@@ -312,15 +386,15 @@
             "modified": parse_datetime(item["cve"]["lastModified"], ignoretz=True),
             "lastModified": parse_datetime(item["cve"]["lastModified"], ignoretz=True),
         }
 
         for description in item["cve"]["descriptions"]:
             if description["lang"] == "en":
                 if "summary" in cve:
-                    cve["summary"] += " {}".format(description["value"])
+                    cve["summary"] += f" {description['value']}"
                 else:
                     cve["summary"] = description["value"]
 
         if "metrics" in item["cve"]:
             cve["access"] = {}
             cve["impact"] = {}
             if "cvssMetricV31" in item["cve"]["metrics"]:
@@ -465,266 +539,101 @@
         if "configurations" in item["cve"]:
             cve["vulnerable_configuration"] = []
             cve["vulnerable_product"] = []
             cve["vendors"] = []
             cve["products"] = []
             cve["vulnerable_product_stems"] = []
             cve["vulnerable_configuration_stems"] = []
-            for cpe in item["cve"]["configurations"][0]["nodes"]:
-                if "cpeMatch" in cpe:
-                    for cpeuri in cpe["cpeMatch"]:
-                        if "criteria" not in cpeuri:
-                            continue
-                        if cpeuri["vulnerable"]:
-                            query, version_info = self.get_cpe_info(cpeuri)
-                            if query != {}:
-                                query["id"] = hashlib.sha1(
-                                    cpeuri["criteria"].encode("utf-8")
-                                    + version_info.encode("utf-8")
-                                ).hexdigest()
-                                cpe_info = self.getCPEVersionInformation(query)
-                                if cpe_info:
-                                    if cpe_info["cpeMatch"]:
-                                        for vulnerable_version in cpe_info["cpeMatch"]:
+            cve["configurations"] = item["cve"]["configurations"]
+            for node in item["cve"]["configurations"]:
+                for cpe in node["nodes"]:
+                    if "cpeMatch" in cpe:
+                        for cpeuri in cpe["cpeMatch"]:
+                            if "criteria" not in cpeuri:
+                                continue
+                            if cpeuri["vulnerable"]:
+                                query = self.get_cpe_info(cpeuri)
+                                if query != {}:
+                                    cpe_info = sorted(
+                                        self.getCPEVersionInformation(query),
+                                        key=lambda x: x["padded_version"],
+                                    )
+                                    if cpe_info:
+                                        if not isinstance(cpe_info, list):
+                                            cpe_info = [cpe_info]
+
+                                        for vulnerable_version in cpe_info:
                                             cve = self.add_if_missing(
                                                 cve,
                                                 "vulnerable_product",
-                                                vulnerable_version["criteria"],
+                                                vulnerable_version["cpeName"],
                                             )
                                             cve = self.add_if_missing(
                                                 cve,
                                                 "vulnerable_configuration",
-                                                vulnerable_version["criteria"],
+                                                vulnerable_version["cpeName"],
                                             )
                                             cve = self.add_if_missing(
                                                 cve,
                                                 "vulnerable_configuration_stems",
-                                                self.stem(
-                                                    vulnerable_version["criteria"]
-                                                ),
-                                            )
-                                            vendor, product = self.get_vendor_product(
-                                                vulnerable_version["criteria"]
+                                                vulnerable_version["stem"],
                                             )
+
                                             cve = self.add_if_missing(
-                                                cve, "vendors", vendor
+                                                cve,
+                                                "vendors",
+                                                vulnerable_version["vendor"],
                                             )
+
                                             cve = self.add_if_missing(
-                                                cve, "products", product
+                                                cve,
+                                                "products",
+                                                vulnerable_version["product"],
                                             )
+
                                             cve = self.add_if_missing(
                                                 cve,
                                                 "vulnerable_product_stems",
-                                                self.stem(
-                                                    vulnerable_version["criteria"]
-                                                ),
+                                                vulnerable_version["stem"],
                                             )
-                                    else:
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_product",
-                                            cpeuri["criteria"],
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_configuration",
-                                            cpeuri["criteria"],
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_configuration_stems",
-                                            self.stem(cpeuri["criteria"]),
-                                        )
-                                        vendor, product = self.get_vendor_product(
-                                            cpeuri["criteria"]
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve, "vendors", vendor
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve, "products", product
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_product_stems",
-                                            self.stem(cpeuri["criteria"]),
-                                        )
-                            else:
-                                # If the cpeMatch did not have any of the version start/end modifiers,
-                                # add the CPE string as it is.
-                                cve = self.add_if_missing(
-                                    cve, "vulnerable_product", cpeuri["criteria"]
-                                )
-                                cve = self.add_if_missing(
-                                    cve, "vulnerable_configuration", cpeuri["criteria"]
-                                )
-                                cve = self.add_if_missing(
-                                    cve,
-                                    "vulnerable_configuration_stems",
-                                    self.stem(cpeuri["criteria"]),
-                                )
-                                vendor, product = self.get_vendor_product(
-                                    cpeuri["criteria"]
-                                )
-                                cve = self.add_if_missing(cve, "vendors", vendor)
-                                cve = self.add_if_missing(cve, "products", product)
-                                cve = self.add_if_missing(
-                                    cve,
-                                    "vulnerable_product_stems",
-                                    self.stem(cpeuri["criteria"]),
-                                )
-                        else:
-                            cve = self.add_if_missing(
-                                cve, "vulnerable_configuration", cpeuri["criteria"]
-                            )
-                            cve = self.add_if_missing(
-                                cve,
-                                "vulnerable_configuration_stems",
-                                self.stem(cpeuri["criteria"]),
-                            )
-                if "children" in cpe:
-                    for child in cpe["children"]:
-                        if "cpeMatch" in child:
-                            for cpeuri in child["cpeMatch"]:
-                                if "criteria" not in cpeuri:
-                                    continue
-                                if cpeuri["vulnerable"]:
-                                    query, version_info = self.get_cpe_info(cpeuri)
-                                    if query != {}:
-                                        query["id"] = hashlib.sha1(
-                                            cpeuri["criteria"].encode("utf-8")
-                                            + version_info.encode("utf-8")
-                                        ).hexdigest()
-                                        cpe_info = self.getCPEVersionInformation(query)
-                                        if cpe_info:
-                                            if cpe_info["cpeMatch"]:
-                                                for vulnerable_version in cpe_info[
-                                                    "cpeMatch"
-                                                ]:
-                                                    cve = self.add_if_missing(
-                                                        cve,
-                                                        "vulnerable_product",
-                                                        vulnerable_version["criteria"],
-                                                    )
-                                                    cve = self.add_if_missing(
-                                                        cve,
-                                                        "vulnerable_configuration",
-                                                        vulnerable_version["criteria"],
-                                                    )
-                                                    cve = self.add_if_missing(
-                                                        cve,
-                                                        "vulnerable_configuration_stems",
-                                                        self.stem(
-                                                            vulnerable_version[
-                                                                "criteria"
-                                                            ]
-                                                        ),
-                                                    )
-                                                    (
-                                                        vendor,
-                                                        product,
-                                                    ) = self.get_vendor_product(
-                                                        vulnerable_version["criteria"]
-                                                    )
-                                                    cve = self.add_if_missing(
-                                                        cve, "vendors", vendor
-                                                    )
-                                                    cve = self.add_if_missing(
-                                                        cve, "products", product
-                                                    )
-                                                    cve = self.add_if_missing(
-                                                        cve,
-                                                        "vulnerable_product_stems",
-                                                        self.stem(
-                                                            vulnerable_version[
-                                                                "criteria"
-                                                            ]
-                                                        ),
-                                                    )
-                                            else:
-                                                cve = self.add_if_missing(
-                                                    cve,
-                                                    "vulnerable_product",
-                                                    cpeuri["criteria"],
-                                                )
-                                                cve = self.add_if_missing(
-                                                    cve,
-                                                    "vulnerable_configuration",
-                                                    cpeuri["criteria"],
-                                                )
-                                                cve = self.add_if_missing(
-                                                    cve,
-                                                    "vulnerable_configuration_stems",
-                                                    self.stem(cpeuri["criteria"]),
-                                                )
-                                                (
-                                                    vendor,
-                                                    product,
-                                                ) = self.get_vendor_product(
-                                                    cpeuri["criteria"]
-                                                )
-                                                cve = self.add_if_missing(
-                                                    cve, "vendors", vendor
-                                                )
-                                                cve = self.add_if_missing(
-                                                    cve, "products", product
-                                                )
-                                                cve = self.add_if_missing(
-                                                    cve,
-                                                    "vulnerable_product_stems",
-                                                    self.stem(cpeuri["criteria"]),
-                                                )
-                                    else:
-                                        # If the cpeMatch did not have any of the version start/end modifiers,
-                                        # add the CPE string as it is.
-                                        if "criteria" not in cpeuri:
-                                            continue
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_product",
-                                            cpeuri["criteria"],
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_configuration",
-                                            cpeuri["criteria"],
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_configuration_stems",
-                                            self.stem(cpeuri["criteria"]),
-                                        )
-                                        vendor, product = self.get_vendor_product(
-                                            cpeuri["criteria"]
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve, "vendors", vendor
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve, "products", product
-                                        )
-                                        cve = self.add_if_missing(
-                                            cve,
-                                            "vulnerable_product_stems",
-                                            self.stem(cpeuri["criteria"]),
-                                        )
                                 else:
-                                    if "criteria" not in cpeuri:
-                                        continue
+                                    # If the cpeMatch did not have any of the version start/end modifiers,
+                                    # add the CPE string as it is.
+                                    cve = self.add_if_missing(
+                                        cve, "vulnerable_product", cpeuri["criteria"]
+                                    )
                                     cve = self.add_if_missing(
                                         cve,
                                         "vulnerable_configuration",
                                         cpeuri["criteria"],
                                     )
                                     cve = self.add_if_missing(
                                         cve,
                                         "vulnerable_configuration_stems",
                                         self.stem(cpeuri["criteria"]),
                                     )
-
+                                    vendor, product = self.get_vendor_product(
+                                        cpeuri["criteria"]
+                                    )
+                                    cve = self.add_if_missing(cve, "vendors", vendor)
+                                    cve = self.add_if_missing(cve, "products", product)
+                                    cve = self.add_if_missing(
+                                        cve,
+                                        "vulnerable_product_stems",
+                                        self.stem(cpeuri["criteria"]),
+                                    )
+                            else:
+                                cve = self.add_if_missing(
+                                    cve, "vulnerable_configuration", cpeuri["criteria"]
+                                )
+                                cve = self.add_if_missing(
+                                    cve,
+                                    "vulnerable_configuration_stems",
+                                    self.stem(cpeuri["criteria"]),
+                                )
         if "weaknesses" in item["cve"]:
             for problem in item["cve"]["weaknesses"]:
                 for cwe in problem[
                     "description"
                 ]:  # NVD JSON not clear if we can get more than one CWE per CVE (until we take the last one) -
                     # NVD-CWE-Other??? list?
                     if cwe["lang"] == "en":
@@ -751,17 +660,21 @@
 
         self.logger.debug(
             f"do_process = {self.do_process}; is_update = {self.is_update}"
         )
 
         if self.do_process:
             if not self.is_update:
-                total_results = self.api_handler.get_count(
-                    self.api_handler.datasource.CVE
-                )
+                try:
+                    total_results = self.api_handler.get_count(
+                        self.api_handler.datasource.CVE
+                    )
+                except ApiMaxRetryError:
+                    # failed to get the count; set total_results to 0 and continue
+                    total_results = 0
 
                 self.logger.info(f"Preparing to download {total_results} CVE entries")
 
                 with tqdm(
                     desc="Downloading and processing content",
                     total=total_results,
                     position=0,
@@ -769,44 +682,61 @@
                 ) as pbar:
                     for entry in self.api_handler.get_all_data(data_type="cve"):
                         # do something here with the results...
                         for data_list in tqdm(
                             entry, desc=f"Processing batch", leave=False
                         ):
                             if not isinstance(data_list, ApiDataRetrievalFailed):
-                                processed_items = [
-                                    self.process_item(item)
-                                    for item in data_list["vulnerabilities"]
-                                ]
-                                self._db_bulk_writer(processed_items)
-                                pbar.update(len(data_list["vulnerabilities"]))
+                                if not isinstance(data_list, Exception):
+                                    processed_items = [
+                                        self.process_item(item)
+                                        for item in data_list["vulnerabilities"]
+                                    ]
+                                    self._db_bulk_writer(
+                                        processed_items, initialization_run=True
+                                    )
+                                    pbar.update(len(data_list["vulnerabilities"]))
+                                else:
+                                    self.logger.error(
+                                        f"Retrieval of api data resulted in an Exception: {data_list}..."
+                                    )
                             else:
                                 self.logger.error(
                                     f"Retrieval of api data on url: {data_list.args[0]} failed...."
                                 )
             else:
                 last_mod_start_date = self.database[self.feed_type.lower()].find_one(
                     {}, {"lastModified": 1}, sort=[("lastModified", -1)]
                 )
 
-                if "lastModified" in last_mod_start_date:
-                    last_mod_start_date = last_mod_start_date["lastModified"]
+                if last_mod_start_date is not None:
+                    if "lastModified" in last_mod_start_date:
+                        last_mod_start_date = last_mod_start_date["lastModified"]
+                    else:
+                        raise KeyError(
+                            "Missing field 'lastModified' from database query..."
+                        )
                 else:
-                    raise KeyError(
-                        "Missing field 'lastModified' from database query..."
+                    self.logger.warning(
+                        "No records found in the mongodb cves collection.."
                     )
+                    return
 
-                # Get datetime from runtime
+                    # Get datetime from runtime
                 last_mod_end_date = datetime.datetime.now()
 
-                total_results = self.api_handler.get_count(
-                    self.api_handler.datasource.CVE,
-                    last_mod_start_date=last_mod_start_date,
-                    last_mod_end_date=last_mod_end_date,
-                )
+                try:
+                    total_results = self.api_handler.get_count(
+                        self.api_handler.datasource.CVE,
+                        last_mod_start_date=last_mod_start_date,
+                        last_mod_end_date=last_mod_end_date,
+                    )
+                except ApiMaxRetryError:
+                    # failed to get the count; set total_results to 0 and continue
+                    total_results = 0
 
                 self.logger.info(f"Preparing to download {total_results} CVE entries")
 
                 with tqdm(
                     desc="Downloading and processing content",
                     total=total_results,
                     position=0,
@@ -818,143 +748,144 @@
                         last_mod_end_date=last_mod_end_date,
                     ):
                         # do something here with the results...
                         for data_list in tqdm(
                             entry, desc=f"Processing batch", leave=False
                         ):
                             if not isinstance(data_list, ApiDataRetrievalFailed):
-                                processed_items = [
-                                    self.process_item(item)
-                                    for item in data_list["vulnerabilities"]
-                                ]
-                                self._db_bulk_writer(processed_items)
-                                pbar.update(len(data_list["vulnerabilities"]))
+                                if not isinstance(data_list, Exception):
+                                    processed_items = [
+                                        self.process_item(item)
+                                        for item in data_list["vulnerabilities"]
+                                    ]
+                                    self._db_bulk_writer(processed_items)
+                                    pbar.update(len(data_list["vulnerabilities"]))
+                                else:
+                                    self.logger.error(
+                                        f"Retrieval of api data resulted in an Exception: {data_list}..."
+                                    )
                             else:
                                 self.logger.error(
                                     f"Retrieval of api data on url: {data_list.args[0]} failed...."
                                 )
 
             # Set the last update time in the info collection
             self.setColUpdate(self.feed_type.lower(), self.last_modified)
 
         self.logger.info(
-            "Duration: {}".format(datetime.timedelta(seconds=time.time() - start_time))
+            f"Duration: {datetime.timedelta(seconds=time.time() - start_time)}"
         )
 
     def update(self):
         self.logger.info("CVE database update started")
 
+        self.process_downloads()
+
         # if collection is non-existent; assume it's not an update
         if self.feed_type.lower() not in self.getTableNames():
-            DatabaseIndexer().create_indexes(collection=self.feed_type.lower())
+            self.database_indexer.create_indexes(collection=self.feed_type.lower())
             self.is_update = False
 
-        self.process_downloads()
-
         self.logger.info("Finished CVE database update")
 
         return self.last_modified
 
     def populate(self):
         self.logger.info("CVE database population started")
 
         self.logger.info(
-            "Starting CVE database population starting from year: {}".format(
-                cveStartYear
-            )
+            f"Starting CVE database population starting from year: {self.config.CVE_START_YEAR}"
         )
 
         self.is_update = False
 
         self.queue.clear()
 
         self.delColInfo(self.feed_type.lower())
 
         self.dropCollection(self.feed_type.lower())
 
-        DatabaseIndexer().create_indexes(collection=self.feed_type.lower())
-
         self.process_downloads()
 
+        self.database_indexer.create_indexes(collection=self.feed_type.lower())
+
         self.logger.info("Finished CVE database population")
 
         return self.last_modified
 
 
 class VIADownloads(JSONFileHandler):
     """
     Class processing VIA4 source files
     """
 
     def __init__(self):
         self.feed_type = "VIA4"
         self.prefix = "cves"
-        super().__init__(self.feed_type, self.prefix)
-
-        self.feed_url = Configuration.getFeedURL(self.feed_type.lower())
+        super().__init__(
+            feed_type=self.feed_type, prefix=self.prefix, logger_name=__name__
+        )
 
-        self.logger = logging.getLogger("VIADownloads")
+        self.feed_url = self.config.SOURCES[self.feed_type.lower()]
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
         working_dir, filename = file_tuple
 
         for cve in self.ijson_handler.fetch(filename=filename, prefix=self.prefix):
             x = 0
             for key, val in cve.items():
                 entry_dict = {"id": key}
                 entry_dict.update(val)
                 self.process_item(item=entry_dict)
                 x += 1
 
-            self.logger.debug("Processed {} items from file: {}".format(x, filename))
+            self.logger.debug(f"Processed {x} items from file: {filename}")
 
         with open(filename, "rb") as input_file:
             data = json.loads(input_file.read().decode("utf-8"))
 
             self.setColInfo("via4", "sources", data["metadata"]["sources"])
             self.setColInfo("via4", "searchables", data["metadata"]["searchables"])
 
-            self.logger.debug("Processed metadata from file: {}".format(filename))
+            self.logger.debug(f"Processed metadata from file: {filename}")
 
         try:
-            self.logger.debug("Removing working dir: {}".format(working_dir))
+            self.logger.debug(f"Removing working dir: {working_dir}")
             shutil.rmtree(working_dir)
         except Exception as err:
-            self.logger.error(
-                "Failed to remove working dir; error produced: {}".format(err)
-            )
+            self.logger.error(f"Failed to remove working dir; error produced: {err}")
 
     def process_item(self, item: dict):
         if self.is_update:
             self.queue.put(
                 DatabaseAction(
                     action=DatabaseAction.actions.UpdateOne,
-                    collection=self.feed_type.lower(),
                     doc=item,
                 )
             )
         else:
             self.queue.put(
                 DatabaseAction(
                     action=DatabaseAction.actions.InsertOne,
-                    collection=self.feed_type.lower(),
                     doc=item,
                 )
             )
 
     def update(self, **kwargs):
         self.logger.info("VIA4 database update started")
 
         # if collection is non-existent; assume it's not an update
         if self.feed_type.lower() not in self.getTableNames():
             self.is_update = False
 
-        self.process_downloads([self.feed_url])
-
-        self.logger.info("Finished VIA4 database update")
+        if self.source_changed(self.feed_url):
+            self.process_downloads([self.feed_url])
+            self.logger.info("Finished VIA4 database update")
+        else:
+            self.logger.info("Skipped VIA4 database update")
 
         return self.last_modified
 
     def populate(self, **kwargs):
         self.is_update = False
         self.queue.clear()
 
@@ -968,19 +899,17 @@
 class CAPECDownloads(XMLFileHandler):
     """
     Class processing CAPEC source files
     """
 
     def __init__(self):
         self.feed_type = "CAPEC"
-        super().__init__(self.feed_type)
+        super().__init__(feed_type=self.feed_type, logger_name=__name__)
 
-        self.feed_url = Configuration.getFeedURL(self.feed_type.lower())
-
-        self.logger = logging.getLogger("CAPECDownloads")
+        self.feed_url = self.config.SOURCES[self.feed_type.lower()]
 
         # make parser
         self.parser = make_parser()
         self.ch = CapecHandler()
         self.parser.setContentHandler(self.ch)
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
@@ -988,34 +917,34 @@
 
         self.parser.parse(filename)
         x = 0
         for attack in self.ch.capec:
             self.process_item(attack)
             x += 1
 
-        self.logger.debug("Processed {} entries from file: {}".format(x, filename))
+        self.logger.debug(f"Processed {x} entries from file: {filename}")
 
         try:
-            self.logger.debug("Removing working dir: {}".format(working_dir))
+            self.logger.debug(f"Removing working dir: {working_dir}")
             shutil.rmtree(working_dir)
         except Exception as err:
-            self.logger.error(
-                "Failed to remove working dir; error produced: {}".format(err)
-            )
+            self.logger.error(f"Failed to remove working dir; error produced: {err}")
 
     def update(self, **kwargs):
         self.logger.info("CAPEC database update started")
 
         # if collection is non-existent; assume it's not an update
         if self.feed_type.lower() not in self.getTableNames():
             self.is_update = False
 
-        self.process_downloads([self.feed_url])
-
-        self.logger.info("Finished CAPEC database update")
+        if self.source_changed(self.feed_url):
+            self.process_downloads([self.feed_url])
+            self.logger.info("Finished CAPEC database update")
+        else:
+            self.logger.info("Skipped CAPEC database update")
 
         return self.last_modified
 
     def populate(self, **kwargs):
         self.is_update = False
         self.queue.clear()
 
@@ -1029,19 +958,17 @@
 class CWEDownloads(XMLFileHandler):
     """
     Class processing CWE source files
     """
 
     def __init__(self):
         self.feed_type = "CWE"
-        super().__init__(self.feed_type)
-
-        self.feed_url = Configuration.getFeedURL(self.feed_type.lower())
+        super().__init__(feed_type=self.feed_type, logger_name=__name__)
 
-        self.logger = logging.getLogger("CWEDownloads")
+        self.feed_url = self.config.SOURCES[self.feed_type.lower()]
 
         # make parser
         self.parser = make_parser()
         self.ch = CWEHandler()
         self.parser.setContentHandler(self.ch)
 
     def file_to_queue(self, file_tuple: Tuple[str, str]):
@@ -1051,166 +978,104 @@
             filename = f
 
         self.parser.parse(f"file://{filename}")
         x = 0
         for cwe in self.ch.cwe:
             try:
                 cwe["related_weaknesses"] = list(set(cwe["related_weaknesses"]))
+                cwe["description"] = cwe["Description"]
+                cwe.pop("Description")
             except KeyError:
                 pass
             self.process_item(cwe)
             x += 1
 
-        self.logger.debug("Processed {} entries from file: {}".format(x, filename))
+        self.logger.debug(f"Processed {x} entries from file: {filename}")
 
         try:
-            self.logger.debug("Removing working dir: {}".format(working_dir))
+            self.logger.debug(f"Removing working dir: {working_dir}")
             shutil.rmtree(working_dir)
         except Exception as err:
-            self.logger.error(
-                "Failed to remove working dir; error produced: {}".format(err)
-            )
+            self.logger.error(f"Failed to remove working dir; error produced: {err}")
 
     def update(self, **kwargs):
         self.logger.info("CWE database update started")
 
         # if collection is non-existent; assume it's not an update
         if self.feed_type.lower() not in self.getTableNames():
             self.is_update = False
 
-        self.process_downloads([self.feed_url])
-
-        self.logger.info("Finished CWE database update")
+        if self.source_changed(self.feed_url):
+            self.process_downloads([self.feed_url])
+            self.logger.info("Finished CWE database update")
+        else:
+            self.logger.info("Skipped CWE database update")
 
         return self.last_modified
 
     def populate(self, **kwargs):
         self.is_update = False
         self.queue.clear()
 
         self.delColInfo(self.feed_type.lower())
 
         self.dropCollection(self.feed_type.lower())
 
         return self.update()
 
 
-MongoUniqueIndex = namedtuple("MongoUniqueIndex", "index name unique")
-MongoAddIndex = namedtuple("MongoAddIndex", "index name")
+class EPSSDownloads(CSVFileHandler):
+    def __init__(self):
+        self.feed_type = "EPSS"
+        self.delimiter = ","
+        super().__init__(
+            feed_type=self.feed_type, logger_name=__name__, delimiter=self.delimiter
+        )
 
+        self.feed_url = self.config.SOURCES[self.feed_type.lower()]
 
-class DatabaseIndexer(object):
-    """
-    Class processing the Mongodb indexes
-    """
+        self.is_update = True
 
-    def __init__(self):
-        database = MongoDBConnection(**json.loads(os.getenv("MONGODB_CON_DETAILS")))
-        self.database = database._dbclient
+    def process_epss_item(self, item=None):
+        if item is None:
+            return None
 
-        self.indexes = {
-            "cpe": [
-                MongoUniqueIndex(index=[("id", ASCENDING)], name="id", unique=True),
-                MongoAddIndex(index=[("vendor", ASCENDING)], name="vendor"),
-                MongoAddIndex(index=[("product", ASCENDING)], name="product"),
-                MongoAddIndex(index=[("cpeNameId", ASCENDING)], name="cpeNameId"),
-                MongoAddIndex(index=[("deprecated", ASCENDING)], name="deprecated"),
-                MongoAddIndex(index=[("cpeName", ASCENDING)], name="cpeName"),
-                MongoAddIndex(index=[("title", ASCENDING)], name="title"),
-            ],
-            "cpeother": [
-                MongoUniqueIndex(index=[("id", ASCENDING)], name="id", unique=True)
-            ],
-            "cves": [
-                MongoAddIndex(index=[("id", ASCENDING)], name="id"),
-                MongoAddIndex(
-                    index=[("vulnerable_configuration", ASCENDING)],
-                    name="vulnerable_configuration",
-                ),
-                MongoAddIndex(
-                    index=[("vulnerable_product", ASCENDING)], name="vulnerable_product"
-                ),
-                MongoAddIndex(index=[("modified", ASCENDING)], name="modified"),
-                MongoAddIndex(index=[("published", ASCENDING)], name="published"),
-                MongoAddIndex(index=[("lastModified", ASCENDING)], name="lastModified"),
-                MongoAddIndex(index=[("cvss", ASCENDING)], name="cvss"),
-                MongoAddIndex(index=[("cvss3", ASCENDING)], name="cvss3"),
-                MongoAddIndex(index=[("summary", TEXT)], name="summary"),
-                MongoAddIndex(index=[("vendors", ASCENDING)], name="vendors"),
-                MongoAddIndex(index=[("products", ASCENDING)], name="products"),
-                MongoAddIndex(index=[("assigner", ASCENDING)], name="assigner"),
-                MongoAddIndex(index=[("cwe", ASCENDING)], name="cwe"),
-                MongoAddIndex(index=[("status", ASCENDING)], name="status"),
-                MongoAddIndex(
-                    index=[("vulnerable_product_stems", ASCENDING)],
-                    name="vulnerable_product_stems",
-                ),
-                MongoAddIndex(
-                    index=[("vulnerable_configuration_stems", ASCENDING)],
-                    name="vulnerable_configuration_stems",
-                ),
-            ],
-            "via4": [MongoAddIndex(index=[("id", ASCENDING)], name="id")],
-            "mgmt_whitelist": [MongoAddIndex(index=[("id", ASCENDING)], name="id")],
-            "mgmt_blacklist": [MongoAddIndex(index=[("id", ASCENDING)], name="id")],
-            "capec": [
-                MongoAddIndex(
-                    index=[("related_weakness", ASCENDING)], name="related_weakness"
-                )
-            ],
+        epss = {
+            "id": item[0],
+            "epss": item[1],
+            "epssMetric": {"percentile": item[2], "lastModified": self.last_modified},
         }
 
-        self.logger = logging.getLogger("DatabaseIndexer")
+        return epss
 
-    def getInfo(self, collection: str):
-        return sanitize(self.database["info"].find_one({"db": collection}))
+    def process_item(self, item):
+        epss = self.process_epss_item(item)
 
-    def create_indexes(self, collection: str = None):
-        if collection is not None:
-            try:
-                for each in self.indexes[collection]:
-                    if isinstance(each, MongoUniqueIndex):
-                        self.setIndex(
-                            collection, each.index, name=each.name, unique=each.unique
-                        )
-                    elif isinstance(each, MongoAddIndex):
-                        self.setIndex(collection, each.index, name=each.name)
-            except KeyError:
-                # no specific index given, continue
-                self.logger.warning(
-                    "Could not find the requested collection: {}, skipping...".format(
-                        collection
-                    )
+        if epss is not None:
+            self.queue.put(
+                DatabaseAction(
+                    action=DatabaseAction.actions.UpdateOne,
+                    doc=epss,
                 )
-                pass
+            )
 
-        else:
-            for index in self.iter_indexes():
-                self.setIndex(index[0], index[1])
+    def update(self, **kwargs):
+        self.logger.info("EPSS database update started")
 
-            for collection in self.indexes.keys():
-                for each in self.indexes[collection]:
-                    if isinstance(each, MongoUniqueIndex):
-                        self.setIndex(
-                            collection, each.index, name=each.name, unique=each.unique
-                        )
-                    elif isinstance(each, MongoAddIndex):
-                        self.setIndex(collection, each.index, name=each.name)
+        self.queue.clear()
 
-    def iter_indexes(self):
-        for each in self.get_via4_indexes():
-            yield each
-
-    def get_via4_indexes(self):
-        via4 = self.getInfo("via4")
-        result = []
-        if via4:
-            for index in via4.get("searchables", []):
-                result.append(("via4", index))
-        return result
+        self.process_downloads([self.feed_url])
 
-    def setIndex(self, col: str, field: str, **kwargs):
-        try:
-            self.database[col].create_index(field, **kwargs)
-            self.logger.info("Success to create index %s on %s" % (field, col))
-        except Exception as e:
-            self.logger.error("Failed to create index %s on %s: %s" % (col, field, e))
+        self.logger.info("Finished EPSS database update")
+
+        return self.last_modified
+
+    def populate(self, **kwargs):
+        self.logger.info("EPSS Database population started")
+
+        self.queue.clear()
+
+        self.process_downloads([self.feed_url])
+
+        self.logger.info("Finished EPSS database population")
+
+        return self.last_modified
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/content_handlers.py` & `CveXplore-6561581/CveXplore/core/database_maintenance/content_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 XML Content Handlers
 ====================
 """
+
 from collections import defaultdict
 from xml.sax.handler import ContentHandler
 
 
 class CapecHandler(ContentHandler):
     """
     Class handling the CAPEC XML parsing
@@ -217,37 +218,29 @@
             cut_entry = entry_id.split(".")
 
             url = ""
 
             if self.taxonomy_name == "ATTACK":
                 if len(cut_entry) == 1:
                     # no subtechnique use plain entry_id
-                    url = "https://attack.mitre.org/techniques/T{}".format(entry_id)
+                    url = f"https://attack.mitre.org/techniques/T{entry_id}"
                 else:
                     # attack with subtechniques use cut_entry
-                    url = "https://attack.mitre.org/techniques/T{}/{}".format(
-                        cut_entry[0], cut_entry[1]
-                    )
+                    url = f"https://attack.mitre.org/techniques/T{cut_entry[0]}/{cut_entry[1]}"
 
             elif self.taxonomy_name == "WASC":
                 if "/" in self.entry_name_ch:
-                    url = "http://projects.webappsec.org/{}".format(
-                        self.entry_name_ch.replace("/", " and ").replace(" ", "-")
-                    )
+                    url = f"http://projects.webappsec.org/{self.entry_name_ch.replace('/', ' and ').replace(' ', '-')}"
                 else:
-                    url = "http://projects.webappsec.org/{}".format(
-                        self.entry_name_ch.replace(" ", "-")
-                    )
+                    url = f"http://projects.webappsec.org/{self.entry_name_ch.replace(' ', '-')}"
 
             elif self.taxonomy_name == "OWASP Attacks":
                 entry_id = "Link"
 
-                url = "https://owasp.org/www-community/attacks/{}".format(
-                    self.entry_name_ch.replace(" ", "_")
-                )
+                url = f"https://owasp.org/www-community/attacks/{self.entry_name_ch.replace(' ', '_')}"
 
             self.taxonomy_mapping[self.taxonomy_name][
                 self.entry_id_ch.rstrip().replace(".", "_")
             ] = {
                 "Entry_ID": entry_id,
                 "Entry_Name": self.entry_name_ch.rstrip(),
                 "URL": url,
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/db_action.py` & `CveXplore-6561581/CveXplore/core/database_actions/db_action.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 
 from pymongo import InsertOne, UpdateOne
 
 
 class DatabaseAction(object):
     actions = collections.namedtuple("Actions", "InsertOne UpdateOne")(0, 1)
 
-    def __init__(self, action: actions, collection: str, doc: dict):
+    def __init__(self, action: actions, doc: dict):
         self.action = action
-        self.collection = collection
         self.doc = doc
 
     @property
     def entry(self):
         if self.action == self.actions.InsertOne:
             return InsertOne(self.doc)
         elif self.action == self.actions.UpdateOne:
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/file_handlers.py` & `CveXplore-6561581/CveXplore/core/database_maintenance/file_handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """
 File Handlers
 =============
 """
+
+import csv
 import shutil
 from abc import abstractmethod
 from typing import Tuple
 
-from CveXplore.database.maintenance.DownloadHandler import DownloadHandler
-from CveXplore.database.maintenance.IJSONHandler import IJSONHandler
-from CveXplore.database.maintenance.db_action import DatabaseAction
+from CveXplore.core.database_actions.db_action import DatabaseAction
+from CveXplore.core.database_maintenance.download_handler import DownloadHandler
+from CveXplore.core.database_maintenance.ijson_handler import IJSONHandler
 
 
 class JSONFileHandler(DownloadHandler):
     """
     This class handles all JSON related download processing and functions as a base class for specific JSON sources
     processing and downloading
     """
 
-    def __init__(self, feed_type: str, prefix: str):
-        super().__init__(feed_type)
+    def __init__(self, feed_type: str, prefix: str, logger_name: str):
+        super().__init__(feed_type=feed_type, prefix=prefix, logger_name=logger_name)
 
         self.is_update = True
 
         self.prefix = prefix
 
         self.ijson_handler = IJSONHandler()
 
-    def __repr__(self):
-        """return string representation of object"""
-        return "<< JSONFileHandler:{} >>".format(self.feed_type)
-
     def file_to_queue(self, file_tuple: Tuple[str, str]):
         """
         Method responsible for transferring file contents to the worker queue for further processing and inserting them
         into the database
         """
 
         working_dir, filename = file_tuple
@@ -41,30 +39,26 @@
         # adjust the interval counter for debug logging when updating
         if self.is_update:
             interval = 500
         else:
             interval = 5000
 
         x = 0
-        self.logger.debug("Starting processing of file: {}".format(filename))
+        self.logger.debug(f"Starting processing of file: {filename}")
         for cpe in self.ijson_handler.fetch(filename=filename, prefix=self.prefix):
             self.process_item(item=cpe)
             x += 1
             if x % interval == 0:
-                self.logger.debug(
-                    "Processed {} entries from file: {}".format(x, filename)
-                )
+                self.logger.debug(f"Processed {x} entries from file: {filename}")
 
         try:
-            self.logger.debug("Removing working dir: {}".format(working_dir))
+            self.logger.debug(f"Removing working dir: {working_dir}")
             shutil.rmtree(working_dir)
         except Exception as err:
-            self.logger.error(
-                "Failed to remove working dir; error produced: {}".format(err)
-            )
+            self.logger.error(f"Failed to remove working dir; error produced: {err}")
 
     @abstractmethod
     def update(self, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def populate(self, **kwargs):
@@ -73,48 +67,90 @@
 
 class XMLFileHandler(DownloadHandler):
     """
     This class handles all XML related download processing and functions as a base class for specific XML sources
     processing and downloading
     """
 
-    def __init__(self, feed_type: str):
-        super().__init__(feed_type)
+    def __init__(self, feed_type: str, logger_name: str):
+        super().__init__(feed_type=feed_type, logger_name=logger_name)
         self.is_update = True
 
-    def __repr__(self):
-        """return string representation of object"""
-        return "<< XMLFileHandler:{} >>".format(self.feed_type)
-
     def process_item(self, item: dict):
         """
         Method responsible for putting items into the worker queue as database actions
         """
 
         if self.is_update:
             self.queue.put(
                 DatabaseAction(
                     action=DatabaseAction.actions.UpdateOne,
-                    collection=self.feed_type.lower(),
                     doc=item,
                 )
             )
         else:
             self.queue.put(
                 DatabaseAction(
                     action=DatabaseAction.actions.InsertOne,
-                    collection=self.feed_type.lower(),
                     doc=item,
                 )
             )
 
     @abstractmethod
     def file_to_queue(self, *args):
         raise NotImplementedError
 
     @abstractmethod
     def update(self, **kwargs):
         raise NotImplementedError
 
     @abstractmethod
     def populate(self, **kwargs):
+        raise NotImplementedError
+
+
+class CSVFileHandler(DownloadHandler):
+    def __init__(self, feed_type, logger_name: str, delimiter=","):
+        super().__init__(feed_type=feed_type, logger_name=logger_name)
+
+        self.is_update = True
+        self.delimiter = delimiter
+
+    def file_to_queue(self, file_tuple):
+        working_dir, filename = file_tuple
+
+        # adjust the interval counter for debug logging when updating
+        if self.is_update:
+            interval = 500
+        else:
+            interval = 5000
+
+        x = 0
+        self.logger.debug(f"Starting processing of file: {filename}")
+
+        f = open(filename, "r")
+
+        reader = csv.reader(f, delimiter=self.delimiter)
+
+        next(reader)
+        next(reader)
+
+        for row in reader:
+            self.process_item(item=row)
+            x += 1
+            if x % interval == 0:
+                self.logger.debug(f"Processed {x} entries from file: {filename}")
+        f.close()
+
+        try:
+            self.logger.debug(f"Removing working dir: {working_dir}")
+            shutil.rmtree(working_dir)
+        except Exception as err:
+            self.logger.error(f"Failed to remove working dir; error produced: {err}")
+
+    @abstractmethod
+    def update(self, **kwargs):
+        raise NotImplementedError
+
+    @abstractmethod
+    def populate(self, **kwargs):
         raise NotImplementedError
```

### Comparing `CveXplore-0.3.9/CveXplore/database/maintenance/worker_q.py` & `CveXplore-6561581/CveXplore/core/worker_queue/worker_q.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from queue import Empty, Queue
 
-from CveXplore.database.maintenance.db_action import DatabaseAction
+from CveXplore.core.database_actions.db_action import DatabaseAction
 
 
 class WorkerQueue(Queue):
     def __init__(self, name: str, maxsize: int = 0):
         super().__init__(maxsize)
         self.name = name
         self.maxsize = maxsize
 
         self.closed = False
 
     def __len__(self):
         self.qsize()
 
     def __repr__(self):
-        return "<< WorkerQueue:{} >>".format(self.name)
+        return f"<< WorkerQueue:{self.name} >>"
 
     def __iter__(self):
         return self
 
     def __next__(self):
         try:
             item = self.get(timeout=1)
```

### Comparing `CveXplore-0.3.9/CveXplore/main.py` & `CveXplore-6561581/CveXplore/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,107 +1,223 @@
 """
 Main
 ====
 """
+
+import os
+import shutil
+
+from dotenv import load_dotenv
+
+if not os.path.exists(os.path.expanduser("~/.cvexplore")):
+    os.mkdir(os.path.expanduser("~/.cvexplore"))
+
+user_wd = os.path.expanduser("~/.cvexplore")
+
+if not os.path.exists(os.path.join(user_wd, ".env")):
+    shutil.copyfile(
+        os.path.join(os.path.dirname(__file__), "common/.env_example"),
+        os.path.join(user_wd, ".env"),
+    )
+
+load_dotenv(os.path.join(user_wd, ".env"))
+
+if not os.path.exists(os.path.join(user_wd, ".sources.ini")):
+    shutil.copyfile(
+        os.path.join(os.path.dirname(__file__), "common/.sources.ini"),
+        os.path.join(user_wd, ".sources.ini"),
+    )
+
 import functools
 import json
-import os
+import logging
+
 import re
+import warnings
 from collections import defaultdict
-from typing import List, Tuple, Union, Iterable
+from typing import List, Tuple, Union, Iterable, Type
 
 from pymongo import DESCENDING
 
 from CveXplore.api.connection.api_db import ApiDatabaseSource
-from CveXplore.common.cpe_converters import from2to3CPE
+from CveXplore.common.config import Configuration
+from CveXplore.common.cpe_converters import create_cpe_regex_string
 from CveXplore.common.db_mapping import database_mapping
-from CveXplore.database.connection.mongo_db import MongoDBConnection
-from CveXplore.database.maintenance.main_updater import MainUpdater
+from CveXplore.core.database_maintenance.main_updater import MainUpdater
+from CveXplore.core.general.datasources import supported_datasources
+from CveXplore.database.connection.database_connection import DatabaseConnection
 from CveXplore.errors import DatabaseIllegalCollection
+from CveXplore.errors.datasource import UnsupportedDatasourceException
 from CveXplore.errors.validation import CveNumberValidationError
 from CveXplore.objects.cvexplore_object import CveXploreObject
 
+
 try:
     from version import VERSION
 except ModuleNotFoundError:
     _PKG_DIR = os.path.dirname(__file__)
     version_file = os.path.join(_PKG_DIR, "VERSION")
     with open(version_file, "r") as fdsec:
         VERSION = fdsec.read()
 
 
 class CveXplore(object):
     """
     Main class for CveXplore package
     """
 
-    def __init__(
-        self,
-        mongodb_connection_details: dict = None,
-        api_connection_details: dict = None,
-    ):
+    def __init__(self, **kwargs):
         """
         Create a new instance of CveXplore
-
+        :param datasource_type: Which datasource to query.
+        :param datasource_connection_details: Provide the connection details needed to establish a connection to the
+                                              datasource. The connection details should be in line with the datasource
+                                              it's documentation.
         :param mongodb_connection_details: Provide the connection details needed to establish a connection to a mongodb
                                            instance. The connection details should be in line with pymongo's
                                            documentation.
-        :type mongodb_connection_details: dict
         :param api_connection_details: Provide the connection details needed to establish a connection to a cve-search
                                        API provider. The cve-search API provider should allow access to the 'query' POST
                                        endpoint; all other API endpoints are not needed for CveXplore to function. For
                                        the connection details supported please check the :ref:`API connection <api>`
                                        documentation.
-        :type api_connection_details: dict
         """
         self.__version = VERSION
+        self._config = Configuration
+        self.logger = logging.getLogger(__name__)
+
+        # adjust self.config with kwargs parameters; lower case parameters are converted to uppercase and then changed
+        # in the self.config object
+        for each in kwargs:
+            setattr(self.config, each.upper(), kwargs[each])
+
+        self._datasource_type = self.config.DATASOURCE_TYPE
+
+        self._datasource_connection_details = self.config.DATASOURCE_CONNECTION_DETAILS
+
+        self._mongodb_connection_details = self.config.MONGODB_CONNECTION_DETAILS
+        self._api_connection_details = self.config.API_CONNECTION_DETAILS
 
         os.environ["DOC_BUILD"] = json.dumps({"DOC_BUILD": "NO"})
 
+        self.logger.info(
+            f"Using {self.datasource_type} as datasource, connection details: {self.datasource_connection_details}"
+        )
+
+        if self.datasource_type not in supported_datasources:
+            raise UnsupportedDatasourceException(
+                f"Unsupported datasource selected: '{self.datasource_type}'; currently supported: {supported_datasources}"
+            )
+
+        if self.datasource_type == "api" and self.datasource_connection_details is None:
+            raise ValueError(
+                "Missing datasource_connection_details for selected datasource ('api')"
+            )
+        elif self.datasource_type == "api":
+            self.datasource_connection_details["user_agent"] = (
+                f"CveXplore:{self.version}"
+            )
+
         if (
-            api_connection_details is not None
-            and mongodb_connection_details is not None
+            self.mongodb_connection_details is not None
+            and self.datasource_type == "mongodb"
         ):
-            raise ValueError(
-                "CveXplore can be used to connect to either a cve-search database OR a cve-search api, not both!"
+            self.logger.warning(
+                "The use of mongodb_connection_details is deprecated and will be removed in the 0.4 release, please "
+                "use datasource_connection_details instead"
+            )
+            self._datasource_connection_details = self.mongodb_connection_details
+        elif self.api_connection_details is not None and self.datasource_type == "api":
+            self.logger.warning(
+                "The use of api_connection_details is deprecated and will be removed in the 0.4 release, please "
+                "use datasource_connection_details instead"
             )
-        elif api_connection_details is None and mongodb_connection_details is None:
-            # by default assume we are talking to a database
-            mongodb_connection_details = {}
-            os.environ["MONGODB_CON_DETAILS"] = json.dumps(mongodb_connection_details)
-            self.datasource = MongoDBConnection(**mongodb_connection_details)
-            self.database = MainUpdater(datasource=self.datasource)
-        elif mongodb_connection_details is not None:
-            os.environ["MONGODB_CON_DETAILS"] = json.dumps(mongodb_connection_details)
-            self.datasource = MongoDBConnection(**mongodb_connection_details)
-            self.database = MainUpdater(datasource=self.datasource)
-        elif api_connection_details is not None:
-            api_connection_details["user_agent"] = "CveXplore:{}".format(self.version)
-            os.environ["API_CON_DETAILS"] = json.dumps(api_connection_details)
-            self.datasource = ApiDatabaseSource(**api_connection_details)
+            self._datasource_connection_details = self.api_connection_details
+        else:
+            if self.datasource_type == "mongodb":
+                self._datasource_connection_details = {
+                    "host": f"{self.config.DATASOURCE_PROTOCOL}://{self.config.DATASOURCE_HOST}:{self.config.DATASOURCE_PORT}"
+                }
+            elif self.datasource_type == "mysql":
+                self._datasource_connection_details = {
+                    "sql_uri": self.config.SQLALCHEMY_DATABASE_URI
+                }
+            elif self.datasource_type == "api":
+                self._datasource_connection_details = {
+                    "address": (
+                        f"{self.config.DATASOURCE_HOST}",
+                        int(f"{self.config.DATASOURCE_PORT}"),
+                    ),
+                    "api_path": "api",
+                }
+
+        setattr(
+            self.config,
+            "DATASOURCE_CONNECTION_DETAILS",
+            self.datasource_connection_details,
+        )
 
-        self.database_mapping = database_mapping
+        self.datasource = DatabaseConnection(
+            database_type=self.datasource_type,
+            database_init_parameters=self.datasource_connection_details,
+        ).database_connection
+        if self.datasource_type != "api":
+            self.database = MainUpdater(
+                datasource=self.datasource, datasource_type=self.datasource_type
+            )
+
+        self._database_mapping = database_mapping
 
-        from CveXplore.database.helpers.generic_db import GenericDatabaseFactory
         from CveXplore.database.helpers.specific_db import (
             CvesDatabaseFunctions,
             CpeDatabaseFunctions,
+            CapecDatabaseFunctions,
+            CWEDatabaseFunctions,
         )
 
-        for each in self.database_mapping:
-            try:
-                if each == "cves":
-                    setattr(self, each, CvesDatabaseFunctions(collection=each))
-                elif each == "cpe":
-                    setattr(self, each, CpeDatabaseFunctions(collection=each))
-                else:
-                    setattr(self, each, GenericDatabaseFactory(collection=each))
-            except KeyError:
-                # no specific or generic methods configured, skipping
-                continue
+        self.cves = CvesDatabaseFunctions(collection="cves")
+        self.cpe = CpeDatabaseFunctions(collection="cpe")
+        self.capec = CapecDatabaseFunctions(collection="capec")
+        self.cwe = CWEDatabaseFunctions(collection="cwe")
+
+        self.logger.info(f"Initialized CveXplore version: {self.version}")
+
+    @property
+    def config(self) -> Type[Configuration]:
+        return self._config
+
+    @property
+    def datasource_type(self) -> str:
+        return self._datasource_type
+
+    @property
+    def datasource_connection_details(self) -> dict:
+        return self._datasource_connection_details
+
+    @property
+    def database_mapping(self) -> dict:
+        return self._database_mapping
+
+    @property
+    def mongodb_connection_details(self) -> dict:
+        warnings.warn(
+            "The use of mongodb_connection_details is deprecated and will be removed in the 0.4 release, "
+            "please use datasource_connection_details instead",
+            DeprecationWarning,
+        )
+        return self._mongodb_connection_details
+
+    @property
+    def api_connection_details(self) -> dict:
+        warnings.warn(
+            "The use of api_connection_details is deprecated and will be removed in the 0.4 release, please "
+            "use datasource_connection_details instead",
+            DeprecationWarning,
+        )
+        return self._api_connection_details
 
     def get_single_store_entry(
         self, entry_type: str, dict_filter: dict = None
     ) -> CveXploreObject | None:
         """
         Method to perform a query on a *single* collection in the data source and return a *single* result.
 
@@ -116,22 +232,18 @@
         if dict_filter is None:
             dict_filter = {}
 
         entry_type = entry_type.lower()
 
         if entry_type not in self.database_mapping:
             raise DatabaseIllegalCollection(
-                "Illegal collection requested: only {} are allowed!".format(
-                    self.database_mapping
-                )
+                f"Illegal collection requested: only {self.database_mapping} are allowed!"
             )
 
-        result = getattr(self.datasource, "store_{}".format(entry_type)).find_one(
-            dict_filter
-        )
+        result = getattr(self.datasource, f"store_{entry_type}").find_one(dict_filter)
 
         return result
 
     def get_single_store_entries(
         self, query: Tuple[str, dict], limit: int = 10
     ) -> List[CveXploreObject] | None:
         """
@@ -140,43 +252,80 @@
         Tuple which contains the entry_type and the dict_filter in a tuple.
             Choices for entry_type:
                 - capec;
                 - cpe;
                 - cwe;
                 - via4;
                 - cves;
+
             dict_filter is a dictionary representing a filter according to pymongo documentation.
+
             example:
                 get_single_store_entries(("cwe", {"id": "78"}))
         """
         if not isinstance(query, tuple):
             raise ValueError(
-                "Wrong parameter type, received: {} expected: tuple".format(type(query))
+                f"Wrong parameter type, received: {type(query)} expected: tuple"
             )
 
         if len(query) != 2:
             raise ValueError(
-                "Query parameter does not consist of the expected amount of variables, expected: 2 received: {}".format(
-                    len(query)
-                )
+                f"Query parameter does not consist of the expected amount of variables, "
+                f"expected: 2 received: {len(query)}"
             )
 
         entry_type, dict_filter = query
 
         entry_type = entry_type.lower()
 
         if entry_type not in self.database_mapping:
             raise DatabaseIllegalCollection(
-                "Illegal collection requested: only {} are allowed!".format(
-                    self.database_mapping
-                )
+                f"Illegal collection requested: only {self.database_mapping} are allowed!"
             )
 
+        if entry_type == "cves":
+            if "id" in dict_filter:
+                if isinstance(dict_filter["id"], str):
+                    dict_filter["id"] = self._validate_cve_id(dict_filter["id"])
+                elif isinstance(dict_filter["id"], dict):
+                    if "$in" in dict_filter["id"]:
+                        dict_filter["id"]["$in"] = [
+                            self._validate_cve_id(x) for x in dict_filter["id"]["$in"]
+                        ]
+            if "cvss" in dict_filter:
+                if isinstance(dict_filter["cvss"], str):
+                    dict_filter["cvss"] = float(dict_filter["cvss"])
+            if "cvss3" in dict_filter:
+                if isinstance(dict_filter["cvss3"], str):
+                    dict_filter["cvss3"] = float(dict_filter["cvss3"])
+
+            if "exploitabilityScore" in dict_filter:
+                if isinstance(dict_filter["exploitabilityScore"], str):
+                    dict_filter["exploitabilityScore"] = float(
+                        dict_filter["exploitabilityScore"]
+                    )
+            if "exploitabilityScore3" in dict_filter:
+                if isinstance(dict_filter["exploitabilityScore3"], str):
+                    dict_filter["exploitabilityScore3"] = float(
+                        dict_filter["exploitabilityScore3"]
+                    )
+
+            if "impactScore" in dict_filter:
+                if isinstance(dict_filter["impactScore"], str):
+                    dict_filter["impactScore"] = float(dict_filter["impactScore"])
+            if "impactScore3" in dict_filter:
+                if isinstance(dict_filter["impactScore3"], str):
+                    dict_filter["impactScore3"] = float(dict_filter["impactScore3"])
+
+            if "epss" in dict_filter:
+                if isinstance(dict_filter["epss"], str):
+                    dict_filter["epss"] = float(dict_filter["epss"])
+
         results = (
-            getattr(self.datasource, "store_{}".format(entry_type))
+            getattr(self.datasource, f"store_{entry_type}")
             .find(dict_filter)
             .limit(limit)
         )
 
         the_results = list(results)
 
         if len(the_results) != 0:
@@ -194,84 +343,76 @@
         A list of tuples which contains the entry_type and the dict_filter.
             Choices for entry_type:
                 - capec;
                 - cpe;
                 - cwe;
                 - via4;
                 - cves;
+
             dict_filter is a dictionary representing a filter according to pymongo documentation.
+
             example:
                 get_multi_store_entries([("cwe", {"id": "78"}), ("cves", {"id": "CVE-2009-0018"})])
         """
 
         results = map(
             functools.partial(self.get_single_store_entries, limit=limit), *queries
         )
 
-        joined_list = []
+        the_results = [
+            result_list for result_list in results if result_list is not None
+        ]
 
-        for result_list in results:
-            joined_list += result_list
-
-        the_results = list(joined_list)
+        # flatten results
+        the_results = [item for row in the_results for item in row]
 
         if len(the_results) != 0:
             return the_results
         else:
             return None
 
     def cves_for_cpe(self, cpe_string: str) -> List[CveXploreObject] | None:
         """
         Method for retrieving Cves that match a single CPE string. By default, the search will be made matching
         the configuration fields of the cves documents.
         CPE string could be formatted like: ``cpe:2.3:o:microsoft:windows_7:*:sp1:*:*:*:*:*:*``
         """
 
-        # format to cpe2.3
-        cpe_string = from2to3CPE(cpe_string)
-
-        if cpe_string.startswith("cpe"):
-            # strict search with term starting with cpe; e.g: cpe:2.3:o:microsoft:windows_7:*:sp1:*:*:*:*:*:*
-
-            remove_trailing_regex_stars = r"(?:\:|\:\:|\:\*)+$"
-
-            cpe_regex = re.escape(re.sub(remove_trailing_regex_stars, "", cpe_string))
-
-            cpe_regex_string = r"^{}:".format(cpe_regex)
-        else:
-            # more general search on same field; e.g. microsoft:windows_7
-            cpe_regex_string = "{}".format(re.escape(cpe_string))
+        cpe_regex_string = create_cpe_regex_string(cpe_string)
 
         cves = self.get_single_store_entries(
             ("cves", {"vulnerable_configuration": {"$regex": cpe_regex_string}}),
             limit=0,
         )
 
         return cves
 
-    def cve_by_id(self, cve_id: str) -> CveXploreObject | None:
-        """
-        Method to retrieve a single CVE from the database by its CVE ID number.
-        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
-        """
-
-        # first try to match full cve number format
+    def _validate_cve_id(self, cve_id: str):
         reg_match = re.compile(r"[cC][vV][eE]-\d{4}-\d{4,10}")
         if reg_match.match(cve_id) is not None:
             cve_id = cve_id.upper()
         else:
             part_match = re.compile(r"\d{4}-\d{4,10}")
             if part_match.match(cve_id) is not None:
                 cve_id = f"CVE-{cve_id}"
             else:
                 raise CveNumberValidationError(
-                    "Could not validate the CVE number. The number format should be either "
+                    f"Could not validate the CVE number: {cve_id}. The number format should be either "
                     "CVE-2000-0001, cve-2000-0001 or 2000-0001."
                 )
 
+        return cve_id
+
+    def cve_by_id(self, cve_id: str) -> CveXploreObject | None:
+        """
+        Method to retrieve a single CVE from the database by its CVE ID number.
+        The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
+        """
+        cve_id = self._validate_cve_id(cve_id=cve_id)
+
         return self.get_single_store_entry("cves", {"id": cve_id})
 
     def cves_by_id(self, *cve_ids: str) -> Union[Iterable[CveXploreObject], Iterable]:
         """
         Method to retrieve a multiple CVE's from the database by its CVE ID number.
         The number format should be either CVE-2000-0001, cve-2000-0001 or 2000-0001.
         """
@@ -325,41 +466,44 @@
 
         if not isinstance(self.datasource, ApiDatabaseSource):
             if hasattr(self.datasource, "store_info"):
                 results = self.datasource.store_info.find({})
                 for each in results:
                     each.pop("_id")
                     db = each["db"]
+                    if db == "epss":
+                        continue
+
                     each.pop("db")
 
                     if "sources" in each:
                         each.pop("sources")
                         each.pop("searchables")
 
                     each["lastModified"] = str(each["lastModified"])
                     each["document count"] = getattr(
-                        self.datasource, "store_{}".format(db)
+                        self.datasource, f"store_{db}"
                     ).count_documents({})
                     stats[db] = each
 
                     for mgmtlist in ["mgmt_blacklist", "mgmt_whitelist"]:
                         stats[mgmtlist] = {
                             "document count": getattr(
-                                self.datasource, "store_{}".format(mgmtlist)
+                                self.datasource, f"store_{mgmtlist}"
                             ).count_documents({})
                         }
 
                 return dict(stats)
 
             else:
                 return "Database info could not be retrieved"
 
-        return "Using api endpoint: {}".format(self.datasource.baseurl)
+        return f"Using api endpoint: {self.datasource.baseurl}"
 
     @property
-    def version(self):
+    def version(self) -> str:
         """Property returning current version"""
         return self.__version
 
     def __repr__(self):
         """String representation of object"""
-        return "<< CveXplore:{} >>".format(self.version)
+        return f"<< CveXplore:{self.version} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/objects/capec.py` & `CveXplore-6561581/CveXplore/objects/capec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 capec
 =====
 """
+
 from CveXplore.common.data_source_connection import DatasourceConnection
 
 
 class Capec(DatasourceConnection):
     """
     Capec database object
     """
@@ -22,15 +23,15 @@
 
         :return: Cwe object
         :rtype: Cwe
         """
         if hasattr(self, "related_weakness"):
             if len(self.related_weakness) != 0:
                 for each in self.related_weakness:
-                    cwe_doc = self._datasource_connection.store_cwe.find_one(
+                    cwe_doc = self.datasource_connection.store_cwe.find_one(
                         {"id": each}
                     )
 
                     yield cwe_doc
 
     def iter_related_capecs(self):
         """
@@ -38,16 +39,16 @@
 
         :return: Capec objects
         :rtype: Capec
         """
         if hasattr(self, "related_capecs"):
             if len(self.related_capecs) != 0:
                 for each in self.related_capecs:
-                    capec_doc = self._datasource_connection.store_capec.find_one(
+                    capec_doc = self.datasource_connection.store_capec.find_one(
                         {"id": each}
                     )
 
                     yield capec_doc
 
     def __repr__(self):
         """String representation of object"""
-        return "<< Capec:{} >>".format(self.id)
+        return f"<< Capec:{self.id} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/objects/cpe.py` & `CveXplore-6561581/CveXplore/objects/cpe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 cpe
 ===
 """
-import re
 
 from pymongo import DESCENDING
 
-from CveXplore.common.cpe_converters import from2to3CPE
+from CveXplore.common.cpe_converters import create_cpe_regex_string
 from CveXplore.common.data_source_connection import DatasourceConnection
 
 
 class Cpe(DatasourceConnection):
     """
     Cpe database object
     """
@@ -27,30 +26,17 @@
         the configuration fields of the cves documents.
         """
 
         cpe_searchField = (
             "vulnerable_product" if vuln_prod_search else "vulnerable_configuration"
         )
 
-        # format to cpe2.3
-        cpe_string = from2to3CPE(self.cpeName)
+        cpe_regex_string = create_cpe_regex_string(self.cpeName)
 
-        if cpe_string.startswith("cpe"):
-            # strict search with term starting with cpe; e.g: cpe:2.3:o:microsoft:windows_7:*:sp1:*:*:*:*:*:*
-
-            remove_trailing_regex_stars = r"(?:\:|\:\:|\:\*)+$"
-
-            cpe_regex = re.escape(re.sub(remove_trailing_regex_stars, "", cpe_string))
-
-            cpe_regex_string = r"^{}:".format(cpe_regex)
-        else:
-            # more general search on same field; e.g. microsoft:windows_7
-            cpe_regex_string = "{}".format(re.escape(cpe_string))
-
-        results = self._datasource_connection.store_cves.find(
+        results = self.datasource_connection.store_cves.find(
             {cpe_searchField: {"$regex": cpe_regex_string}}
         ).sort("cvss", DESCENDING)
 
         for each in results:
             if each is not None:
                 yield each
             else:
@@ -77,8 +63,8 @@
         data_cpe = self.to_dict()
         data_cpe["cvecount"] = len(data_cves)
         data_cpe["cves"] = data_cves
         return data_cpe
 
     def __repr__(self):
         """String representation of object"""
-        return "<< Cpe:{} >>".format(self.id)
+        return f"<< Cpe:{self.id} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/objects/cves.py` & `CveXplore-6561581/CveXplore/objects/cves.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 cves
 ====
 """
+
 import datetime
 
 from CveXplore.common.data_source_connection import DatasourceConnection
 
 
 class Cves(DatasourceConnection):
     """
@@ -22,28 +23,28 @@
             if isinstance(self.cwe, str):
                 if self.cwe.lower() != "unknown":
                     cwe_id = self.cwe[4:]
                     # check if cwe_id can be cast to int
                     try:
                         if int(cwe_id):
                             results = getattr(
-                                self._datasource_connection, "store_{}".format("cwe")
+                                self.datasource_connection, "store_cwe"
                             ).find_one({"id": cwe_id})
                             if results is not None:
                                 self.cwe = results
                     except ValueError:
                         pass
 
-                    capecs = self._datasource_connection.store_capec.find(
+                    capecs = self.datasource_connection.store_capec.find(
                         {"related_weakness": {"$in": [cwe_id]}}
                     )
 
                     setattr(self, "capec", list(capecs))
 
-        via4s = self._datasource_connection.store_via4.find_one({"id": self.id})
+        via4s = self.datasource_connection.store_via4.find_one({"id": self.id})
 
         if via4s is not None:
             setattr(self, "via4_references", via4s)
 
     def iter_vuln_configurations(self):
         """
         Generator function for iterating over vulnerable configurations for this CVE.
@@ -109,8 +110,8 @@
             if isinstance(v, datetime.datetime):
                 full_dict[k] = str(v)
 
         return full_dict
 
     def __repr__(self):
         """String representation of object"""
-        return "<< Cves:{} >>".format(self.id)
+        return f"<< Cves:{self.id} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore/objects/cwe.py` & `CveXplore-6561581/CveXplore/objects/cwe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 cwe
 ===
 """
+
 from CveXplore.common.data_source_connection import DatasourceConnection
 
 
 class Cwe(DatasourceConnection):
     """
     Cwe database object
     """
@@ -22,31 +23,31 @@
 
         :return: Cwe object
         :rtype: Cwe
         """
         if hasattr(self, "related_weaknesses"):
             if len(self.related_weaknesses) != 0:
                 for each in self.related_weaknesses:
-                    cwe_doc = self._datasource_connection.store_cwe.find_one(
+                    cwe_doc = self.datasource_connection.store_cwe.find_one(
                         {"id": each}
                     )
 
                     yield cwe_doc
 
     def iter_related_capecs(self):
         """
          Generator function for iterating the related capecs from the current weakness object
 
         :return: Capec object
         :rtype: Capec
         """
 
-        related_capecs = self._datasource_connection.store_capec.find(
+        related_capecs = self.datasource_connection.store_capec.find(
             {"related_weakness": self.id}
         )
 
         for each in related_capecs:
             yield each
 
     def __repr__(self):
         """String representation of object"""
-        return "<< Cwe:{} >>".format(self.id)
+        return f"<< Cwe:{self.id} >>"
```

### Comparing `CveXplore-0.3.9/CveXplore.egg-info/PKG-INFO` & `CveXplore-6561581/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,23 @@
-Metadata-Version: 2.1
-Name: CveXplore
-Version: 0.3.9
-Summary: Package for interacting with cve-search
-Home-page: https://github.com/cve-search/CveXplore
-Author: Paul Tikken
-Author-email: paul.tikken@gmail.com
-License: GNU General Public License v3.0
-Project-URL: Documentation, https://cve-search.github.io/CveXplore/
-Project-URL: Issues, https://github.com/cve-search/CveXplore/issues
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
+.. image:: images/CveExplore_logo.png
 
+.. Everything after the include marker below is inserted into the sphinx html docs. Everything above this comment is only visible in the github README.rst ##INCLUDE_MARKER##
 
 .. image:: https://img.shields.io/github/release/cve-search/CveXplore.svg
    :target: https://GitHub.com/cve-search/CveXplore/releases/
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
 
 .. image:: https://badgen.net/badge/Github/repo/green?icon=github
    :target: https://GitHub.com/cve-search/CveXplore
 
 
 The CveXplore package aims to provide an object related way to interact with the data collected or hosted by a
-cve-search instance. It provides an ambiguous way to interact either to the cve-search mongodb or to the cve-search API.
+cve-search instance. It provides an ambiguous way to interact with either the cve-search mongodb or the cve-search API.
 
 From version 0.2.5 onwards CveXplore has the possibility to initialize and update the database without the need of any of
 the cve-search binaries and thus providing the same functionality as cve-search but without the GUI components.
 
 A click command line functionality is being build but for now still in progress...
 
 All the data provided by this interaction is converted into objects before being returned. And thus providing a way to
@@ -54,20 +35,41 @@
 
 Both of them can be easily created on a physical machine or via a docker instance of cve-search;
 please check `cve-search <https://github.com/cve-search/cve-search>`_ or
 `CVE-Search-Docker <https://github.com/cve-search/CVE-Search-Docker>`_ for further details.
 
 Installation
 ------------
-Package is hosted on pypi, so just run:
+Package is hosted on pypi, so to install the minimal core just run:
 
 .. code-block:: bash
 
    pip install CveXplore
 
+This command will install the core logic of CveXplore and, by default, installs the mongodb module also.
+
+CveXplore is setup in a modular way and therefor has multiple modules which can be installed separately by specifying
+them as an extra requirement. To install the mysql module only, specify:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql]
+
+Or for multiple modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql, redis]
+
+Or simple install all modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[all]
+
 Documentation
 -------------
 Check `github pages documentation <https://cve-search.github.io/CveXplore/>`_
 
 General
 -------
 
@@ -126,24 +128,24 @@
    '0.1.2'
 
 To let CveXplore connect to an mongodb with specific parameters:
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(mongodb_connection_details={"host": "192.168.1.1", "port": 27017})
+   >>> cvx = CveXplore(datasource_type="mongodb", datasource_connection_details={"host": "mongodb://127.0.0.1:27017"})
    >>> cvx.version
    '0.1.2'
 
 And to let CveXplore talk to an Cve Search API (only query POST endpoint needed):
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(api_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
+   >>> cvx = CveXplore(datasource_type="api", datasource_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
    >>> cvx.version
    '0.1.2'
 
 Query for data
 **************
 CveXplore supports multiple methods to query for data.
```

### Comparing `CveXplore-0.3.9/LICENSE` & `CveXplore-6561581/LICENSE`

 * *Files identical despite different names*

### Comparing `CveXplore-0.3.9/PKG-INFO` & `CveXplore-6561581/CveXplore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,85 @@
 Metadata-Version: 2.1
 Name: CveXplore
-Version: 0.3.9
+Version: 6561581
 Summary: Package for interacting with cve-search
 Home-page: https://github.com/cve-search/CveXplore
 Author: Paul Tikken
 Author-email: paul.tikken@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Documentation, https://cve-search.github.io/CveXplore/
 Project-URL: Issues, https://github.com/cve-search/CveXplore/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3>=2.0.6
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: click==8.1.7
+Requires-Dist: click-completion==0.5.2
+Requires-Dist: ijson>=3.2.3
+Requires-Dist: ansicolors==1.1.8
+Requires-Dist: pygelf>=0.4.2
+Requires-Dist: pandas>=2.1.2
+Requires-Dist: dicttoxml==1.7.16
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: aiohttp>=3.8.6
+Requires-Dist: aioretry>=5.0.2
+Requires-Dist: pymongo>=4.5.0
+Provides-Extra: mysql
+Requires-Dist: sqlalchemy>=2.0.23; extra == "mysql"
+Requires-Dist: alembic>=1.13.0; extra == "mysql"
+Requires-Dist: PyMySQL>=1.1.0; extra == "mysql"
+Provides-Extra: kafka
+Provides-Extra: sqllite
+Requires-Dist: sqlalchemy>=2.0.23; extra == "sqllite"
+Requires-Dist: alembic>=1.13.0; extra == "sqllite"
+Provides-Extra: redis
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy>=2.0.23; extra == "sqlalchemy"
+Requires-Dist: alembic>=1.13.0; extra == "sqlalchemy"
+Provides-Extra: mongodb
+Requires-Dist: pymongo>=4.5.0; extra == "mongodb"
+Provides-Extra: docs
+Requires-Dist: sphinx==7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=1.25.2; extra == "docs"
+Provides-Extra: postgres
+Requires-Dist: sqlalchemy>=2.0.23; extra == "postgres"
+Requires-Dist: alembic>=1.13.0; extra == "postgres"
+Provides-Extra: all
+Requires-Dist: pymongo>=4.5.0; extra == "all"
+Requires-Dist: alembic>=1.13.0; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.23; extra == "all"
+Requires-Dist: sphinx==7.2.6; extra == "all"
+Requires-Dist: sphinx-autodoc-typehints>=1.25.2; extra == "all"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "all"
+Requires-Dist: PyMySQL>=1.1.0; extra == "all"
 
 
 
 .. image:: https://img.shields.io/github/release/cve-search/CveXplore.svg
    :target: https://GitHub.com/cve-search/CveXplore/releases/
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
 
 .. image:: https://badgen.net/badge/Github/repo/green?icon=github
    :target: https://GitHub.com/cve-search/CveXplore
 
 
 The CveXplore package aims to provide an object related way to interact with the data collected or hosted by a
-cve-search instance. It provides an ambiguous way to interact either to the cve-search mongodb or to the cve-search API.
+cve-search instance. It provides an ambiguous way to interact with either the cve-search mongodb or the cve-search API.
 
 From version 0.2.5 onwards CveXplore has the possibility to initialize and update the database without the need of any of
 the cve-search binaries and thus providing the same functionality as cve-search but without the GUI components.
 
 A click command line functionality is being build but for now still in progress...
 
 All the data provided by this interaction is converted into objects before being returned. And thus providing a way to
@@ -54,20 +97,41 @@
 
 Both of them can be easily created on a physical machine or via a docker instance of cve-search;
 please check `cve-search <https://github.com/cve-search/cve-search>`_ or
 `CVE-Search-Docker <https://github.com/cve-search/CVE-Search-Docker>`_ for further details.
 
 Installation
 ------------
-Package is hosted on pypi, so just run:
+Package is hosted on pypi, so to install the minimal core just run:
 
 .. code-block:: bash
 
    pip install CveXplore
 
+This command will install the core logic of CveXplore and, by default, installs the mongodb module also.
+
+CveXplore is setup in a modular way and therefor has multiple modules which can be installed separately by specifying
+them as an extra requirement. To install the mysql module only, specify:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql]
+
+Or for multiple modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql, redis]
+
+Or simple install all modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[all]
+
 Documentation
 -------------
 Check `github pages documentation <https://cve-search.github.io/CveXplore/>`_
 
 General
 -------
 
@@ -126,24 +190,24 @@
    '0.1.2'
 
 To let CveXplore connect to an mongodb with specific parameters:
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(mongodb_connection_details={"host": "192.168.1.1", "port": 27017})
+   >>> cvx = CveXplore(datasource_type="mongodb", datasource_connection_details={"host": "mongodb://127.0.0.1:27017"})
    >>> cvx.version
    '0.1.2'
 
 And to let CveXplore talk to an Cve Search API (only query POST endpoint needed):
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(api_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
+   >>> cvx = CveXplore(datasource_type="api", datasource_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
    >>> cvx.version
    '0.1.2'
 
 Query for data
 **************
 CveXplore supports multiple methods to query for data.
```

### Comparing `CveXplore-0.3.9/README.rst` & `CveXplore-6561581/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,85 @@
-.. image:: images/CveExplore_logo.png
+Metadata-Version: 2.1
+Name: CveXplore
+Version: 6561581
+Summary: Package for interacting with cve-search
+Home-page: https://github.com/cve-search/CveXplore
+Author: Paul Tikken
+Author-email: paul.tikken@gmail.com
+License: GNU General Public License v3.0
+Project-URL: Documentation, https://cve-search.github.io/CveXplore/
+Project-URL: Issues, https://github.com/cve-search/CveXplore/issues
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: urllib3>=2.0.6
+Requires-Dist: tqdm==4.66.1
+Requires-Dist: python-dateutil==2.8.2
+Requires-Dist: click==8.1.7
+Requires-Dist: click-completion==0.5.2
+Requires-Dist: ijson>=3.2.3
+Requires-Dist: ansicolors==1.1.8
+Requires-Dist: pygelf>=0.4.2
+Requires-Dist: pandas>=2.1.2
+Requires-Dist: dicttoxml==1.7.16
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: aiohttp>=3.8.6
+Requires-Dist: aioretry>=5.0.2
+Requires-Dist: pymongo>=4.5.0
+Provides-Extra: mysql
+Requires-Dist: sqlalchemy>=2.0.23; extra == "mysql"
+Requires-Dist: alembic>=1.13.0; extra == "mysql"
+Requires-Dist: PyMySQL>=1.1.0; extra == "mysql"
+Provides-Extra: kafka
+Provides-Extra: sqllite
+Requires-Dist: sqlalchemy>=2.0.23; extra == "sqllite"
+Requires-Dist: alembic>=1.13.0; extra == "sqllite"
+Provides-Extra: redis
+Provides-Extra: sqlalchemy
+Requires-Dist: sqlalchemy>=2.0.23; extra == "sqlalchemy"
+Requires-Dist: alembic>=1.13.0; extra == "sqlalchemy"
+Provides-Extra: mongodb
+Requires-Dist: pymongo>=4.5.0; extra == "mongodb"
+Provides-Extra: docs
+Requires-Dist: sphinx==7.2.6; extra == "docs"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "docs"
+Requires-Dist: sphinx-autodoc-typehints>=1.25.2; extra == "docs"
+Provides-Extra: postgres
+Requires-Dist: sqlalchemy>=2.0.23; extra == "postgres"
+Requires-Dist: alembic>=1.13.0; extra == "postgres"
+Provides-Extra: all
+Requires-Dist: pymongo>=4.5.0; extra == "all"
+Requires-Dist: alembic>=1.13.0; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.23; extra == "all"
+Requires-Dist: sphinx==7.2.6; extra == "all"
+Requires-Dist: sphinx-autodoc-typehints>=1.25.2; extra == "all"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "all"
+Requires-Dist: PyMySQL>=1.1.0; extra == "all"
+
 
-.. Everything after the include marker below is inserted into the sphinx html docs. Everything above this comment is only visible in the github README.rst ##INCLUDE_MARKER##
 
 .. image:: https://img.shields.io/github/release/cve-search/CveXplore.svg
    :target: https://GitHub.com/cve-search/CveXplore/releases/
 
 .. image:: https://img.shields.io/badge/License-GPLv3-blue.svg
    :target: https://www.gnu.org/licenses/gpl-3.0
 
 .. image:: https://badgen.net/badge/Github/repo/green?icon=github
    :target: https://GitHub.com/cve-search/CveXplore
 
 
 The CveXplore package aims to provide an object related way to interact with the data collected or hosted by a
-cve-search instance. It provides an ambiguous way to interact either to the cve-search mongodb or to the cve-search API.
+cve-search instance. It provides an ambiguous way to interact with either the cve-search mongodb or the cve-search API.
 
 From version 0.2.5 onwards CveXplore has the possibility to initialize and update the database without the need of any of
 the cve-search binaries and thus providing the same functionality as cve-search but without the GUI components.
 
 A click command line functionality is being build but for now still in progress...
 
 All the data provided by this interaction is converted into objects before being returned. And thus providing a way to
@@ -35,20 +97,41 @@
 
 Both of them can be easily created on a physical machine or via a docker instance of cve-search;
 please check `cve-search <https://github.com/cve-search/cve-search>`_ or
 `CVE-Search-Docker <https://github.com/cve-search/CVE-Search-Docker>`_ for further details.
 
 Installation
 ------------
-Package is hosted on pypi, so just run:
+Package is hosted on pypi, so to install the minimal core just run:
 
 .. code-block:: bash
 
    pip install CveXplore
 
+This command will install the core logic of CveXplore and, by default, installs the mongodb module also.
+
+CveXplore is setup in a modular way and therefor has multiple modules which can be installed separately by specifying
+them as an extra requirement. To install the mysql module only, specify:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql]
+
+Or for multiple modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[mysql, redis]
+
+Or simple install all modules:
+
+.. code-block:: bash
+
+   pip install CveXplore[all]
+
 Documentation
 -------------
 Check `github pages documentation <https://cve-search.github.io/CveXplore/>`_
 
 General
 -------
 
@@ -107,24 +190,24 @@
    '0.1.2'
 
 To let CveXplore connect to an mongodb with specific parameters:
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(mongodb_connection_details={"host": "192.168.1.1", "port": 27017})
+   >>> cvx = CveXplore(datasource_type="mongodb", datasource_connection_details={"host": "mongodb://127.0.0.1:27017"})
    >>> cvx.version
    '0.1.2'
 
 And to let CveXplore talk to an Cve Search API (only query POST endpoint needed):
 
 .. code-block:: python
 
    >>> from CveXplore import CveXplore
-   >>> cvx = CveXplore(api_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
+   >>> cvx = CveXplore(datasource_type="api", datasource_connection_details={"address": ("mylocal.cve-search.int", 443), "api_path": "api"})
    >>> cvx.version
    '0.1.2'
 
 Query for data
 **************
 CveXplore supports multiple methods to query for data.
```

