# Comparing `tmp/dask-cudf-cu12-24.2.2.tar.gz` & `tmp/dask_cudf_cu12-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cudf-cu12-24.2.2.tar", last modified: Wed Feb 28 01:14:54 2024, max compression
+gzip compressed data, was "dask_cudf_cu12-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `dask-cudf-cu12-24.2.2.tar` & `dask_cudf_cu12-24.4.0.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-28 01:14:54.059841 dask-cudf-cu12-24.2.2/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      461 2024-02-28 01:14:53.000000 dask-cudf-cu12-24.2.2/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 dask-cudf-cu12-24.2.2/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       14 2024-02-28 01:14:53.000000 dask-cudf-cu12-24.2.2/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1642 2024-02-28 01:14:54.059841 dask-cudf-cu12-24.2.2/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      262 2024-02-28 01:14:53.000000 dask-cudf-cu12-24.2.2/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-28 01:14:54.059841 dask-cudf-cu12-24.2.2/dask_cudf_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1642 2024-02-28 01:14:54.000000 dask-cudf-cu12-24.2.2/dask_cudf_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      205 2024-02-28 01:14:54.000000 dask-cudf-cu12-24.2.2/dask_cudf_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-02-28 01:14:54.000000 dask-cudf-cu12-24.2.2/dask_cudf_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-02-28 01:14:54.000000 dask-cudf-cu12-24.2.2/dask_cudf_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-02-28 01:14:54.059841 dask-cudf-cu12-24.2.2/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 dask-cudf-cu12-24.2.2/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     4966 1993-04-05 07:00:00.000000 PKG-INFO
```

