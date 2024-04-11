# Comparing `tmp/cuopt_sh_client-24.3.5.tar.gz` & `tmp/cuopt_sh_client-24.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuopt_sh_client-24.3.5.tar", last modified: Tue Mar 12 13:08:11 2024, max compression
+gzip compressed data, was "cuopt_sh_client-24.3.6.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cuopt_sh_client-24.3.5.tar` & `cuopt_sh_client-24.3.6.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-12 13:08:11.162446 cuopt_sh_client-24.3.5/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      462 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-02-13 20:52:43.000000 cuopt_sh_client-24.3.5/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       15 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1646 2024-03-12 13:08:11.161446 cuopt_sh_client-24.3.5/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      265 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-03-12 13:08:11.161446 cuopt_sh_client-24.3.5/cuopt_sh_client.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1646 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/cuopt_sh_client.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      209 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/cuopt_sh_client.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/cuopt_sh_client.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-03-12 13:08:11.000000 cuopt_sh_client-24.3.5/cuopt_sh_client.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-03-12 13:08:11.162446 cuopt_sh_client-24.3.5/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-02-13 20:52:43.000000 cuopt_sh_client-24.3.5/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     8828 1993-04-05 07:00:00.000000 PKG-INFO
```

