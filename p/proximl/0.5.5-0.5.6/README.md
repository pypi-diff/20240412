# Comparing `tmp/proximl-0.5.5.tar.gz` & `tmp/proximl-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proximl-0.5.5.tar", last modified: Tue Apr  2 13:17:39 2024, max compression
+gzip compressed data, was "proximl-0.5.6.tar", last modified: Fri Apr 12 19:06:44 2024, max compression
```

## Comparing `proximl-0.5.5.tar` & `proximl-0.5.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.702524 proximl-0.5.5/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-02 13:14:52.000000 proximl-0.5.5/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-02 13:17:39.702373 proximl-0.5.5/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-02 13:14:52.000000 proximl-0.5.5/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.685341 proximl-0.5.5/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-02 13:14:52.000000 proximl-0.5.5/examples/training_inference_pipeline.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.688743 proximl-0.5.5/proximl/
--rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.690963 proximl-0.5.5/proximl/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/checkpoint.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.691873 proximl-0.5.5/proximl/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)      534 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/datastore.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/device.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/node.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/region.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/cloudbender/reservation.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.692142 proximl-0.5.5/proximl/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cli/volume.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.693600 proximl-0.5.5/proximl/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      634 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/cloudbender.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/datastores.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/device_configs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/devices.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/nodes.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/regions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3586 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/cloudbender/reservations.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-04-02 13:14:52.000000 proximl-0.5.5/proximl/volumes.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.689502 proximl-0.5.5/proximl.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     3502 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-02 13:17:39.000000 proximl-0.5.5/proximl.egg-info/top_level.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)     1000 2024-04-02 13:14:52.000000 proximl-0.5.5/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-02 13:17:39.702570 proximl-0.5.5/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-02 13:14:52.000000 proximl-0.5.5/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.683774 proximl-0.5.5/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.695319 proximl-0.5.5/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.695535 proximl-0.5.5/tests/integration/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/cloudbender/test_providers_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/integration/test_volumes_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.698396 proximl-0.5.5/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.699740 proximl-0.5.5/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.700585 proximl-0.5.5/tests/unit/cli/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_gpu_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_job_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_model_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_project_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cli/test_cli_volume_unit.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:17:39.702142 proximl-0.5.5/tests/unit/cloudbender/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_datastores_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_devices_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_nodes_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_regions_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5624 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/cloudbender/test_reservations_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    31197 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_proximl.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-02 13:14:52.000000 proximl-0.5.5/tests/unit/test_volumes_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.193520 proximl-0.5.6/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2024-04-12 17:04:07.000000 proximl-0.5.6/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-12 19:06:44.193363 proximl-0.5.6/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2024-04-12 17:04:07.000000 proximl-0.5.6/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.175377 proximl-0.5.6/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2024-04-12 17:04:07.000000 proximl-0.5.6/examples/training_inference_pipeline.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.179232 proximl-0.5.6/proximl/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26565 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.181314 proximl-0.5.6/proximl/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4346 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.182253 proximl-0.5.6/proximl/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      526 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3453 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/device.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2869 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/cloudbender/service.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6871 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.182568 proximl-0.5.6/proximl/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34288 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6111 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3314 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/project.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6246 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cli/volume.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.183916 proximl-0.5.6/proximl/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      618 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3506 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3399 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5660 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/devices.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4332 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2036 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3570 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3222 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/cloudbender/services.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20035 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7935 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4094 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1901 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    17838 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7750 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5001 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10864 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8094 2024-04-12 17:04:07.000000 proximl-0.5.6/proximl/volumes.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.179968 proximl-0.5.6/proximl.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8987 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3490 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2024-04-12 19:06:44.000000 proximl-0.5.6/proximl.egg-info/top_level.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)      992 2024-04-12 17:04:07.000000 proximl-0.5.6/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2024-04-12 19:06:44.193565 proximl-0.5.6/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1225 2024-04-12 17:04:07.000000 proximl-0.5.6/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.173766 proximl-0.5.6/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.185226 proximl-0.5.6/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.185443 proximl-0.5.6/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3230 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3499 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    24730 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2902 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1446 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_projects_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3270 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/integration/test_volumes_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.188844 proximl-0.5.6/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.190508 proximl-0.5.6/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.191471 proximl-0.5.6/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1342 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1311 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1688 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_project_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      644 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cli/test_cli_volume_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2024-04-12 19:06:44.193117 proximl-0.5.6/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5398 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5714 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9103 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_devices_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6231 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4373 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6299 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5043 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/cloudbender/test_services_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    31129 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      858 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9238 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_proximl.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15305 2024-04-12 17:04:07.000000 proximl-0.5.6/tests/unit/test_volumes_unit.py
```

### Comparing `proximl-0.5.5/LICENSE` & `proximl-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/PKG-INFO` & `proximl-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.5
+Version: 0.5.6
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.5 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.6 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.5/README.md` & `proximl-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/examples/create_dataset_and_training_job.py` & `proximl-0.5.6/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/examples/local_storage.py` & `proximl-0.5.6/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/examples/training_inference_pipeline.py` & `proximl-0.5.6/examples/training_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/auth.py` & `proximl-0.5.6/proximl/auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/checkpoints.py` & `proximl-0.5.6/proximl/checkpoints.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/__init__.py` & `proximl-0.5.6/proximl/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/checkpoint.py` & `proximl-0.5.6/proximl/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/__init__.py` & `proximl-0.5.6/proximl/cli/cloudbender/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 
 
 from proximl.cli.cloudbender.provider import provider
 from proximl.cli.cloudbender.region import region
 from proximl.cli.cloudbender.node import node
 from proximl.cli.cloudbender.device import device
 from proximl.cli.cloudbender.datastore import datastore
-from proximl.cli.cloudbender.reservation import reservation
+from proximl.cli.cloudbender.service import service
```

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/datastore.py` & `proximl-0.5.6/proximl/cli/cloudbender/datastore.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/device.py` & `proximl-0.5.6/proximl/cli/cloudbender/device.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/node.py` & `proximl-0.5.6/proximl/cli/cloudbender/node.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/provider.py` & `proximl-0.5.6/proximl/cli/cloudbender/provider.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/region.py` & `proximl-0.5.6/proximl/cli/cloudbender/region.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/cloudbender/reservation.py` & `proximl-0.5.6/proximl/cli/cloudbender/service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,129 @@
 import click
 from proximl.cli import cli, pass_config, search_by_id_name
 from proximl.cli.cloudbender import cloudbender
 
 
 @cloudbender.group()
 @pass_config
-def reservation(config):
-    """proxiML CloudBender reservation commands."""
+def service(config):
+    """proxiML CloudBender service commands."""
     pass
 
 
-@reservation.command()
+@service.command()
 @click.option(
     "--provider",
     "-p",
     type=click.STRING,
     required=True,
     help="The provider ID of the region.",
 )
 @click.option(
     "--region",
     "-r",
     type=click.STRING,
     required=True,
-    help="The region ID to list reservations for.",
+    help="The region ID to list services for.",
 )
 @pass_config
 def list(config, provider, region):
-    """List reservations."""
+    """List services."""
     data = [
-        ["ID", "NAME", "TYPE", "RESOURCE", "HOSTNAME"],
+        ["ID", "NAME", "HOSTNAME"],
         [
             "-" * 80,
             "-" * 80,
             "-" * 80,
-            "-" * 80,
-            "-" * 80,
         ],
     ]
 
-    reservations = config.proximl.run(
-        config.proximl.client.cloudbender.reservations.list(
+    services = config.proximl.run(
+        config.proximl.client.cloudbender.services.list(
             provider_uuid=provider, region_uuid=region
         )
     )
 
-    for reservation in reservations:
+    for service in services:
         data.append(
             [
-                reservation.id,
-                reservation.name,
-                reservation.type,
-                reservation.resource,
-                reservation.hostname,
+                service.id,
+                service.name,
+                service.hostname,
             ]
         )
 
     for row in data:
         click.echo(
-            "{: >37.36} {: >29.28} {: >9.8} {: >9.8} {: >29.28}"
-            "".format(*row),
+            "{: >25.24} {: >29.28} {: >40.39}" "".format(*row),
             file=config.stdout,
         )
 
 
-@reservation.command()
+@service.command()
 @click.option(
     "--provider",
     "-p",
     type=click.STRING,
     required=True,
     help="The provider ID of the region.",
 )
 @click.option(
     "--region",
     "-r",
     type=click.STRING,
     required=True,
-    help="The region ID to create the reservation in.",
-)
-@click.option(
-    "--type",
-    "-t",
-    type=click.Choice(
-        [
-            "port",
-        ],
-        case_sensitive=False,
-    ),
-    required=True,
-    help="The type of reservation to create.",
-)
-@click.option(
-    "--hostname",
-    "-h",
-    type=click.STRING,
-    required=True,
-    help="The hostname to make the reservation on",
+    help="The region ID to create the service in.",
 )
 @click.option(
-    "--resource",
-    "-r",
-    type=click.STRING,
-    required=True,
-    help="The resource to reserve",
+    "--public/--no-public",
+    default=True,
+    show_default=True,
+    help="Service should be accessible from the public internet.",
 )
 @click.argument("name", type=click.STRING, required=True)
 @pass_config
-def create(config, provider, region, type, hostname, resource, name):
+def create(config, provider, region, public, name):
     """
-    Creates a reservation.
+    Creates a service.
     """
     return config.proximl.run(
-        config.proximl.client.cloudbender.reservations.create(
-            provider_uuid=provider,
-            region_uuid=region,
-            name=name,
-            hostname=hostname,
-            resource=resource,
-            type=type,
+        config.proximl.client.cloudbender.services.create(
+            provider_uuid=provider, region_uuid=region, name=name, public=public
         )
     )
 
 
-@reservation.command()
+@service.command()
 @click.option(
     "--provider",
     "-p",
     type=click.STRING,
     required=True,
     help="The provider ID of the region.",
 )
 @click.option(
     "--region",
     "-r",
     type=click.STRING,
     required=True,
-    help="The region ID to remove the reservation from.",
+    help="The region ID to remove the service from.",
 )
-@click.argument("reservation", type=click.STRING)
+@click.argument("service", type=click.STRING)
 @pass_config
-def remove(config, provider, region, reservation):
+def remove(config, provider, region, service):
     """
-    Remove a reservation.
+    Remove a service.
 
     RESERVATION may be specified by name or ID, but ID is preferred.
     """
-    reservations = config.proximl.run(
-        config.proximl.client.cloudbender.reservations.list(
+    services = config.proximl.run(
+        config.proximl.client.cloudbender.services.list(
             provider_uuid=provider, region_uuid=region
         )
     )
 
-    found = search_by_id_name(reservation, reservations)
+    found = search_by_id_name(service, services)
     if None is found:
-        raise click.UsageError("Cannot find specified reservation.")
+        raise click.UsageError("Cannot find specified service.")
 
     return config.proximl.run(found.remove())
```

### Comparing `proximl-0.5.5/proximl/cli/connection.py` & `proximl-0.5.6/proximl/cli/connection.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/dataset.py` & `proximl-0.5.6/proximl/cli/dataset.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/environment.py` & `proximl-0.5.6/proximl/cli/environment.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/gpu.py` & `proximl-0.5.6/proximl/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/job/__init__.py` & `proximl-0.5.6/proximl/cli/job/__init__.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/job/create.py` & `proximl-0.5.6/proximl/cli/job/create.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/model.py` & `proximl-0.5.6/proximl/cli/model.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cli/project.py` & `proximl-0.5.6/proximl/cli/project.py`

 * *Files 13% similar despite different names*

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
     project = config.proximl.run(
         config.proximl.client.projects.get(config.proximl.client.project)
     )
 
-    reservations = config.proximl.run(project.list_reservations())
+    services = config.proximl.run(project.list_services())
 
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

### Comparing `proximl-0.5.5/proximl/cli/volume.py` & `proximl-0.5.6/proximl/cli/volume.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/cloudbender.py` & `proximl-0.5.6/proximl/cloudbender/cloudbender.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from .providers import Providers
 from .regions import Regions
 from .nodes import Nodes
 from .devices import Devices
 from .datastores import Datastores
-from .reservations import Reservations
+from .services import Services
 from .device_configs import DeviceConfigs
 
 
 class Cloudbender(object):
     def __init__(self, proximl):
         self.proximl = proximl
         self.providers = Providers(proximl)
         self.regions = Regions(proximl)
         self.nodes = Nodes(proximl)
         self.devices = Devices(proximl)
         self.datastores = Datastores(proximl)
-        self.reservations = Reservations(proximl)
+        self.services = Services(proximl)
         self.device_configs = DeviceConfigs(proximl)
```

### Comparing `proximl-0.5.5/proximl/cloudbender/datastores.py` & `proximl-0.5.6/proximl/cloudbender/datastores.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/device_configs.py` & `proximl-0.5.6/proximl/cloudbender/device_configs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/devices.py` & `proximl-0.5.6/proximl/cloudbender/devices.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/nodes.py` & `proximl-0.5.6/proximl/cloudbender/nodes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/providers.py` & `proximl-0.5.6/proximl/cloudbender/providers.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/cloudbender/regions.py` & `proximl-0.5.6/proximl/cloudbender/regions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/connections.py` & `proximl-0.5.6/proximl/connections.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/datasets.py` & `proximl-0.5.6/proximl/datasets.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/environments.py` & `proximl-0.5.6/proximl/environments.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/exceptions.py` & `proximl-0.5.6/proximl/exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/gpu_types.py` & `proximl-0.5.6/proximl/gpu_types.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/jobs.py` & `proximl-0.5.6/proximl/jobs.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/models.py` & `proximl-0.5.6/proximl/models.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/projects.py` & `proximl-0.5.6/proximl/projects.py`

 * *Files 14% similar despite different names*

```diff
@@ -68,25 +68,25 @@
     def __repr__(self):
         return f"ProjectDatastore( proximl , **{self._datastore.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
 
-class ProjectReservation:
+class ProjectService:
     def __init__(self, proximl, **kwargs):
         self.proximl = proximl
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
-            f"ProjectReservation( proximl , **{self._reservation.__repr__()})"
-        )
+        return f"ProjectService( proximl , **{self._service.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
 
 class Project:
     def __init__(self, proximl, **kwargs):
@@ -158,30 +156,21 @@
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
         await self.proximl._query(f"/project/{self._id}", "DELETE")
 
     async def list_datastores(self):
-        resp = await self.proximl._query(
-            f"/project/{self._id}/datastores", "GET"
-        )
-        datastores = [
-            ProjectDatastore(self.proximl, **datastore) for datastore in resp
-        ]
+        resp = await self.proximl._query(f"/project/{self._id}/datastores", "GET")
+        datastores = [ProjectDatastore(self.proximl, **datastore) for datastore in resp]
         return datastores
 
-    async def list_reservations(self):
-        resp = await self.proximl._query(
-            f"/project/{self._id}/reservations", "GET"
-        )
-        reservations = [
-            ProjectReservation(self.proximl, **reservation)
-            for reservation in resp
-        ]
-        return reservations
+    async def list_services(self):
+        resp = await self.proximl._query(f"/project/{self._id}/services", "GET")
+        services = [ProjectService(self.proximl, **service) for service in resp]
+        return services
 
     async def refresh_datastores(self):
         await self.proximl._query(f"/project/{self._id}/datastores", "PATCH")
 
-    async def refresh_reservations(self):
-        await self.proximl._query(f"/project/{self._id}/reservations", "PATCH")
+    async def refresh_services(self):
+        await self.proximl._query(f"/project/{self._id}/services", "PATCH")
```

### Comparing `proximl-0.5.5/proximl/proximl.py` & `proximl-0.5.6/proximl/proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl/volumes.py` & `proximl-0.5.6/proximl/volumes.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/proximl.egg-info/PKG-INFO` & `proximl-0.5.6/proximl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proximl
-Version: 0.5.5
+Version: 0.5.6
 Summary: proxiML client SDK and command line utilities
 Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML
 Author-email: support@proximl.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.proximl.ai/"><img src="https://www.proximl.ai/static/img/proxiML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proximl Version: 0.5.5 Summary: proxiML client SDK
+Metadata-Version: 2.1 Name: proximl Version: 0.5.6 Summary: proxiML client SDK
 and command line utilities Home-page: https://github.com/proxiML/python-sdk
 Author: proxiML Author-email: support@proximl.ai License: MIT Description:
           _[_h_t_t_p_s_:_/_/_w_w_w_._p_r_o_x_i_m_l_._a_i_/_s_t_a_t_i_c_/_i_m_g_/_p_r_o_x_i_M_L_-_l_o_g_o_-_p_u_r_p_l_e_._p_n_g_]
 # proxiML Python SDK and Command Line Tools Provides programmatic access to
 [proxiML platform](https://app.proximl.ai). ## Installation Python 3.8 or above
 is required. ``` pip install proximl ``` ## Authentication ### Prerequisites
 You must have a valid [proxiML account](https://app.proximl.ai). On the
```

### Comparing `proximl-0.5.5/proximl.egg-info/SOURCES.txt` & `proximl-0.5.6/proximl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,26 +37,26 @@
 proximl/cli/volume.py
 proximl/cli/cloudbender/__init__.py
 proximl/cli/cloudbender/datastore.py
 proximl/cli/cloudbender/device.py
 proximl/cli/cloudbender/node.py
 proximl/cli/cloudbender/provider.py
 proximl/cli/cloudbender/region.py
-proximl/cli/cloudbender/reservation.py
+proximl/cli/cloudbender/service.py
 proximl/cli/job/__init__.py
 proximl/cli/job/create.py
 proximl/cloudbender/__init__.py
 proximl/cloudbender/cloudbender.py
 proximl/cloudbender/datastores.py
 proximl/cloudbender/device_configs.py
 proximl/cloudbender/devices.py
 proximl/cloudbender/nodes.py
 proximl/cloudbender/providers.py
 proximl/cloudbender/regions.py
-proximl/cloudbender/reservations.py
+proximl/cloudbender/services.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/test_checkpoints_integration.py
 tests/integration/test_datasets_integration.py
 tests/integration/test_environments_integration.py
 tests/integration/test_gpu_types_integration.py
 tests/integration/test_jobs_integration.py
@@ -99,8 +99,8 @@
 tests/unit/cloudbender/__init__.py
 tests/unit/cloudbender/test_datastores_unit.py
 tests/unit/cloudbender/test_device_configs_unit.py
 tests/unit/cloudbender/test_devices_unit.py
 tests/unit/cloudbender/test_nodes_unit.py
 tests/unit/cloudbender/test_providers_unit.py
 tests/unit/cloudbender/test_regions_unit.py
-tests/unit/cloudbender/test_reservations_unit.py
+tests/unit/cloudbender/test_services_unit.py
```

### Comparing `proximl-0.5.5/pyproject.toml` & `proximl-0.5.6/pyproject.toml`

 * *Files 18% similar despite different names*

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
     "unit: All unit tests (no proxiML environment required)",
     "integration: All integration tests (proxiML environment required)",
     "sdk: All tests of the SDK",
     "cli: All test of the cli",
 ]
```

### Comparing `proximl-0.5.5/setup.py` & `proximl-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/cloudbender/test_providers_integration.py` & `proximl-0.5.6/tests/integration/cloudbender/test_providers_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/conftest.py` & `proximl-0.5.6/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_checkpoints_integration.py` & `proximl-0.5.6/tests/integration/test_checkpoints_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_datasets_integration.py` & `proximl-0.5.6/tests/integration/test_datasets_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_environments_integration.py` & `proximl-0.5.6/tests/integration/test_environments_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_gpu_types_integration.py` & `proximl-0.5.6/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_jobs_integration.py` & `proximl-0.5.6/tests/integration/test_jobs_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_models_integration.py` & `proximl-0.5.6/tests/integration/test_models_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_projects_integration.py` & `proximl-0.5.6/tests/integration/test_projects_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/integration/test_volumes_integration.py` & `proximl-0.5.6/tests/integration/test_volumes_integration.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_datastore_unit.py` & `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_datastore_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_device_unit.py` & `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_device_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_node_unit.py` & `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_node_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_provider_unit.py` & `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_provider_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/cloudbender/test_cli_region_unit.py` & `proximl-0.5.6/tests/unit/cli/cloudbender/test_cli_region_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_checkpoint_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_checkpoint_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_datasets_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_environment_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_gpu_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_gpu_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_job_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_job_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_model_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_model_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_project_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_project_unit.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,28 +19,24 @@
         assert result.exit_code == 0
         mock_proximl.projects.list.assert_called_once()
 
 
 def test_list_datastores(runner, mock_project_datastores):
     with patch("proximl.cli.ProxiML", new=AsyncMock) as mock_proximl:
         mock_project = create_autospec(Project)
-        mock_project.list_datastores = AsyncMock(
-            return_value=mock_project_datastores
-        )
+        mock_project.list_datastores = AsyncMock(return_value=mock_project_datastores)
         mock_proximl.projects.get = AsyncMock(return_value=mock_project)
         result = runner.invoke(specimen, ["list-datastores"])
         print(result)
         assert result.exit_code == 0
         mock_project.list_datastores.assert_called_once()
 
 
-def test_list_reservations(runner, mock_project_reservations):
+def test_list_services(runner, mock_project_services):
     with patch("proximl.cli.ProxiML", new=AsyncMock) as mock_proximl:
         mock_project = create_autospec(Project)
-        mock_project.list_reservations = AsyncMock(
-            return_value=mock_project_reservations
-        )
+        mock_project.list_services = AsyncMock(return_value=mock_project_services)
         mock_proximl.projects.get = AsyncMock(return_value=mock_project)
-        result = runner.invoke(specimen, ["list-reservations"])
+        result = runner.invoke(specimen, ["list-services"])
         print(result)
         assert result.exit_code == 0
-        mock_project.list_reservations.assert_called_once()
+        mock_project.list_services.assert_called_once()
```

### Comparing `proximl-0.5.5/tests/unit/cli/test_cli_volume_unit.py` & `proximl-0.5.6/tests/unit/cli/test_cli_volume_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_datastores_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_datastores_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_device_configs_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_device_configs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_devices_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_devices_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_nodes_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_nodes_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_providers_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_providers_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/cloudbender/test_regions_unit.py` & `proximl-0.5.6/tests/unit/cloudbender/test_regions_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/conftest.py` & `proximl-0.5.6/tests/unit/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 from proximl.environments import Environment, Environments
 from proximl.jobs import Job, Jobs
 from proximl.connections import Connections
 from proximl.projects import (
     Projects,
     Project,
     ProjectDatastore,
-    ProjectReservation,
+    ProjectService,
 )
 from proximl.cloudbender import Cloudbender
 from proximl.cloudbender.providers import Provider, Providers
 from proximl.cloudbender.regions import Region, Regions
 from proximl.cloudbender.nodes import Node, Nodes
 from proximl.cloudbender.devices import Device, Devices
 from proximl.cloudbender.datastores import Datastore, Datastores
-from proximl.cloudbender.reservations import Reservation, Reservations
+from proximl.cloudbender.services import Service, Services
 from proximl.cloudbender.device_configs import DeviceConfig, DeviceConfigs
 
 
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
     proximl = Mock()
     yield [
-        Reservation(
+        Service(
             proximl,
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
             proximl,
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
     proximl = Mock()
     yield [
-        ProjectReservation(
+        ProjectService(
             proximl,
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
             proximl,
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
     proximl = create_autospec(ProxiML)
     proximl.active_project = "proj-id-1"
     proximl.project = "proj-id-1"
     proximl.datasets = create_autospec(Datasets)
     proximl.checkpoints = create_autospec(Checkpoints)
@@ -1024,14 +1024,14 @@
     proximl.cloudbender.regions.list = AsyncMock(return_value=mock_regions)
     proximl.cloudbender.nodes = create_autospec(Nodes)
     proximl.cloudbender.nodes.list = AsyncMock(return_value=mock_nodes)
     proximl.cloudbender.devices = create_autospec(Nodes)
     proximl.cloudbender.devices.list = AsyncMock(return_value=mock_devices)
     proximl.cloudbender.datastores = create_autospec(Datastores)
     proximl.cloudbender.datastores.list = AsyncMock(return_value=mock_datastores)
-    proximl.cloudbender.reservations = create_autospec(Reservations)
-    proximl.cloudbender.reservations.list = AsyncMock(return_value=mock_reservations)
+    proximl.cloudbender.services = create_autospec(Services)
+    proximl.cloudbender.services.list = AsyncMock(return_value=mock_services)
     proximl.cloudbender.device_configs = create_autospec(DeviceConfigs)
     proximl.cloudbender.device_configs.list = AsyncMock(
         return_value=mock_device_configs
     )
     yield proximl
```

### Comparing `proximl-0.5.5/tests/unit/test_auth.py` & `proximl-0.5.6/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_checkpoints_unit.py` & `proximl-0.5.6/tests/unit/test_checkpoints_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_connections_unit.py` & `proximl-0.5.6/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_datasets_unit.py` & `proximl-0.5.6/tests/unit/test_datasets_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_environments_unit.py` & `proximl-0.5.6/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_exceptions.py` & `proximl-0.5.6/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_gpu_types_unit.py` & `proximl-0.5.6/tests/unit/test_gpu_types_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_jobs_unit.py` & `proximl-0.5.6/tests/unit/test_jobs_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_models_unit.py` & `proximl-0.5.6/tests/unit/test_models_unit.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_projects_unit.py` & `proximl-0.5.6/tests/unit/test_projects_unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,19 +45,19 @@
         project_uuid="proj-id-1",
         type="nfs",
         region_uuid="reg-id-1",
     )
 
 
 @fixture
-def project_reservation(mock_proximl):
-    yield specimen.ProjectReservation(
+def project_service(mock_proximl):
+    yield specimen.ProjectService(
         mock_proximl,
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
         mock_proximl,
     ):
         api_response = dict()
         mock_proximl._query = AsyncMock(return_value=api_response)
         await projects.get("1234")
-        mock_proximl._query.assert_called_once_with(
-            "/project/1234", "GET", dict()
-        )
+        mock_proximl._query.assert_called_once_with("/project/1234", "GET", dict())
 
     @mark.asyncio
     async def test_list_projects(
         self,
         projects,
         mock_proximl,
     ):
@@ -92,17 +90,15 @@
         self,
         projects,
         mock_proximl,
     ):
         api_response = dict()
         mock_proximl._query = AsyncMock(return_value=api_response)
         await projects.remove("4567")
-        mock_proximl._query.assert_called_once_with(
-            "/project/4567", "DELETE", dict()
-        )
+        mock_proximl._query.assert_called_once_with("/project/4567", "DELETE", dict())
 
     @mark.asyncio
     async def test_create_project_simple(self, projects, mock_proximl):
         requested_config = dict(
             name="new project",
         )
         expected_payload = dict(name="new project", copy_keys=False)
@@ -152,44 +148,44 @@
 
     def test_project_datastore_bool(self, project_datastore, mock_proximl):
         empty_project_datastore = specimen.ProjectDatastore(mock_proximl)
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
-            r"^ProjectReservation\( proximl , \*\*{.*'id': '"
-            + project_reservation.id
+            r"^ProjectService\( proximl , \*\*{.*'id': '"
+            + project_service.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_project_reservation_bool(self, project_reservation, mock_proximl):
-        empty_project_reservation = specimen.ProjectReservation(mock_proximl)
-        assert bool(project_reservation)
-        assert not bool(empty_project_reservation)
+    def test_project_service_bool(self, project_service, mock_proximl):
+        empty_project_service = specimen.ProjectService(mock_proximl)
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
-            r"^Project\( proximl , \*\*{.*'id': '" + project.id + r"'.*}\)$"
-        )
+        regex = r"^Project\( proximl , \*\*{.*'id': '" + project.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     def test_project_bool(self, project, mock_proximl):
         empty_project = specimen.Project(mock_proximl)
         assert bool(project)
         assert not bool(empty_project)
@@ -222,26 +216,22 @@
         mock_proximl._query.assert_called_once_with("/project/1", "DELETE")
 
     @mark.asyncio
     async def test_project_refresh_datastores(self, project, mock_proximl):
         api_response = dict()
         mock_proximl._query = AsyncMock(return_value=api_response)
         await project.refresh_datastores()
-        mock_proximl._query.assert_called_once_with(
-            "/project/1/datastores", "PATCH"
-        )
+        mock_proximl._query.assert_called_once_with("/project/1/datastores", "PATCH")
 
     @mark.asyncio
-    async def test_project_refresh_reservations(self, project, mock_proximl):
+    async def test_project_refresh_services(self, project, mock_proximl):
         api_response = dict()
         mock_proximl._query = AsyncMock(return_value=api_response)
-        await project.refresh_reservations()
-        mock_proximl._query.assert_called_once_with(
-            "/project/1/reservations", "PATCH"
-        )
+        await project.refresh_services()
+        mock_proximl._query.assert_called_once_with("/project/1/services", "PATCH")
 
     @mark.asyncio
     async def test_project_list_datastores(self, project, mock_proximl):
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
         mock_proximl._query = AsyncMock(return_value=api_response)
         resp = await project.list_datastores()
-        mock_proximl._query.assert_called_once_with(
-            "/project/1/datastores", "GET"
-        )
+        mock_proximl._query.assert_called_once_with("/project/1/datastores", "GET")
         assert len(resp) == 2
 
     @mark.asyncio
-    async def test_project_list_reservations(self, project, mock_proximl):
+    async def test_project_list_services(self, project, mock_proximl):
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
         mock_proximl._query = AsyncMock(return_value=api_response)
-        resp = await project.list_reservations()
-        mock_proximl._query.assert_called_once_with(
-            "/project/1/reservations", "GET"
-        )
+        resp = await project.list_services()
+        mock_proximl._query.assert_called_once_with("/project/1/services", "GET")
         assert len(resp) == 2
```

### Comparing `proximl-0.5.5/tests/unit/test_proximl.py` & `proximl-0.5.6/tests/unit/test_proximl.py`

 * *Files identical despite different names*

### Comparing `proximl-0.5.5/tests/unit/test_volumes_unit.py` & `proximl-0.5.6/tests/unit/test_volumes_unit.py`

 * *Files identical despite different names*

