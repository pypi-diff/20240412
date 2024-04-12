# Comparing `tmp/dask-cuda-24.2.0a7.tar.gz` & `tmp/dask-cuda-24.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-24.2.0a7.tar", last modified: Thu Nov 16 06:15:05 2023, max compression
+gzip compressed data, was "dask-cuda-24.2.0a8.tar", last modified: Thu Nov 16 16:24:40 2023, max compression
```

## Comparing `dask-cuda-24.2.0a7.tar` & `dask-cuda-24.2.0a8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.139170 dask-cuda-24.2.0a7/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       56 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2489 2023-11-16 06:15:05.135170 dask-cuda-24.2.0a7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1004 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.127170 dask-cuda-24.2.0a7/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)       11 2023-11-16 06:15:00.000000 dask-cuda-24.2.0a7/dask_cuda/VERSION
--rw-r--r--   0 root         (0) root         (0)     1455 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      778 2023-11-16 06:15:00.000000 dask-cuda-24.2.0a7/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.131170 dask-cuda-24.2.0a7/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8904 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12447 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8608 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10762 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6442 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26896 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15970 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8579 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    10272 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6626 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.131170 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10400 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.131170 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20124 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     6462 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17928 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/plugins.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29812 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.135170 dask-cuda-24.2.0a7/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    17729 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6986 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    12315 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)      601 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_from_array.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     6960 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    18376 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18630 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23758 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)    10239 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     9176 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    25121 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/utils_test.py
--rw-r--r--   0 root         (0) root         (0)     4376 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.131170 dask-cuda-24.2.0a7/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2489 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      287 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-11-16 06:15:05.000000 dask-cuda-24.2.0a7/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.123170 dask-cuda-24.2.0a7/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 06:15:05.135170 dask-cuda-24.2.0a7/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-11-16 06:15:00.000000 dask-cuda-24.2.0a7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-16 06:15:05.139170 dask-cuda-24.2.0a7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-11-16 06:14:58.000000 dask-cuda-24.2.0a7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.080404 dask-cuda-24.2.0a8/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       56 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-11-16 16:24:40.080404 dask-cuda-24.2.0a8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.072404 dask-cuda-24.2.0a8/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)       11 2023-11-16 16:24:35.000000 dask-cuda-24.2.0a8/dask_cuda/VERSION
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-11-16 16:24:35.000000 dask-cuda-24.2.0a8/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.076404 dask-cuda-24.2.0a8/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12447 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8608 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10762 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6442 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26896 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15970 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8579 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)    10272 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.076404 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10400 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.076404 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20124 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     6462 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17928 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29812 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.080404 dask-cuda-24.2.0a8/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    17729 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6986 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    12315 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)      601 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_from_array.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     6960 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    18376 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18630 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23758 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    25121 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1694 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/utils_test.py
+-rw-r--r--   0 root         (0) root         (0)     4376 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.072404 dask-cuda-24.2.0a8/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      283 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-11-16 16:24:40.000000 dask-cuda-24.2.0a8/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.068404 dask-cuda-24.2.0a8/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-16 16:24:40.080404 dask-cuda-24.2.0a8/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-11-16 16:24:35.000000 dask-cuda-24.2.0a8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-16 16:24:40.080404 dask-cuda-24.2.0a8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-11-16 16:24:33.000000 dask-cuda-24.2.0a8/setup.py
```

### Comparing `dask-cuda-24.2.0a7/LICENSE` & `dask-cuda-24.2.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/PKG-INFO` & `dask-cuda-24.2.0a8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 24.2.0a7
+Version: 24.2.0a8
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
@@ -17,25 +17,25 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba>=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas<1.6.0dev0,>=1.3
 Requires-Dist: pynvml<11.5,>=11.0.0
-Requires-Dist: rapids-dask-dependency==24.02.*,>=0.0.0a0
+Requires-Dist: rapids-dask-dependency==24.2.*,>=0.0.0a0
 Requires-Dist: zict>=2.0.0
 Provides-Extra: docs
 Requires-Dist: numpydoc>=1.1.0; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-click>=2.7.1; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=0.5.1; extra == "docs"
 Provides-Extra: test
-Requires-Dist: cudf==24.02.*; extra == "test"
-Requires-Dist: dask-cudf==24.02.*; extra == "test"
-Requires-Dist: kvikio==24.02.*; extra == "test"
+Requires-Dist: cudf==24.2.*; extra == "test"
+Requires-Dist: dask-cudf==24.2.*; extra == "test"
+Requires-Dist: kvikio==24.2.*; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ucx-py==0.36.*; extra == "test"
 
 Dask CUDA
 =========
```

### Comparing `dask-cuda-24.2.0a7/README.md` & `dask-cuda-24.2.0a8/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/__init__.py` & `dask-cuda-24.2.0a8/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/_version.py` & `dask-cuda-24.2.0a8/dask_cuda/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 
 import importlib.resources
 
 __version__ = (
     importlib.resources.files("dask_cuda").joinpath("VERSION").read_text().strip()
 )
-__git_commit__ = "6dd83ed98ed02919eec5df3154a55da8cf0491c3"
+__git_commit__ = "297ad677033c1c0ded32f7c94165291134444b59"
```

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/common.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/benchmarks/utils.py` & `dask-cuda-24.2.0a8/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/cli.py` & `dask-cuda-24.2.0a8/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/cuda_worker.py` & `dask-cuda-24.2.0a8/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/device_host_file.py` & `dask-cuda-24.2.0a8/dask_cuda/device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/disk_io.py` & `dask-cuda-24.2.0a8/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/explicit_comms/comms.py` & `dask-cuda-24.2.0a8/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-24.2.0a8/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/get_device_memory_objects.py` & `dask-cuda-24.2.0a8/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/initialize.py` & `dask-cuda-24.2.0a8/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/is_device_object.py` & `dask-cuda-24.2.0a8/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/is_spillable_object.py` & `dask-cuda-24.2.0a8/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/local_cuda_cluster.py` & `dask-cuda-24.2.0a8/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/plugins.py` & `dask-cuda-24.2.0a8/dask_cuda/plugins.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/proxify_device_objects.py` & `dask-cuda-24.2.0a8/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/proxify_host_file.py` & `dask-cuda-24.2.0a8/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/proxy_object.py` & `dask-cuda-24.2.0a8/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_dgx.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_from_array.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_from_array.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_gds.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_initialize.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_proxy.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_spill.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_utils.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-24.2.0a8/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/utils.py` & `dask-cuda-24.2.0a8/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/utils_test.py` & `dask-cuda-24.2.0a8/dask_cuda/utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda/worker_spec.py` & `dask-cuda-24.2.0a8/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-24.2.0a8/dask_cuda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 24.2.0a7
+Version: 24.2.0a8
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
@@ -17,25 +17,25 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numba>=0.57
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas<1.6.0dev0,>=1.3
 Requires-Dist: pynvml<11.5,>=11.0.0
-Requires-Dist: rapids-dask-dependency==24.02.*,>=0.0.0a0
+Requires-Dist: rapids-dask-dependency==24.2.*,>=0.0.0a0
 Requires-Dist: zict>=2.0.0
 Provides-Extra: docs
 Requires-Dist: numpydoc>=1.1.0; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-click>=2.7.1; extra == "docs"
 Requires-Dist: sphinx-rtd-theme>=0.5.1; extra == "docs"
 Provides-Extra: test
-Requires-Dist: cudf==24.02.*; extra == "test"
-Requires-Dist: dask-cudf==24.02.*; extra == "test"
-Requires-Dist: kvikio==24.02.*; extra == "test"
+Requires-Dist: cudf==24.2.*; extra == "test"
+Requires-Dist: dask-cudf==24.2.*; extra == "test"
+Requires-Dist: kvikio==24.2.*; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: ucx-py==0.36.*; extra == "test"
 
 Dask CUDA
 =========
```

### Comparing `dask-cuda-24.2.0a7/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-24.2.0a8/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/examples/ucx/client_initialize.py` & `dask-cuda-24.2.0a8/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/examples/ucx/local_cuda_cluster.py` & `dask-cuda-24.2.0a8/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-24.2.0a7/pyproject.toml` & `dask-cuda-24.2.0a8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 license = { text = "Apache-2.0" }
 requires-python = ">=3.9"
 dependencies = [
     "numba>=0.57",
     "numpy>=1.21",
     "pandas>=1.3,<1.6.0dev0",
     "pynvml>=11.0.0,<11.5",
-    "rapids-dask-dependency==24.02.*,>=0.0.0a0",
+    "rapids-dask-dependency==24.2.*,>=0.0.0a0",
     "zict>=2.0.0",
 ] # This list was generated by `rapids-dependency-file-generator`. To make changes, edit dependencies.yaml and run `rapids-dependency-file-generator`.
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Database",
     "Topic :: Scientific/Engineering",
     "License :: OSI Approved :: Apache Software License",
@@ -44,17 +44,17 @@
 docs = [
     "numpydoc>=1.1.0",
     "sphinx",
     "sphinx-click>=2.7.1",
     "sphinx-rtd-theme>=0.5.1",
 ] # This list was generated by `rapids-dependency-file-generator`. To make changes, edit dependencies.yaml and run `rapids-dependency-file-generator`.
 test = [
-    "cudf==24.02.*",
-    "dask-cudf==24.02.*",
-    "kvikio==24.02.*",
+    "cudf==24.2.*",
+    "dask-cudf==24.2.*",
+    "kvikio==24.2.*",
     "pytest",
     "pytest-cov",
     "ucx-py==0.36.*",
 ] # This list was generated by `rapids-dependency-file-generator`. To make changes, edit dependencies.yaml and run `rapids-dependency-file-generator`.
 
 [project.urls]
 Homepage = "https://github.com/rapidsai/dask-cuda"
```

