# Comparing `tmp/cugraph-pyg-cu12-24.2.0.tar.gz` & `tmp/cugraph_pyg_cu12-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cugraph-pyg-cu12-24.2.0.tar", last modified: Thu Feb 15 17:59:29 2024, max compression
+gzip compressed data, was "cugraph_pyg_cu12-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cugraph-pyg-cu12-24.2.0.tar` & `cugraph_pyg_cu12-24.4.0.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-15 17:59:29.007434 cugraph-pyg-cu12-24.2.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      463 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 cugraph-pyg-cu12-24.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       16 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1650 2024-02-15 17:59:29.006435 cugraph-pyg-cu12-24.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      268 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-15 17:59:29.006435 cugraph-pyg-cu12-24.2.0/cugraph_pyg_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1650 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/cugraph_pyg_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      213 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/cugraph_pyg_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/cugraph_pyg_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-02-15 17:59:28.000000 cugraph-pyg-cu12-24.2.0/cugraph_pyg_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-02-15 17:59:29.007434 cugraph-pyg-cu12-24.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 cugraph-pyg-cu12-24.2.0/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     1042 1993-04-05 07:00:00.000000 PKG-INFO
```

