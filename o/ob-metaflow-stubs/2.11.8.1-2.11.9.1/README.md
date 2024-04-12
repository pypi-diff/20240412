# Comparing `tmp/ob-metaflow-stubs-2.11.8.1.tar.gz` & `tmp/ob-metaflow-stubs-2.11.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-stubs-2.11.8.1.tar", last modified: Fri Mar 29 12:40:00 2024, max compression
+gzip compressed data, was "ob-metaflow-stubs-2.11.9.1.tar", last modified: Sat Mar 30 09:14:02 2024, max compression
```

## Comparing `ob-metaflow-stubs-2.11.8.1.tar` & `ob-metaflow-stubs-2.11.9.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 12:39:35.000000 ob-metaflow-stubs-2.11.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 12:39:35.000000 ob-metaflow-stubs-2.11.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.007521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107562 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.007521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.007521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.007521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.011521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.011521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.011521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.015521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.015521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.015521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.015521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.019521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.019521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_credential.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.023521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.023521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.023521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.023521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.027521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.027521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.027521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.027521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/procpoll.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-29 12:39:58.000000 ob-metaflow-stubs-2.11.8.1/metaflow-stubs/tagging_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:40:00.031521 ob-metaflow-stubs-2.11.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-29 12:39:35.000000 ob-metaflow-stubs-2.11.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-29 12:39:59.000000 ob-metaflow-stubs-2.11.8.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107562 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.604047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.608047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14373 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.612047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_credential.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.616047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.620047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-30 09:14:01.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/procpoll.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-30 09:14:00.000000 ob-metaflow-stubs-2.11.9.1/metaflow-stubs/tagging_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 09:14:02.624047 ob-metaflow-stubs-2.11.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-30 09:13:40.000000 ob-metaflow-stubs-2.11.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-30 09:14:02.000000 ob-metaflow-stubs-2.11.9.1/version.py
```

### Comparing `ob-metaflow-stubs-2.11.8.1/PKG-INFO` & `ob-metaflow-stubs-2.11.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 2.11.8.1
+Version: 2.11.9.1
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: ob-metaflow==2.11.8.1
+Requires-Dist: ob-metaflow==2.11.9.1
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.338796                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.953272                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import typing
-    import io
-    import metaflow.events
-    import metaflow.plugins.datatools.s3.s3
+    import metaflow.parameters
     import metaflow.datastore.inputs
     import metaflow.client.core
-    import metaflow._vendor.click.types
+    import metaflow.events
+    import metaflow.plugins.datatools.s3.s3
+    import io
     import datetime
-    import metaflow.parameters
+    import typing
+    import metaflow._vendor.click.types
+    import metaflow.metaflow_current
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,100 +722,140 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
-def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
+def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
     """
-    Specifies environment variables to be set prior to the execution of a step.
+    Specifies the resources needed when executing this step.
+    
+    Use `@resources` to specify the resource requirements
+    independently of the specific compute layer (`@batch`, `@kubernetes`).
+    
+    You can choose the compute layer on the command line by executing e.g.
+    ```
+    python myflow.py run --with batch
+    ```
+    or
+    ```
+    python myflow.py run --with kubernetes
+    ```
+    which executes the flow on the desired system using the
+    requirements specified in `@resources`.
     
     Parameters
     ----------
-    vars : Dict[str, str], default {}
-        Dictionary of environment variables to set.
+    cpu : int, default 1
+        Number of CPUs required for this step.
+    gpu : int, default 0
+        Number of GPUs required for this step.
+    disk : int, optional, default None
+        Disk size (in MB) required for this step. Only applies on Kubernetes.
+    memory : int, default 4096
+        Memory size (in MB) required for this step.
+    shared_memory : int, optional, default None
+        The value for the size (in MiB) of the /dev/shm volume for this step.
+        This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
-def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, port: typing.Optional[int] = None, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+@typing.overload
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies that this step should execute on Kubernetes.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    cpu : int, default 1
-        Number of CPUs required for this step. If `@resources` is
-        also present, the maximum value from all decorators is used.
-    memory : int, default 4096
-        Memory size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    disk : int, default 10240
-        Disk size (in MB) required for this step. If
-        `@resources` is also present, the maximum value from all decorators is
-        used.
-    image : str, optional, default None
-        Docker image to use when launching on Kubernetes. If not specified, and
-        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
-        not, a default Docker image mapping to the current version of Python is used.
-    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
-        If given, the imagePullPolicy to be applied to the Docker image of the step.
-    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
-        Kubernetes service account to use when launching pod in Kubernetes.
-    secrets : List[str], optional, default None
-        Kubernetes secrets to use when launching pod in Kubernetes. These
-        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
-        in Metaflow configuration.
-    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
-        Kubernetes namespace to use when launching pod in Kubernetes.
-    gpu : int, optional, default None
-        Number of GPUs required for this step. A value of zero implies that
-        the scheduled node should not have GPUs.
-    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
-        The vendor of the GPUs to be used for this step.
-    tolerations : List[str], default []
-        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
-        Kubernetes tolerations to use when launching pod in Kubernetes.
-    use_tmpfs : bool, default False
-        This enables an explicit tmpfs mount for this step.
-    tmpfs_tempdir : bool, default True
-        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
-    tmpfs_size : int, optional, default: None
-        The value for the size (in MiB) of the tmpfs mount for this step.
-        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
-        memory allocated for this step.
-    tmpfs_path : str, optional, default /metaflow_temp
-        Path to tmpfs mount for this step.
-    persistent_volume_claims : Dict[str, str], optional, default None
-        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
-        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
-    port: int, optional
-        Number of the port to specify in the Kubernetes job object
-    shared_memory: int, optional
-        Shared memory size (in MiB) required for this steps
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
+    """
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+    """
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
+    
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
+    
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
+    
+    Parameters
+    ----------
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
 def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies a timeout for your step.
@@ -869,148 +909,14 @@
         Number of minutes to wait prior to timing out.
     hours : int, default 0
         Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the Conda environment for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-@typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
-    """
-    Specifies the Conda environment for the step.
-    
-    Information in this decorator will augment any
-    attributes set in the `@conda_base` flow-level decorator. Hence,
-    you can use `@conda_base` to set packages required by all
-    steps and use `@conda` to specify step-specific overrides.
-    
-    Parameters
-    ----------
-    packages : Dict[str, str], default {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    libraries : Dict[str, str], default {}
-        Supported for backward compatibility. When used with packages, packages will take precedence.
-    python : str, optional, default None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    disabled : bool, default False
-        If set to True, disables @conda.
-    """
-    ...
-
-@typing.overload
-def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    """
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def resources(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def resources(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None):
-    """
-    Specifies the resources needed when executing this step.
-    
-    Use `@resources` to specify the resource requirements
-    independently of the specific compute layer (`@batch`, `@kubernetes`).
-    
-    You can choose the compute layer on the command line by executing e.g.
-    ```
-    python myflow.py run --with batch
-    ```
-    or
-    ```
-    python myflow.py run --with kubernetes
-    ```
-    which executes the flow on the desired system using the
-    requirements specified in `@resources`.
-    
-    Parameters
-    ----------
-    cpu : int, default 1
-        Number of CPUs required for this step.
-    gpu : int, default 0
-        Number of GPUs required for this step.
-    disk : int, optional, default None
-        Disk size (in MB) required for this step. Only applies on Kubernetes.
-    memory : int, default 4096
-        Memory size (in MB) required for this step.
-    shared_memory : int, optional, default None
-        The value for the size (in MiB) of the /dev/shm volume for this step.
-        This parameter maps to the `--shm-size` option in Docker.
-    """
-    ...
-
-@typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
     cpu : int, default 1
@@ -1150,63 +1056,202 @@
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
+    Creates a human-readable report, a Metaflow Card, after this step completes.
     
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that the step will success under all circumstances.
+    
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
+    
+    Parameters
+    ----------
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
+    """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+@typing.overload
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
+    Specifies that the step will success under all circumstances.
     
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Parameters
+    ----------
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
+    """
+    ...
+
+@typing.overload
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+    """
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
+    
+    Parameters
+    ----------
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
+    """
+    ...
+
+def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, port: typing.Optional[int] = None, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Specifies that this step should execute on Kubernetes.
+    
+    Parameters
+    ----------
+    cpu : int, default 1
+        Number of CPUs required for this step. If `@resources` is
+        also present, the maximum value from all decorators is used.
+    memory : int, default 4096
+        Memory size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    disk : int, default 10240
+        Disk size (in MB) required for this step. If
+        `@resources` is also present, the maximum value from all decorators is
+        used.
+    image : str, optional, default None
+        Docker image to use when launching on Kubernetes. If not specified, and
+        METAFLOW_KUBERNETES_CONTAINER_IMAGE is specified, that image is used. If
+        not, a default Docker image mapping to the current version of Python is used.
+    image_pull_policy: str, default KUBERNETES_IMAGE_PULL_POLICY
+        If given, the imagePullPolicy to be applied to the Docker image of the step.
+    service_account : str, default METAFLOW_KUBERNETES_SERVICE_ACCOUNT
+        Kubernetes service account to use when launching pod in Kubernetes.
+    secrets : List[str], optional, default None
+        Kubernetes secrets to use when launching pod in Kubernetes. These
+        secrets are in addition to the ones defined in `METAFLOW_KUBERNETES_SECRETS`
+        in Metaflow configuration.
+    namespace : str, default METAFLOW_KUBERNETES_NAMESPACE
+        Kubernetes namespace to use when launching pod in Kubernetes.
+    gpu : int, optional, default None
+        Number of GPUs required for this step. A value of zero implies that
+        the scheduled node should not have GPUs.
+    gpu_vendor : str, default KUBERNETES_GPU_VENDOR
+        The vendor of the GPUs to be used for this step.
+    tolerations : List[str], default []
+        The default is extracted from METAFLOW_KUBERNETES_TOLERATIONS.
+        Kubernetes tolerations to use when launching pod in Kubernetes.
+    use_tmpfs : bool, default False
+        This enables an explicit tmpfs mount for this step.
+    tmpfs_tempdir : bool, default True
+        sets METAFLOW_TEMPDIR to tmpfs_path if set for this step.
+    tmpfs_size : int, optional, default: None
+        The value for the size (in MiB) of the tmpfs mount for this step.
+        This parameter maps to the `--tmpfs` option in Docker. Defaults to 50% of the
+        memory allocated for this step.
+    tmpfs_path : str, optional, default /metaflow_temp
+        Path to tmpfs mount for this step.
+    persistent_volume_claims : Dict[str, str], optional, default None
+        A map (dictionary) of persistent volumes to be mounted to the pod for this step. The map is from persistent
+        volumes to the path to which the volume is to be mounted, e.g., `{'pvc-name': '/path/to/mount/on'}`.
+    port: int, optional
+        Number of the port to specify in the Kubernetes job object
+    shared_memory: int, optional
+        Shared memory size (in MiB) required for this steps
     """
     ...
 
 @typing.overload
 def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the PyPI packages for the step.
@@ -1252,143 +1297,197 @@
     python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def conda(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies the Conda environment for the step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def conda(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+def conda(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False):
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies the Conda environment for the step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    Information in this decorator will augment any
+    attributes set in the `@conda_base` flow-level decorator. Hence,
+    you can use `@conda_base` to set packages required by all
+    steps and use `@conda` to specify step-specific overrides.
     
     Parameters
     ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
+    packages : Dict[str, str], default {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    libraries : Dict[str, str], default {}
+        Supported for backward compatibility. When used with packages, packages will take precedence.
+    python : str, optional, default None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    disabled : bool, default False
+        If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
     """
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def environment(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
+def environment(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, vars: typing.Dict[str, str] = {}):
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    vars : Dict[str, str], default {}
+        Dictionary of environment variables to set.
     """
     ...
 
-@typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies that the step will success under all circumstances.
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
     
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
+    """
+    ...
+
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies what flows belong to the same project.
+    
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
     
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
+    
+    
     """
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the PyPI packages for all steps of the flow.
+    
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
+    Parameters
+    ----------
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
+    """
     ...
 
 @typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
     ...
 
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
+def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
+    Specifies the PyPI packages for all steps of the flow.
     
+    Use `@pypi_base` to set common packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     Parameters
     ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
+    packages : Dict[str, str], default: {}
+        Packages to use for this flow. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
 def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the event(s) that this flow depends on.
@@ -1479,135 +1578,14 @@
     options : Dict[str, Any], default {}
         Backend-specific configuration for tuning eventing behavior.
     
     
     """
     ...
 
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies what flows belong to the same project.
-    
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
-    
-    Parameters
-    ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the flow(s) that this flow depends on.
-    
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
-    
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
-    
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
-    
-    Parameters
-    ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
-@typing.overload
-def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
-    """
-    Specifies the flow(s) that this flow depends on.
-    
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
-    
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
-    
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
-    
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
-    
-    Parameters
-    ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
-    """
-    ...
-
 @typing.overload
 def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the times when the flow should be run when running on a
     production scheduler.
     
     Parameters
@@ -1650,95 +1628,14 @@
     timezone : str, optional, default None
         Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
         which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
     """
     ...
 
 @typing.overload
-def pypi_base(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-@typing.overload
-def pypi_base(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def pypi_base(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
-    """
-    Specifies the PyPI packages for all steps of the flow.
-    
-    Use `@pypi_base` to set common packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
-    Parameters
-    ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this flow. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
-    """
-    ...
-
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
-    """
-    ...
-
-@typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
     
@@ -1821,14 +1718,117 @@
     aws_conn_id : str
         a reference to the s3 connection on Airflow. (Default: None)
     verify : bool
         Whether or not to verify SSL certificates for S3 connection. (Default: None)
     """
     ...
 
+@typing.overload
+def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+    
+    Parameters
+    ----------
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
+    """
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+    
+    Parameters
+    ----------
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
     pass None to this call.
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/cards.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cards.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.364037                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.979633                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
-    import typing
-    import metaflow.plugins.cards.card_modules.components
-    import metaflow.plugins.cards.card_client
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_client
+    import typing
     import metaflow
+    import metaflow.plugins.cards.card_modules.components
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/cli.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.370935                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.985572                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.368181                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.982872                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
-    import metaflow.client.core
     import metaflow.events
     import datetime
+    import metaflow.client.core
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/core.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.349753                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.964242                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import tarfile
-    import typing
-    import metaflow.exception
-    import metaflow.events
     import metaflow.client.core
+    import metaflow.events
     import datetime
+    import metaflow.exception
+    import typing
+    import tarfile
     import metaflow
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/client/filecache.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/client/filecache.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.372025                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.986643                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.exception
     import metaflow.datastore.content_addressed_store
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/clone_util.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/clone_util.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.368634                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.983241                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/events.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.352143                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.966700                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.events
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/exception.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/exception.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.339919                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.954414                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/flowspec.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.351415                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.965966                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.exception
-    import metaflow.datastore.inputs
     import metaflow.unbounded_foreach
     import metaflow.parameters
+    import metaflow.datastore.inputs
+    import typing
+    import metaflow.exception
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/includefile.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.361827                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.977307                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import io
+    import metaflow.parameters
     import metaflow.plugins.datatools.s3.s3
+    import typing
     import metaflow._vendor.click.types
-    import metaflow.parameters
+    import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metadata/metadata.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/metadata.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.395038                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.008282                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metadata.metadata
     import metaflow.exception
+    import metaflow.metadata.metadata
 
 class MetaflowInternalError(metaflow.exception.MetaflowException, metaclass=type):
     ...
 
 class MetaflowTaggingError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metadata/util.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metadata/util.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.436969                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.061559                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def copy_tree(src, dst, update = False):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metaflow_config.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.341349                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.955711                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/metaflow_current.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/metaflow_current.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.453613                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.065876                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import typing
     import metaflow.plugins.cards.component_serializer
     import metaflow.events
+    import typing
     import metaflow
+    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,27 +238,14 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger, or @trigger_on_finish decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
-    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -317,11 +304,24 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
+    @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
     ...
 
 current: Current
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/mflog/mflog.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/mflog/mflog.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.395448                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.008685                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/multicore_utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/multicore_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.341879                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.956222                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/parameters.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/parameters.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.343263                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.957659                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
     import metaflow.exception
-    import metaflow._vendor.click.types
     import metaflow.parameters
+    import metaflow._vendor.click.types
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
 
 class ParameterFieldTypeMismatch(metaflow.exception.MetaflowException, metaclass=type):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.354165                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.968728                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.unbounded_foreach
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.unbounded_foreach
 
 CLIS_DESC: list
 
 class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
     def __init__(self, iterable):
         ...
     def __iter__(self):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.431426                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.034343                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow._vendor.click.types
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.432695                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.035535                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.429042                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.031906                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.428462                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.031444                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/exception.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.429316                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.032182                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.429595                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.032453                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.449908                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.062186                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.450393                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.062665                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.450822                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.063109                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow.decorators
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.397702                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.037738                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_events.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.395956                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.036014                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.403218                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.043275                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow._vendor.click.types
+    import metaflow.metaflow_current
     import metaflow.parameters
+    import metaflow._vendor.click.types
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.405233                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.045224                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
+    import metaflow.metaflow_current
     import metaflow.parameters
+    import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.396994                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.036966                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.events
     import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.events
     import metaflow
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/aws_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.411116                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.009718                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/aws_utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.410491                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.009459                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.440468                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.058308                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.442134                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.059917                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.439036                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.056893                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.441412                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.059210                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.448436                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.060403                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import abc
     import metaflow.plugins.secrets
+    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.443417                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.050865                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/production_token.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.436675                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.050519                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def new_token(token_prefix, prev_token = None):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.443075                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.992178                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.446238                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.053794                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.447904                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.055379                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
-    import metaflow.decorators
+    import metaflow.metaflow_current
     import metaflow.parameters
+    import metaflow.decorators
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.443789                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.051240                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.442878                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.050055                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_credential.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_credential.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.434374                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.045958                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class AzureDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.434641                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.046234                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/azure_utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.435156                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.046748                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.435575                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.047160                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/azure/includefile_support.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.388088                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.001988                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.426055                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.021198                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import typing
-    import metaflow.exception
     import metaflow.client.core
-    import datetime
     import metaflow.parameters
+    import datetime
+    import metaflow.exception
+    import typing
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.390542                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.003898                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_client
     import metaflow.exception
+    import metaflow.plugins.cards.card_client
     import metaflow
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_creator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.420781                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.015845                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_datastore.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.422647                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.017729                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.421691                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.016737                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.417902                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.004418                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
 
+TYPE_CHECKING: bool
+
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
         
@@ -54,14 +56,7 @@
     def render(self):
         """
         `render` returns a string or dictionary. This class can be called on the client side to dynamically add components to the `MetaflowCard`
         """
         ...
     ...
 
-EXT_PKG: str
-
-def iter_namespace(ns_pkg):
-    ...
-
-MF_EXTERNAL_CARDS: list
-
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.382461                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.996941                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.391077                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.013091                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
 
-TYPE_CHECKING: bool
-
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
         
@@ -56,7 +54,14 @@
     def render(self):
         """
         `render` returns a string or dictionary. This class can be called on the client side to dynamically add components to the `MetaflowCard`
         """
         ...
     ...
 
+EXT_PKG: str
+
+def iter_namespace(ns_pkg):
+    ...
+
+MF_EXTERNAL_CARDS: list
+
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.449263                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.061217                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.452225                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.064491                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.451758                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.064043                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.451293                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.063586                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.393496                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.006778                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
-    import typing
     import metaflow.plugins.cards.card_modules.card
+    import typing
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.436022                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.048995                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.436248                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.049253                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.383907                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.998424                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.card
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/card_resolver.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.423262                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.018338                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/component_serializer.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.420468                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.015546                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
-    import metaflow.exception
     import metaflow.plugins.cards.card_modules.card
+    import metaflow.exception
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
     @component_id.setter
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/cards/exception.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.418620                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.013838                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/catch_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.377667                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.990715                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.376155                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.989923                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import io
     import metaflow.plugins.datatools.s3.s3
+    import io
 
 def read_in_chunks(dst, src, src_sz, max_chunk_size):
     ...
 
 class MetaflowLocalNotFound(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/local.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.387343                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.001414                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.417288                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.012493                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import io
     import metaflow.plugins.datatools.s3.s3
+    import io
 
 class RangeInfo(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, total_size: int, request_offset: int = 0, request_length: int = -1):
         """
         Create new instance of RangeInfo(total_size, request_offset, request_length)
         """
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.358294                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.973739                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
+    import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
     import typing
-    import io
     import metaflow.exception
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow.datastore.inputs
+    import metaflow.metaflow_current
+    import io
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.448876                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.060817                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.386501                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.000722                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/debug_logger.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.379632                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.994425                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.event_logger
+    import metaflow.monitor
 
-class DebugEventLogger(metaflow.event_logger.NullEventLogger, metaclass=type):
+class DebugMonitor(metaflow.monitor.NullMonitor, metaclass=type):
     @classmethod
     def get_worker(cls):
         ...
     ...
 
-class DebugEventLoggerSidecar(object, metaclass=type):
+class DebugMonitorSidecar(object, metaclass=type):
     def __init__(self):
         ...
     def process_message(self, msg):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/environment_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.372898                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.987724                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/events_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.378206                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.993116                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.411724                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.045698                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.plugins.parallel_decorator
     import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.plugins.parallel_decorator
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gcp_secret_manager_secrets_provider.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.434134                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.048553                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import abc
     import metaflow.plugins.secrets
+    import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.433246                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.047671                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.433021                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.047451                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class GcpDefaultClientProvider(object, metaclass=type):
     @staticmethod
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.433603                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.048031                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.388968                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.002562                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.407892                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.025008                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.410062                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.027175                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import metaflow._vendor.click.types
     import metaflow.decorators
+    import metaflow._vendor.click.types
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
     def __repr__(self):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.406749                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.023864                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.409078                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.026184                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.exception
     import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.406136                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.023249                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/parallel_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.374414                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.991992                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/project_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.378608                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.992693                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.374660                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.991333                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.412422                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.028134                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.414092                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.029681                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
-    import io
     import metaflow.metaflow_environment
+    import io
     import abc
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.412716                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.027468                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.414600                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.030186                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.pypi.conda_environment
     import metaflow.metaflow_environment
+    import metaflow.plugins.pypi.conda_environment
 
 class CondaEnvironment(metaflow.metaflow_environment.MetaflowEnvironment, metaclass=type):
     def __init__(self, flow):
         ...
     def set_local_root(self, local_root):
         ...
     def decospecs(self):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/pypi/utils.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.413088                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.028509                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/resources_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.373291                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.987419                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/retry_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.376535                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.984113                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
 
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
         ...
-    def step_task_retry_count(self):
+    def run(self, logger = None, warnings = False, pylint_config = []):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/__init__.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.376927                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.990973                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.427152                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.022371                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import abc
     import metaflow.plugins.secrets
+    import abc
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.426862                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.022030                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/tag_cli.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.385640                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:01.000114                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
-    import metaflow.exception
-    import metaflow.events
     import metaflow.client.core
+    import metaflow.events
     import datetime
+    import metaflow.exception
+    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.372700                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.987273                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.unbounded_foreach
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/plugins/timeout_decorator.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.373749                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.988298                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/procpoll.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/procpoll.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.369145                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.983759                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/pylint_wrapper.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.369500                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.993693                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class PyLint(object, metaclass=type):
-    def __init__(self, fname):
+class StorageExecutor(object, metaclass=type):
+    def __init__(self, use_processes = False):
         ...
-    def has_pylint(self):
+    def warm_up(self):
         ...
-    def run(self, logger = None, warnings = False, pylint_config = []):
+    def submit(self, *args, **kwargs):
         ...
     ...
 
+def handle_executor_exceptions(func):
+    """
+    Decorator for handling errors that come from an Executor. This decorator should
+    only be used on functions where executor errors are possible. I.e. the function
+    uses StorageExecutor.
+    """
+    ...
+
```

### Comparing `ob-metaflow-stubs-2.11.8.1/metaflow-stubs/tagging_util.pyi` & `ob-metaflow-stubs-2.11.9.1/metaflow-stubs/tagging_util.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8.1                                                           #
-# Generated on 2024-03-29T12:39:58.343659                                        #
+# MF version: 2.11.9.1                                                           #
+# Generated on 2024-03-30T09:14:00.958044                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/PKG-INFO` & `ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ob-metaflow-stubs
-Version: 2.11.8.1
+Version: 2.11.9.1
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: ob-metaflow==2.11.8.1
+Requires-Dist: ob-metaflow==2.11.9.1
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `ob-metaflow-stubs-2.11.8.1/ob_metaflow_stubs.egg-info/SOURCES.txt` & `ob-metaflow-stubs-2.11.9.1/ob_metaflow_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-stubs-2.11.8.1/setup.py` & `ob-metaflow-stubs-2.11.9.1/setup.py`

 * *Files identical despite different names*

