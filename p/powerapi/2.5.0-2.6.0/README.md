# Comparing `tmp/powerapi-2.5.0.tar.gz` & `tmp/powerapi-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerapi-2.5.0.tar", last modified: Thu Mar 28 13:02:33 2024, max compression
+gzip compressed data, was "powerapi-2.6.0.tar", last modified: Fri Apr 12 14:58:20 2024, max compression
```

## Comparing `powerapi-2.5.0.tar` & `powerapi-2.6.0.tar`

### file list

```diff
@@ -1,109 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.808157 powerapi-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 13:02:29.000000 powerapi-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-03-28 13:02:33.808157 powerapi-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-03-28 13:02:29.000000 powerapi-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-28 13:02:29.000000 powerapi-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:02:33.808157 powerapi-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.788156 powerapi-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.792156 powerapi-2.5.0/src/powerapi/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.792156 powerapi-2.5.0/src/powerapi/actor/
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/actor/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/actor/socket_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/actor/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/actor/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.796157 powerapi-2.5.0/src/powerapi/backend_supervisor/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/backend_supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/backend_supervisor/backend_supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.796157 powerapi-2.5.0/src/powerapi/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/binding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/common_cli_parsing_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    33426 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/cli/parsing_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.796157 powerapi-2.5.0/src/powerapi/database/
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/base_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/csvdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/file_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/influxdb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/opentsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/prometheus_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/socket_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/database/virtiofs_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/dispatch_rule/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatch_rule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatch_rule/dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatch_rule/hwpc_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatch_rule/power_dispatch_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatch_rule/procfs_dispatch_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatcher/blocking_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatcher/dispatcher_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatcher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/dispatcher/route_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/filter/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/formula/
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/formula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/formula/abstract_cpu_dram_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/formula/formula_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/formula/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/handler/
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/handler/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/handler/poison_pill_message_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/handler/start_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/processor/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.800156 powerapi-2.5.0/src/powerapi/processor/pre/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/processor/pre/k8s/
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/metadata_cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/k8s/monitor_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/processor/pre/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/processor/processor_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/puller/
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/puller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/puller/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/puller/puller_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/pusher/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/pusher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/pusher/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/pusher/pusher_actor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/report/
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/control_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/formula_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/hwpc_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/power_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/procfs_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.804157 powerapi-2.5.0/src/powerapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/utils/json_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/utils/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-28 13:02:29.000000 powerapi-2.5.0/src/powerapi/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:02:33.808157 powerapi-2.5.0/src/powerapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-03-28 13:02:33.000000 powerapi-2.5.0/src/powerapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-03-28 13:02:33.000000 powerapi-2.5.0/src/powerapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:02:33.000000 powerapi-2.5.0/src/powerapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-28 13:02:33.000000 powerapi-2.5.0/src/powerapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-28 13:02:33.000000 powerapi-2.5.0/src/powerapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.957938 powerapi-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-12 14:58:14.000000 powerapi-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-12 14:58:20.957938 powerapi-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-12 14:58:14.000000 powerapi-2.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-12 14:58:14.000000 powerapi-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:58:20.957938 powerapi-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.941938 powerapi-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.941938 powerapi-2.6.0/src/powerapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.945938 powerapi-2.6.0/src/powerapi/actor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12256 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/actor/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10204 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/actor/socket_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/actor/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/actor/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.945938 powerapi-2.6.0/src/powerapi/backend_supervisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/backend_supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/backend_supervisor/backend_supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.945938 powerapi-2.6.0/src/powerapi/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/binding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18834 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/common_cli_parsing_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33443 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16798 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/cli/parsing_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.945938 powerapi-2.6.0/src/powerapi/database/
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/base_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/csvdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/file_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/influxdb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/opentsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6198 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/prometheus_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/socket_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/database/virtiofs_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/dispatch_rule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatch_rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatch_rule/dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatch_rule/hwpc_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatch_rule/power_dispatch_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatch_rule/procfs_dispatch_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatcher/blocking_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatcher/dispatcher_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatcher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/dispatcher/route_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/filter/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/formula/
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/formula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/formula/abstract_cpu_dram_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/formula/formula_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/formula/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/handler/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/handler/poison_pill_message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/handler/start_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/processor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.949938 powerapi-2.6.0/src/powerapi/processor/pre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/processor/pre/k8s/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/metadata_cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/k8s/monitor_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/processor/pre/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/processor/processor_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/puller/
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/puller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7402 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/puller/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/puller/puller_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/pusher/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/pusher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/pusher/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/pusher/pusher_actor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/report/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/control_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/formula_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/hwpc_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8289 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/power_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/procfs_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4252 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/utils/json_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-12 14:58:14.000000 powerapi-2.6.0/src/powerapi/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:58:20.953938 powerapi-2.6.0/src/powerapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-04-12 14:58:20.000000 powerapi-2.6.0/src/powerapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-12 14:58:20.000000 powerapi-2.6.0/src/powerapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:58:20.000000 powerapi-2.6.0/src/powerapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-12 14:58:20.000000 powerapi-2.6.0/src/powerapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 14:58:20.000000 powerapi-2.6.0/src/powerapi.egg-info/top_level.txt
```

### Comparing `powerapi-2.5.0/LICENSE` & `powerapi-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/PKG-INFO` & `powerapi-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.5.0
+Version: 2.6.0
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyzmq>=18.1.0
 Requires-Dist: setproctitle>=1.1.8
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.1; extra == "test"
 Requires-Dist: pytest-asyncio>=0.20.1; extra == "test"
@@ -80,34 +78,42 @@
 
 ## Contributing
 If you would like to contribute code you can do so through GitHub by forking the repository and sending a pull request.
 
 When submitting code, please make every effort to [follow existing conventions and style](CONTRIBUTING.md) in order to keep the code as readable as possible.
 
 ## Publications
-* **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2021, Melbourne, Australia
-* **[Power Budgeting of Big Data Applications in Container-based Clusters](https://hal.inria.fr/hal-02904300)**: J. Enes, G. Fieni, R. Expósito, R. Rouvoy, J. Tourino. *IEEE Cluster*, September 2020, Kobe, Japan
-* **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2020, Melbourne, Australia
-* **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379)**: Z. Ournani, M.C. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. *ACM/SPEC International Conference on Performance Engineering* (ICPE). April 2020, Edmonton, Canada
-* **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). April 2017, Spain, France
-* **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. *European Conference on Computer Systems* (EuroSys). April 2015, Bordeaux, France
-* **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. *Journal of Automated Software Engineering*, Springer, 2015
-* **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. *International Symposium On Applied Computing* (SAC), March 2014, Gyeongju, South Korea
-* **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. *J'innove en Nord Pas de Calais*, [NFID](http://www.jinnove.com)
-* **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. *ERCIM News, Special Theme: Smart Energy Systems*, 92,  pp.43-44. [ERCIM](http://www.ercim.eu), 2013
-* **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. *01 Business & Technologies*, 2013
-* **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. *ACM SIGOPS Operating Systems Review*, ACM, 2013, 47 (3)
-* **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Conference on Automated Software Engineering* (ASE), September 2012, Essen, Germany
-* **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Workshop on Green and Sustainable Software* (GREENS), June 2012, Zurich, Switzerland
+- **[Evaluating the Impact of Java Virtual Machines on Energy Consumption](https://hal.inria.fr/hal-03275286v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat. _15th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement_ (ESEM). October 2021, Bari, Italy.
+- **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2021). May 2021, Melbourne, Australia.
+- **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2020). May 2020, Melbourne, Australia.
+- **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. _11th ACM/SPEC International Conference on Performance Engineering_ (ICPE'2020). April 2020, Edmonton, Canada.
+- **[The Next 700 CPU Power Models](https://hal.inria.fr/hal-01827132v2)**: M. Colmant, R. Rouvoy, M. Kurpicz, A. Sobe, P. Felber, L. Seinturier. _Elsevier Journal of Systems and Software_ (JSS). 144(10):382-396, Elsevier.
+- **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. _IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing_ (CCGrid). April 2017, Spain, France. pp.1-14.
+- **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. _European Conference on Computer Systems_ (EuroSys). April 2015, Bordeaux, France. pp.1-14.
+- **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. _Journal of Automated Software Engineering_, Springer, 2015, pp.1-42.
+- **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. _International Symposium On Applied Computing_ (SAC), March 2014, Gyeongju, South Korea. pp.1200-1205.
+- **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. _J'innove en Nord Pas de Calais_, [NFID](http://www.jinnove.com), 2013.
+- **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. _ERCIM News, Special Theme: Smart Energy Systems_, 92, pp.43-44. [ERCIM](http://www.ercim.eu), 2013.
+- **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. _01 Business & Technologies_, 2013.
+- **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. _ACM SIGOPS Operating Systems Review_, ACM, 2013, 47 (3), pp.42-49.
+- **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Conference on Automated Software Engineering_ (ASE), September 2012, Essen, Germany. pp.160-169.
+- **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Workshop on Green and Sustainable Software_ (GREENS), June 2012, Zurich, Switzerland. pp.21-27.
 
 ## Use Cases
 PowerAPI is used in a variety of projects to address key challenges of GreenIT:
 * [SmartWatts](https://github.com/powerapi-ng/smartwatts-formula) is a self-adaptive power meter that can estimate the energy consumption of software containers in real-time.
 * [GenPack](https://hal.inria.fr/hal-01403486) provides a container scheduling strategy to minimize the energy footprint of cloud infrastructures.
 * [VirtualWatts](https://github.com/powerapi-ng/virtualwatts-formula) provides process-level power estimation of applications running in virtual machines.
 * [Web Energy Archive](http://webenergyarchive.com) ranks popular websites based on the energy footpring they imposes to browsers.
 * [Greenspector](https://greenspector.com) optimises the power consumption of software by identifying potential energy leaks in the source code.
 
+## Research Projects
+
+Currently, PowerAPI is used in two research projects:
+
+- [Distiller ANR Project](https://www.davidson.fr/blog/comment-reduire-limpact-environnemental-des-applications-cloud-davidson-consulting-inria-ovhcloud-orange-sassocient-pour-le-programme-de-recherche-distiller) that searches to reduce energy consumption of Cloud applications.
+- [Défi Pulse](https://www.inria.fr/fr/pulse-defi-qarnot-computing-ademe-calcul-intensif-hpc-environnement) studies how to valorize emissions from High Performance Computing (HPC) using as use case [Qarnot Computing's](https://qarnot.com/en) offers.
+
 ## License
 PowerAPI is licensed under the BSD-3-Clause License. See the [LICENSE](LICENSE) file for details.
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi?ref=badge_large)
```

### Comparing `powerapi-2.5.0/README.md` & `powerapi-2.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,34 +22,42 @@
 
 ## Contributing
 If you would like to contribute code you can do so through GitHub by forking the repository and sending a pull request.
 
 When submitting code, please make every effort to [follow existing conventions and style](CONTRIBUTING.md) in order to keep the code as readable as possible.
 
 ## Publications
-* **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2021, Melbourne, Australia
-* **[Power Budgeting of Big Data Applications in Container-based Clusters](https://hal.inria.fr/hal-02904300)**: J. Enes, G. Fieni, R. Expósito, R. Rouvoy, J. Tourino. *IEEE Cluster*, September 2020, Kobe, Japan
-* **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2020, Melbourne, Australia
-* **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379)**: Z. Ournani, M.C. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. *ACM/SPEC International Conference on Performance Engineering* (ICPE). April 2020, Edmonton, Canada
-* **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). April 2017, Spain, France
-* **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. *European Conference on Computer Systems* (EuroSys). April 2015, Bordeaux, France
-* **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. *Journal of Automated Software Engineering*, Springer, 2015
-* **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. *International Symposium On Applied Computing* (SAC), March 2014, Gyeongju, South Korea
-* **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. *J'innove en Nord Pas de Calais*, [NFID](http://www.jinnove.com)
-* **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. *ERCIM News, Special Theme: Smart Energy Systems*, 92,  pp.43-44. [ERCIM](http://www.ercim.eu), 2013
-* **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. *01 Business & Technologies*, 2013
-* **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. *ACM SIGOPS Operating Systems Review*, ACM, 2013, 47 (3)
-* **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Conference on Automated Software Engineering* (ASE), September 2012, Essen, Germany
-* **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Workshop on Green and Sustainable Software* (GREENS), June 2012, Zurich, Switzerland
+- **[Evaluating the Impact of Java Virtual Machines on Energy Consumption](https://hal.inria.fr/hal-03275286v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat. _15th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement_ (ESEM). October 2021, Bari, Italy.
+- **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2021). May 2021, Melbourne, Australia.
+- **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2020). May 2020, Melbourne, Australia.
+- **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. _11th ACM/SPEC International Conference on Performance Engineering_ (ICPE'2020). April 2020, Edmonton, Canada.
+- **[The Next 700 CPU Power Models](https://hal.inria.fr/hal-01827132v2)**: M. Colmant, R. Rouvoy, M. Kurpicz, A. Sobe, P. Felber, L. Seinturier. _Elsevier Journal of Systems and Software_ (JSS). 144(10):382-396, Elsevier.
+- **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. _IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing_ (CCGrid). April 2017, Spain, France. pp.1-14.
+- **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. _European Conference on Computer Systems_ (EuroSys). April 2015, Bordeaux, France. pp.1-14.
+- **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. _Journal of Automated Software Engineering_, Springer, 2015, pp.1-42.
+- **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. _International Symposium On Applied Computing_ (SAC), March 2014, Gyeongju, South Korea. pp.1200-1205.
+- **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. _J'innove en Nord Pas de Calais_, [NFID](http://www.jinnove.com), 2013.
+- **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. _ERCIM News, Special Theme: Smart Energy Systems_, 92, pp.43-44. [ERCIM](http://www.ercim.eu), 2013.
+- **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. _01 Business & Technologies_, 2013.
+- **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. _ACM SIGOPS Operating Systems Review_, ACM, 2013, 47 (3), pp.42-49.
+- **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Conference on Automated Software Engineering_ (ASE), September 2012, Essen, Germany. pp.160-169.
+- **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Workshop on Green and Sustainable Software_ (GREENS), June 2012, Zurich, Switzerland. pp.21-27.
 
 ## Use Cases
 PowerAPI is used in a variety of projects to address key challenges of GreenIT:
 * [SmartWatts](https://github.com/powerapi-ng/smartwatts-formula) is a self-adaptive power meter that can estimate the energy consumption of software containers in real-time.
 * [GenPack](https://hal.inria.fr/hal-01403486) provides a container scheduling strategy to minimize the energy footprint of cloud infrastructures.
 * [VirtualWatts](https://github.com/powerapi-ng/virtualwatts-formula) provides process-level power estimation of applications running in virtual machines.
 * [Web Energy Archive](http://webenergyarchive.com) ranks popular websites based on the energy footpring they imposes to browsers.
 * [Greenspector](https://greenspector.com) optimises the power consumption of software by identifying potential energy leaks in the source code.
 
+## Research Projects
+
+Currently, PowerAPI is used in two research projects:
+
+- [Distiller ANR Project](https://www.davidson.fr/blog/comment-reduire-limpact-environnemental-des-applications-cloud-davidson-consulting-inria-ovhcloud-orange-sassocient-pour-le-programme-de-recherche-distiller) that searches to reduce energy consumption of Cloud applications.
+- [Défi Pulse](https://www.inria.fr/fr/pulse-defi-qarnot-computing-ademe-calcul-intensif-hpc-environnement) studies how to valorize emissions from High Performance Computing (HPC) using as use case [Qarnot Computing's](https://qarnot.com/en) offers.
+
 ## License
 PowerAPI is licensed under the BSD-3-Clause License. See the [LICENSE](LICENSE) file for details.
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi?ref=badge_large)
```

#### html2text {}

```diff
@@ -21,69 +21,83 @@
 [University of Lille](https://www.univ-lille.fr) and [Inria](https://
 www.inria.fr). The documentation of the project is available [here](http://
 powerapi.org). ## Mailing list You can follow the latest news and asks
 questions by subscribing to our _m_a_i_l_i_n_g_ _l_i_s_t. ## Contributing If you would like
 to contribute code you can do so through GitHub by forking the repository and
 sending a pull request. When submitting code, please make every effort to
 [follow existing conventions and style](CONTRIBUTING.md) in order to keep the
-code as readable as possible. ## Publications * **[SelfWatts: On-the-fly
+code as readable as possible. ## Publications - **[Evaluating the Impact of
+Java Virtual Machines on Energy Consumption](https://hal.inria.fr/hal-
+03275286v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat. _15th
+ACM/IEEE International Symposium on Empirical Software Engineering and
+Measurement_ (ESEM). October 2021, Bari, Italy. - **[SelfWatts: On-the-fly
 Selection of Performance Events to Optimize Software-defined Power Meters]
-(https://hal.inria.fr/hal-03173410)**: G. Fieni, R. Rouvoy, L. Seinturier.
-*IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing*
-(CCGrid). May 2021, Melbourne, Australia * **[Power Budgeting of Big Data
-Applications in Container-based Clusters](https://hal.inria.fr/hal-02904300)**:
-J. Enes, G. Fieni, R. ExpÃ³sito, R. Rouvoy, J. Tourino. *IEEE Cluster*,
-September 2020, Kobe, Japan * **[SmartWatts: Self-Calibrating Software-Defined
-Power Meter for Containers](https://hal.inria.fr/hal-02470128)**: G. Fieni, R.
-Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and
-Grid Computing* (CCGrid). May 2020, Melbourne, Australia * **[Taming Energy
-Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-
-02403379)**: Z. Ournani, M.C. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L.
-Seinturier. *ACM/SPEC International Conference on Performance Engineering*
-(ICPE). April 2020, Edmonton, Canada * **[WattsKit: Software-Defined Power
-Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M.
-Colmant, P. Felber, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium
-on Cluster, Cloud and Grid Computing* (CCGrid). April 2017, Spain, France * **
+(https://hal.inria.fr/hal-03173410v1)**: G. Fieni, R. Rouvoy, L. Seiturier.
+_20th IEEE/ACM International Symposium on Cluster, Cloud and Internet
+Computing_ (CCGRID 2021). May 2021, Melbourne, Australia. - **[SmartWatts:
+Self-Calibrating Software-Defined Power Meter for Containers](https://
+hal.inria.fr/hal-02470128v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/
+ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID
+2020). May 2020, Melbourne, Australia. - **[Taming Energy Consumption
+Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379v1)**: Z.
+Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. _11th ACM/
+SPEC International Conference on Performance Engineering_ (ICPE'2020). April
+2020, Edmonton, Canada. - **[The Next 700 CPU Power Models](https://
+hal.inria.fr/hal-01827132v2)**: M. Colmant, R. Rouvoy, M. Kurpicz, A. Sobe, P.
+Felber, L. Seinturier. _Elsevier Journal of Systems and Software_ (JSS). 144
+(10):382-396, Elsevier. - **[WattsKit: Software-Defined Power Monitoring of
+Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P.
+Felber, R. Rouvoy, L. Seinturier. _IEEE/ACM International Symposium on Cluster,
+Cloud and Grid Computing_ (CCGrid). April 2017, Spain, France. pp.1-14. - **
 [Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-
 01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe.
-*European Conference on Computer Systems* (EuroSys). April 2015, Bordeaux,
-France * **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-
-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. *Journal of Automated
-Software Engineering*, Springer, 2015 * **[Unit Testing of Energy Consumption
-of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R.
-Rouvoy, L. Seinturier. *International Symposium On Applied Computing* (SAC),
-March 2014, Gyeongju, South Korea * **[Informatique : Des logiciels mis au
-vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-
-vert)**: L. Seinturier, R. Rouvoy. *J'innove en Nord Pas de Calais*, [NFID]
-(http://www.jinnove.com) * **[PowerAPI: A Software Library to Monitor the
-Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/
-powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-
-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. *ERCIM News,
-Special Theme: Smart Energy Systems*, 92, pp.43-44. [ERCIM](http://
-www.ercim.eu), 2013 * **[Mesurer la consommation en Ã©nergie des logiciels avec
-prÃ©cision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**:
-A. Bourdon, R. Rouvoy, L. Seinturier. *01 Business & Technologies*, 2013 * **[A
-review of energy measurement approaches](https://hal.inria.fr/hal-
-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. *ACM SIGOPS Operating
-Systems Review*, ACM, 2013, 47 (3) * **[Runtime Monitoring of Software Energy
-Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R.
-Rouvoy, L. Seinturier. *International Conference on Automated Software
-Engineering* (ASE), September 2012, Essen, Germany * **[A Preliminary Study of
-the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-
-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier.
-*International Workshop on Green and Sustainable Software* (GREENS), June 2012,
-Zurich, Switzerland ## Use Cases PowerAPI is used in a variety of projects to
-address key challenges of GreenIT: * [SmartWatts](https://github.com/powerapi-
-ng/smartwatts-formula) is a self-adaptive power meter that can estimate the
-energy consumption of software containers in real-time. * [GenPack](https://
+_European Conference on Computer Systems_ (EuroSys). April 2015, Bordeaux,
+France. pp.1-14. - **[Monitoring Energy Hotspots in Software](https://
+hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. _Journal
+of Automated Software Engineering_, Springer, 2015, pp.1-42. - **[Unit Testing
+of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-
+00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. _International Symposium
+On Applied Computing_ (SAC), March 2014, Gyeongju, South Korea. pp.1200-1205. -
+**[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/
+Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. _J'innove
+en Nord Pas de Calais_, [NFID](http://www.jinnove.com), 2013. - **[PowerAPI: A
+Software Library to Monitor the Energy Consumed at the Process-Level](http://
+ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-
+energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy,
+L. Seinturier. _ERCIM News, Special Theme: Smart Energy Systems_, 92, pp.43-44.
+[ERCIM](http://www.ercim.eu), 2013. - **[Mesurer la consommation en Ã©nergie
+des logiciels avec prÃ©cision](http://www.lifl.fr/digitalAssets/0/
+807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. _01
+Business & Technologies_, 2013. - **[A review of energy measurement approaches]
+(https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L.
+Seinturier. _ACM SIGOPS Operating Systems Review_, ACM, 2013, 47 (3), pp.42-49.
+- **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-
+00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier.
+_International Conference on Automated Software Engineering_ (ASE), September
+2012, Essen, Germany. pp.160-169. - **[A Preliminary Study of the Impact of
+Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A.
+Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Workshop on
+Green and Sustainable Software_ (GREENS), June 2012, Zurich, Switzerland.
+pp.21-27. ## Use Cases PowerAPI is used in a variety of projects to address key
+challenges of GreenIT: * [SmartWatts](https://github.com/powerapi-ng/
+smartwatts-formula) is a self-adaptive power meter that can estimate the energy
+consumption of software containers in real-time. * [GenPack](https://
 hal.inria.fr/hal-01403486) provides a container scheduling strategy to minimize
 the energy footprint of cloud infrastructures. * [VirtualWatts](https://
 github.com/powerapi-ng/virtualwatts-formula) provides process-level power
 estimation of applications running in virtual machines. * [Web Energy Archive]
 (http://webenergyarchive.com) ranks popular websites based on the energy
 footpring they imposes to browsers. * [Greenspector](https://greenspector.com)
 optimises the power consumption of software by identifying potential energy
-leaks in the source code. ## License PowerAPI is licensed under the BSD-3-
-Clause License. See the [LICENSE](LICENSE) file for details. [![FOSSA Status]
-(https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpowerapi-
+leaks in the source code. ## Research Projects Currently, PowerAPI is used in
+two research projects: - [Distiller ANR Project](https://www.davidson.fr/blog/
+comment-reduire-limpact-environnemental-des-applications-cloud-davidson-
+consulting-inria-ovhcloud-orange-sassocient-pour-le-programme-de-recherche-
+distiller) that searches to reduce energy consumption of Cloud applications. -
+[DÃ©fi Pulse](https://www.inria.fr/fr/pulse-defi-qarnot-computing-ademe-calcul-
+intensif-hpc-environnement) studies how to valorize emissions from High
+Performance Computing (HPC) using as use case [Qarnot Computing's](https://
+qarnot.com/en) offers. ## License PowerAPI is licensed under the BSD-3-Clause
+License. See the [LICENSE](LICENSE) file for details. [![FOSSA Status](https://
+app.fossa.com/api/projects/git%2Bgithub.com%2Fpowerapi-
 ng%2Fpowerapi.svg?type=large)](https://app.fossa.com/projects/
 git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi?ref=badge_large)
```

### Comparing `powerapi-2.5.0/pyproject.toml` & `powerapi-2.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 
 [project]
 name = "powerapi"
 description = "PowerAPI is a middleware toolkit for building software-defined power meters."
 readme = "README.md"
 keywords = ["powerapi", "energy", "power-meter", "green-computing"]
 license = {text = "BSD-3-Clause"}
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dynamic = ["version"]
 
 classifiers = [
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Developers",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `powerapi-2.5.0/src/powerapi/__init__.py` & `powerapi-2.6.0/src/powerapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.5.0"
+__version__ = "2.6.0"
```

### Comparing `powerapi-2.5.0/src/powerapi/actor/__init__.py` & `powerapi-2.6.0/src/powerapi/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/actor/actor.py` & `powerapi-2.6.0/src/powerapi/actor/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 import signal
 import multiprocessing
 import sys
 import traceback
 import setproctitle
 
 from powerapi.exception import PowerAPIExceptionWithMessage, UnknownMessageTypeException
-from powerapi.message import PoisonPillMessage
-from powerapi.handler import HandlerException
+from powerapi.message import PoisonPillMessage, Message
+from powerapi.handler import HandlerException, Handler
 
 from .socket_interface import SocketInterface
 from .state import State
 
 
 class InitializationException(PowerAPIExceptionWithMessage):
     """
@@ -133,15 +133,14 @@
         while self.state.alive:
             try:
                 self.behaviour(self)
             except Exception as exn:
                 if type(exn) in self.low_exception:
                     self.logger.error('Minor exception raised, restart actor !')
                     traceback.print_exc()
-                    self.state.reinit()
                 else:
                     self.state.alive = False
                     self.logger.error('Major Exception raised, stop actor')
                     traceback.print_exc()
 
         self._kill_process()
 
@@ -185,15 +184,15 @@
     def setup(self):
         """
         Function called before entering on the behaviour loop
 
         Can be overriden to use personal actor setup
         """
 
-    def add_handler(self, message_type, handler):
+    def add_handler(self, message_type: type[Message], handler: Handler):
         """
         Map a handler to a message type
 
         :param type message_type: type of the message that the handler can
                                   handle
         :param handler: handler that will handle all messages of the given type
         :type handler: powerapi.handler.Handler
```

### Comparing `powerapi-2.5.0/src/powerapi/actor/socket_interface.py` & `powerapi-2.6.0/src/powerapi/actor/socket_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import pickle
+import ctypes
 import logging
 import multiprocessing
-import ctypes
 
 import zmq
 
 from powerapi.exception import PowerAPIException
 
 LOCAL_ADDR = 'tcp://127.0.0.1'
 
@@ -138,15 +137,14 @@
                                  closing 0 mean hardkill the socket even if msg
                                  are still here.
         :return (zmq.Socket, int): the initialized socket and the port where the
                                    socket is bound
         """
         socket = zmq.Context.instance().socket(socket_type)
         socket.setsockopt(zmq.LINGER, linger_value)
-        socket.set_hwm(0)
         port_number = socket.bind_to_random_port(LOCAL_ADDR)
         self.poller.register(socket, zmq.POLLIN)
         self.logger.debug('Bind socket to %s:%d', LOCAL_ADDR, port_number)
         return (socket, port_number)
 
     def receive(self):
         """
@@ -196,34 +194,30 @@
         if self.pull_socket is not None:
             self.pull_socket.close()
 
         if self.control_socket is not None:
             self.control_socket.close()
 
     @staticmethod
-    def _send_serialized(socket, msg):
+    def _send_serialized(socket: zmq.Socket, msg):
         """
-        Send a serialized msg with pickle to the given socket
-
-        :param zmq.Socket socket: socket used to send the message
-        :param Object msg: message to send
+        Send a message to the given socket.
+        :param socket: Socket to use
+        :param msg: Message to send
         """
-        socket.send(pickle.dumps(msg))
+        socket.send_pyobj(msg)
 
     @staticmethod
-    def _recv_serialized(socket):
+    def _recv_serialized(socket: zmq.Socket):
         """
-        Wait for a message from the given socket and return its deserialized
-        value (using pickle)
-
-        :param zmq.Socket socket: socket to wait for a reception
-        :return Object: the received message
+        Receive and returns a message from the given socket.
+        :param socket: Socket to use
+        :return: Message received
         """
-        msg = pickle.loads(socket.recv())
-        return msg
+        return socket.recv_pyobj()
 
     def connect_data(self):
         """
         Connect to the pull socket of this actor
 
         Open a push socket on the process that want to communicate with this
         actor
@@ -235,15 +229,14 @@
         if self.pull_socket_address is None:
             self._values_available.wait()
             self.pull_socket_address = LOCAL_ADDR + ':' + str(self._pull_port.value)
             self.control_socket_address = LOCAL_ADDR + ':' + str(self._ctrl_port.value)
 
         self.push_socket = zmq.Context.instance().socket(zmq.PUSH)
         self.push_socket.setsockopt(zmq.LINGER, -1)
-        self.push_socket.set_hwm(0)
         self.push_socket.connect(self.pull_socket_address)
         self.logger.debug('Connected data socket to %s', self.pull_socket_address)
 
     def connect_control(self):
         """
         Connect to the control socket of this actor
 
@@ -254,15 +247,14 @@
         if self.pull_socket_address is None:
             self._values_available.wait()
             self.pull_socket_address = LOCAL_ADDR + ':' + str(self._pull_port.value)
             self.control_socket_address = LOCAL_ADDR + ':' + str(self._ctrl_port.value)
 
         self.control_socket = zmq.Context.instance().socket(zmq.PAIR)
         self.control_socket.setsockopt(zmq.LINGER, 0)
-        self.control_socket.set_hwm(0)
         self.control_socket.connect(self.control_socket_address)
         self.logger.debug('Connected control socket to %s', self.control_socket_address)
 
     def send_control(self, msg):
         """
         Send a message on the control canal
```

### Comparing `powerapi-2.5.0/src/powerapi/actor/state.py` & `powerapi-2.6.0/src/powerapi/handler/handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,71 +23,91 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.exception import UnknownMessageTypeException
-from powerapi.actor.supervisor import Supervisor
+from powerapi.exception import PowerAPIException, UnknownMessageTypeException
+from powerapi.message import Message
 
 
-class State:
+class HandlerException(PowerAPIException):
     """
-    A basic state class that encapsulate basic actor values :
+    Exception raised when a problem appear in a handler
+    """
+
+    def __init__(self, msg):
+        """
+        :param str msg: Message of the error
+        """
+        PowerAPIException.__init__(self, msg)
+
 
-    :attr:`initialized <powerapi.actor.state.State.initialized>`
-    :attr:`alive <powerapi.actor.state.State.alive>`
-    :attr:`behaviour <powerapi.actor.state.State.behaviour>`
-    :attr:`handlers <powerapi.actor.state.State.handlers>`
-    :attr:`supervisor <powerapi.actor.state.State.supervisor>`
+class Handler:
+    """
+    Class that handle a message of a given type
     """
 
-    def __init__(self, actor):
+    def __init__(self, state):
         """
-        :param powerapi.Actor actor: Actor
+        :param state: Actor state
         """
-        #: (bool): True if the actor is initialized and can handle all
-        #: message, False otherwise
-        self.initialized = False
-        #: (bool): True if the actor is alive, False otherwise
-        self.alive = True
-        #: ([(type, powerapi.handler.abstract_handler.AbstractHandler)]):
-        #: mapping between message type and handler that the mapped handler
-        #: must handle
-        self.handlers = []
-        #: (powerapi.actor.supervisor.Supervisor): object that supervise actors
-        #: that are handle by this actor
-        self.supervisor = Supervisor()
-        #: (powerapi.Actor): Actor
-        self.actor = actor
+        self.state = state
 
-    def get_corresponding_handler(self, msg):
+    def handle_message(self, msg: Message):
         """
-        Return the handler corresponding to the given message type
+        Handle a message and return a new state value of the actor
+
+        This is the method that should be called to handle received message
+        this method call :meth:`Handler.handle <powerapi.handler.abstract_handler.Handler.handle>`
 
-        :param Object msg: the received message
-        :return: the handler corresponding to the given message type
-        :rtype: powerapi.handler.AbstractHandler
+        :param Object msg: the message received by the actor
+        """
+        self.handle(msg)
 
-        :raises UnknowMessageTypeException: if no handler could be find
+    def handle(self, msg: Message):
         """
-        for (msg_type, handler) in self.handlers:
-            if isinstance(msg, msg_type):
-                return handler
-        raise UnknownMessageTypeException()
+        Handle a message and return a new state value of the actor
+
+        Override this method to implement the handler behaviour
 
-    def add_handler(self, message_type, handler):
+        :param Object msg: the message received by the actor
         """
-        Map a handler to a message type
+        raise NotImplementedError()
 
-        :param type message_type: type of the message that the handler can
-                                  handle
-        :param handler: handler that will handle all messages of the given type
-        :type handler: powerapi.handler.AbstractHandler
+    def delegate_message_handling(self, msg: Message):
         """
-        self.handlers.append((message_type, handler))
+        Deletage the message handling to a suitable handler
+        :param msg: The message to handle
+        """
+        try:
+            handler = self.state.get_corresponding_handler(msg)
+            handler.handle_message(msg)
+        except UnknownMessageTypeException:
+            self.state.actor.logger.warning("UnknowMessageTypeException: " + str(msg))
+        except HandlerException:
+            self.state.actor.logger.warning("HandlerException")
+
+
+class InitHandler(Handler):
+    """
+    Class that handle a message of a given type if the actor is initialized
+    """
 
-    def reinit(self):
+    def handle_message(self, msg: Message):
         """
-        Reinitialize the state
+        Handle a message and return a the new state value of the actor
+
+        This is the method that should be called to handle received message
+
+        if the given state is not initialized, return the given state without
+        side effect. Otherwise, use the
+        :meth:`Handler.handle <powerapi.handler.abstract_handler.Handler.handle>`
+        method to handle the message
+
+        :param Object msg: the message received by the actor
         """
+        if not self.state.initialized:
+            return
+
+        self.handle(msg)
```

### Comparing `powerapi-2.5.0/src/powerapi/actor/supervisor.py` & `powerapi-2.6.0/src/powerapi/actor/supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/backend_supervisor/__init__.py` & `powerapi-2.6.0/src/powerapi/backend_supervisor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/backend_supervisor/backend_supervisor.py` & `powerapi-2.6.0/src/powerapi/backend_supervisor/backend_supervisor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/__init__.py` & `powerapi-2.6.0/src/powerapi/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/binding_manager.py` & `powerapi-2.6.0/src/powerapi/cli/binding_manager.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/common_cli_parsing_manager.py` & `powerapi-2.6.0/src/powerapi/cli/common_cli_parsing_manager.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/config_parser.py` & `powerapi-2.6.0/src/powerapi/cli/config_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from typing import Any, Callable
 
 from powerapi.exception import AlreadyAddedArgumentException, UnknownArgException, \
     MissingValueException, BadContextException, TooManyArgumentNamesException, NoNameSpecifiedForSubgroupException, \
     SubgroupAlreadyExistException, SubgroupParserWithoutNameArgumentException, BadTypeException, \
     MissingArgumentException, SameLengthArgumentNamesException, InvalidPrefixException, RepeatedArgumentException, \
     SubgroupDoesNotExistException, AlreadyAddedSubgroupException
-from powerapi.utils.cli import find_longest_string_in_list, remove_first_characters, string_to_bool
+from powerapi.utils.cli import find_longest_string_in_list, string_to_bool
 
 
 def store_val(argument_name: str, val: Any, configuration: dict, args: list = None) -> (list, dict):
     """
     Action that stores the value of the argument on the parser result
 
     """
@@ -476,16 +476,16 @@
             args, _ = getopt.getopt(args, self.short_arg, self.long_arg)
         except getopt.GetoptError as exn:
             if 'recognized' in exn.msg:
                 raise UnknownArgException(exn.opt) from exn
             if 'requires' in exn.msg:
                 raise MissingValueException(exn.opt) from exn
 
-        # remove minus
-        args = list(map(lambda x: (remove_first_characters(x[0]), x[1]), args))
+        # Remove `-` and `--` prefix in argument name (`--test-arg` to `test-arg`)
+        args = [(arg[0].lstrip('-'), arg[1]) for arg in args]
 
         # verify if help argument exists in args
         if self.help_arg:
             for arg_name, _ in args:
                 if arg_name in ('h', 'help'):
                     print(self.get_help())
                     sys.exit(0)
```

### Comparing `powerapi-2.5.0/src/powerapi/cli/config_validator.py` & `powerapi-2.6.0/src/powerapi/cli/config_validator.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/generator.py` & `powerapi-2.6.0/src/powerapi/cli/generator.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/cli/parsing_manager.py` & `powerapi-2.6.0/src/powerapi/cli/parsing_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,29 +141,18 @@
 
         self.cli_parser.add_subgroup_parser(subgroup_type=subgroup_name, subgroup_parser=subgroup_parser.cli_parser)
 
     def _parse_cli(self, cli_line: list) -> dict:
         return self.cli_parser.parse(cli_line)
 
     def _parse_config_from_json_file(self, file_name: str, current_conf: dict) -> dict:
-
-        # Select for each argument, le long version name
-        conf = self.cli_parser.parse_config_dict(file_name=file_name)
-
-        conf = merge_dictionaries(source=current_conf, destination=conf)
-
-        return conf
+        return merge_dictionaries(current_conf, self.cli_parser.parse_config_dict(file_name))
 
     def _parse_config_from_environment_variables(self, current_conf: dict) -> dict:
-
-        conf = self.cli_parser.parse_config_environment_variables()
-
-        conf = merge_dictionaries(source=current_conf, destination=conf)
-
-        return conf
+        return merge_dictionaries(current_conf, self.cli_parser.parse_config_environment_variables())
 
     def add_argument(self, *names, is_flag: bool = False, action: Callable = store_val, default_value: Any = None,
                      help_text: str = '', argument_type: type = str, is_mandatory: bool = False) -> None:
         """
         Add an argument to the parser.
         """
         self.cli_parser.add_argument(*names, is_flag=is_flag, action=action, default_value=default_value,
```

### Comparing `powerapi-2.5.0/src/powerapi/database/__init__.py` & `powerapi-2.6.0/src/powerapi/database/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/database/base_db.py` & `powerapi-2.6.0/src/powerapi/database/opentsdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,90 +22,95 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+import logging
+try:
+    from opentsdb import TSDBClient
+except ImportError:
+    logging.getLogger().info("opentsdb-py is not installed.")
+
 from typing import List, Type
-from powerapi.report import Report
-from powerapi.exception import PowerAPIExceptionWithMessage
 
+from powerapi.report import PowerReport, Report
+from .base_db import BaseDB, DBError
 
-class DBError(PowerAPIExceptionWithMessage):
 
+class CantConnectToOpenTSDBException(DBError):
     """
-    Error raised when an error occuried when using a database
+    Exception raised to notify that connection to the opentsdb database is impossible
     """
-    def __init__(self, msg: str):
-        PowerAPIExceptionWithMessage.__init__(self, msg)
 
 
-class IterDB:
+class OpenTSDB(BaseDB):
     """
-    IterDB class
+    OpenTSDB class herited from BaseDB
 
-    This class allows to browse a database as an iterable
+    Allow to handle an OpenTSDB database to save PowerReport.
     """
 
-    def __init__(self, db, report_type, stream_mode):
-        """
+    def __init__(self, report_type: Type[Report], host: str, port, metric_name: str):
         """
-        self.db = db
-        self.stream_mode = stream_mode
-        self.report_type = report_type
+        :param host:             host of the OpenTSDB server
+        :param port:            port of the OpenTSDB server
 
-    def __iter__(self):
-        """
-        """
-        raise NotImplementedError()
+        :param metric_name:         mectric name to store
 
-    def __next__(self) -> Report:
-        """
-        """
-        raise NotImplementedError()
 
+        :param report_type:        type of report handled by this database
 
-class BaseDB:
-    """
-    Abstract class which define every common function for database uses.
+        """
+        BaseDB.__init__(self, report_type)
+        self.host = host
+        self.port = port
+        self.metric_name = metric_name
 
-    This class define every common function that need to be implemented
-    by each DB module. A database module correspond to a kind of BDD.
-    For example, Mongodb, influxdb, csv are different kind of BDD.
-    """
-    def __init__(self, report_type: Type[Report], exceptions: List[Type[Exception]] = None, asynchrone: bool = False):
-        self.exceptions = exceptions or []
-        self.asynchrone = asynchrone
-        self.report_type = report_type
+        self.client = None
+
+    def __iter__(self):
+        raise NotImplementedError()
 
     def connect(self):
         """
-        Function that allow to load the database. Depending of the type,
-        different process can happen.
+        Override from BaseDB.
+
+        Create the connection to the openTSDB database with the current
+        configuration (hostname/port), then check if the connection has
+        been created without failure.
 
-        .. note:: Need to be overrided
         """
-        raise NotImplementedError()
+        # close connection if reload
+        if self.client is not None:
+            self.client.close()
+            self.client.wait()
+
+        self.client = TSDBClient(host=self.host, port=self.port)
 
-    def iter(self, stream_mode: bool) -> IterDB:
+        if not self.client.is_connected() and not self.client.is_alive():
+            raise CantConnectToOpenTSDBException('connexion error')
+
+    def disconnect(self):
         """
-        Create the iterator for get the data
-        :param stream_mode: Define if we read in stream mode
+        Disconnect from the OpenTSDB database.
         """
-        raise NotImplementedError()
 
-    def save(self, report: Report):
+    def save(self, report: PowerReport):
         """
-        Allow to save a json input in the db
+        Override from BaseDB
 
-        :param report: Report
+        :param report: Report to save
         """
-        raise NotImplementedError()
+        self.client.send(self.metric_name, report.power, timestamp=int(report.timestamp.timestamp()),
+                         host=report.target)
 
     def save_many(self, reports: List[Report]):
         """
-        Allow to save a batch of data
+        Save a batch of data
 
-        :param reports: Batch of Serialized Report
+        :param reports: Batch of data.
         """
-        raise NotImplementedError()
+
+        for report in reports:
+            self.save(report)
```

### Comparing `powerapi-2.5.0/src/powerapi/database/csvdb.py` & `powerapi-2.6.0/src/powerapi/database/csvdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     def _next(self, filename):
         """
         Get next row, None otherwise
 
         :param str filename: file name we want to read
         """
         try:
-            return self.tmp_read[filename]['reader'].__next__()
+            return next(self.tmp_read[filename]['reader'])
         except StopIteration:
             return None
 
     def _close_file(self):
         for filename in self.filenames:
             if self.tmp_read[filename]['file'] is not None:
                 self.tmp_read[filename]['file'].close()
@@ -241,25 +241,28 @@
         """
         self.filenames.clear()
 
     ########################
     # Override from BaseDB #
     ########################
 
-    def iter(self, stream_mode: bool) -> CsvIterDB:
+    def iter(self, stream_mode: bool = False) -> CsvIterDB:
         """
         Create the iterator for get the data
         """
         return CsvIterDB(self, self.filenames, self.report_type, stream_mode)
 
     def connect(self):
         """
-        Override from BaseDB.
+        Connect to the csv database.
+        """
 
-        Nothing to do with CSV, because it's just files operations.
+    def disconnect(self):
+        """
+        Disconnect from the csv database.
         """
 
     def save(self, report: Report):
         """
         Allow to save a serialized_report in the db
 
         :param report: Report
@@ -269,27 +272,25 @@
         # If the repository doesn't exist, create it
         rep_path = self.current_path + report.sensor + "-" + report.target
         os.makedirs(rep_path, exist_ok=True)
 
         for filename, values in data.items():
             output_filename = f'{rep_path}/{filename}.csv'
 
-            with open(output_filename, 'r+', encoding='utf-8') as csvfile:
+            with open(output_filename, 'a+', encoding='utf-8') as csvfile:
                 expected_header = fixed_header + sorted(set(values[0].keys()) - set(fixed_header))
                 header_exist = False
 
+                csvfile.seek(0)  # Go to beginning of file before reading
                 reader = csv.DictReader(csvfile)
                 if reader.fieldnames:
                     header_exist = True
                     if reader.fieldnames != expected_header:
                         raise HeaderAreNotTheSameError(f"Header are not the same in {output_filename}")
 
-                # Go to EOF before writing rows
-                csvfile.seek(0, 2)
-
                 writer = csv.DictWriter(csvfile, fieldnames=expected_header)
                 if not header_exist:
                     writer.writeheader()
 
                 for row in values:
                     writer.writerow(row)
```

### Comparing `powerapi-2.5.0/src/powerapi/database/file_db.py` & `powerapi-2.6.0/src/powerapi/database/file_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,20 @@
         Override from BaseDB.
 
         It check that the file exist
         """
         if not os.path.exists(self.filename):
             raise FileBadDBError(self.filename)
 
-    def iter(self, stream_mode: bool) -> FileIterDB:
+    def disconnect(self):
+        """
+        Disconnect from the file database.
+        """
+
+    def iter(self, stream_mode: bool = False) -> FileIterDB:
         """
         Create the iterator for get the data
         """
         return FileIterDB(self, self.report_type, stream_mode, self.filename)
 
     def save(self, report: Report):
         """
```

### Comparing `powerapi-2.5.0/src/powerapi/database/influxdb2.py` & `powerapi-2.6.0/src/powerapi/database/influxdb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,20 +90,15 @@
         raise NotImplementedError()
 
     def _ping_client(self):
         self.client.ping()
 
     def connect(self):
         """
-            Override from BaseDB.
-
-            Create the connection to the influxdb database with the current
-            configuration (url:port/bucket_name/org), then check if the connection has
-            been created without failure.
-
+        Connect to the influxdb2 database.
         """
         # close connection if reload
         if self.client is not None:
             self.client.close()
 
         try:
 
@@ -119,14 +114,19 @@
 
         # A bucket is created only if it does not exist
         if self.buckets_api.find_bucket_by_name(self.bucket_name) is not None:
             return
 
         self.buckets_api.create_bucket(bucket_name=self.bucket_name)
 
+    def disconnect(self):
+        """
+        Disconnect from the influxdb2 database.
+        """
+
     def get_db_by_name(self, db_name: str):
         """
             Get the database (bucket) with the given name
 
             :param db_name: database name
             :return: The database (bucket) with the given name
         """
```

### Comparing `powerapi-2.5.0/src/powerapi/database/mongodb.py` & `powerapi-2.6.0/src/powerapi/database/mongodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,15 +141,20 @@
         try:
             self.mongo_client.admin.command('ismaster')
         except pymongo.errors.ServerSelectionTimeoutError as exn:
             raise MongoBadDBError(self.uri) from exn
 
         self.collection = self.mongo_client[self.db_name][self.collection_name]
 
-    def iter(self, stream_mode: bool) -> MongoIterDB:
+    def disconnect(self):
+        """
+        Disconnect from the mongodb database.
+        """
+
+    def iter(self, stream_mode: bool = False) -> MongoIterDB:
         """
         Create the iterator for get the data
         """
         return MongoIterDB(self, self.report_type, stream_mode)
 
     def save(self, report: Report):
         """
```

### Comparing `powerapi-2.5.0/src/powerapi/database/opentsdb.py` & `powerapi-2.6.0/src/powerapi/pusher/pusher_actor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2021, INRIA
-# Copyright (c) 2021, University of Lille
+# Copyright (c) 2022, INRIA
+# Copyright (c) 2022, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -22,90 +22,71 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import logging
-try:
-    from opentsdb import TSDBClient
-except ImportError:
-    logging.getLogger().info("opentsdb-py is not installed.")
-
-from typing import List, Type
-
-from powerapi.report import PowerReport, Report
-from .base_db import BaseDB, DBError
 
+import logging
+from powerapi.actor import Actor, State
+from powerapi.message import PoisonPillMessage, StartMessage
 
-class CantConnectToOpenTSDBException(DBError):
-    """
-    Exception raised to notify that connection to the opentsdb database is impossible
-    """
+from powerapi.pusher.handlers import ReportHandler, PusherStartHandler, PusherPoisonPillMessageHandler
 
 
-class OpenTSDB(BaseDB):
+class PusherState(State):
     """
-    OpenTSDB class herited from BaseDB
+    Pusher Actor State
 
-    Allow to handle an OpenTSDB database to save PowerReport.
+    Contains in addition to State values :
+      - The database interface
     """
 
-    def __init__(self, report_type: Type[Report], host: str, port, metric_name: str):
-        """
-        :param host:             host of the OpenTSDB server
-        :param port:            port of the OpenTSDB server
-
-        :param metric_name:         mectric name to store
-
-
-        :param report_type:        type of report handled by this database
-
+    def __init__(self, actor, database, report_model):
         """
-        BaseDB.__init__(self, report_type)
-        self.host = host
-        self.port = port
-        self.metric_name = metric_name
-
-        self.client = None
-
-    def __iter__(self):
-        raise NotImplementedError()
-
-    def connect(self):
+        :param BaseDB database: Database for saving data.
         """
-        Override from BaseDB.
+        State.__init__(self, actor)
 
-        Create the connection to the openTSDB database with the current
-        configuration (hostname/port), then check if the connection has
-        been created without failure.
+        #: (BaseDB): Database for saving data.
+        self.database = database
 
-        """
-        # close connection if reload
-        if self.client is not None:
-            self.client.close()
-            self.client.wait()
-
-        self.client = TSDBClient(host=self.host, port=self.port)
+        #: (Report): Type of the report that the pusher handle.
+        self.report_model = report_model
 
-        if not self.client.is_connected() and not self.client.is_alive():
-            raise CantConnectToOpenTSDBException('connexion error')
+        #: (Dict): Buffer data.
+        self.buffer = []
 
-    def save(self, report: PowerReport):
-        """
-        Override from BaseDB
 
-        :param report: Report to save
-        """
-        self.client.send(self.metric_name, report.power, timestamp=int(report.timestamp.timestamp()),
-                         host=report.target)
+class PusherActor(Actor):
+    """
+    PusherActor class
 
-    def save_many(self, reports: List[Report]):
-        """
-        Save a batch of data
+    The Pusher allow to save Report sent by Formula.
+    """
 
-        :param reports: Batch of data.
+    def __init__(self, name, report_model, database, level_logger=logging.WARNING, timeout=1000, delay=100,
+                 max_size=50):
         """
-
-        for report in reports:
-            self.save(report)
+        :param str name: Pusher name.
+        :param Report report_model: ReportModel
+        :param BaseDB database: Database use for saving data.
+        :param int level_logger: Define the level of the logger
+        :param int delay: number of ms before message containing in the buffer will be writen in database
+        :param int max_size: maximum of message that the buffer can store before write them in database
+        """
+        Actor.__init__(self, name, level_logger, timeout)
+
+        #: (State): State of the actor.
+        self.state = PusherState(self, database, report_model)
+        self.delay = delay
+        self.max_size = max_size
+
+    def setup(self):
+        """
+        Define StartMessage, PoisonPillMessage handlers and a handler for
+        each report type
+        """
+        self.add_handler(PoisonPillMessage, PusherPoisonPillMessageHandler(self.state))
+        self.add_handler(self.state.report_model, ReportHandler(self.state, self.delay, self.max_size))
+        self.add_handler(StartMessage, PusherStartHandler(self.state))
```

### Comparing `powerapi-2.5.0/src/powerapi/database/prometheus_db.py` & `powerapi-2.6.0/src/powerapi/database/prometheus_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
 
     def connect(self):
         """
         Start an HTTP server exposing metrics
         """
         start_http_server(port=self.port, addr=self.address)
 
+    def disconnect(self):
+        """
+        Disconnect from the Prometheus database.
+        """
+
 
 class PrometheusDB(BasePrometheusDB):
     """
     Database that expose received raw power estimations as metrics in order to be scrapped by a prometheus instance
     It can only be used with a pusher actor
     """
```

### Comparing `powerapi-2.5.0/src/powerapi/database/socket_db.py` & `powerapi-2.6.0/src/powerapi/database/socket_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,46 +27,77 @@
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import asyncio
 from typing import Type, List
 import json
 
-
 from powerapi.utils import JsonStream
 from powerapi.report import Report
 from .base_db import IterDB, BaseDB, DBError
 
-BUFFER_SIZE = 4096
-SOCKET_TIMEOUT = 0.5
+
+class IterSocketDB(IterDB):
+    """
+    iterator connected to a socket that receive report from a sensor
+    """
+
+    def __init__(self, report_type, stream_mode, queue):
+        """
+        """
+        IterDB.__init__(self, None, report_type, stream_mode)
+
+        self.queue = queue
+
+    def __aiter__(self):
+        return self
+
+    async def __anext__(self):
+        try:
+            json_str = await asyncio.wait_for(self.queue.get(), 2)
+            # json = self.queue.get_nowait()
+            # self.queue.get()
+            report = self.report_type.from_json(json.loads(json_str))
+            return report
+        # except Empty:
+        except asyncio.TimeoutError:
+            return None
 
 
 class SocketDB(BaseDB):
     """
     Database that act as a server that expose a socket where data source will push data
     """
 
     def __init__(self, report_type: Type[Report], port: int):
-        BaseDB.__init__(self, report_type, asynchrone=True)
+        BaseDB.__init__(self, report_type, is_async=True)
         self.queue = None
         self.port = port
         self.server = None
 
     async def connect(self):
+        """
+        Connect to the socket database.
+        """
         self.queue = asyncio.Queue()
         self.server = await asyncio.start_server(self._gen_server_callback(), host='127.0.0.1', port=self.port)
 
+    async def disconnect(self):
+        """
+        Disconnect from the socket database.
+        """
+
     async def stop(self):
         """
         stop server connection
         """
         self.server.close()
         await self.server.wait_closed()
 
-    def iter(self, stream_mode):
+    def iter(self, stream_mode: bool = False) -> IterSocketDB:
         return IterSocketDB(self.report_type, stream_mode, self.queue)
 
     def _gen_server_callback(self):
         async def callback(stream_reader, _):
             stream = JsonStream(stream_reader)
             count = 0  # If 10 times in a row we don't have a full message we stop
             while True:
@@ -87,34 +118,7 @@
         raise DBError('Socket db don\'t support __iter__ method')
 
     def save(self, report: Report):
         raise DBError('Socket db don\'t support save method')
 
     def save_many(self, reports: List[Report]):
         raise DBError('Socket db don\'t support save_many method')
-
-
-class IterSocketDB(IterDB):
-    """
-    iterator connected to a socket that receive report from a sensor
-    """
-
-    def __init__(self, report_type, stream_mode, queue):
-        """
-        """
-        IterDB.__init__(self, None, report_type, stream_mode)
-
-        self.queue = queue
-
-    def __aiter__(self):
-        return self
-
-    async def __anext__(self):
-        try:
-            json_str = await asyncio.wait_for(self.queue.get(), 2)
-            # json = self.queue.get_nowait()
-            # self.queue.get()
-            report = self.report_type.from_json(json.loads(json_str))
-            return report
-        # except Empty:
-        except asyncio.TimeoutError:
-            return None
```

### Comparing `powerapi-2.5.0/src/powerapi/database/virtiofs_db.py` & `powerapi-2.6.0/src/powerapi/database/virtiofs_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,19 @@
         vm_name = match.groups()[0]
         return self.vm_directory_name_prefix + vm_name + self.vm_directory_name_suffix
 
     def connect(self):
         if not os.path.exists(self.root_directory_name):
             raise DirectoryDoesNotExistForVirtioFS(self.root_directory_name)
 
+    def disconnect(self):
+        """
+        Disconnect from the virtiosfs database.
+        """
+
     def save(self, report: Report):
         directory_name = self._generate_vm_directory_name(report.target)
         if directory_name is None:
             return
 
         vm_filename, power = self.report_type.to_virtiofs_db(report)
         vm_filename_path = f'{self.root_directory_name}/{directory_name}'
```

### Comparing `powerapi-2.5.0/src/powerapi/dispatch_rule/__init__.py` & `powerapi-2.6.0/src/powerapi/dispatch_rule/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatch_rule/dispatch_rule.py` & `powerapi-2.6.0/src/powerapi/dispatch_rule/dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatch_rule/hwpc_dispatch_rule.py` & `powerapi-2.6.0/src/powerapi/dispatch_rule/hwpc_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatch_rule/power_dispatch_rule.py` & `powerapi-2.6.0/src/powerapi/dispatch_rule/power_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatch_rule/procfs_dispatch_rule.py` & `powerapi-2.6.0/src/powerapi/dispatch_rule/procfs_dispatch_rule.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatcher/__init__.py` & `powerapi-2.6.0/src/powerapi/dispatcher/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 from powerapi.dispatcher.dispatcher_actor import DispatcherActor, RouteTable
-from powerapi.dispatcher.handlers import extract_formula_id
```

### Comparing `powerapi-2.5.0/src/powerapi/dispatcher/blocking_detector.py` & `powerapi-2.6.0/src/powerapi/dispatcher/blocking_detector.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/dispatcher/dispatcher_actor.py` & `powerapi-2.6.0/src/powerapi/dispatcher/dispatcher_actor.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,111 +29,78 @@
 
 import logging
 from typing import Literal, Callable
 
 from powerapi.actor import Actor, State
 from powerapi.dispatcher.handlers import FormulaDispatcherReportHandler, DispatcherPoisonPillMessageHandler
 from powerapi.dispatcher.route_table import RouteTable
-from powerapi.exception import PowerAPIException
+from powerapi.formula import FormulaActor
 from powerapi.handler import StartHandler
-from powerapi.report import Report
 from powerapi.message import PoisonPillMessage, StartMessage
-from powerapi.utils import Tree
-
-
-class NoPrimaryDispatchRuleRuleException(PowerAPIException):
-    """
-    Exception raised when user want to get the primary dispatch_rule rule on a
-    formula dispatcher that doesn't have one
-    """
-
-
-class PrimaryDispatchRuleRuleAlreadyDefinedException(PowerAPIException):
-    """
-    Exception raised when user want to add a primary dispatch_rule rule on a
-    formula dispatcher that already have one
-    """
+from powerapi.pusher import PusherActor
+from powerapi.report import Report
 
 
 class DispatcherState(State):
     """
-    DispatcherState class herited from State.
-
-    State that encapsulate formula's dicionary and tree
-
-    :attr:`formula_dict
-    <powerapi.dispatcher.dispatcher_actor.DispatcherState.formula_dict>`
-    :attr:`formula_tree
-    <powerapi.dispatcher.dispatcher_actor.DispatcherState.formula_tree>`
-    :attr:`formula_factory
-    <powerapi.dispatcher.dispatcher_actor.DispatcherState.formula_factory>`
+    Dispatcher actor state.
     """
 
-    def __init__(self, actor, pushers, route_table):
+    def __init__(self, actor, pushers: dict[str, PusherActor], route_table: RouteTable):
         """
         :param actor: Dispatcher actor instance
         :param pushers: List of pushers
         :param route_table: Route table to use for reports
         """
         super().__init__(actor)
 
         self.formula_dict = {}
-        self.formula_tree = Tree()
 
         self.pushers = pushers
         self.route_table = route_table
 
-    def add_formula(self, formula_id):
+    def add_formula(self, formula_id: tuple) -> FormulaActor:
         """
-        Create a formula corresponding to the given formula id and add it in memory.
-        :param tuple formula_id: Define the key corresponding to a specific Formula
+        Create a new formula corresponding to the given ID.
+        :param formula_id: The formula ID
+        :return: The new formula actor
         """
         formula = self.actor.formula_init_function(name=str((self.actor.name,) + formula_id), pushers=self.pushers)
-        self.supervisor.launch_actor(formula, start_message=False)
-
+        self.supervisor.launch_actor(formula, False)
         self.formula_dict[formula_id] = formula
-        self.formula_tree.add(list(formula_id), formula)
+        return formula
 
-    def get_direct_formula(self, formula_id):
+    def get_formula(self, formula_id: tuple) -> FormulaActor:
         """
-        Get the formula corresponding to the given formula id
-        or create and return it if its didn't exist
-
-        :param tuple formula_id: Key corresponding to a Formula
-        :return: a Formula
-        :rtype: Formula or None
+        Get the formula corresponding to the given formula id.
+        The formula will be created if it does not exist.
+        :param formula_id: The formula id
+        :return: The formula actor
         """
         if formula_id not in self.formula_dict:
-            self.add_formula(formula_id)
-        return self.formula_dict[formula_id]
+            return self.add_formula(formula_id)
 
-    def get_corresponding_formula(self, formula_id):
-        """
-        Get the Formulas which have id match with the given formula_id
-
-        :param tuple formula_id: Key corresponding to a Formula
-        :return: All Formulas that match with the key
-        :rtype: list(Formula)
-        """
-        return self.formula_tree.get(formula_id)
+        return self.formula_dict[formula_id]
 
 
 class DispatcherActor(Actor):
     """
-    Dispatcher Actor.
+    Dispatcher actor.
+    This actor process the reports coming from the pullers and dispatches them to the formula actors according the
+    provided routing table. When a report doesn't have any formula assigned, the dispatcher will create a new formula.
     """
 
     def __init__(self, name: str, formula_init_function: Callable, pushers: [], route_table: RouteTable,
                  level_logger: Literal = logging.WARNING, timeout=None):
         """
-        :param str name: Actor name
-        :param func formula_init_function: Function for creating Formula
-        :param route_table: initialized route table of the DispatcherActor
-        :param int level_logger: Define the level of the logger
-        :param bool timeout: Define the time in millisecond to wait for a message before run timeout_handler
+        :param name: Actor name
+        :param formula_init_function: Factory function for creating Formula
+        :param route_table: Routing table to use for dispatching the reports
+        :param level_logger: Logging level
+        :param timeout: Time in millisecond to wait for a message before running the timeout handler
         """
         Actor.__init__(self, name, level_logger, timeout)
 
         # (func): Function for creating Formula
         self.formula_init_function = formula_init_function
 
         # (powerapi.DispatcherState): Actor state
@@ -141,13 +108,10 @@
 
     def setup(self):
         """
         Setup Dispatcher actor report handlers.
         """
         super().setup()
 
-        if self.state.route_table.primary_dispatch_rule is None:
-            raise NoPrimaryDispatchRuleRuleException()
-
         self.add_handler(Report, FormulaDispatcherReportHandler(self.state))
         self.add_handler(PoisonPillMessage, DispatcherPoisonPillMessageHandler(self.state))
         self.add_handler(StartMessage, StartHandler(self.state))
```

### Comparing `powerapi-2.5.0/src/powerapi/dispatcher/route_table.py` & `powerapi-2.6.0/src/powerapi/filter/filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2021, INRIA
-# Copyright (c) 2021, University of Lille
+# Copyright (c) 2018, INRIA
+# Copyright (c) 2018, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -26,58 +26,53 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from powerapi.exception import PowerAPIException
 
 
-class PrimaryDispatchRuleRuleAlreadyDefinedException(PowerAPIException):
+class FilterUselessError(PowerAPIException):
     """
-    Exception raised when trying to define a primary dispatch rule on a route table that have already one
+    Exception raised when a filter route with 0 filters
     """
 
 
-class RouteTable:
+class Filter:
     """
-    Structure that map a :class:`Report<powerapi.report.Report>` type to a
-    :class:`DispatchRule<powerapi.dispatch_rule.DispatchRule>` rule
+    Filter class
+
+    A filter allow the Puller to route Report of the database to Dispatchers
+    by fixing some rules.
     """
 
     def __init__(self):
-        #: (array): Array of tuple that link a Report type to a DispatchRule
-        # rule
-        self.route_table = []
-        #: (powerapi.DispatchRule): Allow to define how to create the Formula id
-        self.primary_dispatch_rule = None
+        self.filters = []
 
-    def get_dispatch_rule(self, msg):
+    def filter(self, rule, dispatcher):
         """
-        Return the corresponding group by rule mapped to the received message
-        type
+        Define a rule for a kind of report, and send it to the dispatcher
+        if the rule accept it.
 
-        :param type msg: the received message
-        :return: the dispatch_rule rule mapped to the received message type
-        :rtype: powerapi.dispatch_rule.DispatchRule
-        :raise: UnknowMessageTypeException if no group by rule is mapped to the
-                received message type
+        :param (func(report) -> bool) rule:      Function which return if
+                                                 the report has to be send to
+                                                 this dispatcher
+        :param powerapi.Dispatcher dispatcher: Dispatcher we want to send the
+                                                 report
         """
-        for (report_class, dispatch_rule) in self.route_table:
-            if isinstance(msg, report_class):
-                return dispatch_rule
-
-        return None
+        self.filters.append((rule, dispatcher))
 
-    def dispatch_rule(self, report_class, dispatch_rule):
+    def route(self, report):
         """
-        Add a dispatch_rule rule to the route table
+        Get the list of dispatchers to whom send the report, or None
 
-        :param Type report_class: Type of the message that the
-                                  dispatch_rule rule must handle
-        :param dispatch_rule: Group_by rule to add
-        :type dispatch_rule:  powerapi.dispatch_rule.DispatchRule
+        :param powerapi.Report report: Message to send
         """
-        if dispatch_rule.is_primary:
-            if self.primary_dispatch_rule is not None:
-                raise PrimaryDispatchRuleRuleAlreadyDefinedException()
-            self.primary_dispatch_rule = dispatch_rule
+        # Error if filters is empty
+        if not self.filters:
+            raise FilterUselessError()
+
+        dispatchers = []
+        for rule, dispatcher in self.filters:
+            if rule(report):
+                dispatchers.append(dispatcher)
 
-        self.route_table.append((report_class, dispatch_rule))
+        return dispatchers
```

### Comparing `powerapi-2.5.0/src/powerapi/exception.py` & `powerapi-2.6.0/src/powerapi/exception.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/filter/__init__.py` & `powerapi-2.6.0/src/powerapi/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/filter/filter.py` & `powerapi-2.6.0/src/powerapi/dispatcher/handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2018, INRIA
-# Copyright (c) 2018, University of Lille
+# Copyright (c) 2022, INRIA
+# Copyright (c) 2022, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,56 +23,34 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from powerapi.exception import PowerAPIException
+from powerapi.handler import InitHandler, PoisonPillMessageHandler
+from powerapi.report import Report
 
 
-class FilterUselessError(PowerAPIException):
+class DispatcherPoisonPillMessageHandler(PoisonPillMessageHandler):
     """
-    Exception raised when a filter route with 0 filters
+    Dispatcher Handler for PoisonPillMessage
     """
+    def teardown(self, soft=False):
+        self.state.supervisor.kill_actors(soft)
 
 
-class Filter:
+class FormulaDispatcherReportHandler(InitHandler):
     """
-    Filter class
-
-    A filter allow the Puller to route Report of the database to Dispatchers
-    by fixing some rules.
+    Send the received reports to their corresponding formula.
     """
 
-    def __init__(self):
-        self.filters = []
-
-    def filter(self, rule, dispatcher):
-        """
-        Define a rule for a kind of report, and send it to the dispatcher
-        if the rule accept it.
-
-        :param (func(report) -> bool) rule:      Function which return if
-                                                 the report has to be send to
-                                                 this dispatcher
-        :param powerapi.Dispatcher dispatcher: Dispatcher we want to send the
-                                                 report
+    def handle(self, msg: Report):
         """
-        self.filters.append((rule, dispatcher))
-
-    def route(self, report):
-        """
-        Get the list of dispatchers to whom send the report, or None
-
-        :param powerapi.Report report: Message to send
+        Send the report to its corresponding formula(s).
+        :param msg: The report to process
         """
-        # Error if filters is empty
-        if not self.filters:
-            raise FilterUselessError()
-
-        dispatchers = []
-        for rule, dispatcher in self.filters:
-            if rule(report):
-                dispatchers.append(dispatcher)
-
-        return dispatchers
+        dispatch_rule = self.state.route_table.get_dispatch_rule(msg)
+        for formula_id in dispatch_rule.get_formula_id(msg):
+            formula = self.state.get_formula(formula_id)
+            if formula.is_alive():
+                formula.send_data(msg)
```

### Comparing `powerapi-2.5.0/src/powerapi/formula/__init__.py` & `powerapi-2.6.0/src/powerapi/formula/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/formula/abstract_cpu_dram_formula.py` & `powerapi-2.6.0/src/powerapi/formula/abstract_cpu_dram_formula.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/formula/formula_actor.py` & `powerapi-2.6.0/src/powerapi/formula/formula_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/formula/handlers.py` & `powerapi-2.6.0/src/powerapi/formula/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/handler/__init__.py` & `powerapi-2.6.0/src/powerapi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/handler/poison_pill_message_handler.py` & `powerapi-2.6.0/src/powerapi/handler/poison_pill_message_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/handler/start_handler.py` & `powerapi-2.6.0/src/powerapi/handler/start_handler.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/message.py` & `powerapi-2.6.0/src/powerapi/message.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/__init__.py` & `powerapi-2.6.0/src/powerapi/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/handlers.py` & `powerapi-2.6.0/src/powerapi/processor/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/__init__.py` & `powerapi-2.6.0/src/powerapi/processor/pre/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/__init__.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/_utils.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/_utils.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/actor.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/handlers.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/metadata_cache_manager.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/metadata_cache_manager.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/k8s/monitor_agent.py` & `powerapi-2.6.0/src/powerapi/processor/pre/k8s/monitor_agent.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/libvirt/__init__.py` & `powerapi-2.6.0/src/powerapi/processor/pre/libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_actor.py` & `powerapi-2.6.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_handlers.py` & `powerapi-2.6.0/src/powerapi/processor/pre/libvirt/libvirt_pre_processor_handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/processor/processor_actor.py` & `powerapi-2.6.0/src/powerapi/processor/processor_actor.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/puller/__init__.py` & `powerapi-2.6.0/src/powerapi/puller/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/puller/handlers.py` & `powerapi-2.6.0/src/powerapi/puller/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 class DBPullerThread(Thread):
     """
     Thread for pulling data from source
     """
 
     def __init__(self, state, timeout, handler):
-        Thread.__init__(self)
+        Thread.__init__(self, daemon=True)
         self.timeout = timeout
         self.state = state
         self.loop = None
         self.handler = handler
 
     def _connect(self):
         try:
@@ -68,16 +68,16 @@
             self.state.database_it = self.state.database.iter(self.state.stream_mode)
         except DBError as error:
             self.state.actor.send_control(ErrorMessage(sender_name='system', error_message=error.msg))
             self.state.alive = False
 
     def _pull_database(self):
         try:
-            if self.state.asynchrone:
-                report = self.loop.run_until_complete(self.state.database_it.__anext__())
+            if self.state.database.is_async:
+                report = self.loop.run_until_complete(anext(self.state.database_it))
                 if report is None:
                     raise StopIteration()
                 return report
 
             return next(self.state.database_it)
 
         except (StopIteration, BadInputData, DeserializationFail) as database_problem:
@@ -91,15 +91,15 @@
         Read data from Database and send it to the dispatchers.
         If there is no more data, send a kill message to every
         dispatcher.
         If stream mode is disabled, kill the actor.
 
         :param None msg: None.
         """
-        if self.state.asynchrone:
+        if self.state.database.is_async:
             self.loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self.loop)
             self.state.loop = self.loop
             self.loop.set_debug(enabled=True)
             logging.basicConfig(level=logging.DEBUG)
 
             self._connect()
@@ -196,14 +196,14 @@
         while self.state.alive:
             msg = self.state.actor.receive_control(self.timeout)
             if msg is not None:
                 self.handle_internal_msg(msg)
 
     def _database_connection(self):
         try:
-            if not self.state.asynchrone:
+            if not self.state.database.is_async:
                 self.state.database.connect()
                 self.state.database_it = self.state.database.iter(stream_mode=self.state.stream_mode)
 
         except DBError as error:
             self.state.actor.send_control(ErrorMessage(self.state.actor.name, error.msg))
             self.state.alive = False
```

### Comparing `powerapi-2.5.0/src/powerapi/puller/puller_actor.py` & `powerapi-2.6.0/src/powerapi/puller/puller_actor.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,16 +46,15 @@
     Puller Actor State
 
     Contains in addition to State values :
       - the database interface
       - the Filter class
     """
 
-    def __init__(self, actor: Actor, database, report_filter, report_model, stream_mode, timeout_puller,
-                 asynchrone=False):
+    def __init__(self, actor: Actor, database, report_filter, report_model, stream_mode, timeout_puller):
         """
         :param BaseDB database: Allow to interact with a Database
         :param Filter report_filter: Filter of the Puller
         """
         super().__init__(actor)
 
         #: (BaseDB): Allow to interact with a Database
@@ -75,44 +74,39 @@
 
         #: (require stream mode = True) time (in ms) between two database reading
         self.timeout_puller = timeout_puller
 
         #: (int): Counter for "sleeping mode"
         self.counter = 0
 
-        #: (bool): enable asynchronous driver
-        self.asynchrone = asynchrone
-
         self.loop = None
 
 
 class PullerActor(Actor):
     """
     PullerActor class
 
     A Puller allows to handle the reading of a database and to dispatch report
     to many Dispatcher depending on some rules.
     """
 
-    def __init__(self, name, database, report_filter, report_model, stream_mode=False,
-                 level_logger=logging.WARNING,
+    def __init__(self, name, database, report_filter, report_model, stream_mode=False, level_logger=logging.WARNING,
                  timeout=5000, timeout_puller=100):
         """
         :param str name: Actor name.
         :param BaseDB database: Allow to interact with a Database.
         :param Filter report_filter: Filter of the Puller.
         :param int level_logger: Define the level of the logger
         :param int tiemout_puller: (require stream mode) time (in ms) between two database reading
-        :param bool asynchrone: use asynchrone driver
         """
 
         Actor.__init__(self, name, level_logger, timeout)
+
         #: (State): Actor State.
-        self.state = PullerState(self, database=database, report_filter=report_filter, report_model=report_model,
-                                 stream_mode=stream_mode, timeout_puller=timeout_puller, asynchrone=database.asynchrone)
+        self.state = PullerState(self, database, report_filter, report_model, stream_mode, timeout_puller)
 
         self.low_exception += database.exceptions
 
     def setup(self):
         """
         Define StartMessage handler and PoisonPillMessage handler
         """
```

### Comparing `powerapi-2.5.0/src/powerapi/pusher/__init__.py` & `powerapi-2.6.0/src/powerapi/pusher/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/pusher/handlers.py` & `powerapi-2.6.0/src/powerapi/pusher/handlers.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/pusher/pusher_actor.py` & `powerapi-2.6.0/src/powerapi/actor/state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Copyright (c) 2022, INRIA
-# Copyright (c) 2022, University of Lille
+# Copyright (c) 2018, INRIA
+# Copyright (c) 2018, University of Lille
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -23,70 +23,55 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import logging
-from powerapi.actor import Actor, State
-from powerapi.message import PoisonPillMessage, StartMessage
+from powerapi.actor.supervisor import Supervisor
+from powerapi.exception import UnknownMessageTypeException
+from powerapi.handler import Handler
+from powerapi.message import Message
 
-from powerapi.pusher.handlers import ReportHandler, PusherStartHandler, PusherPoisonPillMessageHandler
 
-
-class PusherState(State):
+class State:
     """
-    Pusher Actor State
-
-    Contains in addition to State values :
-      - The database interface
+    Base actor state.
     """
 
-    def __init__(self, actor, database, report_model):
+    def __init__(self, actor):
         """
-        :param BaseDB database: Database for saving data.
+        Initialize the actor state.
+        :param actor: The actor instance
         """
-        State.__init__(self, actor)
-
-        #: (BaseDB): Database for saving data.
-        self.database = database
+        self.actor = actor
 
-        #: (Report): Type of the report that the pusher handle.
-        self.report_model = report_model
+        self.initialized = False
+        self.alive = True
 
-        #: (Dict): Buffer data.
-        self.buffer = []
-
-
-class PusherActor(Actor):
-    """
-    PusherActor class
+        self.handlers = {}
+        self.supervisor = Supervisor()
 
-    The Pusher allow to save Report sent by Formula.
-    """
+    def get_corresponding_handler(self, msg: Message) -> Handler:
+        """
+        Return the corresponding handler for the given message type.
+        :param msg: The message
+        :return: The handler for the given message type
+        :raises UnknownMessageTypeException: If the message type does not have a corresponding handler
+        """
+        try:
+            return self.handlers[msg.__class__.__name__]
+        except ValueError as e:
+            raise UnknownMessageTypeException() from e
 
-    def __init__(self, name, report_model, database, level_logger=logging.WARNING, timeout=1000, delay=100,
-                 max_size=50):
+    def add_handler(self, message_type: type[Message], handler: Handler, include_subclasses: bool = True):
         """
-        :param str name: Pusher name.
-        :param Report report_model: ReportModel
-        :param BaseDB database: Database use for saving data.
-        :param int level_logger: Define the level of the logger
-        :param int delay: number of ms before message containing in the buffer will be writen in database
-        :param int max_size: maximum of message that the buffer can store before write them in database
-        """
-        Actor.__init__(self, name, level_logger, timeout)
-
-        #: (State): State of the actor.
-        self.state = PusherState(self, database, report_model)
-        self.delay = delay
-        self.max_size = max_size
-
-    def setup(self):
-        """
-        Define StartMessage, PoisonPillMessage handlers and a handler for
-        each report type
-        """
-        self.add_handler(PoisonPillMessage, PusherPoisonPillMessageHandler(self.state))
-        self.add_handler(self.state.report_model, ReportHandler(self.state, self.delay, self.max_size))
-        self.add_handler(StartMessage, PusherStartHandler(self.state))
+        Add a handler for the given message type.
+        :param message_type: The message type
+        :param handler: The corresponding handler
+        :param include_subclasses: Whether to include subclasses of the message type
+        """
+        self.handlers[message_type.__name__] = handler
+
+        if include_subclasses:
+            for child_type in message_type.__subclasses__():
+                self.handlers[child_type.__name__] = handler
```

### Comparing `powerapi-2.5.0/src/powerapi/report/__init__.py` & `powerapi-2.6.0/src/powerapi/report/__init__.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/control_report.py` & `powerapi-2.6.0/src/powerapi/report/control_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/formula_report.py` & `powerapi-2.6.0/src/powerapi/report/formula_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/hwpc_report.py` & `powerapi-2.6.0/src/powerapi/report/hwpc_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/power_report.py` & `powerapi-2.6.0/src/powerapi/report/power_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/procfs_report.py` & `powerapi-2.6.0/src/powerapi/report/procfs_report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/report/report.py` & `powerapi-2.6.0/src/powerapi/report/report.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/utils/__init__.py` & `powerapi-2.6.0/src/powerapi/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from .json_stream import JsonStream
-from .tree import Tree
 from .utils import timestamp_to_datetime
```

### Comparing `powerapi-2.5.0/src/powerapi/utils/cli.py` & `powerapi-2.6.0/src/powerapi/utils/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,53 +23,36 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-def remove_first_characters(arg: str):
-    """
-    Remove the two first characters of arg if it has more than 2 characters, otherwise, it removes only the first one.
-    :param str arg: The string to remove the first characters
-    """
-    if len(arg) > 2:
-        return arg[2:]
-    return arg[1]
-
 
-def find_longest_string_in_list(string_list: list) -> str:
+def find_longest_string_in_list(strings: list[str]) -> str:
     """
-    Find the largest string contained in the given list
-    :param list string_list: list of strings
+    Find the longest string from a given list of string.
+    :param strings: List of strings
     """
-    max_len = 0
-    longest_string = ''
-    for name in string_list:
-        if len(name) > max_len:
-            longest_string = name
-            max_len = len(name)
-    return longest_string
+    return max(strings, key=len)
 
 
 def string_to_bool(bool_value: str):
     """
     Transforms a str to bool according to their content
     """
     return bool_value.lower() in ("yes", "true", "t", "1")
 
 
 def merge_dictionaries(source: dict, destination: dict) -> dict:
     """
-    Merge the dictionary source into destination
+    Recursively merge the source dictionary into destination.
     :param source: Dictionary to be merged
-    :param destination: dictionary that will modify with the source content
+    :param destination: Dictionary where the source will be merged to
     """
-    if len(source) > 0:
-        for current_source_key, current_source_value in source.items():
-            if not isinstance(current_source_value, dict) or current_source_key not in destination:
-                destination[current_source_key] = current_source_value
-            else:
-                destination[current_source_key] = merge_dictionaries(current_source_value,
-                                                                     destination[current_source_key])
+    for key, value in source.items():
+        if isinstance(value, dict) and key in destination and isinstance(destination[key], dict):
+            destination[key] = merge_dictionaries(value, destination[key])
+        else:
+            destination[key] = value
 
     return destination
```

### Comparing `powerapi-2.5.0/src/powerapi/utils/json_stream.py` & `powerapi-2.6.0/src/powerapi/utils/json_stream.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi/utils/utils.py` & `powerapi-2.6.0/src/powerapi/utils/utils.py`

 * *Files identical despite different names*

### Comparing `powerapi-2.5.0/src/powerapi.egg-info/PKG-INFO` & `powerapi-2.6.0/src/powerapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: powerapi
-Version: 2.5.0
+Version: 2.6.0
 Summary: PowerAPI is a middleware toolkit for building software-defined power meters.
 Author-email: PowerAPI Staff <powerapi-staff@inria.fr>
 License: BSD-3-Clause
 Project-URL: homepage, https://powerapi.org
 Project-URL: documentation, https://powerapi.readthedocs.org
 Project-URL: repository, https://github.com/powerapi-ng/powerapi
 Keywords: powerapi,energy,power-meter,green-computing
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyzmq>=18.1.0
 Requires-Dist: setproctitle>=1.1.8
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.1; extra == "test"
 Requires-Dist: pytest-asyncio>=0.20.1; extra == "test"
@@ -80,34 +78,42 @@
 
 ## Contributing
 If you would like to contribute code you can do so through GitHub by forking the repository and sending a pull request.
 
 When submitting code, please make every effort to [follow existing conventions and style](CONTRIBUTING.md) in order to keep the code as readable as possible.
 
 ## Publications
-* **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2021, Melbourne, Australia
-* **[Power Budgeting of Big Data Applications in Container-based Clusters](https://hal.inria.fr/hal-02904300)**: J. Enes, G. Fieni, R. Expósito, R. Rouvoy, J. Tourino. *IEEE Cluster*, September 2020, Kobe, Japan
-* **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128)**: G. Fieni, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). May 2020, Melbourne, Australia
-* **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379)**: Z. Ournani, M.C. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. *ACM/SPEC International Conference on Performance Engineering* (ICPE). April 2020, Edmonton, Canada
-* **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. *IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing* (CCGrid). April 2017, Spain, France
-* **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. *European Conference on Computer Systems* (EuroSys). April 2015, Bordeaux, France
-* **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. *Journal of Automated Software Engineering*, Springer, 2015
-* **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. *International Symposium On Applied Computing* (SAC), March 2014, Gyeongju, South Korea
-* **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. *J'innove en Nord Pas de Calais*, [NFID](http://www.jinnove.com)
-* **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. *ERCIM News, Special Theme: Smart Energy Systems*, 92,  pp.43-44. [ERCIM](http://www.ercim.eu), 2013
-* **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. *01 Business & Technologies*, 2013
-* **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. *ACM SIGOPS Operating Systems Review*, ACM, 2013, 47 (3)
-* **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Conference on Automated Software Engineering* (ASE), September 2012, Essen, Germany
-* **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. *International Workshop on Green and Sustainable Software* (GREENS), June 2012, Zurich, Switzerland
+- **[Evaluating the Impact of Java Virtual Machines on Energy Consumption](https://hal.inria.fr/hal-03275286v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat. _15th ACM/IEEE International Symposium on Empirical Software Engineering and Measurement_ (ESEM). October 2021, Bari, Italy.
+- **[SelfWatts: On-the-fly Selection of Performance Events to Optimize Software-defined Power Meters](https://hal.inria.fr/hal-03173410v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2021). May 2021, Melbourne, Australia.
+- **[SmartWatts: Self-Calibrating Software-Defined Power Meter for Containers](https://hal.inria.fr/hal-02470128v1)**: G. Fieni, R. Rouvoy, L. Seiturier. _20th IEEE/ACM International Symposium on Cluster, Cloud and Internet Computing_ (CCGRID 2020). May 2020, Melbourne, Australia.
+- **[Taming Energy Consumption Variations in Systems Benchmarking](https://hal.inria.fr/hal-02403379v1)**: Z. Ournani, MC. Belgaid, R. Rouvoy, P. Rust, J. Penhoat, L. Seinturier. _11th ACM/SPEC International Conference on Performance Engineering_ (ICPE'2020). April 2020, Edmonton, Canada.
+- **[The Next 700 CPU Power Models](https://hal.inria.fr/hal-01827132v2)**: M. Colmant, R. Rouvoy, M. Kurpicz, A. Sobe, P. Felber, L. Seinturier. _Elsevier Journal of Systems and Software_ (JSS). 144(10):382-396, Elsevier.
+- **[WattsKit: Software-Defined Power Monitoring of Distributed Systems](https://hal.inria.fr/hal-01439889)**: M. Colmant, P. Felber, R. Rouvoy, L. Seinturier. _IEEE/ACM International Symposium on Cluster, Cloud and Grid Computing_ (CCGrid). April 2017, Spain, France. pp.1-14.
+- **[Process-level Power Estimation in VM-based Systems](https://hal.inria.fr/hal-01130030)**: M. Colmant, M. Kurpicz, L. Huertas, R. Rouvoy, P. Felber, A. Sobe. _European Conference on Computer Systems_ (EuroSys). April 2015, Bordeaux, France. pp.1-14.
+- **[Monitoring Energy Hotspots in Software](https://hal.inria.fr/hal-01069142)**: A. Noureddine, R. Rouvoy, L. Seinturier. _Journal of Automated Software Engineering_, Springer, 2015, pp.1-42.
+- **[Unit Testing of Energy Consumption of Software Libraries](https://hal.inria.fr/hal-00912613)**: A. Noureddine, R. Rouvoy, L. Seinturier. _International Symposium On Applied Computing_ (SAC), March 2014, Gyeongju, South Korea. pp.1200-1205.
+- **[Informatique : Des logiciels mis au vert](http://www.jinnove.com/Actualites/Informatique-des-logiciels-mis-au-vert)**: L. Seinturier, R. Rouvoy. _J'innove en Nord Pas de Calais_, [NFID](http://www.jinnove.com), 2013.
+- **[PowerAPI: A Software Library to Monitor the Energy Consumed at the Process-Level](http://ercim-news.ercim.eu/en92/special/powerapi-a-software-library-to-monitor-the-energy-consumed-at-the-process-level)**: A. Bourdon, A. Noureddine, R. Rouvoy, L. Seinturier. _ERCIM News, Special Theme: Smart Energy Systems_, 92, pp.43-44. [ERCIM](http://www.ercim.eu), 2013.
+- **[Mesurer la consommation en énergie des logiciels avec précision](http://www.lifl.fr/digitalAssets/0/807_01info_130110_16_39.pdf)**: A. Bourdon, R. Rouvoy, L. Seinturier. _01 Business & Technologies_, 2013.
+- **[A review of energy measurement approaches](https://hal.inria.fr/hal-00912996v2)**: A. Noureddine, R. Rouvoy, L. Seinturier. _ACM SIGOPS Operating Systems Review_, ACM, 2013, 47 (3), pp.42-49.
+- **[Runtime Monitoring of Software Energy Hotspots](https://hal.inria.fr/hal-00715331)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Conference on Automated Software Engineering_ (ASE), September 2012, Essen, Germany. pp.160-169.
+- **[A Preliminary Study of the Impact of Software Engineering on GreenIT](https://hal.inria.fr/hal-00681560)**: A. Noureddine, A. Bourdon, R. Rouvoy, L. Seinturier. _International Workshop on Green and Sustainable Software_ (GREENS), June 2012, Zurich, Switzerland. pp.21-27.
 
 ## Use Cases
 PowerAPI is used in a variety of projects to address key challenges of GreenIT:
 * [SmartWatts](https://github.com/powerapi-ng/smartwatts-formula) is a self-adaptive power meter that can estimate the energy consumption of software containers in real-time.
 * [GenPack](https://hal.inria.fr/hal-01403486) provides a container scheduling strategy to minimize the energy footprint of cloud infrastructures.
 * [VirtualWatts](https://github.com/powerapi-ng/virtualwatts-formula) provides process-level power estimation of applications running in virtual machines.
 * [Web Energy Archive](http://webenergyarchive.com) ranks popular websites based on the energy footpring they imposes to browsers.
 * [Greenspector](https://greenspector.com) optimises the power consumption of software by identifying potential energy leaks in the source code.
 
+## Research Projects
+
+Currently, PowerAPI is used in two research projects:
+
+- [Distiller ANR Project](https://www.davidson.fr/blog/comment-reduire-limpact-environnemental-des-applications-cloud-davidson-consulting-inria-ovhcloud-orange-sassocient-pour-le-programme-de-recherche-distiller) that searches to reduce energy consumption of Cloud applications.
+- [Défi Pulse](https://www.inria.fr/fr/pulse-defi-qarnot-computing-ademe-calcul-intensif-hpc-environnement) studies how to valorize emissions from High Performance Computing (HPC) using as use case [Qarnot Computing's](https://qarnot.com/en) offers.
+
 ## License
 PowerAPI is licensed under the BSD-3-Clause License. See the [LICENSE](LICENSE) file for details.
 
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fpowerapi-ng%2Fpowerapi?ref=badge_large)
```

### Comparing `powerapi-2.5.0/src/powerapi.egg-info/SOURCES.txt` & `powerapi-2.6.0/src/powerapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,9 +78,8 @@
 src/powerapi/report/hwpc_report.py
 src/powerapi/report/power_report.py
 src/powerapi/report/procfs_report.py
 src/powerapi/report/report.py
 src/powerapi/utils/__init__.py
 src/powerapi/utils/cli.py
 src/powerapi/utils/json_stream.py
-src/powerapi/utils/tree.py
 src/powerapi/utils/utils.py
```

### Comparing `powerapi-2.5.0/src/powerapi.egg-info/requires.txt` & `powerapi-2.6.0/src/powerapi.egg-info/requires.txt`

 * *Files identical despite different names*

