# Comparing `tmp/openedx-events-9.7.0.tar.gz` & `tmp/openedx-events-9.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-events-9.7.0.tar", last modified: Thu Apr  4 17:57:41 2024, max compression
+gzip compressed data, was "openedx-events-9.8.0.tar", last modified: Thu Apr 11 22:51:59 2024, max compression
```

## Comparing `openedx-events-9.7.0.tar` & `openedx-events-9.8.0.tar`

### file list

```diff
@@ -1,75 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.064874 openedx-events-9.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2024-04-04 17:57:34.000000 openedx-events-9.7.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-04 17:57:34.000000 openedx-events-9.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-04 17:57:34.000000 openedx-events-9.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-04 17:57:41.064874 openedx-events-9.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-04 17:57:34.000000 openedx-events-9.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/analytics/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/content_authoring/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/content_authoring/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/enterprise/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/enterprise/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/event_bus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.056874 openedx-events-9.7.0/openedx_events/event_bus/avro/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/custom_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_avro.py
--rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/avro/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/event_bus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/event_bus/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/learning/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/learning/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/management/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/consume_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/management/commands/generate_avro_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_consume_events_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_generate_avro_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_producer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/test_tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/tooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-04 17:57:34.000000 openedx-events-9.7.0/openedx_events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/openedx_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17697 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 17:57:41.000000 openedx-events-9.7.0/openedx_events.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 17:57:34.000000 openedx-events-9.7.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-04 17:57:34.000000 openedx-events-9.7.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-04 17:57:41.064874 openedx-events-9.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-04 17:57:34.000000 openedx-events-9.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:57:41.060874 openedx-events-9.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 17:57:34.000000 openedx-events-9.7.0/tests/test_openedx_events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-11 22:51:51.000000 openedx-events-9.8.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-11 22:51:51.000000 openedx-events-9.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 22:51:51.000000 openedx-events-9.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17765 2024-04-11 22:51:59.127064 openedx-events-9.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-11 22:51:51.000000 openedx-events-9.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/analytics/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/analytics/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/content_authoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/content_authoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/content_authoring/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/content_authoring/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/enterprise/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/enterprise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/enterprise/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/enterprise/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/event_bus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.123064 openedx-events-9.8.0/openedx_events/event_bus/avro/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/custom_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12453 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/avro/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/event_bus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8502 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/event_bus/tests/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/learning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16849 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/learning/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12531 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/learning/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/management/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/management/commands/consume_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/management/commands/generate_avro_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/test_consume_events_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/test_generate_avro_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/test_producer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/test_tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/tooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-11 22:51:51.000000 openedx-events-9.8.0/openedx_events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/openedx_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17765 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 22:51:59.000000 openedx-events-9.8.0/openedx_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:51:59.127064 openedx-events-9.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-11 22:51:51.000000 openedx-events-9.8.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-11 22:51:51.000000 openedx-events-9.8.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 22:51:59.127064 openedx-events-9.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-11 22:51:51.000000 openedx-events-9.8.0/setup.py
```

### Comparing `openedx-events-9.7.0/CHANGELOG.rst` & `openedx-events-9.8.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[9.8.0] - 2024-04-11
+
+Added
+~~~~~
+* Added support for Python 3.11
+
 [9.7.0] - 2024-04-04
 --------------------
 Added
 ~~~~~~~
 * Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
 
 [9.6.0] - 2024-04-01
```

### Comparing `openedx-events-9.7.0/LICENSE.txt` & `openedx-events-9.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/PKG-INFO` & `openedx-events-9.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.7.0
+Version: 9.8.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,14 +163,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[9.8.0] - 2024-04-11
+
+Added
+~~~~~
+* Added support for Python 3.11
+
 [9.7.0] - 2024-04-04
 --------------------
 Added
 ~~~~~~~
 * Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
 
 [9.6.0] - 2024-04-01
```

### Comparing `openedx-events-9.7.0/README.rst` & `openedx-events-9.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/analytics/data.py` & `openedx-events-9.8.0/openedx_events/analytics/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/analytics/signals.py` & `openedx-events-9.8.0/openedx_events/analytics/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/apps.py` & `openedx-events-9.8.0/openedx_events/apps.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/content_authoring/data.py` & `openedx-events-9.8.0/openedx_events/content_authoring/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
     library_key = attr.ib(type=LibraryLocatorV2)
     usage_key = attr.ib(type=LibraryUsageLocatorV2)
 
 
 @attr.s(frozen=True)
 class ContentObjectData:
     """
-    Data about changed content object
+    Data about changed content object.
 
     Arguments:
         object_id (str): identifier of the Content object. This represents the id of the course or library block
         as a string. For example:
         block-v1:SampleTaxonomyOrg2+STC1+2023_1+type@vertical+block@f8de78f0897049ce997777a3a31b6ea0
     """
```

### Comparing `openedx-events-9.7.0/openedx_events/content_authoring/signals.py` & `openedx-events-9.8.0/openedx_events/content_authoring/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/data.py` & `openedx-events-9.8.0/openedx_events/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/enterprise/data.py` & `openedx-events-9.8.0/openedx_events/enterprise/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/enterprise/signals.py` & `openedx-events-9.8.0/openedx_events/enterprise/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/__init__.py` & `openedx-events-9.8.0/openedx_events/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/custom_serializers.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/custom_serializers.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/deserializer.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/schema.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/serializer.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_avro.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_deserializer.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_schema.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_serializer.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/avro/tests/test_utilities.py` & `openedx-events-9.8.0/openedx_events/event_bus/avro/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/event_bus/tests/test_loader.py` & `openedx-events-9.8.0/openedx_events/event_bus/tests/test_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Tests for event bus implementation loader.
 """
 
 import copy
+import sys
 import warnings
 from contextlib import contextmanager
 from unittest import TestCase
 
+import pytest
 from django.test import override_settings
 
 from openedx_events.data import EventsMetadata
 from openedx_events.event_bus import _try_load, get_producer, make_single_consumer, merge_producer_configs
 from openedx_events.learning.signals import SESSION_LOGIN_COMPLETED
 
 
@@ -79,26 +81,41 @@
         ]):
             loaded = _try_load(
                 setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
 
+    @pytest.mark.skipif(sys.version_info > (3, 9), reason="Python 3.8.x required")  # Temporary until 3.8 is dropped
     @override_settings(EB_LOAD_PATH='builtins.dict')
     def test_bad_args_for_callable(self):
         with assert_warnings([
                 "Failed to load <class 'dict'> from setting EB_LOAD_PATH: "
                 "TypeError('type object argument after * must be an iterable, not int'); "
                 "component will be inactive"
         ]):
             loaded = _try_load(
                 setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
                 expected_class=dict, default={'def': 'ault'},
             )
         assert loaded == {'def': 'ault'}
+
+    @pytest.mark.skipif(sys.version_info < (3, 9), reason="Python 3.11.x required")  # Temporary until 3.8 is dropped
+    @override_settings(EB_LOAD_PATH='builtins.dict')
+    def test_bad_args_for_callable(self):
+        with assert_warnings([
+                "Failed to load <class 'dict'> from setting EB_LOAD_PATH: "
+                "TypeError('dict() argument after * must be an iterable, not int'); "
+                "component will be inactive"
+        ]):
+            loaded = _try_load(
+                setting_name="EB_LOAD_PATH", args=(1), kwargs={'2': 3},
+                expected_class=dict, default={'def': 'ault'},
+            )
+        assert loaded == {'def': 'ault'}
 
 
 class TestProducer(TestCase):
 
     @override_settings(EVENT_BUS_PRODUCER=None)
     def test_default_does_nothing(self):
         """
```

### Comparing `openedx-events-9.7.0/openedx_events/exceptions.py` & `openedx-events-9.8.0/openedx_events/exceptions.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/learning/data.py` & `openedx-events-9.8.0/openedx_events/learning/data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/learning/signals.py` & `openedx-events-9.8.0/openedx_events/learning/signals.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/management/commands/consume_events.py` & `openedx-events-9.8.0/openedx_events/management/commands/consume_events.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/management/commands/generate_avro_schemas.py` & `openedx-events-9.8.0/openedx_events/management/commands/generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/tests/test_consume_events_command.py` & `openedx-events-9.8.0/openedx_events/tests/test_consume_events_command.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/tests/test_data.py` & `openedx-events-9.8.0/openedx_events/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/tests/test_generate_avro_schemas.py` & `openedx-events-9.8.0/openedx_events/tests/test_generate_avro_schemas.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/tests/test_producer_config.py` & `openedx-events-9.8.0/openedx_events/tests/test_producer_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,26 +38,24 @@
         """
         mock_send = Mock()
         mock_producer.return_value = mock_send
         # XBLOCK_PUBLISHED has three configurations where 2 configurations have set enabled as True.
         XBLOCK_PUBLISHED.send_event(xblock_info=self.xblock_info)
         mock_send.send.assert_called()
         mock_send.send.call_count = 2
+        expected_call_args = [
+            {'topic': 'enabled_topic_a', 'event_key_field': 'xblock_info.usage_key'},
+            {'topic': 'enabled_topic_b', 'event_key_field': 'xblock_info.usage_key'}
+        ]
 
         # check that call_args_list only consists of enabled topics.
         call_args = mock_send.send.call_args_list[0][1]
-        self.assertDictContainsSubset(
-            {'topic': 'enabled_topic_a', 'event_key_field': 'xblock_info.usage_key'},
-            call_args
-        )
+        self.assertEqual(call_args, {**call_args, **expected_call_args[0]})
         call_args = mock_send.send.call_args_list[1][1]
-        self.assertDictContainsSubset(
-            {'topic': 'enabled_topic_b', 'event_key_field': 'xblock_info.usage_key'},
-            call_args
-        )
+        self.assertEqual(call_args, {**call_args, **expected_call_args[1]})
 
     @patch("openedx_events.apps.logger")
     @patch('openedx_events.apps.get_producer')
     def test_send_events_with_custom_metadata_not_replayed_by_handler(self, mock_producer, mock_logger):
         """
         Check wheter XBLOCK_PUBLISHED is connected to the handler and the handler
         do not send any events as the signal is marked "from_event_bus".
```

### Comparing `openedx-events-9.7.0/openedx_events/tests/test_tooling.py` & `openedx-events-9.8.0/openedx_events/tests/test_tooling.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,16 +107,17 @@
             "source": "openedx/lms/web",
             "sourcehost": "edx.devstack.lms",
             "sourcelib": [0, 1, 0],
             "time": expected_time,
         }
 
         metadata = self.public_signal.generate_signal_metadata()
+        metadata_as_dict = attr.asdict(metadata)
 
-        self.assertDictContainsSubset(expected_metadata, attr.asdict(metadata))
+        self.assertEqual(metadata_as_dict, {**expected_metadata, **metadata_as_dict})
         self.assertIsInstance(metadata.id, UUID)
 
     @override_settings(SERVICE_VARIANT="lms")
     @patch("openedx_events.data.openedx_events")
     @patch("openedx_events.data.socket")
     def test_generate_signal_metadata_with_valid_time(self, socket_mock, events_package_mock):
         """
@@ -134,16 +135,17 @@
             "source": "openedx/lms/web",
             "sourcehost": "edx.devstack.lms",
             "sourcelib": [0, 1, 0],
             "time": expected_time,
         }
 
         metadata = self.public_signal.generate_signal_metadata(time=expected_time)
+        metadata_as_dict = attr.asdict(metadata)
 
-        self.assertDictContainsSubset(expected_metadata, attr.asdict(metadata))
+        self.assertEqual(metadata_as_dict, {**expected_metadata, **metadata_as_dict})
         self.assertIsInstance(metadata.id, UUID)
 
     @ddt.data(
         (1, TypeError, "'time' must be <class 'datetime.datetime'",),
         # WARNING: utcnow() has no timezone, and could be misinterpreted in local time
         (datetime.datetime.utcnow(), ValueError, "'time' must have timezone.utc",),
     )
```

### Comparing `openedx-events-9.7.0/openedx_events/tests/utils.py` & `openedx-events-9.8.0/openedx_events/tests/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/tooling.py` & `openedx-events-9.8.0/openedx_events/tooling.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events/utils.py` & `openedx-events-9.8.0/openedx_events/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-events-9.7.0/openedx_events.egg-info/PKG-INFO` & `openedx-events-9.8.0/openedx_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-events
-Version: 9.7.0
+Version: 9.8.0
 Summary: Open edX events from the Hooks Extensions Framework
 Home-page: https://github.com/openedx/openedx-events
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -163,14 +163,21 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ----------
+
+[9.8.0] - 2024-04-11
+
+Added
+~~~~~
+* Added support for Python 3.11
+
 [9.7.0] - 2024-04-04
 --------------------
 Added
 ~~~~~~~
 * Added new ``SUBSIDY_REDEEMED`` and ``SUBSIDY_REDEMPTION_REVERSED`` events in enterprise.
 
 [9.6.0] - 2024-04-01
```

### Comparing `openedx-events-9.7.0/openedx_events.egg-info/SOURCES.txt` & `openedx-events-9.8.0/openedx_events.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,9 +50,8 @@
 openedx_events/tests/test_consume_events_command.py
 openedx_events/tests/test_data.py
 openedx_events/tests/test_generate_avro_schemas.py
 openedx_events/tests/test_producer_config.py
 openedx_events/tests/test_tooling.py
 openedx_events/tests/utils.py
 requirements/base.in
-requirements/constraints.txt
-tests/test_openedx_events.py
+requirements/constraints.txt
```

### Comparing `openedx-events-9.7.0/requirements/constraints.txt` & `openedx-events-9.8.0/requirements/constraints.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 # Common constraints for openedx repos
 -c https://raw.githubusercontent.com/openedx/edx-lint/master/edx_lint/files/common_constraints.txt
 
 # Temporary solution since this version raises RecursionError for test_generate_avro_schemas.py
 # This should be removed once the issue is fixed with a new astroid release or with a test_generate_avro_schemas.py
 # module refactor.
 astroid<3.0.0
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `openedx-events-9.7.0/setup.py` & `openedx-events-9.8.0/setup.py`

 * *Files identical despite different names*

