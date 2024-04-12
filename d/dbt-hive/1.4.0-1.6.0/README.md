# Comparing `tmp/dbt-hive-1.4.0.tar.gz` & `tmp/dbt-hive-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-hive-1.4.0.tar", last modified: Wed Aug 16 03:10:03 2023, max compression
+gzip compressed data, was "dbt-hive-1.6.0.tar", last modified: Fri Apr 12 16:23:04 2024, max compression
```

## Comparing `dbt-hive-1.4.0.tar` & `dbt-hive-1.6.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.898881 dbt-hive-1.4.0/
--rw-r--r--   0 jenkins   (1001) users      (100)    11346 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     4048 2023-08-16 03:10:03.898881 dbt-hive-1.4.0/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     3780 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.886881 dbt-hive-1.4.0/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.886881 dbt-hive-1.4.0/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.890881 dbt-hive-1.4.0/dbt/adapters/hive/
--rw-r--r--   0 jenkins   (1001) users      (100)      225 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt/adapters/hive/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1033 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      595 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8443 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2899 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15961 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    20594 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2662 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/adapters/hive/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.886881 dbt-hive-1.4.0/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.890881 dbt-hive-1.4.0/dbt/include/hive/
--rw-r--r--   0 jenkins   (1001) users      (100)      629 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      648 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.890881 dbt-hive-1.4.0/dbt/include/hive/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    11287 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1553 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/apply_grants.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.894881 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.894881 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/
--rw-r--r--   0 jenkins   (1001) users      (100)     5936 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2378 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     4690 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2070 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/validate.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     4185 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/seed.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6916 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/snapshot.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2056 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/table.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      697 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/materializations/view.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.898881 dbt-hive-1.4.0/dbt/include/hive/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      719 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      192 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      127 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      425 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      720 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      669 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      682 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/date_trunc.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1592 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     3069 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      689 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      742 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1208 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      514 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      724 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      896 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/right.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1140 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      662 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      776 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/dbt/include/hive/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-08-16 03:10:03.898881 dbt-hive-1.4.0/dbt_hive.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     4048 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt_hive.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1903 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt_hive.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt_hive.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)      216 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt_hive.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2023-08-16 03:10:03.000000 dbt-hive-1.4.0/dbt_hive.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2023-08-16 03:10:03.898881 dbt-hive-1.4.0/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3046 2023-08-16 03:08:49.000000 dbt-hive-1.4.0/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/
+-rw-r--r--   0 jenkins   (1001) users      (100)    11346 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     4317 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/adapters/hive/
+-rw-r--r--   0 jenkins   (1001) users      (100)      225 2024-04-12 16:23:03.000000 dbt-hive-1.6.0/dbt/adapters/hive/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1033 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      595 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2899 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    16071 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    20594 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2662 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/
+-rw-r--r--   0 jenkins   (1001) users      (100)      629 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      648 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    11287 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1553 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/apply_grants.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.171416 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/
+-rw-r--r--   0 jenkins   (1001) users      (100)     5936 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2378 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     4690 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2070 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     4185 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/seed.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6916 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/snapshot.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2056 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/table.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      697 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/view.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/dbt/include/hive/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      719 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      192 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      127 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      425 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      720 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      669 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1615 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/date_trunc.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1592 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     3069 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      689 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      742 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      514 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      724 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      894 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/right.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1210 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      662 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      776 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/dbt_hive.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1903 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)      235 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3363 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/setup.py
```

### Comparing `dbt-hive-1.4.0/LICENSE` & `dbt-hive-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/PKG-INFO` & `dbt-hive-1.6.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: dbt-hive
-Version: 1.4.0
-Summary: The Hive adapter plugin for dbt
-Home-page: https://github.com/cloudera/dbt-hive
-Author: Cloudera
-Author-email: innovation-feedback@cloudera.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dbt-hive
 
 The `dbt-hive` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Hive](https://hive.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
 
 
 ## Getting started
 
@@ -57,17 +47,17 @@
 | Name | Supported | Iceberg |
 |------|-----------|---------|
 |Materialization: View | Yes | N/A |
 |Materialization: Table| Yes | Yes |
 |Materialization: Table with Partitions | Yes | Yes |
 |Materialization: Incremental - Append | Yes | Yes|
 |Materialization: Incremental - Append with Partitions | Yes | Yes|
-|Materialization: Incremental - Insert+Overwrite| No | No |
 |Materialization: Incremental - Insert+Overwrite with Partitions | Yes | No |
-|Materialization: Incremental - Merge | No | Yes |
+|Materialization: Incremental - Merge | Yes | Yes |
+|Materialization: Incremental - Merge with Partitions | No | Yes* |
 |Materialization: Ephemeral | No | No |
 |Seeds | Yes | Yes |
 |Tests | Yes | Yes |
 |Snapshots | No | No |
 |Documentation | Yes | No |
 |Authentication: LDAP | Yes | Yes |
 |Authentication: Kerberos | Yes | Yes |
@@ -77,18 +67,24 @@
 Incremental models are explained in [dbt documentation](https://docs.getdbt.com/docs/build/incremental-models). This section covered the details about the incremental strategy supported by the dbt-hive.
 
 | Strategy | ACID Table | Iceberg Table |
 |------|------|---------|
 | Incremental Full-Refresh | Yes | Yes |
 | Incremental Append | Yes | Yes |
 | Incremental Append with Partitions | Yes | Yes |
-| Incremental Insert Overwrite | No | No|
-| Incremental Insert Overwrite with Partitions | Yes | No|
-| Incremental Merge | No | Yes |
-| Incremental Merge with Partitions | No | Yes |
+| Incremental Insert Overwrite | Not recommended without Partitions* | Not recommended without Partitions* |
+| Incremental Insert Overwrite with Partitions | Yes | No |
+| Incremental Merge | Yes | Yes* (only v2) |
+| Incremental Merge with Partitions | No* | Yes* (only v2) |
+
+**Note***:
+1. Incremental Insert overwrite without the partition columns results into completely overwriting the full table and may result in the data-loss. Hence it is not recommended to used. This can happen for Hive ACID, Iceberg v1 & v2 tables.
+1. Incremental Merge for iceberg v1 table is not supported because Iceberg v1 tables are not transactional.
+1. Incremental Merge with partition columns is not supported because Hive ACID tables doesn't support updating values of partition columns.
+
 
 Support for [On-Schema Change](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change) strategy in dbt-hive:
 
 | Strategy | ACID Table | Iceberg Table |
 |------|------|---------|
 | ignore (default)  | Supported  | Supported |
 | fail | Supported | Supported |
@@ -101,16 +97,15 @@
 | Name | Base | Iceberg |
 |------|------|---------|
 |Materialization: View | Yes | N/A |
 |Materialization: Table| Yes | Yes |
 |Materialization: Table with Partitions | Yes | Yes |
 |Materialization: Incremental - Append | Yes | Yes|
 |Materialization: Incremental - Append with Partitions | Yes | Yes|
-|Materialization: Incremental - Insert+Overwrite| Yes | Yes |
-|Materialization: Incremental - Insert+Overwrite with Partitions | Yes | Yes |
+|Materialization: Incremental - Insert+Overwrite with Partitions | Yes | No |
 |Materialization: Incremental - Merge | No | No |
 |Materialization: Ephemeral | No | No |
 |Seeds | Yes | Yes |
 |Tests | Yes | Yes |
 |Snapshots | No | No |
 |Documentation | Yes | No |
 |Authentication: LDAP | Yes | Yes |
```

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/__init__.py` & `dbt-hive-1.6.0/dbt/adapters/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/__version__.py` & `dbt-hive-1.6.0/dbt/adapters/hive/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-version = "1.4.0"
+version = "1.6.0"
```

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/cloudera_tracking.py` & `dbt-hive-1.6.0/dbt/adapters/hive/cloudera_tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/column.py` & `dbt-hive-1.6.0/dbt/adapters/hive/column.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/connections.py` & `dbt-hive-1.6.0/dbt/adapters/hive/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,18 @@
         # generate unique ids for tracking
         tracker.populate_unique_ids(self)
 
     @property
     def type(self):
         return "hive"
 
+    @property
+    def unique_field(self) -> str:
+        return f"{self.host}_{self.schema}_{self.username}"
+
     def _connection_keys(self):
         return "host", "schema", "user"
 
 
 class HiveConnectionWrapper:
     """Wrap a Hive connection in a way that no-ops transactions"""
```

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/impl.py` & `dbt-hive-1.6.0/dbt/adapters/hive/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/adapters/hive/relation.py` & `dbt-hive-1.6.0/dbt/adapters/hive/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/__init__.py` & `dbt-hive-1.6.0/dbt/include/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/dbt_project.yml` & `dbt-hive-1.6.0/dbt/include/hive/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/adapters.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/apply_grants.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/incremental.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/strategies.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/incremental/validate.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/seed.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/snapshot.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/table.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/materializations/view.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/any_value.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/bool_or.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/concat.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/date_trunc.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/escape_single_quotes.sql`

 * *Files 9% similar despite different names*

```diff
@@ -9,11 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
-
-{% macro hive__date_trunc(datepart, date) -%}
-    trunc({{date}}, '{{datepart}}')
+{% macro hive__escape_single_quotes(expression) -%}
+{{ expression | replace("'","\\'") }}
 {%- endmacro %}
```

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/dateadd.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/datediff.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/escape_single_quotes.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/hash.sql`

 * *Files 15% similar despite different names*

```diff
@@ -9,10 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
-{% macro hive__escape_single_quotes(expression) -%}
-{{ expression | replace("'","\\'") }}
+
+{% macro hive__hash(expression) -%}
+    case when {{ expression }} = NULL
+        then md5('')
+    else
+        md5({{ expression }})
+    end
 {%- endmacro %}
```

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/hash.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/timestamps.sql`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
-
-{% macro hive__hash(expression) -%}
-    case when {{ expression }} = NULL
-        then md5('')
-    else
-        md5({{ expression }})
-    end
+{% macro hive__current_timestamp() -%}
+    current_timestamp()
 {%- endmacro %}
```

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/last_day.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/listagg.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/position.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/right.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/right.sql`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #}
 {% macro hive__right(string_text, length_expression) %}
 
     case when {{ length_expression }} = 0
-        then NULL
+        then ''
     else
         substr(
         {{ string_text }},
         (length({{ string_text }})-cast({{ length_expression }} as int)+1),
         length({{ string_text }})-1
     )
     end
```

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/split_part.sql` & `dbt-hive-1.6.0/dbt/include/hive/macros/utils/split_part.sql`

 * *Files 10% similar despite different names*

```diff
@@ -21,18 +21,19 @@
         case when regexp_extract({{ delimiter_text }}, '([^A-Za-z0-9])(.*)', 1) != '_'
             then concat('\\', {{ delimiter_text }})
             else {{ delimiter_text }} end
 
     {% endset %}
 
     {% set split_part_expr %}
-
-    split(
-        {{ string_text }},
-        {{ delimiter_expr }}
-        )[({{ part_number - 1 }})]
-
+        coalesce(
+            split(
+                {{ string_text }},
+                {{ delimiter_expr }}
+            )[({{ part_number - 1 }})],
+            ''
+        )
     {% endset %}
 
     {{ return(split_part_expr) }}
 
 {% endmacro %}
```

### Comparing `dbt-hive-1.4.0/dbt/include/hive/macros/utils/timestamps.sql` & `dbt-hive-1.6.0/dbt/include/hive/sample_profiles.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-{#
 # Copyright 2022 Cloudera Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-#}
-{% macro hive__current_timestamp() -%}
-    current_timestamp()
-{%- endmacro %}
+default:
+  outputs:
+    dev:
+      type: hive
+      # Add sample credentials here, like:
+      # host: <host>
+      # port: <port_num>
+      # username: <user>
+      # password: <pass>
+  target: dev
```

### Comparing `dbt-hive-1.4.0/dbt_hive.egg-info/PKG-INFO` & `dbt-hive-1.6.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-hive
-Version: 1.4.0
+Version: 1.6.0
 Summary: The Hive adapter plugin for dbt
 Home-page: https://github.com/cloudera/dbt-hive
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dbt-core~=1.6.0
+Requires-Dist: setuptools>=40.3.0
+Requires-Dist: impyla==0.18
+Requires-Dist: sqlparams>=3.0.0
+Requires-Dist: python-decouple>=3.6
+Requires-Dist: protobuf<5,>=4.0.0
+Requires-Dist: kerberos>=1.3.0; platform_system == "Darwin" or platform_system == "Linux"
+Requires-Dist: winkerberos>=0.9.1; platform_system == "Windows"
 
 # dbt-hive
 
 The `dbt-hive` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Hive](https://hive.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
 
 
 ## Getting started
@@ -57,17 +65,17 @@
 | Name | Supported | Iceberg |
 |------|-----------|---------|
 |Materialization: View | Yes | N/A |
 |Materialization: Table| Yes | Yes |
 |Materialization: Table with Partitions | Yes | Yes |
 |Materialization: Incremental - Append | Yes | Yes|
 |Materialization: Incremental - Append with Partitions | Yes | Yes|
-|Materialization: Incremental - Insert+Overwrite| No | No |
 |Materialization: Incremental - Insert+Overwrite with Partitions | Yes | No |
-|Materialization: Incremental - Merge | No | Yes |
+|Materialization: Incremental - Merge | Yes | Yes |
+|Materialization: Incremental - Merge with Partitions | No | Yes* |
 |Materialization: Ephemeral | No | No |
 |Seeds | Yes | Yes |
 |Tests | Yes | Yes |
 |Snapshots | No | No |
 |Documentation | Yes | No |
 |Authentication: LDAP | Yes | Yes |
 |Authentication: Kerberos | Yes | Yes |
@@ -77,18 +85,24 @@
 Incremental models are explained in [dbt documentation](https://docs.getdbt.com/docs/build/incremental-models). This section covered the details about the incremental strategy supported by the dbt-hive.
 
 | Strategy | ACID Table | Iceberg Table |
 |------|------|---------|
 | Incremental Full-Refresh | Yes | Yes |
 | Incremental Append | Yes | Yes |
 | Incremental Append with Partitions | Yes | Yes |
-| Incremental Insert Overwrite | No | No|
-| Incremental Insert Overwrite with Partitions | Yes | No|
-| Incremental Merge | No | Yes |
-| Incremental Merge with Partitions | No | Yes |
+| Incremental Insert Overwrite | Not recommended without Partitions* | Not recommended without Partitions* |
+| Incremental Insert Overwrite with Partitions | Yes | No |
+| Incremental Merge | Yes | Yes* (only v2) |
+| Incremental Merge with Partitions | No* | Yes* (only v2) |
+
+**Note***:
+1. Incremental Insert overwrite without the partition columns results into completely overwriting the full table and may result in the data-loss. Hence it is not recommended to used. This can happen for Hive ACID, Iceberg v1 & v2 tables.
+1. Incremental Merge for iceberg v1 table is not supported because Iceberg v1 tables are not transactional.
+1. Incremental Merge with partition columns is not supported because Hive ACID tables doesn't support updating values of partition columns.
+
 
 Support for [On-Schema Change](https://docs.getdbt.com/docs/build/incremental-models#what-if-the-columns-of-my-incremental-model-change) strategy in dbt-hive:
 
 | Strategy | ACID Table | Iceberg Table |
 |------|------|---------|
 | ignore (default)  | Supported  | Supported |
 | fail | Supported | Supported |
@@ -101,16 +115,15 @@
 | Name | Base | Iceberg |
 |------|------|---------|
 |Materialization: View | Yes | N/A |
 |Materialization: Table| Yes | Yes |
 |Materialization: Table with Partitions | Yes | Yes |
 |Materialization: Incremental - Append | Yes | Yes|
 |Materialization: Incremental - Append with Partitions | Yes | Yes|
-|Materialization: Incremental - Insert+Overwrite| Yes | Yes |
-|Materialization: Incremental - Insert+Overwrite with Partitions | Yes | Yes |
+|Materialization: Incremental - Insert+Overwrite with Partitions | Yes | No |
 |Materialization: Incremental - Merge | No | No |
 |Materialization: Ephemeral | No | No |
 |Seeds | Yes | Yes |
 |Tests | Yes | Yes |
 |Snapshots | No | No |
 |Documentation | Yes | No |
 |Authentication: LDAP | Yes | Yes |
```

### Comparing `dbt-hive-1.4.0/dbt_hive.egg-info/SOURCES.txt` & `dbt-hive-1.6.0/dbt_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.4.0/setup.py` & `dbt-hive-1.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-hive"
 # make sure this always matches dbt/adapters/hive/__version__.py
-package_version = "1.4.0"
+package_version = "1.6.0"
 description = """The Hive adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
@@ -73,11 +73,15 @@
     },
     install_requires=[
         f"dbt-core~={dbt_core_version}",
         "setuptools>=40.3.0",
         "impyla==0.18",
         "sqlparams>=3.0.0",
         "python-decouple>=3.6",
+        # pining the protobuf version to 4.x because the dbt-core backports were messed up.
+        # more details in https://github.com/dbt-labs/dbt-core/issues/9830.
+        # TODO: remove this pin once the above issue and https://github.com/dbt-labs/dbt-core/issues/9724 is resolved.
+        "protobuf>=4.0.0,<5",
         "kerberos>=1.3.0; platform_system == 'Darwin' or platform_system == 'Linux' ",
         "winkerberos>=0.9.1; platform_system == 'Windows' ",
     ],
 )
```

