# Comparing `tmp/th2_data_services-2.0.0.dev8344817329.tar.gz` & `tmp/th2_data_services-2.0.0.dev8662586819.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev8344817329.tar", last modified: Tue Mar 19 14:47:10 2024, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev8662586819.tar", last modified: Fri Apr 12 13:10:30 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8344817329.tar` & `th2_data_services-2.0.0.dev8662586819.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    28305 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-19 14:46:58.000000 th2_data_services-2.0.0.dev8344817329/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    39858 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-03-19 14:46:50.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    34510 2024-03-19 14:47:09.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-03-19 14:47:10.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 14:47:09.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-19 14:47:09.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-19 14:47:09.000000 th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29605 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 13:10:20.000000 th2_data_services-2.0.0.dev8662586819/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42456 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6769 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22242 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-12 13:09:10.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    36010 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 13:10:30.000000 th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8344817329/PKG-INFO` & `th2_data_services-2.0.0.dev8662586819/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3833 3434 3831 3733 3239 0a53 756d 6d61  8344817329.Summa
+00000040: 3836 3632 3538 3638 3139 0a53 756d 6d61  8662586819.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -1679,479 +1679,573 @@
 000068e0: 696f 6e0a 2020 2020 2020 2020 6265 6869  ion.        behi
 000068f0: 6e64 2074 6865 2073 6365 6e65 7320 666f  nd the scenes fo
 00006900: 7220 796f 752e 204e 6f74 652c 2069 7420  r you. Note, it 
 00006910: 646f 6573 6e27 7420 6d65 616e 2079 6f75  doesn't mean you
 00006920: 2063 616e 6e6f 7420 6974 6572 6174 6520   cannot iterate 
 00006930: 7468 6520 5f44 6174 6120 6f62 6a65 6374  the _Data object
 00006940: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00006950: 2020 2020 2323 2320 4461 7461 2063 6163      ### Data cac
-00006960: 6869 6e67 0a20 2020 2020 2020 200a 2020  hing.        .  
-00006970: 2020 2020 2020 5468 6520 5f44 6174 6120        The _Data 
-00006980: 6f62 6a65 6374 5f20 7072 6f76 6964 6573  object_ provides
-00006990: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-000069a0: 7573 6520 7468 6520 6361 6368 652e 2054  use the cache. T
-000069b0: 6865 2063 6163 6865 2077 6f72 6b73 2066  he cache works f
-000069c0: 6f72 2065 6163 6820 5f44 6174 6120 6f62  or each _Data ob
-000069d0: 6a65 6374 5f2c 2074 6861 7420 6973 2c20  ject_, that is, 
-000069e0: 796f 7520 6368 6f6f 7365 0a20 2020 2020  you choose.     
-000069f0: 2020 2077 6869 6368 205f 4461 7461 206f     which _Data o
-00006a00: 626a 6563 745f 2079 6f75 2077 616e 7420  bject_ you want 
-00006a10: 746f 2073 6176 652e 2054 6865 205f 4461  to save. The _Da
-00006a20: 7461 206f 626a 6563 745f 2063 6163 6865  ta object_ cache
-00006a30: 2069 7320 7361 7665 6420 6166 7465 7220   is saved after 
-00006a40: 7468 6520 6669 7273 7420 6974 6572 6174  the first iterat
-00006a50: 696f 6e2c 2062 7574 2074 6865 2069 7465  ion, but the ite
-00006a60: 7261 7469 6f6e 0a20 2020 2020 2020 2073  ration.        s
-00006a70: 6f75 7263 6520 6d61 7920 6265 2064 6966  ource may be dif
-00006a80: 6665 7265 6e74 2e0a 2020 2020 2020 2020  ferent..        
-00006a90: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
-00006aa0: 646f 6e27 7420 7573 6520 7468 6520 6361  don't use the ca
-00006ab0: 6368 652c 2079 6f75 7220 736f 7572 6365  che, your source
-00006ac0: 2077 696c 6c20 6265 2074 6865 2064 6174   will be the dat
-00006ad0: 6120 736f 7572 6365 2079 6f75 2068 6176  a source you hav
-00006ae0: 6520 696e 2074 6865 205f 4461 7461 204f  e in the _Data O
-00006af0: 626a 6563 745f 2e20 4275 7420 6966 2079  bject_. But if y
-00006b00: 6f75 2075 7365 2074 6865 2063 6163 6865  ou use the cache
-00006b10: 2c0a 2020 2020 2020 2020 796f 7572 2073  ,.        your s
-00006b20: 6f75 7263 6520 6361 6e20 6265 2074 6865  ource can be the
-00006b30: 2064 6174 6120 736f 7572 6365 2c20 7468   data source, th
-00006b40: 6520 7061 7265 6e74 2063 6163 6865 2c20  e parent cache, 
-00006b50: 6f72 206f 776e 2063 6163 6865 3a0a 2020  or own cache:.  
-00006b60: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-00006b70: 2054 6865 2064 6174 6120 736f 7572 6365   The data source
-00006b80: 3a0a 2020 2020 2020 2020 2020 4966 2074  :.          If t
-00006b90: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00006ba0: 2064 6f65 736e 2774 2068 6176 6520 6120   doesn't have a 
-00006bb0: 7061 7265 6e74 2063 6163 6865 2061 6e64  parent cache and
-00006bc0: 2069 7473 2063 6163 6865 2e0a 2020 2020   its cache..    
-00006bd0: 2020 2020 2a20 5468 6520 7061 7265 6e74      * The parent
-00006be0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-00006bf0: 2020 4966 2074 6865 205f 4461 7461 204f    If the _Data O
-00006c00: 626a 6563 745f 2068 6173 2061 2070 6172  bject_ has a par
-00006c10: 656e 7420 6361 6368 652e 2049 7420 646f  ent cache. It do
-00006c20: 6573 6e27 7420 6d61 7474 6572 2077 6861  esn't matter wha
-00006c30: 7420 706f 7369 7469 6f6e 2074 6865 2070  t position the p
-00006c40: 6172 656e 7420 6361 6368 6520 6861 7320  arent cache has 
-00006c50: 696e 2069 6e68 6572 6974 616e 6365 2e0a  in inheritance..
-00006c60: 2020 2020 2020 2020 2020 5f44 6174 6120            _Data 
-00006c70: 4f62 6a65 6374 5f20 756e 6465 7273 7461  Object_ understa
-00006c80: 6e64 7320 7768 6f73 6520 6361 6368 6520  nds whose cache 
-00006c90: 6974 2069 7320 616e 6420 6578 6563 7574  it is and execut
-00006ca0: 6573 2074 6865 2070 6172 7420 6f66 2074  es the part of t
-00006cb0: 6865 2077 6f72 6b66 6c6f 7720 7468 6174  he workflow that
-00006cc0: 2077 6173 206e 6f74 2065 7865 6375 7465   was not execute
-00006cd0: 642e 0a20 2020 2020 2020 202a 2054 6865  d..        * The
-00006ce0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
-00006cf0: 2020 2020 2020 4966 2069 7420 6973 206e        If it is n
-00006d00: 6f74 2074 6865 2066 6972 7374 2069 7465  ot the first ite
-00006d10: 7261 7469 6f6e 206f 6620 7468 6973 2044  ration of this D
-00006d20: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-00006d30: 2020 2020 0a20 2020 2020 2020 204e 6f74      .        Not
-00006d40: 6520 7468 6174 2074 6865 2063 6163 6865  e that the cache
-00006d50: 2073 7461 7465 206f 6620 7468 6520 4461   state of the Da
-00006d60: 7461 206f 626a 6563 7420 6973 206e 6f74  ta object is not
-00006d70: 2069 6e68 6572 6974 6564 2e0a 2020 2020   inherited..    
-00006d80: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-00006d90: 2320 466f 7263 6564 2063 6163 6869 6e67  # Forced caching
-00006da0: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-00006db0: 2074 656c 6c20 4453 2074 6f20 6361 6368   tell DS to cach
-00006dc0: 6520 6461 7461 2074 6f20 7370 6563 6966  e data to specif
-00006dd0: 6963 2063 6163 6865 2066 696c 652c 2077  ic cache file, w
-00006de0: 6869 6368 2077 6f6e 2774 2062 6520 6465  hich won't be de
-00006df0: 6c65 7465 6420 6166 7465 7220 7363 7269  leted after scri
-00006e00: 7074 2065 6e64 2e0a 2020 2020 2020 2020  pt end..        
-00006e10: 596f 7520 6361 6e20 7365 6520 6578 616d  You can see exam
-00006e20: 706c 6520 696e 2031 2e31 3220 7365 6374  ple in 1.12 sect
-00006e30: 696f 6e20 6f66 205b 6765 745f 7374 6172  ion of [get_star
-00006e40: 7465 645f 6578 616d 706c 655d 2865 7861  ted_example](exa
-00006e50: 6d70 6c65 732f 6765 745f 7374 6172 7465  mples/get_starte
-00006e60: 645f 6578 616d 706c 652e 7079 292e 0a20  d_example.py).. 
-00006e70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006e80: 0a20 2020 2020 2020 2023 2323 2045 7665  .        ### Eve
-00006e90: 6e74 5472 6565 2061 6e64 2063 6f6c 6c65  ntTree and colle
-00006ea0: 6374 696f 6e73 0a20 2020 2020 2020 200a  ctions.        .
-00006eb0: 2020 2020 2020 2020 2323 2323 2045 7665          #### Eve
-00006ec0: 6e74 5472 6565 0a20 2020 2020 2020 200a  ntTree.        .
-00006ed0: 2020 2020 2020 2020 6045 7665 6e74 5472          `EventTr
-00006ee0: 6565 6020 6973 2061 2074 7265 652d 6261  ee` is a tree-ba
-00006ef0: 7365 6420 6461 7461 2073 7472 7563 7475  sed data structu
-00006f00: 7265 206f 6620 6576 656e 7473 2e20 4974  re of events. It
-00006f10: 2061 6c6c 6f77 7320 796f 7520 6765 7420   allows you get 
-00006f20: 6368 696c 6472 656e 2061 6e64 2070 6172  children and par
-00006f30: 656e 7473 206f 6620 6576 656e 742c 0a20  ents of event,. 
-00006f40: 2020 2020 2020 2064 6973 706c 6179 2074         display t
-00006f50: 7265 652c 2067 6574 2066 756c 6c20 7061  ree, get full pa
-00006f60: 7468 2074 6f20 6576 656e 7420 6574 632e  th to event etc.
-00006f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006f80: 2020 4465 7461 696c 733a 0a20 2020 2020    Details:.     
-00006f90: 2020 200a 2020 2020 2020 2020 2a20 6045     .        * `E
-00006fa0: 7665 6e74 5472 6565 6020 636f 6e74 6169  ventTree` contai
-00006fb0: 6e73 2061 6c6c 2065 7665 6e74 7320 696e  ns all events in
-00006fc0: 206d 656d 6f72 792e 0a20 2020 2020 2020   memory..       
-00006fd0: 202a 2054 7265 6520 6861 7320 736f 6d65   * Tree has some
-00006fe0: 2069 6d70 6f72 7461 6e74 2074 6572 6d73   important terms
-00006ff0: 3a0a 2020 2020 2020 2020 2020 2020 312e  :.            1.
-00007000: 205f 416e 6365 7374 6f72 5f20 6973 2061   _Ancestor_ is a
-00007010: 6e79 2072 656c 6174 6976 6520 6f66 2074  ny relative of t
-00007020: 6865 2065 7665 6e74 2075 7020 7468 6520  he event up the 
-00007030: 7472 6565 2028 6772 616e 6470 6172 656e  tree (grandparen
-00007040: 742c 2070 6172 656e 7420 6574 632e 292e  t, parent etc.).
-00007050: 0a20 2020 2020 2020 2020 2020 2032 2e20  .            2. 
-00007060: 5f50 6172 656e 745f 2069 7320 6f6e 6c79  _Parent_ is only
-00007070: 2074 6865 2066 6972 7374 2072 656c 6174   the first relat
-00007080: 6976 6520 6f66 2074 6865 2065 7665 6e74  ive of the event
-00007090: 2075 7020 7468 6520 7472 6565 2e0a 2020   up the tree..  
-000070a0: 2020 2020 2020 2020 2020 332e 205f 4368            3. _Ch
-000070b0: 696c 645f 2069 7320 7468 6520 6669 7273  ild_ is the firs
-000070c0: 7420 7265 6c61 7469 7665 206f 6620 7468  t relative of th
-000070d0: 6520 6576 656e 7420 646f 776e 2074 6865  e event down the
-000070e0: 2074 7265 652e 0a20 2020 2020 2020 200a   tree..        .
-000070f0: 2020 2020 2020 2020 5461 6b65 2061 206c          Take a l
-00007100: 6f6f 6b20 6174 2074 6865 2066 6f6c 6c6f  ook at the follo
-00007110: 7769 6e67 2048 544d 4c20 7472 6565 2074  wing HTML tree t
-00007120: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00007130: 6d2e 0a20 2020 2020 2020 200a 2020 2020  m..        .    
-00007140: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00007150: 2020 2020 2020 203c 626f 6479 3e20 3c21         <body> <!
-00007160: 2d2d 2061 6e63 6573 746f 7220 2867 7261  -- ancestor (gra
-00007170: 6e64 7061 7265 6e74 292c 2062 7574 206e  ndparent), but n
-00007180: 6f74 2070 6172 656e 7420 2d2d 3e0a 2020  ot parent -->.  
-00007190: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000071a0: 6976 3e20 3c21 2d2d 2070 6172 656e 7420  iv> <!-- parent 
-000071b0: 2620 616e 6365 7374 6f72 202d 2d3e 0a20  & ancestor -->. 
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 203c 703e 4865 6c6c 6f2c 2077 6f72     <p>Hello, wor
-000071e0: 6c64 213c 2f70 3e20 3c21 2d2d 2063 6869  ld!</p> <!-- chi
-000071f0: 6c64 202d 2d3e 0a20 2020 2020 2020 2020  ld -->.         
-00007200: 2020 2020 2020 2020 2020 203c 703e 476f             <p>Go
-00007210: 6f64 6279 6521 3c2f 703e 203c 212d 2d20  odbye!</p> <!-- 
-00007220: 7369 626c 696e 6720 2d2d 3e0a 2020 2020  sibling -->.    
-00007230: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00007240: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
-00007250: 2f62 6f64 793e 0a20 2020 2020 2020 2020  /body>.         
-00007260: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-00007270: 2020 2020 2020 2023 2323 2320 436f 6c6c         #### Coll
-00007280: 6563 7469 6f6e 730a 2020 2020 2020 2020  ections.        
-00007290: 0a20 2020 2020 2020 202a 2a45 7665 6e74  .        **Event
-000072a0: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
-000072b0: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
-000072c0: 206f 6620 4576 656e 7454 7265 6573 2e20   of EventTrees. 
-000072d0: 5468 6520 636f 6c6c 6563 7469 6f6e 2062  The collection b
-000072e0: 7569 6c64 7320 6120 6665 7720 5f45 7665  uilds a few _Eve
-000072f0: 6e74 5472 6565 5f20 6279 2070 6173 7365  ntTree_ by passe
-00007300: 6420 5f44 6174 610a 2020 2020 2020 2020  d _Data.        
-00007310: 6f62 6a65 6374 5f2e 2041 6c74 686f 7567  object_. Althoug
-00007320: 6820 796f 7520 6361 6e20 6368 616e 6765  h you can change
-00007330: 2074 6865 2074 7265 6520 6469 7265 6374   the tree direct
-00007340: 6c79 2c20 6974 2773 2062 6574 7465 7220  ly, it's better 
-00007350: 746f 2064 6f20 6974 2074 6872 6f75 6768  to do it through
-00007360: 2063 6f6c 6c65 6374 696f 6e73 2062 6563   collections bec
-00007370: 6175 7365 2074 6865 7920 6172 6520 6177  ause they are aw
-00007380: 6172 6520 6f66 0a20 2020 2020 2020 2060  are of.        `
-00007390: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
-000073a0: 2061 6e64 2063 616e 2073 6f6c 7665 2073   and can solve s
-000073b0: 6f6d 6520 6576 656e 7473 2064 6570 656e  ome events depen
-000073c0: 6465 6e63 6965 732e 2054 6865 2063 6f6c  dencies. The col
-000073d0: 6c65 6374 696f 6e20 6861 7320 7369 6d69  lection has simi
-000073e0: 6c61 7220 6665 6174 7572 6573 206c 696b  lar features lik
-000073f0: 6520 6120 7369 6e67 6c65 205f 4576 656e  e a single _Even
-00007400: 7454 7265 655f 0a20 2020 2020 2020 2062  tTree_.        b
-00007410: 7574 2061 7070 6c79 696e 6720 7468 656d  ut applying them
-00007420: 2066 6f72 2061 6c6c 205f 4576 656e 7454   for all _EventT
-00007430: 7265 6573 5f2e 0a20 2020 2020 2020 200a  rees_..        .
-00007440: 2020 2020 2020 2020 2a2a 5061 7265 6e74          **Parent
-00007450: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00007460: 696f 6e2a 2a20 6973 2061 2063 6f6c 6c65  ion** is a colle
-00007470: 6374 696f 6e20 7369 6d69 6c61 7220 746f  ction similar to
-00007480: 205f 4576 656e 7454 7265 6543 6f6c 6c65   _EventTreeColle
-00007490: 6374 696f 6e5f 2062 7574 2063 6f6e 7461  ction_ but conta
-000074a0: 696e 696e 6720 6f6e 6c79 2070 6172 656e  ining only paren
-000074b0: 7420 6576 656e 7473 2074 6861 740a 2020  t events that.  
-000074c0: 2020 2020 2020 6172 6520 7265 6665 7265        are refere
-000074d0: 6e63 6564 2069 6e20 7468 6520 6461 7461  nced in the data
-000074e0: 2073 7472 6561 6d2e 2054 6865 2063 6f6c   stream. The col
-000074f0: 6c65 6374 696f 6e20 6861 7320 6665 6174  lection has feat
-00007500: 7572 6573 2073 696d 696c 6172 2074 6f20  ures similar to 
-00007510: 5f45 7665 6e74 5472 6565 436f 6c6c 6563  _EventTreeCollec
-00007520: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
-00007530: 2020 2020 2020 2020 4465 7461 696c 733a          Details:
-00007540: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007550: 2020 2a20 546f 2075 7365 2045 5420 636f    * To use ET co
-00007560: 6c6c 6563 7469 6f6e 7320 796f 7520 6e65  llections you ne
-00007570: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
-00007580: 2074 6865 6d20 6279 205f 4554 4344 7269   them by _ETCDri
-00007590: 7665 725f 2e20 4461 7461 2073 6f75 7263  ver_. Data sourc
-000075a0: 6573 2075 7375 616c 6c79 2070 726f 7669  es usually provi
-000075b0: 6465 2074 6865 6d2e 0a20 2020 2020 2020  de them..       
-000075c0: 2020 2059 6f75 2063 616e 2063 7265 6174     You can creat
-000075d0: 6520 6974 2062 7920 796f 7572 7365 6c66  e it by yourself
-000075e0: 2064 6570 656e 6469 6e67 206f 6e20 796f   depending on yo
-000075f0: 7572 2064 6174 6120 7374 7275 6374 7572  ur data structur
-00007600: 652e 0a20 2020 2020 2020 202a 2054 6865  e..        * The
-00007610: 2063 6f6c 6c65 6374 696f 6e20 6861 7320   collection has 
-00007620: 6120 6665 6174 7572 6520 746f 2072 6563  a feature to rec
-00007630: 6f76 6572 2065 7665 6e74 732e 2041 6c6c  over events. All
-00007640: 2065 7665 6e74 7320 7468 6174 2061 7265   events that are
-00007650: 206e 6f74 2069 6e20 7468 6520 7265 6365   not in the rece
-00007660: 6976 6564 2064 6174 6120 7374 7265 616d  ived data stream
-00007670: 2c20 6275 7420 7768 6963 6820 6172 650a  , but which are.
-00007680: 2020 2020 2020 2020 2020 7265 6665 7265            refere
-00007690: 6e63 6564 2077 696c 6c20 6265 206c 6f61  nced will be loa
-000076a0: 6465 6420 6672 6f6d 2074 6865 2064 6174  ded from the dat
-000076b0: 6120 736f 7572 6365 2e0a 2020 2020 2020  a source..      
-000076c0: 2020 2a20 596f 7520 6361 6e20 7461 6b65    * You can take
-000076d0: 2060 6465 7461 6368 6564 5f65 7665 6e74   `detached_event
-000076e0: 7360 2074 6f20 7365 6520 7768 6963 6820  s` to see which 
-000076f0: 6576 656e 7473 2061 7265 206d 6973 7369  events are missi
-00007700: 6e67 2e0a 2020 2020 2020 2020 2a20 4966  ng..        * If
-00007710: 2079 6f75 2077 616e 742c 2079 6f75 2063   you want, you c
-00007720: 616e 2062 7569 6c64 2070 6172 656e 746c  an build parentl
-00007730: 6573 7320 7472 6565 7320 7768 6572 6520  ess trees where 
-00007740: 7468 6520 6d69 7373 696e 6720 6576 656e  the missing even
-00007750: 7473 2061 7265 2073 7475 6262 6564 2069  ts are stubbed i
-00007760: 6e73 7465 6164 2e20 4a75 7374 0a20 2020  nstead. Just.   
-00007770: 2020 2020 2020 2075 7365 2060 6765 745f         use `get_
-00007780: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00007790: 2829 602e 0a20 2020 2020 2020 200a 2020  ()`..        .  
-000077a0: 2020 2020 2020 5265 7175 6972 656d 656e        Requiremen
-000077b0: 7473 3a0a 2020 2020 2020 2020 0a20 2020  ts:.        .   
-000077c0: 2020 2020 2031 2e20 4576 656e 7473 2070       1. Events p
-000077d0: 726f 7669 6465 6420 746f 2045 5443 2068  rovided to ETC h
-000077e0: 6176 6520 746f 2068 6176 6520 6065 7665  ave to have `eve
-000077f0: 6e74 5f6e 616d 6560 2c20 6065 7665 6e74  nt_name`, `event
-00007800: 5f69 6460 2c20 6070 6172 656e 745f 6576  _id`, `parent_ev
-00007810: 656e 745f 6964 6020 6669 656c 6473 2e20  ent_id` fields. 
-00007820: 5468 6579 0a20 2020 2020 2020 2063 616e  They.        can
-00007830: 2068 6176 6520 616e 6f74 6865 7220 6e61   have another na
-00007840: 6d65 7320 2869 7420 7265 736f 6c76 6573  mes (it resolves
-00007850: 2069 6e20 7468 6520 6472 6976 6572 292e   in the driver).
-00007860: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007870: 2020 2323 2323 2048 696e 7473 0a20 2020    #### Hints.   
-00007880: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
-00007890: 5265 6d6f 7665 2061 6c6c 2075 6e6e 6563  Remove all unnec
-000078a0: 6573 7361 7279 2066 6965 6c64 7320 6672  essary fields fr
-000078b0: 6f6d 2065 7665 6e74 7320 6265 666f 7265  om events before
-000078c0: 2070 6173 7369 6e67 2074 6f20 6120 5f63   passing to a _c
-000078d0: 6f6c 6c65 6374 696f 6e5f 2074 6f20 7265  ollection_ to re
-000078e0: 6475 6365 206d 656d 6f72 7920 7573 6167  duce memory usag
-000078f0: 652e 0a20 2020 2020 2020 202a 2055 7365  e..        * Use
-00007900: 2060 7368 6f77 2829 6020 6d65 7468 6f64   `show()` method
-00007910: 2074 6f20 7072 696e 7420 7468 6520 7472   to print the tr
-00007920: 6565 2069 6e20 7472 6565 2d6c 696b 6520  ee in tree-like 
-00007930: 7669 6577 2e0a 2020 2020 2020 2020 2a20  view..        * 
-00007940: 4e6f 7465 2074 6861 7420 7468 6520 6067  Note that the `g
-00007950: 6574 5f78 6020 6d65 7468 6f64 7320 7769  et_x` methods wi
-00007960: 6c6c 2072 6169 7365 2061 6e20 6578 6365  ll raise an exce
-00007970: 7074 696f 6e20 6966 2079 6f75 2070 6173  ption if you pas
-00007980: 7320 616e 2075 6e6b 6e6f 776e 2065 7665  s an unknown eve
-00007990: 6e74 2069 642c 2075 6e6c 696b 6520 7468  nt id, unlike th
-000079a0: 6520 6066 696e 645f 7860 206d 6574 686f  e `find_x` metho
-000079b0: 6473 2028 0a20 2020 2020 2020 2020 2074  ds (.          t
-000079c0: 6865 7920 7265 7475 726e 204e 6f6e 6529  hey return None)
-000079d0: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
-000079e0: 6f75 2077 616e 7420 746f 206b 6e6f 7720  ou want to know 
-000079f0: 7468 6174 2073 7065 6369 6669 6564 2065  that specified e
-00007a00: 7665 6e74 2065 7869 7374 732c 2075 7365  vent exists, use
-00007a10: 2074 6865 2070 7974 686f 6e20 6069 6e60   the python `in`
-00007a20: 206b 6579 776f 7264 2028 652e 672e 2060   keyword (e.g. `
-00007a30: 2765 7665 6e74 2d69 6427 2069 6e20 6576  'event-id' in ev
-00007a40: 656e 7473 5f74 7265 6560 292e 0a20 2020  ents_tree`)..   
-00007a50: 2020 2020 202a 2055 7365 2074 6865 2070       * Use the p
-00007a60: 7974 686f 6e20 606c 656e 6020 6b65 7977  ython `len` keyw
-00007a70: 6f72 6420 746f 2067 6574 2065 7665 6e74  ord to get event
-00007a80: 7320 6e75 6d62 6572 2069 6e20 7468 6520  s number in the 
-00007a90: 7472 6565 2e0a 2020 2020 2020 2020 0a20  tree..        . 
-00007aa0: 2020 2020 2020 2023 2323 2046 6965 6c64         ### Field
-00007ab0: 2052 6573 6f6c 7665 7273 0a20 2020 2020   Resolvers.     
-00007ac0: 2020 2049 6e74 6572 6661 6365 2063 616e     Interface can
-00007ad0: 2062 6520 666f 756e 6420 696e 2060 7468   be found in `th
-00007ae0: 325f 6461 7461 5f73 6572 7669 6365 732f  2_data_services/
-00007af0: 696e 7465 7266 6163 6573 2f75 7469 6c73  interfaces/utils
-00007b00: 2f72 6573 6f6c 7665 722e 7079 602e 2020  /resolver.py`.  
-00007b10: 0a20 2020 2020 2020 2041 6c6c 2064 6174  .        All dat
-00007b20: 612d 736f 7572 6365 7320 7368 6f75 6c64  a-sources should
-00007b30: 2069 6d70 6c65 6d65 6e74 2074 6865 6d2e   implement them.
-00007b40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007b50: 2020 5468 6520 6964 6561 206f 6620 7573    The idea of us
-00007b60: 696e 6720 7265 736f 6c76 6572 733a 0a20  ing resolvers:. 
-00007b70: 2020 2020 2020 2049 7420 736f 6c76 6573         It solves
-00007b80: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
-00007b90: 6861 7669 6e67 2061 2066 6577 2044 6174  having a few Dat
-00007ba0: 6153 6f75 7263 6573 2077 6974 6820 7369  aSources with si
-00007bb0: 6d69 6c61 7220 6461 7461 2c0a 2020 2020  milar data,.    
-00007bc0: 2020 2020 6275 7420 7769 7468 2064 6966      but with dif
-00007bd0: 6665 7265 6e74 2077 6179 7320 746f 2067  ferent ways to g
-00007be0: 6574 2069 742e 0a20 2020 2020 2020 200a  et it..        .
-00007bf0: 2020 2020 2020 2020 5468 6573 6520 636c          These cl
-00007c00: 6173 7365 7320 7072 6f76 6964 6520 796f  asses provide yo
-00007c10: 7520 6765 7474 6572 206d 6574 686f 6473  u getter methods
-00007c20: 2e0a 2020 2020 2020 2020 5573 696e 6720  ..        Using 
-00007c30: 7468 6573 6520 636c 6173 7365 7320 616c  these classes al
-00007c40: 6c6f 7773 2079 6f75 2074 6f20 6672 6565  lows you to free
-00007c50: 6c79 2073 7769 7463 6820 6265 7477 6565  ly switch betwee
-00007c60: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
-00007c70: 0a20 2020 2020 2020 2066 6f72 6d61 7473  .        formats
-00007c80: 2061 6e64 2064 6f6e 2774 2063 6861 6e67   and don't chang
-00007c90: 6520 796f 7572 2063 6f64 652e 0a20 2020  e your code..   
-00007ca0: 2020 2020 200a 2020 2020 2020 2020 5265       .        Re
-00007cb0: 736f 6c76 6572 7320 736f 6c76 6520 7468  solvers solve th
-00007cc0: 6520 7072 6f62 6c65 6d20 6f66 2064 6174  e problem of dat
-00007cd0: 612d 666f 726d 6174 206d 6967 7261 7469  a-format migrati
-00007ce0: 6f6e 2e0a 2020 2020 2020 2020 2d20 6669  on..        - fi
-00007cf0: 656c 6473 2070 6c61 6365 2063 616e 2062  elds place can b
-00007d00: 6520 6368 616e 6765 640a 2020 2020 2020  e changed.      
-00007d10: 2020 2d20 6669 656c 6473 206e 616d 6573    - fields names
-00007d20: 2063 616e 2062 6520 6368 616e 6765 640a   can be changed.
-00007d30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00007d40: 2052 6573 6f6c 7665 7273 2063 616e 2077   Resolvers can w
-00007d50: 6f72 6b20 6f6e 6c79 2077 6974 6820 6f6e  ork only with on
-00007d60: 6520 6576 656e 742f 6d65 7373 6167 652e  e event/message.
-00007d70: 0a20 2020 2020 2020 2049 7420 6d65 616e  .        It mean
-00007d80: 732c 2069 6620 796f 7572 206d 6573 7361  s, if your messa
-00007d90: 6765 2068 6173 2073 7562 2d6d 6573 7361  ge has sub-messa
-00007da0: 6765 7320 286c 696b 6520 7468 322d 6d65  ges (like th2-me
-00007db0: 7373 6167 6573 2069 6e20 6c77 6470 2920  ssages in lwdp) 
-00007dc0: 6974 200a 2020 2020 2020 2020 776f 6e27  it .        won'
-00007dd0: 7420 776f 726b 2c20 6265 6361 7573 6520  t work, because 
-00007de0: 7265 736f 6c76 6572 2077 696c 6c20 6e6f  resolver will no
-00007df0: 7420 6b6e 6f77 2077 6974 6820 7768 6963  t know with whic
-00007e00: 6820 7375 622d 6d65 7373 6167 6520 7368  h sub-message sh
-00007e10: 6f75 6c64 2069 7420 776f 726b 2e20 0a20  ould it work. . 
-00007e20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007e30: 2a2a 576f 726b 6172 6f75 6e64 2a2a 2020  **Workaround**  
-00007e40: 0a20 2020 2020 2020 2031 2e20 4578 7061  .        1. Expa
-00007e50: 6e64 2061 6c6c 2079 6f75 7220 6d65 7373  nd all your mess
-00007e60: 6167 6573 202d 3e20 606e 6577 5f64 203d  ages -> `new_d =
-00007e70: 2079 6f75 725f 6461 7461 2e6d 6170 284d   your_data.map(M
-00007e80: 6573 7361 6765 4669 656c 6452 6573 6f6c  essageFieldResol
-00007e90: 7665 722e 6578 7061 6e64 5f6d 6573 7361  ver.expand_messa
-00007ea0: 6765 2960 0a20 2020 2020 2020 2032 2e20  ge)`.        2. 
-00007eb0: 5573 6520 6045 7870 616e 6465 644d 6573  Use `ExpandedMes
-00007ec0: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
-00007ed0: 7260 2069 6e73 7465 6164 206f 6620 7573  r` instead of us
-00007ee0: 7561 6c20 604d 6573 7361 6765 4669 656c  ual `MessageFiel
-00007ef0: 6452 6573 6f6c 7665 7260 2077 6865 6e20  dResolver` when 
-00007f00: 0a20 2020 2020 2020 2020 2020 2079 6f75  .            you
-00007f10: 2074 616b 6520 6669 656c 6473 2066 6f72   take fields for
-00007f20: 2065 7870 616e 6465 6420 6d65 7373 6167   expanded messag
-00007f30: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00007f40: 2020 2020 202a 2a49 6d70 6c65 6d65 6e74       **Implement
-00007f50: 6174 696f 6e20 6164 7669 6365 3a2a 2a0a  ation advice:**.
-00007f60: 2020 2020 2020 2020 312e 2072 6169 7365          1. raise
-00007f70: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00007f80: 7272 6f72 202d 2d20 6966 2079 6f75 7220  rror -- if your 
-00007f90: 496d 706c 656d 656e 7461 7469 6f6e 2064  Implementation d
-00007fa0: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00007fb0: 6869 7320 6765 7474 6572 2e0a 2020 2020  his getter..    
-00007fc0: 2020 2020 0a20 2020 2020 2020 202a 2a50      .        **P
-00007fd0: 6572 666f 726d 616e 6365 2069 6d70 6163  erformance impac
-00007fe0: 743a 2a2a 0a20 2020 2020 2020 202d 2049  t:**.        - I
-00007ff0: 7420 6120 6269 7420 736c 6f77 6572 2074  t a bit slower t
-00008000: 6861 6e20 7573 696e 6720 6e61 6b65 6420  han using naked 
-00008010: 6669 656c 6420 6163 6365 7373 2060 6469  field access `di
-00008020: 6374 5b27 6b65 7927 5d60 2e0a 2020 2020  ct['key']`..    
-00008030: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00008040: 322e 342e 204c 696e 6b73 0a20 2020 2020  2.4. Links.     
-00008050: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00008060: 6570 6f72 7420 4461 7461 2050 726f 7669  eport Data Provi
-00008070: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
-00008080: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00008090: 7468 322d 7270 742d 6461 7461 2d70 726f  th2-rpt-data-pro
-000080a0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
-000080b0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
-000080c0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
-000080d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-000080e0: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
-000080f0: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
-00008100: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008110: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
-00008120: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
-00008130: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
-00008140: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
-00008150: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
-00008160: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
-00008170: 2e0a 2020 2020 2020 2020 4173 2077 6974  ..        As wit
-00008180: 6820 6120 7265 6c61 7469 6f6e 616c 2064  h a relational d
-00008190: 6174 6162 6173 652c 2079 6f75 2063 616e  atabase, you can
-000081a0: 2077 7269 7465 2061 2071 7565 7279 2074   write a query t
-000081b0: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
-000081c0: 6461 7461 2073 6c6f 776c 7920 6f72 2071  data slowly or q
-000081d0: 7569 636b 6c79 2c0a 2020 2020 2020 2020  uickly,.        
-000081e0: 7468 6520 7361 6d65 2077 6865 6e20 776f  the same when wo
-000081f0: 726b 696e 6720 7769 7468 2061 2060 4461  rking with a `Da
-00008200: 7461 206f 626a 6563 7460 2e0a 2020 2020  ta object`..    
-00008210: 2020 2020 0a20 2020 2020 2020 2046 6f6c      .        Fol
-00008220: 6c6f 7720 7468 6520 7275 6c65 7320 746f  low the rules to
-00008230: 206d 616b 6520 796f 7572 2077 6f72 6b20   make your work 
-00008240: 7769 7468 2044 6174 6120 6f62 6a65 6374  with Data object
-00008250: 2066 6173 743a 0a20 2020 2020 2020 2031   fast:.        1
-00008260: 2e20 5573 6520 6044 6174 612e 7573 655f  . Use `Data.use_
-00008270: 6361 6368 6528 2960 2069 6620 796f 7520  cache()` if you 
-00008280: 6974 6572 6174 6520 6461 7461 206d 6f72  iterate data mor
-00008290: 6520 7468 616e 206f 6e65 2074 696d 652e  e than one time.
-000082a0: 0a20 2020 2020 2020 2032 2e20 5472 7920  .        2. Try 
-000082b0: 746f 2064 6f6e 2774 2069 7465 7261 7465  to don't iterate
-000082c0: 206f 6e65 2060 4461 7461 206f 626a 6563   one `Data objec
-000082d0: 7460 2069 6e73 6964 6520 7468 6520 6f74  t` inside the ot
-000082e0: 6865 7220 6f6e 652e 0a20 2020 2020 2020  her one..       
-000082f0: 2020 2020 4966 2079 6f75 2073 686f 756c      If you shoul
-00008300: 6420 746f 2064 6f20 6974 2c20 7573 6520  d to do it, use 
-00008310: 7368 6f72 7420 6044 6174 6120 6f62 6a65  short `Data obje
-00008320: 6374 6020 6669 7273 7420 616e 6420 6c6f  ct` first and lo
-00008330: 6e67 2060 4461 7461 206f 626a 6563 7460  ng `Data object`
-00008340: 2069 6e73 6964 6520 7468 6520 6c6f 6f70   inside the loop
-00008350: 2e0a 2020 2020 2020 2020 2020 2049 7427  ..           It'
-00008360: 6c6c 2061 6c6c 6f77 2079 6f75 206f 7065  ll allow you ope
-00008370: 6e20 7468 6520 6361 6368 6520 6669 6c65  n the cache file
-00008380: 206f 7220 6372 6561 7465 2061 2072 6571   or create a req
-00008390: 7565 7374 2074 6f20 6044 6174 6120 736f  uest to `Data so
-000083a0: 7572 6365 6020 6c65 7373 206e 756d 6265  urce` less numbe
-000083b0: 7220 6f66 2074 696d 6573 2e0a 2020 2020  r of times..    
-000083c0: 2020 2020 0a20 2020 2020 2020 2023 2034      .        # 4
-000083d0: 2e20 4f66 6669 6369 616c 2044 6174 6153  . Official DataS
-000083e0: 6f75 7263 6520 696d 706c 656d 656e 7461  ource implementa
-000083f0: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
-00008400: 2020 2020 2020 202d 205b 4c69 6768 7477         - [Lightw
-00008410: 6569 6768 7420 4461 7461 2050 726f 7669  eight Data Provi
-00008420: 6465 7220 4461 7461 2053 6f75 7263 655d  der Data Source]
-00008430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00008440: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
-00008450: 6473 2d73 6f75 7263 652d 6c77 6470 290a  ds-source-lwdp).
-00008460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008470: 200a 2020 2020 2020 2020 2320 352e 2041   .        # 5. A
-00008480: 5049 0a20 2020 2020 2020 200a 2020 2020  PI.        .    
-00008490: 2020 2020 4966 2079 6f75 2061 7265 206c      If you are l
-000084a0: 6f6f 6b69 6e67 2066 6f72 2063 6c61 7373  ooking for class
-000084b0: 6573 2064 6573 6372 6970 7469 6f6e 2073  es description s
-000084c0: 6565 2074 6865 205b 4150 4920 446f 6375  ee the [API Docu
-000084d0: 6d65 6e74 6174 696f 6e5d 2864 6f63 756d  mentation](docum
-000084e0: 656e 7461 7469 6f6e 2f61 7069 2f69 6e64  entation/api/ind
-000084f0: 6578 2e6d 6429 2e0a 2020 2020 2020 2020  ex.md)..        
-00008500: 0a20 2020 2020 2020 2023 2036 2e20 4578  .        # 6. Ex
-00008510: 616d 706c 6573 0a20 2020 2020 2020 200a  amples.        .
-00008520: 2020 2020 2020 2020 2d20 5b67 6574 5f73          - [get_s
-00008530: 7461 7274 6564 5f65 7861 6d70 6c65 2e70  tarted_example.p
-00008540: 795d 2865 7861 6d70 6c65 732f 6765 745f  y](examples/get_
-00008550: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
-00008560: 7079 290a 2020 2020 2020 2020 0a50 6c61  py).        .Pla
-00008570: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a52  tform: UNKNOWN.R
-00008580: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00008590: 3e3d 332e 370a 4465 7363 7269 7074 696f  >=3.7.Descriptio
-000085a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000085b0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-000085c0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-000085d0: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
-000085e0: 3a20 7264 7035 0a50 726f 7669 6465 732d  : rdp5.Provides-
-000085f0: 4578 7472 613a 2072 6470 360a 5072 6f76  Extra: rdp6.Prov
-00008600: 6964 6573 2d45 7874 7261 3a20 6c77 6470  ides-Extra: lwdp
-00008610: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00008620: 206c 7764 7031 0a50 726f 7669 6465 732d   lwdp1.Provides-
-00008630: 4578 7472 613a 206c 7764 7032 0a50 726f  Extra: lwdp2.Pro
-00008640: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
-00008650: 7033 0a50 726f 7669 6465 732d 4578 7472  p3.Provides-Extr
-00008660: 613a 206c 7764 702d 6465 760a 5072 6f76  a: lwdp-dev.Prov
-00008670: 6964 6573 2d45 7874 7261 3a20 7574 696c  ides-Extra: util
-00008680: 732d 7270 742d 7669 6577 6572 0a50 726f  s-rpt-viewer.Pro
-00008690: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-000086a0: 6c73 2d72 7074 2d76 6965 7765 7235 0a50  ls-rpt-viewer5.P
-000086b0: 726f 7669 6465 732d 4578 7472 613a 2075  rovides-Extra: u
-000086c0: 7469 6c73 2d61 6476 616e 6365 640a       tils-advanced.
+00006950: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00006960: 2044 6174 6120 6974 6572 6174 696f 6e0a   Data iteration.
+00006970: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006980: 2054 6865 2044 6174 6120 6f62 6a65 6374   The Data object
+00006990: 2063 6f6e 7374 7275 6374 6f72 206d 6574   constructor met
+000069a0: 686f 6420 7461 6b65 7320 696e 2061 7320  hod takes in as 
+000069b0: 6172 6775 6d65 6e74 2065 6974 6865 7220  argument either 
+000069c0: 616e 2069 7465 7261 746f 7220 6f76 6572  an iterator over
+000069d0: 206f 626a 6563 7473 206f 7220 6120 6765   objects or a ge
+000069e0: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
+000069f0: 2e0a 2020 2020 2020 2020 5468 6520 4461  ..        The Da
+00006a00: 7461 206f 626a 6563 7420 6974 6572 6174  ta object iterat
+00006a10: 6f72 2068 616e 646c 6573 2065 6163 6820  or handles each 
+00006a20: 6974 656d 2069 6e20 7468 6973 2069 7465  item in this ite
+00006a30: 7261 746f 7220 6f72 2067 656e 6572 6174  rator or generat
+00006a40: 6f72 2061 7320 7468 6579 2061 7265 2c20  or as they are, 
+00006a50: 6d65 616e 696e 6720 6974 2064 6f65 736e  meaning it doesn
+00006a60: 2774 2074 7279 2074 6f20 7265 6164 2074  't try to read t
+00006a70: 6865 2063 6f6e 7465 6e74 206f 6620 6974  he content of it
+00006a80: 656d 206f 7220 7265 7475 726e 2074 6865  em or return the
+00006a90: 6d20 6d6f 6469 6669 6564 2069 6e20 616e  m modified in an
+00006aa0: 7920 7761 792c 2069 6e73 7465 6164 2072  y way, instead r
+00006ab0: 6574 7572 6e73 2074 6865 2069 7465 6d20  eturns the item 
+00006ac0: 6974 7365 6c66 2e0a 2020 2020 2020 2020  itself..        
+00006ad0: 5468 6520 6f6e 6c79 2065 7863 6570 7469  The only excepti
+00006ae0: 6f6e 2074 6f20 7468 6973 2069 7320 7768  on to this is wh
+00006af0: 656e 2044 6174 6120 6f62 6a65 6374 2069  en Data object i
+00006b00: 7320 6275 696c 7420 7573 696e 6720 6974  s built using it
+00006b10: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00006b20: 746f 7220 6f76 6572 206f 7468 6572 2044  tor over other D
+00006b30: 6174 6120 6f62 6a65 6374 732e 204e 6f74  ata objects. Not
+00006b40: 6520 7468 6174 2074 6869 7320 6974 6572  e that this iter
+00006b50: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
+00006b60: 7220 6d75 7374 206f 6e6c 7920 6265 2079  r must only be y
+00006b70: 6965 6c64 696e 6720 4461 7461 206f 626a  ielding Data obj
+00006b80: 6563 7473 2061 6e64 206e 6f74 6869 6e67  ects and nothing
+00006b90: 2065 6c73 652e 2049 6620 7765 2062 7569   else. If we bui
+00006ba0: 6c64 2066 726f 6d20 6120 6d69 7820 6f66  ld from a mix of
+00006bb0: 2044 6174 6120 6f62 6a65 6374 7320 616e   Data objects an
+00006bc0: 6420 736f 6d65 206f 7468 6572 2074 7970  d some other typ
+00006bd0: 6573 2c20 4461 7461 206f 626a 6563 7473  es, Data objects
+00006be0: 2720 636f 6e74 656e 7420 776f 6e27 7420  ' content won't 
+00006bf0: 6265 2072 6561 6420 616e 6420 696e 7374  be read and inst
+00006c00: 6561 6420 6974 2077 696c 6c20 6265 2072  ead it will be r
+00006c10: 6574 7572 6e65 6420 6173 2044 6174 6120  eturned as Data 
+00006c20: 6f62 6a65 6374 2069 7473 656c 662e 0a20  object itself.. 
+00006c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006c40: 536d 616c 6c20 6578 616d 706c 6520 746f  Small example to
+00006c50: 2064 656d 6f6e 7374 7261 7465 3a0a 2020   demonstrate:.  
+00006c60: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
+00006c70: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+00006c80: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
+00006c90: 6572 7669 6365 732e 6461 7461 2069 6d70  ervices.data imp
+00006ca0: 6f72 7420 4461 7461 0a20 2020 2020 2020  ort Data.       
+00006cb0: 200a 2020 2020 2020 2020 6431 203d 2044   .        d1 = D
+00006cc0: 6174 6128 5b31 2c32 2c33 5d29 0a20 2020  ata([1,2,3]).   
+00006cd0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
+00006ce0: 342c 352c 365d 290a 2020 2020 2020 2020  4,5,6]).        
+00006cf0: 0a20 2020 2020 2020 206f 6e6c 795f 6461  .        only_da
+00006d00: 7461 5f6f 626a 6563 7473 203d 2044 6174  ta_objects = Dat
+00006d10: 6128 5b64 312c 6432 5d29 2023 2057 696c  a([d1,d2]) # Wil
+00006d20: 6c20 6974 6572 6174 6520 6173 2031 2c32  l iterate as 1,2
+00006d30: 2c33 2c34 2c35 2c36 0a20 2020 2020 2020  ,3,4,5,6.       
+00006d40: 2064 6174 615f 616e 645f 6c69 7374 203d   data_and_list =
+00006d50: 2044 6174 6128 5b64 312c 5b34 2c35 2c36   Data([d1,[4,5,6
+00006d60: 5d5d 2920 2320 5769 6c6c 2069 7465 7261  ]]) # Will itera
+00006d70: 7465 2061 7320 6431 2c20 5b34 2c35 2c36  te as d1, [4,5,6
+00006d80: 5d0a 2020 2020 2020 2020 6461 7461 5f61  ].        data_a
+00006d90: 6e64 5f6e 756d 6265 7273 203d 2044 6174  nd_numbers = Dat
+00006da0: 6128 5b64 312c 342c 352c 365d 2920 2320  a([d1,4,5,6]) # 
+00006db0: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00006dc0: 6431 2c34 2c35 2c36 0a20 2020 2020 2020  d1,4,5,6.       
+00006dd0: 206c 6973 7473 5f6f 6e6c 7920 3d20 4461   lists_only = Da
+00006de0: 7461 285b 312c 322c 335d 2c5b 342c 352c  ta([1,2,3],[4,5,
+00006df0: 365d 2920 2320 5769 6c6c 2069 7465 7261  6]) # Will itera
+00006e00: 7465 2061 7320 5b31 2c32 2c33 5d2c 5b34  te as [1,2,3],[4
+00006e10: 2c35 2c36 5d0a 2020 2020 2020 2020 0a20  ,5,6].        . 
+00006e20: 2020 2020 2020 2023 2049 6620 7765 2077         # If we w
+00006e30: 616e 7420 746f 2069 7465 7261 7465 206f  ant to iterate o
+00006e40: 7665 7220 636f 6e74 656e 7420 6f66 206c  ver content of l
+00006e50: 6973 7420 6f66 206c 6973 7473 2c20 7765  ist of lists, we
+00006e60: 2073 686f 756c 6420 6669 7273 7420 6372   should first cr
+00006e70: 6561 7465 2044 6174 6120 6f62 6a65 6374  eate Data object
+00006e80: 7320 6672 6f6d 2074 6865 6d2c 0a20 2020  s from them,.   
+00006e90: 2020 2020 2023 2074 6865 6e20 7573 6520       # then use 
+00006ea0: 7468 656d 2074 6f20 636f 6e73 7472 7563  them to construc
+00006eb0: 7420 6e65 7720 4461 7461 206f 626a 6563  t new Data objec
+00006ec0: 7420 6173 2069 6e20 6361 7365 206f 6620  t as in case of 
+00006ed0: 6431 2061 6e64 2064 322c 2063 7265 6174  d1 and d2, creat
+00006ee0: 696e 6720 276f 6e6c 795f 6461 7461 5f6f  ing 'only_data_o
+00006ef0: 626a 6563 7473 2720 696e 2074 6869 7320  bjects' in this 
+00006f00: 6578 616d 706c 652e 0a20 2020 2020 2020  example..       
+00006f10: 2060 6060 0a20 2020 2020 2020 2020 0a20   ```.         . 
+00006f20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006f30: 2323 2320 4461 7461 2063 6163 6869 6e67  ### Data caching
+00006f40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006f50: 2020 5468 6520 5f44 6174 6120 6f62 6a65    The _Data obje
+00006f60: 6374 5f20 7072 6f76 6964 6573 2074 6865  ct_ provides the
+00006f70: 2061 6269 6c69 7479 2074 6f20 7573 6520   ability to use 
+00006f80: 7468 6520 6361 6368 652e 2054 6865 2063  the cache. The c
+00006f90: 6163 6865 2077 6f72 6b73 2066 6f72 2065  ache works for e
+00006fa0: 6163 6820 5f44 6174 6120 6f62 6a65 6374  ach _Data object
+00006fb0: 5f2c 2074 6861 7420 6973 2c20 796f 7520  _, that is, you 
+00006fc0: 6368 6f6f 7365 0a20 2020 2020 2020 2077  choose.        w
+00006fd0: 6869 6368 205f 4461 7461 206f 626a 6563  hich _Data objec
+00006fe0: 745f 2079 6f75 2077 616e 7420 746f 2073  t_ you want to s
+00006ff0: 6176 652e 2054 6865 205f 4461 7461 206f  ave. The _Data o
+00007000: 626a 6563 745f 2063 6163 6865 2069 7320  bject_ cache is 
+00007010: 7361 7665 6420 6166 7465 7220 7468 6520  saved after the 
+00007020: 6669 7273 7420 6974 6572 6174 696f 6e2c  first iteration,
+00007030: 2062 7574 2074 6865 2069 7465 7261 7469   but the iterati
+00007040: 6f6e 0a20 2020 2020 2020 2073 6f75 7263  on.        sourc
+00007050: 6520 6d61 7920 6265 2064 6966 6665 7265  e may be differe
+00007060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
+00007070: 2020 2020 2049 6620 796f 7520 646f 6e27       If you don'
+00007080: 7420 7573 6520 7468 6520 6361 6368 652c  t use the cache,
+00007090: 2079 6f75 7220 736f 7572 6365 2077 696c   your source wil
+000070a0: 6c20 6265 2074 6865 2064 6174 6120 736f  l be the data so
+000070b0: 7572 6365 2079 6f75 2068 6176 6520 696e  urce you have in
+000070c0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
+000070d0: 745f 2e20 4275 7420 6966 2079 6f75 2075  t_. But if you u
+000070e0: 7365 2074 6865 2063 6163 6865 2c0a 2020  se the cache,.  
+000070f0: 2020 2020 2020 796f 7572 2073 6f75 7263        your sourc
+00007100: 6520 6361 6e20 6265 2074 6865 2064 6174  e can be the dat
+00007110: 6120 736f 7572 6365 2c20 7468 6520 7061  a source, the pa
+00007120: 7265 6e74 2063 6163 6865 2c20 6f72 206f  rent cache, or o
+00007130: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
+00007140: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
+00007150: 2064 6174 6120 736f 7572 6365 3a0a 2020   data source:.  
+00007160: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
+00007170: 4461 7461 204f 626a 6563 745f 2064 6f65  Data Object_ doe
+00007180: 736e 2774 2068 6176 6520 6120 7061 7265  sn't have a pare
+00007190: 6e74 2063 6163 6865 2061 6e64 2069 7473  nt cache and its
+000071a0: 2063 6163 6865 2e0a 2020 2020 2020 2020   cache..        
+000071b0: 2a20 5468 6520 7061 7265 6e74 2063 6163  * The parent cac
+000071c0: 6865 3a0a 2020 2020 2020 2020 2020 4966  he:.          If
+000071d0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
+000071e0: 745f 2068 6173 2061 2070 6172 656e 7420  t_ has a parent 
+000071f0: 6361 6368 652e 2049 7420 646f 6573 6e27  cache. It doesn'
+00007200: 7420 6d61 7474 6572 2077 6861 7420 706f  t matter what po
+00007210: 7369 7469 6f6e 2074 6865 2070 6172 656e  sition the paren
+00007220: 7420 6361 6368 6520 6861 7320 696e 2069  t cache has in i
+00007230: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
+00007240: 2020 2020 2020 5f44 6174 6120 4f62 6a65        _Data Obje
+00007250: 6374 5f20 756e 6465 7273 7461 6e64 7320  ct_ understands 
+00007260: 7768 6f73 6520 6361 6368 6520 6974 2069  whose cache it i
+00007270: 7320 616e 6420 6578 6563 7574 6573 2074  s and executes t
+00007280: 6865 2070 6172 7420 6f66 2074 6865 2077  he part of the w
+00007290: 6f72 6b66 6c6f 7720 7468 6174 2077 6173  orkflow that was
+000072a0: 206e 6f74 2065 7865 6375 7465 642e 0a20   not executed.. 
+000072b0: 2020 2020 2020 202a 2054 6865 206f 776e         * The own
+000072c0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
+000072d0: 2020 4966 2069 7420 6973 206e 6f74 2074    If it is not t
+000072e0: 6865 2066 6972 7374 2069 7465 7261 7469  he first iterati
+000072f0: 6f6e 206f 6620 7468 6973 2044 6174 6120  on of this Data 
+00007300: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00007310: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
+00007320: 6174 2074 6865 2063 6163 6865 2073 7461  at the cache sta
+00007330: 7465 206f 6620 7468 6520 4461 7461 206f  te of the Data o
+00007340: 626a 6563 7420 6973 206e 6f74 2069 6e68  bject is not inh
+00007350: 6572 6974 6564 2e0a 2020 2020 2020 2020  erited..        
+00007360: 0a20 2020 2020 2020 2023 2323 2320 466f  .        #### Fo
+00007370: 7263 6564 2063 6163 6869 6e67 0a20 2020  rced caching.   
+00007380: 2020 2020 2059 6f75 2063 616e 2074 656c       You can tel
+00007390: 6c20 4453 2074 6f20 6361 6368 6520 6461  l DS to cache da
+000073a0: 7461 2074 6f20 7370 6563 6966 6963 2063  ta to specific c
+000073b0: 6163 6865 2066 696c 652c 2077 6869 6368  ache file, which
+000073c0: 2077 6f6e 2774 2062 6520 6465 6c65 7465   won't be delete
+000073d0: 6420 6166 7465 7220 7363 7269 7074 2065  d after script e
+000073e0: 6e64 2e0a 2020 2020 2020 2020 596f 7520  nd..        You 
+000073f0: 6361 6e20 7365 6520 6578 616d 706c 6520  can see example 
+00007400: 696e 2031 2e31 3220 7365 6374 696f 6e20  in 1.12 section 
+00007410: 6f66 205b 6765 745f 7374 6172 7465 645f  of [get_started_
+00007420: 6578 616d 706c 655d 2865 7861 6d70 6c65  example](example
+00007430: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
+00007440: 616d 706c 652e 7079 292e 0a20 2020 2020  ample.py)..     
+00007450: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00007460: 2020 2020 2023 2323 2045 7665 6e74 5472       ### EventTr
+00007470: 6565 2061 6e64 2063 6f6c 6c65 6374 696f  ee and collectio
+00007480: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
+00007490: 2020 2020 2323 2323 2045 7665 6e74 5472      #### EventTr
+000074a0: 6565 0a20 2020 2020 2020 200a 2020 2020  ee.        .    
+000074b0: 2020 2020 6045 7665 6e74 5472 6565 6020      `EventTree` 
+000074c0: 6973 2061 2074 7265 652d 6261 7365 6420  is a tree-based 
+000074d0: 6461 7461 2073 7472 7563 7475 7265 206f  data structure o
+000074e0: 6620 6576 656e 7473 2e20 4974 2061 6c6c  f events. It all
+000074f0: 6f77 7320 796f 7520 6765 7420 6368 696c  ows you get chil
+00007500: 6472 656e 2061 6e64 2070 6172 656e 7473  dren and parents
+00007510: 206f 6620 6576 656e 742c 0a20 2020 2020   of event,.     
+00007520: 2020 2064 6973 706c 6179 2074 7265 652c     display tree,
+00007530: 2067 6574 2066 756c 6c20 7061 7468 2074   get full path t
+00007540: 6f20 6576 656e 7420 6574 632e 0a20 2020  o event etc..   
+00007550: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
+00007560: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
+00007570: 2020 2020 2020 2020 2a20 6045 7665 6e74          * `Event
+00007580: 5472 6565 6020 636f 6e74 6169 6e73 2061  Tree` contains a
+00007590: 6c6c 2065 7665 6e74 7320 696e 206d 656d  ll events in mem
+000075a0: 6f72 792e 0a20 2020 2020 2020 202a 2054  ory..        * T
+000075b0: 7265 6520 6861 7320 736f 6d65 2069 6d70  ree has some imp
+000075c0: 6f72 7461 6e74 2074 6572 6d73 3a0a 2020  ortant terms:.  
+000075d0: 2020 2020 2020 2020 2020 312e 205f 416e            1. _An
+000075e0: 6365 7374 6f72 5f20 6973 2061 6e79 2072  cestor_ is any r
+000075f0: 656c 6174 6976 6520 6f66 2074 6865 2065  elative of the e
+00007600: 7665 6e74 2075 7020 7468 6520 7472 6565  vent up the tree
+00007610: 2028 6772 616e 6470 6172 656e 742c 2070   (grandparent, p
+00007620: 6172 656e 7420 6574 632e 292e 0a20 2020  arent etc.)..   
+00007630: 2020 2020 2020 2020 2032 2e20 5f50 6172           2. _Par
+00007640: 656e 745f 2069 7320 6f6e 6c79 2074 6865  ent_ is only the
+00007650: 2066 6972 7374 2072 656c 6174 6976 6520   first relative 
+00007660: 6f66 2074 6865 2065 7665 6e74 2075 7020  of the event up 
+00007670: 7468 6520 7472 6565 2e0a 2020 2020 2020  the tree..      
+00007680: 2020 2020 2020 332e 205f 4368 696c 645f        3. _Child_
+00007690: 2069 7320 7468 6520 6669 7273 7420 7265   is the first re
+000076a0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+000076b0: 656e 7420 646f 776e 2074 6865 2074 7265  ent down the tre
+000076c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+000076d0: 2020 2020 5461 6b65 2061 206c 6f6f 6b20      Take a look 
+000076e0: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
+000076f0: 2048 544d 4c20 7472 6565 2074 6f20 756e   HTML tree to un
+00007700: 6465 7273 7461 6e64 2074 6865 6d2e 0a20  derstand them.. 
+00007710: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007720: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
+00007730: 2020 203c 626f 6479 3e20 3c21 2d2d 2061     <body> <!-- a
+00007740: 6e63 6573 746f 7220 2867 7261 6e64 7061  ncestor (grandpa
+00007750: 7265 6e74 292c 2062 7574 206e 6f74 2070  rent), but not p
+00007760: 6172 656e 7420 2d2d 3e0a 2020 2020 2020  arent -->.      
+00007770: 2020 2020 2020 2020 2020 3c64 6976 3e20            <div> 
+00007780: 3c21 2d2d 2070 6172 656e 7420 2620 616e  <!-- parent & an
+00007790: 6365 7374 6f72 202d 2d3e 0a20 2020 2020  cestor -->.     
+000077a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000077b0: 703e 4865 6c6c 6f2c 2077 6f72 6c64 213c  p>Hello, world!<
+000077c0: 2f70 3e20 3c21 2d2d 2063 6869 6c64 202d  /p> <!-- child -
+000077d0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+000077e0: 2020 2020 2020 203c 703e 476f 6f64 6279         <p>Goodby
+000077f0: 6521 3c2f 703e 203c 212d 2d20 7369 626c  e!</p> <!-- sibl
+00007800: 696e 6720 2d2d 3e0a 2020 2020 2020 2020  ing -->.        
+00007810: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00007820: 2020 2020 2020 2020 2020 203c 2f62 6f64             </bod
+00007830: 793e 0a20 2020 2020 2020 2020 2020 6060  y>.           ``
+00007840: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+00007850: 2020 2023 2323 2320 436f 6c6c 6563 7469     #### Collecti
+00007860: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00007870: 2020 2020 202a 2a45 7665 6e74 5472 6565       **EventTree
+00007880: 436f 6c6c 6563 7469 6f6e 2a2a 2069 7320  Collection** is 
+00007890: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
+000078a0: 4576 656e 7454 7265 6573 2e20 5468 6520  EventTrees. The 
+000078b0: 636f 6c6c 6563 7469 6f6e 2062 7569 6c64  collection build
+000078c0: 7320 6120 6665 7720 5f45 7665 6e74 5472  s a few _EventTr
+000078d0: 6565 5f20 6279 2070 6173 7365 6420 5f44  ee_ by passed _D
+000078e0: 6174 610a 2020 2020 2020 2020 6f62 6a65  ata.        obje
+000078f0: 6374 5f2e 2041 6c74 686f 7567 6820 796f  ct_. Although yo
+00007900: 7520 6361 6e20 6368 616e 6765 2074 6865  u can change the
+00007910: 2074 7265 6520 6469 7265 6374 6c79 2c20   tree directly, 
+00007920: 6974 2773 2062 6574 7465 7220 746f 2064  it's better to d
+00007930: 6f20 6974 2074 6872 6f75 6768 2063 6f6c  o it through col
+00007940: 6c65 6374 696f 6e73 2062 6563 6175 7365  lections because
+00007950: 2074 6865 7920 6172 6520 6177 6172 6520   they are aware 
+00007960: 6f66 0a20 2020 2020 2020 2060 6465 7461  of.        `deta
+00007970: 6368 6564 5f65 7665 6e74 7360 2061 6e64  ched_events` and
+00007980: 2063 616e 2073 6f6c 7665 2073 6f6d 6520   can solve some 
+00007990: 6576 656e 7473 2064 6570 656e 6465 6e63  events dependenc
+000079a0: 6965 732e 2054 6865 2063 6f6c 6c65 6374  ies. The collect
+000079b0: 696f 6e20 6861 7320 7369 6d69 6c61 7220  ion has similar 
+000079c0: 6665 6174 7572 6573 206c 696b 6520 6120  features like a 
+000079d0: 7369 6e67 6c65 205f 4576 656e 7454 7265  single _EventTre
+000079e0: 655f 0a20 2020 2020 2020 2062 7574 2061  e_.        but a
+000079f0: 7070 6c79 696e 6720 7468 656d 2066 6f72  pplying them for
+00007a00: 2061 6c6c 205f 4576 656e 7454 7265 6573   all _EventTrees
+00007a10: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
+00007a20: 2020 2020 2a2a 5061 7265 6e74 4576 656e      **ParentEven
+00007a30: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
+00007a40: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
+00007a50: 6e20 7369 6d69 6c61 7220 746f 205f 4576  n similar to _Ev
+00007a60: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00007a70: 6e5f 2062 7574 2063 6f6e 7461 696e 696e  n_ but containin
+00007a80: 6720 6f6e 6c79 2070 6172 656e 7420 6576  g only parent ev
+00007a90: 656e 7473 2074 6861 740a 2020 2020 2020  ents that.      
+00007aa0: 2020 6172 6520 7265 6665 7265 6e63 6564    are referenced
+00007ab0: 2069 6e20 7468 6520 6461 7461 2073 7472   in the data str
+00007ac0: 6561 6d2e 2054 6865 2063 6f6c 6c65 6374  eam. The collect
+00007ad0: 696f 6e20 6861 7320 6665 6174 7572 6573  ion has features
+00007ae0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
+00007af0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00007b00: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
+00007b10: 2020 2020 4465 7461 696c 733a 0a20 2020      Details:.   
+00007b20: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
+00007b30: 546f 2075 7365 2045 5420 636f 6c6c 6563  To use ET collec
+00007b40: 7469 6f6e 7320 796f 7520 6e65 6564 2074  tions you need t
+00007b50: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
+00007b60: 6d20 6279 205f 4554 4344 7269 7665 725f  m by _ETCDriver_
+00007b70: 2e20 4461 7461 2073 6f75 7263 6573 2075  . Data sources u
+00007b80: 7375 616c 6c79 2070 726f 7669 6465 2074  sually provide t
+00007b90: 6865 6d2e 0a20 2020 2020 2020 2020 2059  hem..          Y
+00007ba0: 6f75 2063 616e 2063 7265 6174 6520 6974  ou can create it
+00007bb0: 2062 7920 796f 7572 7365 6c66 2064 6570   by yourself dep
+00007bc0: 656e 6469 6e67 206f 6e20 796f 7572 2064  ending on your d
+00007bd0: 6174 6120 7374 7275 6374 7572 652e 0a20  ata structure.. 
+00007be0: 2020 2020 2020 202a 2054 6865 2063 6f6c         * The col
+00007bf0: 6c65 6374 696f 6e20 6861 7320 6120 6665  lection has a fe
+00007c00: 6174 7572 6520 746f 2072 6563 6f76 6572  ature to recover
+00007c10: 2065 7665 6e74 732e 2041 6c6c 2065 7665   events. All eve
+00007c20: 6e74 7320 7468 6174 2061 7265 206e 6f74  nts that are not
+00007c30: 2069 6e20 7468 6520 7265 6365 6976 6564   in the received
+00007c40: 2064 6174 6120 7374 7265 616d 2c20 6275   data stream, bu
+00007c50: 7420 7768 6963 6820 6172 650a 2020 2020  t which are.    
+00007c60: 2020 2020 2020 7265 6665 7265 6e63 6564        referenced
+00007c70: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
+00007c80: 6672 6f6d 2074 6865 2064 6174 6120 736f  from the data so
+00007c90: 7572 6365 2e0a 2020 2020 2020 2020 2a20  urce..        * 
+00007ca0: 596f 7520 6361 6e20 7461 6b65 2060 6465  You can take `de
+00007cb0: 7461 6368 6564 5f65 7665 6e74 7360 2074  tached_events` t
+00007cc0: 6f20 7365 6520 7768 6963 6820 6576 656e  o see which even
+00007cd0: 7473 2061 7265 206d 6973 7369 6e67 2e0a  ts are missing..
+00007ce0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
+00007cf0: 2077 616e 742c 2079 6f75 2063 616e 2062   want, you can b
+00007d00: 7569 6c64 2070 6172 656e 746c 6573 7320  uild parentless 
+00007d10: 7472 6565 7320 7768 6572 6520 7468 6520  trees where the 
+00007d20: 6d69 7373 696e 6720 6576 656e 7473 2061  missing events a
+00007d30: 7265 2073 7475 6262 6564 2069 6e73 7465  re stubbed inste
+00007d40: 6164 2e20 4a75 7374 0a20 2020 2020 2020  ad. Just.       
+00007d50: 2020 2075 7365 2060 6765 745f 7061 7265     use `get_pare
+00007d60: 6e74 6c65 7373 5f74 7265 6573 2829 602e  ntless_trees()`.
+00007d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00007d80: 2020 5265 7175 6972 656d 656e 7473 3a0a    Requirements:.
+00007d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007da0: 2031 2e20 4576 656e 7473 2070 726f 7669   1. Events provi
+00007db0: 6465 6420 746f 2045 5443 2068 6176 6520  ded to ETC have 
+00007dc0: 746f 2068 6176 6520 6065 7665 6e74 5f6e  to have `event_n
+00007dd0: 616d 6560 2c20 6065 7665 6e74 5f69 6460  ame`, `event_id`
+00007de0: 2c20 6070 6172 656e 745f 6576 656e 745f  , `parent_event_
+00007df0: 6964 6020 6669 656c 6473 2e20 5468 6579  id` fields. They
+00007e00: 0a20 2020 2020 2020 2063 616e 2068 6176  .        can hav
+00007e10: 6520 616e 6f74 6865 7220 6e61 6d65 7320  e another names 
+00007e20: 2869 7420 7265 736f 6c76 6573 2069 6e20  (it resolves in 
+00007e30: 7468 6520 6472 6976 6572 292e 0a20 2020  the driver)..   
+00007e40: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00007e50: 2323 2048 696e 7473 0a20 2020 2020 2020  ## Hints.       
+00007e60: 200a 2020 2020 2020 2020 2a20 5265 6d6f   .        * Remo
+00007e70: 7665 2061 6c6c 2075 6e6e 6563 6573 7361  ve all unnecessa
+00007e80: 7279 2066 6965 6c64 7320 6672 6f6d 2065  ry fields from e
+00007e90: 7665 6e74 7320 6265 666f 7265 2070 6173  vents before pas
+00007ea0: 7369 6e67 2074 6f20 6120 5f63 6f6c 6c65  sing to a _colle
+00007eb0: 6374 696f 6e5f 2074 6f20 7265 6475 6365  ction_ to reduce
+00007ec0: 206d 656d 6f72 7920 7573 6167 652e 0a20   memory usage.. 
+00007ed0: 2020 2020 2020 202a 2055 7365 2060 7368         * Use `sh
+00007ee0: 6f77 2829 6020 6d65 7468 6f64 2074 6f20  ow()` method to 
+00007ef0: 7072 696e 7420 7468 6520 7472 6565 2069  print the tree i
+00007f00: 6e20 7472 6565 2d6c 696b 6520 7669 6577  n tree-like view
+00007f10: 2e0a 2020 2020 2020 2020 2a20 4e6f 7465  ..        * Note
+00007f20: 2074 6861 7420 7468 6520 6067 6574 5f78   that the `get_x
+00007f30: 6020 6d65 7468 6f64 7320 7769 6c6c 2072  ` methods will r
+00007f40: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+00007f50: 6e20 6966 2079 6f75 2070 6173 7320 616e  n if you pass an
+00007f60: 2075 6e6b 6e6f 776e 2065 7665 6e74 2069   unknown event i
+00007f70: 642c 2075 6e6c 696b 6520 7468 6520 6066  d, unlike the `f
+00007f80: 696e 645f 7860 206d 6574 686f 6473 2028  ind_x` methods (
+00007f90: 0a20 2020 2020 2020 2020 2074 6865 7920  .          they 
+00007fa0: 7265 7475 726e 204e 6f6e 6529 2e0a 2020  return None)..  
+00007fb0: 2020 2020 2020 2a20 4966 2079 6f75 2077        * If you w
+00007fc0: 616e 7420 746f 206b 6e6f 7720 7468 6174  ant to know that
+00007fd0: 2073 7065 6369 6669 6564 2065 7665 6e74   specified event
+00007fe0: 2065 7869 7374 732c 2075 7365 2074 6865   exists, use the
+00007ff0: 2070 7974 686f 6e20 6069 6e60 206b 6579   python `in` key
+00008000: 776f 7264 2028 652e 672e 2060 2765 7665  word (e.g. `'eve
+00008010: 6e74 2d69 6427 2069 6e20 6576 656e 7473  nt-id' in events
+00008020: 5f74 7265 6560 292e 0a20 2020 2020 2020  _tree`)..       
+00008030: 202a 2055 7365 2074 6865 2070 7974 686f   * Use the pytho
+00008040: 6e20 606c 656e 6020 6b65 7977 6f72 6420  n `len` keyword 
+00008050: 746f 2067 6574 2065 7665 6e74 7320 6e75  to get events nu
+00008060: 6d62 6572 2069 6e20 7468 6520 7472 6565  mber in the tree
+00008070: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008080: 2020 2023 2323 2046 6965 6c64 2052 6573     ### Field Res
+00008090: 6f6c 7665 7273 0a20 2020 2020 2020 2049  olvers.        I
+000080a0: 6e74 6572 6661 6365 2063 616e 2062 6520  nterface can be 
+000080b0: 666f 756e 6420 696e 2060 7468 325f 6461  found in `th2_da
+000080c0: 7461 5f73 6572 7669 6365 732f 696e 7465  ta_services/inte
+000080d0: 7266 6163 6573 2f75 7469 6c73 2f72 6573  rfaces/utils/res
+000080e0: 6f6c 7665 722e 7079 602e 2020 0a20 2020  olver.py`.  .   
+000080f0: 2020 2020 2041 6c6c 2064 6174 612d 736f       All data-so
+00008100: 7572 6365 7320 7368 6f75 6c64 2069 6d70  urces should imp
+00008110: 6c65 6d65 6e74 2074 6865 6d2e 0a20 2020  lement them..   
+00008120: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00008130: 6520 6964 6561 206f 6620 7573 696e 6720  e idea of using 
+00008140: 7265 736f 6c76 6572 733a 0a20 2020 2020  resolvers:.     
+00008150: 2020 2049 7420 736f 6c76 6573 2074 6865     It solves the
+00008160: 2070 726f 626c 656d 206f 6620 6861 7669   problem of havi
+00008170: 6e67 2061 2066 6577 2044 6174 6153 6f75  ng a few DataSou
+00008180: 7263 6573 2077 6974 6820 7369 6d69 6c61  rces with simila
+00008190: 7220 6461 7461 2c0a 2020 2020 2020 2020  r data,.        
+000081a0: 6275 7420 7769 7468 2064 6966 6665 7265  but with differe
+000081b0: 6e74 2077 6179 7320 746f 2067 6574 2069  nt ways to get i
+000081c0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
+000081d0: 2020 2020 5468 6573 6520 636c 6173 7365      These classe
+000081e0: 7320 7072 6f76 6964 6520 796f 7520 6765  s provide you ge
+000081f0: 7474 6572 206d 6574 686f 6473 2e0a 2020  tter methods..  
+00008200: 2020 2020 2020 5573 696e 6720 7468 6573        Using thes
+00008210: 6520 636c 6173 7365 7320 616c 6c6f 7773  e classes allows
+00008220: 2079 6f75 2074 6f20 6672 6565 6c79 2073   you to freely s
+00008230: 7769 7463 6820 6265 7477 6565 6e20 6469  witch between di
+00008240: 6666 6572 656e 7420 6461 7461 0a20 2020  fferent data.   
+00008250: 2020 2020 2066 6f72 6d61 7473 2061 6e64       formats and
+00008260: 2064 6f6e 2774 2063 6861 6e67 6520 796f   don't change yo
+00008270: 7572 2063 6f64 652e 0a20 2020 2020 2020  ur code..       
+00008280: 200a 2020 2020 2020 2020 5265 736f 6c76   .        Resolv
+00008290: 6572 7320 736f 6c76 6520 7468 6520 7072  ers solve the pr
+000082a0: 6f62 6c65 6d20 6f66 2064 6174 612d 666f  oblem of data-fo
+000082b0: 726d 6174 206d 6967 7261 7469 6f6e 2e0a  rmat migration..
+000082c0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
+000082d0: 2070 6c61 6365 2063 616e 2062 6520 6368   place can be ch
+000082e0: 616e 6765 640a 2020 2020 2020 2020 2d20  anged.        - 
+000082f0: 6669 656c 6473 206e 616d 6573 2063 616e  fields names can
+00008300: 2062 6520 6368 616e 6765 640a 2020 2020   be changed.    
+00008310: 2020 2020 0a20 2020 2020 2020 2052 6573      .        Res
+00008320: 6f6c 7665 7273 2063 616e 2077 6f72 6b20  olvers can work 
+00008330: 6f6e 6c79 2077 6974 6820 6f6e 6520 6576  only with one ev
+00008340: 656e 742f 6d65 7373 6167 652e 0a20 2020  ent/message..   
+00008350: 2020 2020 2049 7420 6d65 616e 732c 2069       It means, i
+00008360: 6620 796f 7572 206d 6573 7361 6765 2068  f your message h
+00008370: 6173 2073 7562 2d6d 6573 7361 6765 7320  as sub-messages 
+00008380: 286c 696b 6520 7468 322d 6d65 7373 6167  (like th2-messag
+00008390: 6573 2069 6e20 6c77 6470 2920 6974 200a  es in lwdp) it .
+000083a0: 2020 2020 2020 2020 776f 6e27 7420 776f          won't wo
+000083b0: 726b 2c20 6265 6361 7573 6520 7265 736f  rk, because reso
+000083c0: 6c76 6572 2077 696c 6c20 6e6f 7420 6b6e  lver will not kn
+000083d0: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
+000083e0: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
+000083f0: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
+00008400: 2020 200a 2020 2020 2020 2020 2a2a 576f     .        **Wo
+00008410: 726b 6172 6f75 6e64 2a2a 2020 0a20 2020  rkaround**  .   
+00008420: 2020 2020 2031 2e20 4578 7061 6e64 2061       1. Expand a
+00008430: 6c6c 2079 6f75 7220 6d65 7373 6167 6573  ll your messages
+00008440: 202d 3e20 606e 6577 5f64 203d 2079 6f75   -> `new_d = you
+00008450: 725f 6461 7461 2e6d 6170 284d 6573 7361  r_data.map(Messa
+00008460: 6765 4669 656c 6452 6573 6f6c 7665 722e  geFieldResolver.
+00008470: 6578 7061 6e64 5f6d 6573 7361 6765 2960  expand_message)`
+00008480: 0a20 2020 2020 2020 2032 2e20 5573 6520  .        2. Use 
+00008490: 6045 7870 616e 6465 644d 6573 7361 6765  `ExpandedMessage
+000084a0: 4669 656c 6452 6573 6f6c 7665 7260 2069  FieldResolver` i
+000084b0: 6e73 7465 6164 206f 6620 7573 7561 6c20  nstead of usual 
+000084c0: 604d 6573 7361 6765 4669 656c 6452 6573  `MessageFieldRes
+000084d0: 6f6c 7665 7260 2077 6865 6e20 0a20 2020  olver` when .   
+000084e0: 2020 2020 2020 2020 2079 6f75 2074 616b           you tak
+000084f0: 6520 6669 656c 6473 2066 6f72 2065 7870  e fields for exp
+00008500: 616e 6465 6420 6d65 7373 6167 6573 2e0a  anded messages..
+00008510: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008520: 202a 2a49 6d70 6c65 6d65 6e74 6174 696f   **Implementatio
+00008530: 6e20 6164 7669 6365 3a2a 2a0a 2020 2020  n advice:**.    
+00008540: 2020 2020 312e 2072 6169 7365 204e 6f74      1. raise Not
+00008550: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00008560: 202d 2d20 6966 2079 6f75 7220 496d 706c   -- if your Impl
+00008570: 656d 656e 7461 7469 6f6e 2064 6f65 736e  ementation doesn
+00008580: 2774 2073 7570 706f 7274 2074 6869 7320  't support this 
+00008590: 6765 7474 6572 2e0a 2020 2020 2020 2020  getter..        
+000085a0: 0a20 2020 2020 2020 202a 2a50 6572 666f  .        **Perfo
+000085b0: 726d 616e 6365 2069 6d70 6163 743a 2a2a  rmance impact:**
+000085c0: 0a20 2020 2020 2020 202d 2049 7420 6120  .        - It a 
+000085d0: 6269 7420 736c 6f77 6572 2074 6861 6e20  bit slower than 
+000085e0: 7573 696e 6720 6e61 6b65 6420 6669 656c  using naked fiel
+000085f0: 6420 6163 6365 7373 2060 6469 6374 5b27  d access `dict['
+00008600: 6b65 7927 5d60 2e0a 2020 2020 2020 2020  key']`..        
+00008610: 0a20 2020 2020 2020 2023 2320 322e 342e  .        ## 2.4.
+00008620: 204c 696e 6b73 0a20 2020 2020 2020 200a   Links.        .
+00008630: 2020 2020 2020 2020 2d20 5b52 6570 6f72          - [Repor
+00008640: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
+00008650: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00008660: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+00008670: 7270 742d 6461 7461 2d70 726f 7669 6465  rpt-data-provide
+00008680: 7229 0a20 2020 2020 2020 202d 205b 5468  r).        - [Th
+00008690: 3220 4461 7461 2053 6572 7669 6365 7320  2 Data Services 
+000086a0: 5574 696c 735d 2868 7474 7073 3a2f 2f67  Utils](https://g
+000086b0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
+000086c0: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
+000086d0: 6365 732d 7574 696c 7329 0a20 2020 2020  ces-utils).     
+000086e0: 2020 200a 2020 2020 2020 2020 2320 332e     .        # 3.
+000086f0: 2042 6573 7420 7072 6163 7469 6365 730a   Best practices.
+00008700: 2020 2020 2020 2020 4465 7065 6e64 696e          Dependin
+00008710: 6720 6f6e 2068 6f77 2079 6f75 2077 6f72  g on how you wor
+00008720: 6b20 7769 7468 2060 4461 7461 206f 626a  k with `Data obj
+00008730: 6563 7460 2c20 6974 2063 616e 2062 6520  ect`, it can be 
+00008740: 736c 6f77 206f 6620 6661 7374 2e0a 2020  slow of fast..  
+00008750: 2020 2020 2020 4173 2077 6974 6820 6120        As with a 
+00008760: 7265 6c61 7469 6f6e 616c 2064 6174 6162  relational datab
+00008770: 6173 652c 2079 6f75 2063 616e 2077 7269  ase, you can wri
+00008780: 7465 2061 2071 7565 7279 2074 6861 7420  te a query that 
+00008790: 7769 6c6c 2072 6574 7572 6e20 6461 7461  will return data
+000087a0: 2073 6c6f 776c 7920 6f72 2071 7569 636b   slowly or quick
+000087b0: 6c79 2c0a 2020 2020 2020 2020 7468 6520  ly,.        the 
+000087c0: 7361 6d65 2077 6865 6e20 776f 726b 696e  same when workin
+000087d0: 6720 7769 7468 2061 2060 4461 7461 206f  g with a `Data o
+000087e0: 626a 6563 7460 2e0a 2020 2020 2020 2020  bject`..        
+000087f0: 0a20 2020 2020 2020 2046 6f6c 6c6f 7720  .        Follow 
+00008800: 7468 6520 7275 6c65 7320 746f 206d 616b  the rules to mak
+00008810: 6520 796f 7572 2077 6f72 6b20 7769 7468  e your work with
+00008820: 2044 6174 6120 6f62 6a65 6374 2066 6173   Data object fas
+00008830: 743a 0a20 2020 2020 2020 2031 2e20 5573  t:.        1. Us
+00008840: 6520 6044 6174 612e 7573 655f 6361 6368  e `Data.use_cach
+00008850: 6528 2960 2069 6620 796f 7520 6974 6572  e()` if you iter
+00008860: 6174 6520 6461 7461 206d 6f72 6520 7468  ate data more th
+00008870: 616e 206f 6e65 2074 696d 652e 0a20 2020  an one time..   
+00008880: 2020 2020 2032 2e20 5472 7920 746f 2064       2. Try to d
+00008890: 6f6e 2774 2069 7465 7261 7465 206f 6e65  on't iterate one
+000088a0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
+000088b0: 6e73 6964 6520 7468 6520 6f74 6865 7220  nside the other 
+000088c0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+000088d0: 4966 2079 6f75 2073 686f 756c 6420 746f  If you should to
+000088e0: 2064 6f20 6974 2c20 7573 6520 7368 6f72   do it, use shor
+000088f0: 7420 6044 6174 6120 6f62 6a65 6374 6020  t `Data object` 
+00008900: 6669 7273 7420 616e 6420 6c6f 6e67 2060  first and long `
+00008910: 4461 7461 206f 626a 6563 7460 2069 6e73  Data object` ins
+00008920: 6964 6520 7468 6520 6c6f 6f70 2e0a 2020  ide the loop..  
+00008930: 2020 2020 2020 2020 2049 7427 6c6c 2061           It'll a
+00008940: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
+00008950: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
+00008960: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
+00008970: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
+00008980: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
+00008990: 2074 696d 6573 2e0a 2020 2020 2020 2020   times..        
+000089a0: 0a20 2020 2020 2020 2023 2034 2e20 4f66  .        # 4. Of
+000089b0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
+000089c0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000089d0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+000089e0: 2020 202d 205b 4c69 6768 7477 6569 6768     - [Lightweigh
+000089f0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
+00008a00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
+00008a10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008a20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
+00008a30: 6f75 7263 652d 6c77 6470 290a 2020 2020  ource-lwdp).    
+00008a40: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+00008a50: 2020 2020 2020 2320 352e 2041 5049 0a20        # 5. API. 
+00008a60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008a70: 4966 2079 6f75 2061 7265 206c 6f6f 6b69  If you are looki
+00008a80: 6e67 2066 6f72 2063 6c61 7373 6573 2064  ng for classes d
+00008a90: 6573 6372 6970 7469 6f6e 2073 6565 2074  escription see t
+00008aa0: 6865 205b 4150 4920 446f 6375 6d65 6e74  he [API Document
+00008ab0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
+00008ac0: 7469 6f6e 2f61 7069 2f69 6e64 6578 2e6d  tion/api/index.m
+00008ad0: 6429 2e0a 2020 2020 2020 2020 0a20 2020  d)..        .   
+00008ae0: 2020 2020 2023 2036 2e20 4578 616d 706c       # 6. Exampl
+00008af0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+00008b00: 2020 2020 2d20 5b67 6574 5f73 7461 7274      - [get_start
+00008b10: 6564 5f65 7861 6d70 6c65 2e70 795d 2865  ed_example.py](e
+00008b20: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
+00008b30: 7465 645f 6578 616d 706c 652e 7079 290a  ted_example.py).
+00008b40: 2020 2020 2020 2020 0a50 6c61 7466 6f72          .Platfor
+00008b50: 6d3a 2055 4e4b 4e4f 574e 0a52 6571 7569  m: UNKNOWN.Requi
+00008b60: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+00008b70: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
+00008b80: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00008b90: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
+00008ba0: 6573 2d45 7874 7261 3a20 7264 700a 5072  es-Extra: rdp.Pr
+00008bb0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
+00008bc0: 7035 0a50 726f 7669 6465 732d 4578 7472  p5.Provides-Extr
+00008bd0: 613a 2072 6470 360a 5072 6f76 6964 6573  a: rdp6.Provides
+00008be0: 2d45 7874 7261 3a20 6c77 6470 0a50 726f  -Extra: lwdp.Pro
+00008bf0: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
+00008c00: 7031 0a50 726f 7669 6465 732d 4578 7472  p1.Provides-Extr
+00008c10: 613a 206c 7764 7032 0a50 726f 7669 6465  a: lwdp2.Provide
+00008c20: 732d 4578 7472 613a 206c 7764 7033 0a50  s-Extra: lwdp3.P
+00008c30: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+00008c40: 7764 702d 6465 760a 5072 6f76 6964 6573  wdp-dev.Provides
+00008c50: 2d45 7874 7261 3a20 7574 696c 732d 7270  -Extra: utils-rp
+00008c60: 742d 7669 6577 6572 0a50 726f 7669 6465  t-viewer.Provide
+00008c70: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
+00008c80: 7074 2d76 6965 7765 7235 0a50 726f 7669  pt-viewer5.Provi
+00008c90: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
+00008ca0: 2d61 6476 616e 6365 640a                 -advanced.
```

### Comparing `th2_data_services-2.0.0.dev8344817329/README.md` & `th2_data_services-2.0.0.dev8662586819/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1385,386 +1385,467 @@
 00005680: 7261 7469 6f6e 7320 646f 2074 6865 2069  rations do the i
 00005690: 7465 7261 7469 6f6e 0a62 6568 696e 6420  teration.behind 
 000056a0: 7468 6520 7363 656e 6573 2066 6f72 2079  the scenes for y
 000056b0: 6f75 2e20 4e6f 7465 2c20 6974 2064 6f65  ou. Note, it doe
 000056c0: 736e 2774 206d 6561 6e20 796f 7520 6361  sn't mean you ca
 000056d0: 6e6e 6f74 2069 7465 7261 7465 2074 6865  nnot iterate the
 000056e0: 205f 4461 7461 206f 626a 6563 745f 2e0a   _Data object_..
-000056f0: 0a23 2323 2044 6174 6120 6361 6368 696e  .### Data cachin
-00005700: 670a 0a54 6865 205f 4461 7461 206f 626a  g..The _Data obj
-00005710: 6563 745f 2070 726f 7669 6465 7320 7468  ect_ provides th
-00005720: 6520 6162 696c 6974 7920 746f 2075 7365  e ability to use
-00005730: 2074 6865 2063 6163 6865 2e20 5468 6520   the cache. The 
-00005740: 6361 6368 6520 776f 726b 7320 666f 7220  cache works for 
-00005750: 6561 6368 205f 4461 7461 206f 626a 6563  each _Data objec
-00005760: 745f 2c20 7468 6174 2069 732c 2079 6f75  t_, that is, you
-00005770: 2063 686f 6f73 650a 7768 6963 6820 5f44   choose.which _D
-00005780: 6174 6120 6f62 6a65 6374 5f20 796f 7520  ata object_ you 
-00005790: 7761 6e74 2074 6f20 7361 7665 2e20 5468  want to save. Th
-000057a0: 6520 5f44 6174 6120 6f62 6a65 6374 5f20  e _Data object_ 
-000057b0: 6361 6368 6520 6973 2073 6176 6564 2061  cache is saved a
-000057c0: 6674 6572 2074 6865 2066 6972 7374 2069  fter the first i
-000057d0: 7465 7261 7469 6f6e 2c20 6275 7420 7468  teration, but th
-000057e0: 6520 6974 6572 6174 696f 6e0a 736f 7572  e iteration.sour
-000057f0: 6365 206d 6179 2062 6520 6469 6666 6572  ce may be differ
-00005800: 656e 742e 0a0a 4966 2079 6f75 2064 6f6e  ent...If you don
-00005810: 2774 2075 7365 2074 6865 2063 6163 6865  't use the cache
-00005820: 2c20 796f 7572 2073 6f75 7263 6520 7769  , your source wi
-00005830: 6c6c 2062 6520 7468 6520 6461 7461 2073  ll be the data s
-00005840: 6f75 7263 6520 796f 7520 6861 7665 2069  ource you have i
-00005850: 6e20 7468 6520 5f44 6174 6120 4f62 6a65  n the _Data Obje
-00005860: 6374 5f2e 2042 7574 2069 6620 796f 7520  ct_. But if you 
-00005870: 7573 6520 7468 6520 6361 6368 652c 0a79  use the cache,.y
-00005880: 6f75 7220 736f 7572 6365 2063 616e 2062  our source can b
-00005890: 6520 7468 6520 6461 7461 2073 6f75 7263  e the data sourc
-000058a0: 652c 2074 6865 2070 6172 656e 7420 6361  e, the parent ca
-000058b0: 6368 652c 206f 7220 6f77 6e20 6361 6368  che, or own cach
-000058c0: 653a 0a0a 2a20 5468 6520 6461 7461 2073  e:..* The data s
-000058d0: 6f75 7263 653a 0a20 2049 6620 7468 6520  ource:.  If the 
-000058e0: 5f44 6174 6120 4f62 6a65 6374 5f20 646f  _Data Object_ do
-000058f0: 6573 6e27 7420 6861 7665 2061 2070 6172  esn't have a par
-00005900: 656e 7420 6361 6368 6520 616e 6420 6974  ent cache and it
-00005910: 7320 6361 6368 652e 0a2a 2054 6865 2070  s cache..* The p
-00005920: 6172 656e 7420 6361 6368 653a 0a20 2049  arent cache:.  I
-00005930: 6620 7468 6520 5f44 6174 6120 4f62 6a65  f the _Data Obje
-00005940: 6374 5f20 6861 7320 6120 7061 7265 6e74  ct_ has a parent
-00005950: 2063 6163 6865 2e20 4974 2064 6f65 736e   cache. It doesn
-00005960: 2774 206d 6174 7465 7220 7768 6174 2070  't matter what p
-00005970: 6f73 6974 696f 6e20 7468 6520 7061 7265  osition the pare
-00005980: 6e74 2063 6163 6865 2068 6173 2069 6e20  nt cache has in 
-00005990: 696e 6865 7269 7461 6e63 652e 0a20 205f  inheritance..  _
-000059a0: 4461 7461 204f 626a 6563 745f 2075 6e64  Data Object_ und
-000059b0: 6572 7374 616e 6473 2077 686f 7365 2063  erstands whose c
-000059c0: 6163 6865 2069 7420 6973 2061 6e64 2065  ache it is and e
-000059d0: 7865 6375 7465 7320 7468 6520 7061 7274  xecutes the part
-000059e0: 206f 6620 7468 6520 776f 726b 666c 6f77   of the workflow
-000059f0: 2074 6861 7420 7761 7320 6e6f 7420 6578   that was not ex
-00005a00: 6563 7574 6564 2e0a 2a20 5468 6520 6f77  ecuted..* The ow
-00005a10: 6e20 6361 6368 653a 0a20 2049 6620 6974  n cache:.  If it
-00005a20: 2069 7320 6e6f 7420 7468 6520 6669 7273   is not the firs
-00005a30: 7420 6974 6572 6174 696f 6e20 6f66 2074  t iteration of t
-00005a40: 6869 7320 4461 7461 206f 626a 6563 742e  his Data object.
-00005a50: 0a0a 4e6f 7465 2074 6861 7420 7468 6520  ..Note that the 
-00005a60: 6361 6368 6520 7374 6174 6520 6f66 2074  cache state of t
-00005a70: 6865 2044 6174 6120 6f62 6a65 6374 2069  he Data object i
-00005a80: 7320 6e6f 7420 696e 6865 7269 7465 642e  s not inherited.
-00005a90: 0a0a 2323 2323 2046 6f72 6365 6420 6361  ..#### Forced ca
-00005aa0: 6368 696e 670a 596f 7520 6361 6e20 7465  ching.You can te
-00005ab0: 6c6c 2044 5320 746f 2063 6163 6865 2064  ll DS to cache d
-00005ac0: 6174 6120 746f 2073 7065 6369 6669 6320  ata to specific 
-00005ad0: 6361 6368 6520 6669 6c65 2c20 7768 6963  cache file, whic
-00005ae0: 6820 776f 6e27 7420 6265 2064 656c 6574  h won't be delet
-00005af0: 6564 2061 6674 6572 2073 6372 6970 7420  ed after script 
-00005b00: 656e 642e 0a59 6f75 2063 616e 2073 6565  end..You can see
-00005b10: 2065 7861 6d70 6c65 2069 6e20 312e 3132   example in 1.12
-00005b20: 2073 6563 7469 6f6e 206f 6620 5b67 6574   section of [get
-00005b30: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
-00005b40: 5d28 6578 616d 706c 6573 2f67 6574 5f73  ](examples/get_s
-00005b50: 7461 7274 6564 5f65 7861 6d70 6c65 2e70  tarted_example.p
-00005b60: 7929 2e0a 0a0a 2323 2320 4576 656e 7454  y)....### EventT
-00005b70: 7265 6520 616e 6420 636f 6c6c 6563 7469  ree and collecti
-00005b80: 6f6e 730a 0a23 2323 2320 4576 656e 7454  ons..#### EventT
-00005b90: 7265 650a 0a60 4576 656e 7454 7265 6560  ree..`EventTree`
-00005ba0: 2069 7320 6120 7472 6565 2d62 6173 6564   is a tree-based
-00005bb0: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
-00005bc0: 6f66 2065 7665 6e74 732e 2049 7420 616c  of events. It al
-00005bd0: 6c6f 7773 2079 6f75 2067 6574 2063 6869  lows you get chi
-00005be0: 6c64 7265 6e20 616e 6420 7061 7265 6e74  ldren and parent
-00005bf0: 7320 6f66 2065 7665 6e74 2c0a 6469 7370  s of event,.disp
-00005c00: 6c61 7920 7472 6565 2c20 6765 7420 6675  lay tree, get fu
-00005c10: 6c6c 2070 6174 6820 746f 2065 7665 6e74  ll path to event
-00005c20: 2065 7463 2e0a 0a44 6574 6169 6c73 3a0a   etc...Details:.
-00005c30: 0a2a 2060 4576 656e 7454 7265 6560 2063  .* `EventTree` c
-00005c40: 6f6e 7461 696e 7320 616c 6c20 6576 656e  ontains all even
-00005c50: 7473 2069 6e20 6d65 6d6f 7279 2e0a 2a20  ts in memory..* 
-00005c60: 5472 6565 2068 6173 2073 6f6d 6520 696d  Tree has some im
-00005c70: 706f 7274 616e 7420 7465 726d 733a 0a20  portant terms:. 
-00005c80: 2020 2031 2e20 5f41 6e63 6573 746f 725f     1. _Ancestor_
-00005c90: 2069 7320 616e 7920 7265 6c61 7469 7665   is any relative
-00005ca0: 206f 6620 7468 6520 6576 656e 7420 7570   of the event up
-00005cb0: 2074 6865 2074 7265 6520 2867 7261 6e64   the tree (grand
-00005cc0: 7061 7265 6e74 2c20 7061 7265 6e74 2065  parent, parent e
-00005cd0: 7463 2e29 2e0a 2020 2020 322e 205f 5061  tc.)..    2. _Pa
-00005ce0: 7265 6e74 5f20 6973 206f 6e6c 7920 7468  rent_ is only th
-00005cf0: 6520 6669 7273 7420 7265 6c61 7469 7665  e first relative
-00005d00: 206f 6620 7468 6520 6576 656e 7420 7570   of the event up
-00005d10: 2074 6865 2074 7265 652e 0a20 2020 2033   the tree..    3
-00005d20: 2e20 5f43 6869 6c64 5f20 6973 2074 6865  . _Child_ is the
-00005d30: 2066 6972 7374 2072 656c 6174 6976 6520   first relative 
-00005d40: 6f66 2074 6865 2065 7665 6e74 2064 6f77  of the event dow
-00005d50: 6e20 7468 6520 7472 6565 2e0a 0a54 616b  n the tree...Tak
-00005d60: 6520 6120 6c6f 6f6b 2061 7420 7468 6520  e a look at the 
-00005d70: 666f 6c6c 6f77 696e 6720 4854 4d4c 2074  following HTML t
-00005d80: 7265 6520 746f 2075 6e64 6572 7374 616e  ree to understan
-00005d90: 6420 7468 656d 2e0a 0a20 2020 6060 600a  d them...   ```.
-00005da0: 2020 2020 3c62 6f64 793e 203c 212d 2d20      <body> <!-- 
-00005db0: 616e 6365 7374 6f72 2028 6772 616e 6470  ancestor (grandp
-00005dc0: 6172 656e 7429 2c20 6275 7420 6e6f 7420  arent), but not 
-00005dd0: 7061 7265 6e74 202d 2d3e 0a20 2020 2020  parent -->.     
-00005de0: 2020 203c 6469 763e 203c 212d 2d20 7061     <div> <!-- pa
-00005df0: 7265 6e74 2026 2061 6e63 6573 746f 7220  rent & ancestor 
-00005e00: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
-00005e10: 3c70 3e48 656c 6c6f 2c20 776f 726c 6421  <p>Hello, world!
-00005e20: 3c2f 703e 203c 212d 2d20 6368 696c 6420  </p> <!-- child 
-00005e30: 2d2d 3e0a 2020 2020 2020 2020 2020 2020  -->.            
-00005e40: 3c70 3e47 6f6f 6462 7965 213c 2f70 3e20  <p>Goodbye!</p> 
-00005e50: 3c21 2d2d 2073 6962 6c69 6e67 202d 2d3e  <!-- sibling -->
-00005e60: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-00005e70: 2020 2020 3c2f 626f 6479 3e0a 2020 2060      </body>.   `
-00005e80: 6060 0a0a 2323 2323 2043 6f6c 6c65 6374  ``..#### Collect
-00005e90: 696f 6e73 0a0a 2a2a 4576 656e 7454 7265  ions..**EventTre
-00005ea0: 6543 6f6c 6c65 6374 696f 6e2a 2a20 6973  eCollection** is
-00005eb0: 2061 2063 6f6c 6c65 6374 696f 6e20 6f66   a collection of
-00005ec0: 2045 7665 6e74 5472 6565 732e 2054 6865   EventTrees. The
-00005ed0: 2063 6f6c 6c65 6374 696f 6e20 6275 696c   collection buil
-00005ee0: 6473 2061 2066 6577 205f 4576 656e 7454  ds a few _EventT
-00005ef0: 7265 655f 2062 7920 7061 7373 6564 205f  ree_ by passed _
-00005f00: 4461 7461 0a6f 626a 6563 745f 2e20 416c  Data.object_. Al
-00005f10: 7468 6f75 6768 2079 6f75 2063 616e 2063  though you can c
-00005f20: 6861 6e67 6520 7468 6520 7472 6565 2064  hange the tree d
-00005f30: 6972 6563 746c 792c 2069 7427 7320 6265  irectly, it's be
-00005f40: 7474 6572 2074 6f20 646f 2069 7420 7468  tter to do it th
-00005f50: 726f 7567 6820 636f 6c6c 6563 7469 6f6e  rough collection
-00005f60: 7320 6265 6361 7573 6520 7468 6579 2061  s because they a
-00005f70: 7265 2061 7761 7265 206f 660a 6064 6574  re aware of.`det
-00005f80: 6163 6865 645f 6576 656e 7473 6020 616e  ached_events` an
-00005f90: 6420 6361 6e20 736f 6c76 6520 736f 6d65  d can solve some
-00005fa0: 2065 7665 6e74 7320 6465 7065 6e64 656e   events dependen
-00005fb0: 6369 6573 2e20 5468 6520 636f 6c6c 6563  cies. The collec
-00005fc0: 7469 6f6e 2068 6173 2073 696d 696c 6172  tion has similar
-00005fd0: 2066 6561 7475 7265 7320 6c69 6b65 2061   features like a
-00005fe0: 2073 696e 676c 6520 5f45 7665 6e74 5472   single _EventTr
-00005ff0: 6565 5f0a 6275 7420 6170 706c 7969 6e67  ee_.but applying
-00006000: 2074 6865 6d20 666f 7220 616c 6c20 5f45   them for all _E
-00006010: 7665 6e74 5472 6565 735f 2e0a 0a2a 2a50  ventTrees_...**P
-00006020: 6172 656e 7445 7665 6e74 5472 6565 436f  arentEventTreeCo
-00006030: 6c6c 6563 7469 6f6e 2a2a 2069 7320 6120  llection** is a 
-00006040: 636f 6c6c 6563 7469 6f6e 2073 696d 696c  collection simil
-00006050: 6172 2074 6f20 5f45 7665 6e74 5472 6565  ar to _EventTree
-00006060: 436f 6c6c 6563 7469 6f6e 5f20 6275 7420  Collection_ but 
-00006070: 636f 6e74 6169 6e69 6e67 206f 6e6c 7920  containing only 
-00006080: 7061 7265 6e74 2065 7665 6e74 7320 7468  parent events th
-00006090: 6174 0a61 7265 2072 6566 6572 656e 6365  at.are reference
-000060a0: 6420 696e 2074 6865 2064 6174 6120 7374  d in the data st
-000060b0: 7265 616d 2e20 5468 6520 636f 6c6c 6563  ream. The collec
-000060c0: 7469 6f6e 2068 6173 2066 6561 7475 7265  tion has feature
-000060d0: 7320 7369 6d69 6c61 7220 746f 205f 4576  s similar to _Ev
-000060e0: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
-000060f0: 6e5f 2e0a 0a44 6574 6169 6c73 3a0a 0a2a  n_...Details:..*
-00006100: 2054 6f20 7573 6520 4554 2063 6f6c 6c65   To use ET colle
-00006110: 6374 696f 6e73 2079 6f75 206e 6565 6420  ctions you need 
-00006120: 746f 2069 6e69 7469 616c 697a 6520 7468  to initialize th
-00006130: 656d 2062 7920 5f45 5443 4472 6976 6572  em by _ETCDriver
-00006140: 5f2e 2044 6174 6120 736f 7572 6365 7320  _. Data sources 
-00006150: 7573 7561 6c6c 7920 7072 6f76 6964 6520  usually provide 
-00006160: 7468 656d 2e0a 2020 596f 7520 6361 6e20  them..  You can 
-00006170: 6372 6561 7465 2069 7420 6279 2079 6f75  create it by you
-00006180: 7273 656c 6620 6465 7065 6e64 696e 6720  rself depending 
-00006190: 6f6e 2079 6f75 7220 6461 7461 2073 7472  on your data str
-000061a0: 7563 7475 7265 2e0a 2a20 5468 6520 636f  ucture..* The co
-000061b0: 6c6c 6563 7469 6f6e 2068 6173 2061 2066  llection has a f
-000061c0: 6561 7475 7265 2074 6f20 7265 636f 7665  eature to recove
-000061d0: 7220 6576 656e 7473 2e20 416c 6c20 6576  r events. All ev
-000061e0: 656e 7473 2074 6861 7420 6172 6520 6e6f  ents that are no
-000061f0: 7420 696e 2074 6865 2072 6563 6569 7665  t in the receive
-00006200: 6420 6461 7461 2073 7472 6561 6d2c 2062  d data stream, b
-00006210: 7574 2077 6869 6368 2061 7265 0a20 2072  ut which are.  r
-00006220: 6566 6572 656e 6365 6420 7769 6c6c 2062  eferenced will b
-00006230: 6520 6c6f 6164 6564 2066 726f 6d20 7468  e loaded from th
-00006240: 6520 6461 7461 2073 6f75 7263 652e 0a2a  e data source..*
-00006250: 2059 6f75 2063 616e 2074 616b 6520 6064   You can take `d
-00006260: 6574 6163 6865 645f 6576 656e 7473 6020  etached_events` 
-00006270: 746f 2073 6565 2077 6869 6368 2065 7665  to see which eve
-00006280: 6e74 7320 6172 6520 6d69 7373 696e 672e  nts are missing.
-00006290: 0a2a 2049 6620 796f 7520 7761 6e74 2c20  .* If you want, 
-000062a0: 796f 7520 6361 6e20 6275 696c 6420 7061  you can build pa
-000062b0: 7265 6e74 6c65 7373 2074 7265 6573 2077  rentless trees w
-000062c0: 6865 7265 2074 6865 206d 6973 7369 6e67  here the missing
-000062d0: 2065 7665 6e74 7320 6172 6520 7374 7562   events are stub
-000062e0: 6265 6420 696e 7374 6561 642e 204a 7573  bed instead. Jus
-000062f0: 740a 2020 7573 6520 6067 6574 5f70 6172  t.  use `get_par
-00006300: 656e 746c 6573 735f 7472 6565 7328 2960  entless_trees()`
-00006310: 2e0a 0a52 6571 7569 7265 6d65 6e74 733a  ...Requirements:
-00006320: 0a0a 312e 2045 7665 6e74 7320 7072 6f76  ..1. Events prov
-00006330: 6964 6564 2074 6f20 4554 4320 6861 7665  ided to ETC have
-00006340: 2074 6f20 6861 7665 2060 6576 656e 745f   to have `event_
-00006350: 6e61 6d65 602c 2060 6576 656e 745f 6964  name`, `event_id
-00006360: 602c 2060 7061 7265 6e74 5f65 7665 6e74  `, `parent_event
-00006370: 5f69 6460 2066 6965 6c64 732e 2054 6865  _id` fields. The
-00006380: 790a 6361 6e20 6861 7665 2061 6e6f 7468  y.can have anoth
-00006390: 6572 206e 616d 6573 2028 6974 2072 6573  er names (it res
-000063a0: 6f6c 7665 7320 696e 2074 6865 2064 7269  olves in the dri
-000063b0: 7665 7229 2e0a 0a23 2323 2320 4869 6e74  ver)...#### Hint
-000063c0: 730a 0a2a 2052 656d 6f76 6520 616c 6c20  s..* Remove all 
-000063d0: 756e 6e65 6365 7373 6172 7920 6669 656c  unnecessary fiel
-000063e0: 6473 2066 726f 6d20 6576 656e 7473 2062  ds from events b
-000063f0: 6566 6f72 6520 7061 7373 696e 6720 746f  efore passing to
-00006400: 2061 205f 636f 6c6c 6563 7469 6f6e 5f20   a _collection_ 
-00006410: 746f 2072 6564 7563 6520 6d65 6d6f 7279  to reduce memory
-00006420: 2075 7361 6765 2e0a 2a20 5573 6520 6073   usage..* Use `s
-00006430: 686f 7728 2960 206d 6574 686f 6420 746f  how()` method to
-00006440: 2070 7269 6e74 2074 6865 2074 7265 6520   print the tree 
-00006450: 696e 2074 7265 652d 6c69 6b65 2076 6965  in tree-like vie
-00006460: 772e 0a2a 204e 6f74 6520 7468 6174 2074  w..* Note that t
-00006470: 6865 2060 6765 745f 7860 206d 6574 686f  he `get_x` metho
-00006480: 6473 2077 696c 6c20 7261 6973 6520 616e  ds will raise an
-00006490: 2065 7863 6570 7469 6f6e 2069 6620 796f   exception if yo
-000064a0: 7520 7061 7373 2061 6e20 756e 6b6e 6f77  u pass an unknow
-000064b0: 6e20 6576 656e 7420 6964 2c20 756e 6c69  n event id, unli
-000064c0: 6b65 2074 6865 2060 6669 6e64 5f78 6020  ke the `find_x` 
-000064d0: 6d65 7468 6f64 7320 280a 2020 7468 6579  methods (.  they
-000064e0: 2072 6574 7572 6e20 4e6f 6e65 292e 0a2a   return None)..*
-000064f0: 2049 6620 796f 7520 7761 6e74 2074 6f20   If you want to 
-00006500: 6b6e 6f77 2074 6861 7420 7370 6563 6966  know that specif
-00006510: 6965 6420 6576 656e 7420 6578 6973 7473  ied event exists
-00006520: 2c20 7573 6520 7468 6520 7079 7468 6f6e  , use the python
-00006530: 2060 696e 6020 6b65 7977 6f72 6420 2865   `in` keyword (e
-00006540: 2e67 2e20 6027 6576 656e 742d 6964 2720  .g. `'event-id' 
-00006550: 696e 2065 7665 6e74 735f 7472 6565 6029  in events_tree`)
-00006560: 2e0a 2a20 5573 6520 7468 6520 7079 7468  ..* Use the pyth
-00006570: 6f6e 2060 6c65 6e60 206b 6579 776f 7264  on `len` keyword
-00006580: 2074 6f20 6765 7420 6576 656e 7473 206e   to get events n
-00006590: 756d 6265 7220 696e 2074 6865 2074 7265  umber in the tre
-000065a0: 652e 0a0a 2323 2320 4669 656c 6420 5265  e...### Field Re
-000065b0: 736f 6c76 6572 730a 496e 7465 7266 6163  solvers.Interfac
-000065c0: 6520 6361 6e20 6265 2066 6f75 6e64 2069  e can be found i
-000065d0: 6e20 6074 6832 5f64 6174 615f 7365 7276  n `th2_data_serv
-000065e0: 6963 6573 2f69 6e74 6572 6661 6365 732f  ices/interfaces/
-000065f0: 7574 696c 732f 7265 736f 6c76 6572 2e70  utils/resolver.p
-00006600: 7960 2e20 200a 416c 6c20 6461 7461 2d73  y`.  .All data-s
-00006610: 6f75 7263 6573 2073 686f 756c 6420 696d  ources should im
-00006620: 706c 656d 656e 7420 7468 656d 2e0a 0a54  plement them...T
-00006630: 6865 2069 6465 6120 6f66 2075 7369 6e67  he idea of using
-00006640: 2072 6573 6f6c 7665 7273 3a0a 4974 2073   resolvers:.It s
-00006650: 6f6c 7665 7320 7468 6520 7072 6f62 6c65  olves the proble
-00006660: 6d20 6f66 2068 6176 696e 6720 6120 6665  m of having a fe
-00006670: 7720 4461 7461 536f 7572 6365 7320 7769  w DataSources wi
-00006680: 7468 2073 696d 696c 6172 2064 6174 612c  th similar data,
-00006690: 0a62 7574 2077 6974 6820 6469 6666 6572  .but with differ
-000066a0: 656e 7420 7761 7973 2074 6f20 6765 7420  ent ways to get 
-000066b0: 6974 2e0a 0a54 6865 7365 2063 6c61 7373  it...These class
-000066c0: 6573 2070 726f 7669 6465 2079 6f75 2067  es provide you g
-000066d0: 6574 7465 7220 6d65 7468 6f64 732e 0a55  etter methods..U
-000066e0: 7369 6e67 2074 6865 7365 2063 6c61 7373  sing these class
-000066f0: 6573 2061 6c6c 6f77 7320 796f 7520 746f  es allows you to
-00006700: 2066 7265 656c 7920 7377 6974 6368 2062   freely switch b
-00006710: 6574 7765 656e 2064 6966 6665 7265 6e74  etween different
-00006720: 2064 6174 610a 666f 726d 6174 7320 616e   data.formats an
-00006730: 6420 646f 6e27 7420 6368 616e 6765 2079  d don't change y
-00006740: 6f75 7220 636f 6465 2e0a 0a52 6573 6f6c  our code...Resol
-00006750: 7665 7273 2073 6f6c 7665 2074 6865 2070  vers solve the p
-00006760: 726f 626c 656d 206f 6620 6461 7461 2d66  roblem of data-f
-00006770: 6f72 6d61 7420 6d69 6772 6174 696f 6e2e  ormat migration.
-00006780: 0a2d 2066 6965 6c64 7320 706c 6163 6520  .- fields place 
-00006790: 6361 6e20 6265 2063 6861 6e67 6564 0a2d  can be changed.-
-000067a0: 2066 6965 6c64 7320 6e61 6d65 7320 6361   fields names ca
-000067b0: 6e20 6265 2063 6861 6e67 6564 0a0a 5265  n be changed..Re
-000067c0: 736f 6c76 6572 7320 6361 6e20 776f 726b  solvers can work
-000067d0: 206f 6e6c 7920 7769 7468 206f 6e65 2065   only with one e
-000067e0: 7665 6e74 2f6d 6573 7361 6765 2e0a 4974  vent/message..It
-000067f0: 206d 6561 6e73 2c20 6966 2079 6f75 7220   means, if your 
-00006800: 6d65 7373 6167 6520 6861 7320 7375 622d  message has sub-
-00006810: 6d65 7373 6167 6573 2028 6c69 6b65 2074  messages (like t
-00006820: 6832 2d6d 6573 7361 6765 7320 696e 206c  h2-messages in l
-00006830: 7764 7029 2069 7420 0a77 6f6e 2774 2077  wdp) it .won't w
-00006840: 6f72 6b2c 2062 6563 6175 7365 2072 6573  ork, because res
-00006850: 6f6c 7665 7220 7769 6c6c 206e 6f74 206b  olver will not k
-00006860: 6e6f 7720 7769 7468 2077 6869 6368 2073  now with which s
-00006870: 7562 2d6d 6573 7361 6765 2073 686f 756c  ub-message shoul
-00006880: 6420 6974 2077 6f72 6b2e 200a 0a2a 2a57  d it work. ..**W
-00006890: 6f72 6b61 726f 756e 642a 2a20 200a 312e  orkaround**  .1.
-000068a0: 2045 7870 616e 6420 616c 6c20 796f 7572   Expand all your
-000068b0: 206d 6573 7361 6765 7320 2d3e 2060 6e65   messages -> `ne
-000068c0: 775f 6420 3d20 796f 7572 5f64 6174 612e  w_d = your_data.
-000068d0: 6d61 7028 4d65 7373 6167 6546 6965 6c64  map(MessageField
-000068e0: 5265 736f 6c76 6572 2e65 7870 616e 645f  Resolver.expand_
-000068f0: 6d65 7373 6167 6529 600a 322e 2055 7365  message)`.2. Use
-00006900: 2060 4578 7061 6e64 6564 4d65 7373 6167   `ExpandedMessag
-00006910: 6546 6965 6c64 5265 736f 6c76 6572 6020  eFieldResolver` 
-00006920: 696e 7374 6561 6420 6f66 2075 7375 616c  instead of usual
-00006930: 2060 4d65 7373 6167 6546 6965 6c64 5265   `MessageFieldRe
-00006940: 736f 6c76 6572 6020 7768 656e 200a 2020  solver` when .  
-00006950: 2020 796f 7520 7461 6b65 2066 6965 6c64    you take field
-00006960: 7320 666f 7220 6578 7061 6e64 6564 206d  s for expanded m
-00006970: 6573 7361 6765 732e 0a0a 2a2a 496d 706c  essages...**Impl
-00006980: 656d 656e 7461 7469 6f6e 2061 6476 6963  ementation advic
-00006990: 653a 2a2a 0a31 2e20 7261 6973 6520 4e6f  e:**.1. raise No
-000069a0: 7449 6d70 6c65 6d65 6e74 6564 4572 726f  tImplementedErro
-000069b0: 7220 2d2d 2069 6620 796f 7572 2049 6d70  r -- if your Imp
-000069c0: 6c65 6d65 6e74 6174 696f 6e20 646f 6573  lementation does
-000069d0: 6e27 7420 7375 7070 6f72 7420 7468 6973  n't support this
-000069e0: 2067 6574 7465 722e 0a0a 2a2a 5065 7266   getter...**Perf
-000069f0: 6f72 6d61 6e63 6520 696d 7061 6374 3a2a  ormance impact:*
-00006a00: 2a0a 2d20 4974 2061 2062 6974 2073 6c6f  *.- It a bit slo
-00006a10: 7765 7220 7468 616e 2075 7369 6e67 206e  wer than using n
-00006a20: 616b 6564 2066 6965 6c64 2061 6363 6573  aked field acces
-00006a30: 7320 6064 6963 745b 276b 6579 275d 602e  s `dict['key']`.
-00006a40: 0a0a 2323 2032 2e34 2e20 4c69 6e6b 730a  ..## 2.4. Links.
-00006a50: 0a2d 205b 5265 706f 7274 2044 6174 6120  .- [Report Data 
-00006a60: 5072 6f76 6964 6572 5d28 6874 7470 733a  Provider](https:
-00006a70: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
-00006a80: 2d6e 6574 2f74 6832 2d72 7074 2d64 6174  -net/th2-rpt-dat
-00006a90: 612d 7072 6f76 6964 6572 290a 2d20 5b54  a-provider).- [T
-00006aa0: 6832 2044 6174 6120 5365 7276 6963 6573  h2 Data Services
-00006ab0: 2055 7469 6c73 5d28 6874 7470 733a 2f2f   Utils](https://
-00006ac0: 6769 7468 7562 2e63 6f6d 2f74 6832 2d6e  github.com/th2-n
-00006ad0: 6574 2f74 6832 2d64 6174 612d 7365 7276  et/th2-data-serv
-00006ae0: 6963 6573 2d75 7469 6c73 290a 0a23 2033  ices-utils)..# 3
-00006af0: 2e20 4265 7374 2070 7261 6374 6963 6573  . Best practices
-00006b00: 0a44 6570 656e 6469 6e67 206f 6e20 686f  .Depending on ho
-00006b10: 7720 796f 7520 776f 726b 2077 6974 6820  w you work with 
-00006b20: 6044 6174 6120 6f62 6a65 6374 602c 2069  `Data object`, i
-00006b30: 7420 6361 6e20 6265 2073 6c6f 7720 6f66  t can be slow of
-00006b40: 2066 6173 742e 0a41 7320 7769 7468 2061   fast..As with a
-00006b50: 2072 656c 6174 696f 6e61 6c20 6461 7461   relational data
-00006b60: 6261 7365 2c20 796f 7520 6361 6e20 7772  base, you can wr
-00006b70: 6974 6520 6120 7175 6572 7920 7468 6174  ite a query that
-00006b80: 2077 696c 6c20 7265 7475 726e 2064 6174   will return dat
-00006b90: 6120 736c 6f77 6c79 206f 7220 7175 6963  a slowly or quic
-00006ba0: 6b6c 792c 0a74 6865 2073 616d 6520 7768  kly,.the same wh
-00006bb0: 656e 2077 6f72 6b69 6e67 2077 6974 6820  en working with 
-00006bc0: 6120 6044 6174 6120 6f62 6a65 6374 602e  a `Data object`.
-00006bd0: 0a0a 466f 6c6c 6f77 2074 6865 2072 756c  ..Follow the rul
-00006be0: 6573 2074 6f20 6d61 6b65 2079 6f75 7220  es to make your 
-00006bf0: 776f 726b 2077 6974 6820 4461 7461 206f  work with Data o
-00006c00: 626a 6563 7420 6661 7374 3a0a 312e 2055  bject fast:.1. U
-00006c10: 7365 2060 4461 7461 2e75 7365 5f63 6163  se `Data.use_cac
-00006c20: 6865 2829 6020 6966 2079 6f75 2069 7465  he()` if you ite
-00006c30: 7261 7465 2064 6174 6120 6d6f 7265 2074  rate data more t
-00006c40: 6861 6e20 6f6e 6520 7469 6d65 2e0a 322e  han one time..2.
-00006c50: 2054 7279 2074 6f20 646f 6e27 7420 6974   Try to don't it
-00006c60: 6572 6174 6520 6f6e 6520 6044 6174 6120  erate one `Data 
-00006c70: 6f62 6a65 6374 6020 696e 7369 6465 2074  object` inside t
-00006c80: 6865 206f 7468 6572 206f 6e65 2e0a 2020  he other one..  
-00006c90: 2049 6620 796f 7520 7368 6f75 6c64 2074   If you should t
-00006ca0: 6f20 646f 2069 742c 2075 7365 2073 686f  o do it, use sho
-00006cb0: 7274 2060 4461 7461 206f 626a 6563 7460  rt `Data object`
-00006cc0: 2066 6972 7374 2061 6e64 206c 6f6e 6720   first and long 
-00006cd0: 6044 6174 6120 6f62 6a65 6374 6020 696e  `Data object` in
-00006ce0: 7369 6465 2074 6865 206c 6f6f 702e 0a20  side the loop.. 
-00006cf0: 2020 4974 276c 6c20 616c 6c6f 7720 796f    It'll allow yo
-00006d00: 7520 6f70 656e 2074 6865 2063 6163 6865  u open the cache
-00006d10: 2066 696c 6520 6f72 2063 7265 6174 6520   file or create 
-00006d20: 6120 7265 7175 6573 7420 746f 2060 4461  a request to `Da
-00006d30: 7461 2073 6f75 7263 6560 206c 6573 7320  ta source` less 
-00006d40: 6e75 6d62 6572 206f 6620 7469 6d65 732e  number of times.
-00006d50: 0a0a 2320 342e 204f 6666 6963 6961 6c20  ..# 4. Official 
-00006d60: 4461 7461 536f 7572 6365 2069 6d70 6c65  DataSource imple
-00006d70: 6d65 6e74 6174 696f 6e73 0a0a 2d20 5b4c  mentations..- [L
-00006d80: 6967 6874 7765 6967 6874 2044 6174 6120  ightweight Data 
-00006d90: 5072 6f76 6964 6572 2044 6174 6120 536f  Provider Data So
-00006da0: 7572 6365 5d28 6874 7470 733a 2f2f 6769  urce](https://gi
-00006db0: 7468 7562 2e63 6f6d 2f74 6832 2d6e 6574  thub.com/th2-net
-00006dc0: 2f74 6832 2d64 732d 736f 7572 6365 2d6c  /th2-ds-source-l
-00006dd0: 7764 7029 0a0a 0a23 2035 2e20 4150 490a  wdp)...# 5. API.
-00006de0: 0a49 6620 796f 7520 6172 6520 6c6f 6f6b  .If you are look
-00006df0: 696e 6720 666f 7220 636c 6173 7365 7320  ing for classes 
-00006e00: 6465 7363 7269 7074 696f 6e20 7365 6520  description see 
-00006e10: 7468 6520 5b41 5049 2044 6f63 756d 656e  the [API Documen
-00006e20: 7461 7469 6f6e 5d28 646f 6375 6d65 6e74  tation](document
-00006e30: 6174 696f 6e2f 6170 692f 696e 6465 782e  ation/api/index.
-00006e40: 6d64 292e 0a0a 2320 362e 2045 7861 6d70  md)...# 6. Examp
-00006e50: 6c65 730a 0a2d 205b 6765 745f 7374 6172  les..- [get_star
-00006e60: 7465 645f 6578 616d 706c 652e 7079 5d28  ted_example.py](
-00006e70: 6578 616d 706c 6573 2f67 6574 5f73 7461  examples/get_sta
-00006e80: 7274 6564 5f65 7861 6d70 6c65 2e70 7929  rted_example.py)
-00006e90: 0a                                       .
+000056f0: 0a0a 2323 2320 4461 7461 2069 7465 7261  ..### Data itera
+00005700: 7469 6f6e 0a0a 5468 6520 4461 7461 206f  tion..The Data o
+00005710: 626a 6563 7420 636f 6e73 7472 7563 746f  bject constructo
+00005720: 7220 6d65 7468 6f64 2074 616b 6573 2069  r method takes i
+00005730: 6e20 6173 2061 7267 756d 656e 7420 6569  n as argument ei
+00005740: 7468 6572 2061 6e20 6974 6572 6174 6f72  ther an iterator
+00005750: 206f 7665 7220 6f62 6a65 6374 7320 6f72   over objects or
+00005760: 2061 2067 656e 6572 6174 6f72 2066 756e   a generator fun
+00005770: 6374 696f 6e2e 0a54 6865 2044 6174 6120  ction..The Data 
+00005780: 6f62 6a65 6374 2069 7465 7261 746f 7220  object iterator 
+00005790: 6861 6e64 6c65 7320 6561 6368 2069 7465  handles each ite
+000057a0: 6d20 696e 2074 6869 7320 6974 6572 6174  m in this iterat
+000057b0: 6f72 206f 7220 6765 6e65 7261 746f 7220  or or generator 
+000057c0: 6173 2074 6865 7920 6172 652c 206d 6561  as they are, mea
+000057d0: 6e69 6e67 2069 7420 646f 6573 6e27 7420  ning it doesn't 
+000057e0: 7472 7920 746f 2072 6561 6420 7468 6520  try to read the 
+000057f0: 636f 6e74 656e 7420 6f66 2069 7465 6d20  content of item 
+00005800: 6f72 2072 6574 7572 6e20 7468 656d 206d  or return them m
+00005810: 6f64 6966 6965 6420 696e 2061 6e79 2077  odified in any w
+00005820: 6179 2c20 696e 7374 6561 6420 7265 7475  ay, instead retu
+00005830: 726e 7320 7468 6520 6974 656d 2069 7473  rns the item its
+00005840: 656c 662e 0a54 6865 206f 6e6c 7920 6578  elf..The only ex
+00005850: 6365 7074 696f 6e20 746f 2074 6869 7320  ception to this 
+00005860: 6973 2077 6865 6e20 4461 7461 206f 626a  is when Data obj
+00005870: 6563 7420 6973 2062 7569 6c74 2075 7369  ect is built usi
+00005880: 6e67 2069 7465 7261 746f 7220 6f72 2067  ng iterator or g
+00005890: 656e 6572 6174 6f72 206f 7665 7220 6f74  enerator over ot
+000058a0: 6865 7220 4461 7461 206f 626a 6563 7473  her Data objects
+000058b0: 2e20 4e6f 7465 2074 6861 7420 7468 6973  . Note that this
+000058c0: 2069 7465 7261 746f 7220 6f72 2067 656e   iterator or gen
+000058d0: 6572 6174 6f72 206d 7573 7420 6f6e 6c79  erator must only
+000058e0: 2062 6520 7969 656c 6469 6e67 2044 6174   be yielding Dat
+000058f0: 6120 6f62 6a65 6374 7320 616e 6420 6e6f  a objects and no
+00005900: 7468 696e 6720 656c 7365 2e20 4966 2077  thing else. If w
+00005910: 6520 6275 696c 6420 6672 6f6d 2061 206d  e build from a m
+00005920: 6978 206f 6620 4461 7461 206f 626a 6563  ix of Data objec
+00005930: 7473 2061 6e64 2073 6f6d 6520 6f74 6865  ts and some othe
+00005940: 7220 7479 7065 732c 2044 6174 6120 6f62  r types, Data ob
+00005950: 6a65 6374 7327 2063 6f6e 7465 6e74 2077  jects' content w
+00005960: 6f6e 2774 2062 6520 7265 6164 2061 6e64  on't be read and
+00005970: 2069 6e73 7465 6164 2069 7420 7769 6c6c   instead it will
+00005980: 2062 6520 7265 7475 726e 6564 2061 7320   be returned as 
+00005990: 4461 7461 206f 626a 6563 7420 6974 7365  Data object itse
+000059a0: 6c66 2e0a 0a53 6d61 6c6c 2065 7861 6d70  lf...Small examp
+000059b0: 6c65 2074 6f20 6465 6d6f 6e73 7472 6174  le to demonstrat
+000059c0: 653a 0a0a 6060 6070 7974 686f 6e0a 6672  e:..```python.fr
+000059d0: 6f6d 2074 6832 5f64 6174 615f 7365 7276  om th2_data_serv
+000059e0: 6963 6573 2e64 6174 6120 696d 706f 7274  ices.data import
+000059f0: 2044 6174 610a 0a64 3120 3d20 4461 7461   Data..d1 = Data
+00005a00: 285b 312c 322c 335d 290a 6432 203d 2044  ([1,2,3]).d2 = D
+00005a10: 6174 6128 5b34 2c35 2c36 5d29 0a0a 6f6e  ata([4,5,6])..on
+00005a20: 6c79 5f64 6174 615f 6f62 6a65 6374 7320  ly_data_objects 
+00005a30: 3d20 4461 7461 285b 6431 2c64 325d 2920  = Data([d1,d2]) 
+00005a40: 2320 5769 6c6c 2069 7465 7261 7465 2061  # Will iterate a
+00005a50: 7320 312c 322c 332c 342c 352c 360a 6461  s 1,2,3,4,5,6.da
+00005a60: 7461 5f61 6e64 5f6c 6973 7420 3d20 4461  ta_and_list = Da
+00005a70: 7461 285b 6431 2c5b 342c 352c 365d 5d29  ta([d1,[4,5,6]])
+00005a80: 2023 2057 696c 6c20 6974 6572 6174 6520   # Will iterate 
+00005a90: 6173 2064 312c 205b 342c 352c 365d 0a64  as d1, [4,5,6].d
+00005aa0: 6174 615f 616e 645f 6e75 6d62 6572 7320  ata_and_numbers 
+00005ab0: 3d20 4461 7461 285b 6431 2c34 2c35 2c36  = Data([d1,4,5,6
+00005ac0: 5d29 2023 2057 696c 6c20 6974 6572 6174  ]) # Will iterat
+00005ad0: 6520 6173 2064 312c 342c 352c 360a 6c69  e as d1,4,5,6.li
+00005ae0: 7374 735f 6f6e 6c79 203d 2044 6174 6128  sts_only = Data(
+00005af0: 5b31 2c32 2c33 5d2c 5b34 2c35 2c36 5d29  [1,2,3],[4,5,6])
+00005b00: 2023 2057 696c 6c20 6974 6572 6174 6520   # Will iterate 
+00005b10: 6173 205b 312c 322c 335d 2c5b 342c 352c  as [1,2,3],[4,5,
+00005b20: 365d 0a0a 2320 4966 2077 6520 7761 6e74  6]..# If we want
+00005b30: 2074 6f20 6974 6572 6174 6520 6f76 6572   to iterate over
+00005b40: 2063 6f6e 7465 6e74 206f 6620 6c69 7374   content of list
+00005b50: 206f 6620 6c69 7374 732c 2077 6520 7368   of lists, we sh
+00005b60: 6f75 6c64 2066 6972 7374 2063 7265 6174  ould first creat
+00005b70: 6520 4461 7461 206f 626a 6563 7473 2066  e Data objects f
+00005b80: 726f 6d20 7468 656d 2c0a 2320 7468 656e  rom them,.# then
+00005b90: 2075 7365 2074 6865 6d20 746f 2063 6f6e   use them to con
+00005ba0: 7374 7275 6374 206e 6577 2044 6174 6120  struct new Data 
+00005bb0: 6f62 6a65 6374 2061 7320 696e 2063 6173  object as in cas
+00005bc0: 6520 6f66 2064 3120 616e 6420 6432 2c20  e of d1 and d2, 
+00005bd0: 6372 6561 7469 6e67 2027 6f6e 6c79 5f64  creating 'only_d
+00005be0: 6174 615f 6f62 6a65 6374 7327 2069 6e20  ata_objects' in 
+00005bf0: 7468 6973 2065 7861 6d70 6c65 2e0a 6060  this example..``
+00005c00: 600a 200a 0a23 2323 2044 6174 6120 6361  `. ..### Data ca
+00005c10: 6368 696e 670a 0a54 6865 205f 4461 7461  ching..The _Data
+00005c20: 206f 626a 6563 745f 2070 726f 7669 6465   object_ provide
+00005c30: 7320 7468 6520 6162 696c 6974 7920 746f  s the ability to
+00005c40: 2075 7365 2074 6865 2063 6163 6865 2e20   use the cache. 
+00005c50: 5468 6520 6361 6368 6520 776f 726b 7320  The cache works 
+00005c60: 666f 7220 6561 6368 205f 4461 7461 206f  for each _Data o
+00005c70: 626a 6563 745f 2c20 7468 6174 2069 732c  bject_, that is,
+00005c80: 2079 6f75 2063 686f 6f73 650a 7768 6963   you choose.whic
+00005c90: 6820 5f44 6174 6120 6f62 6a65 6374 5f20  h _Data object_ 
+00005ca0: 796f 7520 7761 6e74 2074 6f20 7361 7665  you want to save
+00005cb0: 2e20 5468 6520 5f44 6174 6120 6f62 6a65  . The _Data obje
+00005cc0: 6374 5f20 6361 6368 6520 6973 2073 6176  ct_ cache is sav
+00005cd0: 6564 2061 6674 6572 2074 6865 2066 6972  ed after the fir
+00005ce0: 7374 2069 7465 7261 7469 6f6e 2c20 6275  st iteration, bu
+00005cf0: 7420 7468 6520 6974 6572 6174 696f 6e0a  t the iteration.
+00005d00: 736f 7572 6365 206d 6179 2062 6520 6469  source may be di
+00005d10: 6666 6572 656e 742e 0a0a 4966 2079 6f75  fferent...If you
+00005d20: 2064 6f6e 2774 2075 7365 2074 6865 2063   don't use the c
+00005d30: 6163 6865 2c20 796f 7572 2073 6f75 7263  ache, your sourc
+00005d40: 6520 7769 6c6c 2062 6520 7468 6520 6461  e will be the da
+00005d50: 7461 2073 6f75 7263 6520 796f 7520 6861  ta source you ha
+00005d60: 7665 2069 6e20 7468 6520 5f44 6174 6120  ve in the _Data 
+00005d70: 4f62 6a65 6374 5f2e 2042 7574 2069 6620  Object_. But if 
+00005d80: 796f 7520 7573 6520 7468 6520 6361 6368  you use the cach
+00005d90: 652c 0a79 6f75 7220 736f 7572 6365 2063  e,.your source c
+00005da0: 616e 2062 6520 7468 6520 6461 7461 2073  an be the data s
+00005db0: 6f75 7263 652c 2074 6865 2070 6172 656e  ource, the paren
+00005dc0: 7420 6361 6368 652c 206f 7220 6f77 6e20  t cache, or own 
+00005dd0: 6361 6368 653a 0a0a 2a20 5468 6520 6461  cache:..* The da
+00005de0: 7461 2073 6f75 7263 653a 0a20 2049 6620  ta source:.  If 
+00005df0: 7468 6520 5f44 6174 6120 4f62 6a65 6374  the _Data Object
+00005e00: 5f20 646f 6573 6e27 7420 6861 7665 2061  _ doesn't have a
+00005e10: 2070 6172 656e 7420 6361 6368 6520 616e   parent cache an
+00005e20: 6420 6974 7320 6361 6368 652e 0a2a 2054  d its cache..* T
+00005e30: 6865 2070 6172 656e 7420 6361 6368 653a  he parent cache:
+00005e40: 0a20 2049 6620 7468 6520 5f44 6174 6120  .  If the _Data 
+00005e50: 4f62 6a65 6374 5f20 6861 7320 6120 7061  Object_ has a pa
+00005e60: 7265 6e74 2063 6163 6865 2e20 4974 2064  rent cache. It d
+00005e70: 6f65 736e 2774 206d 6174 7465 7220 7768  oesn't matter wh
+00005e80: 6174 2070 6f73 6974 696f 6e20 7468 6520  at position the 
+00005e90: 7061 7265 6e74 2063 6163 6865 2068 6173  parent cache has
+00005ea0: 2069 6e20 696e 6865 7269 7461 6e63 652e   in inheritance.
+00005eb0: 0a20 205f 4461 7461 204f 626a 6563 745f  .  _Data Object_
+00005ec0: 2075 6e64 6572 7374 616e 6473 2077 686f   understands who
+00005ed0: 7365 2063 6163 6865 2069 7420 6973 2061  se cache it is a
+00005ee0: 6e64 2065 7865 6375 7465 7320 7468 6520  nd executes the 
+00005ef0: 7061 7274 206f 6620 7468 6520 776f 726b  part of the work
+00005f00: 666c 6f77 2074 6861 7420 7761 7320 6e6f  flow that was no
+00005f10: 7420 6578 6563 7574 6564 2e0a 2a20 5468  t executed..* Th
+00005f20: 6520 6f77 6e20 6361 6368 653a 0a20 2049  e own cache:.  I
+00005f30: 6620 6974 2069 7320 6e6f 7420 7468 6520  f it is not the 
+00005f40: 6669 7273 7420 6974 6572 6174 696f 6e20  first iteration 
+00005f50: 6f66 2074 6869 7320 4461 7461 206f 626a  of this Data obj
+00005f60: 6563 742e 0a0a 4e6f 7465 2074 6861 7420  ect...Note that 
+00005f70: 7468 6520 6361 6368 6520 7374 6174 6520  the cache state 
+00005f80: 6f66 2074 6865 2044 6174 6120 6f62 6a65  of the Data obje
+00005f90: 6374 2069 7320 6e6f 7420 696e 6865 7269  ct is not inheri
+00005fa0: 7465 642e 0a0a 2323 2323 2046 6f72 6365  ted...#### Force
+00005fb0: 6420 6361 6368 696e 670a 596f 7520 6361  d caching.You ca
+00005fc0: 6e20 7465 6c6c 2044 5320 746f 2063 6163  n tell DS to cac
+00005fd0: 6865 2064 6174 6120 746f 2073 7065 6369  he data to speci
+00005fe0: 6669 6320 6361 6368 6520 6669 6c65 2c20  fic cache file, 
+00005ff0: 7768 6963 6820 776f 6e27 7420 6265 2064  which won't be d
+00006000: 656c 6574 6564 2061 6674 6572 2073 6372  eleted after scr
+00006010: 6970 7420 656e 642e 0a59 6f75 2063 616e  ipt end..You can
+00006020: 2073 6565 2065 7861 6d70 6c65 2069 6e20   see example in 
+00006030: 312e 3132 2073 6563 7469 6f6e 206f 6620  1.12 section of 
+00006040: 5b67 6574 5f73 7461 7274 6564 5f65 7861  [get_started_exa
+00006050: 6d70 6c65 5d28 6578 616d 706c 6573 2f67  mple](examples/g
+00006060: 6574 5f73 7461 7274 6564 5f65 7861 6d70  et_started_examp
+00006070: 6c65 2e70 7929 2e0a 0a0a 2323 2320 4576  le.py)....### Ev
+00006080: 656e 7454 7265 6520 616e 6420 636f 6c6c  entTree and coll
+00006090: 6563 7469 6f6e 730a 0a23 2323 2320 4576  ections..#### Ev
+000060a0: 656e 7454 7265 650a 0a60 4576 656e 7454  entTree..`EventT
+000060b0: 7265 6560 2069 7320 6120 7472 6565 2d62  ree` is a tree-b
+000060c0: 6173 6564 2064 6174 6120 7374 7275 6374  ased data struct
+000060d0: 7572 6520 6f66 2065 7665 6e74 732e 2049  ure of events. I
+000060e0: 7420 616c 6c6f 7773 2079 6f75 2067 6574  t allows you get
+000060f0: 2063 6869 6c64 7265 6e20 616e 6420 7061   children and pa
+00006100: 7265 6e74 7320 6f66 2065 7665 6e74 2c0a  rents of event,.
+00006110: 6469 7370 6c61 7920 7472 6565 2c20 6765  display tree, ge
+00006120: 7420 6675 6c6c 2070 6174 6820 746f 2065  t full path to e
+00006130: 7665 6e74 2065 7463 2e0a 0a44 6574 6169  vent etc...Detai
+00006140: 6c73 3a0a 0a2a 2060 4576 656e 7454 7265  ls:..* `EventTre
+00006150: 6560 2063 6f6e 7461 696e 7320 616c 6c20  e` contains all 
+00006160: 6576 656e 7473 2069 6e20 6d65 6d6f 7279  events in memory
+00006170: 2e0a 2a20 5472 6565 2068 6173 2073 6f6d  ..* Tree has som
+00006180: 6520 696d 706f 7274 616e 7420 7465 726d  e important term
+00006190: 733a 0a20 2020 2031 2e20 5f41 6e63 6573  s:.    1. _Ances
+000061a0: 746f 725f 2069 7320 616e 7920 7265 6c61  tor_ is any rela
+000061b0: 7469 7665 206f 6620 7468 6520 6576 656e  tive of the even
+000061c0: 7420 7570 2074 6865 2074 7265 6520 2867  t up the tree (g
+000061d0: 7261 6e64 7061 7265 6e74 2c20 7061 7265  randparent, pare
+000061e0: 6e74 2065 7463 2e29 2e0a 2020 2020 322e  nt etc.)..    2.
+000061f0: 205f 5061 7265 6e74 5f20 6973 206f 6e6c   _Parent_ is onl
+00006200: 7920 7468 6520 6669 7273 7420 7265 6c61  y the first rela
+00006210: 7469 7665 206f 6620 7468 6520 6576 656e  tive of the even
+00006220: 7420 7570 2074 6865 2074 7265 652e 0a20  t up the tree.. 
+00006230: 2020 2033 2e20 5f43 6869 6c64 5f20 6973     3. _Child_ is
+00006240: 2074 6865 2066 6972 7374 2072 656c 6174   the first relat
+00006250: 6976 6520 6f66 2074 6865 2065 7665 6e74  ive of the event
+00006260: 2064 6f77 6e20 7468 6520 7472 6565 2e0a   down the tree..
+00006270: 0a54 616b 6520 6120 6c6f 6f6b 2061 7420  .Take a look at 
+00006280: 7468 6520 666f 6c6c 6f77 696e 6720 4854  the following HT
+00006290: 4d4c 2074 7265 6520 746f 2075 6e64 6572  ML tree to under
+000062a0: 7374 616e 6420 7468 656d 2e0a 0a20 2020  stand them...   
+000062b0: 6060 600a 2020 2020 3c62 6f64 793e 203c  ```.    <body> <
+000062c0: 212d 2d20 616e 6365 7374 6f72 2028 6772  !-- ancestor (gr
+000062d0: 616e 6470 6172 656e 7429 2c20 6275 7420  andparent), but 
+000062e0: 6e6f 7420 7061 7265 6e74 202d 2d3e 0a20  not parent -->. 
+000062f0: 2020 2020 2020 203c 6469 763e 203c 212d         <div> <!-
+00006300: 2d20 7061 7265 6e74 2026 2061 6e63 6573  - parent & ances
+00006310: 746f 7220 2d2d 3e0a 2020 2020 2020 2020  tor -->.        
+00006320: 2020 2020 3c70 3e48 656c 6c6f 2c20 776f      <p>Hello, wo
+00006330: 726c 6421 3c2f 703e 203c 212d 2d20 6368  rld!</p> <!-- ch
+00006340: 696c 6420 2d2d 3e0a 2020 2020 2020 2020  ild -->.        
+00006350: 2020 2020 3c70 3e47 6f6f 6462 7965 213c      <p>Goodbye!<
+00006360: 2f70 3e20 3c21 2d2d 2073 6962 6c69 6e67  /p> <!-- sibling
+00006370: 202d 2d3e 0a20 2020 2020 2020 203c 2f64   -->.        </d
+00006380: 6976 3e0a 2020 2020 3c2f 626f 6479 3e0a  iv>.    </body>.
+00006390: 2020 2060 6060 0a0a 2323 2323 2043 6f6c     ```..#### Col
+000063a0: 6c65 6374 696f 6e73 0a0a 2a2a 4576 656e  lections..**Even
+000063b0: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
+000063c0: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
+000063d0: 6e20 6f66 2045 7665 6e74 5472 6565 732e  n of EventTrees.
+000063e0: 2054 6865 2063 6f6c 6c65 6374 696f 6e20   The collection 
+000063f0: 6275 696c 6473 2061 2066 6577 205f 4576  builds a few _Ev
+00006400: 656e 7454 7265 655f 2062 7920 7061 7373  entTree_ by pass
+00006410: 6564 205f 4461 7461 0a6f 626a 6563 745f  ed _Data.object_
+00006420: 2e20 416c 7468 6f75 6768 2079 6f75 2063  . Although you c
+00006430: 616e 2063 6861 6e67 6520 7468 6520 7472  an change the tr
+00006440: 6565 2064 6972 6563 746c 792c 2069 7427  ee directly, it'
+00006450: 7320 6265 7474 6572 2074 6f20 646f 2069  s better to do i
+00006460: 7420 7468 726f 7567 6820 636f 6c6c 6563  t through collec
+00006470: 7469 6f6e 7320 6265 6361 7573 6520 7468  tions because th
+00006480: 6579 2061 7265 2061 7761 7265 206f 660a  ey are aware of.
+00006490: 6064 6574 6163 6865 645f 6576 656e 7473  `detached_events
+000064a0: 6020 616e 6420 6361 6e20 736f 6c76 6520  ` and can solve 
+000064b0: 736f 6d65 2065 7665 6e74 7320 6465 7065  some events depe
+000064c0: 6e64 656e 6369 6573 2e20 5468 6520 636f  ndencies. The co
+000064d0: 6c6c 6563 7469 6f6e 2068 6173 2073 696d  llection has sim
+000064e0: 696c 6172 2066 6561 7475 7265 7320 6c69  ilar features li
+000064f0: 6b65 2061 2073 696e 676c 6520 5f45 7665  ke a single _Eve
+00006500: 6e74 5472 6565 5f0a 6275 7420 6170 706c  ntTree_.but appl
+00006510: 7969 6e67 2074 6865 6d20 666f 7220 616c  ying them for al
+00006520: 6c20 5f45 7665 6e74 5472 6565 735f 2e0a  l _EventTrees_..
+00006530: 0a2a 2a50 6172 656e 7445 7665 6e74 5472  .**ParentEventTr
+00006540: 6565 436f 6c6c 6563 7469 6f6e 2a2a 2069  eeCollection** i
+00006550: 7320 6120 636f 6c6c 6563 7469 6f6e 2073  s a collection s
+00006560: 696d 696c 6172 2074 6f20 5f45 7665 6e74  imilar to _Event
+00006570: 5472 6565 436f 6c6c 6563 7469 6f6e 5f20  TreeCollection_ 
+00006580: 6275 7420 636f 6e74 6169 6e69 6e67 206f  but containing o
+00006590: 6e6c 7920 7061 7265 6e74 2065 7665 6e74  nly parent event
+000065a0: 7320 7468 6174 0a61 7265 2072 6566 6572  s that.are refer
+000065b0: 656e 6365 6420 696e 2074 6865 2064 6174  enced in the dat
+000065c0: 6120 7374 7265 616d 2e20 5468 6520 636f  a stream. The co
+000065d0: 6c6c 6563 7469 6f6e 2068 6173 2066 6561  llection has fea
+000065e0: 7475 7265 7320 7369 6d69 6c61 7220 746f  tures similar to
+000065f0: 205f 4576 656e 7454 7265 6543 6f6c 6c65   _EventTreeColle
+00006600: 6374 696f 6e5f 2e0a 0a44 6574 6169 6c73  ction_...Details
+00006610: 3a0a 0a2a 2054 6f20 7573 6520 4554 2063  :..* To use ET c
+00006620: 6f6c 6c65 6374 696f 6e73 2079 6f75 206e  ollections you n
+00006630: 6565 6420 746f 2069 6e69 7469 616c 697a  eed to initializ
+00006640: 6520 7468 656d 2062 7920 5f45 5443 4472  e them by _ETCDr
+00006650: 6976 6572 5f2e 2044 6174 6120 736f 7572  iver_. Data sour
+00006660: 6365 7320 7573 7561 6c6c 7920 7072 6f76  ces usually prov
+00006670: 6964 6520 7468 656d 2e0a 2020 596f 7520  ide them..  You 
+00006680: 6361 6e20 6372 6561 7465 2069 7420 6279  can create it by
+00006690: 2079 6f75 7273 656c 6620 6465 7065 6e64   yourself depend
+000066a0: 696e 6720 6f6e 2079 6f75 7220 6461 7461  ing on your data
+000066b0: 2073 7472 7563 7475 7265 2e0a 2a20 5468   structure..* Th
+000066c0: 6520 636f 6c6c 6563 7469 6f6e 2068 6173  e collection has
+000066d0: 2061 2066 6561 7475 7265 2074 6f20 7265   a feature to re
+000066e0: 636f 7665 7220 6576 656e 7473 2e20 416c  cover events. Al
+000066f0: 6c20 6576 656e 7473 2074 6861 7420 6172  l events that ar
+00006700: 6520 6e6f 7420 696e 2074 6865 2072 6563  e not in the rec
+00006710: 6569 7665 6420 6461 7461 2073 7472 6561  eived data strea
+00006720: 6d2c 2062 7574 2077 6869 6368 2061 7265  m, but which are
+00006730: 0a20 2072 6566 6572 656e 6365 6420 7769  .  referenced wi
+00006740: 6c6c 2062 6520 6c6f 6164 6564 2066 726f  ll be loaded fro
+00006750: 6d20 7468 6520 6461 7461 2073 6f75 7263  m the data sourc
+00006760: 652e 0a2a 2059 6f75 2063 616e 2074 616b  e..* You can tak
+00006770: 6520 6064 6574 6163 6865 645f 6576 656e  e `detached_even
+00006780: 7473 6020 746f 2073 6565 2077 6869 6368  ts` to see which
+00006790: 2065 7665 6e74 7320 6172 6520 6d69 7373   events are miss
+000067a0: 696e 672e 0a2a 2049 6620 796f 7520 7761  ing..* If you wa
+000067b0: 6e74 2c20 796f 7520 6361 6e20 6275 696c  nt, you can buil
+000067c0: 6420 7061 7265 6e74 6c65 7373 2074 7265  d parentless tre
+000067d0: 6573 2077 6865 7265 2074 6865 206d 6973  es where the mis
+000067e0: 7369 6e67 2065 7665 6e74 7320 6172 6520  sing events are 
+000067f0: 7374 7562 6265 6420 696e 7374 6561 642e  stubbed instead.
+00006800: 204a 7573 740a 2020 7573 6520 6067 6574   Just.  use `get
+00006810: 5f70 6172 656e 746c 6573 735f 7472 6565  _parentless_tree
+00006820: 7328 2960 2e0a 0a52 6571 7569 7265 6d65  s()`...Requireme
+00006830: 6e74 733a 0a0a 312e 2045 7665 6e74 7320  nts:..1. Events 
+00006840: 7072 6f76 6964 6564 2074 6f20 4554 4320  provided to ETC 
+00006850: 6861 7665 2074 6f20 6861 7665 2060 6576  have to have `ev
+00006860: 656e 745f 6e61 6d65 602c 2060 6576 656e  ent_name`, `even
+00006870: 745f 6964 602c 2060 7061 7265 6e74 5f65  t_id`, `parent_e
+00006880: 7665 6e74 5f69 6460 2066 6965 6c64 732e  vent_id` fields.
+00006890: 2054 6865 790a 6361 6e20 6861 7665 2061   They.can have a
+000068a0: 6e6f 7468 6572 206e 616d 6573 2028 6974  nother names (it
+000068b0: 2072 6573 6f6c 7665 7320 696e 2074 6865   resolves in the
+000068c0: 2064 7269 7665 7229 2e0a 0a23 2323 2320   driver)...#### 
+000068d0: 4869 6e74 730a 0a2a 2052 656d 6f76 6520  Hints..* Remove 
+000068e0: 616c 6c20 756e 6e65 6365 7373 6172 7920  all unnecessary 
+000068f0: 6669 656c 6473 2066 726f 6d20 6576 656e  fields from even
+00006900: 7473 2062 6566 6f72 6520 7061 7373 696e  ts before passin
+00006910: 6720 746f 2061 205f 636f 6c6c 6563 7469  g to a _collecti
+00006920: 6f6e 5f20 746f 2072 6564 7563 6520 6d65  on_ to reduce me
+00006930: 6d6f 7279 2075 7361 6765 2e0a 2a20 5573  mory usage..* Us
+00006940: 6520 6073 686f 7728 2960 206d 6574 686f  e `show()` metho
+00006950: 6420 746f 2070 7269 6e74 2074 6865 2074  d to print the t
+00006960: 7265 6520 696e 2074 7265 652d 6c69 6b65  ree in tree-like
+00006970: 2076 6965 772e 0a2a 204e 6f74 6520 7468   view..* Note th
+00006980: 6174 2074 6865 2060 6765 745f 7860 206d  at the `get_x` m
+00006990: 6574 686f 6473 2077 696c 6c20 7261 6973  ethods will rais
+000069a0: 6520 616e 2065 7863 6570 7469 6f6e 2069  e an exception i
+000069b0: 6620 796f 7520 7061 7373 2061 6e20 756e  f you pass an un
+000069c0: 6b6e 6f77 6e20 6576 656e 7420 6964 2c20  known event id, 
+000069d0: 756e 6c69 6b65 2074 6865 2060 6669 6e64  unlike the `find
+000069e0: 5f78 6020 6d65 7468 6f64 7320 280a 2020  _x` methods (.  
+000069f0: 7468 6579 2072 6574 7572 6e20 4e6f 6e65  they return None
+00006a00: 292e 0a2a 2049 6620 796f 7520 7761 6e74  )..* If you want
+00006a10: 2074 6f20 6b6e 6f77 2074 6861 7420 7370   to know that sp
+00006a20: 6563 6966 6965 6420 6576 656e 7420 6578  ecified event ex
+00006a30: 6973 7473 2c20 7573 6520 7468 6520 7079  ists, use the py
+00006a40: 7468 6f6e 2060 696e 6020 6b65 7977 6f72  thon `in` keywor
+00006a50: 6420 2865 2e67 2e20 6027 6576 656e 742d  d (e.g. `'event-
+00006a60: 6964 2720 696e 2065 7665 6e74 735f 7472  id' in events_tr
+00006a70: 6565 6029 2e0a 2a20 5573 6520 7468 6520  ee`)..* Use the 
+00006a80: 7079 7468 6f6e 2060 6c65 6e60 206b 6579  python `len` key
+00006a90: 776f 7264 2074 6f20 6765 7420 6576 656e  word to get even
+00006aa0: 7473 206e 756d 6265 7220 696e 2074 6865  ts number in the
+00006ab0: 2074 7265 652e 0a0a 2323 2320 4669 656c   tree...### Fiel
+00006ac0: 6420 5265 736f 6c76 6572 730a 496e 7465  d Resolvers.Inte
+00006ad0: 7266 6163 6520 6361 6e20 6265 2066 6f75  rface can be fou
+00006ae0: 6e64 2069 6e20 6074 6832 5f64 6174 615f  nd in `th2_data_
+00006af0: 7365 7276 6963 6573 2f69 6e74 6572 6661  services/interfa
+00006b00: 6365 732f 7574 696c 732f 7265 736f 6c76  ces/utils/resolv
+00006b10: 6572 2e70 7960 2e20 200a 416c 6c20 6461  er.py`.  .All da
+00006b20: 7461 2d73 6f75 7263 6573 2073 686f 756c  ta-sources shoul
+00006b30: 6420 696d 706c 656d 656e 7420 7468 656d  d implement them
+00006b40: 2e0a 0a54 6865 2069 6465 6120 6f66 2075  ...The idea of u
+00006b50: 7369 6e67 2072 6573 6f6c 7665 7273 3a0a  sing resolvers:.
+00006b60: 4974 2073 6f6c 7665 7320 7468 6520 7072  It solves the pr
+00006b70: 6f62 6c65 6d20 6f66 2068 6176 696e 6720  oblem of having 
+00006b80: 6120 6665 7720 4461 7461 536f 7572 6365  a few DataSource
+00006b90: 7320 7769 7468 2073 696d 696c 6172 2064  s with similar d
+00006ba0: 6174 612c 0a62 7574 2077 6974 6820 6469  ata,.but with di
+00006bb0: 6666 6572 656e 7420 7761 7973 2074 6f20  fferent ways to 
+00006bc0: 6765 7420 6974 2e0a 0a54 6865 7365 2063  get it...These c
+00006bd0: 6c61 7373 6573 2070 726f 7669 6465 2079  lasses provide y
+00006be0: 6f75 2067 6574 7465 7220 6d65 7468 6f64  ou getter method
+00006bf0: 732e 0a55 7369 6e67 2074 6865 7365 2063  s..Using these c
+00006c00: 6c61 7373 6573 2061 6c6c 6f77 7320 796f  lasses allows yo
+00006c10: 7520 746f 2066 7265 656c 7920 7377 6974  u to freely swit
+00006c20: 6368 2062 6574 7765 656e 2064 6966 6665  ch between diffe
+00006c30: 7265 6e74 2064 6174 610a 666f 726d 6174  rent data.format
+00006c40: 7320 616e 6420 646f 6e27 7420 6368 616e  s and don't chan
+00006c50: 6765 2079 6f75 7220 636f 6465 2e0a 0a52  ge your code...R
+00006c60: 6573 6f6c 7665 7273 2073 6f6c 7665 2074  esolvers solve t
+00006c70: 6865 2070 726f 626c 656d 206f 6620 6461  he problem of da
+00006c80: 7461 2d66 6f72 6d61 7420 6d69 6772 6174  ta-format migrat
+00006c90: 696f 6e2e 0a2d 2066 6965 6c64 7320 706c  ion..- fields pl
+00006ca0: 6163 6520 6361 6e20 6265 2063 6861 6e67  ace can be chang
+00006cb0: 6564 0a2d 2066 6965 6c64 7320 6e61 6d65  ed.- fields name
+00006cc0: 7320 6361 6e20 6265 2063 6861 6e67 6564  s can be changed
+00006cd0: 0a0a 5265 736f 6c76 6572 7320 6361 6e20  ..Resolvers can 
+00006ce0: 776f 726b 206f 6e6c 7920 7769 7468 206f  work only with o
+00006cf0: 6e65 2065 7665 6e74 2f6d 6573 7361 6765  ne event/message
+00006d00: 2e0a 4974 206d 6561 6e73 2c20 6966 2079  ..It means, if y
+00006d10: 6f75 7220 6d65 7373 6167 6520 6861 7320  our message has 
+00006d20: 7375 622d 6d65 7373 6167 6573 2028 6c69  sub-messages (li
+00006d30: 6b65 2074 6832 2d6d 6573 7361 6765 7320  ke th2-messages 
+00006d40: 696e 206c 7764 7029 2069 7420 0a77 6f6e  in lwdp) it .won
+00006d50: 2774 2077 6f72 6b2c 2062 6563 6175 7365  't work, because
+00006d60: 2072 6573 6f6c 7665 7220 7769 6c6c 206e   resolver will n
+00006d70: 6f74 206b 6e6f 7720 7769 7468 2077 6869  ot know with whi
+00006d80: 6368 2073 7562 2d6d 6573 7361 6765 2073  ch sub-message s
+00006d90: 686f 756c 6420 6974 2077 6f72 6b2e 200a  hould it work. .
+00006da0: 0a2a 2a57 6f72 6b61 726f 756e 642a 2a20  .**Workaround** 
+00006db0: 200a 312e 2045 7870 616e 6420 616c 6c20   .1. Expand all 
+00006dc0: 796f 7572 206d 6573 7361 6765 7320 2d3e  your messages ->
+00006dd0: 2060 6e65 775f 6420 3d20 796f 7572 5f64   `new_d = your_d
+00006de0: 6174 612e 6d61 7028 4d65 7373 6167 6546  ata.map(MessageF
+00006df0: 6965 6c64 5265 736f 6c76 6572 2e65 7870  ieldResolver.exp
+00006e00: 616e 645f 6d65 7373 6167 6529 600a 322e  and_message)`.2.
+00006e10: 2055 7365 2060 4578 7061 6e64 6564 4d65   Use `ExpandedMe
+00006e20: 7373 6167 6546 6965 6c64 5265 736f 6c76  ssageFieldResolv
+00006e30: 6572 6020 696e 7374 6561 6420 6f66 2075  er` instead of u
+00006e40: 7375 616c 2060 4d65 7373 6167 6546 6965  sual `MessageFie
+00006e50: 6c64 5265 736f 6c76 6572 6020 7768 656e  ldResolver` when
+00006e60: 200a 2020 2020 796f 7520 7461 6b65 2066   .    you take f
+00006e70: 6965 6c64 7320 666f 7220 6578 7061 6e64  ields for expand
+00006e80: 6564 206d 6573 7361 6765 732e 0a0a 2a2a  ed messages...**
+00006e90: 496d 706c 656d 656e 7461 7469 6f6e 2061  Implementation a
+00006ea0: 6476 6963 653a 2a2a 0a31 2e20 7261 6973  dvice:**.1. rais
+00006eb0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
+00006ec0: 4572 726f 7220 2d2d 2069 6620 796f 7572  Error -- if your
+00006ed0: 2049 6d70 6c65 6d65 6e74 6174 696f 6e20   Implementation 
+00006ee0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
+00006ef0: 7468 6973 2067 6574 7465 722e 0a0a 2a2a  this getter...**
+00006f00: 5065 7266 6f72 6d61 6e63 6520 696d 7061  Performance impa
+00006f10: 6374 3a2a 2a0a 2d20 4974 2061 2062 6974  ct:**.- It a bit
+00006f20: 2073 6c6f 7765 7220 7468 616e 2075 7369   slower than usi
+00006f30: 6e67 206e 616b 6564 2066 6965 6c64 2061  ng naked field a
+00006f40: 6363 6573 7320 6064 6963 745b 276b 6579  ccess `dict['key
+00006f50: 275d 602e 0a0a 2323 2032 2e34 2e20 4c69  ']`...## 2.4. Li
+00006f60: 6e6b 730a 0a2d 205b 5265 706f 7274 2044  nks..- [Report D
+00006f70: 6174 6120 5072 6f76 6964 6572 5d28 6874  ata Provider](ht
+00006f80: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00006f90: 2f74 6832 2d6e 6574 2f74 6832 2d72 7074  /th2-net/th2-rpt
+00006fa0: 2d64 6174 612d 7072 6f76 6964 6572 290a  -data-provider).
+00006fb0: 2d20 5b54 6832 2044 6174 6120 5365 7276  - [Th2 Data Serv
+00006fc0: 6963 6573 2055 7469 6c73 5d28 6874 7470  ices Utils](http
+00006fd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
+00006fe0: 6832 2d6e 6574 2f74 6832 2d64 6174 612d  h2-net/th2-data-
+00006ff0: 7365 7276 6963 6573 2d75 7469 6c73 290a  services-utils).
+00007000: 0a23 2033 2e20 4265 7374 2070 7261 6374  .# 3. Best pract
+00007010: 6963 6573 0a44 6570 656e 6469 6e67 206f  ices.Depending o
+00007020: 6e20 686f 7720 796f 7520 776f 726b 2077  n how you work w
+00007030: 6974 6820 6044 6174 6120 6f62 6a65 6374  ith `Data object
+00007040: 602c 2069 7420 6361 6e20 6265 2073 6c6f  `, it can be slo
+00007050: 7720 6f66 2066 6173 742e 0a41 7320 7769  w of fast..As wi
+00007060: 7468 2061 2072 656c 6174 696f 6e61 6c20  th a relational 
+00007070: 6461 7461 6261 7365 2c20 796f 7520 6361  database, you ca
+00007080: 6e20 7772 6974 6520 6120 7175 6572 7920  n write a query 
+00007090: 7468 6174 2077 696c 6c20 7265 7475 726e  that will return
+000070a0: 2064 6174 6120 736c 6f77 6c79 206f 7220   data slowly or 
+000070b0: 7175 6963 6b6c 792c 0a74 6865 2073 616d  quickly,.the sam
+000070c0: 6520 7768 656e 2077 6f72 6b69 6e67 2077  e when working w
+000070d0: 6974 6820 6120 6044 6174 6120 6f62 6a65  ith a `Data obje
+000070e0: 6374 602e 0a0a 466f 6c6c 6f77 2074 6865  ct`...Follow the
+000070f0: 2072 756c 6573 2074 6f20 6d61 6b65 2079   rules to make y
+00007100: 6f75 7220 776f 726b 2077 6974 6820 4461  our work with Da
+00007110: 7461 206f 626a 6563 7420 6661 7374 3a0a  ta object fast:.
+00007120: 312e 2055 7365 2060 4461 7461 2e75 7365  1. Use `Data.use
+00007130: 5f63 6163 6865 2829 6020 6966 2079 6f75  _cache()` if you
+00007140: 2069 7465 7261 7465 2064 6174 6120 6d6f   iterate data mo
+00007150: 7265 2074 6861 6e20 6f6e 6520 7469 6d65  re than one time
+00007160: 2e0a 322e 2054 7279 2074 6f20 646f 6e27  ..2. Try to don'
+00007170: 7420 6974 6572 6174 6520 6f6e 6520 6044  t iterate one `D
+00007180: 6174 6120 6f62 6a65 6374 6020 696e 7369  ata object` insi
+00007190: 6465 2074 6865 206f 7468 6572 206f 6e65  de the other one
+000071a0: 2e0a 2020 2049 6620 796f 7520 7368 6f75  ..   If you shou
+000071b0: 6c64 2074 6f20 646f 2069 742c 2075 7365  ld to do it, use
+000071c0: 2073 686f 7274 2060 4461 7461 206f 626a   short `Data obj
+000071d0: 6563 7460 2066 6972 7374 2061 6e64 206c  ect` first and l
+000071e0: 6f6e 6720 6044 6174 6120 6f62 6a65 6374  ong `Data object
+000071f0: 6020 696e 7369 6465 2074 6865 206c 6f6f  ` inside the loo
+00007200: 702e 0a20 2020 4974 276c 6c20 616c 6c6f  p..   It'll allo
+00007210: 7720 796f 7520 6f70 656e 2074 6865 2063  w you open the c
+00007220: 6163 6865 2066 696c 6520 6f72 2063 7265  ache file or cre
+00007230: 6174 6520 6120 7265 7175 6573 7420 746f  ate a request to
+00007240: 2060 4461 7461 2073 6f75 7263 6560 206c   `Data source` l
+00007250: 6573 7320 6e75 6d62 6572 206f 6620 7469  ess number of ti
+00007260: 6d65 732e 0a0a 2320 342e 204f 6666 6963  mes...# 4. Offic
+00007270: 6961 6c20 4461 7461 536f 7572 6365 2069  ial DataSource i
+00007280: 6d70 6c65 6d65 6e74 6174 696f 6e73 0a0a  mplementations..
+00007290: 2d20 5b4c 6967 6874 7765 6967 6874 2044  - [Lightweight D
+000072a0: 6174 6120 5072 6f76 6964 6572 2044 6174  ata Provider Dat
+000072b0: 6120 536f 7572 6365 5d28 6874 7470 733a  a Source](https:
+000072c0: 2f2f 6769 7468 7562 2e63 6f6d 2f74 6832  //github.com/th2
+000072d0: 2d6e 6574 2f74 6832 2d64 732d 736f 7572  -net/th2-ds-sour
+000072e0: 6365 2d6c 7764 7029 0a0a 0a23 2035 2e20  ce-lwdp)...# 5. 
+000072f0: 4150 490a 0a49 6620 796f 7520 6172 6520  API..If you are 
+00007300: 6c6f 6f6b 696e 6720 666f 7220 636c 6173  looking for clas
+00007310: 7365 7320 6465 7363 7269 7074 696f 6e20  ses description 
+00007320: 7365 6520 7468 6520 5b41 5049 2044 6f63  see the [API Doc
+00007330: 756d 656e 7461 7469 6f6e 5d28 646f 6375  umentation](docu
+00007340: 6d65 6e74 6174 696f 6e2f 6170 692f 696e  mentation/api/in
+00007350: 6465 782e 6d64 292e 0a0a 2320 362e 2045  dex.md)...# 6. E
+00007360: 7861 6d70 6c65 730a 0a2d 205b 6765 745f  xamples..- [get_
+00007370: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
+00007380: 7079 5d28 6578 616d 706c 6573 2f67 6574  py](examples/get
+00007390: 5f73 7461 7274 6564 5f65 7861 6d70 6c65  _started_example
+000073a0: 2e70 7929 0a                             .py).
```

### Comparing `th2_data_services-2.0.0.dev8344817329/setup.py` & `th2_data_services-2.0.0.dev8662586819/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/data.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import copy
 import csv
+from dataclasses import dataclass
 import orjson as json
 import gc
 import pickle
 import pprint
 from warnings import warn
 from functools import partial
 from os import rename
@@ -51,42 +52,152 @@
 # LOG logger = logging.getLogger(__name__)
 
 
 # LOG class _DataLogger(logging.LoggerAdapter):
 # LOG     def process(self, msg, kwargs):
 # LOG         return "Data[%s] %s" % (self.extra["id"], msg), kwargs
 from th2_data_services.utils.path_utils import check_if_filename_valid, check_if_file_exists
+from deprecated.classic import deprecated
+
 
 DataIterValues = TypeVar("DataIterValues")
 DataGenerator = Generator[DataIterValues, None, None]
 DataSet = Union[Iterator, Callable[..., DataGenerator], List[Iterable], Iterable]
 WorkFlow = List[Dict[str, Union[Callable, str]]]
 
 
+def _build_limit_callback(num) -> Callable:
+    def callback(r):
+        callback.pushed += 1
+        if callback.pushed > num:
+            raise StopIteration(r)
+        else:
+            return r
+
+    callback.limit = num
+    callback.pushed = 0
+    return callback
+
+
+@dataclass
+class WfRecord:
+    type: str
+    callback: Callable
+
+
+@dataclass
+class WfLimitRecord(WfRecord):
+    limit: int
+
+
+class Workflow:
+    def __init__(self):
+        """Data object workflow."""
+        self._data: List[WfRecord] = []
+
+    def __bool__(self):
+        return bool(self._data)
+
+    def __str__(self):
+        return f"Workflow({pprint.pformat(self._data)})"
+
+    def __repr__(self):
+        return str(self)
+
+    def add(self, wfr: WfRecord):
+        """Add callback to workflow.
+
+        Args:
+            wfr: WfRecord
+
+        Returns:
+            self
+        """
+        self._data.append(wfr)
+        return self
+
+    # def update(self, upd_func: Callable[[List[WfRecord]], List[WfRecord]]):
+    #     self._data = upd_func(self._data)
+
+    # def _apply_record(self, record):
+    #     for wfr in self._data:
+    #         # print(f"apply '{wfr.type}' for '{record}'")
+    #         record = wfr.callback(record)
+    #         # print(f"\t --> '{record}'")
+    #
+    #     return record
+
+    def apply_records(self, records):
+        """Execute workflow against some stream.
+
+        Args:
+            records: some stream.
+
+        Yields:
+            workflow-handled records.
+        """
+        map_chain = records
+        for wfr in self._data:
+            if wfr.type == "map_stream":
+                map_chain = wfr.callback(map_chain)
+            else:
+                map_chain = map(wfr.callback, map_chain)
+
+        yield from map_chain
+
+    def refresh_limit_callbacks(self):
+        """Updates limit callbacks each time when Data object is iterated.
+
+        It used to have the possibility to iterate the same Data object
+        several times in the loops.
+        """
+        for wfr in self._data:
+            if isinstance(wfr, WfLimitRecord):
+                wfr.callback = _build_limit_callback(wfr.limit)
+
+
+# TODO
+#   Хочется уметь менять состояние дата объекта во время итерации
+
+
+# def show_message_if_exception_decorator(callback):
+#     def wrapper(stream):
+#         try:
+#             for record in stream:
+#                 yield from callback(stream)
+#         except Exception:
+#             try:
+#                 print("Exception during handling the message: \n" f"{pprint.pformat(record)}")
+#             except UnboundLocalError:
+#                 pass
+#
+#             raise
+#
+#     return wrapper
+
+
 class Data(Generic[DataIterValues]):
     """A wrapper for data/data_stream.
 
     The class provides methods for working with data as a stream.
 
-    Such approach to data analysis called streaming transformation.
+    Such an approach to data analysis called streaming transformation.
     """
 
     def __init__(
         self,
         data: DataSet,
         cache: bool = False,
-        workflow: WorkFlow = None,
         pickle_version: int = o.DEFAULT_PICKLE_VERSION,
     ):
         """Data constructor.
 
         Args:
             data: Data source. Any iterable, Data object or a function that creates generator.
             cache: Set True if you want to write and read from cache.
-            workflow: Workflow.
             pickle_version: Pickle protocol version. Set if using cache.
 
         """
         if isinstance(data, types.GeneratorType) and cache is False:
             warn(
                 "Putted data has a generator type. "
                 "Data object will work wrong in non-cache mode because generators "
@@ -105,38 +216,86 @@
         self._cache_filename = f"{self._id}_{time()}.pickle"
         self._cache_path = Path("temp", self._cache_filename).resolve().absolute()
         self._pending_cache_path = (
             self._cache_path.with_name("[PENDING]" + self._cache_filename).resolve().absolute()
         )
         self._cache_file_obj = None
         self._len = None
-        self._workflow = (
-            [] if workflow is None else workflow
-        )  # Normally it has empty list or one Step.
+        self.workflow = Workflow()
+
         self._length_hint = None  # The value is populated when we use limit method.
         self._cache_status = cache
         # We use finalize instead of __del__ because __del__ won't be executed sometimes.
         # Read more about __del__ problems here: https://stackoverflow.com/a/2452895
         self._finalizer = finalize(self, self.__remove)
         # LOG         self._logger = _DataLogger(logger, {"id": self._id})
         # It used to indicate the number of current iteration of the Data object.
         # It's required if the same instance iterates several times in for-in loops.
         self.iter_num = 0  # Indicates what level of the loop the Data object is in.
-        self.stop_iteration = None
+        self._stop_iteration = None
         self._read_from_external_cache_file = False
         self.__metadata = {}
         self._pickle_version = pickle_version  # Default pickle protocol version
 
     # LOG         self._logger.info(
     # LOG            "New data object with data stream = '%s', cache = '%s' initialized", id(self._data_stream), cache
     # LOG        )
 
-    @property
-    def metadata(self):
-        return self.__metadata
+    def __str__(self):
+        s = f"Data({id(self)}\n" f"     {self.workflow}\n" f"     metadata={self.metadata})"
+        return s
+
+    def __repr__(self):
+        return str(self)
+
+    def __bool__(self):
+        for _ in self:
+            return True
+        return False
+
+    def __add__(self, other_data: Iterable) -> "Data":
+        """Joining feature.
+
+        Don't keep cache status.
+
+        e.g. data3 = data1 + data2  -- data3 will have cache_status = False.
+        """
+        data = Data(self._create_data_set_from_iterables([self, other_data]))
+        data._set_metadata(self.metadata)
+        if isinstance(other_data, Data):
+            data.update_metadata(other_data.metadata)
+        return data
+
+    def __iadd__(self, other_data: Iterable) -> "Data":
+        """Joining feature.
+
+        Keeps cache status.
+
+        e.g. data1 += data2  -- will keep the cache status of data1.
+        """
+        return self.__add__(other_data).use_cache(self._cache_status)
+
+    def _set_custom_cache_destination(self, filename):
+        path = Path(filename).resolve()
+        self._cache_filename = path.name
+        self._cache_path = path
+        self._cache_status = True
+        self._read_from_external_cache_file = True
+
+    def _copy_cache_file(self, new_name):
+        from shutil import copy2
+
+        copy2(self.get_cache_filepath(), new_name)
+
+    def __copy__(self):
+        obj = Data(self._data_stream, pickle_version=self._pickle_version)
+        obj._set_metadata(self.metadata)
+        obj.workflow = copy.deepcopy(self.workflow)
+
+        return obj
 
     def __remove(self):
         """Data class destructor."""
         if self.__is_cache_file_exists() and not self._read_from_external_cache_file:
             self.__delete_cache()
         del self._data_stream
 
@@ -165,39 +324,15 @@
         """Creates a generator from the list of iterables."""
         for data in iterables_list:
             yield from data
 
     def _is_iterables_list(self, data: DataSet) -> bool:
         if not isinstance(data, (list, tuple)):
             return False
-
-        return all([isinstance(d, (Data, tuple, list)) for d in data])
-
-    @property
-    def len(self) -> int:
-        """int: How many records in the Data stream.
-
-        Notes:
-        1. It is a wasteful operation if you are performing it on the Data object that has never been iterated before.
-
-        2. If you want just to check emptiness, use is_empty property instead.
-        """
-        return self._len if self._len is not None else self.__calc_len()
-
-    # Actually it should be a function, not a property.
-    @property
-    def is_empty(self) -> bool:
-        """bool: Indicates that the Data object doesn't contain data."""
-        for _ in self:
-            return False
-        return True
-
-    @property
-    def cache_status(self) -> bool:
-        return self._cache_status
+        return all(isinstance(d, Data) for d in data)
 
     def __calc_len(self) -> int:
         for _ in self:
             pass
         return self._len
 
     def __length_hint__(self):
@@ -212,28 +347,29 @@
             return 8192
 
     def _iter_logic(self):
         interruption = True
         if self._cache_status and self.__is_cache_file_exists():
             is_data_writes_cache = False
         else:
+            # FIXME -- bug -- мы считаем что мы пишем файл, когда он уже существует а мы его просто читаем
             is_data_writes_cache = True
 
         try:
             for record in self.__load_data(self._cache_status):
                 yield record
             else:
                 # Loop successfully finished. Do not delete cache file.
                 # LOG                 self._logger.debug("Successfully iterated")
                 interruption = False
 
         finally:
             if interruption:
 
-                if self.stop_iteration:  # When limit was reached.
+                if self._stop_iteration:  # When limit was reached.
                     # You can save _len in this case because iteration was stopped by limit.
                     # LOG                     self._logger.info("Iteration was interrupted because limit reached")
                     pass
                 else:  # When something went wrong but NOT StopIteration
                     # LOG                     self._logger.info("Iteration was interrupted")
                     # You shouldn't save _len in this case because iteration was interrupted.
                     if self.iter_num == 1:
@@ -250,146 +386,98 @@
                     # Do not delete cache file if it reads an external cache file.
                     if not self._read_from_external_cache_file:
                         # Do not delete cache file if it's an interactive mode and Data has read cache.
                         if not o.INTERACTIVE_MODE:
                             self.__delete_cache()
 
             self.iter_num -= 1
-            self.stop_iteration = False
+            self._stop_iteration = False
 
     def __iter__(self) -> DataGenerator:
-        self.stop_iteration = False
+        self._stop_iteration = False
         self.iter_num += 1
         # LOG         self._logger.info("Starting iteration, iter_num = %s", self.iter_num)
+
         if self._len is None and self.iter_num == 1:
             self._len = 0
             for record in self._iter_logic():
                 self._len += 1
                 yield record
         else:
             # Do not calculate self._len if it is not None.
             yield from self._iter_logic()
 
-    def _build_workflow(self, workflow):
+    def _build_workflow(self, workflow: Workflow):
         """Updates limit callbacks each time when Data object is iterated.
 
-        It used to have possibility iterate the same Data object several times in the loops.
+        It used to have the possibility to iterate the same Data object
+        several times in the loops.
         """
         new_workflow = copy.deepcopy(workflow)
-        for w in new_workflow[::-1]:
-            if w["type"] == "limit":
-                w["callback"] = self._build_limit_callback(w["callback"].limit)
+        new_workflow.refresh_limit_callbacks()
 
         return new_workflow
 
+    def _build_data_stream(self):
+        return self._data_stream() if callable(self._data_stream) else self._data_stream
+
     def __load_data(self, cache: bool) -> DataGenerator:
         """Loads data from cache or data.
 
         Args:
             cache: Flag if you what to write and read from cache.
 
         Returns:
             obj: Generator
         """
         if cache and self.__is_cache_file_exists():
             # LOG             self._logger.info("Iterating using own cache file '%s'" % self.get_cache_filepath())
             data_stream = self.__load_file(self.get_cache_filepath())
             yield from data_stream
         else:
-            data_stream = self._data_stream() if callable(self._data_stream) else self._data_stream
-            workflow = self._build_workflow(self._workflow)
+            data_stream = self._build_data_stream()  # we do it for every iterable data object.
+            workflow = self._build_workflow(self.workflow)
 
             if self.__check_file_recording():
                 # Do not read from the cache file if it has PENDING status (if the file is not filled yet).
                 # It used to handle case when Data object iterates in the loop several times.
                 cache = False
 
-            yield from self.__change_data(data_stream=data_stream, workflow=workflow, cache=cache)
+            if workflow:
+                iteration_obj = workflow.apply_records(data_stream)
+            else:
+                iteration_obj = data_stream
+
+            if cache:
+                filepath = self.get_pending_cache_filepath()
+                filepath.parent.mkdir(exist_ok=True)
+                # LOG             self._logger.debug("Recording cache file '%s'" % filepath)
+                self._cache_file_obj = open(filepath, "wb")
+
+                for modified_record in iteration_obj:
+                    pickle.dump(
+                        modified_record, self._cache_file_obj, protocol=self._pickle_version
+                    )
+                    yield modified_record
+
+                self._cache_file_obj.close()
+                rename(self._cache_file_obj.name, str(self.get_cache_filepath()))
+            # LOG             self._logger.debug("Cache file was created '%s'" % self.get_cache_filepath())
+            else:
+                yield from iteration_obj
 
     def __check_file_recording(self) -> bool:
         """Checks whether there is a current recording in the file.
 
         Returns:
             bool: File recording status.
         """
         path = self.get_pending_cache_filepath()
         return path.is_file()
 
-    def get_pending_cache_filepath(self) -> Path:
-        """Returns filepath for a pending cache file."""
-        return self._pending_cache_path
-
-    def get_cache_filepath(self) -> Path:
-        """Returns filepath for a cache file."""
-        return self._cache_path
-
-    def _iterate_modified_data_stream(
-        self, data_stream: DataGenerator, workflow: WorkFlow
-    ) -> DataGenerator:
-        """Returns generator that iterates data stream with applied workflow.
-
-        StopIteration from limit function will be handled here.
-        """
-        # LOG         self._logger.debug("Iterating data stream = '%s'", id(data_stream))
-        for record in data_stream:
-            try:
-                modified_records = self.__apply_workflow(record, workflow)
-            except StopIteration as e:
-                # LOG                 self._logger.debug("Handle StopIteration")
-                modified_records = e.value
-
-                if modified_records is not None:
-                    if isinstance(modified_records, (list, tuple)):
-                        yield from modified_records
-                    else:  # Just one record.
-                        yield modified_records
-
-                # There is some magic.
-                # It'll stop data stream and will be handled in the finally statements.
-                # If you put return not under except block it will NOT work.
-                #
-                # It happens because python returns control to data_stream here due to `yield`.
-                return
-
-            if modified_records is None:
-                continue
-            elif isinstance(modified_records, (list, tuple)):
-                yield from modified_records
-            else:  # Just one record.
-                yield modified_records
-
-    def __change_data(
-        self, data_stream: DataGenerator, workflow: WorkFlow, cache: bool
-    ) -> DataGenerator:
-        """Applies workflow for data.
-
-        Args:
-            data_stream: Data for apply workflow.
-            workflow: Workflow.
-            cache: Set True if you are going to write and read from the cache.
-
-        Yields:
-            obj: Generator
-        """
-        if cache:
-            filepath = self.get_pending_cache_filepath()
-            filepath.parent.mkdir(exist_ok=True)  # Create dir if it does not exist.
-            # LOG             self._logger.debug("Recording cache file '%s'" % filepath)
-            self._cache_file_obj = open(filepath, "wb")
-
-            for modified_record in self._iterate_modified_data_stream(data_stream, workflow):
-                pickle.dump(modified_record, self._cache_file_obj, protocol=self._pickle_version)
-                yield modified_record
-
-            self._cache_file_obj.close()
-            rename(self._cache_file_obj.name, str(self.get_cache_filepath()))
-        # LOG             self._logger.debug("Cache file was created '%s'" % self.get_cache_filepath())
-        else:
-            yield from self._iterate_modified_data_stream(data_stream, workflow)
-
     def __is_cache_file_exists(self) -> bool:
         """Checks whether cache file exist."""
         path = self.get_cache_filepath()
         r = path.is_file()
         # LOG         self._logger.debug("Cache file exists" if r else "Cache file doesn't exist")
         return r
 
@@ -404,127 +492,147 @@
         """
         if not filepath.exists():
             raise FileNotFoundError(f"{filepath} doesn't exist")
 
         if not filepath.is_file():
             raise FileExistsError(f"{filepath} isn't file")
 
-        with open(filepath, "rb") as file:
-            while True:
-                try:
-                    decoded_data = pickle.load(file)
-                    yield decoded_data
-                except EOFError:
-                    break
-                except pickle.UnpicklingError:
-                    print(f"Cannot read {filepath} cache file")
-                    raise
+        yield from _iter_pickle_file_logic(filepath)
+        # with open(filepath, "rb") as file:
+        #     while True:
+        #         try:
+        #             decoded_data = pickle.load(file)
+        #             yield decoded_data
+        #         except EOFError:
+        #             break
+        #         except pickle.UnpicklingError:
+        #             print(f"Cannot read {filepath} cache file")
+        #             raise
+
+    # def _process_step(self, step: dict, record):
+    #     res = step["callback"](record)
+    #     # LOG         self._logger.debug("    - step '%s' -> %s", step["type"], res)
+    #     return res
+
+    # def __apply_workflow(
+    #     self, record: Any, workflow: WorkFlow
+    # ) -> Optional[Union[dict, List[dict]]]:
+    #     """Creates generator records with apply workflow.
+    #
+    #     Returns:
+    #         obj: Generator records.
+    #
+    #     """
+    #     # LOG         self._logger.debug("Apply workflow for %s", record)
+    #     for step in workflow:
+    #         try:
+    #             # TODO -2 -- мы каждый раз делаем step["callback"](record)
+    #             # TODO -3 -- по факту мы сейчас не используем воркфлоу, а ка
+    #             #  каждый раз создаём новый дата объект
+    #             #   у этого есть минусы -- эксепшен с итерациями,
+    #             #   и когда много объектов вложены доуг в друга, это медленно работает
+    #             record = self._process_step(step, record)
+    #             if record is None:
+    #                 break  # Break workflow iteration if step result is None.
+    #         except StopIteration:
+    #             raise
+    #
+    #     # LOG         self._logger.debug("-> %s", record)
+    #     return record
 
-    def _process_step(self, step: dict, record):
-        res = step["callback"](record)
-        # LOG         self._logger.debug("    - step '%s' -> %s", step["type"], res)
-        return res
-
-    def __apply_workflow(
-        self, record: Any, workflow: WorkFlow
-    ) -> Optional[Union[dict, List[dict]]]:
-        """Creates generator records with apply workflow.
+    @property
+    def metadata(self):
+        return self.__metadata
 
-        Returns:
-            obj: Generator records.
+    @property
+    def len(self) -> int:
+        """int: How many records in the Data stream.
 
+        Notes:
+        1. It is a wasteful operation if you are performing it on the Data object that has never been iterated before.
+
+        2. If you want just to check emptiness, use is_empty property instead.
         """
-        # LOG         self._logger.debug("Apply workflow for %s", record)
-        for step in workflow:
-            if isinstance(record, (list, tuple)):
-                result = []
-                for r in record:
-                    step_res = None
-                    try:
-                        step_res = self._process_step(step, r)
-                    except StopIteration as e:
-                        step_res = e.value
-                        raise StopIteration(result if result else None)
-                    finally:
-                        if step_res is not None:
-                            if isinstance(step_res, (list, tuple)):
-                                result += step_res  # To make flat list.
-                            else:
-                                result.append(step_res)
-
-                record = result
-                if not record:
-                    record = None
-                    break  # Break iteration if step result is None.
-            else:
-                try:
-                    record = self._process_step(step, record)
-                    if record is None:
-                        break  # Break workflow iteration if step result is None.
-                except StopIteration:
-                    raise
+        return self._len if self._len is not None else self.__calc_len()
+
+    @property
+    def is_empty(self) -> bool:
+        """bool: Indicates that the Data object doesn't contain data."""
+        for _ in self:
+            return False
+        return True
+
+    @property
+    def cache_status(self) -> bool:
+        return self._cache_status
+
+    def get_pending_cache_filepath(self) -> Path:
+        """Returns filepath for a pending cache file."""
+        return self._pending_cache_path
 
-        # LOG         self._logger.debug("-> %s", record)
-        return record
+    def get_cache_filepath(self) -> Path:
+        """Returns filepath for a cache file."""
+        return self._cache_path
 
     def filter(self, callback: Callable) -> "Data":
         """Append `filter` to workflow.
 
         Args:
             callback: Filter function.
                 This function should return True or False.
                 If function returns False, the record will be removed from the dataflow.
 
         Returns:
             Data: Data object.
 
         """
 
-        def get_source(handler):
-            yield from handler(self)
-
         def filter_yield(stream):
             try:
                 for record in stream:
                     if callback(record):
                         yield record
             except Exception:
                 try:
                     print("Exception during filtering the message: \n" f"{pprint.pformat(record)}")
                 except UnboundLocalError:
                     pass
 
                 raise
 
-        source = partial(get_source, filter_yield)
-        data = Data(source)
-        data._set_metadata(self.metadata)
-        return data
+        new_data = self.map_stream(filter_yield)
+        # TODO - rename workflow type map_stream to filter
+
+        return new_data
 
     def map(self, callback_or_adapter: Union[Callable, IRecordAdapter]) -> "Data":
         """Append `transform` function to workflow.
 
         Args:
             callback_or_adapter: Transform function or an Adapter with IRecordAdapter
                 interface implementation.
-                If the function returns None value, this value will be skipped from OUT stream.
-                If you don't want skip None values -- use `map_stream`.
+                Note:
+                    - If the function returns None value, this value will be
+                    pushed to the next workflow function.
+                    If you want to skip None values -- use `map_stream` instead.
 
         Returns:
             Data: Data object.
 
         """
         # LOG         self._logger.info("Apply map")
+
+        new_data = copy.copy(self)
+
         if isinstance(callback_or_adapter, IRecordAdapter):
-            new_workflow = [{"type": "map", "callback": callback_or_adapter.handle}]
+            new_data.workflow.add(WfRecord(type="map", callback=callback_or_adapter.handle))
         else:
-            new_workflow = [{"type": "map", "callback": callback_or_adapter}]
-        data = Data(data=self, workflow=new_workflow)
-        data._set_metadata(self.metadata)
-        return data
+            new_data.workflow.add(WfRecord(type="map", callback=callback_or_adapter))
+
+        return new_data
 
     def map_stream(
         self, adapter_or_generator: Union[IStreamAdapter, Callable[..., Generator]]
     ) -> "Data":
         """Append `stream-transform` function to workflow.
 
         If StreamAdapter is passed StreamAdapter.handle method will be used as a map function.
@@ -538,86 +646,79 @@
         Args:
             adapter_or_generator: StreamAdapter object or generator function.
 
         Returns:
             Data: Data object.
 
         """
-
-        def get_source(handler):
-            yield from handler(self)
+        new_data = copy.copy(self)
 
         if isinstance(adapter_or_generator, IStreamAdapter) and isgeneratorfunction(
             adapter_or_generator.handle
         ):
-            source = partial(get_source, adapter_or_generator.handle)
+            callback = adapter_or_generator.handle
+
         elif isgeneratorfunction(adapter_or_generator):
-            source = partial(get_source, adapter_or_generator)
+            callback = adapter_or_generator
+
         else:
             raise Exception(
                 "map_stream Only accepts IStreamAdapter class with generator function or Generator function"
             )
-        data = Data(source)
-        data._set_metadata(self.metadata)
-        return data
 
-    def _build_limit_callback(self, num) -> Callable:
-        # LOG         self._logger.debug("Build limit callback with limit = %s", num)
+        new_data.workflow.add(WfRecord(type="map_stream", callback=callback))
 
-        def callback(r):
-            callback.pushed += 1
-            if callback.pushed == num:
-                callback.pushed = 0
-                # LOG                 self._logger.debug("Limit reached - raise StopIteration")
-                raise StopIteration(r)
-            else:
-                return r
+        return new_data
 
-        callback.limit = num
-        callback.pushed = 0
-        return callback
+        # data = Data(source)
+        # data._set_metadata(self.metadata)
+        # return data
+
+    def map_yield(self, callback_or_adapter: Union[Callable, IRecordAdapter]) -> "Data":
+        """Maps the stream using callback function or adapter.
+
+        Differences between map and map yield:
+        1. map_yield is a wrapper function using map_stream.
+        2. map_yield iterates over each item in record if callback returns
+        a value, which is a list or tuple.
+
+        Args:
+            callback_or_adapter: Transform function or an Adapter with IRecordAdapter interface implementation.
+
+        Returns:
+            Data: Data object.
+
+        """
+
+        def generator(stream):
+            for record in stream:
+                modified_record = callback_or_adapter(record)
+                if isinstance(modified_record, (list, tuple)):
+                    for item in modified_record:
+                        yield item
+                else:
+                    yield modified_record
+
+        return self.map_stream(generator)
 
     def limit(self, num: int) -> "Data":
         """Limits the stream to `num` entries.
 
         Args:
             num: How many records will be provided.
 
         Returns:
             Data: Data object.
         """
         # LOG         self._logger.info("Apply limit = %s", num)
-        # def get_source(handler):
-        #     try:
-        #         yield from handler(self)
-        #     except StopIteration as e:
-        #
-        #         # There is some magic.
-        #         # It'll stop data stream and will be handled in the finally statements.
-        #         # If you put return not under except block it will NOT work.
-        #         #
-        #         # It happens because python returns control to data_stream here due to `yield`.
-        #         return
-        #
-        # def filter_yield(stream):
-        #     callback = self._build_limit_callback(num)
-        #     for record in stream:
-        #         if callback(record):
-        #             yield record
-        #
-        # source = partial(get_source, filter_yield)
-        # data = Data(source)
-        # data._length_hint = num
-        # data._set_metadata(self.metadata)
-        # return data
-
-        new_workflow = [{"type": "limit", "callback": self._build_limit_callback(num)}]
-        data_obj = Data(data=self, workflow=new_workflow)
+        data_obj = copy.copy(self)
+        data_obj.workflow.add(
+            WfLimitRecord(type="limit", callback=_build_limit_callback(num), limit=num)
+        )
         data_obj._length_hint = num
-        data_obj._set_metadata(self.metadata)
         return data_obj
 
     def sift(self, limit: int = None, skip: int = None) -> Generator[dict, None, None]:
         """Skips and limits records.
 
         Args:
             limit: Limited records.
@@ -698,94 +799,59 @@
             file: Path to file.
 
         """
         with open(file, "w") as txt_file:
             for record in self:
                 txt_file.write(f"{pprint.pformat(record)}\n" + ("-" * 50) + "\n")
 
-    def __str__(self):
-        output = "------------- Printed first 5 records -------------\n"
+    def show(self, n=5, print_=True):
+        print("------------- Printed first 5 records -------------")
         for index, record in enumerate(self):
-            if index == 5:
+            if index == n:
                 break
-            output += pprint.pformat(record) + "\n"
-        return output
-
-    def __bool__(self):
-        for _ in self:
-            return True
-        return False
+            pprint.pprint(record)
 
-    def __add__(self, other_data: Iterable) -> "Data":
-        """Joining feature.
-
-        Don't keep cache status.
-
-        e.g. data3 = data1 + data2  -- data3 will have cache_status = False.
-        """
-        data = Data(self._create_data_set_from_iterables([self, other_data]))
-        data._set_metadata(self.metadata)
-        if isinstance(other_data, Data):
-            data.update_metadata(other_data.metadata)
-        return data
-
-    def __iadd__(self, other_data: Iterable) -> "Data":
-        """Joining feature.
-
-        Keeps cache status.
-
-        e.g. data1 += data2  -- will keep the cache status of data1.
-        """
-        return self.__add__(other_data).use_cache(self._cache_status)
-
-    def _set_custom_cache_destination(self, filename):
-        path = Path(filename).resolve()
-        self._cache_filename = path.name
-        self._cache_path = path
-        self._cache_status = True
-        self._read_from_external_cache_file = True
-
-    def _copy_cache_file(self, new_name):
-        from shutil import copy2
-
-        copy2(self.get_cache_filepath(), new_name)
-
-    def build_cache(self, filename):
+    def build_cache(self, filename, pickle_version: Optional[int] = None):
         """Creates cache file with provided name.
 
         Important:
             If the Data object cache status is True, it'll iterate itself. As a result the cache file
              will be created and copied.
             When you will iterate the Data object next time, it'll iterate created cache file.
 
             NOTE! If you build cache file, Data.cache_status was False and after that you'll set
              Data.cache_status == TRUE -- the Data object WON'T iterate build file because it doesn't
              keep the path to built cache file..
 
         Args:
             filename: Name or path to cache file.
+            pickle_version: Pickle protocol version. Change the default value
+                if you want to create pickle file with another pickle version.
 
         """
         path_name = Path(filename).name
         status, reason = check_if_filename_valid(path_name)
         if not status:
             raise Exception(f"Cannot build cache file. {reason}")
 
+        if pickle_version is None:
+            pickle_version = self._pickle_version
+
         if self.__is_cache_file_exists():
             self._copy_cache_file(filename)
         else:
             gc.disable()  # https://exactpro.atlassian.net/browse/TH2-4775
             if self._cache_status:
                 _ = self.len  # Just to iterate
                 self._copy_cache_file(filename)
             else:
                 file = open(filename, "wb")
 
                 for record in self:
-                    pickle.dump(record, file, protocol=self._pickle_version)
+                    pickle.dump(record, file, protocol=pickle_version)
 
                 file.close()
             gc.enable()
 
     def clear_cache(self):
         """Clears related to data object cache file.
 
@@ -795,38 +861,39 @@
             raise Exception("It's not possible to remove external cache file via this method")
         else:
             if self.__is_cache_file_exists():
                 self.__delete_cache()
 
     @classmethod
     def from_cache_file(cls, filename, pickle_version: int = o.DEFAULT_PICKLE_VERSION) -> "Data":
-        """Creates Data object from cache file with provided name.
+        """Creates Data object from cache file with the provided name.
 
         Args:
             filename: Name or path to cache file.
-            pickle_version: Pickle protocol version. Change default value
+            pickle_version: Pickle protocol version. Change the default value
                 if your pickle file was created with another pickle version.
 
         Returns:
             Data: Data object.
 
         Raises:
             FileNotFoundError if provided file does not exist.
 
         """
         check_if_file_exists(filename)
-        data_obj = cls([], cache=True)
-        data_obj._set_custom_cache_destination(filename=filename)
-        data_obj.update_metadata({"source_file": filename})
+
+        path = Path(filename).resolve()
+        data_obj = cls(_iter_pickle_cache_file(path, pickle_version))
+        data_obj.update_metadata({"source_file": path})
         data_obj._pickle_version = pickle_version
         return data_obj
 
     @classmethod
     def from_json(cls, filename, buffer_limit=250, gzip=False) -> "Data[dict]":
-        """Creates Data object from json file with provided name.
+        """Creates Data object from json-lines file with provided name.
 
         Args:
             filename: Name or path to cache file.
             buffer_limit: If limit is 0 buffer will not be used. Number of messages in buffer before parsing.
             gzip: Set to true if file is json file compressed using gzip.
 
         Returns:
@@ -842,15 +909,15 @@
         else:
             data = cls(iter_json_file(filename, buffer_limit))
         data.update_metadata({"source_file": filename})
         return data
 
     @classmethod
     def from_any_file(cls, filename, mode="r") -> "Data[str]":
-        """Creates Data object from any file with provided name.
+        """Creates a Data object from any file with the provided name.
 
         It will just iterate file and return data line be line.
 
         Args:
             filename: Name or path to the file.
             mode: Read mode of open function.
 
@@ -864,17 +931,22 @@
         check_if_file_exists(filename)
         data = cls(_iter_any_file(filename, mode))
         data.update_metadata({"source_file": filename})
         return data
 
     @classmethod
     def from_csv(
-        cls, filename, header=None, header_first_line=False, mode="r", delimiter=","
+        cls,
+        filename: Union[str, Path],
+        header=None,
+        header_first_line=False,
+        mode="r",
+        delimiter=",",
     ) -> "Data":
-        """Creates Data object from CSV file with provided name.
+        """Creates Data object from CSV file with the provided name.
 
         It will iterate the CSV file as if you were doing it with CSV module.
 
         Args:
             filename: Name or path to the file.
             header: If provided header for csv, Data object will yield Dict[str].
                 Note, if your first line is header in csv, it also will be yielded.
@@ -897,27 +969,14 @@
             FileNotFoundError if provided file does not exist.
 
         """
         # TODO - bug here TH2-4930 - new data object doesn't work with limit method
         check_if_file_exists(filename)
         data = cls(_iter_csv(filename, header, header_first_line, mode, delimiter))
         data.update_metadata({"source_file": filename})
-
-        # TH2-4930
-        # TODO - should be deleted after bugfix
-        if header is None and not header_first_line:
-
-            def limit(*args, **kwargs):
-                raise RuntimeError(
-                    "The data object that was get by using 'from_csv' "
-                    "cannot work with 'limit' method. Known issue TH2-4930."
-                )
-
-            data.limit = limit
-
         return data
 
     def _set_metadata(self, metadata: Dict) -> None:
         """Set metadata of object to metadata argument.
 
         Args:
             metadata (dict): New Metadata
@@ -927,15 +986,15 @@
         """
         if not isinstance(metadata, Dict):
             raise Exception("metadata must be dictionary!")
 
         self.__metadata = copy.deepcopy(metadata)
 
     def update_metadata(self, metadata: Dict) -> "Data":
-        """Update metadata of object with metadata argument.
+        """Update metadata of the object with metadata argument.
 
         Metadata is updated with new values, meaning previous values are kept and added with new values.
 
         | Example:
         | data = Data(...)
         | # data.metadata => {'num': 1, 'nums': [1], 'letters': {'a': 97}}
         | new_metadata = {'num': 9, 'nums': [7], 'letters': {'z': 122}, 'new': 'key'}
@@ -975,60 +1034,97 @@
                         self.__metadata[k] = v
             else:
                 # Add New Item
                 self.__metadata[k] = v
 
         return self
 
-    def to_json(self, filename: str, indent: int = None, overwrite: bool = False):
-        """Converts data to json format.
+    def to_json(self, filename: Union[str, Path], indent: int = None, overwrite: bool = False):
+        """Converts data to valid json format.
 
         Args:
             filename (str): Output JSON filename
             indent (int, optional): JSON format indent. Defaults to None.
             overwrite (bool, optional): Overwrite if filename exists. Defaults to False.
 
+        NOTE:
+            Data object can iterate not only dicts. So not every data can be
+            saved as json.
+
         Raises:
             FileExistsError: If file exists and overwrite=False
         """
         if Path(filename).absolute().exists() and not overwrite:
             raise FileExistsError(
                 f"{filename} already exists. If you want to overwrite current file set `overwrite=True`"
             )
 
         with open(filename, "w", encoding="UTF-8") as file:
             file.write("[")  # Start list
             for record in self:
+                # TODO
+                (json.dumps(record) + b"\n").decode()
                 json.dump(record, file, indent=indent)
                 file.write(",\n")
             file.seek(file.tell() - 3)  # Delete last comma for valid JSON
             file.write("]")  # Close list
 
+    @deprecated(
+        reason="Use `to_json_lines` instead. " "`to_jsons` will be removed on 2.0.0 release."
+    )
     def to_jsons(
         self,
-        filename: str,
+        filename: Union[str, Path],
         indent: int = None,
         overwrite: bool = False,
         gzip=False,
         compresslevel=5,
     ):
-        """Converts data to jsons format.
+        """[DEPRECATED] Converts data to json lines.
 
-        `Jsons format` means every line is a valid json, but the whole file - not.
+        Every line is a valid json, but the whole file - not.
 
         Args:
             filename (str): Output JSON filename.
             indent (int, optional): DON'T used now.
             overwrite (bool, optional): Overwrite if filename exists. Defaults to False.
             gzip: Set to True if you want to compress the file using gzip.
             compresslevel: gzip compression level.
 
         Raises:
             FileExistsError: If file exists and overwrite=False
         """
+        return self.to_json_lines(filename, indent, overwrite, gzip, compresslevel)
+
+    def to_json_lines(
+        self,
+        filename: Union[str, Path],
+        indent: int = None,
+        overwrite: bool = False,
+        gzip: bool = False,
+        compresslevel: int = 5,
+    ):
+        """Converts Data to json lines.
+
+        Every line is a valid json, but the whole file - not.
+
+        Args:
+            filename (str): Output JSON filename.
+            indent (int, optional): DON'T used now.
+            overwrite (bool, optional): Overwrite if filename exists. Defaults to False.
+            gzip: Set to True if you want to compress the file using gzip.
+            compresslevel: gzip compression level.
+
+        NOTE:
+            Data object can iterate not only dicts. So not every data can be
+            saved as json.
+
+        Raises:
+            FileExistsError: If file exists and overwrite=False
+        """
         if Path(filename).absolute().exists() and not overwrite:
             raise FileExistsError(
                 f"{filename} already exists. If you want to overwrite current file set `overwrite=True`"
             )
 
         if gzip:
             with gzip_.open(filename, "wb", compresslevel=compresslevel) as f:
@@ -1036,15 +1132,15 @@
                     f.write(json.dumps(record) + b"\n")
         else:
             with open(filename, "w", encoding="UTF-8") as file:
                 for record in self:
                     file.write((json.dumps(record) + b"\n").decode())
 
 
-def _iter_any_file(filename, mode="r"):
+def _iter_any_file(filename: Union[str, Path], mode="r"):
     """Returns the function that returns generators."""
 
     def iter_any_file_logic():
         with open(filename, mode) as data:
             while True:
                 try:
                     v = data.readline()
@@ -1059,15 +1155,17 @@
     def iter_any_file_wrapper(*args, **kwargs):
         """Wrapper function that allows passing arguments to the generator."""
         return iter_any_file_logic(*args, **kwargs)
 
     return iter_any_file_wrapper
 
 
-def _iter_csv(filename, header=None, header_first_line=False, mode="r", delimiter=","):
+def _iter_csv(
+    filename: Union[str, Path], header=None, header_first_line=False, mode="r", delimiter=","
+):
     """Returns the function that returns generators."""
 
     def iter_logic():
         with open(filename, mode) as data:
             if header is not None and header_first_line:
                 reader = csv.DictReader(data, fieldnames=header, delimiter=delimiter)
                 next(reader)  # Skip first line with header.
@@ -1075,14 +1173,41 @@
                 reader = csv.DictReader(data, fieldnames=header, delimiter=delimiter)
             elif header_first_line:
                 reader = csv.DictReader(data, delimiter=delimiter)
             else:
                 reader = csv.reader(data, delimiter=delimiter)
 
             for row in reader:
-                yield (row,)  # Because if provide just a list it will iterate it.
+                yield row
 
     def iter_wrapper(*args, **kwargs):
         """Wrapper function that allows passing arguments to the generator."""
         return iter_logic(*args, **kwargs)
 
     return iter_wrapper
+
+
+def _iter_pickle_file_logic(filepath):
+    """Generator that reads and yields decoded JSON objects from a file.
+
+    The protocol version of the pickle is detected automatically,
+    so no protocol argument is needed. Bytes past the pickled representation
+    of the object are ignored.
+    """
+    with open(filepath, "rb") as file:
+        while True:
+            try:
+                decoded_data = pickle.load(file)
+                yield decoded_data
+            except EOFError:
+                break
+            except pickle.UnpicklingError:
+                print(f"Cannot read {filepath} cache file")
+                raise
+
+
+def _iter_pickle_cache_file(filepath: Path, pickle_version: int):
+    def iter_json_file_wrapper(*args, **kwargs):
+        """Wrapper function that allows passing arguments to the generator."""
+        return _iter_pickle_file_logic(filepath)
+
+    return iter_json_file_wrapper
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_json.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  limitations under the License.
 
 from typing import Generator
 import gzip
 
 import orjson as json
 from orjson import JSONDecodeError
+
 from th2_data_services.utils.decode_error_handler import UNICODE_REPLACE_HANDLER
 
 
 def iter_json_file(filename, buffer_limit=250):
     """Returns the function that returns generators."""
 
     def iter_json_file_logic():
@@ -51,30 +52,54 @@
 def iter_json_gzip_file(filename, buffer_limit=250):
     """Returns the function that returns generators."""
 
     def iter_json_gzip_file_logic():
         """Generator that reads and yields decoded JSON objects from a file."""
         json_processor = BufferedJSONProcessor(buffer_limit)
 
-        with gzip.open(filename, "r") as data:
-            while True:
-                try:
-                    v = data.readline().decode("utf-8", UNICODE_REPLACE_HANDLER)
-                    if not v:
-                        break
+        if buffer_limit != 0:
+            finished = False
+            with gzip.open(filename, "r") as data:
+                while True:
+                    try:
+                        for _ in range(buffer_limit):
+                            v = data.readline().decode("utf-8", UNICODE_REPLACE_HANDLER)
+                            if not v:
+                                finished = True
+                                break
+                            json_processor.buffer.append(v)
+
+                        yield from json_processor.from_buffer()
+
+                        if finished:
+                            break
+
+                    except ValueError:
+                        print(len(json_processor.buffer))
+                        print(f"Error string: {v}")
+                        raise
 
-                    yield from json_processor.decode(v)
-                except ValueError:
-                    print(len(json_processor.buffer))
-                    print(f"Error string: {v}")
-                    raise
-            yield from json_processor.fin()
+                yield from json_processor.fin()
+        else:
+            with gzip.open(filename, "r") as data:
+                while True:
+                    try:
+                        v = data.readline().decode("utf-8", UNICODE_REPLACE_HANDLER)
+                        if not v:
+                            break
+
+                        yield from json_processor.decode(v)
+
+                    except ValueError:
+                        print(len(json_processor.buffer))
+                        print(f"Error string: {v}")
+                        raise
 
     def iter_json_gzip_file_wrapper(*args, **kwargs):
-        """Wrapper function that allows passing arguments to the generator."""
+        """Wrapper function that allows to rerun generator one more time."""
         return iter_json_gzip_file_logic(*args, **kwargs)
 
     return iter_json_gzip_file_wrapper
 
 
 class BufferedJSONProcessor:
     def __init__(self, buffer_limit: int = 250):
@@ -103,41 +128,47 @@
             raise ValueError(
                 f"json.decoder.JSONDecodeError: Invalid json received.\n" f"{e}\n" f"{self.buffer}"
             )
         finally:
             # Prevents StopIteration issues
             self.buffer = []
 
-    def _decode_without_buffer(self, x: str) -> dict:
+    def _decode_without_buffer(self, x: str) -> Generator:
         """Decode JSON without buffer.
 
         Args:
             x: JSON Object
 
         Returns:
             dict
         """
         yield json.loads(x)
 
-    def _decode_with_buffer(self, x: str) -> dict:
+    def _decode_with_buffer(self, x: str) -> Generator:
         """Decode JSON with buffer.
 
         Args:
             x: JSON Object
 
         Returns:
             dict
         """
-        if len(self.buffer) < self.buffer_limit:
-            self.buffer.append(x)
-        else:
-            yield from self.from_buffer()
-            self.buffer = [x]
+        # for i in range(self.buffer_limit):
+
+        # # FIXME -- we check len every message. It can take a lot of time
+        # if len(self.buffer) < self.buffer_limit:
+        #     self.buffer.append(x)
+        # else:
+        #     yield from self.from_buffer()
+        #     self.buffer = [x]
+
+        yield from self.from_buffer()
+        self.buffer = [x]
 
     def fin(self) -> Generator:
-        """If buffer exists returns dicts from buffer.
+        """If buffer exists, returns dicts from buffer.
 
         Returns:
             Generator[dict]
         """
         if self.buffer:
             yield from self.from_buffer()
```

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/path_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-
+from typing import Union
 
 from th2_data_services.config import options
 from pathlib import Path
 import os
 
 
 def transform_filename_to_valid(filename: str) -> str:
@@ -63,15 +63,15 @@
     for sym in filename:
         if sym in chars:
             return False, f"Forbidden char: '{sym}', filename: '{filename}'"
 
     return True, ""
 
 
-def check_if_file_exists(filename):
+def check_if_file_exists(filename: Union[str, Path]):
     """Raises error if file doesn't exist.
 
     Args:
         filename: string.
 
     Raises:
         FileNotFoundError: if file doesn't exist.
@@ -81,11 +81,12 @@
         if not Path(filename).resolve().exists():
             raise FileNotFoundError(f"{filename} doesn't exist")
     except OSError as e:
         if os.name == "nt" and e.winerror == 123:
             illegal_characters = set([char for char in filename if char in r'\/:*?"<>|'])
             illegal_characters_str = ", ".join(illegal_characters)
             raise ValueError(
-                f"Invalid file path: {filename}. It contains illegal characters: {illegal_characters_str}"
+                f"Invalid file path: {filename}. "
+                f"It contains illegal characters: {illegal_characters_str}"
             )
         else:
             raise e
```

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev8662586819/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3833 3434 3831 3733 3239 0a53 756d 6d61  8344817329.Summa
+00000040: 3836 3632 3538 3638 3139 0a53 756d 6d61  8662586819.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
@@ -1679,479 +1679,573 @@
 000068e0: 696f 6e0a 2020 2020 2020 2020 6265 6869  ion.        behi
 000068f0: 6e64 2074 6865 2073 6365 6e65 7320 666f  nd the scenes fo
 00006900: 7220 796f 752e 204e 6f74 652c 2069 7420  r you. Note, it 
 00006910: 646f 6573 6e27 7420 6d65 616e 2079 6f75  doesn't mean you
 00006920: 2063 616e 6e6f 7420 6974 6572 6174 6520   cannot iterate 
 00006930: 7468 6520 5f44 6174 6120 6f62 6a65 6374  the _Data object
 00006940: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
-00006950: 2020 2020 2323 2320 4461 7461 2063 6163      ### Data cac
-00006960: 6869 6e67 0a20 2020 2020 2020 200a 2020  hing.        .  
-00006970: 2020 2020 2020 5468 6520 5f44 6174 6120        The _Data 
-00006980: 6f62 6a65 6374 5f20 7072 6f76 6964 6573  object_ provides
-00006990: 2074 6865 2061 6269 6c69 7479 2074 6f20   the ability to 
-000069a0: 7573 6520 7468 6520 6361 6368 652e 2054  use the cache. T
-000069b0: 6865 2063 6163 6865 2077 6f72 6b73 2066  he cache works f
-000069c0: 6f72 2065 6163 6820 5f44 6174 6120 6f62  or each _Data ob
-000069d0: 6a65 6374 5f2c 2074 6861 7420 6973 2c20  ject_, that is, 
-000069e0: 796f 7520 6368 6f6f 7365 0a20 2020 2020  you choose.     
-000069f0: 2020 2077 6869 6368 205f 4461 7461 206f     which _Data o
-00006a00: 626a 6563 745f 2079 6f75 2077 616e 7420  bject_ you want 
-00006a10: 746f 2073 6176 652e 2054 6865 205f 4461  to save. The _Da
-00006a20: 7461 206f 626a 6563 745f 2063 6163 6865  ta object_ cache
-00006a30: 2069 7320 7361 7665 6420 6166 7465 7220   is saved after 
-00006a40: 7468 6520 6669 7273 7420 6974 6572 6174  the first iterat
-00006a50: 696f 6e2c 2062 7574 2074 6865 2069 7465  ion, but the ite
-00006a60: 7261 7469 6f6e 0a20 2020 2020 2020 2073  ration.        s
-00006a70: 6f75 7263 6520 6d61 7920 6265 2064 6966  ource may be dif
-00006a80: 6665 7265 6e74 2e0a 2020 2020 2020 2020  ferent..        
-00006a90: 0a20 2020 2020 2020 2049 6620 796f 7520  .        If you 
-00006aa0: 646f 6e27 7420 7573 6520 7468 6520 6361  don't use the ca
-00006ab0: 6368 652c 2079 6f75 7220 736f 7572 6365  che, your source
-00006ac0: 2077 696c 6c20 6265 2074 6865 2064 6174   will be the dat
-00006ad0: 6120 736f 7572 6365 2079 6f75 2068 6176  a source you hav
-00006ae0: 6520 696e 2074 6865 205f 4461 7461 204f  e in the _Data O
-00006af0: 626a 6563 745f 2e20 4275 7420 6966 2079  bject_. But if y
-00006b00: 6f75 2075 7365 2074 6865 2063 6163 6865  ou use the cache
-00006b10: 2c0a 2020 2020 2020 2020 796f 7572 2073  ,.        your s
-00006b20: 6f75 7263 6520 6361 6e20 6265 2074 6865  ource can be the
-00006b30: 2064 6174 6120 736f 7572 6365 2c20 7468   data source, th
-00006b40: 6520 7061 7265 6e74 2063 6163 6865 2c20  e parent cache, 
-00006b50: 6f72 206f 776e 2063 6163 6865 3a0a 2020  or own cache:.  
-00006b60: 2020 2020 2020 0a20 2020 2020 2020 202a        .        *
-00006b70: 2054 6865 2064 6174 6120 736f 7572 6365   The data source
-00006b80: 3a0a 2020 2020 2020 2020 2020 4966 2074  :.          If t
-00006b90: 6865 205f 4461 7461 204f 626a 6563 745f  he _Data Object_
-00006ba0: 2064 6f65 736e 2774 2068 6176 6520 6120   doesn't have a 
-00006bb0: 7061 7265 6e74 2063 6163 6865 2061 6e64  parent cache and
-00006bc0: 2069 7473 2063 6163 6865 2e0a 2020 2020   its cache..    
-00006bd0: 2020 2020 2a20 5468 6520 7061 7265 6e74      * The parent
-00006be0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
-00006bf0: 2020 4966 2074 6865 205f 4461 7461 204f    If the _Data O
-00006c00: 626a 6563 745f 2068 6173 2061 2070 6172  bject_ has a par
-00006c10: 656e 7420 6361 6368 652e 2049 7420 646f  ent cache. It do
-00006c20: 6573 6e27 7420 6d61 7474 6572 2077 6861  esn't matter wha
-00006c30: 7420 706f 7369 7469 6f6e 2074 6865 2070  t position the p
-00006c40: 6172 656e 7420 6361 6368 6520 6861 7320  arent cache has 
-00006c50: 696e 2069 6e68 6572 6974 616e 6365 2e0a  in inheritance..
-00006c60: 2020 2020 2020 2020 2020 5f44 6174 6120            _Data 
-00006c70: 4f62 6a65 6374 5f20 756e 6465 7273 7461  Object_ understa
-00006c80: 6e64 7320 7768 6f73 6520 6361 6368 6520  nds whose cache 
-00006c90: 6974 2069 7320 616e 6420 6578 6563 7574  it is and execut
-00006ca0: 6573 2074 6865 2070 6172 7420 6f66 2074  es the part of t
-00006cb0: 6865 2077 6f72 6b66 6c6f 7720 7468 6174  he workflow that
-00006cc0: 2077 6173 206e 6f74 2065 7865 6375 7465   was not execute
-00006cd0: 642e 0a20 2020 2020 2020 202a 2054 6865  d..        * The
-00006ce0: 206f 776e 2063 6163 6865 3a0a 2020 2020   own cache:.    
-00006cf0: 2020 2020 2020 4966 2069 7420 6973 206e        If it is n
-00006d00: 6f74 2074 6865 2066 6972 7374 2069 7465  ot the first ite
-00006d10: 7261 7469 6f6e 206f 6620 7468 6973 2044  ration of this D
-00006d20: 6174 6120 6f62 6a65 6374 2e0a 2020 2020  ata object..    
-00006d30: 2020 2020 0a20 2020 2020 2020 204e 6f74      .        Not
-00006d40: 6520 7468 6174 2074 6865 2063 6163 6865  e that the cache
-00006d50: 2073 7461 7465 206f 6620 7468 6520 4461   state of the Da
-00006d60: 7461 206f 626a 6563 7420 6973 206e 6f74  ta object is not
-00006d70: 2069 6e68 6572 6974 6564 2e0a 2020 2020   inherited..    
-00006d80: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
-00006d90: 2320 466f 7263 6564 2063 6163 6869 6e67  # Forced caching
-00006da0: 0a20 2020 2020 2020 2059 6f75 2063 616e  .        You can
-00006db0: 2074 656c 6c20 4453 2074 6f20 6361 6368   tell DS to cach
-00006dc0: 6520 6461 7461 2074 6f20 7370 6563 6966  e data to specif
-00006dd0: 6963 2063 6163 6865 2066 696c 652c 2077  ic cache file, w
-00006de0: 6869 6368 2077 6f6e 2774 2062 6520 6465  hich won't be de
-00006df0: 6c65 7465 6420 6166 7465 7220 7363 7269  leted after scri
-00006e00: 7074 2065 6e64 2e0a 2020 2020 2020 2020  pt end..        
-00006e10: 596f 7520 6361 6e20 7365 6520 6578 616d  You can see exam
-00006e20: 706c 6520 696e 2031 2e31 3220 7365 6374  ple in 1.12 sect
-00006e30: 696f 6e20 6f66 205b 6765 745f 7374 6172  ion of [get_star
-00006e40: 7465 645f 6578 616d 706c 655d 2865 7861  ted_example](exa
-00006e50: 6d70 6c65 732f 6765 745f 7374 6172 7465  mples/get_starte
-00006e60: 645f 6578 616d 706c 652e 7079 292e 0a20  d_example.py).. 
-00006e70: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00006e80: 0a20 2020 2020 2020 2023 2323 2045 7665  .        ### Eve
-00006e90: 6e74 5472 6565 2061 6e64 2063 6f6c 6c65  ntTree and colle
-00006ea0: 6374 696f 6e73 0a20 2020 2020 2020 200a  ctions.        .
-00006eb0: 2020 2020 2020 2020 2323 2323 2045 7665          #### Eve
-00006ec0: 6e74 5472 6565 0a20 2020 2020 2020 200a  ntTree.        .
-00006ed0: 2020 2020 2020 2020 6045 7665 6e74 5472          `EventTr
-00006ee0: 6565 6020 6973 2061 2074 7265 652d 6261  ee` is a tree-ba
-00006ef0: 7365 6420 6461 7461 2073 7472 7563 7475  sed data structu
-00006f00: 7265 206f 6620 6576 656e 7473 2e20 4974  re of events. It
-00006f10: 2061 6c6c 6f77 7320 796f 7520 6765 7420   allows you get 
-00006f20: 6368 696c 6472 656e 2061 6e64 2070 6172  children and par
-00006f30: 656e 7473 206f 6620 6576 656e 742c 0a20  ents of event,. 
-00006f40: 2020 2020 2020 2064 6973 706c 6179 2074         display t
-00006f50: 7265 652c 2067 6574 2066 756c 6c20 7061  ree, get full pa
-00006f60: 7468 2074 6f20 6576 656e 7420 6574 632e  th to event etc.
-00006f70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00006f80: 2020 4465 7461 696c 733a 0a20 2020 2020    Details:.     
-00006f90: 2020 200a 2020 2020 2020 2020 2a20 6045     .        * `E
-00006fa0: 7665 6e74 5472 6565 6020 636f 6e74 6169  ventTree` contai
-00006fb0: 6e73 2061 6c6c 2065 7665 6e74 7320 696e  ns all events in
-00006fc0: 206d 656d 6f72 792e 0a20 2020 2020 2020   memory..       
-00006fd0: 202a 2054 7265 6520 6861 7320 736f 6d65   * Tree has some
-00006fe0: 2069 6d70 6f72 7461 6e74 2074 6572 6d73   important terms
-00006ff0: 3a0a 2020 2020 2020 2020 2020 2020 312e  :.            1.
-00007000: 205f 416e 6365 7374 6f72 5f20 6973 2061   _Ancestor_ is a
-00007010: 6e79 2072 656c 6174 6976 6520 6f66 2074  ny relative of t
-00007020: 6865 2065 7665 6e74 2075 7020 7468 6520  he event up the 
-00007030: 7472 6565 2028 6772 616e 6470 6172 656e  tree (grandparen
-00007040: 742c 2070 6172 656e 7420 6574 632e 292e  t, parent etc.).
-00007050: 0a20 2020 2020 2020 2020 2020 2032 2e20  .            2. 
-00007060: 5f50 6172 656e 745f 2069 7320 6f6e 6c79  _Parent_ is only
-00007070: 2074 6865 2066 6972 7374 2072 656c 6174   the first relat
-00007080: 6976 6520 6f66 2074 6865 2065 7665 6e74  ive of the event
-00007090: 2075 7020 7468 6520 7472 6565 2e0a 2020   up the tree..  
-000070a0: 2020 2020 2020 2020 2020 332e 205f 4368            3. _Ch
-000070b0: 696c 645f 2069 7320 7468 6520 6669 7273  ild_ is the firs
-000070c0: 7420 7265 6c61 7469 7665 206f 6620 7468  t relative of th
-000070d0: 6520 6576 656e 7420 646f 776e 2074 6865  e event down the
-000070e0: 2074 7265 652e 0a20 2020 2020 2020 200a   tree..        .
-000070f0: 2020 2020 2020 2020 5461 6b65 2061 206c          Take a l
-00007100: 6f6f 6b20 6174 2074 6865 2066 6f6c 6c6f  ook at the follo
-00007110: 7769 6e67 2048 544d 4c20 7472 6565 2074  wing HTML tree t
-00007120: 6f20 756e 6465 7273 7461 6e64 2074 6865  o understand the
-00007130: 6d2e 0a20 2020 2020 2020 200a 2020 2020  m..        .    
-00007140: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00007150: 2020 2020 2020 203c 626f 6479 3e20 3c21         <body> <!
-00007160: 2d2d 2061 6e63 6573 746f 7220 2867 7261  -- ancestor (gra
-00007170: 6e64 7061 7265 6e74 292c 2062 7574 206e  ndparent), but n
-00007180: 6f74 2070 6172 656e 7420 2d2d 3e0a 2020  ot parent -->.  
-00007190: 2020 2020 2020 2020 2020 2020 2020 3c64                <d
-000071a0: 6976 3e20 3c21 2d2d 2070 6172 656e 7420  iv> <!-- parent 
-000071b0: 2620 616e 6365 7374 6f72 202d 2d3e 0a20  & ancestor -->. 
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 203c 703e 4865 6c6c 6f2c 2077 6f72     <p>Hello, wor
-000071e0: 6c64 213c 2f70 3e20 3c21 2d2d 2063 6869  ld!</p> <!-- chi
-000071f0: 6c64 202d 2d3e 0a20 2020 2020 2020 2020  ld -->.         
-00007200: 2020 2020 2020 2020 2020 203c 703e 476f             <p>Go
-00007210: 6f64 6279 6521 3c2f 703e 203c 212d 2d20  odbye!</p> <!-- 
-00007220: 7369 626c 696e 6720 2d2d 3e0a 2020 2020  sibling -->.    
-00007230: 2020 2020 2020 2020 2020 2020 3c2f 6469              </di
-00007240: 763e 0a20 2020 2020 2020 2020 2020 203c  v>.            <
-00007250: 2f62 6f64 793e 0a20 2020 2020 2020 2020  /body>.         
-00007260: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
-00007270: 2020 2020 2020 2023 2323 2320 436f 6c6c         #### Coll
-00007280: 6563 7469 6f6e 730a 2020 2020 2020 2020  ections.        
-00007290: 0a20 2020 2020 2020 202a 2a45 7665 6e74  .        **Event
-000072a0: 5472 6565 436f 6c6c 6563 7469 6f6e 2a2a  TreeCollection**
-000072b0: 2069 7320 6120 636f 6c6c 6563 7469 6f6e   is a collection
-000072c0: 206f 6620 4576 656e 7454 7265 6573 2e20   of EventTrees. 
-000072d0: 5468 6520 636f 6c6c 6563 7469 6f6e 2062  The collection b
-000072e0: 7569 6c64 7320 6120 6665 7720 5f45 7665  uilds a few _Eve
-000072f0: 6e74 5472 6565 5f20 6279 2070 6173 7365  ntTree_ by passe
-00007300: 6420 5f44 6174 610a 2020 2020 2020 2020  d _Data.        
-00007310: 6f62 6a65 6374 5f2e 2041 6c74 686f 7567  object_. Althoug
-00007320: 6820 796f 7520 6361 6e20 6368 616e 6765  h you can change
-00007330: 2074 6865 2074 7265 6520 6469 7265 6374   the tree direct
-00007340: 6c79 2c20 6974 2773 2062 6574 7465 7220  ly, it's better 
-00007350: 746f 2064 6f20 6974 2074 6872 6f75 6768  to do it through
-00007360: 2063 6f6c 6c65 6374 696f 6e73 2062 6563   collections bec
-00007370: 6175 7365 2074 6865 7920 6172 6520 6177  ause they are aw
-00007380: 6172 6520 6f66 0a20 2020 2020 2020 2060  are of.        `
-00007390: 6465 7461 6368 6564 5f65 7665 6e74 7360  detached_events`
-000073a0: 2061 6e64 2063 616e 2073 6f6c 7665 2073   and can solve s
-000073b0: 6f6d 6520 6576 656e 7473 2064 6570 656e  ome events depen
-000073c0: 6465 6e63 6965 732e 2054 6865 2063 6f6c  dencies. The col
-000073d0: 6c65 6374 696f 6e20 6861 7320 7369 6d69  lection has simi
-000073e0: 6c61 7220 6665 6174 7572 6573 206c 696b  lar features lik
-000073f0: 6520 6120 7369 6e67 6c65 205f 4576 656e  e a single _Even
-00007400: 7454 7265 655f 0a20 2020 2020 2020 2062  tTree_.        b
-00007410: 7574 2061 7070 6c79 696e 6720 7468 656d  ut applying them
-00007420: 2066 6f72 2061 6c6c 205f 4576 656e 7454   for all _EventT
-00007430: 7265 6573 5f2e 0a20 2020 2020 2020 200a  rees_..        .
-00007440: 2020 2020 2020 2020 2a2a 5061 7265 6e74          **Parent
-00007450: 4576 656e 7454 7265 6543 6f6c 6c65 6374  EventTreeCollect
-00007460: 696f 6e2a 2a20 6973 2061 2063 6f6c 6c65  ion** is a colle
-00007470: 6374 696f 6e20 7369 6d69 6c61 7220 746f  ction similar to
-00007480: 205f 4576 656e 7454 7265 6543 6f6c 6c65   _EventTreeColle
-00007490: 6374 696f 6e5f 2062 7574 2063 6f6e 7461  ction_ but conta
-000074a0: 696e 696e 6720 6f6e 6c79 2070 6172 656e  ining only paren
-000074b0: 7420 6576 656e 7473 2074 6861 740a 2020  t events that.  
-000074c0: 2020 2020 2020 6172 6520 7265 6665 7265        are refere
-000074d0: 6e63 6564 2069 6e20 7468 6520 6461 7461  nced in the data
-000074e0: 2073 7472 6561 6d2e 2054 6865 2063 6f6c   stream. The col
-000074f0: 6c65 6374 696f 6e20 6861 7320 6665 6174  lection has feat
-00007500: 7572 6573 2073 696d 696c 6172 2074 6f20  ures similar to 
-00007510: 5f45 7665 6e74 5472 6565 436f 6c6c 6563  _EventTreeCollec
-00007520: 7469 6f6e 5f2e 0a20 2020 2020 2020 200a  tion_..        .
-00007530: 2020 2020 2020 2020 4465 7461 696c 733a          Details:
-00007540: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007550: 2020 2a20 546f 2075 7365 2045 5420 636f    * To use ET co
-00007560: 6c6c 6563 7469 6f6e 7320 796f 7520 6e65  llections you ne
-00007570: 6564 2074 6f20 696e 6974 6961 6c69 7a65  ed to initialize
-00007580: 2074 6865 6d20 6279 205f 4554 4344 7269   them by _ETCDri
-00007590: 7665 725f 2e20 4461 7461 2073 6f75 7263  ver_. Data sourc
-000075a0: 6573 2075 7375 616c 6c79 2070 726f 7669  es usually provi
-000075b0: 6465 2074 6865 6d2e 0a20 2020 2020 2020  de them..       
-000075c0: 2020 2059 6f75 2063 616e 2063 7265 6174     You can creat
-000075d0: 6520 6974 2062 7920 796f 7572 7365 6c66  e it by yourself
-000075e0: 2064 6570 656e 6469 6e67 206f 6e20 796f   depending on yo
-000075f0: 7572 2064 6174 6120 7374 7275 6374 7572  ur data structur
-00007600: 652e 0a20 2020 2020 2020 202a 2054 6865  e..        * The
-00007610: 2063 6f6c 6c65 6374 696f 6e20 6861 7320   collection has 
-00007620: 6120 6665 6174 7572 6520 746f 2072 6563  a feature to rec
-00007630: 6f76 6572 2065 7665 6e74 732e 2041 6c6c  over events. All
-00007640: 2065 7665 6e74 7320 7468 6174 2061 7265   events that are
-00007650: 206e 6f74 2069 6e20 7468 6520 7265 6365   not in the rece
-00007660: 6976 6564 2064 6174 6120 7374 7265 616d  ived data stream
-00007670: 2c20 6275 7420 7768 6963 6820 6172 650a  , but which are.
-00007680: 2020 2020 2020 2020 2020 7265 6665 7265            refere
-00007690: 6e63 6564 2077 696c 6c20 6265 206c 6f61  nced will be loa
-000076a0: 6465 6420 6672 6f6d 2074 6865 2064 6174  ded from the dat
-000076b0: 6120 736f 7572 6365 2e0a 2020 2020 2020  a source..      
-000076c0: 2020 2a20 596f 7520 6361 6e20 7461 6b65    * You can take
-000076d0: 2060 6465 7461 6368 6564 5f65 7665 6e74   `detached_event
-000076e0: 7360 2074 6f20 7365 6520 7768 6963 6820  s` to see which 
-000076f0: 6576 656e 7473 2061 7265 206d 6973 7369  events are missi
-00007700: 6e67 2e0a 2020 2020 2020 2020 2a20 4966  ng..        * If
-00007710: 2079 6f75 2077 616e 742c 2079 6f75 2063   you want, you c
-00007720: 616e 2062 7569 6c64 2070 6172 656e 746c  an build parentl
-00007730: 6573 7320 7472 6565 7320 7768 6572 6520  ess trees where 
-00007740: 7468 6520 6d69 7373 696e 6720 6576 656e  the missing even
-00007750: 7473 2061 7265 2073 7475 6262 6564 2069  ts are stubbed i
-00007760: 6e73 7465 6164 2e20 4a75 7374 0a20 2020  nstead. Just.   
-00007770: 2020 2020 2020 2075 7365 2060 6765 745f         use `get_
-00007780: 7061 7265 6e74 6c65 7373 5f74 7265 6573  parentless_trees
-00007790: 2829 602e 0a20 2020 2020 2020 200a 2020  ()`..        .  
-000077a0: 2020 2020 2020 5265 7175 6972 656d 656e        Requiremen
-000077b0: 7473 3a0a 2020 2020 2020 2020 0a20 2020  ts:.        .   
-000077c0: 2020 2020 2031 2e20 4576 656e 7473 2070       1. Events p
-000077d0: 726f 7669 6465 6420 746f 2045 5443 2068  rovided to ETC h
-000077e0: 6176 6520 746f 2068 6176 6520 6065 7665  ave to have `eve
-000077f0: 6e74 5f6e 616d 6560 2c20 6065 7665 6e74  nt_name`, `event
-00007800: 5f69 6460 2c20 6070 6172 656e 745f 6576  _id`, `parent_ev
-00007810: 656e 745f 6964 6020 6669 656c 6473 2e20  ent_id` fields. 
-00007820: 5468 6579 0a20 2020 2020 2020 2063 616e  They.        can
-00007830: 2068 6176 6520 616e 6f74 6865 7220 6e61   have another na
-00007840: 6d65 7320 2869 7420 7265 736f 6c76 6573  mes (it resolves
-00007850: 2069 6e20 7468 6520 6472 6976 6572 292e   in the driver).
-00007860: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007870: 2020 2323 2323 2048 696e 7473 0a20 2020    #### Hints.   
-00007880: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
-00007890: 5265 6d6f 7665 2061 6c6c 2075 6e6e 6563  Remove all unnec
-000078a0: 6573 7361 7279 2066 6965 6c64 7320 6672  essary fields fr
-000078b0: 6f6d 2065 7665 6e74 7320 6265 666f 7265  om events before
-000078c0: 2070 6173 7369 6e67 2074 6f20 6120 5f63   passing to a _c
-000078d0: 6f6c 6c65 6374 696f 6e5f 2074 6f20 7265  ollection_ to re
-000078e0: 6475 6365 206d 656d 6f72 7920 7573 6167  duce memory usag
-000078f0: 652e 0a20 2020 2020 2020 202a 2055 7365  e..        * Use
-00007900: 2060 7368 6f77 2829 6020 6d65 7468 6f64   `show()` method
-00007910: 2074 6f20 7072 696e 7420 7468 6520 7472   to print the tr
-00007920: 6565 2069 6e20 7472 6565 2d6c 696b 6520  ee in tree-like 
-00007930: 7669 6577 2e0a 2020 2020 2020 2020 2a20  view..        * 
-00007940: 4e6f 7465 2074 6861 7420 7468 6520 6067  Note that the `g
-00007950: 6574 5f78 6020 6d65 7468 6f64 7320 7769  et_x` methods wi
-00007960: 6c6c 2072 6169 7365 2061 6e20 6578 6365  ll raise an exce
-00007970: 7074 696f 6e20 6966 2079 6f75 2070 6173  ption if you pas
-00007980: 7320 616e 2075 6e6b 6e6f 776e 2065 7665  s an unknown eve
-00007990: 6e74 2069 642c 2075 6e6c 696b 6520 7468  nt id, unlike th
-000079a0: 6520 6066 696e 645f 7860 206d 6574 686f  e `find_x` metho
-000079b0: 6473 2028 0a20 2020 2020 2020 2020 2074  ds (.          t
-000079c0: 6865 7920 7265 7475 726e 204e 6f6e 6529  hey return None)
-000079d0: 2e0a 2020 2020 2020 2020 2a20 4966 2079  ..        * If y
-000079e0: 6f75 2077 616e 7420 746f 206b 6e6f 7720  ou want to know 
-000079f0: 7468 6174 2073 7065 6369 6669 6564 2065  that specified e
-00007a00: 7665 6e74 2065 7869 7374 732c 2075 7365  vent exists, use
-00007a10: 2074 6865 2070 7974 686f 6e20 6069 6e60   the python `in`
-00007a20: 206b 6579 776f 7264 2028 652e 672e 2060   keyword (e.g. `
-00007a30: 2765 7665 6e74 2d69 6427 2069 6e20 6576  'event-id' in ev
-00007a40: 656e 7473 5f74 7265 6560 292e 0a20 2020  ents_tree`)..   
-00007a50: 2020 2020 202a 2055 7365 2074 6865 2070       * Use the p
-00007a60: 7974 686f 6e20 606c 656e 6020 6b65 7977  ython `len` keyw
-00007a70: 6f72 6420 746f 2067 6574 2065 7665 6e74  ord to get event
-00007a80: 7320 6e75 6d62 6572 2069 6e20 7468 6520  s number in the 
-00007a90: 7472 6565 2e0a 2020 2020 2020 2020 0a20  tree..        . 
-00007aa0: 2020 2020 2020 2023 2323 2046 6965 6c64         ### Field
-00007ab0: 2052 6573 6f6c 7665 7273 0a20 2020 2020   Resolvers.     
-00007ac0: 2020 2049 6e74 6572 6661 6365 2063 616e     Interface can
-00007ad0: 2062 6520 666f 756e 6420 696e 2060 7468   be found in `th
-00007ae0: 325f 6461 7461 5f73 6572 7669 6365 732f  2_data_services/
-00007af0: 696e 7465 7266 6163 6573 2f75 7469 6c73  interfaces/utils
-00007b00: 2f72 6573 6f6c 7665 722e 7079 602e 2020  /resolver.py`.  
-00007b10: 0a20 2020 2020 2020 2041 6c6c 2064 6174  .        All dat
-00007b20: 612d 736f 7572 6365 7320 7368 6f75 6c64  a-sources should
-00007b30: 2069 6d70 6c65 6d65 6e74 2074 6865 6d2e   implement them.
-00007b40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00007b50: 2020 5468 6520 6964 6561 206f 6620 7573    The idea of us
-00007b60: 696e 6720 7265 736f 6c76 6572 733a 0a20  ing resolvers:. 
-00007b70: 2020 2020 2020 2049 7420 736f 6c76 6573         It solves
-00007b80: 2074 6865 2070 726f 626c 656d 206f 6620   the problem of 
-00007b90: 6861 7669 6e67 2061 2066 6577 2044 6174  having a few Dat
-00007ba0: 6153 6f75 7263 6573 2077 6974 6820 7369  aSources with si
-00007bb0: 6d69 6c61 7220 6461 7461 2c0a 2020 2020  milar data,.    
-00007bc0: 2020 2020 6275 7420 7769 7468 2064 6966      but with dif
-00007bd0: 6665 7265 6e74 2077 6179 7320 746f 2067  ferent ways to g
-00007be0: 6574 2069 742e 0a20 2020 2020 2020 200a  et it..        .
-00007bf0: 2020 2020 2020 2020 5468 6573 6520 636c          These cl
-00007c00: 6173 7365 7320 7072 6f76 6964 6520 796f  asses provide yo
-00007c10: 7520 6765 7474 6572 206d 6574 686f 6473  u getter methods
-00007c20: 2e0a 2020 2020 2020 2020 5573 696e 6720  ..        Using 
-00007c30: 7468 6573 6520 636c 6173 7365 7320 616c  these classes al
-00007c40: 6c6f 7773 2079 6f75 2074 6f20 6672 6565  lows you to free
-00007c50: 6c79 2073 7769 7463 6820 6265 7477 6565  ly switch betwee
-00007c60: 6e20 6469 6666 6572 656e 7420 6461 7461  n different data
-00007c70: 0a20 2020 2020 2020 2066 6f72 6d61 7473  .        formats
-00007c80: 2061 6e64 2064 6f6e 2774 2063 6861 6e67   and don't chang
-00007c90: 6520 796f 7572 2063 6f64 652e 0a20 2020  e your code..   
-00007ca0: 2020 2020 200a 2020 2020 2020 2020 5265       .        Re
-00007cb0: 736f 6c76 6572 7320 736f 6c76 6520 7468  solvers solve th
-00007cc0: 6520 7072 6f62 6c65 6d20 6f66 2064 6174  e problem of dat
-00007cd0: 612d 666f 726d 6174 206d 6967 7261 7469  a-format migrati
-00007ce0: 6f6e 2e0a 2020 2020 2020 2020 2d20 6669  on..        - fi
-00007cf0: 656c 6473 2070 6c61 6365 2063 616e 2062  elds place can b
-00007d00: 6520 6368 616e 6765 640a 2020 2020 2020  e changed.      
-00007d10: 2020 2d20 6669 656c 6473 206e 616d 6573    - fields names
-00007d20: 2063 616e 2062 6520 6368 616e 6765 640a   can be changed.
-00007d30: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00007d40: 2052 6573 6f6c 7665 7273 2063 616e 2077   Resolvers can w
-00007d50: 6f72 6b20 6f6e 6c79 2077 6974 6820 6f6e  ork only with on
-00007d60: 6520 6576 656e 742f 6d65 7373 6167 652e  e event/message.
-00007d70: 0a20 2020 2020 2020 2049 7420 6d65 616e  .        It mean
-00007d80: 732c 2069 6620 796f 7572 206d 6573 7361  s, if your messa
-00007d90: 6765 2068 6173 2073 7562 2d6d 6573 7361  ge has sub-messa
-00007da0: 6765 7320 286c 696b 6520 7468 322d 6d65  ges (like th2-me
-00007db0: 7373 6167 6573 2069 6e20 6c77 6470 2920  ssages in lwdp) 
-00007dc0: 6974 200a 2020 2020 2020 2020 776f 6e27  it .        won'
-00007dd0: 7420 776f 726b 2c20 6265 6361 7573 6520  t work, because 
-00007de0: 7265 736f 6c76 6572 2077 696c 6c20 6e6f  resolver will no
-00007df0: 7420 6b6e 6f77 2077 6974 6820 7768 6963  t know with whic
-00007e00: 6820 7375 622d 6d65 7373 6167 6520 7368  h sub-message sh
-00007e10: 6f75 6c64 2069 7420 776f 726b 2e20 0a20  ould it work. . 
-00007e20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00007e30: 2a2a 576f 726b 6172 6f75 6e64 2a2a 2020  **Workaround**  
-00007e40: 0a20 2020 2020 2020 2031 2e20 4578 7061  .        1. Expa
-00007e50: 6e64 2061 6c6c 2079 6f75 7220 6d65 7373  nd all your mess
-00007e60: 6167 6573 202d 3e20 606e 6577 5f64 203d  ages -> `new_d =
-00007e70: 2079 6f75 725f 6461 7461 2e6d 6170 284d   your_data.map(M
-00007e80: 6573 7361 6765 4669 656c 6452 6573 6f6c  essageFieldResol
-00007e90: 7665 722e 6578 7061 6e64 5f6d 6573 7361  ver.expand_messa
-00007ea0: 6765 2960 0a20 2020 2020 2020 2032 2e20  ge)`.        2. 
-00007eb0: 5573 6520 6045 7870 616e 6465 644d 6573  Use `ExpandedMes
-00007ec0: 7361 6765 4669 656c 6452 6573 6f6c 7665  sageFieldResolve
-00007ed0: 7260 2069 6e73 7465 6164 206f 6620 7573  r` instead of us
-00007ee0: 7561 6c20 604d 6573 7361 6765 4669 656c  ual `MessageFiel
-00007ef0: 6452 6573 6f6c 7665 7260 2077 6865 6e20  dResolver` when 
-00007f00: 0a20 2020 2020 2020 2020 2020 2079 6f75  .            you
-00007f10: 2074 616b 6520 6669 656c 6473 2066 6f72   take fields for
-00007f20: 2065 7870 616e 6465 6420 6d65 7373 6167   expanded messag
-00007f30: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00007f40: 2020 2020 202a 2a49 6d70 6c65 6d65 6e74       **Implement
-00007f50: 6174 696f 6e20 6164 7669 6365 3a2a 2a0a  ation advice:**.
-00007f60: 2020 2020 2020 2020 312e 2072 6169 7365          1. raise
-00007f70: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00007f80: 7272 6f72 202d 2d20 6966 2079 6f75 7220  rror -- if your 
-00007f90: 496d 706c 656d 656e 7461 7469 6f6e 2064  Implementation d
-00007fa0: 6f65 736e 2774 2073 7570 706f 7274 2074  oesn't support t
-00007fb0: 6869 7320 6765 7474 6572 2e0a 2020 2020  his getter..    
-00007fc0: 2020 2020 0a20 2020 2020 2020 202a 2a50      .        **P
-00007fd0: 6572 666f 726d 616e 6365 2069 6d70 6163  erformance impac
-00007fe0: 743a 2a2a 0a20 2020 2020 2020 202d 2049  t:**.        - I
-00007ff0: 7420 6120 6269 7420 736c 6f77 6572 2074  t a bit slower t
-00008000: 6861 6e20 7573 696e 6720 6e61 6b65 6420  han using naked 
-00008010: 6669 656c 6420 6163 6365 7373 2060 6469  field access `di
-00008020: 6374 5b27 6b65 7927 5d60 2e0a 2020 2020  ct['key']`..    
-00008030: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-00008040: 322e 342e 204c 696e 6b73 0a20 2020 2020  2.4. Links.     
-00008050: 2020 200a 2020 2020 2020 2020 2d20 5b52     .        - [R
-00008060: 6570 6f72 7420 4461 7461 2050 726f 7669  eport Data Provi
-00008070: 6465 725d 2868 7474 7073 3a2f 2f67 6974  der](https://git
-00008080: 6875 622e 636f 6d2f 7468 322d 6e65 742f  hub.com/th2-net/
-00008090: 7468 322d 7270 742d 6461 7461 2d70 726f  th2-rpt-data-pro
-000080a0: 7669 6465 7229 0a20 2020 2020 2020 202d  vider).        -
-000080b0: 205b 5468 3220 4461 7461 2053 6572 7669   [Th2 Data Servi
-000080c0: 6365 7320 5574 696c 735d 2868 7474 7073  ces Utils](https
-000080d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7468  ://github.com/th
-000080e0: 322d 6e65 742f 7468 322d 6461 7461 2d73  2-net/th2-data-s
-000080f0: 6572 7669 6365 732d 7574 696c 7329 0a20  ervices-utils). 
-00008100: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00008110: 2320 332e 2042 6573 7420 7072 6163 7469  # 3. Best practi
-00008120: 6365 730a 2020 2020 2020 2020 4465 7065  ces.        Depe
-00008130: 6e64 696e 6720 6f6e 2068 6f77 2079 6f75  nding on how you
-00008140: 2077 6f72 6b20 7769 7468 2060 4461 7461   work with `Data
-00008150: 206f 626a 6563 7460 2c20 6974 2063 616e   object`, it can
-00008160: 2062 6520 736c 6f77 206f 6620 6661 7374   be slow of fast
-00008170: 2e0a 2020 2020 2020 2020 4173 2077 6974  ..        As wit
-00008180: 6820 6120 7265 6c61 7469 6f6e 616c 2064  h a relational d
-00008190: 6174 6162 6173 652c 2079 6f75 2063 616e  atabase, you can
-000081a0: 2077 7269 7465 2061 2071 7565 7279 2074   write a query t
-000081b0: 6861 7420 7769 6c6c 2072 6574 7572 6e20  hat will return 
-000081c0: 6461 7461 2073 6c6f 776c 7920 6f72 2071  data slowly or q
-000081d0: 7569 636b 6c79 2c0a 2020 2020 2020 2020  uickly,.        
-000081e0: 7468 6520 7361 6d65 2077 6865 6e20 776f  the same when wo
-000081f0: 726b 696e 6720 7769 7468 2061 2060 4461  rking with a `Da
-00008200: 7461 206f 626a 6563 7460 2e0a 2020 2020  ta object`..    
-00008210: 2020 2020 0a20 2020 2020 2020 2046 6f6c      .        Fol
-00008220: 6c6f 7720 7468 6520 7275 6c65 7320 746f  low the rules to
-00008230: 206d 616b 6520 796f 7572 2077 6f72 6b20   make your work 
-00008240: 7769 7468 2044 6174 6120 6f62 6a65 6374  with Data object
-00008250: 2066 6173 743a 0a20 2020 2020 2020 2031   fast:.        1
-00008260: 2e20 5573 6520 6044 6174 612e 7573 655f  . Use `Data.use_
-00008270: 6361 6368 6528 2960 2069 6620 796f 7520  cache()` if you 
-00008280: 6974 6572 6174 6520 6461 7461 206d 6f72  iterate data mor
-00008290: 6520 7468 616e 206f 6e65 2074 696d 652e  e than one time.
-000082a0: 0a20 2020 2020 2020 2032 2e20 5472 7920  .        2. Try 
-000082b0: 746f 2064 6f6e 2774 2069 7465 7261 7465  to don't iterate
-000082c0: 206f 6e65 2060 4461 7461 206f 626a 6563   one `Data objec
-000082d0: 7460 2069 6e73 6964 6520 7468 6520 6f74  t` inside the ot
-000082e0: 6865 7220 6f6e 652e 0a20 2020 2020 2020  her one..       
-000082f0: 2020 2020 4966 2079 6f75 2073 686f 756c      If you shoul
-00008300: 6420 746f 2064 6f20 6974 2c20 7573 6520  d to do it, use 
-00008310: 7368 6f72 7420 6044 6174 6120 6f62 6a65  short `Data obje
-00008320: 6374 6020 6669 7273 7420 616e 6420 6c6f  ct` first and lo
-00008330: 6e67 2060 4461 7461 206f 626a 6563 7460  ng `Data object`
-00008340: 2069 6e73 6964 6520 7468 6520 6c6f 6f70   inside the loop
-00008350: 2e0a 2020 2020 2020 2020 2020 2049 7427  ..           It'
-00008360: 6c6c 2061 6c6c 6f77 2079 6f75 206f 7065  ll allow you ope
-00008370: 6e20 7468 6520 6361 6368 6520 6669 6c65  n the cache file
-00008380: 206f 7220 6372 6561 7465 2061 2072 6571   or create a req
-00008390: 7565 7374 2074 6f20 6044 6174 6120 736f  uest to `Data so
-000083a0: 7572 6365 6020 6c65 7373 206e 756d 6265  urce` less numbe
-000083b0: 7220 6f66 2074 696d 6573 2e0a 2020 2020  r of times..    
-000083c0: 2020 2020 0a20 2020 2020 2020 2023 2034      .        # 4
-000083d0: 2e20 4f66 6669 6369 616c 2044 6174 6153  . Official DataS
-000083e0: 6f75 7263 6520 696d 706c 656d 656e 7461  ource implementa
-000083f0: 7469 6f6e 730a 2020 2020 2020 2020 0a20  tions.        . 
-00008400: 2020 2020 2020 202d 205b 4c69 6768 7477         - [Lightw
-00008410: 6569 6768 7420 4461 7461 2050 726f 7669  eight Data Provi
-00008420: 6465 7220 4461 7461 2053 6f75 7263 655d  der Data Source]
-00008430: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00008440: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
-00008450: 6473 2d73 6f75 7263 652d 6c77 6470 290a  ds-source-lwdp).
-00008460: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00008470: 200a 2020 2020 2020 2020 2320 352e 2041   .        # 5. A
-00008480: 5049 0a20 2020 2020 2020 200a 2020 2020  PI.        .    
-00008490: 2020 2020 4966 2079 6f75 2061 7265 206c      If you are l
-000084a0: 6f6f 6b69 6e67 2066 6f72 2063 6c61 7373  ooking for class
-000084b0: 6573 2064 6573 6372 6970 7469 6f6e 2073  es description s
-000084c0: 6565 2074 6865 205b 4150 4920 446f 6375  ee the [API Docu
-000084d0: 6d65 6e74 6174 696f 6e5d 2864 6f63 756d  mentation](docum
-000084e0: 656e 7461 7469 6f6e 2f61 7069 2f69 6e64  entation/api/ind
-000084f0: 6578 2e6d 6429 2e0a 2020 2020 2020 2020  ex.md)..        
-00008500: 0a20 2020 2020 2020 2023 2036 2e20 4578  .        # 6. Ex
-00008510: 616d 706c 6573 0a20 2020 2020 2020 200a  amples.        .
-00008520: 2020 2020 2020 2020 2d20 5b67 6574 5f73          - [get_s
-00008530: 7461 7274 6564 5f65 7861 6d70 6c65 2e70  tarted_example.p
-00008540: 795d 2865 7861 6d70 6c65 732f 6765 745f  y](examples/get_
-00008550: 7374 6172 7465 645f 6578 616d 706c 652e  started_example.
-00008560: 7079 290a 2020 2020 2020 2020 0a50 6c61  py).        .Pla
-00008570: 7466 6f72 6d3a 2055 4e4b 4e4f 574e 0a52  tform: UNKNOWN.R
-00008580: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
-00008590: 3e3d 332e 370a 4465 7363 7269 7074 696f  >=3.7.Descriptio
-000085a0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-000085b0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-000085c0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
-000085d0: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
-000085e0: 3a20 7264 7035 0a50 726f 7669 6465 732d  : rdp5.Provides-
-000085f0: 4578 7472 613a 2072 6470 360a 5072 6f76  Extra: rdp6.Prov
-00008600: 6964 6573 2d45 7874 7261 3a20 6c77 6470  ides-Extra: lwdp
-00008610: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00008620: 206c 7764 7031 0a50 726f 7669 6465 732d   lwdp1.Provides-
-00008630: 4578 7472 613a 206c 7764 7032 0a50 726f  Extra: lwdp2.Pro
-00008640: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
-00008650: 7033 0a50 726f 7669 6465 732d 4578 7472  p3.Provides-Extr
-00008660: 613a 206c 7764 702d 6465 760a 5072 6f76  a: lwdp-dev.Prov
-00008670: 6964 6573 2d45 7874 7261 3a20 7574 696c  ides-Extra: util
-00008680: 732d 7270 742d 7669 6577 6572 0a50 726f  s-rpt-viewer.Pro
-00008690: 7669 6465 732d 4578 7472 613a 2075 7469  vides-Extra: uti
-000086a0: 6c73 2d72 7074 2d76 6965 7765 7235 0a50  ls-rpt-viewer5.P
-000086b0: 726f 7669 6465 732d 4578 7472 613a 2075  rovides-Extra: u
-000086c0: 7469 6c73 2d61 6476 616e 6365 640a       tils-advanced.
+00006950: 2020 2020 0a20 2020 2020 2020 2023 2323      .        ###
+00006960: 2044 6174 6120 6974 6572 6174 696f 6e0a   Data iteration.
+00006970: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00006980: 2054 6865 2044 6174 6120 6f62 6a65 6374   The Data object
+00006990: 2063 6f6e 7374 7275 6374 6f72 206d 6574   constructor met
+000069a0: 686f 6420 7461 6b65 7320 696e 2061 7320  hod takes in as 
+000069b0: 6172 6775 6d65 6e74 2065 6974 6865 7220  argument either 
+000069c0: 616e 2069 7465 7261 746f 7220 6f76 6572  an iterator over
+000069d0: 206f 626a 6563 7473 206f 7220 6120 6765   objects or a ge
+000069e0: 6e65 7261 746f 7220 6675 6e63 7469 6f6e  nerator function
+000069f0: 2e0a 2020 2020 2020 2020 5468 6520 4461  ..        The Da
+00006a00: 7461 206f 626a 6563 7420 6974 6572 6174  ta object iterat
+00006a10: 6f72 2068 616e 646c 6573 2065 6163 6820  or handles each 
+00006a20: 6974 656d 2069 6e20 7468 6973 2069 7465  item in this ite
+00006a30: 7261 746f 7220 6f72 2067 656e 6572 6174  rator or generat
+00006a40: 6f72 2061 7320 7468 6579 2061 7265 2c20  or as they are, 
+00006a50: 6d65 616e 696e 6720 6974 2064 6f65 736e  meaning it doesn
+00006a60: 2774 2074 7279 2074 6f20 7265 6164 2074  't try to read t
+00006a70: 6865 2063 6f6e 7465 6e74 206f 6620 6974  he content of it
+00006a80: 656d 206f 7220 7265 7475 726e 2074 6865  em or return the
+00006a90: 6d20 6d6f 6469 6669 6564 2069 6e20 616e  m modified in an
+00006aa0: 7920 7761 792c 2069 6e73 7465 6164 2072  y way, instead r
+00006ab0: 6574 7572 6e73 2074 6865 2069 7465 6d20  eturns the item 
+00006ac0: 6974 7365 6c66 2e0a 2020 2020 2020 2020  itself..        
+00006ad0: 5468 6520 6f6e 6c79 2065 7863 6570 7469  The only excepti
+00006ae0: 6f6e 2074 6f20 7468 6973 2069 7320 7768  on to this is wh
+00006af0: 656e 2044 6174 6120 6f62 6a65 6374 2069  en Data object i
+00006b00: 7320 6275 696c 7420 7573 696e 6720 6974  s built using it
+00006b10: 6572 6174 6f72 206f 7220 6765 6e65 7261  erator or genera
+00006b20: 746f 7220 6f76 6572 206f 7468 6572 2044  tor over other D
+00006b30: 6174 6120 6f62 6a65 6374 732e 204e 6f74  ata objects. Not
+00006b40: 6520 7468 6174 2074 6869 7320 6974 6572  e that this iter
+00006b50: 6174 6f72 206f 7220 6765 6e65 7261 746f  ator or generato
+00006b60: 7220 6d75 7374 206f 6e6c 7920 6265 2079  r must only be y
+00006b70: 6965 6c64 696e 6720 4461 7461 206f 626a  ielding Data obj
+00006b80: 6563 7473 2061 6e64 206e 6f74 6869 6e67  ects and nothing
+00006b90: 2065 6c73 652e 2049 6620 7765 2062 7569   else. If we bui
+00006ba0: 6c64 2066 726f 6d20 6120 6d69 7820 6f66  ld from a mix of
+00006bb0: 2044 6174 6120 6f62 6a65 6374 7320 616e   Data objects an
+00006bc0: 6420 736f 6d65 206f 7468 6572 2074 7970  d some other typ
+00006bd0: 6573 2c20 4461 7461 206f 626a 6563 7473  es, Data objects
+00006be0: 2720 636f 6e74 656e 7420 776f 6e27 7420  ' content won't 
+00006bf0: 6265 2072 6561 6420 616e 6420 696e 7374  be read and inst
+00006c00: 6561 6420 6974 2077 696c 6c20 6265 2072  ead it will be r
+00006c10: 6574 7572 6e65 6420 6173 2044 6174 6120  eturned as Data 
+00006c20: 6f62 6a65 6374 2069 7473 656c 662e 0a20  object itself.. 
+00006c30: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006c40: 536d 616c 6c20 6578 616d 706c 6520 746f  Small example to
+00006c50: 2064 656d 6f6e 7374 7261 7465 3a0a 2020   demonstrate:.  
+00006c60: 2020 2020 2020 0a20 2020 2020 2020 2060        .        `
+00006c70: 6060 7079 7468 6f6e 0a20 2020 2020 2020  ``python.       
+00006c80: 2066 726f 6d20 7468 325f 6461 7461 5f73   from th2_data_s
+00006c90: 6572 7669 6365 732e 6461 7461 2069 6d70  ervices.data imp
+00006ca0: 6f72 7420 4461 7461 0a20 2020 2020 2020  ort Data.       
+00006cb0: 200a 2020 2020 2020 2020 6431 203d 2044   .        d1 = D
+00006cc0: 6174 6128 5b31 2c32 2c33 5d29 0a20 2020  ata([1,2,3]).   
+00006cd0: 2020 2020 2064 3220 3d20 4461 7461 285b       d2 = Data([
+00006ce0: 342c 352c 365d 290a 2020 2020 2020 2020  4,5,6]).        
+00006cf0: 0a20 2020 2020 2020 206f 6e6c 795f 6461  .        only_da
+00006d00: 7461 5f6f 626a 6563 7473 203d 2044 6174  ta_objects = Dat
+00006d10: 6128 5b64 312c 6432 5d29 2023 2057 696c  a([d1,d2]) # Wil
+00006d20: 6c20 6974 6572 6174 6520 6173 2031 2c32  l iterate as 1,2
+00006d30: 2c33 2c34 2c35 2c36 0a20 2020 2020 2020  ,3,4,5,6.       
+00006d40: 2064 6174 615f 616e 645f 6c69 7374 203d   data_and_list =
+00006d50: 2044 6174 6128 5b64 312c 5b34 2c35 2c36   Data([d1,[4,5,6
+00006d60: 5d5d 2920 2320 5769 6c6c 2069 7465 7261  ]]) # Will itera
+00006d70: 7465 2061 7320 6431 2c20 5b34 2c35 2c36  te as d1, [4,5,6
+00006d80: 5d0a 2020 2020 2020 2020 6461 7461 5f61  ].        data_a
+00006d90: 6e64 5f6e 756d 6265 7273 203d 2044 6174  nd_numbers = Dat
+00006da0: 6128 5b64 312c 342c 352c 365d 2920 2320  a([d1,4,5,6]) # 
+00006db0: 5769 6c6c 2069 7465 7261 7465 2061 7320  Will iterate as 
+00006dc0: 6431 2c34 2c35 2c36 0a20 2020 2020 2020  d1,4,5,6.       
+00006dd0: 206c 6973 7473 5f6f 6e6c 7920 3d20 4461   lists_only = Da
+00006de0: 7461 285b 312c 322c 335d 2c5b 342c 352c  ta([1,2,3],[4,5,
+00006df0: 365d 2920 2320 5769 6c6c 2069 7465 7261  6]) # Will itera
+00006e00: 7465 2061 7320 5b31 2c32 2c33 5d2c 5b34  te as [1,2,3],[4
+00006e10: 2c35 2c36 5d0a 2020 2020 2020 2020 0a20  ,5,6].        . 
+00006e20: 2020 2020 2020 2023 2049 6620 7765 2077         # If we w
+00006e30: 616e 7420 746f 2069 7465 7261 7465 206f  ant to iterate o
+00006e40: 7665 7220 636f 6e74 656e 7420 6f66 206c  ver content of l
+00006e50: 6973 7420 6f66 206c 6973 7473 2c20 7765  ist of lists, we
+00006e60: 2073 686f 756c 6420 6669 7273 7420 6372   should first cr
+00006e70: 6561 7465 2044 6174 6120 6f62 6a65 6374  eate Data object
+00006e80: 7320 6672 6f6d 2074 6865 6d2c 0a20 2020  s from them,.   
+00006e90: 2020 2020 2023 2074 6865 6e20 7573 6520       # then use 
+00006ea0: 7468 656d 2074 6f20 636f 6e73 7472 7563  them to construc
+00006eb0: 7420 6e65 7720 4461 7461 206f 626a 6563  t new Data objec
+00006ec0: 7420 6173 2069 6e20 6361 7365 206f 6620  t as in case of 
+00006ed0: 6431 2061 6e64 2064 322c 2063 7265 6174  d1 and d2, creat
+00006ee0: 696e 6720 276f 6e6c 795f 6461 7461 5f6f  ing 'only_data_o
+00006ef0: 626a 6563 7473 2720 696e 2074 6869 7320  bjects' in this 
+00006f00: 6578 616d 706c 652e 0a20 2020 2020 2020  example..       
+00006f10: 2060 6060 0a20 2020 2020 2020 2020 0a20   ```.         . 
+00006f20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00006f30: 2323 2320 4461 7461 2063 6163 6869 6e67  ### Data caching
+00006f40: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00006f50: 2020 5468 6520 5f44 6174 6120 6f62 6a65    The _Data obje
+00006f60: 6374 5f20 7072 6f76 6964 6573 2074 6865  ct_ provides the
+00006f70: 2061 6269 6c69 7479 2074 6f20 7573 6520   ability to use 
+00006f80: 7468 6520 6361 6368 652e 2054 6865 2063  the cache. The c
+00006f90: 6163 6865 2077 6f72 6b73 2066 6f72 2065  ache works for e
+00006fa0: 6163 6820 5f44 6174 6120 6f62 6a65 6374  ach _Data object
+00006fb0: 5f2c 2074 6861 7420 6973 2c20 796f 7520  _, that is, you 
+00006fc0: 6368 6f6f 7365 0a20 2020 2020 2020 2077  choose.        w
+00006fd0: 6869 6368 205f 4461 7461 206f 626a 6563  hich _Data objec
+00006fe0: 745f 2079 6f75 2077 616e 7420 746f 2073  t_ you want to s
+00006ff0: 6176 652e 2054 6865 205f 4461 7461 206f  ave. The _Data o
+00007000: 626a 6563 745f 2063 6163 6865 2069 7320  bject_ cache is 
+00007010: 7361 7665 6420 6166 7465 7220 7468 6520  saved after the 
+00007020: 6669 7273 7420 6974 6572 6174 696f 6e2c  first iteration,
+00007030: 2062 7574 2074 6865 2069 7465 7261 7469   but the iterati
+00007040: 6f6e 0a20 2020 2020 2020 2073 6f75 7263  on.        sourc
+00007050: 6520 6d61 7920 6265 2064 6966 6665 7265  e may be differe
+00007060: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
+00007070: 2020 2020 2049 6620 796f 7520 646f 6e27       If you don'
+00007080: 7420 7573 6520 7468 6520 6361 6368 652c  t use the cache,
+00007090: 2079 6f75 7220 736f 7572 6365 2077 696c   your source wil
+000070a0: 6c20 6265 2074 6865 2064 6174 6120 736f  l be the data so
+000070b0: 7572 6365 2079 6f75 2068 6176 6520 696e  urce you have in
+000070c0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
+000070d0: 745f 2e20 4275 7420 6966 2079 6f75 2075  t_. But if you u
+000070e0: 7365 2074 6865 2063 6163 6865 2c0a 2020  se the cache,.  
+000070f0: 2020 2020 2020 796f 7572 2073 6f75 7263        your sourc
+00007100: 6520 6361 6e20 6265 2074 6865 2064 6174  e can be the dat
+00007110: 6120 736f 7572 6365 2c20 7468 6520 7061  a source, the pa
+00007120: 7265 6e74 2063 6163 6865 2c20 6f72 206f  rent cache, or o
+00007130: 776e 2063 6163 6865 3a0a 2020 2020 2020  wn cache:.      
+00007140: 2020 0a20 2020 2020 2020 202a 2054 6865    .        * The
+00007150: 2064 6174 6120 736f 7572 6365 3a0a 2020   data source:.  
+00007160: 2020 2020 2020 2020 4966 2074 6865 205f          If the _
+00007170: 4461 7461 204f 626a 6563 745f 2064 6f65  Data Object_ doe
+00007180: 736e 2774 2068 6176 6520 6120 7061 7265  sn't have a pare
+00007190: 6e74 2063 6163 6865 2061 6e64 2069 7473  nt cache and its
+000071a0: 2063 6163 6865 2e0a 2020 2020 2020 2020   cache..        
+000071b0: 2a20 5468 6520 7061 7265 6e74 2063 6163  * The parent cac
+000071c0: 6865 3a0a 2020 2020 2020 2020 2020 4966  he:.          If
+000071d0: 2074 6865 205f 4461 7461 204f 626a 6563   the _Data Objec
+000071e0: 745f 2068 6173 2061 2070 6172 656e 7420  t_ has a parent 
+000071f0: 6361 6368 652e 2049 7420 646f 6573 6e27  cache. It doesn'
+00007200: 7420 6d61 7474 6572 2077 6861 7420 706f  t matter what po
+00007210: 7369 7469 6f6e 2074 6865 2070 6172 656e  sition the paren
+00007220: 7420 6361 6368 6520 6861 7320 696e 2069  t cache has in i
+00007230: 6e68 6572 6974 616e 6365 2e0a 2020 2020  nheritance..    
+00007240: 2020 2020 2020 5f44 6174 6120 4f62 6a65        _Data Obje
+00007250: 6374 5f20 756e 6465 7273 7461 6e64 7320  ct_ understands 
+00007260: 7768 6f73 6520 6361 6368 6520 6974 2069  whose cache it i
+00007270: 7320 616e 6420 6578 6563 7574 6573 2074  s and executes t
+00007280: 6865 2070 6172 7420 6f66 2074 6865 2077  he part of the w
+00007290: 6f72 6b66 6c6f 7720 7468 6174 2077 6173  orkflow that was
+000072a0: 206e 6f74 2065 7865 6375 7465 642e 0a20   not executed.. 
+000072b0: 2020 2020 2020 202a 2054 6865 206f 776e         * The own
+000072c0: 2063 6163 6865 3a0a 2020 2020 2020 2020   cache:.        
+000072d0: 2020 4966 2069 7420 6973 206e 6f74 2074    If it is not t
+000072e0: 6865 2066 6972 7374 2069 7465 7261 7469  he first iterati
+000072f0: 6f6e 206f 6620 7468 6973 2044 6174 6120  on of this Data 
+00007300: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00007310: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
+00007320: 6174 2074 6865 2063 6163 6865 2073 7461  at the cache sta
+00007330: 7465 206f 6620 7468 6520 4461 7461 206f  te of the Data o
+00007340: 626a 6563 7420 6973 206e 6f74 2069 6e68  bject is not inh
+00007350: 6572 6974 6564 2e0a 2020 2020 2020 2020  erited..        
+00007360: 0a20 2020 2020 2020 2023 2323 2320 466f  .        #### Fo
+00007370: 7263 6564 2063 6163 6869 6e67 0a20 2020  rced caching.   
+00007380: 2020 2020 2059 6f75 2063 616e 2074 656c       You can tel
+00007390: 6c20 4453 2074 6f20 6361 6368 6520 6461  l DS to cache da
+000073a0: 7461 2074 6f20 7370 6563 6966 6963 2063  ta to specific c
+000073b0: 6163 6865 2066 696c 652c 2077 6869 6368  ache file, which
+000073c0: 2077 6f6e 2774 2062 6520 6465 6c65 7465   won't be delete
+000073d0: 6420 6166 7465 7220 7363 7269 7074 2065  d after script e
+000073e0: 6e64 2e0a 2020 2020 2020 2020 596f 7520  nd..        You 
+000073f0: 6361 6e20 7365 6520 6578 616d 706c 6520  can see example 
+00007400: 696e 2031 2e31 3220 7365 6374 696f 6e20  in 1.12 section 
+00007410: 6f66 205b 6765 745f 7374 6172 7465 645f  of [get_started_
+00007420: 6578 616d 706c 655d 2865 7861 6d70 6c65  example](example
+00007430: 732f 6765 745f 7374 6172 7465 645f 6578  s/get_started_ex
+00007440: 616d 706c 652e 7079 292e 0a20 2020 2020  ample.py)..     
+00007450: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00007460: 2020 2020 2023 2323 2045 7665 6e74 5472       ### EventTr
+00007470: 6565 2061 6e64 2063 6f6c 6c65 6374 696f  ee and collectio
+00007480: 6e73 0a20 2020 2020 2020 200a 2020 2020  ns.        .    
+00007490: 2020 2020 2323 2323 2045 7665 6e74 5472      #### EventTr
+000074a0: 6565 0a20 2020 2020 2020 200a 2020 2020  ee.        .    
+000074b0: 2020 2020 6045 7665 6e74 5472 6565 6020      `EventTree` 
+000074c0: 6973 2061 2074 7265 652d 6261 7365 6420  is a tree-based 
+000074d0: 6461 7461 2073 7472 7563 7475 7265 206f  data structure o
+000074e0: 6620 6576 656e 7473 2e20 4974 2061 6c6c  f events. It all
+000074f0: 6f77 7320 796f 7520 6765 7420 6368 696c  ows you get chil
+00007500: 6472 656e 2061 6e64 2070 6172 656e 7473  dren and parents
+00007510: 206f 6620 6576 656e 742c 0a20 2020 2020   of event,.     
+00007520: 2020 2064 6973 706c 6179 2074 7265 652c     display tree,
+00007530: 2067 6574 2066 756c 6c20 7061 7468 2074   get full path t
+00007540: 6f20 6576 656e 7420 6574 632e 0a20 2020  o event etc..   
+00007550: 2020 2020 200a 2020 2020 2020 2020 4465       .        De
+00007560: 7461 696c 733a 0a20 2020 2020 2020 200a  tails:.        .
+00007570: 2020 2020 2020 2020 2a20 6045 7665 6e74          * `Event
+00007580: 5472 6565 6020 636f 6e74 6169 6e73 2061  Tree` contains a
+00007590: 6c6c 2065 7665 6e74 7320 696e 206d 656d  ll events in mem
+000075a0: 6f72 792e 0a20 2020 2020 2020 202a 2054  ory..        * T
+000075b0: 7265 6520 6861 7320 736f 6d65 2069 6d70  ree has some imp
+000075c0: 6f72 7461 6e74 2074 6572 6d73 3a0a 2020  ortant terms:.  
+000075d0: 2020 2020 2020 2020 2020 312e 205f 416e            1. _An
+000075e0: 6365 7374 6f72 5f20 6973 2061 6e79 2072  cestor_ is any r
+000075f0: 656c 6174 6976 6520 6f66 2074 6865 2065  elative of the e
+00007600: 7665 6e74 2075 7020 7468 6520 7472 6565  vent up the tree
+00007610: 2028 6772 616e 6470 6172 656e 742c 2070   (grandparent, p
+00007620: 6172 656e 7420 6574 632e 292e 0a20 2020  arent etc.)..   
+00007630: 2020 2020 2020 2020 2032 2e20 5f50 6172           2. _Par
+00007640: 656e 745f 2069 7320 6f6e 6c79 2074 6865  ent_ is only the
+00007650: 2066 6972 7374 2072 656c 6174 6976 6520   first relative 
+00007660: 6f66 2074 6865 2065 7665 6e74 2075 7020  of the event up 
+00007670: 7468 6520 7472 6565 2e0a 2020 2020 2020  the tree..      
+00007680: 2020 2020 2020 332e 205f 4368 696c 645f        3. _Child_
+00007690: 2069 7320 7468 6520 6669 7273 7420 7265   is the first re
+000076a0: 6c61 7469 7665 206f 6620 7468 6520 6576  lative of the ev
+000076b0: 656e 7420 646f 776e 2074 6865 2074 7265  ent down the tre
+000076c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+000076d0: 2020 2020 5461 6b65 2061 206c 6f6f 6b20      Take a look 
+000076e0: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
+000076f0: 2048 544d 4c20 7472 6565 2074 6f20 756e   HTML tree to un
+00007700: 6465 7273 7461 6e64 2074 6865 6d2e 0a20  derstand them.. 
+00007710: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00007720: 2020 2060 6060 0a20 2020 2020 2020 2020     ```.         
+00007730: 2020 203c 626f 6479 3e20 3c21 2d2d 2061     <body> <!-- a
+00007740: 6e63 6573 746f 7220 2867 7261 6e64 7061  ncestor (grandpa
+00007750: 7265 6e74 292c 2062 7574 206e 6f74 2070  rent), but not p
+00007760: 6172 656e 7420 2d2d 3e0a 2020 2020 2020  arent -->.      
+00007770: 2020 2020 2020 2020 2020 3c64 6976 3e20            <div> 
+00007780: 3c21 2d2d 2070 6172 656e 7420 2620 616e  <!-- parent & an
+00007790: 6365 7374 6f72 202d 2d3e 0a20 2020 2020  cestor -->.     
+000077a0: 2020 2020 2020 2020 2020 2020 2020 203c                 <
+000077b0: 703e 4865 6c6c 6f2c 2077 6f72 6c64 213c  p>Hello, world!<
+000077c0: 2f70 3e20 3c21 2d2d 2063 6869 6c64 202d  /p> <!-- child -
+000077d0: 2d3e 0a20 2020 2020 2020 2020 2020 2020  ->.             
+000077e0: 2020 2020 2020 203c 703e 476f 6f64 6279         <p>Goodby
+000077f0: 6521 3c2f 703e 203c 212d 2d20 7369 626c  e!</p> <!-- sibl
+00007800: 696e 6720 2d2d 3e0a 2020 2020 2020 2020  ing -->.        
+00007810: 2020 2020 2020 2020 3c2f 6469 763e 0a20          </div>. 
+00007820: 2020 2020 2020 2020 2020 203c 2f62 6f64             </bod
+00007830: 793e 0a20 2020 2020 2020 2020 2020 6060  y>.           ``
+00007840: 600a 2020 2020 2020 2020 0a20 2020 2020  `.        .     
+00007850: 2020 2023 2323 2320 436f 6c6c 6563 7469     #### Collecti
+00007860: 6f6e 730a 2020 2020 2020 2020 0a20 2020  ons.        .   
+00007870: 2020 2020 202a 2a45 7665 6e74 5472 6565       **EventTree
+00007880: 436f 6c6c 6563 7469 6f6e 2a2a 2069 7320  Collection** is 
+00007890: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
+000078a0: 4576 656e 7454 7265 6573 2e20 5468 6520  EventTrees. The 
+000078b0: 636f 6c6c 6563 7469 6f6e 2062 7569 6c64  collection build
+000078c0: 7320 6120 6665 7720 5f45 7665 6e74 5472  s a few _EventTr
+000078d0: 6565 5f20 6279 2070 6173 7365 6420 5f44  ee_ by passed _D
+000078e0: 6174 610a 2020 2020 2020 2020 6f62 6a65  ata.        obje
+000078f0: 6374 5f2e 2041 6c74 686f 7567 6820 796f  ct_. Although yo
+00007900: 7520 6361 6e20 6368 616e 6765 2074 6865  u can change the
+00007910: 2074 7265 6520 6469 7265 6374 6c79 2c20   tree directly, 
+00007920: 6974 2773 2062 6574 7465 7220 746f 2064  it's better to d
+00007930: 6f20 6974 2074 6872 6f75 6768 2063 6f6c  o it through col
+00007940: 6c65 6374 696f 6e73 2062 6563 6175 7365  lections because
+00007950: 2074 6865 7920 6172 6520 6177 6172 6520   they are aware 
+00007960: 6f66 0a20 2020 2020 2020 2060 6465 7461  of.        `deta
+00007970: 6368 6564 5f65 7665 6e74 7360 2061 6e64  ched_events` and
+00007980: 2063 616e 2073 6f6c 7665 2073 6f6d 6520   can solve some 
+00007990: 6576 656e 7473 2064 6570 656e 6465 6e63  events dependenc
+000079a0: 6965 732e 2054 6865 2063 6f6c 6c65 6374  ies. The collect
+000079b0: 696f 6e20 6861 7320 7369 6d69 6c61 7220  ion has similar 
+000079c0: 6665 6174 7572 6573 206c 696b 6520 6120  features like a 
+000079d0: 7369 6e67 6c65 205f 4576 656e 7454 7265  single _EventTre
+000079e0: 655f 0a20 2020 2020 2020 2062 7574 2061  e_.        but a
+000079f0: 7070 6c79 696e 6720 7468 656d 2066 6f72  pplying them for
+00007a00: 2061 6c6c 205f 4576 656e 7454 7265 6573   all _EventTrees
+00007a10: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
+00007a20: 2020 2020 2a2a 5061 7265 6e74 4576 656e      **ParentEven
+00007a30: 7454 7265 6543 6f6c 6c65 6374 696f 6e2a  tTreeCollection*
+00007a40: 2a20 6973 2061 2063 6f6c 6c65 6374 696f  * is a collectio
+00007a50: 6e20 7369 6d69 6c61 7220 746f 205f 4576  n similar to _Ev
+00007a60: 656e 7454 7265 6543 6f6c 6c65 6374 696f  entTreeCollectio
+00007a70: 6e5f 2062 7574 2063 6f6e 7461 696e 696e  n_ but containin
+00007a80: 6720 6f6e 6c79 2070 6172 656e 7420 6576  g only parent ev
+00007a90: 656e 7473 2074 6861 740a 2020 2020 2020  ents that.      
+00007aa0: 2020 6172 6520 7265 6665 7265 6e63 6564    are referenced
+00007ab0: 2069 6e20 7468 6520 6461 7461 2073 7472   in the data str
+00007ac0: 6561 6d2e 2054 6865 2063 6f6c 6c65 6374  eam. The collect
+00007ad0: 696f 6e20 6861 7320 6665 6174 7572 6573  ion has features
+00007ae0: 2073 696d 696c 6172 2074 6f20 5f45 7665   similar to _Eve
+00007af0: 6e74 5472 6565 436f 6c6c 6563 7469 6f6e  ntTreeCollection
+00007b00: 5f2e 0a20 2020 2020 2020 200a 2020 2020  _..        .    
+00007b10: 2020 2020 4465 7461 696c 733a 0a20 2020      Details:.   
+00007b20: 2020 2020 200a 2020 2020 2020 2020 2a20       .        * 
+00007b30: 546f 2075 7365 2045 5420 636f 6c6c 6563  To use ET collec
+00007b40: 7469 6f6e 7320 796f 7520 6e65 6564 2074  tions you need t
+00007b50: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
+00007b60: 6d20 6279 205f 4554 4344 7269 7665 725f  m by _ETCDriver_
+00007b70: 2e20 4461 7461 2073 6f75 7263 6573 2075  . Data sources u
+00007b80: 7375 616c 6c79 2070 726f 7669 6465 2074  sually provide t
+00007b90: 6865 6d2e 0a20 2020 2020 2020 2020 2059  hem..          Y
+00007ba0: 6f75 2063 616e 2063 7265 6174 6520 6974  ou can create it
+00007bb0: 2062 7920 796f 7572 7365 6c66 2064 6570   by yourself dep
+00007bc0: 656e 6469 6e67 206f 6e20 796f 7572 2064  ending on your d
+00007bd0: 6174 6120 7374 7275 6374 7572 652e 0a20  ata structure.. 
+00007be0: 2020 2020 2020 202a 2054 6865 2063 6f6c         * The col
+00007bf0: 6c65 6374 696f 6e20 6861 7320 6120 6665  lection has a fe
+00007c00: 6174 7572 6520 746f 2072 6563 6f76 6572  ature to recover
+00007c10: 2065 7665 6e74 732e 2041 6c6c 2065 7665   events. All eve
+00007c20: 6e74 7320 7468 6174 2061 7265 206e 6f74  nts that are not
+00007c30: 2069 6e20 7468 6520 7265 6365 6976 6564   in the received
+00007c40: 2064 6174 6120 7374 7265 616d 2c20 6275   data stream, bu
+00007c50: 7420 7768 6963 6820 6172 650a 2020 2020  t which are.    
+00007c60: 2020 2020 2020 7265 6665 7265 6e63 6564        referenced
+00007c70: 2077 696c 6c20 6265 206c 6f61 6465 6420   will be loaded 
+00007c80: 6672 6f6d 2074 6865 2064 6174 6120 736f  from the data so
+00007c90: 7572 6365 2e0a 2020 2020 2020 2020 2a20  urce..        * 
+00007ca0: 596f 7520 6361 6e20 7461 6b65 2060 6465  You can take `de
+00007cb0: 7461 6368 6564 5f65 7665 6e74 7360 2074  tached_events` t
+00007cc0: 6f20 7365 6520 7768 6963 6820 6576 656e  o see which even
+00007cd0: 7473 2061 7265 206d 6973 7369 6e67 2e0a  ts are missing..
+00007ce0: 2020 2020 2020 2020 2a20 4966 2079 6f75          * If you
+00007cf0: 2077 616e 742c 2079 6f75 2063 616e 2062   want, you can b
+00007d00: 7569 6c64 2070 6172 656e 746c 6573 7320  uild parentless 
+00007d10: 7472 6565 7320 7768 6572 6520 7468 6520  trees where the 
+00007d20: 6d69 7373 696e 6720 6576 656e 7473 2061  missing events a
+00007d30: 7265 2073 7475 6262 6564 2069 6e73 7465  re stubbed inste
+00007d40: 6164 2e20 4a75 7374 0a20 2020 2020 2020  ad. Just.       
+00007d50: 2020 2075 7365 2060 6765 745f 7061 7265     use `get_pare
+00007d60: 6e74 6c65 7373 5f74 7265 6573 2829 602e  ntless_trees()`.
+00007d70: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00007d80: 2020 5265 7175 6972 656d 656e 7473 3a0a    Requirements:.
+00007d90: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007da0: 2031 2e20 4576 656e 7473 2070 726f 7669   1. Events provi
+00007db0: 6465 6420 746f 2045 5443 2068 6176 6520  ded to ETC have 
+00007dc0: 746f 2068 6176 6520 6065 7665 6e74 5f6e  to have `event_n
+00007dd0: 616d 6560 2c20 6065 7665 6e74 5f69 6460  ame`, `event_id`
+00007de0: 2c20 6070 6172 656e 745f 6576 656e 745f  , `parent_event_
+00007df0: 6964 6020 6669 656c 6473 2e20 5468 6579  id` fields. They
+00007e00: 0a20 2020 2020 2020 2063 616e 2068 6176  .        can hav
+00007e10: 6520 616e 6f74 6865 7220 6e61 6d65 7320  e another names 
+00007e20: 2869 7420 7265 736f 6c76 6573 2069 6e20  (it resolves in 
+00007e30: 7468 6520 6472 6976 6572 292e 0a20 2020  the driver)..   
+00007e40: 2020 2020 200a 2020 2020 2020 2020 2323       .        ##
+00007e50: 2323 2048 696e 7473 0a20 2020 2020 2020  ## Hints.       
+00007e60: 200a 2020 2020 2020 2020 2a20 5265 6d6f   .        * Remo
+00007e70: 7665 2061 6c6c 2075 6e6e 6563 6573 7361  ve all unnecessa
+00007e80: 7279 2066 6965 6c64 7320 6672 6f6d 2065  ry fields from e
+00007e90: 7665 6e74 7320 6265 666f 7265 2070 6173  vents before pas
+00007ea0: 7369 6e67 2074 6f20 6120 5f63 6f6c 6c65  sing to a _colle
+00007eb0: 6374 696f 6e5f 2074 6f20 7265 6475 6365  ction_ to reduce
+00007ec0: 206d 656d 6f72 7920 7573 6167 652e 0a20   memory usage.. 
+00007ed0: 2020 2020 2020 202a 2055 7365 2060 7368         * Use `sh
+00007ee0: 6f77 2829 6020 6d65 7468 6f64 2074 6f20  ow()` method to 
+00007ef0: 7072 696e 7420 7468 6520 7472 6565 2069  print the tree i
+00007f00: 6e20 7472 6565 2d6c 696b 6520 7669 6577  n tree-like view
+00007f10: 2e0a 2020 2020 2020 2020 2a20 4e6f 7465  ..        * Note
+00007f20: 2074 6861 7420 7468 6520 6067 6574 5f78   that the `get_x
+00007f30: 6020 6d65 7468 6f64 7320 7769 6c6c 2072  ` methods will r
+00007f40: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
+00007f50: 6e20 6966 2079 6f75 2070 6173 7320 616e  n if you pass an
+00007f60: 2075 6e6b 6e6f 776e 2065 7665 6e74 2069   unknown event i
+00007f70: 642c 2075 6e6c 696b 6520 7468 6520 6066  d, unlike the `f
+00007f80: 696e 645f 7860 206d 6574 686f 6473 2028  ind_x` methods (
+00007f90: 0a20 2020 2020 2020 2020 2074 6865 7920  .          they 
+00007fa0: 7265 7475 726e 204e 6f6e 6529 2e0a 2020  return None)..  
+00007fb0: 2020 2020 2020 2a20 4966 2079 6f75 2077        * If you w
+00007fc0: 616e 7420 746f 206b 6e6f 7720 7468 6174  ant to know that
+00007fd0: 2073 7065 6369 6669 6564 2065 7665 6e74   specified event
+00007fe0: 2065 7869 7374 732c 2075 7365 2074 6865   exists, use the
+00007ff0: 2070 7974 686f 6e20 6069 6e60 206b 6579   python `in` key
+00008000: 776f 7264 2028 652e 672e 2060 2765 7665  word (e.g. `'eve
+00008010: 6e74 2d69 6427 2069 6e20 6576 656e 7473  nt-id' in events
+00008020: 5f74 7265 6560 292e 0a20 2020 2020 2020  _tree`)..       
+00008030: 202a 2055 7365 2074 6865 2070 7974 686f   * Use the pytho
+00008040: 6e20 606c 656e 6020 6b65 7977 6f72 6420  n `len` keyword 
+00008050: 746f 2067 6574 2065 7665 6e74 7320 6e75  to get events nu
+00008060: 6d62 6572 2069 6e20 7468 6520 7472 6565  mber in the tree
+00008070: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
+00008080: 2020 2023 2323 2046 6965 6c64 2052 6573     ### Field Res
+00008090: 6f6c 7665 7273 0a20 2020 2020 2020 2049  olvers.        I
+000080a0: 6e74 6572 6661 6365 2063 616e 2062 6520  nterface can be 
+000080b0: 666f 756e 6420 696e 2060 7468 325f 6461  found in `th2_da
+000080c0: 7461 5f73 6572 7669 6365 732f 696e 7465  ta_services/inte
+000080d0: 7266 6163 6573 2f75 7469 6c73 2f72 6573  rfaces/utils/res
+000080e0: 6f6c 7665 722e 7079 602e 2020 0a20 2020  olver.py`.  .   
+000080f0: 2020 2020 2041 6c6c 2064 6174 612d 736f       All data-so
+00008100: 7572 6365 7320 7368 6f75 6c64 2069 6d70  urces should imp
+00008110: 6c65 6d65 6e74 2074 6865 6d2e 0a20 2020  lement them..   
+00008120: 2020 2020 200a 2020 2020 2020 2020 5468       .        Th
+00008130: 6520 6964 6561 206f 6620 7573 696e 6720  e idea of using 
+00008140: 7265 736f 6c76 6572 733a 0a20 2020 2020  resolvers:.     
+00008150: 2020 2049 7420 736f 6c76 6573 2074 6865     It solves the
+00008160: 2070 726f 626c 656d 206f 6620 6861 7669   problem of havi
+00008170: 6e67 2061 2066 6577 2044 6174 6153 6f75  ng a few DataSou
+00008180: 7263 6573 2077 6974 6820 7369 6d69 6c61  rces with simila
+00008190: 7220 6461 7461 2c0a 2020 2020 2020 2020  r data,.        
+000081a0: 6275 7420 7769 7468 2064 6966 6665 7265  but with differe
+000081b0: 6e74 2077 6179 7320 746f 2067 6574 2069  nt ways to get i
+000081c0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
+000081d0: 2020 2020 5468 6573 6520 636c 6173 7365      These classe
+000081e0: 7320 7072 6f76 6964 6520 796f 7520 6765  s provide you ge
+000081f0: 7474 6572 206d 6574 686f 6473 2e0a 2020  tter methods..  
+00008200: 2020 2020 2020 5573 696e 6720 7468 6573        Using thes
+00008210: 6520 636c 6173 7365 7320 616c 6c6f 7773  e classes allows
+00008220: 2079 6f75 2074 6f20 6672 6565 6c79 2073   you to freely s
+00008230: 7769 7463 6820 6265 7477 6565 6e20 6469  witch between di
+00008240: 6666 6572 656e 7420 6461 7461 0a20 2020  fferent data.   
+00008250: 2020 2020 2066 6f72 6d61 7473 2061 6e64       formats and
+00008260: 2064 6f6e 2774 2063 6861 6e67 6520 796f   don't change yo
+00008270: 7572 2063 6f64 652e 0a20 2020 2020 2020  ur code..       
+00008280: 200a 2020 2020 2020 2020 5265 736f 6c76   .        Resolv
+00008290: 6572 7320 736f 6c76 6520 7468 6520 7072  ers solve the pr
+000082a0: 6f62 6c65 6d20 6f66 2064 6174 612d 666f  oblem of data-fo
+000082b0: 726d 6174 206d 6967 7261 7469 6f6e 2e0a  rmat migration..
+000082c0: 2020 2020 2020 2020 2d20 6669 656c 6473          - fields
+000082d0: 2070 6c61 6365 2063 616e 2062 6520 6368   place can be ch
+000082e0: 616e 6765 640a 2020 2020 2020 2020 2d20  anged.        - 
+000082f0: 6669 656c 6473 206e 616d 6573 2063 616e  fields names can
+00008300: 2062 6520 6368 616e 6765 640a 2020 2020   be changed.    
+00008310: 2020 2020 0a20 2020 2020 2020 2052 6573      .        Res
+00008320: 6f6c 7665 7273 2063 616e 2077 6f72 6b20  olvers can work 
+00008330: 6f6e 6c79 2077 6974 6820 6f6e 6520 6576  only with one ev
+00008340: 656e 742f 6d65 7373 6167 652e 0a20 2020  ent/message..   
+00008350: 2020 2020 2049 7420 6d65 616e 732c 2069       It means, i
+00008360: 6620 796f 7572 206d 6573 7361 6765 2068  f your message h
+00008370: 6173 2073 7562 2d6d 6573 7361 6765 7320  as sub-messages 
+00008380: 286c 696b 6520 7468 322d 6d65 7373 6167  (like th2-messag
+00008390: 6573 2069 6e20 6c77 6470 2920 6974 200a  es in lwdp) it .
+000083a0: 2020 2020 2020 2020 776f 6e27 7420 776f          won't wo
+000083b0: 726b 2c20 6265 6361 7573 6520 7265 736f  rk, because reso
+000083c0: 6c76 6572 2077 696c 6c20 6e6f 7420 6b6e  lver will not kn
+000083d0: 6f77 2077 6974 6820 7768 6963 6820 7375  ow with which su
+000083e0: 622d 6d65 7373 6167 6520 7368 6f75 6c64  b-message should
+000083f0: 2069 7420 776f 726b 2e20 0a20 2020 2020   it work. .     
+00008400: 2020 200a 2020 2020 2020 2020 2a2a 576f     .        **Wo
+00008410: 726b 6172 6f75 6e64 2a2a 2020 0a20 2020  rkaround**  .   
+00008420: 2020 2020 2031 2e20 4578 7061 6e64 2061       1. Expand a
+00008430: 6c6c 2079 6f75 7220 6d65 7373 6167 6573  ll your messages
+00008440: 202d 3e20 606e 6577 5f64 203d 2079 6f75   -> `new_d = you
+00008450: 725f 6461 7461 2e6d 6170 284d 6573 7361  r_data.map(Messa
+00008460: 6765 4669 656c 6452 6573 6f6c 7665 722e  geFieldResolver.
+00008470: 6578 7061 6e64 5f6d 6573 7361 6765 2960  expand_message)`
+00008480: 0a20 2020 2020 2020 2032 2e20 5573 6520  .        2. Use 
+00008490: 6045 7870 616e 6465 644d 6573 7361 6765  `ExpandedMessage
+000084a0: 4669 656c 6452 6573 6f6c 7665 7260 2069  FieldResolver` i
+000084b0: 6e73 7465 6164 206f 6620 7573 7561 6c20  nstead of usual 
+000084c0: 604d 6573 7361 6765 4669 656c 6452 6573  `MessageFieldRes
+000084d0: 6f6c 7665 7260 2077 6865 6e20 0a20 2020  olver` when .   
+000084e0: 2020 2020 2020 2020 2079 6f75 2074 616b           you tak
+000084f0: 6520 6669 656c 6473 2066 6f72 2065 7870  e fields for exp
+00008500: 616e 6465 6420 6d65 7373 6167 6573 2e0a  anded messages..
+00008510: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00008520: 202a 2a49 6d70 6c65 6d65 6e74 6174 696f   **Implementatio
+00008530: 6e20 6164 7669 6365 3a2a 2a0a 2020 2020  n advice:**.    
+00008540: 2020 2020 312e 2072 6169 7365 204e 6f74      1. raise Not
+00008550: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+00008560: 202d 2d20 6966 2079 6f75 7220 496d 706c   -- if your Impl
+00008570: 656d 656e 7461 7469 6f6e 2064 6f65 736e  ementation doesn
+00008580: 2774 2073 7570 706f 7274 2074 6869 7320  't support this 
+00008590: 6765 7474 6572 2e0a 2020 2020 2020 2020  getter..        
+000085a0: 0a20 2020 2020 2020 202a 2a50 6572 666f  .        **Perfo
+000085b0: 726d 616e 6365 2069 6d70 6163 743a 2a2a  rmance impact:**
+000085c0: 0a20 2020 2020 2020 202d 2049 7420 6120  .        - It a 
+000085d0: 6269 7420 736c 6f77 6572 2074 6861 6e20  bit slower than 
+000085e0: 7573 696e 6720 6e61 6b65 6420 6669 656c  using naked fiel
+000085f0: 6420 6163 6365 7373 2060 6469 6374 5b27  d access `dict['
+00008600: 6b65 7927 5d60 2e0a 2020 2020 2020 2020  key']`..        
+00008610: 0a20 2020 2020 2020 2023 2320 322e 342e  .        ## 2.4.
+00008620: 204c 696e 6b73 0a20 2020 2020 2020 200a   Links.        .
+00008630: 2020 2020 2020 2020 2d20 5b52 6570 6f72          - [Repor
+00008640: 7420 4461 7461 2050 726f 7669 6465 725d  t Data Provider]
+00008650: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00008660: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
+00008670: 7270 742d 6461 7461 2d70 726f 7669 6465  rpt-data-provide
+00008680: 7229 0a20 2020 2020 2020 202d 205b 5468  r).        - [Th
+00008690: 3220 4461 7461 2053 6572 7669 6365 7320  2 Data Services 
+000086a0: 5574 696c 735d 2868 7474 7073 3a2f 2f67  Utils](https://g
+000086b0: 6974 6875 622e 636f 6d2f 7468 322d 6e65  ithub.com/th2-ne
+000086c0: 742f 7468 322d 6461 7461 2d73 6572 7669  t/th2-data-servi
+000086d0: 6365 732d 7574 696c 7329 0a20 2020 2020  ces-utils).     
+000086e0: 2020 200a 2020 2020 2020 2020 2320 332e     .        # 3.
+000086f0: 2042 6573 7420 7072 6163 7469 6365 730a   Best practices.
+00008700: 2020 2020 2020 2020 4465 7065 6e64 696e          Dependin
+00008710: 6720 6f6e 2068 6f77 2079 6f75 2077 6f72  g on how you wor
+00008720: 6b20 7769 7468 2060 4461 7461 206f 626a  k with `Data obj
+00008730: 6563 7460 2c20 6974 2063 616e 2062 6520  ect`, it can be 
+00008740: 736c 6f77 206f 6620 6661 7374 2e0a 2020  slow of fast..  
+00008750: 2020 2020 2020 4173 2077 6974 6820 6120        As with a 
+00008760: 7265 6c61 7469 6f6e 616c 2064 6174 6162  relational datab
+00008770: 6173 652c 2079 6f75 2063 616e 2077 7269  ase, you can wri
+00008780: 7465 2061 2071 7565 7279 2074 6861 7420  te a query that 
+00008790: 7769 6c6c 2072 6574 7572 6e20 6461 7461  will return data
+000087a0: 2073 6c6f 776c 7920 6f72 2071 7569 636b   slowly or quick
+000087b0: 6c79 2c0a 2020 2020 2020 2020 7468 6520  ly,.        the 
+000087c0: 7361 6d65 2077 6865 6e20 776f 726b 696e  same when workin
+000087d0: 6720 7769 7468 2061 2060 4461 7461 206f  g with a `Data o
+000087e0: 626a 6563 7460 2e0a 2020 2020 2020 2020  bject`..        
+000087f0: 0a20 2020 2020 2020 2046 6f6c 6c6f 7720  .        Follow 
+00008800: 7468 6520 7275 6c65 7320 746f 206d 616b  the rules to mak
+00008810: 6520 796f 7572 2077 6f72 6b20 7769 7468  e your work with
+00008820: 2044 6174 6120 6f62 6a65 6374 2066 6173   Data object fas
+00008830: 743a 0a20 2020 2020 2020 2031 2e20 5573  t:.        1. Us
+00008840: 6520 6044 6174 612e 7573 655f 6361 6368  e `Data.use_cach
+00008850: 6528 2960 2069 6620 796f 7520 6974 6572  e()` if you iter
+00008860: 6174 6520 6461 7461 206d 6f72 6520 7468  ate data more th
+00008870: 616e 206f 6e65 2074 696d 652e 0a20 2020  an one time..   
+00008880: 2020 2020 2032 2e20 5472 7920 746f 2064       2. Try to d
+00008890: 6f6e 2774 2069 7465 7261 7465 206f 6e65  on't iterate one
+000088a0: 2060 4461 7461 206f 626a 6563 7460 2069   `Data object` i
+000088b0: 6e73 6964 6520 7468 6520 6f74 6865 7220  nside the other 
+000088c0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+000088d0: 4966 2079 6f75 2073 686f 756c 6420 746f  If you should to
+000088e0: 2064 6f20 6974 2c20 7573 6520 7368 6f72   do it, use shor
+000088f0: 7420 6044 6174 6120 6f62 6a65 6374 6020  t `Data object` 
+00008900: 6669 7273 7420 616e 6420 6c6f 6e67 2060  first and long `
+00008910: 4461 7461 206f 626a 6563 7460 2069 6e73  Data object` ins
+00008920: 6964 6520 7468 6520 6c6f 6f70 2e0a 2020  ide the loop..  
+00008930: 2020 2020 2020 2020 2049 7427 6c6c 2061           It'll a
+00008940: 6c6c 6f77 2079 6f75 206f 7065 6e20 7468  llow you open th
+00008950: 6520 6361 6368 6520 6669 6c65 206f 7220  e cache file or 
+00008960: 6372 6561 7465 2061 2072 6571 7565 7374  create a request
+00008970: 2074 6f20 6044 6174 6120 736f 7572 6365   to `Data source
+00008980: 6020 6c65 7373 206e 756d 6265 7220 6f66  ` less number of
+00008990: 2074 696d 6573 2e0a 2020 2020 2020 2020   times..        
+000089a0: 0a20 2020 2020 2020 2023 2034 2e20 4f66  .        # 4. Of
+000089b0: 6669 6369 616c 2044 6174 6153 6f75 7263  ficial DataSourc
+000089c0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000089d0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+000089e0: 2020 202d 205b 4c69 6768 7477 6569 6768     - [Lightweigh
+000089f0: 7420 4461 7461 2050 726f 7669 6465 7220  t Data Provider 
+00008a00: 4461 7461 2053 6f75 7263 655d 2868 7474  Data Source](htt
+00008a10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00008a20: 7468 322d 6e65 742f 7468 322d 6473 2d73  th2-net/th2-ds-s
+00008a30: 6f75 7263 652d 6c77 6470 290a 2020 2020  ource-lwdp).    
+00008a40: 2020 2020 0a20 2020 2020 2020 200a 2020      .        .  
+00008a50: 2020 2020 2020 2320 352e 2041 5049 0a20        # 5. API. 
+00008a60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00008a70: 4966 2079 6f75 2061 7265 206c 6f6f 6b69  If you are looki
+00008a80: 6e67 2066 6f72 2063 6c61 7373 6573 2064  ng for classes d
+00008a90: 6573 6372 6970 7469 6f6e 2073 6565 2074  escription see t
+00008aa0: 6865 205b 4150 4920 446f 6375 6d65 6e74  he [API Document
+00008ab0: 6174 696f 6e5d 2864 6f63 756d 656e 7461  ation](documenta
+00008ac0: 7469 6f6e 2f61 7069 2f69 6e64 6578 2e6d  tion/api/index.m
+00008ad0: 6429 2e0a 2020 2020 2020 2020 0a20 2020  d)..        .   
+00008ae0: 2020 2020 2023 2036 2e20 4578 616d 706c       # 6. Exampl
+00008af0: 6573 0a20 2020 2020 2020 200a 2020 2020  es.        .    
+00008b00: 2020 2020 2d20 5b67 6574 5f73 7461 7274      - [get_start
+00008b10: 6564 5f65 7861 6d70 6c65 2e70 795d 2865  ed_example.py](e
+00008b20: 7861 6d70 6c65 732f 6765 745f 7374 6172  xamples/get_star
+00008b30: 7465 645f 6578 616d 706c 652e 7079 290a  ted_example.py).
+00008b40: 2020 2020 2020 2020 0a50 6c61 7466 6f72          .Platfor
+00008b50: 6d3a 2055 4e4b 4e4f 574e 0a52 6571 7569  m: UNKNOWN.Requi
+00008b60: 7265 732d 5079 7468 6f6e 3a20 3e3d 332e  res-Python: >=3.
+00008b70: 370a 4465 7363 7269 7074 696f 6e2d 436f  7.Description-Co
+00008b80: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00008b90: 2f6d 6172 6b64 6f77 6e0a 5072 6f76 6964  /markdown.Provid
+00008ba0: 6573 2d45 7874 7261 3a20 7264 700a 5072  es-Extra: rdp.Pr
+00008bb0: 6f76 6964 6573 2d45 7874 7261 3a20 7264  ovides-Extra: rd
+00008bc0: 7035 0a50 726f 7669 6465 732d 4578 7472  p5.Provides-Extr
+00008bd0: 613a 2072 6470 360a 5072 6f76 6964 6573  a: rdp6.Provides
+00008be0: 2d45 7874 7261 3a20 6c77 6470 0a50 726f  -Extra: lwdp.Pro
+00008bf0: 7669 6465 732d 4578 7472 613a 206c 7764  vides-Extra: lwd
+00008c00: 7031 0a50 726f 7669 6465 732d 4578 7472  p1.Provides-Extr
+00008c10: 613a 206c 7764 7032 0a50 726f 7669 6465  a: lwdp2.Provide
+00008c20: 732d 4578 7472 613a 206c 7764 7033 0a50  s-Extra: lwdp3.P
+00008c30: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+00008c40: 7764 702d 6465 760a 5072 6f76 6964 6573  wdp-dev.Provides
+00008c50: 2d45 7874 7261 3a20 7574 696c 732d 7270  -Extra: utils-rp
+00008c60: 742d 7669 6577 6572 0a50 726f 7669 6465  t-viewer.Provide
+00008c70: 732d 4578 7472 613a 2075 7469 6c73 2d72  s-Extra: utils-r
+00008c80: 7074 2d76 6965 7765 7235 0a50 726f 7669  pt-viewer5.Provi
+00008c90: 6465 732d 4578 7472 613a 2075 7469 6c73  des-Extra: utils
+00008ca0: 2d61 6476 616e 6365 640a                 -advanced.
```

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8344817329/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev8662586819/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

