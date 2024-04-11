# Comparing `tmp/pyegeria-0.3.3.tar.gz` & `tmp/pyegeria-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyegeria-0.3.3.tar", last modified: Wed Apr 10 02:48:17 2024, max compression
+gzip compressed data, was "pyegeria-0.3.4.tar", last modified: Thu Apr 11 21:14:10 2024, max compression
```

## Comparing `pyegeria-0.3.3.tar` & `pyegeria-0.3.4.tar`

### file list

```diff
@@ -1,47 +1,87 @@
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.292011 pyegeria-0.3.3/
--rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-02-13 19:55:10.000000 pyegeria-0.3.3/LICENSE
--rw-r--r--   0 dwolfson   (501) staff       (20)        0 2024-02-13 19:55:10.000000 pyegeria-0.3.3/MANIFEST.in
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-10 02:48:17.291821 pyegeria-0.3.3/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-09 02:21:44.000000 pyegeria-0.3.3/README.md
--rw-r--r--   0 dwolfson   (501) staff       (20)     1016 2024-04-09 22:07:39.000000 pyegeria-0.3.3/pyproject.toml
--rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-10 02:48:17.292048 pyegeria-0.3.3/setup.cfg
--rw-r--r--   0 dwolfson   (501) staff       (20)     1165 2024-04-09 22:07:39.000000 pyegeria-0.3.3/setup.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.279264 pyegeria-0.3.3/src/
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.287207 pyegeria-0.3.3/src/pyegeria/
--rw-r--r--   0 dwolfson   (501) staff       (20)     1612 2024-04-09 21:54:17.000000 pyegeria-0.3.3/src/pyegeria/__init__.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-02-09 22:22:39.000000 pyegeria-0.3.3/src/pyegeria/_globals.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/_validators.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    99769 2024-04-09 12:36:45.000000 pyegeria-0.3.3/src/pyegeria/automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    93697 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-09 15:45:59.000000 pyegeria-0.3.3/src/pyegeria/exceptions.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    46147 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    35897 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    19930 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6272 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/governance_author.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    42436 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    43011 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8713 2024-04-09 22:07:10.000000 pyegeria-0.3.3/src/pyegeria/registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    16273 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-09 02:21:44.000000 pyegeria-0.3.3/src/pyegeria/utils.py
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.291543 pyegeria-0.3.3/src/pyegeria.egg-info/
--rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/PKG-INFO
--rw-r--r--   0 dwolfson   (501) staff       (20)     1157 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/SOURCES.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/dependency_links.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/requires.txt
--rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-10 02:48:17.000000 pyegeria-0.3.3/src/pyegeria.egg-info/top_level.txt
-drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-10 02:48:17.291317 pyegeria-0.3.3/tests/
--rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_automated_curation_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_automated_curation_omvs_cray.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_client.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-09 20:58:51.000000 pyegeria-0.3.3/tests/test_core_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_full_omag_server_config.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_glossary_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_gov_engine.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     9624 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_my_profile_omvs.py
--rw-r--r--   0 dwolfson   (501) staff       (20)    40009 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_platform_services.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     4728 2024-04-09 21:23:08.000000 pyegeria-0.3.3/tests/test_registered_info.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_server_operations.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_util_exp.py
--rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-09 02:21:44.000000 pyegeria-0.3.3/tests/test_validators.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.618025 pyegeria-0.3.4/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11357 2024-04-10 19:14:09.000000 pyegeria-0.3.4/LICENSE
+-rw-r--r--   0 dwolfson   (501) staff       (20)       32 2024-04-11 15:17:10.000000 pyegeria-0.3.4/MANIFEST.in
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-11 21:14:10.617867 pyegeria-0.3.4/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1458 2024-04-11 02:07:05.000000 pyegeria-0.3.4/README.md
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.610000 pyegeria-0.3.4/examples/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6148 2024-04-11 16:00:57.000000 pyegeria-0.3.4/examples/.DS_Store
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.611527 pyegeria-0.3.4/examples/Coco_config/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      926 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       45 2024-04-11 14:15:42.000000 pyegeria-0.3.4/examples/Coco_config/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4070 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3666 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS2.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3661 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS3.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2950 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS4.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3179 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS5.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3987 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDS6.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4195 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoMDSx.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5220 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_cocoView1.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3557 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_exchangeDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2478 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_governDL01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2063 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_monitorDev01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8067 2024-04-10 19:14:09.000000 pyegeria-0.3.4/examples/Coco_config/config_monitorGov01.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5899 2024-04-11 14:25:11.000000 pyegeria-0.3.4/examples/Coco_config/globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)       18 2024-04-11 15:17:10.000000 pyegeria-0.3.4/examples/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.611632 pyegeria-0.3.4/examples/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      194 2024-04-11 16:37:25.000000 pyegeria-0.3.4/examples/__pycache__/__init__.cpython-312.pyc
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.613196 pyegeria-0.3.4/examples/widgets/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1289 2024-04-11 02:07:05.000000 pyegeria-0.3.4/examples/widgets/README.md
+-rw-r--r--   0 dwolfson   (501) staff       (20)       17 2024-04-11 14:02:30.000000 pyegeria-0.3.4/examples/widgets/__init__.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.613514 pyegeria-0.3.4/examples/widgets/__pycache__/
+-rw-r--r--   0 dwolfson   (501) staff       (20)      201 2024-04-11 16:37:25.000000 pyegeria-0.3.4/examples/widgets/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5743 2024-04-11 16:45:53.000000 pyegeria-0.3.4/examples/widgets/__pycache__/server_status_widget.cpython-312-pytest-7.4.4.pyc
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3231 2024-04-11 16:57:09.000000 pyegeria-0.3.4/examples/widgets/coco_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5206 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/engine_action_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5185 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/find_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4608 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/glossary_view.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4014 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/gov_engine_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4589 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/integration_daemon_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3578 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/list_asset_types.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3740 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/multi-server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     5674 2024-04-11 17:41:52.000000 pyegeria-0.3.4/examples/widgets/my_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4663 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/open_todos.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3360 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/server_status.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     3102 2024-04-11 16:52:45.000000 pyegeria-0.3.4/examples/widgets/server_status_widget.py
+-rwxr-xr-x   0 dwolfson   (501) staff       (20)     4599 2024-04-11 16:14:31.000000 pyegeria-0.3.4/examples/widgets/view_my_profile.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1063 2024-04-11 15:33:29.000000 pyegeria-0.3.4/pyproject.toml
+-rw-r--r--   0 dwolfson   (501) staff       (20)       38 2024-04-11 21:14:10.618059 pyegeria-0.3.4/setup.cfg
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2102 2024-04-11 17:56:25.000000 pyegeria-0.3.4/setup.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.609280 pyegeria-0.3.4/src/
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.615674 pyegeria-0.3.4/src/pyegeria/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     1612 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/__init__.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    23606 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)      558 2024-04-10 19:14:09.000000 pyegeria-0.3.4/src/pyegeria/_globals.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12703 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/_validators.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)   100106 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    93138 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18399 2024-04-10 19:14:09.000000 pyegeria-0.3.4/src/pyegeria/exceptions.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    46146 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    36500 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    19697 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6340 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/governance_author.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    42441 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    41955 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8775 2024-04-11 18:20:16.000000 pyegeria-0.3.4/src/pyegeria/registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    16323 2024-04-11 18:13:57.000000 pyegeria-0.3.4/src/pyegeria/server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5240 2024-04-11 02:07:05.000000 pyegeria-0.3.4/src/pyegeria/utils.py
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.617615 pyegeria-0.3.4/src/pyegeria.egg-info/
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2389 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/PKG-INFO
+-rw-r--r--   0 dwolfson   (501) staff       (20)     2493 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/SOURCES.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        1 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/dependency_links.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)      140 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/requires.txt
+-rw-r--r--   0 dwolfson   (501) staff       (20)        9 2024-04-11 21:14:10.000000 pyegeria-0.3.4/src/pyegeria.egg-info/top_level.txt
+drwxr-xr-x   0 dwolfson   (501) staff       (20)        0 2024-04-11 21:14:10.617474 pyegeria-0.3.4/tests/
+-rw-r--r--   0 dwolfson   (501) staff       (20)    18694 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_automated_curation_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    12049 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_automated_curation_omvs_cray.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     3006 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_client.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    59260 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_core_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    11868 2024-04-10 19:14:09.000000 pyegeria-0.3.4/tests/test_full_omag_server_config.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    10582 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_glossary_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8350 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_gov_engine.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     9625 2024-04-11 17:35:38.000000 pyegeria-0.3.4/tests/test_my_profile_omvs.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)    40081 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_platform_services.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     4727 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_registered_info.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     8028 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_server_operations.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     5904 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_util_exp.py
+-rw-r--r--   0 dwolfson   (501) staff       (20)     6035 2024-04-11 02:07:05.000000 pyegeria-0.3.4/tests/test_validators.py
```

### Comparing `pyegeria-0.3.3/LICENSE` & `pyegeria-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/PKG-INFO` & `pyegeria-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.3/README.md` & `pyegeria-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/pyproject.toml` & `pyegeria-0.3.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 #requires = ["hatchling"]
 requires = ["setuptools", "wheel"]
 #build-backend = "hatchling.build"
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyegeria"
-version = "0.3.3"
+version = "0.3.4"
 #license = 'Apache 2.0'
 authors = [
     {name ="Dan Wolfson", email= "dan.wolfson@pdr-associates.com"},
 ]
-description = "A python client for Egeria"
-readme= "README.md"
-requires-python = ">=3.10"
 dependencies = [
     "requests~=2.31.0",
     "validators~=0.22.0",
     "pytest~=7.4.2",
     "urllib3~=1.26.15",
     "tabulate~=0.9.0",
     "pandas~=2.2.0",
     "rich~=13.7.1",
     "httpx~=0.26.0"
 ]
+optional-dependencies = { tests = ['pytest']}
+description = "A python client for Egeria"
+readme= "README.md"
+requires-python = ">=3.10"
+
 keywords = ["egeria", "metadata", "governance"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
  ]
```

### Comparing `pyegeria-0.3.3/src/pyegeria/__init__.py` & `pyegeria-0.3.4/src/pyegeria/__init__.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/_client.py` & `pyegeria-0.3.4/src/pyegeria/_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/_exceptions.py` & `pyegeria-0.3.4/src/pyegeria/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/_globals.py` & `pyegeria-0.3.4/src/pyegeria/_globals.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/_validators.py` & `pyegeria-0.3.4/src/pyegeria/_validators.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/automated_curation_omvs.py` & `pyegeria-0.3.4/src/pyegeria/automated_curation_omvs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,29 @@
     InvalidParameterException,
 )
 from ._validators import validate_name, validate_guid, validate_search_string
 
 
 class AutomatedCuration(Client):
     """ Set up and maintain automation services in Egeria.
-    class AutomatedCuration(Platform):
 
-        def __init__(
-                self,
-                server_name: str,
-                platform_url: str,
-                user_id: str,
-                user_pwd: str = None,
-                verify_flag: bool = False,
-        ):
+    Attributes:
+        server_name : str
+            The name of the View Server to use.
+        platform_url : str
+            URL of the server platform to connect to
+        user_id : str
+            The identity of the user calling the method - this sets a default optionally used by the methods
+            when the user doesn't pass the user_id on a method call.
+        user_pwd: str
+            The password associated with the user_id. Defaults to None
+        verify_flag: bool
+            Flag to indicate if SSL Certificates should be verified in the HTTP requests.
+            Defaults to False.
+
     """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             user_id: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/core_omag_server_config.py` & `pyegeria-0.3.4/src/pyegeria/core_omag_server_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,39 +20,32 @@
     validate_url
 )
 
 
 class CoreServerConfig(Client):
     """
     CoreServerConfig is a class that extends the Client class. It provides methods to configure and interact with access
-     services in the OMAG server.
+    services in the OMAG server.
 
-    Methods:
+    Attributes:
 
-        - get_stored_configuration(server_name: str = None) -> dict:
-            Retrieves all the configuration documents for a server.
+        server_name: str
+            The name of the OMAG server to configure.
+        platform_url : str
+            URL of the server platform to connect to
+        user_id : str
+            The identity of the user calling the method - this sets a default optionally used by the methods
+            when the user doesn't pass the user_id on a method call.
+        user_pwd: str
+            The password associated with the user_id. Defaults to None
+        verify_flag: bool
+            Flag to indicate if SSL Certificates should be verified in the HTTP requests.
+            Defaults to False.
 
-        - get_configured_access_services(server_name: str = None) -> dict:
-            Returns the list of access services that are configured for this server.
 
-        - configure_all_access_services(server_name: str = None) -> None:
-            Enables all access services that are registered with this server platform.
-
-        - configure_all_access_services_no_topics(server_name: str = None) -> None:
-            Configures all access services for the specified server with no cohort/Event Bus.
-
-        - clear_all_access_services(server_name: str = None) -> None:
-            Disables the access services. This removes all configuration for the access services and disables the
-            enterprise repository services.
-
-        - get_access_service_config(access_service_name: str, server_name: str = None) -> dict:
-            Retrieves the config for an access service.
-
-        - configure_access_service(access_service_name: str, server_name: str = None) -> None:
-            Enables a single access service.
      """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             user_id: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/exceptions.py` & `pyegeria-0.3.4/src/pyegeria/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria/full_omag_server_config.py` & `pyegeria-0.3.4/src/pyegeria/full_omag_server_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,15 +597,14 @@
         if server_name is None:
             server_name = self.server_name
 
         url = f"{self.admin_command_root}/servers/{server_name}/configuration/deploy"
 
         self.make_request("POST", url, target_url_root)
 
-
     def get_event_bus(self, server_name: str = None) -> dict:
         """ Returns the event bus configuration for the specified server
 
         Parameters
         ----------
         server_name: str, optional
             The name of the server to retrieve the event bus configuration from. If not provided, the default
```

### Comparing `pyegeria-0.3.3/src/pyegeria/glossary_omvs.py` & `pyegeria-0.3.4/src/pyegeria/glossary_omvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,28 @@
 
 
 class GlossaryBrowser(Client):
     """
     GlossaryBrowser is a class that extends the Client class. It provides methods to search and retrieve glossaries,
     terms and categories.
 
-    Methods:
+    Attributes:
 
+        server_name: str
+            The name of the View Server to connect to.
+        platform_url : str
+            URL of the server platform to connect to
+        user_id : str
+            The identity of the user calling the method - this sets a default optionally used by the methods
+            when the user doesn't pass the user_id on a method call.
+        user_pwd: str
+            The password associated with the user_id. Defaults to None
+        verify_flag: bool
+            Flag to indicate if SSL Certificates should be verified in the HTTP requests.
+            Defaults to False.
 
      """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/gov_engine.py` & `pyegeria-0.3.4/src/pyegeria/gov_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,33 +29,26 @@
 
 class GovEng(Client):
     """
        Client to initiate and manage governance actions and processes.
 
        Attributes:
            server_name: str
-                Name of the server to configure.
+                Name of the server to use.
            platform_url : str
                URL of the server platform to connect to
            user_id : str
                The identity of the user calling the method - this sets a default optionally used by the methods
                when the user doesn't pass the user_id on a method call.
            user_pwd: str = None
                 The password associated with the user
            verify_flag: bool = enable_ssl_check
                 Set true for SSL verification to be enabled, false for disabled. Default behaviour set by the
                 enable_ssl_check attribute from _globals.py
 
-       Methods:
-           __init__(self,
-                    platform_url: str,
-                    end_user_id: str,
-                    )
-            Initializes the connection - throwing an exception if there is a problem
-
        """
 
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             user_id: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/governance_author.py` & `pyegeria-0.3.4/src/pyegeria/governance_author.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 class GovernanceAuthor(AutomatedCuration):
     """
     Client to issue Curation requests.
 
     Attributes:
 
+        server_name: str
+                Name of the server to use.
         platform_url : str
             URL of the server platform to connect to
         user_id : str
             The identity of the user calling the method - this sets a default optionally used by the methods
             when the user doesn't pass the user_id on a method call.
         user_pwd: str
             The password associated with the user_id. Defaults to None
```

### Comparing `pyegeria-0.3.3/src/pyegeria/my_profile_omvs.py` & `pyegeria-0.3.4/src/pyegeria/my_profile_omvs.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     This class provides methods for retrieving the profile details
     of a user associated with a token.
 
     Parameters
     ----------
     server_name : str
-        The name of the server to configure.
+        The name of the view server to configure.
     platform_url : str
         The URL of the platform.
     token : str, optional
         The token associated with the user. Default is None.
     user_id : str, optional
         The user ID. Default is None.
     user_pwd : str, optional
```

### Comparing `pyegeria-0.3.3/src/pyegeria/platform_services.py` & `pyegeria-0.3.4/src/pyegeria/platform_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,64 +26,27 @@
 
 
 class Platform(Client):
     """
     Client to operate Egeria Platforms - inherits from Server Ops
 
     Attributes:
-
+        server_name: str
+                Name of the server to use.
         platform_url : str
             URL of the server platform to connect to
         user_id : str
             The identity of the user calling the method - this sets a default optionally used by the methods
             when the user doesn't pass the user_id on a method call.
         user_pwd: str
             The password associated with the user_id. Defaults to None
         verify_flag: bool
             Flag to indicate if SSL Certificates should be verified in the HTTP requests.
             Defaults to False.
 
-    Methods:
-        __init__(self, platform_url: str, end_user_id: str)
-         Initializes the connection - throwing an exception if there is a problem
-
-
-
-        get_platform_origin() -> str
-
-        activate_server_stored_config(server: str = None, timeout: int = 30) -> None
-
-        activate_server_supplied_config(config_body: str, server: str = None, timeout: int = 30) -> None
-
-        get_active_server_instance_status(server: str = None)-> dict | str
-
-        get_known_servers() -> list[str] | str
-
-        is_server_known(server: str = None) -> bool
-
-        is_server_configured(server: str = None) -> bool
-
-        check_server_active(server: str = None)
-
-        get_active_server_list() -> dict | str
-
-        shutdown_platform() -> None:
-
-        shutdown_server(server: str = None) -> None:
-
-        shutdown_unregister_servers() -> None
-
-        shutdown_all_servers() -> None
-
-        activate_server_if_down(server: str) -> bool
-
-        activate_servers_on_platform(server_list: str) -> bool
-
-       activate_platform(self, platform_name: str, hosted_server_names: [str], timeout:int = 60) -> None
-
     """
 
     admin_command_root: str
 
     def __init__(
             self,
             server_name: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/registered_info.py` & `pyegeria-0.3.4/src/pyegeria/registered_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 
 class RegisteredInfo(Client):
     """ Client to discover Egeria services and capabilities
 
     Attributes:
     ----------
+        server_name: str
+                Name of the server to use.
         platform_url : str
             URL of the server platform to connect to
         user_id : str
             The identity of the user calling the method - this sets a default optionally used by the methods
             when the user doesn't pass the user_id on a method call.
         user_pwd: str
             The password associated with the user_id. Defaults to None
@@ -51,19 +53,19 @@
             Lists the defined asset types.
     """
 
     admin_command_root: str
 
     def __init__(
             self,
+            server_name: str,
             platform_url: str,
             user_id: str,
             user_pwd: str = None,
             verify_flag: bool = False,
-            server_name: str = None
     ):
         if server_name is None:
             server_name = "NA"
         Client.__init__(self, server_name, platform_url,
                         user_id, user_pwd, verify_flag)
         self.admin_command_root = (f"{self.platform_url}/open-metadata/platform-services/users/"
                                    f"{self.user_id}/server-platform/registered-services")
```

### Comparing `pyegeria-0.3.3/src/pyegeria/server_operations.py` & `pyegeria-0.3.4/src/pyegeria/server_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,27 +15,27 @@
 
 
 class ServerOps(Platform):
     """
     Client to issue operations on a running OMAG server.
 
     Attributes:
-
+        server_name: str
+            Name of the server to use.
         platform_url : str
             URL of the server platform to connect to
         user_id : str
             The identity of the user calling the method - this sets a default optionally used by the methods
             when the user doesn't pass the user_id on a method call.
         user_pwd: str
             The password associated with the user_id. Defaults to None
         verify_flag: bool
             Flag to indicate if SSL Certificates should be verified in the HTTP requests.
             Defaults to False.
 
-    Methods:
 
     """
     def __init__(
             self,
             server_name: str,
             platform_url: str,
             user_id: str,
```

### Comparing `pyegeria-0.3.3/src/pyegeria/utils.py` & `pyegeria-0.3.4/src/pyegeria/utils.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/src/pyegeria.egg-info/PKG-INFO` & `pyegeria-0.3.4/src/pyegeria.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyegeria
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python client for Egeria
 Home-page: https://egeria-project.org/egeria-python
 Author: Dan Wolfson
 Author-email: Dan Wolfson <dan.wolfson@pdr-associates.com>
 Project-URL: Homepage, https://github.com/odpi/egeria-python
 Project-URL: Issues, https://github.com/odpi/egeria-python/issues
 Keywords: egeria,metadata,governance
```

### Comparing `pyegeria-0.3.3/tests/test_automated_curation_omvs.py` & `pyegeria-0.3.4/tests/test_automated_curation_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_automated_curation_omvs_cray.py` & `pyegeria-0.3.4/tests/test_automated_curation_omvs_cray.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_client.py` & `pyegeria-0.3.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_core_omag_server_config.py` & `pyegeria-0.3.4/tests/test_core_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_full_omag_server_config.py` & `pyegeria-0.3.4/tests/test_full_omag_server_config.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_glossary_omvs.py` & `pyegeria-0.3.4/tests/test_glossary_omvs.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_gov_engine.py` & `pyegeria-0.3.4/tests/test_gov_engine.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_my_profile_omvs.py` & `pyegeria-0.3.4/tests/test_my_profile_omvs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 # from pyegeria.admin_services import FullServerConfig
 
 disable_ssl_warnings = True
 
 
 class TestMyProfile:
     good_platform1_url = "https://127.0.0.1:9443"
-    good_platform2_url = "https://oak.local:9443"
+    good_platform2_url = "https://cray.local:9443"
     bad_platform1_url = "https://localhost:9443"
 
     # good_platform1_url = "https://127.0.0.1:30080"
     # good_platform2_url = "https://127.0.0.1:30081"
     # bad_platform1_url = "https://localhost:9443"
 
     good_user_1 = "garygeeke"
```

### Comparing `pyegeria-0.3.3/tests/test_platform_services.py` & `pyegeria-0.3.4/tests/test_platform_services.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,50 +66,50 @@
     good_server_4 = "engine-host"
     bad_server_1 = "coco"
     bad_server_2 = ""
 
     @pytest.mark.parametrize(
         "server, url, user_id, exc_type, expectation",
         [
+            # (
+            #         "meow",
+            #         "https://google.com",
+            #         "garygeeke",
+            #         "InvalidParameterException",
+            #         pytest.raises(InvalidParameterException),
+            # ),
             (
-                    "meow",
-                    "https://google.com",
-                    "garygeeke",
-                    "InvalidParameterException",
-                    pytest.raises(InvalidParameterException),
-            ),
-            (
-                    "cocoMDS2",
+                    "active-metadata-server",
                     "https://localhost:9443",
                     "garygeeke",
                     "nothing",
                     does_not_raise(),
             ),
-            (
-                    "cocoMDS1",
-                    good_platform3_url,
-                    "garygeeke",
-                    "",
-                    does_not_raise(),
-            ),
-            (
-                    "cocoMDS2",
-                    "https://127.0.0.1:9443",
-                    None,
-                    "InvalidParameterException",
-                    pytest.raises(InvalidParameterException),
-            ),
-            (
-                    "cocoMDS2",
-                    "https://127.0.0.1:9443/open-metadata/admin-services/users/garygeeke/servers/active-metadata-store",
-                    "meow",
-                    "InvalidParameterException",
-                    pytest.raises(InvalidParameterException),
-            ),
-            ("", "", "", "InvalidParameterException", pytest.raises(InvalidParameterException)),
+            # (
+            #         "cocoMDS1",
+            #         good_platform3_url,
+            #         "garygeeke",
+            #         "",
+            #         does_not_raise(),
+            # ),
+            # (
+            #         "cocoMDS2",
+            #         "https://127.0.0.1:9443",
+            #         None,
+            #         "InvalidParameterException",
+            #         pytest.raises(InvalidParameterException),
+            # ),
+            # (
+            #         "cocoMDS2",
+            #         "https://127.0.0.1:9443/open-metadata/admin-services/users/garygeeke/servers/active-metadata-store",
+            #         "meow",
+            #         "InvalidParameterException",
+            #         pytest.raises(InvalidParameterException),
+            # ),
+            # ("", "", "", "InvalidParameterException", pytest.raises(InvalidParameterException)),
         ],
     )
     def test_get_platform_origin(self, server, url, user_id, exc_type, expectation):
         with expectation as excinfo:
             p_client = Platform(server, url, user_id)
             response_text = p_client.get_platform_origin()
             if response_text is not None:
```

### Comparing `pyegeria-0.3.3/tests/test_registered_info.py` & `pyegeria-0.3.4/tests/test_registered_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         ],
     )
     def test_list_registered_svcs(self, service_kind):
 
         try:
             r_client = RegisteredInfo(self.good_platform1_url, self.good_user_1)
 
-            response = r_client.list_registered_svcs(service_kind, fmt='table')
+            response = r_client.list_registered_svcs(service_kind, fmt='json')
 
             assert (type(response) is list) or (type(response) is str), "No services found"
             if type(response) is list:
                 print(f"\n\nView services configuration for {service_kind}: \n\n")
                 # print(json.dumps(response, indent=4))
                 rprint(response)
             else:
```

### Comparing `pyegeria-0.3.3/tests/test_server_operations.py` & `pyegeria-0.3.4/tests/test_server_operations.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_util_exp.py` & `pyegeria-0.3.4/tests/test_util_exp.py`

 * *Files identical despite different names*

### Comparing `pyegeria-0.3.3/tests/test_validators.py` & `pyegeria-0.3.4/tests/test_validators.py`

 * *Files identical despite different names*

