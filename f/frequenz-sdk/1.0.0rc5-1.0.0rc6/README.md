# Comparing `tmp/frequenz-sdk-1.0.0rc5.tar.gz` & `tmp/frequenz-sdk-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-sdk-1.0.0rc5.tar", last modified: Mon Feb 26 14:20:39 2024, max compression
+gzip compressed data, was "frequenz-sdk-1.0.0rc6.tar", last modified: Fri Apr 12 14:04:26 2024, max compression
```

## Comparing `frequenz-sdk-1.0.0rc5.tar` & `frequenz-sdk-1.0.0rc6.tar`

### file list

```diff
@@ -1,148 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.059469 frequenz-sdk-1.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-02-26 14:20:39.059469 frequenz-sdk-1.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.039469 frequenz-sdk-1.0.0rc5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/examples/battery_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 14:20:39.059469 frequenz-sdk-1.0.0rc5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.039469 frequenz-sdk-1.0.0rc5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.039469 frequenz-sdk-1.0.0rc5/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.039469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_api_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_singleton_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/
--rw-r--r--   0 runner    (1001) docker     (127)    23022 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_background_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_channel_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_config_managing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17211 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11507 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_matryoshka.py
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_sorted_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_run_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.043469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18012 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29214 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/power_distributing.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/config/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/_power_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/client/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23169 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/client/_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/client/_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.047469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    18231 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/_component_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/_component_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    36930 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.051469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_fuse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_grid_frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)    16481 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_moving_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    38921 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)    30072 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_resampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.051469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_voltage_streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.051469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18108 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    21520 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.051469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4319 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.051469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    40547 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.055469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.055469 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/logical_meter/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/logical_meter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-02-26 14:20:22.000000 frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 14:20:39.055469 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-02-26 14:20:38.000000 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-02-26 14:20:39.000000 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 14:20:38.000000 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-26 14:20:38.000000 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-26 14:20:38.000000 frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/examples/battery_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:04:26.515937 frequenz-sdk-1.0.0rc6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.491938 frequenz-sdk-1.0.0rc6/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_singleton_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.495938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/
+-rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_background_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_channel_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_config_managing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_matryoshka.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_sorted_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_run_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25731 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.499938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8031 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29217 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/power_distributing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24626 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_power_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36983 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/component_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_fuse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_grid_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_moving_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38921 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30181 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.503938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_voltage_streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40624 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7449 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8923 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.507938 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_result_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-04-12 14:04:19.000000 frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:26.511937 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 14:04:26.000000 frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/top_level.txt
```

### Comparing `frequenz-sdk-1.0.0rc5/LICENSE` & `frequenz-sdk-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/PKG-INFO` & `frequenz-sdk-1.0.0rc6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-sdk-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
@@ -17,15 +17,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: frequenz-api-microgrid<0.16.0,>=0.15.3
-Requires-Dist: frequenz-channels==1.0.0b2
+Requires-Dist: frequenz-channels<2.0.0,>=1.0.0-rc1
+Requires-Dist: frequenz-client-microgrid<0.4.0,>=0.3.0
 Requires-Dist: google-api-python-client<3,>=2.71
 Requires-Dist: grpcio<2,>=1.54.2
 Requires-Dist: grpcio-tools<2,>=1.54.2
 Requires-Dist: networkx<4,>=2.8
 Requires-Dist: numpy<2,>=1.24.2
 Requires-Dist: protobuf<5,>=4.21.6
 Requires-Dist: pydantic<3,>=2.3
@@ -33,53 +34,53 @@
 Requires-Dist: tqdm<5,>=4.38.0
 Requires-Dist: typing_extensions<5,>=4.6.1
 Requires-Dist: watchfiles>=0.15.0
 Provides-Extra: dev-flake8
 Requires-Dist: flake8==7.0.0; extra == "dev-flake8"
 Requires-Dist: flake8-docstrings==1.7.0; extra == "dev-flake8"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "dev-flake8"
-Requires-Dist: pydoclint==0.3.8; extra == "dev-flake8"
+Requires-Dist: pydoclint==0.4.1; extra == "dev-flake8"
 Requires-Dist: pydocstyle==6.3.0; extra == "dev-flake8"
 Provides-Extra: dev-examples
-Requires-Dist: polars==0.20.2; extra == "dev-examples"
+Requires-Dist: polars==0.20.18; extra == "dev-examples"
 Provides-Extra: dev-formatting
-Requires-Dist: black==24.1.1; extra == "dev-formatting"
+Requires-Dist: black==24.3.0; extra == "dev-formatting"
 Requires-Dist: isort==5.13.2; extra == "dev-formatting"
 Provides-Extra: dev-mkdocs
-Requires-Dist: black==24.1.1; extra == "dev-mkdocs"
-Requires-Dist: Markdown==3.5.1; extra == "dev-mkdocs"
+Requires-Dist: black==24.3.0; extra == "dev-mkdocs"
+Requires-Dist: Markdown==3.6; extra == "dev-mkdocs"
 Requires-Dist: mike==2.0.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == "dev-mkdocs"
-Requires-Dist: mkdocs-material==9.5.3; extra == "dev-mkdocs"
-Requires-Dist: mkdocstrings[python]==0.24.0; extra == "dev-mkdocs"
-Requires-Dist: frequenz-repo-config[lib]==0.7.4; extra == "dev-mkdocs"
+Requires-Dist: mkdocs-material==9.5.16; extra == "dev-mkdocs"
+Requires-Dist: mkdocstrings[python]==0.24.1; extra == "dev-mkdocs"
+Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-mkdocs"
 Provides-Extra: dev-mypy
-Requires-Dist: mypy==1.8.0; extra == "dev-mypy"
+Requires-Dist: mypy==1.9.0; extra == "dev-mypy"
 Requires-Dist: grpc-stubs==1.24.12; extra == "dev-mypy"
-Requires-Dist: types-Markdown==3.5.0.3; extra == "dev-mypy"
+Requires-Dist: types-Markdown==3.6.0.20240316; extra == "dev-mypy"
 Requires-Dist: types-protobuf==4.24.0.20240129; extra == "dev-mypy"
-Requires-Dist: types-setuptools==69.0.0.20240125; extra == "dev-mypy"
+Requires-Dist: types-setuptools==69.2.0.20240317; extra == "dev-mypy"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-mypy"
 Provides-Extra: dev-noxfile
 Requires-Dist: nox==2023.4.22; extra == "dev-noxfile"
-Requires-Dist: frequenz-repo-config[lib]==0.7.4; extra == "dev-noxfile"
+Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-noxfile"
 Provides-Extra: dev-pylint
-Requires-Dist: pylint==3.0.3; extra == "dev-pylint"
+Requires-Dist: pylint==3.1.0; extra == "dev-pylint"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-pylint"
 Provides-Extra: dev-pytest
-Requires-Dist: pytest==7.4.4; extra == "dev-pytest"
-Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.7.4; extra == "dev-pytest"
-Requires-Dist: pytest-mock==3.12.0; extra == "dev-pytest"
-Requires-Dist: pytest-asyncio==0.23.3; extra == "dev-pytest"
+Requires-Dist: pytest==8.1.1; extra == "dev-pytest"
+Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.1; extra == "dev-pytest"
+Requires-Dist: pytest-mock==3.14.0; extra == "dev-pytest"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev-pytest"
 Requires-Dist: time-machine==2.12.0; extra == "dev-pytest"
-Requires-Dist: async-solipsism==0.5; extra == "dev-pytest"
+Requires-Dist: async-solipsism==0.6; extra == "dev-pytest"
 Requires-Dist: frequenz-sdk[dev-examples]; extra == "dev-pytest"
-Requires-Dist: hypothesis==6.92.1; extra == "dev-pytest"
+Requires-Dist: hypothesis==6.100.0; extra == "dev-pytest"
 Provides-Extra: dev
 Requires-Dist: frequenz-sdk[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]; extra == "dev"
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
```

### Comparing `frequenz-sdk-1.0.0rc5/README.md` & `frequenz-sdk-1.0.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/examples/battery_pool.py` & `frequenz-sdk-1.0.0rc6/examples/battery_pool.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 
 """Script with an example how to use BatteryPool."""
 
 
 import asyncio
 import logging
 from datetime import timedelta
-from typing import Any
 
-from frequenz.channels import Receiver
-from frequenz.channels.util import MergeNamed
+from frequenz.channels import merge
 
 from frequenz.sdk import microgrid
 from frequenz.sdk.actor import ResamplerConfig
 
 HOST = "microgrid.sandbox.api.frequenz.io"  # it should be the host name.
 PORT = 61060
 
@@ -27,21 +25,20 @@
     await microgrid.initialize(
         host=HOST,
         port=PORT,
         resampler_config=ResamplerConfig(resampling_period=timedelta(seconds=1.0)),
     )
 
     battery_pool = microgrid.battery_pool()
-    receivers: dict[str, Receiver[Any]] = {
-        "soc": battery_pool.soc.new_receiver(maxsize=1),
-        "capacity": battery_pool.capacity.new_receiver(maxsize=1),
+    receivers = [
+        battery_pool.soc.new_receiver(limit=1),
+        battery_pool.capacity.new_receiver(limit=1),
         # pylint: disable=protected-access
-        "power_bounds": battery_pool._system_power_bounds.new_receiver(maxsize=1),
+        battery_pool._system_power_bounds.new_receiver(limit=1),
         # pylint: enable=protected-access
-    }
+    ]
 
-    merged_channel = MergeNamed[Any](**receivers)
-    async for metric_name, metric in merged_channel:
-        print(f"Received new {metric_name}: {metric}")
+    async for metric in merge(*receivers):
+        print(f"Received new metric: {metric}")
 
 
 asyncio.run(main())
```

### Comparing `frequenz-sdk-1.0.0rc5/pyproject.toml` & `frequenz-sdk-1.0.0rc6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 [build-system]
 requires = [
   "setuptools == 69.0.3",
   "setuptools_scm[toml] == 8.0.4",
-  "frequenz-repo-config[lib] == 0.7.4",
+  "frequenz-repo-config[lib] == 0.9.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-sdk"
 description = "A development kit to interact with the Frequenz development platform"
 readme = "README.md"
@@ -26,15 +26,16 @@
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
   "frequenz-api-microgrid >= 0.15.3, < 0.16.0",
   # Make sure to update the mkdocs.yml file when
   # changing the version
   # (plugins.mkdocstrings.handlers.python.import)
-  "frequenz-channels == 1.0.0b2",
+  "frequenz-channels >= 1.0.0-rc1, < 2.0.0",
+  "frequenz-client-microgrid >= 0.3.0, < 0.4.0",
   "google-api-python-client >= 2.71, < 3",
   "grpcio >= 1.54.2, < 2",
   "grpcio-tools >= 1.54.2, < 2",
   "networkx >= 2.8, < 4",
   "numpy >= 1.24.2, < 2",
   "protobuf >= 4.21.6, < 5",
   "pydantic >= 2.3, < 3",
@@ -50,55 +51,55 @@
 email = "floss@frequenz.com"
 
 [project.optional-dependencies]
 dev-flake8 = [
   "flake8 == 7.0.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
-  "pydoclint == 0.3.8",
+  "pydoclint == 0.4.1",
   "pydocstyle == 6.3.0",
 ]
-dev-examples = ["polars == 0.20.2"]
-dev-formatting = ["black == 24.1.1", "isort == 5.13.2"]
+dev-examples = ["polars == 0.20.18"]
+dev-formatting = ["black == 24.3.0", "isort == 5.13.2"]
 dev-mkdocs = [
-  "black == 24.1.1",
-  "Markdown==3.5.1",
+  "black == 24.3.0",
+  "Markdown==3.6",
   "mike == 2.0.0",
   "mkdocs-gen-files == 0.5.0",
   "mkdocs-literate-nav == 0.6.1",
   "mkdocs-macros-plugin == 1.0.5",
-  "mkdocs-material == 9.5.3",
-  "mkdocstrings[python] == 0.24.0",
-  "frequenz-repo-config[lib] == 0.7.4",
+  "mkdocs-material == 9.5.16",
+  "mkdocstrings[python] == 0.24.1",
+  "frequenz-repo-config[lib] == 0.9.1",
 ]
 dev-mypy = [
-  "mypy == 1.8.0",
+  "mypy == 1.9.0",
   "grpc-stubs == 1.24.12",               # This dependency introduces breaking changes in patch releases
-  "types-Markdown == 3.5.0.3",
+  "types-Markdown == 3.6.0.20240316",
   "types-protobuf == 4.24.0.20240129",
-  "types-setuptools == 69.0.0.20240125",
+  "types-setuptools == 69.2.0.20240317",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.7.4"]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[lib] == 0.9.1"]
 dev-pylint = [
-  "pylint == 3.0.3",
+  "pylint == 3.1.0",
   # For checking the noxfile, docs/ script, and tests
   "frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]",
 ]
 dev-pytest = [
-  "pytest == 7.4.4",
-  "frequenz-repo-config[extra-lint-examples] == 0.7.4",
-  "pytest-mock == 3.12.0",
-  "pytest-asyncio == 0.23.3",
+  "pytest == 8.1.1",
+  "frequenz-repo-config[extra-lint-examples] == 0.9.1",
+  "pytest-mock == 3.14.0",
+  "pytest-asyncio == 0.23.6",
   "time-machine == 2.12.0",
-  "async-solipsism == 0.5",
+  "async-solipsism == 0.6",
   # For checking docstring code examples
   "frequenz-sdk[dev-examples]",
-  "hypothesis == 6.92.1",
+  "hypothesis == 6.100.0",
 ]
 dev = [
   "frequenz-sdk[dev-mkdocs,dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]",
 ]
 
 [project.urls]
 Documentation = "https://frequenz-floss.github.io/frequenz-sdk-python/"
@@ -139,21 +140,24 @@
 ignore-docstrings = ['yes']
 ignore-imports = ['no']
 min-similarity-lines = 40
 
 [tool.pylint.messages_control]
 disable = [
   "too-few-public-methods",
+  "too-many-return-statements",
   # disabled because it conflicts with isort
   "wrong-import-order",
   "ungrouped-imports",
   # pylint's unsubscriptable check is buggy and is not needed because
   # it is a type-check, for which we already have mypy.
   "unsubscriptable-object",
   # Checked by flake8
+  "redefined-outer-name",
+  "unused-import",
   "line-too-long",
   "redefined-outer-name",
   "unnecessary-lambda-assignment",
   "unused-import",
   "unused-variable",
 ]
 
@@ -186,14 +190,12 @@
   "async_solipsism.*",
   "grpc.aio",
   "grpc.aio.*",
   "mkdocs_macros.*",
   # The available stubs packages are outdated or incomplete (WIP/experimental):
   # https://github.com/frequenz-floss/frequenz-sdk-python/issues/430
   "networkx",
-  "sybil",
-  "sybil.*",
 ]
 ignore_missing_imports = true
 
 [tool.setuptools_scm]
 version_scheme = "post-release"
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_asyncio.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_asyncio.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_channels.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_channels.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,50 +5,52 @@
 
 import abc
 import asyncio
 import typing
 
 from frequenz.channels import Receiver
 
-T = typing.TypeVar("T")
+from ._asyncio import cancel_and_await
 
+T_co = typing.TypeVar("T_co", covariant=True)
 
-class ReceiverFetcher(typing.Generic[T], typing.Protocol):
+
+class ReceiverFetcher(typing.Generic[T_co], typing.Protocol):
     """An interface that just exposes a `new_receiver` method."""
 
     @abc.abstractmethod
-    def new_receiver(self, *, maxsize: int = 50) -> Receiver[T]:
+    def new_receiver(self, *, limit: int = 50) -> Receiver[T_co]:
         """Get a receiver from the channel.
 
         Args:
-            maxsize: The maximum size of the receiver.
+            limit: The maximum size of the receiver.
 
         Returns:
             A receiver instance.
         """
 
 
 class _Sentinel:
     """A sentinel to denote that no value has been received yet."""
 
 
-class LatestValueCache(typing.Generic[T]):
+class LatestValueCache(typing.Generic[T_co]):
     """A cache that stores the latest value in a receiver."""
 
-    def __init__(self, receiver: Receiver[T]) -> None:
+    def __init__(self, receiver: Receiver[T_co]) -> None:
         """Create a new cache.
 
         Args:
             receiver: The receiver to cache.
         """
         self._receiver = receiver
-        self._latest_value: T | _Sentinel = _Sentinel()
+        self._latest_value: T_co | _Sentinel = _Sentinel()
         self._task = asyncio.create_task(self._run())
 
-    def get(self) -> T:
+    def get(self) -> T_co:
         """Return the latest value that has been received.
 
         This raises a `ValueError` if no value has been received yet. Use `has_value` to
         check whether a value has been received yet, before trying to access the value,
         to avoid the exception.
 
         Returns:
@@ -68,7 +70,11 @@
             `True` if a value has been received, `False` otherwise.
         """
         return not isinstance(self._latest_value, _Sentinel)
 
     async def _run(self) -> None:
         async for value in self._receiver:
             self._latest_value = value
+
+    async def stop(self) -> None:
+        """Stop the cache."""
+        await cancel_and_await(self._task)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_constants.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_constants.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_math.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_math.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/_internal/_singleton_meta.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/_internal/_singleton_meta.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/__init__.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,36 +66,36 @@
        the [Python `asyncio`
        documentation](https://docs.python.org/3/library/asyncio-task.html#asyncio.create_task).
 
 
 ### The `run()` Function
 
 The [`run()`][frequenz.sdk.actor.run] function can start many actors at once and waits
-for them to finish. If any of the actors are stopped with errors, the errors will be
+for them to finish. If any of the actors is stopped with errors, the errors will be
 logged.
 
 ???+ example
 
     ```python
     from frequenz.sdk.actor import Actor, run
 
     class MyActor(Actor):
         async def _run(self) -> None:
             print("Hello World!")
 
     await run(MyActor()) # (1)!
     ```
 
-    1. This line will block until the actor is stopped.
+    1. This line will block until the actor completes its execution or is manually stopped.
 
 ### Async Context Manager
 
 When an actor is used as an [async context manager], it is started when the
 `async with` block is entered and stopped automatically when the block is exited
-(even if an exception is raised).
+(even if an unhandled exception is raised).
 
 ???+ example
 
     ```python
     from frequenz.sdk.actor import Actor
 
     class MyActor(Actor):
@@ -112,15 +112,15 @@
     2. [`stop()`][frequenz.sdk.actor.Actor.stop] is called automatically when exiting
         the `async with` block.
 
 ### The `start()` Method
 
 When using the [`start()`][frequenz.sdk.actor.Actor.start] method, the actor is
 started in the background and the method returns immediately. The actor will
-continue to run until it is **manually** stopped.
+continue to run until it is **manually** stopped or until it completes its execution.
 
 ???+ example
 
     ```python
     from frequenz.sdk.actor import Actor
 
     class MyActor(Actor):
@@ -199,27 +199,29 @@
     2. We accept an `input` argument that will be used to receive messages from
         a channel.
     3. We accept an `output` argument that will be used to send messages to a channel.
     4. We accept an optional `name` argument that will be used to identify the actor in
         logs.
     5. We call [`Actor.__init__()`][frequenz.sdk.actor.Actor.__init__] to make sure the
         actor is properly initialized.
-    6. We store the `input` argument in a *private* instance variable to use it later.
-    7. We store the `output` argument in a *private* instance variable to use it later.
+    6. We store the `input` argument in a *private* attribute to use it later.
+    7. We store the `output` argument in a *private* attribute to use it later.
 
 ### The `_run()` Method
 
 The abstract `_run()` method is called automatically by the base class when the actor is
 [started][frequenz.sdk.actor.Actor.start].
 
 Normally an actor should run forever (or until it is
 [stopped][frequenz.sdk.actor.Actor.stop]), so it is very common to have an infinite loop
 in the `_run()` method, typically receiving messages from one or more channels
 ([receivers][frequenz.channels.Receiver]), processing them and sending the results to
 other channels ([senders][frequenz.channels.Sender]).
+However, it is worth noting that an actor can also be designed for a one-time execution
+or a limited number of runs, terminating upon completion.
 
 ???+ example "Example echo actor"
 
     ```python
     from frequenz.channels import Receiver, Sender
     from frequenz.sdk.actor import Actor
 
@@ -379,29 +381,29 @@
     output_channel: Broadcast[str] = Broadcast("Actor2 output")
 
     input_sender = input_channel.new_sender()
     output_receiver = output_channel.new_receiver()
 
     async with (  # (5)!
         Actor1(input_channel.new_receiver(), middle_channel.new_sender(), "actor1"),
-        Actor2(middle_channel.new_receiver(), output_channel.new_sender(), "actor1"),
+        Actor2(middle_channel.new_receiver(), output_channel.new_sender(), "actor2"),
     ):
         await input_sender.send("Hello")  # (6)!
         msg = await output_receiver.receive()  # (7)!
         print(msg)  # (10)!
     # (11)!
 
 if __name__ == "__main__":  # (3)!
     asyncio.run(main())
 ```
 
 1. We define 2 actors: `Actor1` and `Actor2` that will just forward a message
    from an input channel to an output channel, adding some text.
 
-2. We define an async `main()` function with the main logic of our [asyncio][] program.
+2. We define an async `main()` function within the main logic of our [asyncio][] program.
 
 3. We start the `main()` function in the async loop using [`asyncio.run()`][asyncio.run].
 
 4. We create a bunch of [broadcast][frequenz.channels.Broadcast]
    [channels][frequenz.channels] to connect our actors.
 
     * `input_channel` is the input channel for `Actor1`.
@@ -521,16 +523,16 @@
     asyncio.run(main())
 ```
 
 1. We define an `EchoActor` that receives messages from two channels and sends
     them to another channel.
 
 2. We implement the [`_run()`][_run] method that will receive messages from the two
-    channels using and send them to the output channel. The `run()` method will stop if
-    a `False` message is received.
+    channels using [`select()`][frequenz.channels.util.select] and send them to the
+    output channel. The `run()` method will stop if a `False` message is received.
 
 3. We create the channels that will be used with the actor.
 
 4. We create the actor and connect it to the channels by creating new receivers and
     senders from the channels.
 
 5. We create a receiver for the `echo_channel` to eventually receive the messages sent
@@ -552,16 +554,15 @@
     `input_channel_1` (`True`) and the second from `input_channel_1` (`False`).
 
 11. The [`selected_from()`][frequenz.channels.util.selected_from] function will return
     `True` for the `input_channel_1` receiver. `selected.value` holds the received
     message, so `"Received from receiver_1: True"` will be printed and `True` will be
     sent to the `output` channel.
 
-12. Since `selected.value` is `True`, the loop will continue, going back to the and the
-    the loop will continue, going back to the
+12. Since `selected.value` is `True`, the loop will continue, going back to the
     [`select()`][frequenz.channels.util.select] function.
 
 13. The [`selected_from()`][frequenz.channels.util.selected_from] function will return
     `False` for the `input_channel_1` receiver and `True` for the `input_channel_2`
     receiver. The message stored in `selected.value` will now be `False`, so
     `"Received from receiver_2: False"` will be printed and `False` will be sent to the
     `output` channel.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_actor.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,21 +69,23 @@
         # Not just for the restart-delay but actually for the n_restarts counter as well.
         if iteration > 0:
             delay = self.RESTART_DELAY.total_seconds()
             _logger.info("Actor %s: Waiting %s seconds...", self, delay)
             await asyncio.sleep(delay)
 
     async def _run_loop(self) -> None:
-        """Run this actor's task in a loop until `_restart_limit` is reached.
+        """Run the actor's task continuously, managing restarts, cancellation, and termination.
+
+        This method handles the execution of the actor's task, including
+        restarts for unhandled exceptions, cancellation, or normal termination.
 
         Raises:
-            asyncio.CancelledError: If this actor's `_run()` gets cancelled.
-            Exception: If this actor's `_run()` raises any other `Exception` and reached
-                the maximum number of restarts.
-            BaseException: If this actor's `_run()` raises any other `BaseException`.
+            asyncio.CancelledError: If the actor's `_run()` method is cancelled.
+            Exception: If the actor's `_run()` method raises any other exception.
+            BaseException: If the actor's `_run()` method raises any base exception.
         """
         _logger.info("Actor %s: Started.", self)
         n_restarts = 0
         while True:
             try:
                 await self._delay_if_restart(n_restarts)
                 await self._run()
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_background_service.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_background_service.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_channel_registry.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_channel_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,17 @@
             if _logger.isEnabledFor(logging.DEBUG):
                 _logger.debug(
                     "Creating a new channel for key %r with type %s at:\n%s",
                     key,
                     message_type,
                     "".join(traceback.format_stack(limit=10)[:9]),
                 )
-            self._channels[key] = _Entry(message_type, Broadcast(f"{self._name}-{key}"))
+            self._channels[key] = _Entry(
+                message_type, Broadcast(name=f"{self._name}-{key}")
+            )
 
         entry = self._channels[key]
         if entry.message_type is not message_type:
             exception = ValueError(
                 f"Type mismatch, a channel for key {key!r} exists and the requested "
                 f"message type {message_type} is not the same as the existing "
                 f"message type {entry.message_type}."
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_config_managing.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_config_managing.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import pathlib
 import tomllib
 from collections import abc
 from typing import Any, assert_never
 
 from frequenz.channels import Sender
-from frequenz.channels.util import FileWatcher
+from frequenz.channels.file_watcher import EventType, FileWatcher
 
 from ..actor._actor import Actor
 from ..config import Config
 
 _logger = logging.getLogger(__name__)
 
 
@@ -30,15 +30,15 @@
     reading too.
     """
 
     def __init__(
         self,
         config_path: pathlib.Path | str,
         output: Sender[Config],
-        event_types: abc.Set[FileWatcher.EventType] = frozenset(FileWatcher.EventType),
+        event_types: abc.Set[EventType] = frozenset(EventType),
         *,
         name: str | None = None,
     ) -> None:
         """Initialize this instance.
 
         Args:
             config_path: The path to the TOML file with the configuration.
@@ -95,29 +95,29 @@
         async for event in self._file_watcher:
             # Since we are watching the whole parent directory, we need to make sure
             # we only react to events related to the configuration file.
             if event.path != self._config_path:
                 continue
 
             match event.type:
-                case FileWatcher.EventType.CREATE:
+                case EventType.CREATE:
                     _logger.info(
                         "%s: The configuration file %s was created, sending new config...",
                         self,
                         self._config_path,
                     )
                     await self.send_config()
-                case FileWatcher.EventType.MODIFY:
+                case EventType.MODIFY:
                     _logger.info(
                         "%s: The configuration file %s was modified, sending update...",
                         self,
                         self._config_path,
                     )
                     await self.send_config()
-                case FileWatcher.EventType.DELETE:
+                case EventType.DELETE:
                     _logger.info(
                         "%s: The configuration file %s was deleted, ignoring...",
                         self,
                         self._config_path,
                     )
                 case _:
                     assert_never(event.type)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/_component_metric_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """The ComponentMetricRequest class."""
 
 from dataclasses import dataclass
 from datetime import datetime
 
-from ...microgrid.component._component import ComponentMetricId
+from frequenz.client.microgrid import ComponentMetricId
 
 
 @dataclass
 class ComponentMetricRequest:
     """A request object to start streaming a metric for a component."""
 
     namespace: str
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/data_sourcing.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_data_sourcing/microgrid_api_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 import asyncio
 import logging
 from collections.abc import Callable
 from typing import Any
 
 from frequenz.channels import Receiver, Sender
-
-from ...microgrid import connection_manager
-from ...microgrid.component import (
+from frequenz.client.microgrid import (
     BatteryData,
     ComponentCategory,
     ComponentMetricId,
     EVChargerData,
     InverterData,
     MeterData,
 )
+
+from ...microgrid import connection_manager
 from ...timeseries import Sample
 from ...timeseries._quantities import Quantity
 from .._channel_registry import ChannelRegistry
 from ._component_metric_request import ComponentMetricRequest
 
 _logger = logging.getLogger(__name__)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_base_classes.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_base_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -227,14 +227,43 @@
         Returns:
             Whether this proposal has a higher priority than the other proposal.
         """
         return (self.priority < other.priority) or (
             self.priority == other.priority and self.source_id < other.source_id
         )
 
+    def __eq__(self, other: object) -> bool:
+        """Check if two proposals are equal.
+
+        Equality is determined by the priority and source ID of the proposals, so
+        two proposals are equal if they have the same priority and source ID, even
+        if they have different power values or creation times.
+
+        This is so that there is only one active proposal for each actor in the bucket,
+        and older proposals are replaced by newer ones.
+
+        Args:
+            other: The other proposal to compare to.
+
+        Returns:
+            Whether the two proposals are equal.
+        """
+        if not isinstance(other, Proposal):
+            return NotImplemented
+
+        return self.priority == other.priority and self.source_id == other.source_id
+
+    def __hash__(self) -> int:
+        """Get the hash of the proposal.
+
+        Returns:
+            The hash of the proposal.
+        """
+        return hash((self.priority, self.source_id))
+
 
 class Algorithm(enum.Enum):
     """The available algorithms for the power manager."""
 
     MATRYOSHKA = "matryoshka"
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_bounds.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_bounds.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_matryoshka.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_matryoshka.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,35 +25,34 @@
 
 from typing_extensions import override
 
 from ... import timeseries
 from ...timeseries import Power
 from . import _bounds
 from ._base_classes import BaseAlgorithm, Proposal, _Report
-from ._sorted_set import SortedSet
 
 if typing.TYPE_CHECKING:
     from ...timeseries._base_types import SystemBounds
     from .. import power_distributing
 
 _logger = logging.getLogger(__name__)
 
 
 class Matryoshka(BaseAlgorithm):
     """The matryoshka algorithm."""
 
     def __init__(self, max_proposal_age: timedelta) -> None:
         """Create a new instance of the matryoshka algorithm."""
         self._max_proposal_age_sec = max_proposal_age.total_seconds()
-        self._component_buckets: dict[frozenset[int], SortedSet[Proposal]] = {}
+        self._component_buckets: dict[frozenset[int], set[Proposal]] = {}
         self._target_power: dict[frozenset[int], Power] = {}
 
     def _calc_target_power(
         self,
-        proposals: SortedSet[Proposal],
+        proposals: set[Proposal],
         system_bounds: SystemBounds,
     ) -> Power:
         """Calculate the target power for the given components.
 
         Args:
             proposals: The proposals for the given components.
             system_bounds: The system bounds for the components in the proposal.
@@ -79,15 +78,15 @@
         if system_bounds.exclusion_bounds is not None and (
             system_bounds.exclusion_bounds.lower != Power.zero()
             or system_bounds.exclusion_bounds.upper != Power.zero()
         ):
             exclusion_bounds = system_bounds.exclusion_bounds
 
         target_power = Power.zero()
-        for next_proposal in reversed(proposals):
+        for next_proposal in sorted(proposals, reverse=True):
             if upper_bound < lower_bound:
                 break
             if next_proposal.preferred_power:
                 match _bounds.clamp_to_bounds(
                     next_proposal.preferred_power,
                     lower_bound,
                     upper_bound,
@@ -179,17 +178,18 @@
             NotImplementedError: When the proposal contains component IDs that are
                 already part of another bucket.
         """
         if not self._validate_component_ids(component_ids, proposal, system_bounds):
             return None
 
         if proposal is not None:
-            self._component_buckets.setdefault(component_ids, SortedSet()).insert(
-                proposal
-            )
+            bucket = self._component_buckets.setdefault(component_ids, set())
+            if proposal in bucket:
+                bucket.remove(proposal)
+            bucket.add(proposal)
 
         # If there has not been any proposal for the given components, don't calculate a
         # target power and just return `None`.
         proposals = self._component_buckets.get(component_ids)
         if proposals is None:
             return None
 
@@ -239,15 +239,17 @@
         exclusion_bounds = None
         if system_bounds.exclusion_bounds is not None and (
             system_bounds.exclusion_bounds.lower != Power.zero()
             or system_bounds.exclusion_bounds.upper != Power.zero()
         ):
             exclusion_bounds = system_bounds.exclusion_bounds
 
-        for next_proposal in reversed(self._component_buckets.get(component_ids, [])):
+        for next_proposal in sorted(
+            self._component_buckets.get(component_ids, []), reverse=True
+        ):
             if next_proposal.priority <= priority:
                 break
             proposal_lower = next_proposal.bounds.lower or lower_bound
             proposal_upper = next_proposal.bounds.upper or upper_bound
             match _bounds.check_exclusion_bounds_overlap(
                 proposal_lower, proposal_upper, exclusion_bounds
             ):
@@ -282,8 +284,8 @@
         """
         for bucket in self._component_buckets.values():
             to_delete = []
             for proposal in bucket:
                 if (loop_time - proposal.creation_time) > self._max_proposal_age_sec:
                     to_delete.append(proposal)
             for proposal in to_delete:
-                bucket.delete(proposal)
+                bucket.remove(proposal)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_power_managing_actor.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import typing
 from datetime import datetime, timedelta, timezone
 
-from frequenz.channels import Receiver, Sender
-from frequenz.channels.util import SkipMissedAndDrift, Timer, select, selected_from
+from frequenz.channels import Receiver, Sender, select, selected_from
+from frequenz.channels.timer import SkipMissedAndDrift, Timer
+from frequenz.client.microgrid import ComponentCategory, ComponentType, InverterType
 from typing_extensions import override
 
-from ...microgrid.component import ComponentCategory
 from ...timeseries._base_types import SystemBounds
 from .._actor import Actor
 from .._channel_registry import ChannelRegistry
 from ._base_classes import Algorithm, BaseAlgorithm, Proposal, ReportRequest, _Report
 from ._matryoshka import Matryoshka
 
 _logger = logging.getLogger(__name__)
@@ -28,47 +28,57 @@
 
 
 class PowerManagingActor(Actor):
     """The power manager."""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        component_category: ComponentCategory,
         proposals_receiver: Receiver[Proposal],
         bounds_subscription_receiver: Receiver[ReportRequest],
         power_distributing_requests_sender: Sender[power_distributing.Request],
         power_distributing_results_receiver: Receiver[power_distributing.Result],
         channel_registry: ChannelRegistry,
+        *,
+        component_category: ComponentCategory,
+        component_type: ComponentType | None = None,
         # arguments to actors need to serializable, so we pass an enum for the algorithm
         # instead of an instance of the algorithm.
         algorithm: Algorithm = Algorithm.MATRYOSHKA,
     ):
         """Create a new instance of the power manager.
 
         Args:
-            component_category: The category of the component this power manager
-                instance is going to support.
             proposals_receiver: The receiver for proposals.
             bounds_subscription_receiver: The receiver for bounds subscriptions.
             power_distributing_requests_sender: The sender for power distribution
                 requests.
             power_distributing_results_receiver: The receiver for power distribution
                 results.
             channel_registry: The channel registry.
+            component_category: The category of the component this power manager
+                instance is going to support.
+            component_type: The type of the component of the given category that this
+                actor is responsible for.  This is used only when the component category
+                is not enough to uniquely identify the component.  For example, when the
+                category is `ComponentCategory.INVERTER`, the type is needed to identify
+                the inverter as a solar inverter or a battery inverter.  This can be
+                `None` when the component category is enough to uniquely identify the
+                component.
             algorithm: The power management algorithm to use.
 
         Raises:
             NotImplementedError: When an unknown algorithm is given.
         """
         if algorithm is not Algorithm.MATRYOSHKA:
             raise NotImplementedError(
                 f"PowerManagingActor: Unknown algorithm: {algorithm}"
             )
 
         self._component_category = component_category
+        self._component_type = component_type
         self._bounds_subscription_receiver = bounds_subscription_receiver
         self._power_distributing_requests_sender = power_distributing_requests_sender
         self._power_distributing_results_receiver = power_distributing_results_receiver
         self._channel_registry = channel_registry
         self._proposals_receiver = proposals_receiver
 
         self._system_bounds: dict[frozenset[int], SystemBounds] = {}
@@ -129,25 +139,36 @@
             NotImplementedError: When the pool type is not supported.
         """
         # Pylint assumes that this import is cyclic, but it's not.
         from ... import (  # pylint: disable=import-outside-toplevel,cyclic-import
             microgrid,
         )
 
-        if self._component_category is not ComponentCategory.BATTERY:
+        bounds_receiver: Receiver[SystemBounds]
+        # pylint: disable=protected-access
+        if self._component_category is ComponentCategory.BATTERY:
+            battery_pool = microgrid.battery_pool(component_ids)
+            bounds_receiver = battery_pool._system_power_bounds.new_receiver()
+        elif self._component_category is ComponentCategory.EV_CHARGER:
+            ev_charger_pool = microgrid.ev_charger_pool(component_ids)
+            bounds_receiver = ev_charger_pool._system_power_bounds.new_receiver()
+        elif (
+            self._component_category is ComponentCategory.INVERTER
+            and self._component_type is InverterType.SOLAR
+        ):
+            pv_pool = microgrid.pv_pool(component_ids)
+            bounds_receiver = pv_pool._system_power_bounds.new_receiver()
+        # pylint: enable=protected-access
+        else:
             err = (
                 "PowerManagingActor: Unsupported component category: "
                 f"{self._component_category}"
             )
             _logger.error(err)
             raise NotImplementedError(err)
-        battery_pool = microgrid.battery_pool(component_ids)
-        # pylint: disable=protected-access
-        bounds_receiver = battery_pool._system_power_bounds.new_receiver()
-        # pylint: enable=protected-access
 
         self._system_bounds[component_ids] = SystemBounds(
             timestamp=datetime.now(tz=timezone.utc),
             inclusion_bounds=None,
             exclusion_bounds=None,
         )
 
@@ -191,15 +212,15 @@
         async for selected in select(
             self._proposals_receiver,
             self._bounds_subscription_receiver,
             self._power_distributing_results_receiver,
             drop_old_proposals_timer,
         ):
             if selected_from(selected, self._proposals_receiver):
-                proposal = selected.value
+                proposal = selected.message
                 if proposal.component_ids not in self._bound_tracker_tasks:
                     self._add_bounds_tracker(proposal.component_ids)
 
                 # TODO: must_send=True forces a new request to # pylint: disable=fixme
                 # be sent to the PowerDistributor, even if there's no change in power.
                 #
                 # This is needed because requests would expire in the microgrid service
@@ -210,15 +231,15 @@
                 # implemented.
                 await self._send_updated_target_power(
                     proposal.component_ids, proposal, must_send=True
                 )
                 await self._send_reports(proposal.component_ids)
 
             elif selected_from(selected, self._bounds_subscription_receiver):
-                sub = selected.value
+                sub = selected.message
                 component_ids = sub.component_ids
                 priority = sub.priority
 
                 if component_ids not in self._subscriptions:
                     self._subscriptions[component_ids] = {
                         priority: self._channel_registry.get_or_create(
                             _Report, sub.get_channel_name()
@@ -235,15 +256,15 @@
                     self._add_bounds_tracker(sub.component_ids)
 
             elif selected_from(selected, self._power_distributing_results_receiver):
                 from .. import (  # pylint: disable=import-outside-toplevel
                     power_distributing,
                 )
 
-                result = selected.value
+                result = selected.message
                 self._distribution_results[frozenset(result.request.component_ids)] = (
                     result
                 )
                 if not isinstance(result, power_distributing.Success):
                     _logger.warning(
                         "PowerManagingActor: PowerDistributing failed: %s", result
                     )
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_power_managing/_sorted_set.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_power_managing/_sorted_set.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_resampling.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_resampling.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/_run_utils.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/_run_utils.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/__init__.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 import logging
 import math
 import typing
 from datetime import timedelta
 
 import grpc
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import BatteryData, ComponentCategory, InverterData
 from typing_extensions import override
 
 from .... import microgrid
 from ...._internal._channels import LatestValueCache
 from ...._internal._math import is_close_to_zero
 from ....microgrid import connection_manager
-from ....microgrid.component import BatteryData, ComponentCategory, InverterData
 from ....timeseries._quantities import Power
 from .._component_pool_status_tracker import ComponentPoolStatusTracker
 from .._component_status import BatteryStatusTracker, ComponentPoolStatus
 from .._distribution_algorithm import (
     AggregatedBatteryData,
     BatteryDistributionAlgorithm,
     DistributionResult,
@@ -123,16 +123,26 @@
 class BatteryManager(ComponentManager):
     """Class to manage the data streams for batteries."""
 
     @override
     def __init__(
         self,
         component_pool_status_sender: Sender[ComponentPoolStatus],
+        results_sender: Sender[Result],
     ):
-        """Initialize the battery data manager."""
+        """Initialize this instance.
+
+        Args:
+            component_pool_status_sender: Channel sender to send the status of the
+                battery pool to.  This status is used by the battery pool metric
+                streams, to dynamically adjust the values based on the health of the
+                individual batteries.
+            results_sender: Channel sender to send the power distribution results to.
+        """
+        self._results_sender = results_sender
         self._batteries = connection_manager.get().component_graph.components(
             component_categories={ComponentCategory.BATTERY}
         )
         self._battery_ids = {battery.component_id for battery in self._batteries}
 
         maps = _get_battery_inverter_mappings(self._battery_ids)
 
@@ -174,31 +184,33 @@
     async def start(self) -> None:
         """Start the battery data manager."""
         await self._create_channels()
 
     @override
     async def stop(self) -> None:
         """Stop the battery data manager."""
+        for bat_cache in self._battery_caches.values():
+            await bat_cache.stop()
+        for inv_cache in self._inverter_caches.values():
+            await inv_cache.stop()
         await self._component_pool_status_tracker.stop()
 
     @override
-    async def distribute_power(self, request: Request) -> Result:
+    async def distribute_power(self, request: Request) -> None:
         """Distribute the requested power to the components.
 
         Args:
             request: Request to get the distribution for.
-
-        Returns:
-            Result of the distribution.
         """
         distribution_result = await self._get_distribution(request)
         if not isinstance(distribution_result, DistributionResult):
-            return distribution_result
-        result = await self._distribute_power(request, distribution_result)
-        return result
+            result = distribution_result
+        else:
+            result = await self._distribute_power(request, distribution_result)
+        await self._results_sender.send(result)
 
     async def _get_distribution(self, request: Request) -> DistributionResult | Result:
         """Get the distribution of the batteries.
 
         Args:
             request: Request to get the distribution for.
 
@@ -656,14 +668,21 @@
                 failed_power += distribution[inverter_id]
                 failed_batteries = failed_batteries.union(battery_ids)
                 _logger.warning(
                     "Battery %s didn't respond in %f sec. Mark it as broken.",
                     battery_ids,
                     request_timeout.total_seconds(),
                 )
+            except Exception:  # pylint: disable=broad-except
+                failed_power += distribution[inverter_id]
+                failed_batteries = failed_batteries.union(battery_ids)
+                _logger.exception(
+                    "Unknown error while setting power to batteries: %s",
+                    battery_ids,
+                )
 
         return failed_power, failed_batteries
 
     async def _cancel_tasks(
         self, tasks: collections.abc.Iterable[asyncio.Task[typing.Any]]
     ) -> None:
         """Cancel given asyncio tasks and wait for them.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,32 +16,34 @@
 class ComponentManager(abc.ABC):
     """Abstract class to manage the data streams for components."""
 
     @abc.abstractmethod
     def __init__(
         self,
         component_pool_status_sender: Sender[ComponentPoolStatus],
+        results_sender: Sender[Result],
     ):
         """Initialize the component data manager.
 
         Args:
             component_pool_status_sender: Channel for sending information about which
                 components are expected to be working.
+            results_sender: Channel for sending the results of power distribution.
         """
 
     @abc.abstractmethod
     def component_ids(self) -> collections.abc.Set[int]:
         """Return the set of component ids."""
 
     @abc.abstractmethod
     async def start(self) -> None:
         """Start the component data manager."""
 
     @abc.abstractmethod
-    async def distribute_power(self, request: Request) -> Result:
+    async def distribute_power(self, request: Request) -> None:
         """Distribute the requested power to the components.
 
         Args:
             request: Request to get the distribution for.
 
         Returns:
             Result of the distribution.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 import asyncio
 import contextlib
 import logging
 from collections import abc
 from datetime import timedelta
 
-from frequenz.channels import Broadcast, Receiver, Sender
-from frequenz.channels.util import Merge
+from frequenz.channels import Broadcast, Merger, Receiver, Sender, merge
 
 from ..._internal._asyncio import cancel_and_await
 from ._component_status import (
     ComponentPoolStatus,
     ComponentStatus,
     ComponentStatusEnum,
     ComponentStatusTracker,
@@ -62,15 +61,15 @@
 
         # At first no component is working, we will get notification when they start
         # working.
         self._current_status = ComponentPoolStatus(working=set(), uncertain=set())
 
         # Channel for sending results of requests to the components.
         self._set_power_result_channel = Broadcast[SetPowerResult](
-            "component_request_status"
+            name="component_request_status"
         )
         self._set_power_result_sender = self._set_power_result_channel.new_sender()
         self._component_status_trackers: list[ComponentStatusTracker] = []
         self._merged_status_receiver = self._make_merged_status_receiver()
 
         self._task = asyncio.create_task(self._run())
 
@@ -84,31 +83,31 @@
     async def stop(self) -> None:
         """Stop the ComponentPoolStatusTracker instance."""
         await cancel_and_await(self._task)
         await self._merged_status_receiver.stop()
 
     def _make_merged_status_receiver(
         self,
-    ) -> Merge[ComponentStatus]:
+    ) -> Merger[ComponentStatus]:
         status_receivers: list[Receiver[ComponentStatus]] = []
 
         for component_id in self._component_ids:
             channel: Broadcast[ComponentStatus] = Broadcast(
-                f"component_{component_id}_status"
+                name=f"component_{component_id}_status"
             )
             tracker = self._component_status_tracker_type(
                 component_id=component_id,
                 max_data_age=self._max_data_age,
                 max_blocking_duration=self._max_blocking_duration,
                 status_sender=channel.new_sender(),
                 set_power_result_receiver=self._set_power_result_channel.new_receiver(),
             )
             self._component_status_trackers.append(tracker)
             status_receivers.append(channel.new_receiver())
-        return Merge(*status_receivers)
+        return merge(*status_receivers)
 
     async def _run(self) -> None:
         """Start tracking component status."""
         async with contextlib.AsyncExitStack() as stack:
             for tracker in self._component_status_trackers:
                 await stack.enter_async_context(tracker)
             while True:
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 # pylint: disable=no-name-in-module
 from frequenz.api.microgrid.battery_pb2 import ComponentState as BatteryComponentState
 from frequenz.api.microgrid.battery_pb2 import RelayState as BatteryRelayState
 from frequenz.api.microgrid.common_pb2 import ErrorLevel
 from frequenz.api.microgrid.inverter_pb2 import ComponentState as InverterComponentState
 
 # pylint: enable=no-name-in-module
-from frequenz.channels import Receiver, Sender
-from frequenz.channels.util import Timer, select, selected_from
-from typing_extensions import override
-
-from ....microgrid import connection_manager
-from ....microgrid.component import (
+from frequenz.channels import Receiver, Sender, select, selected_from
+from frequenz.channels.timer import SkipMissedAndDrift, Timer
+from frequenz.client.microgrid import (
     BatteryData,
     ComponentCategory,
     ComponentData,
     InverterData,
 )
+from typing_extensions import override
+
+from ....microgrid import connection_manager
 from ..._background_service import BackgroundService
 from ._blocking_status import BlockingStatus
 from ._component_status import (
     ComponentStatus,
     ComponentStatusEnum,
     ComponentStatusTracker,
     SetPowerResult,
@@ -143,19 +143,19 @@
         if inverter_id is None:
             raise RuntimeError(
                 f"Can't find inverter adjacent to battery: {component_id}"
             )
 
         self._battery: _ComponentStreamStatus = _ComponentStreamStatus(
             component_id,
-            data_recv_timer=Timer.timeout(max_data_age),
+            data_recv_timer=Timer(max_data_age, SkipMissedAndDrift()),
         )
         self._inverter: _ComponentStreamStatus = _ComponentStreamStatus(
             inverter_id,
-            data_recv_timer=Timer.timeout(max_data_age),
+            data_recv_timer=Timer(max_data_age, SkipMissedAndDrift()),
         )
 
         # Select needs receivers that can be get in async way only.
 
     @override
     def start(self) -> None:
         """Start the BatteryStatusTracker instance."""
@@ -273,21 +273,21 @@
                     inverter_timer,
                     inverter,
                     set_power_result,
                 ):
                     new_status = None
 
                     if selected_from(selected, battery):
-                        self._handle_status_battery(selected.value)
+                        self._handle_status_battery(selected.message)
 
                     elif selected_from(selected, inverter):
-                        self._handle_status_inverter(selected.value)
+                        self._handle_status_inverter(selected.message)
 
                     elif selected_from(selected, set_power_result):
-                        self._handle_status_set_power_result(selected.value)
+                        self._handle_status_set_power_result(selected.message)
 
                     elif selected_from(selected, battery_timer):
                         if (
                             datetime.now(tz=timezone.utc)
                             - self._battery.last_msg_timestamp
                         ) < self._max_data_age:
                             # This means that we have received data from the battery
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 """Power distribution algorithm to distribute power between batteries."""
 
 import logging
 import math
 from dataclasses import dataclass
 from typing import NamedTuple, Sequence
 
+from frequenz.client.microgrid import BatteryData, InverterData
+
 from ...._internal._math import is_close_to_zero
-from ....microgrid.component import BatteryData, InverterData
 from ..result import PowerBounds
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass()
 class AggregatedBatteryData:
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/power_distributing.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/power_distributing.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,17 +11,23 @@
 Purpose of this actor is to keep SoC level of each component at the equal level.
 """
 
 
 import asyncio
 
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import ComponentCategory, ComponentType, InverterType
 
 from ...actor._actor import Actor
-from ._component_managers import BatteryManager, ComponentManager
+from ._component_managers import (
+    BatteryManager,
+    ComponentManager,
+    EVChargerManager,
+    PVManager,
+)
 from ._component_status import ComponentPoolStatus
 from .request import Request
 from .result import Result
 
 
 class PowerDistributingActor(Actor):
     # pylint: disable=too-many-instance-attributes
@@ -50,39 +56,72 @@
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         requests_receiver: Receiver[Request],
         results_sender: Sender[Result],
         component_pool_status_sender: Sender[ComponentPoolStatus],
-        wait_for_data_sec: float = 2,
+        wait_for_data_sec: float,
         *,
+        component_category: ComponentCategory,
+        component_type: ComponentType | None = None,
         name: str | None = None,
     ) -> None:
         """Create class instance.
 
         Args:
             requests_receiver: Receiver for receiving power requests from the power
                 manager.
             results_sender: Sender for sending results to the power manager.
             component_pool_status_sender: Channel for sending information about which
                 components are expected to be working.
             wait_for_data_sec: How long actor should wait before processing first
                 request. It is a time needed to collect first components data.
+            component_category: The category of the components that this actor is
+                responsible for.
+            component_type: The type of the component of the given category that this
+                actor is responsible for.  This is used only when the component category
+                is not enough to uniquely identify the component.  For example, when the
+                category is `ComponentCategory.INVERTER`, the type is needed to identify
+                the inverter as a solar inverter or a battery inverter.  This can be
+                `None` when the component category is enough to uniquely identify the
+                component.
             name: The name of the actor. If `None`, `str(id(self))` will be used. This
                 is used mostly for debugging purposes.
+
+        Raises:
+            ValueError: If the given component category is not supported.
         """
         super().__init__(name=name)
+        self._component_category = component_category
+        self._component_type = component_type
         self._requests_receiver = requests_receiver
         self._result_sender = results_sender
         self._wait_for_data_sec = wait_for_data_sec
 
-        self._component_manager: ComponentManager = BatteryManager(
-            component_pool_status_sender
-        )
+        self._component_manager: ComponentManager
+        if component_category == ComponentCategory.BATTERY:
+            self._component_manager = BatteryManager(
+                component_pool_status_sender, results_sender
+            )
+        elif component_category == ComponentCategory.EV_CHARGER:
+            self._component_manager = EVChargerManager(
+                component_pool_status_sender, results_sender
+            )
+        elif (
+            component_category == ComponentCategory.INVERTER
+            and component_type == InverterType.SOLAR
+        ):
+            self._component_manager = PVManager(
+                component_pool_status_sender, results_sender
+            )
+        else:
+            raise ValueError(
+                f"PowerDistributor doesn't support controlling: {component_category}"
+            )
 
     async def _run(self) -> None:  # pylint: disable=too-many-locals
         """Run actor main function.
 
         It waits for new requests in task_queue and process it, and send
         `set_power` request with distributed power.
         The output of the `set_power` method is processed.
@@ -91,16 +130,15 @@
         """
         await self._component_manager.start()
 
         # Wait few seconds to get data from the channels created above.
         await asyncio.sleep(self._wait_for_data_sec)
 
         async for request in self._requests_receiver:
-            result = await self._component_manager.distribute_power(request)
-            await self._result_sender.send(result)
+            await self._component_manager.distribute_power(request)
 
     async def stop(self, msg: str | None = None) -> None:
         """Stop this actor.
 
         Args:
             msg: The message to be passed to the tasks being cancelled.
         """
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/request.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/request.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/actor/power_distributing/result.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/actor/power_distributing/result.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/config/_config.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/config/_config.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/__init__.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -70,24 +70,39 @@
 {{glossary("load")}} the microgrid is built to support.  The power drawn by the consumer
 is available through [`consumer_power`][frequenz.sdk.timeseries.consumer.Consumer.power]
 
 In locations without a consumer, this method streams zero values.
 
 ## Producers: PV Arrays, CHP
 
-The total {{glossary("pv", "PV")}} power production in a microgrid can be streamed
-through [`pv_power`][frequenz.sdk.timeseries.logical_meter.LogicalMeter.pv_power] , and
-similarly the total CHP production in a site can be streamed through
-[`chp_power`][frequenz.sdk.timeseries.logical_meter.LogicalMeter.chp_power].  And total
-producer power is available through
-[`producer_power`][frequenz.sdk.timeseries.producer.Producer.power].
+The total CHP production in a site can be streamed through
+[`chp_power`][frequenz.sdk.timeseries.logical_meter.LogicalMeter.chp_power].  PV Power
+is available through the PV pool described below.  And total producer power is available
+through [`microgrid.producer().power`][frequenz.sdk.timeseries.producer.Producer.power].
 
 As is the case with the other methods, if PV Arrays or CHPs are not available in a
 microgrid, the corresponding methods stream zero values.
 
+## PV Arrays
+
+The total PV power production is available through
+[`pv_pool`][frequenz.sdk.microgrid.pv_pool]'s
+[`power`][frequenz.sdk.timeseries.pv_pool.PVPool.power].  The PV pool by default uses
+all PV inverters available at a location, but PV pool instances can be created for
+subsets of PV inverters if necessary, by specifying the inverter ids.
+
+The `pv_pool` also provides available power bounds through the
+[`power_status`][frequenz.sdk.timeseries.pv_pool.PVPool.power_status] method.
+
+The `pv_pool` also provides a control method
+[`propose_power`][frequenz.sdk.timeseries.pv_pool.PVPool.propose_power], which accepts
+values in the {{glossary("psc", "Passive Sign Convention")}} and supports only
+production.
+
+
 ## Batteries
 
 The total Battery power is available through
 [`battery_pool`][frequenz.sdk.microgrid.battery_pool]'s
 [`power`][frequenz.sdk.timeseries.battery_pool.BatteryPool.power].  The battery pool by
 default uses all batteries available at a location, but battery pool instances can be
 created for subsets of batteries if necessary, by specifying the battery ids.
@@ -109,32 +124,36 @@
 ## EV Chargers
 
 The [`ev_charger_pool`][frequenz.sdk.microgrid.ev_charger_pool] offers a
 [`power`][frequenz.sdk.timeseries.ev_charger_pool.EVChargerPool.power] method that
 streams the total power measured for all the {{glossary("ev-charger", "EV Chargers")}}
 at a site.
 
-It also offers a
-[`component_data`][frequenz.sdk.timeseries.ev_charger_pool.EVChargerPool.component_data]
-method for fetching the status of individual EV Chargers, including state changes like
-when an EV is connected or disconnected, and a
-[`set_bounds`][frequenz.sdk.timeseries.ev_charger_pool.EVChargerPool.set_bounds] method
-to limit the charge power of individual EV Chargers.
+The `ev_charger_pool` also provides available power bounds through the
+[`power_status`][frequenz.sdk.timeseries.ev_charger_pool.EVChargerPool.power_status]
+method.
+
+
+The `ev_charger_pool` also provides a control method
+[`propose_power`][frequenz.sdk.timeseries.ev_charger_pool.EVChargerPool.propose_power],
+which accepts values in the {{glossary("psc", "Passive Sign Convention")}} and supports
+only charging.
 """  # noqa: D205, D400
 
 from ..actor import ResamplerConfig
-from . import _data_pipeline, client, component, connection_manager, metadata
+from . import _data_pipeline, connection_manager
 from ._data_pipeline import (
     battery_pool,
     consumer,
     ev_charger_pool,
     frequency,
     grid,
     logical_meter,
     producer,
+    pv_pool,
     voltage,
 )
 
 
 async def initialize(host: str, port: int, resampler_config: ResamplerConfig) -> None:
     """Initialize the microgrid connection manager and the data pipeline.
 
@@ -145,19 +164,17 @@
     """
     await connection_manager.initialize(host, port)
     await _data_pipeline.initialize(resampler_config)
 
 
 __all__ = [
     "initialize",
-    "client",
-    "component",
     "consumer",
     "battery_pool",
     "ev_charger_pool",
     "grid",
     "frequency",
     "logical_meter",
-    "metadata",
     "producer",
+    "pv_pool",
     "voltage",
 ]
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/_power_wrapper.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/_power_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import typing
 
 from frequenz.channels import Broadcast
 
 # pylint seems to think this is a cyclic import, but it is not.
 #
 # pylint: disable=cyclic-import
-from .component import ComponentCategory
+from frequenz.client.microgrid import ComponentCategory, ComponentType
 
 # A number of imports had to be done inside functions where they are used, to break
 # import cycles.
 #
 # pylint: disable=import-outside-toplevel
 if typing.TYPE_CHECKING:
     from ..actor import ChannelRegistry, _power_managing
@@ -26,70 +26,92 @@
         PowerDistributingActor,
         Request,
         Result,
     )
 
 _logger = logging.getLogger(__name__)
 
+_POWER_DISTRIBUTING_ACTOR_WAIT_FOR_DATA_SEC = 2.0
+
 
 class PowerWrapper:
     """Wrapper around the power managing and power distributing actors."""
 
-    def __init__(self, channel_registry: ChannelRegistry):
+    def __init__(
+        self,
+        channel_registry: ChannelRegistry,
+        *,
+        component_category: ComponentCategory,
+        component_type: ComponentType | None = None,
+    ):
         """Initialize the power control.
 
         Args:
             channel_registry: A channel registry for use in the actors.
+            component_category: The category of the components that actors started by
+                this instance of the PowerWrapper will be responsible for.
+            component_type: The type of the component of the given category that this
+                actor is responsible for.  This is used only when the component category
+                is not enough to uniquely identify the component.  For example, when the
+                category is `ComponentCategory.INVERTER`, the type is needed to identify
+                the inverter as a solar inverter or a battery inverter.  This can be
+                `None` when the component category is enough to uniquely identify the
+                component.
         """
+        self._component_category = component_category
+        self._component_type = component_type
         self._channel_registry = channel_registry
 
         self.status_channel: Broadcast[ComponentPoolStatus] = Broadcast(
-            "Component Status Channel", resend_latest=True
+            name="Component Status Channel", resend_latest=True
         )
         self._power_distribution_requests_channel: Broadcast[Request] = Broadcast(
-            "Power Distributing Actor, Requests Broadcast Channel"
+            name="Power Distributing Actor, Requests Broadcast Channel"
         )
         self._power_distribution_results_channel: Broadcast[Result] = Broadcast(
-            "Power Distributing Actor, Results Broadcast Channel"
+            name="Power Distributing Actor, Results Broadcast Channel"
         )
 
         self.proposal_channel: Broadcast[_power_managing.Proposal] = Broadcast(
-            "Power Managing Actor, Requests Broadcast Channel"
+            name="Power Managing Actor, Requests Broadcast Channel"
         )
         self.bounds_subscription_channel: Broadcast[_power_managing.ReportRequest] = (
-            Broadcast("Power Managing Actor, Bounds Subscription Channel")
+            Broadcast(name="Power Managing Actor, Bounds Subscription Channel")
         )
 
         self._power_distributing_actor: PowerDistributingActor | None = None
         self._power_managing_actor: _power_managing.PowerManagingActor | None = None
+        self._pd_wait_for_data_sec: float = _POWER_DISTRIBUTING_ACTOR_WAIT_FOR_DATA_SEC
 
     def _start_power_managing_actor(self) -> None:
         """Start the power managing actor if it is not already running."""
         if self._power_managing_actor:
             return
 
         from .. import microgrid
 
         component_graph = microgrid.connection_manager.get().component_graph
         # Currently the power managing actor only supports batteries.  The below
         # constraint needs to be relaxed if the actor is extended to support other
         # components.
         if not component_graph.components(
-            component_categories={ComponentCategory.BATTERY}
+            component_categories={self._component_category}
         ):
             _logger.warning(
-                "No batteries found in the component graph. "
-                "The power managing actor will not be started."
+                "No %s found in the component graph. "
+                "The power managing actor will not be started.",
+                self._component_category,
             )
             return
 
         from ..actor._power_managing._power_managing_actor import PowerManagingActor
 
         self._power_managing_actor = PowerManagingActor(
-            component_category=ComponentCategory.BATTERY,
+            component_category=self._component_category,
+            component_type=self._component_type,
             proposals_receiver=self.proposal_channel.new_receiver(),
             bounds_subscription_receiver=(
                 self.bounds_subscription_channel.new_receiver()
             ),
             power_distributing_requests_sender=(
                 self._power_distribution_requests_channel.new_sender()
             ),
@@ -105,31 +127,35 @@
         if self._power_distributing_actor:
             return
 
         from .. import microgrid
 
         component_graph = microgrid.connection_manager.get().component_graph
         if not component_graph.components(
-            component_categories={ComponentCategory.BATTERY}
+            component_categories={self._component_category}
         ):
             _logger.warning(
-                "No batteries found in the component graph. "
-                "The power distributing actor will not be started."
+                "No %s found in the component graph. "
+                "The power distributing actor will not be started.",
+                self._component_category,
             )
             return
 
         from ..actor.power_distributing import PowerDistributingActor
 
         # The PowerDistributingActor is started with only a single default user channel.
         # Until the PowerManager is implemented, support for multiple use-case actors
         # will not be available in the high level interface.
         self._power_distributing_actor = PowerDistributingActor(
+            component_category=self._component_category,
+            component_type=self._component_type,
             requests_receiver=self._power_distribution_requests_channel.new_receiver(),
             results_sender=self._power_distribution_results_channel.new_sender(),
             component_pool_status_sender=self.status_channel.new_sender(),
+            wait_for_data_sec=self._pd_wait_for_data_sec,
         )
         self._power_distributing_actor.start()
 
     @property
     def started(self) -> bool:
         """Return True if power managing and power distributing actors are started."""
         return (
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component/_component.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_consumer_power_formula.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,249 +1,187 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
-"""Defines the components that can be used in a microgrid."""
-from __future__ import annotations
+"""Formula generator from component graph for Consumer Power."""
 
-from dataclasses import dataclass
-from enum import Enum
-from typing import TYPE_CHECKING
+import logging
 
-import frequenz.api.common.components_pb2 as components_pb
-import frequenz.api.microgrid.grid_pb2 as grid_pb
-import frequenz.api.microgrid.inverter_pb2 as inverter_pb
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
 
-if TYPE_CHECKING:
-    # Break circular import
-    from ...timeseries import Fuse
+from ....microgrid import connection_manager
+from ..._quantities import Power
+from .._formula_engine import FormulaEngine
+from .._resampled_formula_builder import ResampledFormulaBuilder
+from ._formula_generator import (
+    NON_EXISTING_COMPONENT_ID,
+    ComponentNotFound,
+    FormulaGenerator,
+)
 
+_logger = logging.getLogger(__name__)
 
-class ComponentType(Enum):
-    """A base class from which individual component types are derived."""
 
+class ConsumerPowerFormula(FormulaGenerator[Power]):
+    """Formula generator from component graph for calculating the Consumer Power.
 
-# pylint: disable=no-member
-
-
-class InverterType(ComponentType):
-    """Enum representing inverter types."""
-
-    NONE = inverter_pb.Type.TYPE_UNSPECIFIED
-    """Unspecified inverter type."""
-
-    BATTERY = inverter_pb.Type.TYPE_BATTERY
-    """Battery inverter."""
-
-    SOLAR = inverter_pb.Type.TYPE_SOLAR
-    """Solar inverter."""
-
-    HYBRID = inverter_pb.Type.TYPE_HYBRID
-    """Hybrid inverter."""
-
-
-def _component_type_from_protobuf(
-    component_category: components_pb.ComponentCategory.ValueType,
-    component_metadata: inverter_pb.Metadata,
-) -> ComponentType | None:
-    """Convert a protobuf InverterType message to Component enum.
-
-    For internal-only use by the `microgrid` package.
-
-    Args:
-        component_category: category the type belongs to.
-        component_metadata: protobuf metadata to fetch type from.
-
-    Returns:
-        Enum value corresponding to the protobuf message.
+    The consumer power is calculated by summing up the power of all components that
+    are not part of a battery, CHP, PV or EV charger chain.
     """
-    # ComponentType values in the protobuf definition are not unique across categories
-    # as of v0.11.0, so we need to check the component category first, before doing any
-    # component type checks.
-    if (
-        component_category
-        == components_pb.ComponentCategory.COMPONENT_CATEGORY_INVERTER
-    ):
-        # mypy 1.4.1 crashes at this line, maybe it doesn't like the name of the "type"
-        # attribute in this context.  Hence the "# type: ignore".
-        if not any(
-            t.value == component_metadata.type for t in InverterType  # type: ignore
-        ):
-            return None
-
-        return InverterType(component_metadata.type)
-
-    return None
-
-
-class ComponentCategory(Enum):
-    """Possible types of microgrid component."""
-
-    NONE = components_pb.ComponentCategory.COMPONENT_CATEGORY_UNSPECIFIED
-    """Unspecified component category."""
-
-    GRID = components_pb.ComponentCategory.COMPONENT_CATEGORY_GRID
-    """Grid component."""
-
-    METER = components_pb.ComponentCategory.COMPONENT_CATEGORY_METER
-    """Meter component."""
-
-    INVERTER = components_pb.ComponentCategory.COMPONENT_CATEGORY_INVERTER
-    """Inverter component."""
-
-    BATTERY = components_pb.ComponentCategory.COMPONENT_CATEGORY_BATTERY
-    """Battery component."""
-
-    EV_CHARGER = components_pb.ComponentCategory.COMPONENT_CATEGORY_EV_CHARGER
-    """EV charger component."""
-
-    CHP = components_pb.ComponentCategory.COMPONENT_CATEGORY_CHP
-    """CHP component."""
-
-
-def _component_category_from_protobuf(
-    component_category: components_pb.ComponentCategory.ValueType,
-) -> ComponentCategory:
-    """Convert a protobuf ComponentCategory message to ComponentCategory enum.
 
-    For internal-only use by the `microgrid` package.
+    def generate(self) -> FormulaEngine[Power]:
+        """Generate formula for calculating consumer power from the component graph.
 
-    Args:
-        component_category: protobuf enum to convert
-
-    Returns:
-        Enum value corresponding to the protobuf message.
-
-    Raises:
-        ValueError: if `component_category` is a sensor (this is not considered
-            a valid component category as it does not form part of the
-            microgrid itself)
-    """
-    if component_category == components_pb.ComponentCategory.COMPONENT_CATEGORY_SENSOR:
-        raise ValueError("Cannot create a component from a sensor!")
-
-    if not any(t.value == component_category for t in ComponentCategory):
-        return ComponentCategory.NONE
-
-    return ComponentCategory(component_category)
-
-
-@dataclass(frozen=True)
-class ComponentMetadata:
-    """Base class for component metadata classes."""
-
-    fuse: Fuse | None = None
-    """The fuse at the grid connection point."""
-
-
-@dataclass(frozen=True)
-class GridMetadata(ComponentMetadata):
-    """Metadata for a grid connection point."""
-
-
-def _component_metadata_from_protobuf(
-    component_category: components_pb.ComponentCategory.ValueType,
-    component_metadata: grid_pb.Metadata,
-) -> GridMetadata | None:
-    from ...timeseries import Current, Fuse  # pylint: disable=import-outside-toplevel
-
-    if component_category == components_pb.ComponentCategory.COMPONENT_CATEGORY_GRID:
-        max_current = Current.from_amperes(component_metadata.rated_fuse_current)
-        fuse = Fuse(max_current)
-        return GridMetadata(fuse)
-
-    return None
-
-
-@dataclass(frozen=True)
-class Component:
-    """Metadata for a single microgrid component."""
-
-    component_id: int
-    """The ID of this component."""
-
-    category: ComponentCategory
-    """The category of this component."""
+        Returns:
+            A formula engine that will calculate the consumer power.
 
-    type: ComponentType | None = None
-    """The type of this component."""
+        Raises:
+            ComponentNotFound: If the component graph does not contain a consumer power
+                component.
+            RuntimeError: If the grid component has a single successor that is not a
+                meter.
+        """
+        builder = self._get_builder(
+            "consumer-power", ComponentMetricId.ACTIVE_POWER, Power.from_watts
+        )
+
+        grid_successors = self._get_grid_component_successors()
+
+        if not grid_successors:
+            raise ComponentNotFound("No components found in the component graph.")
+
+        component_graph = connection_manager.get().component_graph
+        if all(
+            successor.category == ComponentCategory.METER
+            and not component_graph.is_battery_chain(successor)
+            and not component_graph.is_chp_chain(successor)
+            and not component_graph.is_pv_chain(successor)
+            and not component_graph.is_ev_charger_chain(successor)
+            for successor in grid_successors
+        ):
+            return self._gen_with_grid_meter(builder, grid_successors)
 
-    metadata: ComponentMetadata | None = None
-    """The metadata of this component."""
+        return self._gen_without_grid_meter(builder, self._get_grid_component())
 
-    def is_valid(self) -> bool:
-        """Check if this instance contains valid data.
+    def _gen_with_grid_meter(
+        self,
+        builder: ResampledFormulaBuilder[Power],
+        grid_meters: set[Component],
+    ) -> FormulaEngine[Power]:
+        """Generate formula for calculating consumer power with grid meter.
+
+        Args:
+            builder: The formula engine builder.
+            grid_meters: The grid meter component.
 
         Returns:
-            `True` if `id > 0` and `type` is a valid `ComponentCategory`, or if `id
-                == 0` and `type` is `GRID`, `False` otherwise
+            A formula engine that will calculate the consumer power.
         """
-        return (
-            self.component_id > 0 and any(t == self.category for t in ComponentCategory)
-        ) or (self.component_id == 0 and self.category == ComponentCategory.GRID)
+        assert grid_meters
+        component_graph = connection_manager.get().component_graph
 
-    def __hash__(self) -> int:
-        """Compute a hash of this instance, obtained by hashing the `component_id` field.
+        def non_consumer_component(component: Component) -> bool:
+            """
+            Check if a component is not a consumer component.
+
+            Args:
+                component: The component to check.
+
+            Returns:
+                True if the component is not a consumer component, False otherwise.
+            """
+            # If the component graph supports additional types of grid successors in the
+            # future, additional checks need to be added here.
+            return (
+                component_graph.is_battery_chain(component)
+                or component_graph.is_chp_chain(component)
+                or component_graph.is_pv_chain(component)
+                or component_graph.is_ev_charger_chain(component)
+            )
+
+        # join all non consumer components reachable from the different grid meters
+        non_consumer_components: set[Component] = set()
+        for grid_meter in grid_meters:
+            non_consumer_components = non_consumer_components.union(
+                component_graph.dfs(grid_meter, set(), non_consumer_component)
+            )
+
+        # push all grid meters
+        for idx, grid_meter in enumerate(grid_meters):
+            if idx > 0:
+                builder.push_oper("+")
+            builder.push_component_metric(
+                grid_meter.component_id, nones_are_zeros=False
+            )
+
+        # push all non consumer components and subtract them from the grid meters
+        for component in non_consumer_components:
+            builder.push_oper("-")
+            builder.push_component_metric(
+                component.component_id,
+                nones_are_zeros=component.category != ComponentCategory.METER,
+            )
+
+        return builder.build()
+
+    def _gen_without_grid_meter(
+        self,
+        builder: ResampledFormulaBuilder[Power],
+        grid: Component,
+    ) -> FormulaEngine[Power]:
+        """Generate formula for calculating consumer power without a grid meter.
+
+        Args:
+            builder: The formula engine builder.
+            grid: The grid component.
 
         Returns:
-            Hash of this instance.
+            A formula engine that will calculate the consumer power.
         """
-        return hash(self.component_id)
-
-
-class ComponentMetricId(Enum):
-    """An enum representing the various metrics available in the microgrid."""
-
-    ACTIVE_POWER = "active_power"
-    """Active power."""
 
-    ACTIVE_POWER_PHASE_1 = "active_power_phase_1"
-    """Active power in phase 1."""
-    ACTIVE_POWER_PHASE_2 = "active_power_phase_2"
-    """Active power in phase 2."""
-    ACTIVE_POWER_PHASE_3 = "active_power_phase_3"
-    """Active power in phase 3."""
-
-    CURRENT_PHASE_1 = "current_phase_1"
-    """Current in phase 1."""
-    CURRENT_PHASE_2 = "current_phase_2"
-    """Current in phase 2."""
-    CURRENT_PHASE_3 = "current_phase_3"
-    """Current in phase 3."""
-
-    VOLTAGE_PHASE_1 = "voltage_phase_1"
-    """Voltage in phase 1."""
-    VOLTAGE_PHASE_2 = "voltage_phase_2"
-    """Voltage in phase 2."""
-    VOLTAGE_PHASE_3 = "voltage_phase_3"
-    """Voltage in phase 3."""
-
-    FREQUENCY = "frequency"
-
-    SOC = "soc"
-    """State of charge."""
-    SOC_LOWER_BOUND = "soc_lower_bound"
-    """Lower bound of state of charge."""
-    SOC_UPPER_BOUND = "soc_upper_bound"
-    """Upper bound of state of charge."""
-    CAPACITY = "capacity"
-    """Capacity."""
-
-    POWER_INCLUSION_LOWER_BOUND = "power_inclusion_lower_bound"
-    """Power inclusion lower bound."""
-    POWER_EXCLUSION_LOWER_BOUND = "power_exclusion_lower_bound"
-    """Power exclusion lower bound."""
-    POWER_EXCLUSION_UPPER_BOUND = "power_exclusion_upper_bound"
-    """Power exclusion upper bound."""
-    POWER_INCLUSION_UPPER_BOUND = "power_inclusion_upper_bound"
-    """Power inclusion upper bound."""
-
-    ACTIVE_POWER_INCLUSION_LOWER_BOUND = "active_power_inclusion_lower_bound"
-    """Active power inclusion lower bound."""
-    ACTIVE_POWER_EXCLUSION_LOWER_BOUND = "active_power_exclusion_lower_bound"
-    """Active power exclusion lower bound."""
-    ACTIVE_POWER_EXCLUSION_UPPER_BOUND = "active_power_exclusion_upper_bound"
-    """Active power exclusion upper bound."""
-    ACTIVE_POWER_INCLUSION_UPPER_BOUND = "active_power_inclusion_upper_bound"
-    """Active power inclusion upper bound."""
+        def consumer_component(component: Component) -> bool:
+            """
+            Check if a component is a consumer component.
+
+            Args:
+                component: The component to check.
+
+            Returns:
+                True if the component is a consumer component, False otherwise.
+            """
+            # If the component graph supports additional types of grid successors in the
+            # future, additional checks need to be added here.
+            return (
+                component.category
+                in {ComponentCategory.METER, ComponentCategory.INVERTER}
+                and not component_graph.is_battery_chain(component)
+                and not component_graph.is_chp_chain(component)
+                and not component_graph.is_pv_chain(component)
+                and not component_graph.is_ev_charger_chain(component)
+            )
+
+        component_graph = connection_manager.get().component_graph
+        consumer_components = component_graph.dfs(grid, set(), consumer_component)
+
+        if not consumer_components:
+            _logger.warning(
+                "Unable to find any consumers in the component graph. "
+                "Subscribing to the resampling actor with a non-existing "
+                "component id, so that `0` values are sent from the formula."
+            )
+            # If there are no consumer components, we have to send 0 values at the same
+            # frequency as the other streams.  So we subscribe with a non-existing
+            # component id, just to get a `None` message at the resampling interval.
+            builder.push_component_metric(
+                NON_EXISTING_COMPONENT_ID, nones_are_zeros=True
+            )
+            return builder.build()
+
+        for idx, component in enumerate(consumer_components):
+            if idx > 0:
+                builder.push_oper("+")
+
+            builder.push_component_metric(
+                component.component_id,
+                nones_are_zeros=component.category != ComponentCategory.METER,
+            )
 
-    TEMPERATURE = "temperature"
-    """Temperature."""
+        return builder.build()
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/component_graph.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/component_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,23 +18,28 @@
 
 It deliberately does not include all pieces of hardware placed in the microgrid,
 instead limiting itself to just those that are needed to monitor and control the
 flow of power.
 """
 
 import asyncio
+import dataclasses
 import logging
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterable
 from dataclasses import asdict
 
 import networkx as nx
-
-from .client import Connection, MicrogridApiClient
-from .component import Component, ComponentCategory, InverterType
+from frequenz.client.microgrid import (
+    ApiClient,
+    Component,
+    ComponentCategory,
+    Connection,
+    InverterType,
+)
 
 _logger = logging.getLogger(__name__)
 
 # pylint: disable=too-many-lines
 
 
 class InvalidGraphError(Exception):
@@ -505,15 +510,15 @@
         if not all(connection.is_valid() for connection in connections):
             raise InvalidGraphError(f"Invalid connections in input: {connections}")
 
         new_graph = nx.DiGraph()
         for component in components:
             new_graph.add_node(component.component_id, **asdict(component))
 
-        new_graph.add_edges_from(connections)
+        new_graph.add_edges_from(dataclasses.astuple(c) for c in connections)
 
         # check if we can construct a valid ComponentGraph
         # from the new NetworkX graph data
         _provisional = _MicrogridComponentGraph()
         _provisional._graph = new_graph  # pylint: disable=protected-access
         if correct_errors is not None:
             try:
@@ -532,15 +537,15 @@
 
         old_graph = self._graph
         self._graph = new_graph
         old_graph.clear()  # just in case any references remain, but should not
 
     async def refresh_from_api(
         self,
-        api: MicrogridApiClient,
+        api: ApiClient,
         correct_errors: Callable[["_MicrogridComponentGraph"], None] | None = None,
     ) -> None:
         """Refresh the contents of a component graph from the remote API.
 
         Args:
             api: API client from which to fetch graph data
             correct_errors: callback that, if set, will be invoked if the
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/microgrid/connection_manager.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/microgrid/connection_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 component graph.
 """
 
 import logging
 from abc import ABC, abstractmethod
 
 import grpc.aio as grpcaio
+from frequenz.client.microgrid import ApiClient, Location, Metadata
 
-from .client import MicrogridApiClient
-from .client._client import MicrogridGrpcClient
 from .component_graph import ComponentGraph, _MicrogridComponentGraph
-from .metadata import Location, Metadata
 
 # Not public default host and port
 _DEFAULT_MICROGRID_HOST = "[::1]"
 _DEFAULT_MICROGRID_PORT = 443
 
 _logger = logging.getLogger(__name__)
 
@@ -55,16 +53,16 @@
         Returns:
             port
         """
         return self._port
 
     @property
     @abstractmethod
-    def api_client(self) -> MicrogridApiClient:
-        """Get MicrogridApiClient.
+    def api_client(self) -> ApiClient:
+        """Get ApiClient.
 
         Returns:
             api client
         """
 
     @property
     @abstractmethod
@@ -113,25 +111,25 @@
         Args:
             host: host. Defaults to _DEFAULT_MICROGRID_HOST.
             port: port. Defaults to _DEFAULT_MICROGRID_PORT.
         """
         super().__init__(host, port)
         target = f"{host}:{port}"
         grpc_channel = grpcaio.insecure_channel(target)
-        self._api = MicrogridGrpcClient(grpc_channel, target)
+        self._api = ApiClient(grpc_channel, target)
         # To create graph from the api we need await.
         # So create empty graph here, and update it in `run` method.
         self._graph = _MicrogridComponentGraph()
 
         self._metadata: Metadata
         """The metadata of the microgrid."""
 
     @property
-    def api_client(self) -> MicrogridApiClient:
-        """Get MicrogridApiClient.
+    def api_client(self) -> ApiClient:
+        """Get ApiClient.
 
         Returns:
             api client
         """
         return self._api
 
     @property
@@ -168,15 +166,15 @@
             host: new host
             port: new port
         """
         await super()._update_api(host, port)  # pylint: disable=protected-access
 
         target = f"{host}:{port}"
         grpc_channel = grpcaio.insecure_channel(target)
-        self._api = MicrogridGrpcClient(grpc_channel, target)
+        self._api = ApiClient(grpc_channel, target)
         self._metadata = await self._api.metadata()
         await self._graph.refresh_from_api(self._api)
 
     async def _initialize(self) -> None:
         self._metadata = await self._api.metadata()
         await self._graph.refresh_from_api(self._api)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/__init__.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_base_types.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_base_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_grid_frequency.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_grid_frequency.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING
 
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
 
 from ..actor import ChannelRegistry
 from ..microgrid import connection_manager
-from ..microgrid.component import Component, ComponentCategory, ComponentMetricId
 from ..timeseries._base_types import Sample
 from ..timeseries._quantities import Frequency, Quantity
 
 if TYPE_CHECKING:
     # Imported here to avoid a circular import.
     from ..actor import ComponentMetricRequest
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_moving_window.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_moving_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
         async def send_mock_data(sender: Sender[Sample]) -> None:
             while True:
                 await sender.send(Sample(datetime.now(tz=timezone.utc), 10.0))
                 await asyncio.sleep(1.0)
 
         async def run() -> None:
-            resampled_data_channel = Broadcast[Sample]("sample-data")
+            resampled_data_channel = Broadcast[Sample](name="sample-data")
             resampled_data_receiver = resampled_data_channel.new_receiver()
             resampled_data_sender = resampled_data_channel.new_sender()
 
             send_task = asyncio.create_task(send_mock_data(resampled_data_sender))
 
             async with MovingWindow(
                 size=timedelta(seconds=5),
@@ -98,15 +98,15 @@
 
         async def send_mock_data(sender: Sender[Sample]) -> None:
             while True:
                 await sender.send(Sample(datetime.now(tz=timezone.utc), 10.0))
                 await asyncio.sleep(1.0)
 
         async def run() -> None:
-            resampled_data_channel = Broadcast[Sample]("sample-data")
+            resampled_data_channel = Broadcast[Sample](name="sample-data")
             resampled_data_receiver = resampled_data_channel.new_receiver()
             resampled_data_sender = resampled_data_channel.new_sender()
 
             send_task = asyncio.create_task(send_mock_data(resampled_data_sender))
 
             # create a window that stores two days of data
             # starting at 1.1.23 with samplerate=1
@@ -341,15 +341,15 @@
         """Configure the components needed to run the resampler."""
         assert self._resampler is not None
 
         async def sink_buffer(sample: Sample[Quantity]) -> None:
             if sample.value is not None:
                 self._buffer.update(sample)
 
-        resampler_channel = Broadcast[Sample[Quantity]]("average")
+        resampler_channel = Broadcast[Sample[Quantity]](name="average")
         self._resampler_sender = resampler_channel.new_sender()
         self._resampler.add_timeseries(
             "avg", resampler_channel.new_receiver(), sink_buffer
         )
         self._tasks.add(
             asyncio.create_task(self._resampler.resample(), name="resample")
         )
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_periodic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_quantities.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_quantities.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_resampling.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_resampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 from bisect import bisect
 from collections import deque
 from collections.abc import AsyncIterator, Callable, Coroutine, Sequence
 from dataclasses import dataclass
 from datetime import datetime, timedelta, timezone
 from typing import cast
 
-from frequenz.channels.util import Timer
-from frequenz.channels.util._timer import _to_microseconds
+from frequenz.channels.timer import Timer, TriggerAllMissed, _to_microseconds
 
 from .._internal._asyncio import cancel_and_await
 from ._base_types import UNIX_EPOCH, Sample
 from ._quantities import Quantity, QuantityT
 
 _logger = logging.getLogger(__name__)
 
@@ -381,15 +380,15 @@
         time for the end of the window, the resampling windows we produce will
         have different sizes.
 
         The window end will also be aligned to the `config.align_to` time, so
         the window end is deterministic.
         """
 
-        self._timer: Timer = Timer.periodic(config.resampling_period)
+        self._timer: Timer = Timer(config.resampling_period, TriggerAllMissed())
         """The timer used to trigger the resampling windows."""
 
         # Hack to align the timer, this should be implemented in the Timer class
         self._timer._next_tick_time = _to_microseconds(
             timedelta(seconds=asyncio.get_running_loop().time())
             + config.resampling_period
             + start_delay_time
@@ -742,14 +741,16 @@
         # Using itertools for slicing doesn't look very efficient, but
         # experiments with a custom (ring) buffer that can slice showed that
         # it is not that bad. See:
         # https://github.com/frequenz-floss/frequenz-sdk-python/pull/130
         # So if we need more performance beyond this point, we probably need to
         # resort to some C (or similar) implementation.
         relevant_samples = list(itertools.islice(self._buffer, min_index, max_index))
+        if not relevant_samples:
+            _logger.warning("No relevant samples found for component: %s", self._name)
         value = (
             conf.resampling_function(relevant_samples, conf, props)
             if relevant_samples
             else None
         )
         return Sample(timestamp, None if value is None else Quantity(value))
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/buffer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_ringbuffer/serialization.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/_voltage_streamer.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/_voltage_streamer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from typing import TYPE_CHECKING
 
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
 
 from ..actor import ChannelRegistry
 from ..microgrid import connection_manager
-from ..microgrid.component import Component, ComponentCategory, ComponentMetricId
 from ..timeseries._base_types import Sample, Sample3Phase
 from ..timeseries._quantities import Quantity, Voltage
 
 if TYPE_CHECKING:
     # Imported here to avoid a circular import.
     from ..actor import ComponentMetricRequest
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,14 @@
 
 # pylint: disable=protected-access
 
 
 class BatteryPool:
     """An interface for interaction with pools of batteries.
 
-    !!! note
-        `BatteryPool` instances are not meant to be created directly by users.  Use the
-        [`microgrid.battery_pool`][frequenz.sdk.microgrid.battery_pool] method for
-        creating `BatteryPool` instances.
-
     Provides:
       - properties for fetching reporting streams of instantaneous
         [power][frequenz.sdk.timeseries.battery_pool.BatteryPool.power],
         [soc][frequenz.sdk.timeseries.battery_pool.BatteryPool.soc],
         [capacity][frequenz.sdk.timeseries.battery_pool.BatteryPool.capacity] values and
         available power bounds and other status through
         [power_status][frequenz.sdk.timeseries.battery_pool.BatteryPool.power_status].
@@ -211,30 +206,32 @@
                 pool.  If None, the proposed power of higher priority actors will take
                 precedence as the target power.
             request_timeout: The timeout for the request.
 
         Raises:
             ValueError: If the given power is negative.
         """
-        if power and power < Power.zero():
-            raise ValueError("Discharge power must be positive.")
+        if power:
+            if power < Power.zero():
+                raise ValueError("Discharge power must be positive.")
+            power = -power
         await self._battery_pool._power_manager_requests_sender.send(
             _power_managing.Proposal(
                 source_id=self._source_id,
                 preferred_power=power,
                 bounds=timeseries.Bounds(None, None),
                 component_ids=self._battery_pool._batteries,
                 priority=self._priority,
                 creation_time=asyncio.get_running_loop().time(),
                 request_timeout=request_timeout,
             )
         )
 
     @property
-    def battery_ids(self) -> abc.Set[int]:
+    def component_ids(self) -> abc.Set[int]:
         """Return ids of the batteries in the pool.
 
         Returns:
             Ids of the batteries in the pool
         """
         return self._battery_pool._batteries
 
@@ -423,7 +420,11 @@
             self._battery_pool._active_methods[method_name] = SendOnUpdate(
                 metric_calculator=calculator,
                 working_batteries=self._battery_pool._working_batteries,
                 min_update_interval=self._battery_pool._min_update_interval,
             )
 
         return self._battery_pool._active_methods[method_name]
+
+    async def stop(self) -> None:
+        """Stop all tasks and channels owned by the BatteryPool."""
+        await self._battery_pool.stop()
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_battery_pool_reference_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import asyncio
 import uuid
 from collections.abc import Awaitable, Set
 from datetime import timedelta
 from typing import Any
 
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import ComponentCategory
 
 from ..._internal._asyncio import cancel_and_await
 from ...actor._channel_registry import ChannelRegistry
 from ...actor._data_sourcing._component_metric_request import ComponentMetricRequest
 from ...actor._power_managing._base_classes import Proposal, ReportRequest
 from ...actor.power_distributing._component_status import ComponentPoolStatus
 from ...microgrid import connection_manager
-from ...microgrid.component import ComponentCategory
 from ..formula_engine._formula_engine_pool import FormulaEnginePool
 from ._methods import MetricAggregator
 
 
 class BatteryPoolReferenceStore:  # pylint: disable=too-many-instance-attributes
     """A class for maintaining the shared state/tasks for a set of pool of batteries.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from datetime import datetime, timezone
 from typing import Any, Generic, Self, TypeVar
 
 from frequenz.channels import ChannelClosedError, Receiver
+from frequenz.client.microgrid import (
+    BatteryData,
+    ComponentCategory,
+    ComponentData,
+    ComponentMetricId,
+    InverterData,
+)
 
 from ..._internal._asyncio import AsyncConstructible
 from ..._internal._constants import MAX_BATTERY_DATA_AGE_SEC
 from ...actor._data_sourcing.microgrid_api_source import (
     _BatteryDataMethods,
     _InverterDataMethods,
 )
 from ...microgrid import connection_manager
-from ...microgrid.component import (
-    BatteryData,
-    ComponentCategory,
-    ComponentData,
-    ComponentMetricId,
-    InverterData,
-)
 from ._component_metrics import ComponentMetricsData
 
 _logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=ComponentData)
 """Type variable for component data."""
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Class that stores values of the component metrics."""
 
 
 from collections.abc import Mapping
 from datetime import datetime
 
-from ...microgrid.component import ComponentMetricId
+from frequenz.client.microgrid import ComponentMetricId
 
 
 class ComponentMetricsData:
     """Store values of the component metrics."""
 
     def __init__(
         self,
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_methods.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         """Update set of the working batteries.
 
         Args:
             new_working_batteries: Set of the working batteries.
         """
 
     @abstractmethod
-    def new_receiver(self, maxsize: int | None = RECEIVER_MAX_SIZE) -> Receiver[T]:
+    def new_receiver(self, limit: int | None = RECEIVER_MAX_SIZE) -> Receiver[T]:
         """Return new receiver for the aggregated metric results.
 
         Args:
-            maxsize: Buffer size of the receiver
+            limit: Buffer size of the receiver
 
         Returns:
             Receiver for the metric results.
         """
 
     @abstractmethod
     async def stop(self) -> None:
@@ -115,26 +115,26 @@
         """Get name of the method.
 
         Returns:
             Name of the method.
         """
         return "SendOnUpdate"
 
-    def new_receiver(self, maxsize: int | None = RECEIVER_MAX_SIZE) -> Receiver[T]:
+    def new_receiver(self, limit: int | None = RECEIVER_MAX_SIZE) -> Receiver[T]:
         """Return new receiver for the aggregated metric results.
 
         Args:
-            maxsize: Buffer size of the receiver
+            limit: Buffer size of the receiver
 
         Returns:
             Receiver for the metric results.
         """
-        if maxsize is None:
+        if limit is None:
             return self._result_channel.new_receiver()
-        return self._result_channel.new_receiver(maxsize=maxsize)
+        return self._result_channel.new_receiver(limit=limit)
 
     def update_working_batteries(self, new_working_batteries: set[int]) -> None:
         """Update set of the working batteries.
 
         Recalculate metric if set changed.
 
         Args:
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 import logging
 import math
 from abc import ABC, abstractmethod
 from collections.abc import Mapping, Set
 from datetime import datetime, timezone
 from typing import Generic, TypeVar
 
+from frequenz.client.microgrid import ComponentMetricId
+
 from ... import timeseries
 from ..._internal import _math
 from ...actor.power_distributing._component_managers._battery_manager import (
     _get_battery_inverter_mappings,
 )
 from ...actor.power_distributing._distribution_algorithm._battery_distribution_algorithm import (
     _aggregate_battery_power_bounds,
 )
 from ...actor.power_distributing.result import PowerBounds
-from ...microgrid.component import ComponentMetricId
 from .._base_types import Sample, SystemBounds
 from .._quantities import Energy, Percentage, Power, Temperature
 from ._component_metrics import ComponentMetricsData
 
 _logger = logging.getLogger(__name__)
 
 _MIN_TIMESTAMP = datetime.min.replace(tzinfo=timezone.utc)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/battery_pool/_result_types.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/battery_pool/_result_types.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/consumer.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/consumer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 """A task for sending EV Charger power bounds to the microgrid API."""
 
 import asyncio
 import logging
 from dataclasses import dataclass
 from datetime import timedelta
 
-from frequenz.channels import Broadcast, Sender
-from frequenz.channels.util import Timer, select, selected_from
+from frequenz.channels import Broadcast, Sender, select, selected_from
+from frequenz.channels.timer import SkipMissedAndDrift, Timer
+from frequenz.client.microgrid import ComponentCategory, MeterData
 
 from ..._internal._asyncio import cancel_and_await
 from ..._internal._channels import LatestValueCache
 from ...microgrid import connection_manager
-from ...microgrid.component import ComponentCategory
 
 _logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ComponentCurrentLimit:
     """A current limit, to be sent to the EV Charger."""
@@ -46,17 +46,20 @@
         Args:
             repeat_interval: Interval after which to repeat the last set bounds to the
                 microgrid API, if no new calls to `set_bounds` have been made.
         """
         self._repeat_interval = repeat_interval
 
         self._task: asyncio.Task[None] = asyncio.create_task(self._run())
-        self._bounds_chan: Broadcast[ComponentCurrentLimit] = Broadcast("BoundsSetter")
+        self._bounds_chan: Broadcast[ComponentCurrentLimit] = Broadcast(
+            name="BoundsSetter"
+        )
         self._bounds_rx = self._bounds_chan.new_receiver()
         self._bounds_tx = self._bounds_chan.new_sender()
+        self._meter_data_cache: LatestValueCache[MeterData] | None = None
 
     async def set(self, component_id: int, max_amps: float) -> None:
         """Send the given current limit to the microgrid for the given component id.
 
         Args:
             component_id: ID of EV Charger to set the current bounds to.
             max_amps: maximum current in amps, that an EV can draw from this EV Charger.
@@ -69,14 +72,16 @@
         Returns:
             A new `Sender`.
         """
         return self._bounds_chan.new_sender()
 
     async def stop(self) -> None:
         """Stop the BoundsSetter."""
+        if self._meter_data_cache is not None:
+            await self._meter_data_cache.stop()
         await self._bounds_chan.close()
         await cancel_and_await(self._task)
 
     async def _run(self) -> None:
         """Wait for new bounds and forward them to the microgrid API.
 
         Also, periodically resend the last set bounds to the microgrid API, if no new
@@ -90,29 +95,31 @@
         graph = connection_manager.get().component_graph
         meters = graph.components(component_categories={ComponentCategory.METER})
         if not meters:
             err = "No meters found in the component graph."
             _logger.error(err)
             raise RuntimeError(err)
 
-        meter_data = LatestValueCache(
+        self._meter_data_cache = LatestValueCache(
             await api_client.meter_data(next(iter(meters)).component_id)
         )
         latest_bound: dict[int, ComponentCurrentLimit] = {}
 
         bound_chan = self._bounds_rx
-        timer = Timer.timeout(timedelta(self._repeat_interval.total_seconds()))
+        timer = Timer(
+            timedelta(self._repeat_interval.total_seconds()), SkipMissedAndDrift()
+        )
 
         async for selected in select(bound_chan, timer):
-            meter = meter_data.get()
+            meter = self._meter_data_cache.get()
             if meter is None:
                 raise ValueError("Meter channel closed.")
 
             if selected_from(selected, bound_chan):
-                bound: ComponentCurrentLimit = selected.value
+                bound: ComponentCurrentLimit = selected.message
                 if (
                     bound.component_id in latest_bound
                     and latest_bound[bound.component_id] == bound
                 ):
                     continue
                 latest_bound[bound.component_id] = bound
                 min_voltage = min(meter.voltage_per_phase)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
                 formula is for generating power values, this would be
                 `Power.from_watts`, for example.
         """
         self._higher_order_builder = HigherOrderFormulaBuilder
         self._name: str = builder.name
         self._builder: FormulaBuilder[QuantityT] = builder
         self._create_method = create_method
-        self._channel: Broadcast[Sample[QuantityT]] = Broadcast(self._name)
+        self._channel: Broadcast[Sample[QuantityT]] = Broadcast(name=self._name)
 
     @classmethod
     def from_receiver(
         cls,
         name: str,
         receiver: Receiver[Sample[QuantityT]],
         create_method: Callable[[float], QuantityT],
@@ -411,15 +411,15 @@
 
         Returns:
             A receiver that streams output `Sample`s from the formula engine.
         """
         if self._task is None:
             self._task = asyncio.create_task(self._run())
 
-        recv = self._channel.new_receiver(name, max_size)
+        recv = self._channel.new_receiver(name=name, limit=max_size)
 
         # This is a hack to ensure that the lifetime of the engine is tied to the
         # lifetime of the receiver.  This is necessary because the engine is a task that
         # runs forever, and in cases where higher order built for example with the below
         # idiom, the user would hold no references to the engine and it could get
         # garbage collected before the receiver.  This behaviour is explained in the
         # `asyncio.create_task` docs here:
@@ -503,15 +503,15 @@
                 formula is for generating power values, this would be
                 `Power.from_watts`, for example.
             phase_streams: output streams of formula engines running per-phase formulas.
         """
         self._higher_order_builder = HigherOrderFormulaBuilder3Phase
         self._name: str = name
         self._create_method = create_method
-        self._channel: Broadcast[Sample3Phase[QuantityT]] = Broadcast(self._name)
+        self._channel: Broadcast[Sample3Phase[QuantityT]] = Broadcast(name=self._name)
         self._task: asyncio.Task[None] | None = None
         self._streams: tuple[
             FormulaEngine[QuantityT],
             FormulaEngine[QuantityT],
             FormulaEngine[QuantityT],
         ] = phase_streams
 
@@ -549,15 +549,15 @@
 
         Returns:
             A receiver that streams output `Sample`s from the formula engine.
         """
         if self._task is None:
             self._task = asyncio.create_task(self._run())
 
-        return self._channel.new_receiver(name, max_size)
+        return self._channel.new_receiver(name=name, limit=max_size)
 
 
 class FormulaBuilder(Generic[QuantityT]):
     """Builds a post-fix formula engine that operates on `Sample` receivers.
 
     Operators and metrics need to be pushed in in-fix order, and they get rearranged
     into post-fix order.  This is done using the [Shunting yard
@@ -566,17 +566,17 @@
     Example:
         To create an engine that adds the latest entries from two receivers, the
         following calls need to be made:
 
         ```python
         from frequenz.sdk.timeseries import Power
 
-        channel = Broadcast[Sample[Power]]("channel")
-        receiver_1 = channel.new_receiver("receiver_1")
-        receiver_2 = channel.new_receiver("receiver_2")
+        channel = Broadcast[Sample[Power]](name="channel")
+        receiver_1 = channel.new_receiver(name="receiver_1")
+        receiver_2 = channel.new_receiver(name="receiver_2")
         builder = FormulaBuilder("addition", Power)
         builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
         builder.push_oper("+")
         builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
         engine = builder.build()
         ```
 
@@ -677,17 +677,17 @@
 
         For example, this clips the output of the entire expression:
 
         ```python
         from frequenz.sdk.timeseries import Power
 
         builder = FormulaBuilder("example", Power)
-        channel = Broadcast[Sample[Power]]("channel")
-        receiver_1 = channel.new_receiver("receiver_1")
-        receiver_2 = channel.new_receiver("receiver_2")
+        channel = Broadcast[Sample[Power]](name="channel")
+        receiver_1 = channel.new_receiver(name="receiver_1")
+        receiver_2 = channel.new_receiver(name="receiver_2")
 
         builder.push_oper("(")
         builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
         builder.push_oper("+")
         builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
         builder.push_oper(")")
         builder.push_clipper(min_value=0.0, max_value=None)
@@ -695,17 +695,17 @@
 
         And this clips the output of metric_2 only, and not the final result:
 
         ```python
         from frequenz.sdk.timeseries import Power
 
         builder = FormulaBuilder("example", Power)
-        channel = Broadcast[Sample[Power]]("channel")
-        receiver_1 = channel.new_receiver("receiver_1")
-        receiver_2 = channel.new_receiver("receiver_2")
+        channel = Broadcast[Sample[Power]](name="channel")
+        receiver_1 = channel.new_receiver(name="receiver_1")
+        receiver_2 = channel.new_receiver(name="receiver_2")
 
         builder.push_metric("metric_1", receiver_1, nones_are_zeros=True)
         builder.push_oper("+")
         builder.push_metric("metric_2", receiver_2, nones_are_zeros=True)
         builder.push_clipper(min_value=0.0, max_value=None)
         ```
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 """A formula pool for helping with tracking running formula engines."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from frequenz.channels import Sender
+from frequenz.client.microgrid import ComponentMetricId
 
-from ...microgrid.component import ComponentMetricId
 from .._quantities import Current, Power, Quantity
 from ._formula_generators._formula_generator import (
     FormulaGenerator,
     FormulaGeneratorConfig,
 )
 from ._resampled_formula_builder import ResampledFormulaBuilder
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/__init__.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_battery_power_formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
 import logging
 
+from frequenz.client.microgrid import ComponentMetricId
+
 from ....microgrid import connection_manager
-from ....microgrid.component import ComponentMetricId
 from ..._quantities import Power
 from ...formula_engine import FormulaEngine
 from ._formula_generator import (
     NON_EXISTING_COMPONENT_ID,
     ComponentNotFound,
     FormulaGenerationError,
     FormulaGenerator,
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_chp_power_formula.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 
 """Formula generator from component graph for CHP Power."""
 
 
 import logging
 from collections import abc
 
+from frequenz.client.microgrid import ComponentCategory, ComponentMetricId
+
 from ....microgrid import connection_manager
-from ....microgrid.component import ComponentCategory, ComponentMetricId
 from ..._quantities import Power
 from ...formula_engine import FormulaEngine
 from ._formula_generator import (
     NON_EXISTING_COMPONENT_ID,
     FormulaGenerationError,
     FormulaGenerator,
 )
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_current_formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 """Formula generator from component graph for 3-phase Grid Current."""
 
 
 import logging
 from collections import abc
 
-from ....microgrid.component import ComponentMetricId
+from frequenz.client.microgrid import ComponentMetricId
+
 from ..._quantities import Current
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
 _logger = logging.getLogger(__name__)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_ev_charger_power_formula.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # License: MIT
 # Copyright © 2023 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
 import logging
 
-from ....microgrid.component import ComponentMetricId
+from frequenz.client.microgrid import ComponentMetricId
+
 from ..._quantities import Power
 from .._formula_engine import FormulaEngine
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
 _logger = logging.getLogger(__name__)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_formula_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from abc import ABC, abstractmethod
 from collections import abc
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Generic
 
 from frequenz.channels import Sender
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
 
-from ....microgrid import component, connection_manager
-from ....microgrid.component import ComponentMetricId
+from ....microgrid import connection_manager
 from ..._quantities import QuantityT
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from .._resampled_formula_builder import ResampledFormulaBuilder
 
 if TYPE_CHECKING:
     # Break circular import
     from ....actor import ChannelRegistry, ComponentMetricRequest
@@ -91,39 +91,39 @@
             self._channel_registry,
             self._resampler_subscription_sender,
             component_metric_id,
             create_method,
         )
         return builder
 
-    def _get_grid_component(self) -> component.Component:
+    def _get_grid_component(self) -> Component:
         """
         Get the grid component in the component graph.
 
         Returns:
             The first grid component found in the graph.
 
         Raises:
             ComponentNotFound: If the grid component is not found in the component graph.
         """
         component_graph = connection_manager.get().component_graph
         grid_component = next(
             iter(
                 component_graph.components(
-                    component_categories={component.ComponentCategory.GRID}
+                    component_categories={ComponentCategory.GRID}
                 )
             ),
             None,
         )
         if grid_component is None:
             raise ComponentNotFound("Grid component not found in the component graph.")
 
         return grid_component
 
-    def _get_grid_component_successors(self) -> set[component.Component]:
+    def _get_grid_component_successors(self) -> set[Component]:
         """Get the set of grid component successors in the component graph.
 
         Returns:
             A set of grid component successors.
 
         Raises:
             ComponentNotFound: If no successor components are found in the component graph.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for 3-phase Grid Current."""
 
-from ....microgrid.component import Component, ComponentCategory, ComponentMetricId
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
+
 from ..._quantities import Current
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from ._formula_generator import FormulaGenerator
 
 
 class GridCurrentFormula(FormulaGenerator[Current]):
     """Create a formula engine from the component graph for calculating grid current."""
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # License: MIT
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for 3-phase Grid Power."""
 
-from ....microgrid.component import Component, ComponentCategory, ComponentMetricId
+from frequenz.client.microgrid import Component, ComponentCategory, ComponentMetricId
+
 from ..._quantities import Power
 from .._formula_engine import FormulaEngine, FormulaEngine3Phase
 from ._formula_generator import FormulaGenerator
 
 
 class GridPower3PhaseFormula(FormulaGenerator[Power]):
     """Create a formula engine for calculating the grid 3-phase power."""
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Grid Power."""
 
-from ....microgrid.component import ComponentCategory, ComponentMetricId
+from frequenz.client.microgrid import ComponentCategory, ComponentMetricId
+
 from ..._quantities import Power
 from .._formula_engine import FormulaEngine
 from ._formula_generator import FormulaGenerator
 
 
 class GridPowerFormula(FormulaGenerator[Power]):
     """Creates a formula engine from the component graph for calculating grid power."""
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator from component graph for Producer Power."""
 
 import logging
 
+from frequenz.client.microgrid import ComponentCategory, ComponentMetricId
+
 from ....microgrid import connection_manager
-from ....microgrid.component import ComponentCategory, ComponentMetricId
 from ..._quantities import Power
 from .._formula_engine import FormulaEngine
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
 _logger = logging.getLogger(__name__)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # License: MIT
 # Copyright © 2022 Frequenz Energy-as-a-Service GmbH
 
 """Formula generator for PV Power, from the component graph."""
 
 import logging
 
+from frequenz.client.microgrid import ComponentCategory, ComponentMetricId
+
 from ....microgrid import connection_manager
-from ....microgrid.component import ComponentCategory, ComponentMetricId
 from ..._quantities import Power
 from .._formula_engine import FormulaEngine
 from ._formula_generator import NON_EXISTING_COMPONENT_ID, FormulaGenerator
 
 _logger = logging.getLogger(__name__)
 
 
@@ -33,19 +34,23 @@
                 successors.
         """
         builder = self._get_builder(
             "pv-power", ComponentMetricId.ACTIVE_POWER, Power.from_watts
         )
 
         component_graph = connection_manager.get().component_graph
-        pv_components = component_graph.dfs(
-            self._get_grid_component(),
-            set(),
-            component_graph.is_pv_chain,
-        )
+        component_ids = self._config.component_ids
+        if component_ids:
+            pv_components = component_graph.components(set(component_ids))
+        else:
+            pv_components = component_graph.dfs(
+                self._get_grid_component(),
+                set(),
+                component_graph.is_pv_chain,
+            )
 
         if not pv_components:
             _logger.warning(
                 "Unable to find any PV components in the component graph. "
                 "Subscribing to the resampling actor with a non-existing "
                 "component id, so that `0` values are sent from the formula."
             )
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_resampled_formula_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from __future__ import annotations
 
 from collections.abc import Callable
 from typing import TYPE_CHECKING
 
 from frequenz.channels import Receiver, Sender
+from frequenz.client.microgrid import ComponentMetricId
 
-from ...microgrid.component import ComponentMetricId
 from .. import Sample
 from .._quantities import Quantity, QuantityT
 from ._formula_engine import FormulaBuilder, FormulaEngine
 from ._tokenizer import Tokenizer, TokenType
 
 if TYPE_CHECKING:
     # Break circular import
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/formula_engine/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/grid.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 import logging
 import uuid
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from frequenz.channels import Sender
+from frequenz.client.microgrid._component import ComponentCategory
 
 from ..microgrid import connection_manager
-from ..microgrid.component._component import ComponentCategory
-from . import Fuse
+from ._fuse import Fuse
 from ._quantities import Current, Power
 from .formula_engine import FormulaEngine, FormulaEngine3Phase
 from .formula_engine._formula_engine_pool import FormulaEnginePool
 from .formula_engine._formula_generators import (
     GridCurrentFormula,
     GridPower3PhaseFormula,
     GridPowerFormula,
@@ -191,16 +191,18 @@
         # The current implementation of the Component Graph fails to
         # effectively convert components from a dictionary representation to
         # the expected Component object.
         # Specifically for the component metadata, it hands back a dictionary
         # instead of the expected ComponentMetadata type.
         metadata = grid_connections[0].metadata
         if isinstance(metadata, dict):
-            fuse_dict = metadata.get("fuse", None)
-            fuse = Fuse(**fuse_dict) if fuse_dict else None
+            if fuse_dict := metadata.get("fuse", None):
+                fuse = Fuse(
+                    max_current=Current.from_amperes(fuse_dict.get("max_current", 0.0))
+                )
 
         if fuse is None:
             _logger.warning("The grid connection point does not have a fuse")
 
     namespace = f"grid-{uuid.uuid4()}"
     formula_pool = FormulaEnginePool(
         namespace,
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 """A logical meter for calculating high level metrics for a microgrid."""
 
 
 import uuid
 
 from frequenz.channels import Sender
+from frequenz.client.microgrid import ComponentMetricId
 
 from ...actor import ChannelRegistry, ComponentMetricRequest
-from ...microgrid.component import ComponentMetricId
 from .._quantities import Power, Quantity
 from ..formula_engine import FormulaEngine
 from ..formula_engine._formula_engine_pool import FormulaEnginePool
-from ..formula_engine._formula_generators import CHPPowerFormula, PVPowerFormula
+from ..formula_engine._formula_generators import CHPPowerFormula
 
 
 class LogicalMeter:
     """A logical meter for calculating high level metrics in a microgrid.
 
     LogicalMeter provides methods for fetching power values from different points in the
     microgrid.  These methods return `FormulaReceiver` objects, which can be used like
@@ -38,25 +38,26 @@
         await microgrid.initialize(
             "127.0.0.1",
             50051,
             ResamplerConfig(resampling_period=timedelta(seconds=1))
         )
 
         logical_meter = microgrid.logical_meter()
+        pv_pool = microgrid.pv_pool()
         grid = microgrid.grid()
 
         # Get a receiver for a builtin formula
-        pv_power_recv = logical_meter.pv_power.new_receiver()
+        pv_power_recv = pv_pool.power.new_receiver()
         async for pv_power_sample in pv_power_recv:
             print(pv_power_sample)
 
         # or compose formulas to create a new formula
         net_power_recv = (
             (
-                grid.power - logical_meter.pv_power
+                grid.power - pv_pool.power
             )
             .build("net_power")
             .new_receiver()
         )
         async for net_power_sample in net_power_recv:
             print(net_power_sample)
         ```
@@ -120,36 +121,14 @@
             A FormulaEngine that applies the formula and streams values.
         """
         return self._formula_pool.from_string(
             formula, component_metric_id, nones_are_zeros=nones_are_zeros
         )
 
     @property
-    def pv_power(self) -> FormulaEngine[Power]:
-        """Fetch the PV power in the microgrid.
-
-        This formula produces values that are in the Passive Sign Convention (PSC).
-
-        If a formula engine to calculate PV power is not already running, it will be
-        started.
-
-        A receiver from the formula engine can be created using the `new_receiver`
-        method.
-
-        Returns:
-            A FormulaEngine that will calculate and stream PV total power.
-        """
-        engine = self._formula_pool.from_power_formula_generator(
-            "pv_power",
-            PVPowerFormula,
-        )
-        assert isinstance(engine, FormulaEngine)
-        return engine
-
-    @property
     def chp_power(self) -> FormulaEngine[Power]:
         """Fetch the CHP power production in the microgrid.
 
         This formula produces values that are in the Passive Sign Convention (PSC).
 
         If a formula engine to calculate CHP power production is not already running, it
         will be started.
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz/sdk/timeseries/producer.py` & `frequenz-sdk-1.0.0rc6/src/frequenz/sdk/timeseries/producer.py`

 * *Files identical despite different names*

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/PKG-INFO` & `frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-sdk
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: A development kit to interact with the Frequenz development platform
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-sdk-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-sdk-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-sdk-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-sdk-python
@@ -17,15 +17,16 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: <4,>=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: frequenz-api-microgrid<0.16.0,>=0.15.3
-Requires-Dist: frequenz-channels==1.0.0b2
+Requires-Dist: frequenz-channels<2.0.0,>=1.0.0-rc1
+Requires-Dist: frequenz-client-microgrid<0.4.0,>=0.3.0
 Requires-Dist: google-api-python-client<3,>=2.71
 Requires-Dist: grpcio<2,>=1.54.2
 Requires-Dist: grpcio-tools<2,>=1.54.2
 Requires-Dist: networkx<4,>=2.8
 Requires-Dist: numpy<2,>=1.24.2
 Requires-Dist: protobuf<5,>=4.21.6
 Requires-Dist: pydantic<3,>=2.3
@@ -33,53 +34,53 @@
 Requires-Dist: tqdm<5,>=4.38.0
 Requires-Dist: typing_extensions<5,>=4.6.1
 Requires-Dist: watchfiles>=0.15.0
 Provides-Extra: dev-flake8
 Requires-Dist: flake8==7.0.0; extra == "dev-flake8"
 Requires-Dist: flake8-docstrings==1.7.0; extra == "dev-flake8"
 Requires-Dist: flake8-pyproject==1.2.3; extra == "dev-flake8"
-Requires-Dist: pydoclint==0.3.8; extra == "dev-flake8"
+Requires-Dist: pydoclint==0.4.1; extra == "dev-flake8"
 Requires-Dist: pydocstyle==6.3.0; extra == "dev-flake8"
 Provides-Extra: dev-examples
-Requires-Dist: polars==0.20.2; extra == "dev-examples"
+Requires-Dist: polars==0.20.18; extra == "dev-examples"
 Provides-Extra: dev-formatting
-Requires-Dist: black==24.1.1; extra == "dev-formatting"
+Requires-Dist: black==24.3.0; extra == "dev-formatting"
 Requires-Dist: isort==5.13.2; extra == "dev-formatting"
 Provides-Extra: dev-mkdocs
-Requires-Dist: black==24.1.1; extra == "dev-mkdocs"
-Requires-Dist: Markdown==3.5.1; extra == "dev-mkdocs"
+Requires-Dist: black==24.3.0; extra == "dev-mkdocs"
+Requires-Dist: Markdown==3.6; extra == "dev-mkdocs"
 Requires-Dist: mike==2.0.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-gen-files==0.5.0; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-literate-nav==0.6.1; extra == "dev-mkdocs"
 Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == "dev-mkdocs"
-Requires-Dist: mkdocs-material==9.5.3; extra == "dev-mkdocs"
-Requires-Dist: mkdocstrings[python]==0.24.0; extra == "dev-mkdocs"
-Requires-Dist: frequenz-repo-config[lib]==0.7.4; extra == "dev-mkdocs"
+Requires-Dist: mkdocs-material==9.5.16; extra == "dev-mkdocs"
+Requires-Dist: mkdocstrings[python]==0.24.1; extra == "dev-mkdocs"
+Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-mkdocs"
 Provides-Extra: dev-mypy
-Requires-Dist: mypy==1.8.0; extra == "dev-mypy"
+Requires-Dist: mypy==1.9.0; extra == "dev-mypy"
 Requires-Dist: grpc-stubs==1.24.12; extra == "dev-mypy"
-Requires-Dist: types-Markdown==3.5.0.3; extra == "dev-mypy"
+Requires-Dist: types-Markdown==3.6.0.20240316; extra == "dev-mypy"
 Requires-Dist: types-protobuf==4.24.0.20240129; extra == "dev-mypy"
-Requires-Dist: types-setuptools==69.0.0.20240125; extra == "dev-mypy"
+Requires-Dist: types-setuptools==69.2.0.20240317; extra == "dev-mypy"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-mypy"
 Provides-Extra: dev-noxfile
 Requires-Dist: nox==2023.4.22; extra == "dev-noxfile"
-Requires-Dist: frequenz-repo-config[lib]==0.7.4; extra == "dev-noxfile"
+Requires-Dist: frequenz-repo-config[lib]==0.9.1; extra == "dev-noxfile"
 Provides-Extra: dev-pylint
-Requires-Dist: pylint==3.0.3; extra == "dev-pylint"
+Requires-Dist: pylint==3.1.0; extra == "dev-pylint"
 Requires-Dist: frequenz-sdk[dev-mkdocs,dev-noxfile,dev-pytest]; extra == "dev-pylint"
 Provides-Extra: dev-pytest
-Requires-Dist: pytest==7.4.4; extra == "dev-pytest"
-Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.7.4; extra == "dev-pytest"
-Requires-Dist: pytest-mock==3.12.0; extra == "dev-pytest"
-Requires-Dist: pytest-asyncio==0.23.3; extra == "dev-pytest"
+Requires-Dist: pytest==8.1.1; extra == "dev-pytest"
+Requires-Dist: frequenz-repo-config[extra-lint-examples]==0.9.1; extra == "dev-pytest"
+Requires-Dist: pytest-mock==3.14.0; extra == "dev-pytest"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev-pytest"
 Requires-Dist: time-machine==2.12.0; extra == "dev-pytest"
-Requires-Dist: async-solipsism==0.5; extra == "dev-pytest"
+Requires-Dist: async-solipsism==0.6; extra == "dev-pytest"
 Requires-Dist: frequenz-sdk[dev-examples]; extra == "dev-pytest"
-Requires-Dist: hypothesis==6.92.1; extra == "dev-pytest"
+Requires-Dist: hypothesis==6.100.0; extra == "dev-pytest"
 Provides-Extra: dev
 Requires-Dist: frequenz-sdk[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]; extra == "dev"
 
 # Frequenz Python SDK
 
 [![Build Status](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml/badge.svg)](https://github.com/frequenz-floss/frequenz-sdk-python/actions/workflows/ci.yaml)
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-sdk)](https://pypi.org/project/frequenz-sdk/)
```

### Comparing `frequenz-sdk-1.0.0rc5/src/frequenz_sdk.egg-info/SOURCES.txt` & `frequenz-sdk-1.0.0rc6/src/frequenz_sdk.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 RELEASE_NOTES.md
 pyproject.toml
 examples/__init__.py
 examples/battery_pool.py
 src/frequenz/sdk/__init__.py
 src/frequenz/sdk/conftest.py
 src/frequenz/sdk/py.typed
-src/frequenz/sdk/_api_client/__init__.py
-src/frequenz/sdk/_api_client/api_client.py
 src/frequenz/sdk/_internal/__init__.py
 src/frequenz/sdk/_internal/_asyncio.py
 src/frequenz/sdk/_internal/_channels.py
 src/frequenz/sdk/_internal/_constants.py
 src/frequenz/sdk/_internal/_math.py
 src/frequenz/sdk/_internal/_singleton_meta.py
 src/frequenz/sdk/actor/__init__.py
@@ -37,36 +35,35 @@
 src/frequenz/sdk/actor/power_distributing/_component_pool_status_tracker.py
 src/frequenz/sdk/actor/power_distributing/power_distributing.py
 src/frequenz/sdk/actor/power_distributing/request.py
 src/frequenz/sdk/actor/power_distributing/result.py
 src/frequenz/sdk/actor/power_distributing/_component_managers/__init__.py
 src/frequenz/sdk/actor/power_distributing/_component_managers/_battery_manager.py
 src/frequenz/sdk/actor/power_distributing/_component_managers/_component_manager.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/__init__.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_config.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_ev_charger_manager.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_ev_charger_manager/_states.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/__init__.py
+src/frequenz/sdk/actor/power_distributing/_component_managers/_pv_inverter_manager/_pv_inverter_manager.py
 src/frequenz/sdk/actor/power_distributing/_component_status/__init__.py
 src/frequenz/sdk/actor/power_distributing/_component_status/_battery_status_tracker.py
 src/frequenz/sdk/actor/power_distributing/_component_status/_blocking_status.py
 src/frequenz/sdk/actor/power_distributing/_component_status/_component_status.py
+src/frequenz/sdk/actor/power_distributing/_component_status/_ev_charger_status_tracker.py
+src/frequenz/sdk/actor/power_distributing/_component_status/_pv_inverter_status_tracker.py
 src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/__init__.py
 src/frequenz/sdk/actor/power_distributing/_distribution_algorithm/_battery_distribution_algorithm.py
 src/frequenz/sdk/config/__init__.py
 src/frequenz/sdk/config/_config.py
 src/frequenz/sdk/microgrid/__init__.py
 src/frequenz/sdk/microgrid/_data_pipeline.py
 src/frequenz/sdk/microgrid/_power_wrapper.py
 src/frequenz/sdk/microgrid/component_graph.py
 src/frequenz/sdk/microgrid/connection_manager.py
-src/frequenz/sdk/microgrid/metadata.py
-src/frequenz/sdk/microgrid/client/__init__.py
-src/frequenz/sdk/microgrid/client/_client.py
-src/frequenz/sdk/microgrid/client/_connection.py
-src/frequenz/sdk/microgrid/client/_retry.py
-src/frequenz/sdk/microgrid/component/__init__.py
-src/frequenz/sdk/microgrid/component/_component.py
-src/frequenz/sdk/microgrid/component/_component_data.py
-src/frequenz/sdk/microgrid/component/_component_states.py
 src/frequenz/sdk/timeseries/__init__.py
 src/frequenz/sdk/timeseries/_base_types.py
 src/frequenz/sdk/timeseries/_fuse.py
 src/frequenz/sdk/timeseries/_grid_frequency.py
 src/frequenz/sdk/timeseries/_moving_window.py
 src/frequenz/sdk/timeseries/_periodic_feature_extractor.py
 src/frequenz/sdk/timeseries/_quantities.py
@@ -84,16 +81,18 @@
 src/frequenz/sdk/timeseries/battery_pool/_component_metric_fetcher.py
 src/frequenz/sdk/timeseries/battery_pool/_component_metrics.py
 src/frequenz/sdk/timeseries/battery_pool/_methods.py
 src/frequenz/sdk/timeseries/battery_pool/_metric_calculator.py
 src/frequenz/sdk/timeseries/battery_pool/_result_types.py
 src/frequenz/sdk/timeseries/ev_charger_pool/__init__.py
 src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool.py
+src/frequenz/sdk/timeseries/ev_charger_pool/_ev_charger_pool_reference_store.py
+src/frequenz/sdk/timeseries/ev_charger_pool/_result_types.py
 src/frequenz/sdk/timeseries/ev_charger_pool/_set_current_bounds.py
-src/frequenz/sdk/timeseries/ev_charger_pool/_state_tracker.py
+src/frequenz/sdk/timeseries/ev_charger_pool/_system_bounds_tracker.py
 src/frequenz/sdk/timeseries/formula_engine/__init__.py
 src/frequenz/sdk/timeseries/formula_engine/_exceptions.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_engine.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_engine_pool.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_evaluator.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_formatter.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_steps.py
@@ -109,12 +108,17 @@
 src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_current_formula.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_3_phase_formula.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_grid_power_formula.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_producer_power_formula.py
 src/frequenz/sdk/timeseries/formula_engine/_formula_generators/_pv_power_formula.py
 src/frequenz/sdk/timeseries/logical_meter/__init__.py
 src/frequenz/sdk/timeseries/logical_meter/_logical_meter.py
+src/frequenz/sdk/timeseries/pv_pool/__init__.py
+src/frequenz/sdk/timeseries/pv_pool/_pv_pool.py
+src/frequenz/sdk/timeseries/pv_pool/_pv_pool_reference_store.py
+src/frequenz/sdk/timeseries/pv_pool/_result_types.py
+src/frequenz/sdk/timeseries/pv_pool/_system_bounds_tracker.py
 src/frequenz_sdk.egg-info/PKG-INFO
 src/frequenz_sdk.egg-info/SOURCES.txt
 src/frequenz_sdk.egg-info/dependency_links.txt
 src/frequenz_sdk.egg-info/requires.txt
 src/frequenz_sdk.egg-info/top_level.txt
```

