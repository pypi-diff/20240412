# Comparing `tmp/cuml-cu12-24.2.0.tar.gz` & `tmp/cuml_cu12-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuml-cu12-24.2.0.tar", last modified: Wed Feb 14 14:14:11 2024, max compression
+gzip compressed data, was "cuml_cu12-24.4.0.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cuml-cu12-24.2.0.tar` & `cuml_cu12-24.4.0.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-14 14:14:11.127521 cuml-cu12-24.2.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      456 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 cuml-cu12-24.2.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1622 2024-02-14 14:14:11.126521 cuml-cu12-24.2.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      247 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-02-14 14:14:11.126521 cuml-cu12-24.2.0/cuml_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1622 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/cuml_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/cuml_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/cuml_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-02-14 14:14:11.000000 cuml-cu12-24.2.0/cuml_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-02-14 14:14:11.127521 cuml-cu12-24.2.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 cuml-cu12-24.2.0/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     4354 1993-04-05 07:00:00.000000 PKG-INFO
```

