# Comparing `tmp/trainml-0.5.5.tar.gz` & `tmp/trainml-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainml-0.5.5.tar", last modified: Tue Apr  2 13:15:54 2024, max compression
+gzip compressed data, was "trainml-0.5.6.tar", last modified: Fri Apr 12 19:06:16 2024, max compression
```

## Comparing `trainml-0.5.5.tar` & `trainml-0.5.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.186591 trainml-0.5.5/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.5/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-02 13:15:54.186436 trainml-0.5.5/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.5/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.164142 trainml-0.5.5/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.5/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.5/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.5/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.5/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1000 2024-02-29 19:07:44.000000 trainml-0.5.5/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-02 13:15:54.186637 trainml-0.5.5/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.5/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.162157 trainml-0.5.5/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.166468 trainml-0.5.5/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.5/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.166835 trainml-0.5.5/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.5/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.5/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.5/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.5/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.5/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.5/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.5/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-03-19 18:51:28.000000 trainml-0.5.5/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.5/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.5/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.5/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.170410 trainml-0.5.5/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.5/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.172501 trainml-0.5.5/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.5/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.173898 trainml-0.5.5/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.5/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-06-22 02:20:03.000000 trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.5/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.5/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.5/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.5/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.5/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.5/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2023-06-22 01:48:21.000000 trainml-0.5.5/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.5/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.175686 trainml-0.5.5/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.5/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.5/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.5/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.5/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.5/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.5/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2023-06-23 16:54:00.000000 trainml-0.5.5/tests/unit/cloudbender/test_reservations_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31197 2024-03-12 15:29:40.000000 trainml-0.5.5/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.5/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.5/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.5/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.5/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.5/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.5/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.5/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.5/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.5/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2023-06-22 01:37:38.000000 trainml-0.5.5/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.5/tests/unit/test_trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.5/tests/unit/test_volumes_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.179251 trainml-0.5.5/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-02 13:13:59.000000 trainml-0.5.5/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.5/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.5/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2023-09-08 19:04:34.000000 trainml-0.5.5/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.181962 trainml-0.5.5/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.5/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.5/trainml/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.183442 trainml-0.5.5/trainml/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      534 2023-06-23 19:38:26.000000 trainml-0.5.5/trainml/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.5/trainml/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.5/trainml/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.5/trainml/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.5/trainml/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.5/trainml/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2023-06-22 02:14:39.000000 trainml-0.5.5/trainml/cli/cloudbender/reservation.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.5/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.5/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.5/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.5/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.183921 trainml-0.5.5/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.5/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.5/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.5/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2023-06-21 21:09:43.000000 trainml-0.5.5/trainml/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.5/trainml/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.186145 trainml-0.5.5/trainml/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.5/trainml/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      634 2023-06-23 15:52:00.000000 trainml-0.5.5/trainml/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.5/trainml/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.5/trainml/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.5/trainml/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.5/trainml/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.5/trainml/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.5/trainml/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2023-06-23 16:23:17.000000 trainml-0.5.5/trainml/cloudbender/reservations.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.5/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-01-23 15:13:39.000000 trainml-0.5.5/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.5/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.5/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.5/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-03-11 15:18:02.000000 trainml-0.5.5/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2023-09-08 19:05:25.000000 trainml-0.5.5/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2023-06-21 21:05:20.000000 trainml-0.5.5/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.5/trainml/trainml.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-03-12 13:04:15.000000 trainml-0.5.5/trainml/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:15:54.180047 trainml-0.5.5/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3502 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-02 13:15:54.000000 trainml-0.5.5/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.612984 trainml-0.5.6/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.6/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-12 19:06:16.612820 trainml-0.5.6/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.6/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.586161 trainml-0.5.6/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.6/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.6/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.6/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.6/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      992 2024-04-09 21:22:14.000000 trainml-0.5.6/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-12 19:06:16.613032 trainml-0.5.6/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.6/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.584323 trainml-0.5.6/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.588516 trainml-0.5.6/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.6/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.589038 trainml-0.5.6/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.6/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.6/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.6/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-03-14 16:09:32.000000 trainml-0.5.6/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-03-19 18:31:45.000000 trainml-0.5.6/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.6/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.6/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-03-19 18:51:28.000000 trainml-0.5.6/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-03-14 16:09:23.000000 trainml-0.5.6/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-02-29 23:09:06.000000 trainml-0.5.6/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:07:27.000000 trainml-0.5.6/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.593091 trainml-0.5.6/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.6/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.595707 trainml-0.5.6/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.6/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.597503 trainml-0.5.6/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.6/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2023-06-23 19:47:44.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-09 16:44:31.000000 trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.6/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.6/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.6/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.6/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.6/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.6/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-09 16:44:25.000000 trainml-0.5.6/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-03-12 15:29:44.000000 trainml-0.5.6/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.599677 trainml-0.5.6/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.6/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2023-06-23 16:49:35.000000 trainml-0.5.6/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2023-06-23 16:50:27.000000 trainml-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2023-06-23 19:46:10.000000 trainml-0.5.6/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2023-06-23 16:51:45.000000 trainml-0.5.6/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2023-06-23 16:52:25.000000 trainml-0.5.6/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2023-06-23 16:53:15.000000 trainml-0.5.6/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5043 2024-04-09 21:24:58.000000 trainml-0.5.6/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-09 16:44:31.000000 trainml-0.5.6/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2023-07-27 15:10:38.000000 trainml-0.5.6/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.6/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.6/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.6/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.6/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.6/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.6/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.6/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.6/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9238 2024-04-09 16:44:31.000000 trainml-0.5.6/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.6/tests/unit/test_trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-03-12 17:51:37.000000 trainml-0.5.6/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.604349 trainml-0.5.6/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-12 17:03:22.000000 trainml-0.5.6/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.6/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2023-09-08 15:42:01.000000 trainml-0.5.6/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2023-09-08 19:04:34.000000 trainml-0.5.6/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.607221 trainml-0.5.6/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-02-29 19:03:52.000000 trainml-0.5.6/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.6/trainml/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.609066 trainml-0.5.6/trainml/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      526 2024-04-09 16:40:15.000000 trainml-0.5.6/trainml/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.6/trainml/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2023-06-25 18:44:34.000000 trainml-0.5.6/trainml/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.6/trainml/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.6/trainml/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.6/trainml/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2869 2024-04-10 15:40:55.000000 trainml-0.5.6/trainml/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.6/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-02-08 17:04:38.000000 trainml-0.5.6/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.6/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.6/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.609608 trainml-0.5.6/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.6/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-02-14 15:58:34.000000 trainml-0.5.6/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2023-09-08 19:00:58.000000 trainml-0.5.6/trainml/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-09 16:42:40.000000 trainml-0.5.6/trainml/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-03-12 17:50:39.000000 trainml-0.5.6/trainml/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.612468 trainml-0.5.6/trainml/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.6/trainml/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      618 2024-04-09 16:39:20.000000 trainml-0.5.6/trainml/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2023-06-23 16:22:15.000000 trainml-0.5.6/trainml/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2023-06-23 16:22:25.000000 trainml-0.5.6/trainml/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2023-06-23 16:28:32.000000 trainml-0.5.6/trainml/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2023-06-23 16:25:10.000000 trainml-0.5.6/trainml/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2023-06-23 16:22:51.000000 trainml-0.5.6/trainml/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2023-06-23 16:23:07.000000 trainml-0.5.6/trainml/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3222 2024-04-09 16:43:41.000000 trainml-0.5.6/trainml/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-09-08 19:03:44.000000 trainml-0.5.6/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-01-23 15:13:39.000000 trainml-0.5.6/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.6/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-02-29 19:05:24.000000 trainml-0.5.6/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2023-06-23 15:24:57.000000 trainml-0.5.6/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-03-11 15:18:02.000000 trainml-0.5.6/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2023-09-08 19:05:25.000000 trainml-0.5.6/trainml/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5001 2024-04-09 16:45:06.000000 trainml-0.5.6/trainml/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-02-29 19:06:10.000000 trainml-0.5.6/trainml/trainml.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-03-12 13:04:15.000000 trainml-0.5.6/trainml/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:16.605243 trainml-0.5.6/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3490 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-12 19:06:16.000000 trainml-0.5.6/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.5.5/LICENSE` & `trainml-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/PKG-INFO` & `trainml-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.5
+Version: 0.5.6
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.5 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.6 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.5/README.md` & `trainml-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/examples/create_dataset_and_training_job.py` & `trainml-0.5.6/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/examples/local_storage.py` & `trainml-0.5.6/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/examples/training_inference_pipeline.py` & `trainml-0.5.6/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/pyproject.toml` & `trainml-0.5.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     "projects: Projects tests",
     "cloudbender: CloudBender tests",
     "providers: Providers tests",
     "regions: Regions tests",
     "nodes: Nodes tests",
     "devices: Devices tests",
     "datastores: Datastores tests",
-    "reservations: Reservations tests",
+    "services: Services tests",
     "device_configs: DeviceConfigs tests",
     "unit: All unit tests (no trainML environment required)",
     "integration: All integration tests (trainML environment required)",
     "sdk: All tests of the SDK",
     "cli: All test of the cli",
 ]
```

### Comparing `trainml-0.5.5/setup.py` & `trainml-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/cloudbender/test_providers_integration.py` & `trainml-0.5.6/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/conftest.py` & `trainml-0.5.6/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_checkpoints_integration.py` & `trainml-0.5.6/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_datasets_integration.py` & `trainml-0.5.6/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_environments_integration.py` & `trainml-0.5.6/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_gpu_types_integration.py` & `trainml-0.5.6/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_jobs_integration.py` & `trainml-0.5.6/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_models_integration.py` & `trainml-0.5.6/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_projects_integration.py` & `trainml-0.5.6/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/integration/test_volumes_integration.py` & `trainml-0.5.6/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `trainml-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_datasets_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_gpu_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_job_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_model_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_project_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_project_unit.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,24 @@
         assert result.exit_code == 0
         mock_trainml.projects.list.assert_called_once()
 
 
 def test_list_datastores(runner, mock_project_datastores):
     with patch("trainml.cli.TrainML", new=AsyncMock) as mock_trainml:
         mock_project = create_autospec(Project)
-        mock_project.list_datastores = AsyncMock(
-            return_value=mock_project_datastores
-        )
+        mock_project.list_datastores = AsyncMock(return_value=mock_project_datastores)
         mock_trainml.projects.get = AsyncMock(return_value=mock_project)
         result = runner.invoke(specimen, ["list-datastores"])
         print(result)
         assert result.exit_code == 0
         mock_project.list_datastores.assert_called_once()
 
 
-def test_list_reservations(runner, mock_project_reservations):
+def test_list_services(runner, mock_project_services):
     with patch("trainml.cli.TrainML", new=AsyncMock) as mock_trainml:
         mock_project = create_autospec(Project)
-        mock_project.list_reservations = AsyncMock(
-            return_value=mock_project_reservations
-        )
+        mock_project.list_services = AsyncMock(return_value=mock_project_services)
         mock_trainml.projects.get = AsyncMock(return_value=mock_project)
-        result = runner.invoke(specimen, ["list-reservations"])
+        result = runner.invoke(specimen, ["list-services"])
         print(result)
         assert result.exit_code == 0
-        mock_project.list_reservations.assert_called_once()
+        mock_project.list_services.assert_called_once()
```

### Comparing `trainml-0.5.5/tests/unit/cli/test_cli_volume_unit.py` & `trainml-0.5.6/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_datastores_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_devices_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_nodes_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_providers_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_regions_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/cloudbender/test_reservations_unit.py` & `trainml-0.5.6/tests/unit/cloudbender/test_services_unit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,161 @@
 import re
 import json
 import logging
 from unittest.mock import AsyncMock, patch
 from pytest import mark, fixture, raises
 from aiohttp import WSMessage, WSMsgType
 
-import trainml.cloudbender.reservations as specimen
+import trainml.cloudbender.services as specimen
 from trainml.exceptions import (
     ApiError,
     SpecificationError,
     TrainMLException,
 )
 
-pytestmark = [mark.sdk, mark.unit, mark.cloudbender, mark.reservations]
+pytestmark = [mark.sdk, mark.unit, mark.cloudbender, mark.services]
 
 
 @fixture
-def reservations(mock_trainml):
-    yield specimen.Reservations(mock_trainml)
+def services(mock_trainml):
+    yield specimen.Services(mock_trainml)
 
 
 @fixture
-def reservation(mock_trainml):
-    yield specimen.Reservation(
+def service(mock_trainml):
+    yield specimen.Service(
         mock_trainml,
         provider_uuid="1",
         region_uuid="a",
-        reservation_id="x",
-        name="On-Prem Reservation",
-        type="port",
-        resource="8001",
-        hostname="service.local",
+        service_id="x",
+        name="On-Prem Service",
+        public=False,
+        hostname="app1.proximl.cloud",
     )
 
 
 class RegionsTests:
     @mark.asyncio
-    async def test_get_reservation(
+    async def test_get_service(
         self,
-        reservations,
+        services,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
-        await reservations.get("1234", "5687", "91011")
+        await services.get("1234", "5687", "91011")
         mock_trainml._query.assert_called_once_with(
-            "/provider/1234/region/5687/reservation/91011", "GET", {}
+            "/provider/1234/region/5687/service/91011", "GET", {}
         )
 
     @mark.asyncio
-    async def test_list_reservations(
+    async def test_list_services(
         self,
-        reservations,
+        services,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
-        await reservations.list("1234", "5687")
+        await services.list("1234", "5687")
         mock_trainml._query.assert_called_once_with(
-            "/provider/1234/region/5687/reservation", "GET", {}
+            "/provider/1234/region/5687/service", "GET", {}
         )
 
     @mark.asyncio
-    async def test_remove_reservation(
+    async def test_remove_service(
         self,
-        reservations,
+        services,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
-        await reservations.remove("1234", "4567", "8910")
+        await services.remove("1234", "4567", "8910")
         mock_trainml._query.assert_called_once_with(
-            "/provider/1234/region/4567/reservation/8910", "DELETE", {}
+            "/provider/1234/region/4567/service/8910", "DELETE", {}
         )
 
     @mark.asyncio
-    async def test_create_reservation(self, reservations, mock_trainml):
+    async def test_create_service(self, services, mock_trainml):
         requested_config = dict(
             provider_uuid="provider-id-1",
             region_uuid="region-id-1",
-            name="On-Prem Reservation",
-            type="port",
-            resource="8001",
-            hostname="service.local",
+            name="On-Prem Service",
+            public=False,
         )
         expected_payload = dict(
-            name="On-Prem Reservation",
-            type="port",
-            resource="8001",
-            hostname="service.local",
+            name="On-Prem Service",
+            public=False,
         )
         api_response = {
             "provider_uuid": "provider-id-1",
             "region_uuid": "region-id-1",
-            "reservation_id": "reservation-id-1",
-            "name": "On-Prem Reservation",
-            "type": "port",
-            "resource": "8001",
-            "hostname": "service.local",
+            "service_id": "service-id-1",
+            "name": "On-Prem Service",
+            "public": False,
+            "hostname": "app1.proximl.cloud",
             "createdAt": "2020-12-31T23:59:59.000Z",
         }
 
         mock_trainml._query = AsyncMock(return_value=api_response)
-        response = await reservations.create(**requested_config)
+        response = await services.create(**requested_config)
         mock_trainml._query.assert_called_once_with(
-            "/provider/provider-id-1/region/region-id-1/reservation",
+            "/provider/provider-id-1/region/region-id-1/service",
             "POST",
             None,
             expected_payload,
         )
-        assert response.id == "reservation-id-1"
+        assert response.id == "service-id-1"
 
 
-class reservationTests:
-    def test_reservation_properties(self, reservation):
-        assert isinstance(reservation.id, str)
-        assert isinstance(reservation.provider_uuid, str)
-        assert isinstance(reservation.region_uuid, str)
-        assert isinstance(reservation.type, str)
-        assert isinstance(reservation.name, str)
-        assert isinstance(reservation.resource, str)
-        assert isinstance(reservation.hostname, str)
-
-    def test_reservation_str(self, reservation):
-        string = str(reservation)
-        regex = r"^{.*\"reservation_id\": \"" + reservation.id + r"\".*}$"
+class serviceTests:
+    def test_service_properties(self, service):
+        assert isinstance(service.id, str)
+        assert isinstance(service.provider_uuid, str)
+        assert isinstance(service.region_uuid, str)
+        assert isinstance(service.public, bool)
+        assert isinstance(service.name, str)
+        assert isinstance(service.hostname, str)
+
+    def test_service_str(self, service):
+        string = str(service)
+        regex = r"^{.*\"service_id\": \"" + service.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_reservation_repr(self, reservation):
-        string = repr(reservation)
-        regex = (
-            r"^Reservation\( trainml , \*\*{.*'reservation_id': '"
-            + reservation.id
-            + r"'.*}\)$"
-        )
+    def test_service_repr(self, service):
+        string = repr(service)
+        regex = r"^Service\( trainml , \*\*{.*'service_id': '" + service.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_reservation_bool(self, reservation, mock_trainml):
-        empty_reservation = specimen.Reservation(mock_trainml)
-        assert bool(reservation)
-        assert not bool(empty_reservation)
+    def test_service_bool(self, service, mock_trainml):
+        empty_service = specimen.Service(mock_trainml)
+        assert bool(service)
+        assert not bool(empty_service)
 
     @mark.asyncio
-    async def test_reservation_remove(self, reservation, mock_trainml):
+    async def test_service_remove(self, service, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
-        await reservation.remove()
+        await service.remove()
         mock_trainml._query.assert_called_once_with(
-            "/provider/1/region/a/reservation/x", "DELETE"
+            "/provider/1/region/a/service/x", "DELETE"
         )
 
     @mark.asyncio
-    async def test_reservation_refresh(self, reservation, mock_trainml):
+    async def test_service_refresh(self, service, mock_trainml):
         api_response = {
             "provider_uuid": "provider-id-1",
             "region_uuid": "region-id-1",
-            "reservation_id": "reservation-id-1",
-            "name": "On-Prem Reservation",
-            "type": "port",
-            "resource": "8001",
-            "hostname": "service.local",
+            "service_id": "service-id-1",
+            "name": "On-Prem Service",
+            "public": False,
+            "hostname": "app1.proximl.cloud",
             "createdAt": "2020-12-31T23:59:59.000Z",
         }
         mock_trainml._query = AsyncMock(return_value=api_response)
-        response = await reservation.refresh()
+        response = await service.refresh()
         mock_trainml._query.assert_called_once_with(
-            f"/provider/1/region/a/reservation/x", "GET"
+            f"/provider/1/region/a/service/x", "GET"
         )
-        assert reservation.id == "reservation-id-1"
-        assert response.id == "reservation-id-1"
+        assert service.id == "service-id-1"
+        assert response.id == "service-id-1"
```

### Comparing `trainml-0.5.5/tests/unit/conftest.py` & `trainml-0.5.6/tests/unit/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from trainml.environments import Environment, Environments
 from trainml.jobs import Job, Jobs
 from trainml.connections import Connections
 from trainml.projects import (
     Projects,
     Project,
     ProjectDatastore,
-    ProjectReservation,
+    ProjectService,
 )
 from trainml.cloudbender import Cloudbender
 from trainml.cloudbender.providers import Provider, Providers
 from trainml.cloudbender.regions import Region, Regions
 from trainml.cloudbender.nodes import Node, Nodes
 from trainml.cloudbender.devices import Device, Devices
 from trainml.cloudbender.datastores import Datastore, Datastores
-from trainml.cloudbender.reservations import Reservation, Reservations
+from trainml.cloudbender.services import Service, Services
 from trainml.cloudbender.device_configs import DeviceConfig, DeviceConfigs
 
 
 pytestmark = mark.unit
 
 
 @fixture(scope="session")
@@ -883,61 +883,61 @@
                 "name": "GCP Samba",
             },
         ),
     ]
 
 
 @fixture(scope="session")
-def mock_reservations():
+def mock_services():
     trainml = Mock()
     yield [
-        Reservation(
+        Service(
             trainml,
             **{
                 "provider_uuid": "prov-id-1",
                 "region_uuid": "reg-id-1",
-                "reservation_id": "res-id-1",
+                "service_id": "res-id-1",
                 "type": "port",
                 "name": "On-Prem Service A",
                 "resource": "8001",
                 "hostname": "service-a.local",
             },
         ),
-        Reservation(
+        Service(
             trainml,
             **{
                 "provider_uuid": "prov-id-2",
                 "region_uuid": "reg-id-2",
-                "reservation_id": "res-id-2",
+                "service_id": "res-id-2",
                 "type": "port",
                 "name": "Cloud Service B",
                 "resource": "8001",
                 "hostname": "service-b.local",
             },
         ),
     ]
 
 
 @fixture(scope="session")
-def mock_project_reservations():
+def mock_project_services():
     trainml = Mock()
     yield [
-        ProjectReservation(
+        ProjectService(
             trainml,
             **{
                 "project_uuid": "proj-id-1",
                 "region_uuid": "reg-id-1",
                 "id": "res-id-1",
                 "type": "port",
                 "name": "On-Prem Service A",
                 "resource": "8001",
                 "hostname": "service-a.local",
             },
         ),
-        ProjectReservation(
+        ProjectService(
             trainml,
             **{
                 "project_uuid": "proj-id-1",
                 "region_uuid": "reg-id-2",
                 "id": "res-id-2",
                 "type": "port",
                 "name": "Cloud Service B",
@@ -986,15 +986,15 @@
     mock_jobs,
     mock_projects,
     mock_providers,
     mock_regions,
     mock_nodes,
     mock_devices,
     mock_datastores,
-    mock_reservations,
+    mock_services,
     mock_device_configs,
 ):
     trainml = create_autospec(TrainML)
     trainml.active_project = "proj-id-1"
     trainml.project = "proj-id-1"
     trainml.datasets = create_autospec(Datasets)
     trainml.checkpoints = create_autospec(Checkpoints)
@@ -1024,14 +1024,14 @@
     trainml.cloudbender.regions.list = AsyncMock(return_value=mock_regions)
     trainml.cloudbender.nodes = create_autospec(Nodes)
     trainml.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     trainml.cloudbender.devices = create_autospec(Nodes)
     trainml.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     trainml.cloudbender.datastores = create_autospec(Datastores)
     trainml.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
-    trainml.cloudbender.reservations = create_autospec(Reservations)
-    trainml.cloudbender.reservations.list = AsyncMock(return_value=mock_reservations)
+    trainml.cloudbender.services = create_autospec(Services)
+    trainml.cloudbender.services.list = AsyncMock(return_value=mock_services)
     trainml.cloudbender.device_configs = create_autospec(DeviceConfigs)
     trainml.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield trainml
```

### Comparing `trainml-0.5.5/tests/unit/test_auth.py` & `trainml-0.5.6/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_checkpoints_unit.py` & `trainml-0.5.6/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_connections_unit.py` & `trainml-0.5.6/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_datasets_unit.py` & `trainml-0.5.6/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_environments_unit.py` & `trainml-0.5.6/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_exceptions.py` & `trainml-0.5.6/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_gpu_types_unit.py` & `trainml-0.5.6/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_jobs_unit.py` & `trainml-0.5.6/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_models_unit.py` & `trainml-0.5.6/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_projects_unit.py` & `trainml-0.5.6/tests/unit/test_projects_unit.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         project_uuid="proj-id-1",
         type="nfs",
         region_uuid="reg-id-1",
     )
 
 
 @fixture
-def project_reservation(mock_trainml):
-    yield specimen.ProjectReservation(
+def project_service(mock_trainml):
+    yield specimen.ProjectService(
         mock_trainml,
         id="res-id-1",
-        name="reservation 1",
+        name="service 1",
         project_uuid="proj-id-1",
         region_uuid="reg-id-1",
         type="port",
         resource="8001",
         hostname="service.local",
     )
 
@@ -68,17 +68,15 @@
         self,
         projects,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await projects.get("1234")
-        mock_trainml._query.assert_called_once_with(
-            "/project/1234", "GET", dict()
-        )
+        mock_trainml._query.assert_called_once_with("/project/1234", "GET", dict())
 
     @mark.asyncio
     async def test_list_projects(
         self,
         projects,
         mock_trainml,
     ):
@@ -92,17 +90,15 @@
         self,
         projects,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await projects.remove("4567")
-        mock_trainml._query.assert_called_once_with(
-            "/project/4567", "DELETE", dict()
-        )
+        mock_trainml._query.assert_called_once_with("/project/4567", "DELETE", dict())
 
     @mark.asyncio
     async def test_create_project_simple(self, projects, mock_trainml):
         requested_config = dict(
             name="new project",
         )
         expected_payload = dict(name="new project", copy_keys=False)
@@ -152,44 +148,44 @@
 
     def test_project_datastore_bool(self, project_datastore, mock_trainml):
         empty_project_datastore = specimen.ProjectDatastore(mock_trainml)
         assert bool(project_datastore)
         assert not bool(empty_project_datastore)
 
 
-class ProjectReservationTests:
-    def test_project_reservation_properties(self, project_reservation):
-        assert isinstance(project_reservation.id, str)
-        assert isinstance(project_reservation.name, str)
-        assert isinstance(project_reservation.project_uuid, str)
-        assert isinstance(project_reservation.type, str)
-        assert isinstance(project_reservation.hostname, str)
-        assert isinstance(project_reservation.resource, str)
-        assert isinstance(project_reservation.region_uuid, str)
-
-    def test_project_reservation_str(self, project_reservation):
-        string = str(project_reservation)
-        regex = r"^{.*\"id\": \"" + project_reservation.id + r"\".*}$"
+class ProjectServiceTests:
+    def test_project_service_properties(self, project_service):
+        assert isinstance(project_service.id, str)
+        assert isinstance(project_service.name, str)
+        assert isinstance(project_service.project_uuid, str)
+        assert isinstance(project_service.type, str)
+        assert isinstance(project_service.hostname, str)
+        assert isinstance(project_service.resource, str)
+        assert isinstance(project_service.region_uuid, str)
+
+    def test_project_service_str(self, project_service):
+        string = str(project_service)
+        regex = r"^{.*\"id\": \"" + project_service.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_project_reservation_repr(self, project_reservation):
-        string = repr(project_reservation)
+    def test_project_service_repr(self, project_service):
+        string = repr(project_service)
         regex = (
-            r"^ProjectReservation\( trainml , \*\*{.*'id': '"
-            + project_reservation.id
+            r"^ProjectService\( trainml , \*\*{.*'id': '"
+            + project_service.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_project_reservation_bool(self, project_reservation, mock_trainml):
-        empty_project_reservation = specimen.ProjectReservation(mock_trainml)
-        assert bool(project_reservation)
-        assert not bool(empty_project_reservation)
+    def test_project_service_bool(self, project_service, mock_trainml):
+        empty_project_service = specimen.ProjectService(mock_trainml)
+        assert bool(project_service)
+        assert not bool(empty_project_service)
 
 
 class ProjectTests:
     def test_project_properties(self, project):
         assert isinstance(project.id, str)
         assert isinstance(project.name, str)
         assert isinstance(project.owner_name, str)
@@ -199,17 +195,15 @@
         string = str(project)
         regex = r"^{.*\"id\": \"" + project.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     def test_project_repr(self, project):
         string = repr(project)
-        regex = (
-            r"^Project\( trainml , \*\*{.*'id': '" + project.id + r"'.*}\)$"
-        )
+        regex = r"^Project\( trainml , \*\*{.*'id': '" + project.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     def test_project_bool(self, project, mock_trainml):
         empty_project = specimen.Project(mock_trainml)
         assert bool(project)
         assert not bool(empty_project)
@@ -222,26 +216,22 @@
         mock_trainml._query.assert_called_once_with("/project/1", "DELETE")
 
     @mark.asyncio
     async def test_project_refresh_datastores(self, project, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await project.refresh_datastores()
-        mock_trainml._query.assert_called_once_with(
-            "/project/1/datastores", "PATCH"
-        )
+        mock_trainml._query.assert_called_once_with("/project/1/datastores", "PATCH")
 
     @mark.asyncio
-    async def test_project_refresh_reservations(self, project, mock_trainml):
+    async def test_project_refresh_services(self, project, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
-        await project.refresh_reservations()
-        mock_trainml._query.assert_called_once_with(
-            "/project/1/reservations", "PATCH"
-        )
+        await project.refresh_services()
+        mock_trainml._query.assert_called_once_with("/project/1/services", "PATCH")
 
     @mark.asyncio
     async def test_project_list_datastores(self, project, mock_trainml):
         api_response = [
             {
                 "project_uuid": "proj-id-1",
                 "region_uuid": "reg-id-1",
@@ -255,21 +245,19 @@
                 "id": "store-id-2",
                 "type": "smb",
                 "name": "GCP Samba",
             },
         ]
         mock_trainml._query = AsyncMock(return_value=api_response)
         resp = await project.list_datastores()
-        mock_trainml._query.assert_called_once_with(
-            "/project/1/datastores", "GET"
-        )
+        mock_trainml._query.assert_called_once_with("/project/1/datastores", "GET")
         assert len(resp) == 2
 
     @mark.asyncio
-    async def test_project_list_reservations(self, project, mock_trainml):
+    async def test_project_list_services(self, project, mock_trainml):
         api_response = [
             {
                 "project_uuid": "proj-id-1",
                 "region_uuid": "reg-id-1",
                 "id": "res-id-1",
                 "type": "port",
                 "name": "On-Prem Service A",
@@ -283,12 +271,10 @@
                 "type": "port",
                 "name": "Cloud Service B",
                 "resource": "8001",
                 "hostname": "service-b.local",
             },
         ]
         mock_trainml._query = AsyncMock(return_value=api_response)
-        resp = await project.list_reservations()
-        mock_trainml._query.assert_called_once_with(
-            "/project/1/reservations", "GET"
-        )
+        resp = await project.list_services()
+        mock_trainml._query.assert_called_once_with("/project/1/services", "GET")
         assert len(resp) == 2
```

### Comparing `trainml-0.5.5/tests/unit/test_trainml.py` & `trainml-0.5.6/tests/unit/test_trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/tests/unit/test_volumes_unit.py` & `trainml-0.5.6/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/auth.py` & `trainml-0.5.6/trainml/auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/checkpoints.py` & `trainml-0.5.6/trainml/checkpoints.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/__init__.py` & `trainml-0.5.6/trainml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/checkpoint.py` & `trainml-0.5.6/trainml/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/__init__.py` & `trainml-0.5.6/trainml/cli/cloudbender/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 
 from trainml.cli.cloudbender.provider import provider
 from trainml.cli.cloudbender.region import region
 from trainml.cli.cloudbender.node import node
 from trainml.cli.cloudbender.device import device
 from trainml.cli.cloudbender.datastore import datastore
-from trainml.cli.cloudbender.reservation import reservation
+from trainml.cli.cloudbender.service import service
```

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/datastore.py` & `trainml-0.5.6/trainml/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/device.py` & `trainml-0.5.6/trainml/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/node.py` & `trainml-0.5.6/trainml/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/provider.py` & `trainml-0.5.6/trainml/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/cloudbender/region.py` & `trainml-0.5.6/trainml/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/connection.py` & `trainml-0.5.6/trainml/cli/connection.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/dataset.py` & `trainml-0.5.6/trainml/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/environment.py` & `trainml-0.5.6/trainml/cli/environment.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/gpu.py` & `trainml-0.5.6/trainml/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/job/__init__.py` & `trainml-0.5.6/trainml/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/job/create.py` & `trainml-0.5.6/trainml/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/model.py` & `trainml-0.5.6/trainml/cli/model.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cli/project.py` & `trainml-0.5.6/trainml/cli/project.py`

 * *Files 11% similar despite different names*

```diff
@@ -111,44 +111,39 @@
             "{: >38.36} {: >30.28} {: >15.13} {: >38.36}" "".format(*row),
             file=config.stdout,
         )
 
 
 @project.command()
 @pass_config
-def list_reservations(config):
-    """List project reservations."""
+def list_services(config):
+    """List project services."""
     data = [
-        ["ID", "NAME", "TYPE", "RESOURCE", "HOSTNAME", "REGION_UUID"],
+        ["ID", "NAME", "HOSTNAME", "REGION_UUID"],
         [
             "-" * 80,
             "-" * 80,
             "-" * 80,
             "-" * 80,
-            "-" * 80,
-            "-" * 80,
         ],
     ]
     project = config.trainml.run(
         config.trainml.client.projects.get(config.trainml.client.project)
     )
 
-    reservations = config.trainml.run(project.list_reservations())
+    services = config.trainml.run(project.list_services())
 
-    for reservation in reservations:
+    for service in services:
         data.append(
             [
-                reservation.id,
-                reservation.name,
-                reservation.type,
-                reservation.resource,
-                reservation.hostname,
-                reservation.region_uuid,
+                service.id,
+                service.name,
+                service.hostname,
+                service.region_uuid,
             ]
         )
 
     for row in data:
         click.echo(
-            "{: >38.36} {: >30.28} {: >8.6} {: >15.13} {: >30.28} {: >38.36}"
-            "".format(*row),
+            "{: >38.36} {: >30.28} {: >30.28} {: >38.36}" "".format(*row),
             file=config.stdout,
         )
```

### Comparing `trainml-0.5.5/trainml/cli/volume.py` & `trainml-0.5.6/trainml/cli/volume.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/datastores.py` & `trainml-0.5.6/trainml/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/device_configs.py` & `trainml-0.5.6/trainml/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/devices.py` & `trainml-0.5.6/trainml/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/nodes.py` & `trainml-0.5.6/trainml/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/providers.py` & `trainml-0.5.6/trainml/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/regions.py` & `trainml-0.5.6/trainml/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/cloudbender/reservations.py` & `trainml-0.5.6/trainml/cloudbender/services.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,126 +1,115 @@
 import json
 import logging
 
 
-class Reservations(object):
+class Services(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def get(self, provider_uuid, region_uuid, id, **kwargs):
         resp = await self.trainml._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/reservation/{id}",
+            f"/provider/{provider_uuid}/region/{region_uuid}/service/{id}",
             "GET",
             kwargs,
         )
-        return Reservation(self.trainml, **resp)
+        return Service(self.trainml, **resp)
 
     async def list(self, provider_uuid, region_uuid, **kwargs):
         resp = await self.trainml._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/reservation",
+            f"/provider/{provider_uuid}/region/{region_uuid}/service",
             "GET",
             kwargs,
         )
-        reservations = [
-            Reservation(self.trainml, **reservation) for reservation in resp
-        ]
-        return reservations
+        services = [Service(self.trainml, **service) for service in resp]
+        return services
 
     async def create(
         self,
         provider_uuid,
         region_uuid,
         name,
-        type,
-        resource,
-        hostname,
+        public,
         **kwargs,
     ):
-        logging.info(f"Creating Reservation {name}")
+        logging.info(f"Creating Service {name}")
         data = dict(
             name=name,
-            type=type,
-            resource=resource,
-            hostname=hostname,
+            public=public,
             **kwargs,
         )
         payload = {k: v for k, v in data.items() if v is not None}
         resp = await self.trainml._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/reservation",
+            f"/provider/{provider_uuid}/region/{region_uuid}/service",
             "POST",
             None,
             payload,
         )
-        reservation = Reservation(self.trainml, **resp)
-        logging.info(f"Created Reservation {name} with id {reservation.id}")
-        return reservation
+        service = Service(self.trainml, **resp)
+        logging.info(f"Created Service {name} with id {service.id}")
+        return service
 
     async def remove(self, provider_uuid, region_uuid, id, **kwargs):
         await self.trainml._query(
-            f"/provider/{provider_uuid}/region/{region_uuid}/reservation/{id}",
+            f"/provider/{provider_uuid}/region/{region_uuid}/service/{id}",
             "DELETE",
             kwargs,
         )
 
 
-class Reservation:
+class Service:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
-        self._reservation = kwargs
-        self._id = self._reservation.get("reservation_id")
-        self._provider_uuid = self._reservation.get("provider_uuid")
-        self._region_uuid = self._reservation.get("region_uuid")
-        self._type = self._reservation.get("type")
-        self._name = self._reservation.get("name")
-        self._resource = self._reservation.get("resource")
-        self._hostname = self._reservation.get("hostname")
+        self._service = kwargs
+        self._id = self._service.get("service_id")
+        self._provider_uuid = self._service.get("provider_uuid")
+        self._region_uuid = self._service.get("region_uuid")
+        self._public = self._service.get("public")
+        self._name = self._service.get("name")
+        self._hostname = self._service.get("hostname")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def provider_uuid(self) -> str:
         return self._provider_uuid
 
     @property
     def region_uuid(self) -> str:
         return self._region_uuid
 
     @property
-    def type(self) -> str:
-        return self._type
+    def public(self) -> bool:
+        return self._public
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def resource(self) -> str:
-        return self._resource
-
-    @property
     def hostname(self) -> str:
         return self._hostname
 
     def __str__(self):
-        return json.dumps({k: v for k, v in self._reservation.items()})
+        return json.dumps({k: v for k, v in self._service.items()})
 
     def __repr__(self):
-        return f"Reservation( trainml , **{self._reservation.__repr__()})"
+        return f"Service( trainml , **{self._service.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
         await self.trainml._query(
-            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/reservation/{self._id}",
+            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/service/{self._id}",
             "DELETE",
         )
 
     async def refresh(self):
         resp = await self.trainml._query(
-            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/reservation/{self._id}",
+            f"/provider/{self._provider_uuid}/region/{self._region_uuid}/service/{self._id}",
             "GET",
         )
         self.__init__(self.trainml, **resp)
         return self
```

### Comparing `trainml-0.5.5/trainml/connections.py` & `trainml-0.5.6/trainml/connections.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/datasets.py` & `trainml-0.5.6/trainml/datasets.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/environments.py` & `trainml-0.5.6/trainml/environments.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/exceptions.py` & `trainml-0.5.6/trainml/exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/gpu_types.py` & `trainml-0.5.6/trainml/gpu_types.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/jobs.py` & `trainml-0.5.6/trainml/jobs.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/models.py` & `trainml-0.5.6/trainml/models.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/projects.py` & `trainml-0.5.6/trainml/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,25 +68,25 @@
     def __repr__(self):
         return f"ProjectDatastore( trainml , **{self._datastore.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
 
-class ProjectReservation:
+class ProjectService:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
-        self._reservation = kwargs
-        self._id = self._reservation.get("id")
-        self._project_uuid = self._reservation.get("project_uuid")
-        self._name = self._reservation.get("name")
-        self._type = self._reservation.get("type")
-        self._hostname = self._reservation.get("hostname")
-        self._resource = self._reservation.get("resource")
-        self._region_uuid = self._reservation.get("region_uuid")
+        self._service = kwargs
+        self._id = self._service.get("id")
+        self._project_uuid = self._service.get("project_uuid")
+        self._name = self._service.get("name")
+        self._type = self._service.get("type")
+        self._hostname = self._service.get("hostname")
+        self._resource = self._service.get("resource")
+        self._region_uuid = self._service.get("region_uuid")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def project_uuid(self) -> str:
@@ -109,20 +109,18 @@
         return self._resource
 
     @property
     def region_uuid(self) -> str:
         return self._region_uuid
 
     def __str__(self):
-        return json.dumps({k: v for k, v in self._reservation.items()})
+        return json.dumps({k: v for k, v in self._service.items()})
 
     def __repr__(self):
-        return (
-            f"ProjectReservation( trainml , **{self._reservation.__repr__()})"
-        )
+        return f"ProjectService( trainml , **{self._service.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
 
 class Project:
     def __init__(self, trainml, **kwargs):
@@ -158,30 +156,21 @@
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
         await self.trainml._query(f"/project/{self._id}", "DELETE")
 
     async def list_datastores(self):
-        resp = await self.trainml._query(
-            f"/project/{self._id}/datastores", "GET"
-        )
-        datastores = [
-            ProjectDatastore(self.trainml, **datastore) for datastore in resp
-        ]
+        resp = await self.trainml._query(f"/project/{self._id}/datastores", "GET")
+        datastores = [ProjectDatastore(self.trainml, **datastore) for datastore in resp]
         return datastores
 
-    async def list_reservations(self):
-        resp = await self.trainml._query(
-            f"/project/{self._id}/reservations", "GET"
-        )
-        reservations = [
-            ProjectReservation(self.trainml, **reservation)
-            for reservation in resp
-        ]
-        return reservations
+    async def list_services(self):
+        resp = await self.trainml._query(f"/project/{self._id}/services", "GET")
+        services = [ProjectService(self.trainml, **service) for service in resp]
+        return services
 
     async def refresh_datastores(self):
         await self.trainml._query(f"/project/{self._id}/datastores", "PATCH")
 
-    async def refresh_reservations(self):
-        await self.trainml._query(f"/project/{self._id}/reservations", "PATCH")
+    async def refresh_services(self):
+        await self.trainml._query(f"/project/{self._id}/services", "PATCH")
```

### Comparing `trainml-0.5.5/trainml/trainml.py` & `trainml-0.5.6/trainml/trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml/volumes.py` & `trainml-0.5.6/trainml/volumes.py`

 * *Files identical despite different names*

### Comparing `trainml-0.5.5/trainml.egg-info/PKG-INFO` & `trainml-0.5.6/trainml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.5.5
+Version: 0.5.6
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.5.5 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.6 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._t_r_a_i_n_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_t_r_a_i_n_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.5.5/trainml.egg-info/SOURCES.txt` & `trainml-0.5.6/trainml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 tests/unit/cloudbender/__init__.py
 tests/unit/cloudbender/test_datastores_unit.py
 tests/unit/cloudbender/test_device_configs_unit.py
 tests/unit/cloudbender/test_devices_unit.py
 tests/unit/cloudbender/test_nodes_unit.py
 tests/unit/cloudbender/test_providers_unit.py
 tests/unit/cloudbender/test_regions_unit.py
-tests/unit/cloudbender/test_reservations_unit.py
+tests/unit/cloudbender/test_services_unit.py
 trainml/__init__.py
 trainml/__main__.py
 trainml/auth.py
 trainml/checkpoints.py
 trainml/connections.py
 trainml/datasets.py
 trainml/environments.py
@@ -88,19 +88,19 @@
 trainml/cli/volume.py
 trainml/cli/cloudbender/__init__.py
 trainml/cli/cloudbender/datastore.py
 trainml/cli/cloudbender/device.py
 trainml/cli/cloudbender/node.py
 trainml/cli/cloudbender/provider.py
 trainml/cli/cloudbender/region.py
-trainml/cli/cloudbender/reservation.py
+trainml/cli/cloudbender/service.py
 trainml/cli/job/__init__.py
 trainml/cli/job/create.py
 trainml/cloudbender/__init__.py
 trainml/cloudbender/cloudbender.py
 trainml/cloudbender/datastores.py
 trainml/cloudbender/device_configs.py
 trainml/cloudbender/devices.py
 trainml/cloudbender/nodes.py
 trainml/cloudbender/providers.py
 trainml/cloudbender/regions.py
-trainml/cloudbender/reservations.py
+trainml/cloudbender/services.py
```

