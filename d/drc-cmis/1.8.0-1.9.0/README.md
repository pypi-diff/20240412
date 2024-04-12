# Comparing `tmp/drc-cmis-1.8.0.tar.gz` & `tmp/drc-cmis-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drc-cmis-1.8.0.tar", last modified: Mon Oct 23 13:13:06 2023, max compression
+gzip compressed data, was "drc-cmis-1.9.0.tar", last modified: Fri Apr 12 15:46:21 2024, max compression
```

## Comparing `drc-cmis-1.8.0.tar` & `drc-cmis-1.9.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.196526 drc-cmis-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29798 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21618 2023-10-23 13:13:06.196526 drc-cmis-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.180526 drc-cmis-1.8.0/drc_cmis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.184526 drc-cmis-1.8.0/drc_cmis/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19166 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/browser/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20630 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/browser/drc_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/browser/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/browser/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/client_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.188526 drc-cmis-1.8.0/drc_cmis/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0001_initial_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0002_auto_20190523_1054.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0003_auto_20191029_1349.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0004_auto_20200616_0919.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0005_auto_20200723_1352.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0006_cmisconfig_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0007_cmisconfig_time_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0008_auto_20200806_1030.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0009_auto_20200810_0830.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0010_auto_20200811_1221.py
--rw-r--r--   0 runner    (1001) docker     (127)    27932 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0011_auto_20200813_1640.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0012_auto_20200821_1512.py
--rw-r--r--   0 runner    (1001) docker     (127)    27969 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0013_auto_20201216_1046.py
--rw-r--r--   0 runner    (1001) docker     (127)    29023 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0013_auto_20201224_1302.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0014_auto_20210106_1602.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0015_merge_20210204_1046.py
--rw-r--r--   0 runner    (1001) docker     (127)    27451 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0016_alter_cmisconfig_time_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0017_cmisconfig_verzoek_folder_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    27142 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/0018_alter_cmisconfig_time_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.176526 drc-cmis-1.8.0/drc_cmis/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.176526 drc-cmis-1.8.0/drc_cmis/static/drc_cmis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.188526 drc-cmis-1.8.0/drc_cmis/static/drc_cmis/js/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/static/drc_cmis/js/cmis_config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.188526 drc-cmis-1.8.0/drc_cmis/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/templates/configuration_form.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.188526 drc-cmis-1.8.0/drc_cmis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.192526 drc-cmis-1.8.0/drc_cmis/webservice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32947 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/data_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    29374 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/drc_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/drc_cmis/webservice/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.184526 drc-cmis-1.8.0/drc_cmis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21618 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-23 13:13:06.000000 drc-cmis-1.8.0/drc_cmis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2023-10-23 13:13:06.196526 drc-cmis-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-23 13:13:06.192526 drc-cmis-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    95567 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_connection_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_delete_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    51249 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2023-10-23 13:13:00.000000 drc-cmis-1.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.338048 drc-cmis-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29798 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21652 2024-04-12 15:46:21.338048 drc-cmis-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.326048 drc-cmis-1.9.0/drc_cmis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.330048 drc-cmis-1.9.0/drc_cmis/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19168 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/browser/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20630 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/browser/drc_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/browser/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/browser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/client_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.334048 drc-cmis-1.9.0/drc_cmis/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0001_initial_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0002_auto_20190523_1054.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0003_auto_20191029_1349.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0004_auto_20200616_0919.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0005_auto_20200723_1352.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0006_cmisconfig_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0007_cmisconfig_time_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0008_auto_20200806_1030.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0009_auto_20200810_0830.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0010_auto_20200811_1221.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27932 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0011_auto_20200813_1640.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0012_auto_20200821_1512.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27969 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0013_auto_20201216_1046.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29023 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0013_auto_20201224_1302.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0014_auto_20210106_1602.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0015_merge_20210204_1046.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27451 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0016_alter_cmisconfig_time_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0017_cmisconfig_verzoek_folder_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27142 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/0018_alter_cmisconfig_time_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.322048 drc-cmis-1.9.0/drc_cmis/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.322048 drc-cmis-1.9.0/drc_cmis/static/drc_cmis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.334048 drc-cmis-1.9.0/drc_cmis/static/drc_cmis/js/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/static/drc_cmis/js/cmis_config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.334048 drc-cmis-1.9.0/drc_cmis/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/templates/configuration_form.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.334048 drc-cmis-1.9.0/drc_cmis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.334048 drc-cmis-1.9.0/drc_cmis/webservice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32947 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/data_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29374 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/drc_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/drc_cmis/webservice/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.338048 drc-cmis-1.9.0/drc_cmis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21652 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 15:46:21.000000 drc-cmis-1.9.0/drc_cmis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-12 15:46:21.338048 drc-cmis-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:46:21.338048 drc-cmis-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95567 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_connection_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_delete_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51249 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-04-12 15:46:17.000000 drc-cmis-1.9.0/tests/test_utils.py
```

### Comparing `drc-cmis-1.8.0/AUTHORS` & `drc-cmis-1.9.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/CHANGELOG.rst` & `drc-cmis-1.9.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =========
 Changelog
 =========
 
+1.9.0 (2024-04-12)
+------------------
+
+* Supported Django 4.2
+* Supported python 3.11
+* Dropped support of python 3.7, python 3.8, python 3.9
+
 1.8.0 (2023-09-18)
 ------------------
 
 Remove django-choices dependency and migrate to native Django choices enums.
 
 1.7.0 (2022-12-14)
 ------------------
```

### Comparing `drc-cmis-1.8.0/LICENSE.md` & `drc-cmis-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/PKG-INFO` & `drc-cmis-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: drc-cmis
-Version: 1.8.0
+Version: 1.9.0
 Summary: An adapter to manage Documenten API resources in a CMIS backend.
 Home-page: https://github.com/open-zaak/cmis-adapter
 Author: Maykin Media, Joeri Bekker, Jorik Kraaikamp, Sergei Maertens, Silvia Amabilino
 Author-email: support@maykinmedia.nl
 License: EUPL-1.2
 Keywords: CMIS,Documenten API,VNG,Common Ground
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.md
 License-File: AUTHORS
-Requires-Dist: django<4.0,>=3.2.0
+Requires-Dist: django>=3.2.0
 Requires-Dist: cmislib-maykin>=0.7.2.dev0
 Requires-Dist: django-solo
 Requires-Dist: iso8601
 Requires-Dist: commonground-api-common
 Requires-Dist: python-decouple
 Requires-Dist: furl
 Provides-Extra: tests
@@ -53,15 +54,15 @@
 Requires-Dist: bumpversion; extra == "release"
 Requires-Dist: twine; extra == "release"
 
 ===========================
 Documenten API CMIS adapter
 ===========================
 
-:Version: 1.8.0
+:Version: 1.9.0
 :Source: https://github.com/open-zaak/cmis-adapter
 :Keywords: CMIS, Documenten API, VNG, Common Ground
 :PythonVersion: 3.7
 
 |build-status| |coverage| |linting| |black| |python-versions| |django-versions| |pypi-version|
 
 A CMIS backend-connector for the `Documenten API`_.
```

### Comparing `drc-cmis-1.8.0/README.rst` & `drc-cmis-1.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================
 Documenten API CMIS adapter
 ===========================
 
-:Version: 1.8.0
+:Version: 1.9.0
 :Source: https://github.com/open-zaak/cmis-adapter
 :Keywords: CMIS, Documenten API, VNG, Common Ground
 :PythonVersion: 3.7
 
 |build-status| |coverage| |linting| |black| |python-versions| |django-versions| |pypi-version|
 
 A CMIS backend-connector for the `Documenten API`_.
```

### Comparing `drc-cmis-1.8.0/drc_cmis/admin.py` & `drc-cmis-1.9.0/drc_cmis/admin.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/apps.py` & `drc-cmis-1.9.0/drc_cmis/apps.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/browser/client.py` & `drc-cmis-1.9.0/drc_cmis/browser/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,17 +300,17 @@
             "propertyValue[1]": str(uuid.uuid4()),
         }
 
         json_data["propertyId[2]"] = "cmis:objectTypeId"
         if "cmis:objectTypeId" in properties.keys():
             json_data["propertyValue[2]"] = properties.pop("cmis:objectTypeId")
         else:
-            json_data[
-                "propertyValue[2]"
-            ] = f"{self.get_object_type_id_prefix(object_type)}drc:{object_type}"
+            json_data["propertyValue[2]"] = (
+                f"{self.get_object_type_id_prefix(object_type)}drc:{object_type}"
+            )
 
         prop_count = 3
         for prop_key, prop_value in properties.items():
             if isinstance(prop_value, datetime.date):
                 prop_value = prop_value.strftime("%Y-%m-%dT%H:%M:%S.000Z")
 
             json_data[f"propertyId[{prop_count}]"] = prop_key
```

### Comparing `drc-cmis-1.8.0/drc_cmis/browser/drc_document.py` & `drc-cmis-1.9.0/drc_cmis/browser/drc_document.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/browser/request.py` & `drc-cmis-1.9.0/drc_cmis/browser/request.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/browser/utils.py` & `drc-cmis-1.9.0/drc_cmis/browser/utils.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/client.py` & `drc-cmis-1.9.0/drc_cmis/client.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/client_builder.py` & `drc-cmis-1.9.0/drc_cmis/client_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from drc_cmis.browser.client import CMISDRCClient
 from drc_cmis.models import CMISConfig
 from drc_cmis.webservice.client import SOAPCMISClient
 
 try:
     from zgw_consumers.client import get_client_class
-except ImportError:
+except (ImportError, RuntimeError):
 
     def get_client_class() -> Type[Client]:
         return Client
 
 
 def get_cmis_client() -> Union[CMISDRCClient, SOAPCMISClient]:
     """Build the CMIS client with the binding specified in the configuration"""
```

### Comparing `drc-cmis-1.8.0/drc_cmis/connections.py` & `drc-cmis-1.9.0/drc_cmis/connections.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/forms.py` & `drc-cmis-1.9.0/drc_cmis/forms.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0001_initial_new.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0002_auto_20190523_1054.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0002_auto_20190523_1054.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0004_auto_20200616_0919.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0004_auto_20200616_0919.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0006_cmisconfig_binding.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0006_cmisconfig_binding.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0007_cmisconfig_time_zone.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0007_cmisconfig_time_zone.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0008_auto_20200806_1030.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0008_auto_20200806_1030.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0009_auto_20200810_0830.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0009_auto_20200810_0830.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0010_auto_20200811_1221.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0010_auto_20200811_1221.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0011_auto_20200813_1640.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0011_auto_20200813_1640.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0012_auto_20200821_1512.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0012_auto_20200821_1512.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0013_auto_20201216_1046.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0013_auto_20201216_1046.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0013_auto_20201224_1302.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0013_auto_20201224_1302.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0014_auto_20210106_1602.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0014_auto_20210106_1602.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0016_alter_cmisconfig_time_zone.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0016_alter_cmisconfig_time_zone.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0017_cmisconfig_verzoek_folder_path.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0017_cmisconfig_verzoek_folder_path.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/migrations/0018_alter_cmisconfig_time_zone.py` & `drc-cmis-1.9.0/drc_cmis/migrations/0018_alter_cmisconfig_time_zone.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/mixins.py` & `drc-cmis-1.9.0/drc_cmis/mixins.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/models.py` & `drc-cmis-1.9.0/drc_cmis/models.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/notifications.py` & `drc-cmis-1.9.0/drc_cmis/notifications.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Listen to the notifications that are send by the NRC
 """
+
 from vng_api_common.notifications.handlers import RoutingHandler, default
 
 from drc_cmis.client_builder import get_cmis_client, get_zds_client
 
 
 class ZakenHandler:
     def __init__(self):
```

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/convert.py` & `drc-cmis-1.9.0/drc_cmis/utils/convert.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     return tmp_datetime
 
 
 def parseDateTimeValue(value):
     """
     Utility function to return a datetime from a string.
     """
-    if type(value) == str:
+    if isinstance(value, str):
         return iso8601.parse_date(value)
-    elif type(value) == int:
+    elif isinstance(value, int):
         return datetime.fromtimestamp(value / 1000)
     else:
         return None
 
 
 def make_enkelvoudiginformatieobject_dataclass(cmis_doc, dataclass, skip_deleted=False):
     if cmis_doc.verwijderd and not skip_deleted:
```

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/exceptions.py` & `drc-cmis-1.9.0/drc_cmis/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/folder.py` & `drc-cmis-1.9.0/drc_cmis/utils/folder.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/mapper.py` & `drc-cmis-1.9.0/drc_cmis/utils/mapper.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/query.py` & `drc-cmis-1.9.0/drc_cmis/utils/query.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/utils/utils.py` & `drc-cmis-1.9.0/drc_cmis/utils/utils.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/validators.py` & `drc-cmis-1.9.0/drc_cmis/validators.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/client.py` & `drc-cmis-1.9.0/drc_cmis/webservice/client.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/data_models.py` & `drc-cmis-1.9.0/drc_cmis/webservice/data_models.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/drc_document.py` & `drc-cmis-1.9.0/drc_cmis/webservice/drc_document.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/fetcher.py` & `drc-cmis-1.9.0/drc_cmis/webservice/fetcher.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/request.py` & `drc-cmis-1.9.0/drc_cmis/webservice/request.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis/webservice/utils.py` & `drc-cmis-1.9.0/drc_cmis/webservice/utils.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/drc_cmis.egg-info/PKG-INFO` & `drc-cmis-1.9.0/drc_cmis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: drc-cmis
-Version: 1.8.0
+Version: 1.9.0
 Summary: An adapter to manage Documenten API resources in a CMIS backend.
 Home-page: https://github.com/open-zaak/cmis-adapter
 Author: Maykin Media, Joeri Bekker, Jorik Kraaikamp, Sergei Maertens, Silvia Amabilino
 Author-email: support@maykinmedia.nl
 License: EUPL-1.2
 Keywords: CMIS,Documenten API,VNG,Common Ground
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.md
 License-File: AUTHORS
-Requires-Dist: django<4.0,>=3.2.0
+Requires-Dist: django>=3.2.0
 Requires-Dist: cmislib-maykin>=0.7.2.dev0
 Requires-Dist: django-solo
 Requires-Dist: iso8601
 Requires-Dist: commonground-api-common
 Requires-Dist: python-decouple
 Requires-Dist: furl
 Provides-Extra: tests
@@ -53,15 +54,15 @@
 Requires-Dist: bumpversion; extra == "release"
 Requires-Dist: twine; extra == "release"
 
 ===========================
 Documenten API CMIS adapter
 ===========================
 
-:Version: 1.8.0
+:Version: 1.9.0
 :Source: https://github.com/open-zaak/cmis-adapter
 :Keywords: CMIS, Documenten API, VNG, Common Ground
 :PythonVersion: 3.7
 
 |build-status| |coverage| |linting| |black| |python-versions| |django-versions| |pypi-version|
 
 A CMIS backend-connector for the `Documenten API`_.
```

### Comparing `drc-cmis-1.8.0/drc_cmis.egg-info/SOURCES.txt` & `drc-cmis-1.9.0/drc_cmis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/setup.cfg` & `drc-cmis-1.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [metadata]
 name = drc-cmis
-version = 1.8.0
+version = 1.9.0
 description = An adapter to manage Documenten API resources in a CMIS backend.
 long_description = file: README.rst
 url = https://github.com/open-zaak/cmis-adapter
 license = EUPL-1.2
 author = Maykin Media, Joeri Bekker, Jorik Kraaikamp, Sergei Maertens, Silvia Amabilino
 author_email = support@maykinmedia.nl
 keywords = CMIS, Documenten API, VNG, Common Ground
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 3.2
+	Framework :: Django :: 4.2
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
@@ -26,15 +27,15 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	django>=3.2.0,<4.0
+	django>=3.2.0
 	cmislib-maykin >= 0.7.2.dev0
 	django-solo
 	iso8601
 	commonground-api-common
 	python-decouple
 	furl
 tests_require =
```

### Comparing `drc-cmis-1.8.0/tests/test_admin.py` & `drc-cmis-1.9.0/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_clients.py` & `drc-cmis-1.9.0/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_connection_pooling.py` & `drc-cmis-1.9.0/tests/test_connection_pooling.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_delete_relations.py` & `drc-cmis-1.9.0/tests/test_delete_relations.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_documents.py` & `drc-cmis-1.9.0/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_fetcher.py` & `drc-cmis-1.9.0/tests/test_fetcher.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_mapper.py` & `drc-cmis-1.9.0/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_path_validators.py` & `drc-cmis-1.9.0/tests/test_path_validators.py`

 * *Files identical despite different names*

### Comparing `drc-cmis-1.8.0/tests/test_utils.py` & `drc-cmis-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

