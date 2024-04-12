# Comparing `tmp/tierkreis-0.7.0.tar.gz` & `tmp/tierkreis-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tierkreis-0.7.0.tar", last modified: Tue Apr  9 08:38:50 2024, max compression
+gzip compressed data, was "tierkreis-0.7.1.tar", last modified: Fri Apr 12 11:06:10 2024, max compression
```

## Comparing `tierkreis-0.7.0.tar` & `tierkreis-0.7.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.890560 tierkreis-0.7.0/
--rw-r--r--   0 seyon      (502) staff       (20)     6928 2024-04-09 08:38:50.890315 tierkreis-0.7.0/PKG-INFO
--rw-r--r--   0 seyon      (502) staff       (20)     5315 2024-04-08 15:53:23.000000 tierkreis-0.7.0/README.md
--rw-r--r--   0 seyon      (502) staff       (20)     2149 2024-04-08 15:53:22.000000 tierkreis-0.7.0/pyproject.toml
--rw-r--r--   0 seyon      (502) staff       (20)       38 2024-04-09 08:38:50.890614 tierkreis-0.7.0/setup.cfg
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.877149 tierkreis-0.7.0/tests/
--rw-r--r--   0 seyon      (502) staff       (20)    29142 2024-04-09 08:38:37.000000 tierkreis-0.7.0/tests/test_builder.py
--rw-r--r--   0 seyon      (502) staff       (20)     3467 2024-02-13 11:22:18.000000 tierkreis-0.7.0/tests/test_commontypes.py
--rw-r--r--   0 seyon      (502) staff       (20)     7553 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_frontend.py
--rw-r--r--   0 seyon      (502) staff       (20)     5937 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_generics.py
--rw-r--r--   0 seyon      (502) staff       (20)      834 2024-02-13 11:22:18.000000 tierkreis-0.7.0/tests/test_pyruntime.py
--rw-r--r--   0 seyon      (502) staff       (20)     2680 2024-02-09 15:49:47.000000 tierkreis-0.7.0/tests/test_pytket_worker.py
--rw-r--r--   0 seyon      (502) staff       (20)     6541 2024-02-13 16:35:16.000000 tierkreis-0.7.0/tests/test_tierkreis_graph.py
--rw-r--r--   0 seyon      (502) staff       (20)     9996 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tests/test_type_check.py
--rw-r--r--   0 seyon      (502) staff       (20)    12126 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tests/test_variants.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.878931 tierkreis-0.7.0/tierkreis/
--rw-r--r--   0 seyon      (502) staff       (20)      423 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.879895 tierkreis-0.7.0/tierkreis/_build/
--rw-r--r--   0 seyon      (502) staff       (20)     2034 2024-01-31 13:06:30.000000 tierkreis-0.7.0/tierkreis/_build/generate_protos.py
--rw-r--r--   0 seyon      (502) staff       (20)       22 2024-04-09 08:38:37.000000 tierkreis-0.7.0/tierkreis/_version.py
--rw-r--r--   0 seyon      (502) staff       (20)    29295 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tierkreis/builder.py
--rw-r--r--   0 seyon      (502) staff       (20)     8197 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/cli.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.880791 tierkreis-0.7.0/tierkreis/client/
--rw-r--r--   0 seyon      (502) staff       (20)      120 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)      665 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/runtime_client.py
--rw-r--r--   0 seyon      (502) staff       (20)     6292 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/client/server_client.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.881385 tierkreis-0.7.0/tierkreis/common_types/
--rw-r--r--   0 seyon      (502) staff       (20)     3267 2024-02-09 15:49:47.000000 tierkreis-0.7.0/tierkreis/common_types/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)     3678 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/common_types/circuit.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.884718 tierkreis-0.7.0/tierkreis/core/
--rw-r--r--   0 seyon      (502) staff       (20)      334 2023-12-12 17:11:07.000000 tierkreis-0.7.0/tierkreis/core/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)      993 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/function.py
--rw-r--r--   0 seyon      (502) staff       (20)    14621 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/graphviz.py
--rw-r--r--   0 seyon      (502) staff       (20)     3559 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/core/internal.py
--rw-r--r--   0 seyon      (502) staff       (20)      800 2024-02-08 09:05:47.000000 tierkreis-0.7.0/tierkreis/core/opaque_model.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885125 tierkreis-0.7.0/tierkreis/core/protos/
--rw-r--r--   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.872980 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885234 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/
--rw-r--r--   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885346 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/
--rw-r--r--   0 seyon      (502) staff       (20)     7330 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885491 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/
--rw-r--r--   0 seyon      (502) staff       (20)     9122 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885641 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/
--rw-r--r--   0 seyon      (502) staff       (20)     2834 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885803 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/
--rw-r--r--   0 seyon      (502) staff       (20)     8629 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.885959 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/
--rw-r--r--   0 seyon      (502) staff       (20)     2504 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)      631 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/python.py
--rw-r--r--   0 seyon      (502) staff       (20)     2299 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/signature.py
--rw-r--r--   0 seyon      (502) staff       (20)    22367 2024-04-08 11:23:50.000000 tierkreis-0.7.0/tierkreis/core/tierkreis_graph.py
--rw-r--r--   0 seyon      (502) staff       (20)     6796 2024-02-13 16:19:23.000000 tierkreis-0.7.0/tierkreis/core/type_errors.py
--rw-r--r--   0 seyon      (502) staff       (20)     2290 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/type_inference.py
--rw-r--r--   0 seyon      (502) staff       (20)    21946 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/core/types.py
--rw-r--r--   0 seyon      (502) staff       (20)     1616 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/core/utils.py
--rw-r--r--   0 seyon      (502) staff       (20)    28160 2024-04-08 15:53:23.000000 tierkreis-0.7.0/tierkreis/core/values.py
--rw-r--r--   0 seyon      (502) staff       (20)        0 2023-06-28 10:16:02.000000 tierkreis-0.7.0/tierkreis/py.typed
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.886890 tierkreis-0.7.0/tierkreis/pyruntime/
--rw-r--r--   0 seyon      (502) staff       (20)       38 2023-12-05 11:53:45.000000 tierkreis-0.7.0/tierkreis/pyruntime/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)    21024 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/pyruntime/python_builtin.py
--rw-r--r--   0 seyon      (502) staff       (20)    12559 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/pyruntime/python_runtime.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.888796 tierkreis-0.7.0/tierkreis/worker/
--rw-r--r--   0 seyon      (502) staff       (20)       82 2023-12-05 11:53:45.000000 tierkreis-0.7.0/tierkreis/worker/__init__.py
--rw-r--r--   0 seyon      (502) staff       (20)     1430 2024-02-01 14:26:16.000000 tierkreis-0.7.0/tierkreis/worker/callback.py
--rw-r--r--   0 seyon      (502) staff       (20)      643 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/worker/exceptions.py
--rw-r--r--   0 seyon      (502) staff       (20)    10452 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/worker/namespace.py
--rw-r--r--   0 seyon      (502) staff       (20)     1797 2024-03-08 11:34:47.000000 tierkreis-0.7.0/tierkreis/worker/prelude.py
--rw-r--r--   0 seyon      (502) staff       (20)      945 2023-12-07 09:29:31.000000 tierkreis-0.7.0/tierkreis/worker/tracing.py
--rw-r--r--   0 seyon      (502) staff       (20)     9611 2024-04-08 15:53:22.000000 tierkreis-0.7.0/tierkreis/worker/worker.py
-drwxr-xr-x   0 seyon      (502) staff       (20)        0 2024-04-09 08:38:50.889089 tierkreis-0.7.0/tierkreis.egg-info/
--rw-r--r--   0 seyon      (502) staff       (20)     6928 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/PKG-INFO
--rw-r--r--   0 seyon      (502) staff       (20)     1812 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/SOURCES.txt
--rw-r--r--   0 seyon      (502) staff       (20)        1 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/dependency_links.txt
--rw-r--r--   0 seyon      (502) staff       (20)       43 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/entry_points.txt
--rw-r--r--   0 seyon      (502) staff       (20)      550 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/requires.txt
--rw-r--r--   0 seyon      (502) staff       (20)       10 2024-04-09 08:38:50.000000 tierkreis-0.7.0/tierkreis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.672152 tierkreis-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-12 11:06:10.672152 tierkreis-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-12 11:05:53.000000 tierkreis-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-12 11:05:53.000000 tierkreis-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:06:10.672152 tierkreis-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.660152 tierkreis-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    29142 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_commontypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_pyruntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_pytket_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6541 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_tierkreis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9996 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tests/test_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.664152 tierkreis-0.7.1/tierkreis/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.664152 tierkreis-0.7.1/tierkreis/_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/_build/generate_protos.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29295 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8197 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.664152 tierkreis-0.7.1/tierkreis/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/client/runtime_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/client/server_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.664152 tierkreis-0.7.1/tierkreis/common_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/common_types/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14621 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/opaque_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.660152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22367 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/tierkreis_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/type_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/type_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21946 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28160 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/core/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.668152 tierkreis-0.7.1/tierkreis/pyruntime/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/pyruntime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21024 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/pyruntime/python_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12559 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/pyruntime/python_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.672152 tierkreis-0.7.1/tierkreis/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/prelude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-04-12 11:05:53.000000 tierkreis-0.7.1/tierkreis/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:06:10.672152 tierkreis-0.7.1/tierkreis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 11:06:10.000000 tierkreis-0.7.1/tierkreis.egg-info/top_level.txt
```

### Comparing `tierkreis-0.7.0/PKG-INFO` & `tierkreis-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: betterproto[compiler]==2.0.0b6
-Requires-Dist: protobuf<4,>=3.19
 Requires-Dist: grpclib<0.5,>=0.4.3rc
 Requires-Dist: networkx<3,>=2.6.3
 Requires-Dist: graphviz<0.21,>=0.20
 Requires-Dist: click==8.1.3
 Requires-Dist: yachalk<0.2,>=0.1.4
 Requires-Dist: requests<3,>=2.31
 Requires-Dist: pydantic~=2.5
 Provides-Extra: docker
 Requires-Dist: docker<6,>=5; extra == "docker"
 Provides-Extra: telemetry
-Requires-Dist: opentelemetry-sdk<2,>=1.5.0; extra == "telemetry"
-Requires-Dist: opentelemetry-exporter-otlp<2,>=1.5.0; extra == "telemetry"
+Requires-Dist: opentelemetry-sdk<2,>=1.15.0; extra == "telemetry"
+Requires-Dist: opentelemetry-exporter-otlp<2,>=1.15.0; extra == "telemetry"
 Provides-Extra: commontypes
 Requires-Dist: pytket>=1.0; extra == "commontypes"
 Provides-Extra: lint
 Requires-Dist: ruff~=0.3; extra == "lint"
 Requires-Dist: pyright==1.1.345; extra == "lint"
 Requires-Dist: tierkreis[docker,sc22-example,telemetry]; extra == "lint"
 Provides-Extra: test
```

### Comparing `tierkreis-0.7.0/README.md` & `tierkreis-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/pyproject.toml` & `tierkreis-0.7.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     { name = "John Children", email = "john.children@quantinuum.com" },
     { name = "Alan Lawrence", email = "alan.lawrence@quantinuum.com" },
 ]
 
 requires-python = ">=3.10,<3.13"
 dependencies = [
     "betterproto[compiler]==2.0.0b6",
-    "protobuf>=3.19,<4",              # Restrict version to maintain compatibility with opentelemetry
     "grpclib>=0.4.3rc,<0.5",          # pre-release to support python 3.10
     "networkx>=2.6.3,<3",
     "graphviz>=0.20,<0.21",
     "click==8.1.3",                   # 8.1.4 causes mypy fails
     "yachalk>=0.1.4,<0.2",
     "requests>=2.31,<3",
     "pydantic~=2.5",
@@ -26,16 +25,16 @@
 [project.scripts]
 tkrs = 'tierkreis.cli:cli'
 
 [project.optional-dependencies]
 docker = ["docker>=5,<6"]
 
 telemetry = [
-    "opentelemetry-sdk>=1.5.0,<2",
-    "opentelemetry-exporter-otlp>=1.5.0,<2",
+    "opentelemetry-sdk>=1.15.0,<2",
+    "opentelemetry-exporter-otlp>=1.15.0,<2",
 ]
 
 commontypes = ["pytket>=1.0"]
 lint = [
     "ruff~=0.3",
     "pyright==1.1.345",
     "tierkreis[sc22-example,telemetry,docker]",
```

### Comparing `tierkreis-0.7.0/tests/test_builder.py` & `tierkreis-0.7.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_commontypes.py` & `tierkreis-0.7.1/tests/test_commontypes.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_frontend.py` & `tierkreis-0.7.1/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_generics.py` & `tierkreis-0.7.1/tests/test_generics.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_pyruntime.py` & `tierkreis-0.7.1/tests/test_pyruntime.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_pytket_worker.py` & `tierkreis-0.7.1/tests/test_pytket_worker.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_tierkreis_graph.py` & `tierkreis-0.7.1/tests/test_tierkreis_graph.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_type_check.py` & `tierkreis-0.7.1/tests/test_type_check.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tests/test_variants.py` & `tierkreis-0.7.1/tests/test_variants.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/_build/generate_protos.py` & `tierkreis-0.7.1/tierkreis/_build/generate_protos.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/builder.py` & `tierkreis-0.7.1/tierkreis/builder.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/cli.py` & `tierkreis-0.7.1/tierkreis/cli.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/client/runtime_client.py` & `tierkreis-0.7.1/tierkreis/client/runtime_client.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/client/server_client.py` & `tierkreis-0.7.1/tierkreis/client/server_client.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/common_types/__init__.py` & `tierkreis-0.7.1/tierkreis/common_types/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/common_types/circuit.py` & `tierkreis-0.7.1/tierkreis/common_types/circuit.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/function.py` & `tierkreis-0.7.1/tierkreis/core/function.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/graphviz.py` & `tierkreis-0.7.1/tierkreis/core/graphviz.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/internal.py` & `tierkreis-0.7.1/tierkreis/core/internal.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/opaque_model.py` & `tierkreis-0.7.1/tierkreis/core/opaque_model.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py` & `tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py` & `tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py` & `tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py` & `tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py` & `tierkreis-0.7.1/tierkreis/core/protos/tierkreis/v1alpha1/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/python.py` & `tierkreis-0.7.1/tierkreis/core/python.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/signature.py` & `tierkreis-0.7.1/tierkreis/core/signature.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/tierkreis_graph.py` & `tierkreis-0.7.1/tierkreis/core/tierkreis_graph.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/type_errors.py` & `tierkreis-0.7.1/tierkreis/core/type_errors.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/type_inference.py` & `tierkreis-0.7.1/tierkreis/core/type_inference.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/types.py` & `tierkreis-0.7.1/tierkreis/core/types.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/utils.py` & `tierkreis-0.7.1/tierkreis/core/utils.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/core/values.py` & `tierkreis-0.7.1/tierkreis/core/values.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/pyruntime/python_builtin.py` & `tierkreis-0.7.1/tierkreis/pyruntime/python_builtin.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/pyruntime/python_runtime.py` & `tierkreis-0.7.1/tierkreis/pyruntime/python_runtime.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/callback.py` & `tierkreis-0.7.1/tierkreis/worker/callback.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/exceptions.py` & `tierkreis-0.7.1/tierkreis/worker/exceptions.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/namespace.py` & `tierkreis-0.7.1/tierkreis/worker/namespace.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/prelude.py` & `tierkreis-0.7.1/tierkreis/worker/prelude.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/tracing.py` & `tierkreis-0.7.1/tierkreis/worker/tracing.py`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis/worker/worker.py` & `tierkreis-0.7.1/tierkreis/worker/worker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Worker server implementation."""
 
 import functools
 import sys
 from contextvars import ContextVar
 from tempfile import TemporaryDirectory
-from traceback import print_tb
+from traceback import print_exception
 from typing import Any, Callable, Coroutine, Optional
 
 import grpclib
 import grpclib.events
 import grpclib.server
 from grpclib.const import Status as StatusCode
 from grpclib.exceptions import GRPCError
@@ -209,18 +209,20 @@
             ) from err
         except FunctionNotFound as err:
             raise GRPCError(
                 status=StatusCode.UNIMPLEMENTED,
                 message=f"Unsupported function: {function}",
             ) from err
         except NodeExecutionError as err:
-            # The response resulting from the GRPCError below does not seem to include
-            # any part of the original stack trace
+            # The response resulting from the GRPCError below does not include
+            # the original traceback to avoid leaking implementation details.
+            # The traceback is instead printed to local stderr.
             print(f"Error in running {function}:", file=sys.stderr)
-            print_tb((err.__cause__ or err).__traceback__)
+            print_exception(err.base_exception)
+
             raise GRPCError(
                 status=StatusCode.UNKNOWN,
                 message=f"Error while running operation: {repr(err.base_exception)}",
             ) from err
 
 
 class SignatureServerImpl(ps.SignatureBase):
```

### Comparing `tierkreis-0.7.0/tierkreis.egg-info/PKG-INFO` & `tierkreis-0.7.1/tierkreis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: tierkreis
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python client and utilities for tierkreis.
 Author-email: Seyon Sivarajah <seyon.sivarajah@quantinuum.com>, Lukas Heidemann <lukas.heidemann@quantinuum.com>, John Children <john.children@quantinuum.com>, Alan Lawrence <alan.lawrence@quantinuum.com>
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: betterproto[compiler]==2.0.0b6
-Requires-Dist: protobuf<4,>=3.19
 Requires-Dist: grpclib<0.5,>=0.4.3rc
 Requires-Dist: networkx<3,>=2.6.3
 Requires-Dist: graphviz<0.21,>=0.20
 Requires-Dist: click==8.1.3
 Requires-Dist: yachalk<0.2,>=0.1.4
 Requires-Dist: requests<3,>=2.31
 Requires-Dist: pydantic~=2.5
 Provides-Extra: docker
 Requires-Dist: docker<6,>=5; extra == "docker"
 Provides-Extra: telemetry
-Requires-Dist: opentelemetry-sdk<2,>=1.5.0; extra == "telemetry"
-Requires-Dist: opentelemetry-exporter-otlp<2,>=1.5.0; extra == "telemetry"
+Requires-Dist: opentelemetry-sdk<2,>=1.15.0; extra == "telemetry"
+Requires-Dist: opentelemetry-exporter-otlp<2,>=1.15.0; extra == "telemetry"
 Provides-Extra: commontypes
 Requires-Dist: pytket>=1.0; extra == "commontypes"
 Provides-Extra: lint
 Requires-Dist: ruff~=0.3; extra == "lint"
 Requires-Dist: pyright==1.1.345; extra == "lint"
 Requires-Dist: tierkreis[docker,sc22-example,telemetry]; extra == "lint"
 Provides-Extra: test
```

### Comparing `tierkreis-0.7.0/tierkreis.egg-info/SOURCES.txt` & `tierkreis-0.7.1/tierkreis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tierkreis-0.7.0/tierkreis.egg-info/requires.txt` & `tierkreis-0.7.1/tierkreis.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 betterproto[compiler]==2.0.0b6
-protobuf<4,>=3.19
 grpclib<0.5,>=0.4.3rc
 networkx<3,>=2.6.3
 graphviz<0.21,>=0.20
 click==8.1.3
 yachalk<0.2,>=0.1.4
 requests<3,>=2.31
 pydantic~=2.5
@@ -20,16 +19,16 @@
 tierkreis[docker,sc22-example,telemetry]
 
 [sc22-example]
 numpy<2,>=1.20
 pytket>=1.0
 
 [telemetry]
-opentelemetry-sdk<2,>=1.5.0
-opentelemetry-exporter-otlp<2,>=1.5.0
+opentelemetry-sdk<2,>=1.15.0
+opentelemetry-exporter-otlp<2,>=1.15.0
 
 [test]
 pytest<7,>=6.2
 pytest-asyncio<0.17,>=0.16
 tierkreis[commontypes,typecheck]
 
 [typecheck]
```

