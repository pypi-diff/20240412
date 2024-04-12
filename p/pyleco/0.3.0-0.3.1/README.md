# Comparing `tmp/pyleco-0.3.0.tar.gz` & `tmp/pyleco-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyleco-0.3.0.tar", last modified: Wed Mar 13 14:49:32 2024, max compression
+gzip compressed data, was "pyleco-0.3.1.tar", last modified: Fri Apr 12 08:28:50 2024, max compression
```

## Comparing `pyleco-0.3.0.tar` & `pyleco-0.3.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.443170 pyleco-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-13 14:49:22.000000 pyleco-0.3.0/.github/pytest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-13 14:49:22.000000 pyleco-0.3.0/.github/sphinx.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-03-13 14:49:22.000000 pyleco-0.3.0/.github/workflows/pyleco_CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-13 14:49:22.000000 pyleco-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-03-13 14:49:22.000000 pyleco-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-13 14:49:22.000000 pyleco-0.3.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-13 14:49:22.000000 pyleco-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-03-13 14:49:22.000000 pyleco-0.3.0/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-13 14:49:22.000000 pyleco-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-03-13 14:49:32.443170 pyleco-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-03-13 14:49:22.000000 pyleco-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-13 14:49:22.000000 pyleco-0.3.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-03-13 14:49:22.000000 pyleco-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-03-13 14:49:22.000000 pyleco-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-13 14:49:22.000000 pyleco-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-03-13 14:49:22.000000 pyleco-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-13 14:49:22.000000 pyleco-0.3.0/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-13 14:49:22.000000 pyleco-0.3.0/examples/measurement_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-03-13 14:49:22.000000 pyleco-0.3.0/examples/pymeasure_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/pyleco/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/pyleco/actors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/actors/actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.427169 pyleco-0.3.0/pyleco/coordinators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/coordinators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/coordinators/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/coordinators/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.431170 pyleco-0.3.0/pyleco/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/internal_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/leco_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/core/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.431170 pyleco-0.3.0/pyleco/directors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/coordinator_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/data_logger_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/director.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/starter_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/directors/transparent_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.431170 pyleco-0.3.0/pyleco/json_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/json_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/rpc_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/json_utils/rpc_server_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.431170 pyleco-0.3.0/pyleco/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/management/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/management/starter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.431170 pyleco-0.3.0/pyleco/management/test_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/management/test_tasks/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/pyleco/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/base_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21601 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/coordinator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/data_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/extended_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/pipe_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/qt_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/timers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyleco/utils/zmq_log_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.439170 pyleco-0.3.0/pyleco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9401 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 14:49:32.000000 pyleco-0.3.0/pyleco.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-13 14:49:22.000000 pyleco-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 14:49:32.443170 pyleco-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/tests/acceptance_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/acceptance_tests/test_coordinator_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/acceptance_tests/test_director_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/acceptance_tests/test_proxy_server_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/acceptance_tests/test_starter_live.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/tests/actors/
--rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/actors/test_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/tests/coordinators/
--rw-r--r--   0 runner    (1001) docker     (127)    32622 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/coordinators/test_coordinator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.435170 pyleco-0.3.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/core/test_data_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/core/test_internal_protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/core/test_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/core/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.439170 pyleco-0.3.0/tests/directors/
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/directors/test_coordinator_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/directors/test_data_logger_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/directors/test_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/directors/test_starter_director.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/directors/test_transparent_director.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.439170 pyleco-0.3.0/tests/json_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/json_utils/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/json_utils/test_json_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/json_utils/test_rpc_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/json_utils/test_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.439170 pyleco-0.3.0/tests/management/
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/management/test_data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/management/test_starter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/test_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 14:49:32.439170 pyleco-0.3.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_base_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22466 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_coordinator_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_data_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_extended_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_log_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_pipe_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_qt_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-13 14:49:22.000000 pyleco-0.3.0/tests/utils/test_zmq_log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.271855 pyleco-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/pytest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/sphinx.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.271855 pyleco-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/workflows/pyleco_CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-12 08:28:40.000000 pyleco-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-12 08:28:40.000000 pyleco-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 08:28:40.000000 pyleco-0.3.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-12 08:28:40.000000 pyleco-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13960 2024-04-12 08:28:40.000000 pyleco-0.3.1/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-12 08:28:40.000000 pyleco-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-12 08:28:50.287855 pyleco-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7207 2024-04-12 08:28:40.000000 pyleco-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-12 08:28:40.000000 pyleco-0.3.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-04-12 08:28:40.000000 pyleco-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-12 08:28:40.000000 pyleco-0.3.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-12 08:28:40.000000 pyleco-0.3.1/examples/measurement_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-12 08:28:40.000000 pyleco-0.3.1/examples/pymeasure_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/actors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/actors/actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.275856 pyleco-0.3.1/pyleco/coordinators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21798 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/coordinators/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/internal_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/leco_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/core/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/directors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/coordinator_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/data_logger_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/starter_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/directors/transparent_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/json_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/json_utils/rpc_server_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/starter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.279856 pyleco-0.3.1/pyleco/management/test_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/management/test_tasks/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/pyleco/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8495 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/base_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21601 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/coordinator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/data_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/extended_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15471 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/pipe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/qt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/timers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyleco/utils/zmq_log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/pyleco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 08:28:50.000000 pyleco-0.3.1/pyleco.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 08:28:40.000000 pyleco-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:28:50.287855 pyleco-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/acceptance_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_coordinator_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_director_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_proxy_server_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/acceptance_tests/test_starter_live.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/actors/
+-rw-r--r--   0 runner    (1001) docker     (127)     9128 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/actors/test_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/coordinators/
+-rw-r--r--   0 runner    (1001) docker     (127)    33403 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/coordinators/test_coordinator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_data_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_internal_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/core/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.283856 pyleco-0.3.1/tests/directors/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_coordinator_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_data_logger_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_starter_director.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/directors/test_transparent_director.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/json_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_json_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_rpc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/json_utils/test_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/management/
+-rw-r--r--   0 runner    (1001) docker     (127)    16238 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/management/test_data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/management/test_starter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:50.287855 pyleco-0.3.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_base_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22466 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_coordinator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_data_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_extended_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26879 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_pipe_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_qt_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-12 08:28:40.000000 pyleco-0.3.1/tests/utils/test_zmq_log_handler.py
```

### Comparing `pyleco-0.3.0/.github/pytest.json` & `pyleco-0.3.1/.github/pytest.json`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/.github/sphinx.json` & `pyleco-0.3.1/.github/sphinx.json`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/.github/workflows/pyleco_CI.yml` & `pyleco-0.3.1/.github/workflows/pyleco_CI.yml`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/.github/workflows/python-publish.yml` & `pyleco-0.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/.gitignore` & `pyleco-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/CHANGELOG.md` & `pyleco-0.3.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # CHANGELOG
 
+## [0.3.1] 2024-04-12
+
+### Fixed
+
+* Fix `Coordinator` to not use period in hostname as namespace ([#69](https://github.com/pymeasure/pyleco/pull/69))
+* Fix `DataLogger` timer ([#70](https://github.com/pymeasure/pyleco/pull/70))
+
+**Full Changelog**: https://github.com/pymeasure/pyleco/compare/v0.3.0...v0.3.1
+
+
 ## [0.3.0] 2024-03-13
 
 _Use self defined objects instead of jsonrpc2-objects and jsonrpc2-pyclient._
 
 ### Changed
 
 - Rename `cls` parameter to `device_class` in `Actor` and `TransparentDirector`.
@@ -112,14 +122,15 @@
 _Initial alpha version, complies with [LECO protocol alpha-0.0.1](https://github.com/pymeasure/leco-protocol/releases/tag/alpha-0.0.1)_
 
 ### New Contributors
 
 @BenediktBurger, @bilderbuchi, @bklebel
 
 
-[unreleased]: https://github.com/pymeasure/pyleco/compare/v0.3.0...HEAD
+[unreleased]: https://github.com/pymeasure/pyleco/compare/v0.3.1...HEAD
+[0.3.1]: https://github.com/pymeasure/pyleco/releases/tag/v0.3.1
 [0.3.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.3.0
 [0.2.2]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.2
 [0.2.1]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.1
 [0.2.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.2.0
 [0.1.0]: https://github.com/pymeasure/pyleco/releases/tag/v0.1.0
 [alpha-0.0.1]: https://github.com/pymeasure/pyleco/releases/tag/alpha-0.0.1
```

### Comparing `pyleco-0.3.0/GETTING_STARTED.md` & `pyleco-0.3.1/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/LICENSE` & `pyleco-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/PKG-INFO` & `pyleco-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleco
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python reference implementation of the Laboratory Experiment COntrol (LECO) protocol
 Author: PyLECO Developers
 License: MIT License
         
         Copyright (c) 2023-2024 PyLECO Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/pymeasure/pyleco
 Project-URL: Bug Tracker, https://github.com/pymeasure/pyleco/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -56,14 +56,15 @@
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
 [![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
 [![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
 [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
 
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
```

### Comparing `pyleco-0.3.0/README.md` & `pyleco-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
 [![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
 [![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
 [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
 
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
```

### Comparing `pyleco-0.3.0/docs/Makefile` & `pyleco-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/docs/conf.py` & `pyleco-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/docs/make.bat` & `pyleco-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/examples/measurement_script.py` & `pyleco-0.3.1/examples/measurement_script.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/examples/pymeasure_actor.py` & `pyleco-0.3.1/examples/pymeasure_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/__init__.py` & `pyleco-0.3.1/pyleco/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/actors/actor.py` & `pyleco-0.3.1/pyleco/actors/actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/coordinators/coordinator.py` & `pyleco-0.3.1/pyleco/coordinators/coordinator.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         cleaning_interval: float = 5,
         expiration_time: float = 15,
         context: Optional[zmq.Context] = None,
         multi_socket: Optional[MultiSocket] = None,
         **kwargs,
     ) -> None:
         if namespace is None:
-            self.namespace = gethostname().encode()
+            self.namespace = gethostname().split(".")[0].encode()
         elif isinstance(namespace, str):
             self.namespace = namespace.encode()
         elif isinstance(namespace, bytes):
             self.namespace = namespace
         else:
             raise ValueError("`namespace` must be str or bytes or None.")
         self.full_name = self.namespace + b".COORDINATOR"
```

### Comparing `pyleco-0.3.0/pyleco/coordinators/proxy_server.py` & `pyleco-0.3.1/pyleco/coordinators/proxy_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/__init__.py` & `pyleco-0.3.1/pyleco/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/data_message.py` & `pyleco-0.3.1/pyleco/core/data_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/internal_protocols.py` & `pyleco-0.3.1/pyleco/core/internal_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/leco_protocols.py` & `pyleco-0.3.1/pyleco/core/leco_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/message.py` & `pyleco-0.3.1/pyleco/core/message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/core/serialization.py` & `pyleco-0.3.1/pyleco/core/serialization.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/directors/coordinator_director.py` & `pyleco-0.3.1/pyleco/directors/coordinator_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/directors/data_logger_director.py` & `pyleco-0.3.1/pyleco/directors/data_logger_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/directors/director.py` & `pyleco-0.3.1/pyleco/directors/director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/directors/starter_director.py` & `pyleco-0.3.1/pyleco/directors/starter_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/directors/transparent_director.py` & `pyleco-0.3.1/pyleco/directors/transparent_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/errors.py` & `pyleco-0.3.1/pyleco/errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/__init__.py` & `pyleco-0.3.1/pyleco/json_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/errors.py` & `pyleco-0.3.1/pyleco/json_utils/errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/json_objects.py` & `pyleco-0.3.1/pyleco/json_utils/json_objects.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/rpc_generator.py` & `pyleco-0.3.1/pyleco/json_utils/rpc_generator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/rpc_server.py` & `pyleco-0.3.1/pyleco/json_utils/rpc_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/json_utils/rpc_server_definition.py` & `pyleco-0.3.1/pyleco/json_utils/rpc_server_definition.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/management/data_logger.py` & `pyleco-0.3.1/pyleco/management/data_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     # For python<3.11
     from enum import Enum
 
     class StrEnum(str, Enum):  # type: ignore
         pass
 import json
 import logging
+from threading import Lock
 from typing import Any, Callable, Optional, Iterable
 
 try:
     import numpy as np  # type: ignore[import-not-found]
 except ModuleNotFoundError:
     def average(values: Sequence[Union[float, int]]) -> float:
         return sum(values) / len(values)
@@ -94,18 +95,18 @@
 
         datalogger = DataLogger()
         datalogger.listen()  # listen until a shutdown signal is received.
         # Now you may send a "start_collecting" message to start a measurement.
     """
 
     # TODO names
-    tmp: dict[str, list[Any]] = {}  # contains all values since last datapoint
-    lists: dict[str, list[Any]] = {}  # contains datapoints.
-    units: dict[str, Any] = {}  # contains the units of the variables  TODO TBD what the value is.
-    last_datapoint: dict[str, Any] = {}
+    tmp: dict[str, list[Any]]  # contains all values since last datapoint
+    lists: dict[str, list[Any]]  # contains datapoints.
+    units: dict[str, Any]  # contains the units of the variables  TODO TBD what the value is.
+    last_datapoint: dict[str, Any]
     last_save_name: str = ""
 
     # configuration variables
     trigger_type: TriggerTypes = TriggerTypes.NONE
     _last_trigger_type: TriggerTypes = TriggerTypes.NONE
     trigger_timeout: float = 1
     trigger_variable: str = ""
@@ -113,14 +114,18 @@
     valuing: Callable[[list], Any]
 
     def __init__(self, name: str = "DataLoggerN", directory: str = ".", **kwargs) -> None:
         super().__init__(name=name, **kwargs)
         self.directory = directory
         self.publisher = DataPublisher(full_name=name)
         self.valuing = average
+        # Initialize values
+        self.list_lock = Lock()
+        self.reset_data_storage()
+        self.units = {}
         # TODO add auto_save functionality?
 
     def register_rpc_methods(self) -> None:
         super().register_rpc_methods()
         self.register_rpc_method(self.set_valuing_mode)  # TODO offer during a measurement?
         self.register_rpc_method(self.start_collecting)
         self.register_rpc_method(self.save_data)
@@ -157,51 +162,57 @@
         except Exception:
             log.exception(f"Could not decode message {data_message}.")
         else:
             self.handle_subscription_data(modified_dict)
 
     def handle_subscription_data(self, data: dict[str, Any]) -> None:
         """Store `data` dict in `tmp`"""
-        for key, value in data.items():
-            try:
-                self.tmp[key].append(value)
-            except KeyError:
-                log.error(f"Got value for '{key}', but no list present.")
+        with self.list_lock:
+            for key, value in data.items():
+                try:
+                    self.tmp[key].append(value)
+                except KeyError:
+                    log.debug("Got value for '%s', but no list present.", key)
         if self.trigger_type == TriggerTypes.VARIABLE and self.trigger_variable in data.keys():
             self.make_datapoint()
 
     def make_datapoint(self) -> dict[str, Any]:
         """Store a datapoint."""
         datapoint = self.calculate_data()
         self.last_datapoint = datapoint
         if self.namespace is not None:
             self.publisher.send_data(data=self.last_datapoint)
         return datapoint
 
     def calculate_data(self) -> dict[str, Any]:
         """Calculate data for a data point and return the data point."""
         datapoint = {}
-        if 'time' in self.lists.keys():
-            now = datetime.datetime.now(datetime.timezone.utc)
-            today = datetime.datetime.combine(self.today, datetime.time(),
-                                              datetime.timezone.utc)
-            time = (now - today).total_seconds()
-            self.tmp['time'].append(time)
-        for variable, datalist in self.lists.items():
-            value = datapoint[variable] = self.calculate_single_data(variable, self.tmp[variable])
-            datalist.append(value)
-        for key in self.tmp.keys():
-            self.tmp[key].clear()
-        return datapoint
+        with self.list_lock:
+            if 'time' in self.lists.keys():
+                now = datetime.datetime.now(datetime.timezone.utc)
+                today = datetime.datetime.combine(
+                    self.today, datetime.time(), datetime.timezone.utc
+                )
+                time = (now - today).total_seconds()
+                self.tmp['time'].append(time)
+            for variable, datalist in self.lists.items():
+                value = datapoint[variable] = self.calculate_single_data(
+                    variable, self.tmp[variable]
+                )
+                datalist.append(value)
+            for key in self.tmp.keys():
+                self.tmp[key].clear()
+            return datapoint
 
     def calculate_single_data(self, variable: str, tmp: list):
         if tmp:
             value = self.valuing(tmp)
         elif self.value_repeating:
             try:
+                # no lock, as this method is called in in a locked environment!
                 value = self.lists[variable][-1]
             except (KeyError, IndexError):  # No last value present.
                 value = nan
         else:
             value = nan
         return value
 
@@ -232,22 +243,22 @@
         """
         self.stop_collecting()
         log.info(f"Start collecting data. Trigger: {trigger_type}, {trigger_timeout}, "
                  f"{trigger_variable}; subscriptions: {variables}")
         self.today = datetime.datetime.now(datetime.timezone.utc).date()
         self.trigger_type = trigger_type or self._last_trigger_type
         self._last_trigger_type = self.trigger_type
-        if self.trigger_type == TriggerTypes.TIMER:
-            self.start_timer_trigger()
         if trigger_timeout is not None:
             self.trigger_timeout = trigger_timeout
         if trigger_variable is not None:
             self.trigger_variable = trigger_variable
         if value_repeating is not None:
             self.value_repeating = value_repeating
+        if self.trigger_type == TriggerTypes.TIMER:
+            self.start_timer_trigger(timeout=self.trigger_timeout)
         self.set_valuing_mode(valuing_mode=valuing_mode)
         self.setup_variables(self.lists.keys() if variables is None else variables)
         self.units = units if units else {}
 
     def setup_variables(self, variables: Iterable[str]) -> None:
         """Subscribe to the variables."""
         self.reset_data_storage()
@@ -263,26 +274,28 @@
                         continue
                     parts.insert(0, self.namespace)
                     variable = ".".join(parts)
                 subscriptions.add(".".join(parts[:2]))
             else:
                 # old style: topic is variable name
                 subscriptions.add(variable)
-            self.lists[variable] = []
-            self.tmp[variable] = []
+            with self.list_lock:
+                self.lists[variable] = []
+                self.tmp[variable] = []
         self.subscribe(topics=subscriptions)
 
     def reset_data_storage(self) -> None:
         """Reset the data storage."""
-        self.tmp = {}
-        self.lists = {}
+        with self.list_lock:
+            self.tmp = {}
+            self.lists = {}
         self.last_datapoint = {}
 
-    def start_timer_trigger(self) -> None:
-        self.timer = RepeatingTimer(self.trigger_timeout, self.make_datapoint)
+    def start_timer_trigger(self, timeout: float) -> None:
+        self.timer = RepeatingTimer(timeout, self.make_datapoint)
         self.timer.start()
 
     def set_valuing_mode(self, valuing_mode: Optional[ValuingModes]) -> None:
         if valuing_mode == ValuingModes.LAST:
             self.valuing = self.last
         elif valuing_mode == ValuingModes.AVERAGE:
             self.valuing = average
@@ -309,16 +322,17 @@
             'today': self.today.isoformat(),
             'file_name': file_name,
             'logger_name': self.full_name,
             'configuration': self.get_configuration(),
             # 'user': self.user_data,  # user stored meta data
         })
         try:
-            with open(f"{folder}/{file_name}.json", 'w') as file:
-                json.dump(obj=(header, self.lists, meta), fp=file)
+            with self.list_lock:
+                with open(f"{folder}/{file_name}.json", 'w') as file:
+                    json.dump(obj=(header, self.lists, meta), fp=file)
         except TypeError as exc:
             log.exception("Some type error during saving occurred.", exc_info=exc)
             raise
         except PermissionError as exc:
             log.exception(f"Writing permission denied for '{folder}'.", exc_info=exc)
             raise
         else:
@@ -346,31 +360,33 @@
         config['trigger_timeout'] = self.trigger_timeout
         config['trigger_variable'] = self.trigger_variable
         # Value
         vm = ValuingModes.LAST if self.valuing == self.last else ValuingModes.AVERAGE
         config['valuing_mode'] = vm.value
         config['value_repeating'] = self.value_repeating
         # Header and Variables.
-        config['variables'] = list(self.lists.keys())
+        with self.list_lock:
+            config['variables'] = list(self.lists.keys())
         config['units'] = self.units
         # config['autoSave'] = self.actionAutoSave.isChecked()
         return config
 
     def get_last_datapoint(self) -> dict[str, Any]:
         """Read the last datapoint."""
         return self.last_datapoint
 
     def get_last_save_name(self) -> Union[str, None]:
         """Return the name of the last save."""
         return self.last_save_name
 
     def get_list_length(self) -> int:
         """Return the length of the lists."""
-        length = len(self.lists[list(self.lists.keys())[0]]) if self.lists else 0
-        return length
+        with self.list_lock:
+            length = len(self.lists[list(self.lists.keys())[0]]) if self.lists else 0
+            return length
 
 
 def main() -> None:
     """Start a datalogger at script execution."""
     parser.description = "Log data."
     parser.add_argument("-d", "--directory",
                         help="set the directory to save the data to")
```

### Comparing `pyleco-0.3.0/pyleco/management/starter.py` & `pyleco-0.3.1/pyleco/management/starter.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/management/test_tasks/test_task.py` & `pyleco-0.3.1/pyleco/management/test_tasks/test_task.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/test.py` & `pyleco-0.3.1/pyleco/test.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/base_communicator.py` & `pyleco-0.3.1/pyleco/utils/base_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/communicator.py` & `pyleco-0.3.1/pyleco/utils/communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/coordinator_utils.py` & `pyleco-0.3.1/pyleco/utils/coordinator_utils.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/data_publisher.py` & `pyleco-0.3.1/pyleco/utils/data_publisher.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/events.py` & `pyleco-0.3.1/pyleco/utils/events.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/extended_message_handler.py` & `pyleco-0.3.1/pyleco/utils/extended_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/listener.py` & `pyleco-0.3.1/pyleco/utils/listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/log_levels.py` & `pyleco-0.3.1/pyleco/utils/log_levels.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/message_handler.py` & `pyleco-0.3.1/pyleco/utils/message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/parser.py` & `pyleco-0.3.1/pyleco/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/pipe_handler.py` & `pyleco-0.3.1/pyleco/utils/pipe_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/qt_listener.py` & `pyleco-0.3.1/pyleco/utils/qt_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/timers.py` & `pyleco-0.3.1/pyleco/utils/timers.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco/utils/zmq_log_handler.py` & `pyleco-0.3.1/pyleco/utils/zmq_log_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyleco.egg-info/PKG-INFO` & `pyleco-0.3.1/pyleco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyleco
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python reference implementation of the Laboratory Experiment COntrol (LECO) protocol
 Author: PyLECO Developers
 License: MIT License
         
         Copyright (c) 2023-2024 PyLECO Developers
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,15 +24,15 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/pymeasure/pyleco
 Project-URL: Bug Tracker, https://github.com/pymeasure/pyleco/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -56,14 +56,15 @@
 
 Note: LECO is still under development, such that the code and API might change.
 The LECO protocol branch [pyleco-state](https://github.com/pymeasure/leco-protocol/tree/pyleco-state) contains the assumptions used in this project, which are not yet accepted into the LECO main branch.
 These things might change, if LECO defines them differently.
 
 [![codecov](https://codecov.io/gh/pymeasure/pyleco/graph/badge.svg?token=9OB3GWDLRB)](https://codecov.io/gh/pymeasure/pyleco)
 [![pypi release](https://img.shields.io/pypi/v/pyleco.svg)](https://pypi.org/project/pyleco/)
+[![DOI](https://zenodo.org/badge/594982645.svg)](https://zenodo.org/doi/10.5281/zenodo.10837366)
 [![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
 
 For a tutorial on how to get started, see [GETTING_STARTED.md](https://github.com/pymeasure/pyleco/blob/main/GETTING_STARTED.md).
 
 
 ## Quick Start
```

### Comparing `pyleco-0.3.0/pyleco.egg-info/SOURCES.txt` & `pyleco-0.3.1/pyleco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/pyproject.toml` & `pyleco-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dynamic = ["version"]
 
 description = "Python reference implementation of the Laboratory Experiment COntrol (LECO) protocol"
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: System :: Networking",
 ]
```

### Comparing `pyleco-0.3.0/tests/acceptance_tests/test_coordinator_live.py` & `pyleco-0.3.1/tests/acceptance_tests/test_coordinator_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/acceptance_tests/test_director_actor.py` & `pyleco-0.3.1/tests/acceptance_tests/test_director_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/acceptance_tests/test_proxy_server_live.py` & `pyleco-0.3.1/tests/acceptance_tests/test_proxy_server_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/acceptance_tests/test_starter_live.py` & `pyleco-0.3.1/tests/acceptance_tests/test_starter_live.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/actors/test_actor.py` & `pyleco-0.3.1/tests/actors/test_actor.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/coordinators/test_coordinator.py` & `pyleco-0.3.1/tests/coordinators/test_coordinator.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,18 +34,19 @@
 from pyleco.core.leco_protocols import ExtendedComponentProtocol, Protocol, CoordinatorProtocol
 from pyleco.utils.coordinator_utils import FakeMultiSocket, FakeNode
 from pyleco.json_utils.rpc_generator import RPCGenerator
 from pyleco.test import FakeContext
 from pyleco.utils.events import SimpleEvent
 
 from pyleco.coordinators.coordinator import Coordinator
+from pyleco.coordinators import coordinator as coordinator_module  # type: ignore
 
 
 @pytest.fixture
-def coordinator():
+def coordinator() -> Coordinator:
     coordinator = Coordinator(namespace="N1", host="N1host", cleaning_interval=1e5,
                               context=FakeContext(),  # type: ignore
                               multi_socket=FakeMultiSocket()
                               )
     d = coordinator.directory
     d.add_component(b"send", b"321")
     d.add_component(b"rec", b"123")
@@ -57,32 +58,32 @@
     n2 = coordinator.directory.get_node(b"N2")
     n2._messages_sent = []  # type: ignore # reset dealer sock._socket.
     n2.heartbeat = -1
     coordinator.sock._messages_sent = []  # type: ignore  # reset router sock._socket:
     return coordinator
 
 
-def fake_perf_counter():
+def fake_perf_counter() -> float:
     return 0.
 
 
 @pytest.fixture()
-def fake_counting(monkeypatch):
+def fake_counting(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr("pyleco.utils.coordinator_utils.perf_counter", fake_perf_counter)
 
 
 cid = b"conversation_id;"
 
 
-def fake_generate_cid():
+def fake_generate_cid() -> bytes:
     return cid
 
 
 @pytest.fixture(autouse=True)
-def fake_cid_generation(monkeypatch):
+def fake_cid_generation(monkeypatch: pytest.MonkeyPatch) -> None:
     monkeypatch.setattr("pyleco.core.serialization.generate_conversation_id", fake_generate_cid)
 
 
 class ExtendedCoordinator(CoordinatorProtocol, ExtendedComponentProtocol, Protocol):
     pass
 
 
@@ -105,17 +106,32 @@
     def test_method_is_available(self, component_methods, method):
         for m in component_methods:
             if m.get('name') == method:
                 return
         raise AssertionError(f"Method {method} is not available.")
 
 
-def test_coordinator_set_namespace_from_hostname():
-    coordinator = Coordinator(context=FakeContext())  # type: ignore
-    assert isinstance(coordinator.namespace, bytes)
+class Test_coordinator_set_namespace_from_hostname:
+    @pytest.fixture
+    def namespace(self) -> bytes:
+        coordinator = Coordinator(context=FakeContext())  # type: ignore
+        return coordinator.namespace
+
+    def test_namespace_is_bytes(self, namespace):
+        assert isinstance(namespace, bytes)
+
+    def test_namespace_without_periods(self, namespace):
+        assert b"." not in namespace
+
+    def test_namespace_from_hostname_with_periods(self, monkeypatch: pytest.MonkeyPatch):
+        def fake_gethostname() -> str:
+            return "hostname.domain.tld"
+        monkeypatch.setattr(coordinator_module, "gethostname", fake_gethostname)
+        coordinator = Coordinator(context=FakeContext())  # type: ignore
+        assert coordinator.namespace == b"hostname"
 
 
 def test_coordinator_set_namespace_bytes():
     coordinator = Coordinator(namespace=b"test", context=FakeContext())  # type: ignore
     assert coordinator.namespace == b"test"
```

### Comparing `pyleco-0.3.0/tests/core/test_data_message.py` & `pyleco-0.3.1/tests/core/test_data_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/core/test_internal_protocols.py` & `pyleco-0.3.1/tests/core/test_internal_protocols.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/core/test_message.py` & `pyleco-0.3.1/tests/core/test_message.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/core/test_serialization.py` & `pyleco-0.3.1/tests/core/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/directors/test_coordinator_director.py` & `pyleco-0.3.1/tests/directors/test_coordinator_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/directors/test_data_logger_director.py` & `pyleco-0.3.1/tests/directors/test_data_logger_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/directors/test_director.py` & `pyleco-0.3.1/tests/directors/test_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/directors/test_starter_director.py` & `pyleco-0.3.1/tests/directors/test_starter_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/directors/test_transparent_director.py` & `pyleco-0.3.1/tests/directors/test_transparent_director.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/json_utils/test_errors.py` & `pyleco-0.3.1/tests/json_utils/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/json_utils/test_json_objects.py` & `pyleco-0.3.1/tests/json_utils/test_json_objects.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/json_utils/test_rpc_generator.py` & `pyleco-0.3.1/tests/json_utils/test_rpc_generator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/json_utils/test_rpc_server.py` & `pyleco-0.3.1/tests/json_utils/test_rpc_server.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/management/test_data_logger.py` & `pyleco-0.3.1/tests/management/test_data_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,26 +77,27 @@
             assert key in data_logger_sc.lists.keys()
 
 
 def test_start_collecting_starts_timer(data_logger: DataLogger):
     # arrange
     data_logger.trigger_timeout = 1000
     # act
-    data_logger.start_collecting(trigger_type=TriggerTypes.TIMER)
+    data_logger.start_collecting(trigger_type=TriggerTypes.TIMER, trigger_timeout=500)
     # assert
-    assert data_logger.timer.interval == 1000
+    assert data_logger.timer.interval == 500
     # cleanup
     data_logger.timer.cancel()
 
 
 def test_start_collecting_starts_timer_even_second_time(data_logger: DataLogger):
     """Even a second time, without explicit trigger type, the timer should be started."""
     # arrange
-    data_logger.trigger_timeout = 1000
-    data_logger.start_collecting(trigger_type=TriggerTypes.TIMER)  # first time, to set type
+    data_logger.trigger_timeout = 500
+    # first time, to set type
+    data_logger.start_collecting(trigger_type=TriggerTypes.TIMER, trigger_timeout=1000)
     data_logger.stop_collecting()
     assert not hasattr(data_logger, "timer")  # no timer left
     # act
     data_logger.start_collecting()
     # assert
     assert data_logger.timer.interval == 1000
     # cleanup
@@ -207,29 +208,29 @@
     data_logger.make_datapoint = MagicMock()  # type: ignore[method-assign]
     data_logger.handle_subscription_data({"test": 5})
     data_logger.make_datapoint.assert_called_once()
 
 
 def test_handle_subscription_data_without_list(data_logger: DataLogger,
                                                caplog: pytest.LogCaptureFixture):
+    caplog.set_level(0)
     data_logger.handle_subscription_data({'not_present': 42})
     assert caplog.messages == ["Got value for 'not_present', but no list present."]
 
 
 def test_set_publisher_name(data_logger: DataLogger):
     data_logger.set_full_name("N1.cA")
     assert data_logger.publisher.full_name == "N1.cA"
     assert data_logger.full_name == "N1.cA"
 
 
 class Test_start_timer_trigger:
     @pytest.fixture
     def data_logger_stt(self, data_logger: DataLogger):
-        data_logger.trigger_timeout = 1000
-        data_logger.start_timer_trigger()
+        data_logger.start_timer_trigger(1000)
         yield data_logger
         data_logger.timer.cancel()
 
     def test_timer_interval(self, data_logger_stt: DataLogger):
         assert data_logger_stt.timer.interval == 1000
 
     def test_timer_started(self, data_logger_stt: DataLogger):
@@ -338,18 +339,31 @@
         assert result is not None
 
     @pytest.fixture
     def saved_file(self, data_logger_sd: DataLogger):
         path = Path(data_logger_sd.directory) / data_logger_sd.last_save_name
         return path.with_suffix(".json").read_text()
 
-    @pytest.mark.xfail(True, reason="Not yet date recognition implemented.")
     def test_output(self, saved_file: str):
-        # TODO make date comparison work.
-        assert saved_file == """["", {"time": [], "test": [], "2": [], "N1.sender.var": []}, {"units": {}, "today": "2023-11-27", "file_name": "2023_11_27T15_07_06", "logger_name": "DataLoggerN", "configuration": {"trigger": "variable", "triggerVariable": "test", "trigger_variable": "test", "valuing_mode": "mean", "valueRepeat": false, "value_repeating": false, "variables": "time test 2 N1.sender.var"}}]"""  # noqa
+        today_string = self.today.isoformat()
+        assert saved_file == "".join(
+            (
+                """["", {"time": [], "test": [], "2": [], "N1.sender.var": []}, """,
+                '''{"units": {}, "today": "''',
+                today_string,
+                '''", "file_name": "''',
+                self.file_name,
+                """", "logger_name": "DataLoggerN", """,
+                """"configuration": {"trigger_type": "variable", "trigger_timeout": 10, """,
+                """"trigger_variable": "test", "valuing_mode": "average", """,
+                """"value_repeating": false, """,
+                """"variables": ["time", "test", "2", "N1.sender.var"], """,
+                """"units": {}}}]""",
+            )
+        )
 
     def test_json_content(self, saved_file: str):
         today_string = self.today.isoformat()
         assert json.loads(saved_file) == [
             "",
             {"time": [], "test": [], "2": [], "N1.sender.var": []},
             {"units": {}, "today": today_string, "file_name": self.file_name,
```

### Comparing `pyleco-0.3.0/tests/management/test_starter.py` & `pyleco-0.3.1/tests/management/test_starter.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/test_test.py` & `pyleco-0.3.1/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_base_communicator.py` & `pyleco-0.3.1/tests/utils/test_base_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_communicator.py` & `pyleco-0.3.1/tests/utils/test_communicator.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_coordinator_utils.py` & `pyleco-0.3.1/tests/utils/test_coordinator_utils.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_data_publisher.py` & `pyleco-0.3.1/tests/utils/test_data_publisher.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_extended_message_handler.py` & `pyleco-0.3.1/tests/utils/test_extended_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_listener.py` & `pyleco-0.3.1/tests/utils/test_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_log_levels.py` & `pyleco-0.3.1/tests/utils/test_log_levels.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_message_handler.py` & `pyleco-0.3.1/tests/utils/test_message_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_parser.py` & `pyleco-0.3.1/tests/utils/test_parser.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_pipe_handler.py` & `pyleco-0.3.1/tests/utils/test_pipe_handler.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_qt_listener.py` & `pyleco-0.3.1/tests/utils/test_qt_listener.py`

 * *Files identical despite different names*

### Comparing `pyleco-0.3.0/tests/utils/test_zmq_log_handler.py` & `pyleco-0.3.1/tests/utils/test_zmq_log_handler.py`

 * *Files identical despite different names*

