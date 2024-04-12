# Comparing `tmp/noisebase-1.0.tar.gz` & `tmp/noisebase-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noisebase-1.0.tar", last modified: Fri Apr 12 09:42:22 2024, max compression
+gzip compressed data, was "noisebase-1.1.tar", last modified: Fri Apr 12 10:02:29 2024, max compression
```

## Comparing `noisebase-1.0.tar` & `noisebase-1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.866147 noisebase-1.0/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)    11344 2024-04-09 15:43:21.000000 noisebase-1.0/LICENSE
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       39 2024-04-02 13:47:26.000000 noisebase-1.0/MANIFEST.in
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5620 2024-04-12 09:42:22.000000 noisebase-1.0/PKG-INFO
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     4821 2024-04-09 15:43:21.000000 noisebase-1.0/README.md
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.462148 noisebase-1.0/noisebase/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2413 2024-04-12 09:32:38.000000 noisebase-1.0/noisebase/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2239 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/compression.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.354148 noisebase-1.0/noisebase/conf/
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.566148 noisebase-1.0/noisebase/conf/noisebase/
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.586148 noisebase-1.0/noisebase/conf/noisebase/format/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      427 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/conf/noisebase/format/test_sample_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      634 2024-04-04 01:01:46.000000 noisebase-1.0/noisebase/conf/noisebase/format/training_sample_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      800 2024-04-02 16:37:47.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_test32_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      879 2024-04-02 15:53:00.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_test8_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      385 2024-04-02 16:37:54.000000 noisebase-1.0/noisebase/conf/noisebase/sampleset_v1.yaml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     3028 2024-04-03 14:40:25.000000 noisebase-1.0/noisebase/data.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.610148 noisebase-1.0/noisebase/lightning/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       45 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/lightning/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1805 2024-04-01 20:01:42.000000 noisebase-1.0/noisebase/lightning/midepoch_ckpt.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.626148 noisebase-1.0/noisebase/loaders/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:20.000000 noisebase-1.0/noisebase/loaders/__init__.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.650148 noisebase-1.0/noisebase/loaders/lightning/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       55 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/loaders/lightning/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      776 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/loaders/lightning/training_sample_v1.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.710147 noisebase-1.0/noisebase/loaders/torch/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      103 2024-04-01 20:01:43.000000 noisebase-1.0/noisebase/loaders/torch/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     9728 2024-04-02 16:02:24.000000 noisebase-1.0/noisebase/loaders/torch/test_sample_v1.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     9202 2024-04-04 01:02:35.000000 noisebase-1.0/noisebase/loaders/torch/training_sample_v1.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.750147 noisebase-1.0/noisebase/metrics/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:31.000000 noisebase-1.0/noisebase/metrics/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)    29927 2024-04-01 20:01:44.000000 noisebase-1.0/noisebase/metrics/flip.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     4815 2024-04-04 20:16:47.000000 noisebase-1.0/noisebase/metrics/fvvdp.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     8026 2024-04-01 20:01:41.000000 noisebase-1.0/noisebase/projective.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.810147 noisebase-1.0/noisebase/scripts/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      213 2024-04-02 15:32:45.000000 noisebase-1.0/noisebase/scripts/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5116 2024-04-02 17:19:45.000000 noisebase-1.0/noisebase/scripts/nb_compute_metrics.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      763 2024-04-02 14:22:09.000000 noisebase-1.0/noisebase/scripts/nb_download.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     2012 2024-04-05 00:45:54.000000 noisebase-1.0/noisebase/scripts/nb_result_table.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      486 2024-04-02 17:20:49.000000 noisebase-1.0/noisebase/scripts/nb_save_reference.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.850147 noisebase-1.0/noisebase/torch/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       85 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/__init__.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1059 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/misc.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1631 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/projective.py
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5641 2024-04-01 20:01:45.000000 noisebase-1.0/noisebase/torch/video_sampler.py
-drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 09:42:22.530148 noisebase-1.0/noisebase.egg-info/
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     5620 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/PKG-INFO
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1283 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/SOURCES.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)        1 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/dependency_links.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      228 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/entry_points.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/requires.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)       10 2024-04-12 09:42:22.000000 noisebase-1.0/noisebase.egg-info/top_level.txt
--rw-r--r--   0 mbalint  (23702) seidel    (4000)     1061 2024-04-12 09:30:32.000000 noisebase-1.0/pyproject.toml
--rw-r--r--   0 mbalint  (23702) seidel    (4000)      133 2024-04-12 09:42:22.000000 noisebase-1.0/setup.cfg
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.174639 noisebase-1.1/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    11344 2024-04-09 15:43:21.000000 noisebase-1.1/LICENSE
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       39 2024-04-02 13:47:26.000000 noisebase-1.1/MANIFEST.in
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5792 2024-04-12 10:02:29.000000 noisebase-1.1/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4993 2024-04-12 09:55:08.000000 noisebase-1.1/README.md
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.810640 noisebase-1.1/noisebase/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2413 2024-04-12 10:02:10.000000 noisebase-1.1/noisebase/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2239 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/compression.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.690640 noisebase-1.1/noisebase/conf/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.934640 noisebase-1.1/noisebase/conf/noisebase/
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.962640 noisebase-1.1/noisebase/conf/noisebase/format/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      427 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/conf/noisebase/format/test_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      634 2024-04-04 01:01:46.000000 noisebase-1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      800 2024-04-02 16:37:47.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      879 2024-04-02 15:53:00.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      385 2024-04-02 16:37:54.000000 noisebase-1.1/noisebase/conf/noisebase/sampleset_v1.yaml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     3028 2024-04-03 14:40:25.000000 noisebase-1.1/noisebase/data.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.986640 noisebase-1.1/noisebase/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       45 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1805 2024-04-01 20:01:42.000000 noisebase-1.1/noisebase/lightning/midepoch_ckpt.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.994639 noisebase-1.1/noisebase/loaders/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:20.000000 noisebase-1.1/noisebase/loaders/__init__.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.018639 noisebase-1.1/noisebase/loaders/lightning/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       55 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/loaders/lightning/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      776 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/loaders/lightning/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.046639 noisebase-1.1/noisebase/loaders/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      103 2024-04-01 20:01:43.000000 noisebase-1.1/noisebase/loaders/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9728 2024-04-02 16:02:24.000000 noisebase-1.1/noisebase/loaders/torch/test_sample_v1.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     9202 2024-04-04 01:02:35.000000 noisebase-1.1/noisebase/loaders/torch/training_sample_v1.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.074639 noisebase-1.1/noisebase/metrics/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        0 2024-04-02 14:02:31.000000 noisebase-1.1/noisebase/metrics/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)    29927 2024-04-01 20:01:44.000000 noisebase-1.1/noisebase/metrics/flip.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     4815 2024-04-04 20:16:47.000000 noisebase-1.1/noisebase/metrics/fvvdp.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     8026 2024-04-01 20:01:41.000000 noisebase-1.1/noisebase/projective.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.118639 noisebase-1.1/noisebase/scripts/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      213 2024-04-02 15:32:45.000000 noisebase-1.1/noisebase/scripts/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5116 2024-04-02 17:19:45.000000 noisebase-1.1/noisebase/scripts/nb_compute_metrics.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      763 2024-04-02 14:22:09.000000 noisebase-1.1/noisebase/scripts/nb_download.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     2012 2024-04-05 00:45:54.000000 noisebase-1.1/noisebase/scripts/nb_result_table.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      486 2024-04-02 17:20:49.000000 noisebase-1.1/noisebase/scripts/nb_save_reference.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:29.158639 noisebase-1.1/noisebase/torch/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       85 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/__init__.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1059 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/misc.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1631 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/projective.py
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5641 2024-04-01 20:01:45.000000 noisebase-1.1/noisebase/torch/video_sampler.py
+drwxr-xr-x   0 mbalint  (23702) seidel    (4000)        0 2024-04-12 10:02:28.874640 noisebase-1.1/noisebase.egg-info/
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     5792 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/PKG-INFO
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1283 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)        1 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      228 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/entry_points.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       69 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/requires.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)       10 2024-04-12 10:02:28.000000 noisebase-1.1/noisebase.egg-info/top_level.txt
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)     1061 2024-04-12 09:30:32.000000 noisebase-1.1/pyproject.toml
+-rw-r--r--   0 mbalint  (23702) seidel    (4000)      133 2024-04-12 10:02:29.000000 noisebase-1.1/setup.cfg
```

### Comparing `noisebase-1.0/LICENSE` & `noisebase-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/PKG-INFO` & `noisebase-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisebase
-Version: 1.0
+Version: 1.1
 Summary: Datasets and benchmarks for neural Monte Carlo denoising
 Author-email: Martin Bálint <martin@balint.io>
 Project-URL: Documentation, https://balint.io/noisebase
 Project-URL: Repository, https://github.com/balintio/noisebase.git
 Keywords: denoising,Monte Carlo,MC,neural
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Requires-Dist: zarr>=2
 Requires-Dist: pytorch-msssim
 Requires-Dist: hydra-core
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 <p align="center">
-  <img src="docs/_static/logo-01.png" width="100%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png" width="100%">
 </p>
 
 <div align="center">
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Version](https://img.shields.io/pypi/v/noisebase)](https://pypi.org/project/noisebase/)
 [![GitHub Repo stars](https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/balintio/noisebase)
@@ -36,23 +36,24 @@
 <p align="center">
 <a href="https://balint.io/noisebase/news.html">News</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/benchmarks/index.html">Benchmarks</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/datasets/index.html">Datasets</a>
 </p>
 
 **Datasets and benchmarks for neural Monte Carlo denoising.**
 
 <p align="center">
-  <img src="docs/_static/teaser.png" width="70%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png" width="70%">
 </p>
 
-
+What is Monte Carlo denoising?
+------------------------------
 <details>
-<summary><h2>What is Monte Carlo denoising?</h2></summary>
+<summary>Read More</summary>
 
 <div align="center">
-  <img src="docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
   <p>Monte Carlo integration <a href="https://commons.wikimedia.org/w/index.php?curid=140013480"><b>Kmhkmh</b></a></p>
 </div>
 
 Monte Carlo methods approximate integrals by sampling random points from the function's domain, evaluating the function, and averaging the resulting samples. We mainly focus on *light transport simulation* as it's a complex and mature application, usually producing visual and intuitive results. In this case, our samples are light paths that a "photon" might take. Above on the right, you see an image rendered with 4 samples per pixel. It's quite noisy.
 
 With a bit of napkin maths, we can estimate that rendering a relatively noise-free 4K image requires tens of billions of samples while rendering a two-hour movie requires quadrillions of samples. Astonishingly, we have data centres fit for this task. Not only do they consume electricity on par with a small town, but such computational requirements put creating 3D art outside the reach of many.
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: noisebase Version: 1.0 Summary: Datasets and
+Metadata-Version: 2.1 Name: noisebase Version: 1.1 Summary: Datasets and
 benchmarks for neural Monte Carlo denoising Author-email: Martin BÃ¡lint
 balint.io> Project-URL: Documentation, https://balint.io/noisebase Project-URL:
 Repository, https://github.com/balintio/noisebase.git Keywords: denoising,Monte
 Carlo,MC,neural Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Environment :: GPU
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: torch Requires-Dist: pyfvvdp==1.2.0 Requires-Dist: zarr>=2
 Requires-Dist: pytorch-msssim Requires-Dist: hydra-core Requires-Dist: requests
 Requires-Dist: tqdm
-                          [docs/_static/logo-01.png]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png]
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) [![PyPI - Version](https://img.shields.io/
  pypi/v/noisebase)](https://pypi.org/project/noisebase/) [![GitHub Repo stars]
  (https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/
                               balintio/noisebase)
                        _N_e_w_s  |  _B_e_n_c_h_m_a_r_k_s  |  _D_a_t_a_s_e_t_s
 **Datasets and benchmarks for neural Monte Carlo denoising.**
-                           [docs/_static/teaser.png]
-********** WWhhaatt iiss MMoonnttee CCaarrlloo ddeennooiissiinngg?? **********
-                     [docs/_static/Pi_monte_carlo_all.gif]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png]
+What is Monte Carlo denoising? ------------------------------ Read More
+         [https://github.com/balintio/noisebase/raw/main/docs/_static/
+                            Pi_monte_carlo_all.gif]
                         Monte Carlo integration _KK_mm_hh_kk_mm_hh
 Monte Carlo methods approximate integrals by sampling random points from the
 function's domain, evaluating the function, and averaging the resulting
 samples. We mainly focus on *light transport simulation* as it's a complex and
 mature application, usually producing visual and intuitive results. In this
 case, our samples are light paths that a "photon" might take. Above on the
 right, you see an image rendered with 4 samples per pixel. It's quite noisy.
```

### Comparing `noisebase-1.0/README.md` & `noisebase-1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="docs/_static/logo-01.png" width="100%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png" width="100%">
 </p>
 
 <div align="center">
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Version](https://img.shields.io/pypi/v/noisebase)](https://pypi.org/project/noisebase/)
 [![GitHub Repo stars](https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/balintio/noisebase)
@@ -13,23 +13,24 @@
 <p align="center">
 <a href="https://balint.io/noisebase/news.html">News</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/benchmarks/index.html">Benchmarks</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/datasets/index.html">Datasets</a>
 </p>
 
 **Datasets and benchmarks for neural Monte Carlo denoising.**
 
 <p align="center">
-  <img src="docs/_static/teaser.png" width="70%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png" width="70%">
 </p>
 
-
+What is Monte Carlo denoising?
+------------------------------
 <details>
-<summary><h2>What is Monte Carlo denoising?</h2></summary>
+<summary>Read More</summary>
 
 <div align="center">
-  <img src="docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
   <p>Monte Carlo integration <a href="https://commons.wikimedia.org/w/index.php?curid=140013480"><b>Kmhkmh</b></a></p>
 </div>
 
 Monte Carlo methods approximate integrals by sampling random points from the function's domain, evaluating the function, and averaging the resulting samples. We mainly focus on *light transport simulation* as it's a complex and mature application, usually producing visual and intuitive results. In this case, our samples are light paths that a "photon" might take. Above on the right, you see an image rendered with 4 samples per pixel. It's quite noisy.
 
 With a bit of napkin maths, we can estimate that rendering a relatively noise-free 4K image requires tens of billions of samples while rendering a two-hour movie requires quadrillions of samples. Astonishingly, we have data centres fit for this task. Not only do they consume electricity on par with a small town, but such computational requirements put creating 3D art outside the reach of many.
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-                          [docs/_static/logo-01.png]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png]
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) [![PyPI - Version](https://img.shields.io/
  pypi/v/noisebase)](https://pypi.org/project/noisebase/) [![GitHub Repo stars]
  (https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/
                               balintio/noisebase)
                        _N_e_w_s  |  _B_e_n_c_h_m_a_r_k_s  |  _D_a_t_a_s_e_t_s
 **Datasets and benchmarks for neural Monte Carlo denoising.**
-                           [docs/_static/teaser.png]
-********** WWhhaatt iiss MMoonnttee CCaarrlloo ddeennooiissiinngg?? **********
-                     [docs/_static/Pi_monte_carlo_all.gif]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png]
+What is Monte Carlo denoising? ------------------------------ Read More
+         [https://github.com/balintio/noisebase/raw/main/docs/_static/
+                            Pi_monte_carlo_all.gif]
                         Monte Carlo integration _KK_mm_hh_kk_mm_hh
 Monte Carlo methods approximate integrals by sampling random points from the
 function's domain, evaluating the function, and averaging the resulting
 samples. We mainly focus on *light transport simulation* as it's a complex and
 mature application, usually producing visual and intuitive results. In this
 case, our samples are light paths that a "photon" might take. Above on the
 right, you see an image rendered with 4 samples per pixel. It's quite noisy.
```

### Comparing `noisebase-1.0/noisebase/__init__.py` & `noisebase-1.1/noisebase/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Datasets and benchmarks for neural Monte Carlo denoising.
 
 This file serves as the main entry point for Noisebase. It registers all 
 Noisebase config files in your Hydra path and, in addition, provides a 
 `Noisebase` function should you wish to keep your use of Hydra to a minimum.
 """
 
-__version__ = '1.0'
+__version__ = '1.1'
 
 import os
 
 from hydra.plugins.search_path_plugin import SearchPathPlugin
 from hydra.core.plugins import Plugins
 
 class NoisebaseSearchPathPlugin(SearchPathPlugin):
```

### Comparing `noisebase-1.0/noisebase/compression.py` & `noisebase-1.1/noisebase/compression.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/conf/noisebase/format/training_sample_v1.yaml` & `noisebase-1.1/noisebase/conf/noisebase/format/training_sample_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/conf/noisebase/sampleset_test32_v1.yaml` & `noisebase-1.1/noisebase/conf/noisebase/sampleset_test32_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/conf/noisebase/sampleset_test8_v1.yaml` & `noisebase-1.1/noisebase/conf/noisebase/sampleset_test8_v1.yaml`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/data.py` & `noisebase-1.1/noisebase/data.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/lightning/midepoch_ckpt.py` & `noisebase-1.1/noisebase/lightning/midepoch_ckpt.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/loaders/lightning/training_sample_v1.py` & `noisebase-1.1/noisebase/loaders/lightning/training_sample_v1.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/loaders/torch/test_sample_v1.py` & `noisebase-1.1/noisebase/loaders/torch/test_sample_v1.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/loaders/torch/training_sample_v1.py` & `noisebase-1.1/noisebase/loaders/torch/training_sample_v1.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/metrics/flip.py` & `noisebase-1.1/noisebase/metrics/flip.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/metrics/fvvdp.py` & `noisebase-1.1/noisebase/metrics/fvvdp.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/projective.py` & `noisebase-1.1/noisebase/projective.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/scripts/nb_compute_metrics.py` & `noisebase-1.1/noisebase/scripts/nb_compute_metrics.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/scripts/nb_download.py` & `noisebase-1.1/noisebase/scripts/nb_download.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/scripts/nb_result_table.py` & `noisebase-1.1/noisebase/scripts/nb_result_table.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/torch/misc.py` & `noisebase-1.1/noisebase/torch/misc.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/torch/projective.py` & `noisebase-1.1/noisebase/torch/projective.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase/torch/video_sampler.py` & `noisebase-1.1/noisebase/torch/video_sampler.py`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/noisebase.egg-info/PKG-INFO` & `noisebase-1.1/noisebase.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisebase
-Version: 1.0
+Version: 1.1
 Summary: Datasets and benchmarks for neural Monte Carlo denoising
 Author-email: Martin Bálint <martin@balint.io>
 Project-URL: Documentation, https://balint.io/noisebase
 Project-URL: Repository, https://github.com/balintio/noisebase.git
 Keywords: denoising,Monte Carlo,MC,neural
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,15 +18,15 @@
 Requires-Dist: zarr>=2
 Requires-Dist: pytorch-msssim
 Requires-Dist: hydra-core
 Requires-Dist: requests
 Requires-Dist: tqdm
 
 <p align="center">
-  <img src="docs/_static/logo-01.png" width="100%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png" width="100%">
 </p>
 
 <div align="center">
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![PyPI - Version](https://img.shields.io/pypi/v/noisebase)](https://pypi.org/project/noisebase/)
 [![GitHub Repo stars](https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/balintio/noisebase)
@@ -36,23 +36,24 @@
 <p align="center">
 <a href="https://balint.io/noisebase/news.html">News</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/benchmarks/index.html">Benchmarks</a> &emsp;|&emsp; <a href="https://balint.io/noisebase/datasets/index.html">Datasets</a>
 </p>
 
 **Datasets and benchmarks for neural Monte Carlo denoising.**
 
 <p align="center">
-  <img src="docs/_static/teaser.png" width="70%">
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png" width="70%">
 </p>
 
-
+What is Monte Carlo denoising?
+------------------------------
 <details>
-<summary><h2>What is Monte Carlo denoising?</h2></summary>
+<summary>Read More</summary>
 
 <div align="center">
-  <img src="docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
+  <img src="https://github.com/balintio/noisebase/raw/main/docs/_static/Pi_monte_carlo_all.gif" width="30%"> <br>
   <p>Monte Carlo integration <a href="https://commons.wikimedia.org/w/index.php?curid=140013480"><b>Kmhkmh</b></a></p>
 </div>
 
 Monte Carlo methods approximate integrals by sampling random points from the function's domain, evaluating the function, and averaging the resulting samples. We mainly focus on *light transport simulation* as it's a complex and mature application, usually producing visual and intuitive results. In this case, our samples are light paths that a "photon" might take. Above on the right, you see an image rendered with 4 samples per pixel. It's quite noisy.
 
 With a bit of napkin maths, we can estimate that rendering a relatively noise-free 4K image requires tens of billions of samples while rendering a two-hour movie requires quadrillions of samples. Astonishingly, we have data centres fit for this task. Not only do they consume electricity on par with a small town, but such computational requirements put creating 3D art outside the reach of many.
```

#### html2text {}

```diff
@@ -1,29 +1,30 @@
-Metadata-Version: 2.1 Name: noisebase Version: 1.0 Summary: Datasets and
+Metadata-Version: 2.1 Name: noisebase Version: 1.1 Summary: Datasets and
 benchmarks for neural Monte Carlo denoising Author-email: Martin BÃ¡lint
 balint.io> Project-URL: Documentation, https://balint.io/noisebase Project-URL:
 Repository, https://github.com/balintio/noisebase.git Keywords: denoising,Monte
 Carlo,MC,neural Classifier: Development Status :: 4 - Beta Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Environment :: GPU
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: torch Requires-Dist: pyfvvdp==1.2.0 Requires-Dist: zarr>=2
 Requires-Dist: pytorch-msssim Requires-Dist: hydra-core Requires-Dist: requests
 Requires-Dist: tqdm
-                          [docs/_static/logo-01.png]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/logo-01.png]
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://
 opensource.org/licenses/Apache-2.0) [![PyPI - Version](https://img.shields.io/
  pypi/v/noisebase)](https://pypi.org/project/noisebase/) [![GitHub Repo stars]
  (https://img.shields.io/github/stars/balintio/noisebase)](https://github.com/
                               balintio/noisebase)
                        _N_e_w_s  |  _B_e_n_c_h_m_a_r_k_s  |  _D_a_t_a_s_e_t_s
 **Datasets and benchmarks for neural Monte Carlo denoising.**
-                           [docs/_static/teaser.png]
-********** WWhhaatt iiss MMoonnttee CCaarrlloo ddeennooiissiinngg?? **********
-                     [docs/_static/Pi_monte_carlo_all.gif]
+   [https://github.com/balintio/noisebase/raw/main/docs/_static/teaser.png]
+What is Monte Carlo denoising? ------------------------------ Read More
+         [https://github.com/balintio/noisebase/raw/main/docs/_static/
+                            Pi_monte_carlo_all.gif]
                         Monte Carlo integration _KK_mm_hh_kk_mm_hh
 Monte Carlo methods approximate integrals by sampling random points from the
 function's domain, evaluating the function, and averaging the resulting
 samples. We mainly focus on *light transport simulation* as it's a complex and
 mature application, usually producing visual and intuitive results. In this
 case, our samples are light paths that a "photon" might take. Above on the
 right, you see an image rendered with 4 samples per pixel. It's quite noisy.
```

### Comparing `noisebase-1.0/noisebase.egg-info/SOURCES.txt` & `noisebase-1.1/noisebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noisebase-1.0/pyproject.toml` & `noisebase-1.1/pyproject.toml`

 * *Files identical despite different names*

