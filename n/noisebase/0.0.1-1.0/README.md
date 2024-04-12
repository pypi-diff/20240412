# Comparing `tmp/noisebase-0.0.1.tar.gz` & `tmp/noisebase-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisebase-0.0.1.tar", last modified: Thu Feb 29 21:10:46 2024, max compression
+gzip compressed data, was "noisebase-1.0.tar", last modified: Fri Apr 12 09:42:22 2024, max compression
```

## Comparing `noisebase-0.0.1.tar` & `noisebase-1.0.tar`

### file list

```diff
@@ -1,13 +1,54 @@
-drwxrwsr-x   0 mbalint  (23702) seidel    (4000)        0 2024-02-29 21:10:46.298292 noisebase-0.0.1/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      621 2024-02-29 21:10:46.298292 noisebase-0.0.1/PKG-INFO
--rw-rw-r--   0 mbalint  (23702) seidel    (4000)       12 2024-02-29 21:01:28.000000 noisebase-0.0.1/README.md
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      706 2024-02-29 21:01:28.000000 noisebase-0.0.1/pyproject.toml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      105 2024-02-29 21:10:46.302293 noisebase-0.0.1/setup.cfg
-drwxrwsr-x   0 mbalint  (23702) seidel    (4000)        0 2024-02-29 21:10:46.246292 noisebase-0.0.1/src/
-drwxrwsr-x   0 mbalint  (23702) seidel    (4000)        0 2024-02-29 21:10:46.262292 noisebase-0.0.1/src/noisebase/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-02-29 21:10:38.000000 noisebase-0.0.1/src/noisebase/__init__.py
-drwxrwsr-x   0 mbalint  (23702) seidel    (4000)        0 2024-02-29 21:10:46.290293 noisebase-0.0.1/src/noisebase.egg-info/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      621 2024-02-29 21:10:46.000000 noisebase-0.0.1/src/noisebase.egg-info/PKG-INFO
--rw-rw-r--   0 mbalint  (23702) seidel    (4000)      208 2024-02-29 21:10:46.000000 noisebase-0.0.1/src/noisebase.egg-info/SOURCES.txt
--rw-rw-r--   0 mbalint  (23702) seidel    (4000)        1 2024-02-29 21:10:46.000000 noisebase-0.0.1/src/noisebase.egg-info/dependency_links.txt
--rw-rw-r--   0 mbalint  (23702) seidel    (4000)       10 2024-02-29 21:10:46.000000 noisebase-0.0.1/src/noisebase.egg-info/top_level.txt
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.866147 noisebase-1.0/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    11344 2024-04-09 15:43:21.000000 noisebase-1.0/LICENSE
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       39 2024-04-02 13:47:26.000000 noisebase-1.0/MANIFEST.in
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5620 2024-04-12 09:42:22.000000 noisebase-1.0/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4821 2024-04-09 15:43:21.000000 noisebase-1.0/README.md
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.462148 noisebase-1.0/noisebase/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2413 2024-04-12 09:32:38.000000 noisebase-1.0/noisebase/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2239 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/compression.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.354148 noisebase-1.0/noisebase/conf/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.566148 noisebase-1.0/noisebase/conf/noisebase/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.586148 noisebase-1.0/noisebase/conf/noisebase/format/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      427 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/conf/noisebase/format/test_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      634 2024-04-04 01:01:46.000000 noisebase-1.0/noisebase/conf/noisebase/format/training_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      800 2024-04-02 16:37:47.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_test32_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      879 2024-04-02 15:53:00.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_test8_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      385 2024-04-02 16:37:54.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     3028 2024-04-03 14:40:25.000000 noisebase-1.0/noisebase/data.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.610148 noisebase-1.0/noisebase/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       45 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1805 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/lightning/midepoch_ckpt.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.626148 noisebase-1.0/noisebase/loaders/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:20.000000 noisebase-1.0/noisebase/loaders/__init__.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.650148 noisebase-1.0/noisebase/loaders/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       55 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/loaders/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      776 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/loaders/lightning/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.710147 noisebase-1.0/noisebase/loaders/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      103 2024-04-01 20:01:43.000000 noisebase-1.0/noisebase/loaders/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9728 2024-04-02 16:02:24.000000 noisebase-1.0/noisebase/loaders/torch/test_sample_v1.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9202 2024-04-04 01:02:35.000000 noisebase-1.0/noisebase/loaders/torch/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.750147 noisebase-1.0/noisebase/metrics/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:31.000000 noisebase-1.0/noisebase/metrics/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    29927 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/metrics/flip.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4815 2024-04-04 20:16:47.000000 noisebase-1.0/noisebase/metrics/fvvdp.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     8026 2024-04-01 20:01:41.000000 noisebase-1.0/noisebase/projective.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.810147 noisebase-1.0/noisebase/scripts/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      213 2024-04-02 15:32:45.000000 noisebase-1.0/noisebase/scripts/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5116 2024-04-02 17:19:45.000000 noisebase-1.0/noisebase/scripts/nb_compute_metrics.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      763 2024-04-02 14:22:09.000000 noisebase-1.0/noisebase/scripts/nb_download.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2012 2024-04-05 00:45:54.000000 noisebase-1.0/noisebase/scripts/nb_result_table.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      486 2024-04-02 17:20:49.000000 noisebase-1.0/noisebase/scripts/nb_save_reference.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.850147 noisebase-1.0/noisebase/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       85 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1059 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/misc.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1631 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/projective.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5641 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/video_sampler.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.530148 noisebase-1.0/noisebase.egg-info/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5620 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1283 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        1 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      228 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/entry_points.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/requires.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       10 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/top_level.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1061 2024-04-12 09:30:32.000000 noisebase-1.0/pyproject.toml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      133 2024-04-12 09:42:22.000000 noisebase-1.0/setup.cfg
```

### Comparing `noisebase-0.0.1/pyproject.toml` & `noisebase-1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,38 @@
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["version"]
 name = "noisebase"
 description = "Datasets and benchmarks for neural Monte Carlo denoising"
+dependencies = [
+  "torch",
+  "pyfvvdp==1.2.0",
+  "zarr>=2",
+  "pytorch-msssim",
+  "hydra-core",
+  "requests",
+  "tqdm"
+]
 authors = [{name = "Martin Bálint", email = "martin@balint.io"}]
 readme = "README.md"
 keywords = ["denoising", "Monte Carlo", "MC", "neural"]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: Apache Software License",
 
     "Environment :: GPU",
     "Operating System :: OS Independent",
 
     "Programming Language :: Python :: 3",
 ]
 
+[project.scripts]
+nb-save-reference = "noisebase:scripts.nb_save_reference"
+nb-compute-metrics = "noisebase:scripts.nb_compute_metrics"
+nb-result-table = "noisebase:scripts.nb_result_table"
+nb-download = "noisebase:scripts.nb_download"
+
 [project.urls]
 Documentation = "https://balint.io/noisebase"
 Repository = "https://github.com/balintio/noisebase.git"
```

