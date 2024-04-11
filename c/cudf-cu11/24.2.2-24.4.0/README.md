# Comparing `tmp/cudf-cu11-24.2.2.tar.gz` & `tmp/cudf_cu11-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudf-cu11-24.2.2.tar", last modified: Tue Feb 27 22:41:39 2024, max compression
+gzip compressed data, was "cudf_cu11-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cudf-cu11-24.2.2.tar` & `cudf_cu11-24.4.0.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-27 22:41:39.267588 cudf-cu11-24.2.2/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      456 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 cudf-cu11-24.2.2/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1622 2024-02-27 22:41:39.266589 cudf-cu11-24.2.2/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-27 22:41:39.266589 cudf-cu11-24.2.2/cudf_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1622 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/cudf_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/cudf_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/cudf_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-02-27 22:41:39.000000 cudf-cu11-24.2.2/cudf_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-02-27 22:41:39.267588 cudf-cu11-24.2.2/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 cudf-cu11-24.2.2/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     6056 1993-04-05 07:00:00.000000 PKG-INFO
```

