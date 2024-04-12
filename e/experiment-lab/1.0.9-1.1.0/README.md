# Comparing `tmp/experiment-lab-1.0.9.tar.gz` & `tmp/experiment-lab-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experiment-lab-1.0.9.tar", last modified: Wed Apr 10 14:43:13 2024, max compression
+gzip compressed data, was "experiment-lab-1.1.0.tar", last modified: Fri Apr 12 04:43:36 2024, max compression
```

## Comparing `experiment-lab-1.0.9.tar` & `experiment-lab-1.1.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.945220 experiment-lab-1.0.9/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.0.9/LICENCE
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/MANIFEST.in
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-10 14:43:13.945040 experiment-lab-1.0.9/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/README.md
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.938050 experiment-lab-1.0.9/experiment_lab/
--rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-10 14:42:30.000000 experiment-lab-1.0.9/experiment_lab/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.938931 experiment-lab-1.0.9/experiment_lab/common/
--rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/common/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.939379 experiment-lab-1.0.9/experiment_lab/common/networks/
--rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/common/networks/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.0.9/experiment_lab/common/networks/blocks.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/common/networks/mlp.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6734 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/common/networks/network.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.939751 experiment-lab-1.0.9/experiment_lab/common/resolvers/
--rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/common/resolvers/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/common/resolvers/list_resolvers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/common/resolvers/object_resolvers.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.939889 experiment-lab-1.0.9/experiment_lab/common/utils/
--rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.0.9/experiment_lab/common/utils/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.940009 experiment-lab-1.0.9/experiment_lab/configs/
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.940115 experiment-lab-1.0.9/experiment_lab/configs/__pycache__/
--rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.0.9/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/config.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.940397 experiment-lab-1.0.9/experiment_lab/configs/mc/
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/mc/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/mc/estimate_pi.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.940992 experiment-lab-1.0.9/experiment_lab/configs/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/rl/atari.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      472 2024-04-10 14:31:57.000000 experiment-lab-1.0.9/experiment_lab/configs/rl/cartpole.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/rl/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/rl/crossing.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/rl/walker.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.941231 experiment-lab-1.0.9/experiment_lab/configs/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/supervised/config.yaml
--rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/configs/supervised/fashion_mnist.yaml
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.941786 experiment-lab-1.0.9/experiment_lab/core/
--rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-09 22:37:45.000000 experiment-lab-1.0.9/experiment_lab/core/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3777 2024-04-10 14:42:49.000000 experiment-lab-1.0.9/experiment_lab/core/base_analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1285 2024-04-10 14:31:57.000000 experiment-lab-1.0.9/experiment_lab/core/base_config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.0.9/experiment_lab/core/base_experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.0.9/experiment_lab/core/runner.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.941895 experiment-lab-1.0.9/experiment_lab/experiments/
--rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.0.9/experiment_lab/experiments/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.942186 experiment-lab-1.0.9/experiment_lab/experiments/examples/
--rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/experiments/examples/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/examples/mc_pi_estimate.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/experiments/examples/random_waits.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.942584 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/
--rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/__init__.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.943114 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/
--rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/aggregators.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/post_processors.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/sample_filters.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/samplers.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.943833 experiment-lab-1.0.9/experiment_lab/experiments/rl/
--rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/analysis.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)    10429 2024-03-24 16:11:49.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/environment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.0.9/experiment_lab/experiments/rl/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.944336 experiment-lab-1.0.9/experiment_lab/experiments/supervised/
--rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/experiments/supervised/__init__.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.0.9/experiment_lab/experiments/supervised/config.py
--rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.0.9/experiment_lab/experiments/supervised/experiment.py
--rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/experiment_lab/experiments/supervised/main.py
-drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-10 14:43:13.944485 experiment-lab-1.0.9/experiment_lab.egg-info/
--rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/PKG-INFO
--rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/SOURCES.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/dependency_links.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/entry_points.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/requires.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-10 14:43:13.000000 experiment-lab-1.0.9/experiment_lab.egg-info/top_level.txt
--rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.0.9/pyproject.toml
--rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-10 14:43:13.945252 experiment-lab-1.0.9/setup.cfg
--rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.0.9/setup.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.995277 experiment-lab-1.1.0/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1066 2024-03-01 07:08:11.000000 experiment-lab-1.1.0/LICENCE
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/MANIFEST.in
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-12 04:43:36.995080 experiment-lab-1.1.0/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2763 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/README.md
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.986799 experiment-lab-1.1.0/experiment_lab/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       75 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.987644 experiment-lab-1.1.0/experiment_lab/common/
+-rw-r--r--   0 rbhagat    (501) staff       (20)        0 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/common/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988016 experiment-lab-1.1.0/experiment_lab/common/networks/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      240 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/networks/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1773 2024-03-11 20:50:57.000000 experiment-lab-1.1.0/experiment_lab/common/networks/blocks.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1820 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/networks/mlp.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6764 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/common/networks/network.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988306 experiment-lab-1.1.0/experiment_lab/common/resolvers/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      682 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1708 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/list_resolvers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/common/resolvers/object_resolvers.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988394 experiment-lab-1.1.0/experiment_lab/common/utils/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1548 2024-03-11 19:31:56.000000 experiment-lab-1.1.0/experiment_lab/common/utils/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988481 experiment-lab-1.1.0/experiment_lab/configs/
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.988726 experiment-lab-1.1.0/experiment_lab/configs/__pycache__/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      181 2024-03-02 18:58:05.000000 experiment-lab-1.1.0/experiment_lab/configs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 rbhagat    (501) staff       (20)       40 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/config.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.989216 experiment-lab-1.1.0/experiment_lab/configs/mc/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/mc/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      750 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/mc/estimate_pi.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.990420 experiment-lab-1.1.0/experiment_lab/configs/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      423 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/atari.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      472 2024-04-10 14:31:57.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/cartpole.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       39 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      503 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/crossing.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)      534 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/rl/walker.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991245 experiment-lab-1.1.0/experiment_lab/configs/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       42 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/supervised/config.yaml
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2478 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/configs/supervised/fashion_mnist.yaml
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991809 experiment-lab-1.1.0/experiment_lab/core/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      265 2024-04-09 22:37:45.000000 experiment-lab-1.1.0/experiment_lab/core/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5398 2024-04-10 16:31:44.000000 experiment-lab-1.1.0/experiment_lab/core/base_analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-04-10 16:31:44.000000 experiment-lab-1.1.0/experiment_lab/core/base_config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     5645 2024-04-07 19:18:36.000000 experiment-lab-1.1.0/experiment_lab/core/base_experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2299 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/core/runner.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.991921 experiment-lab-1.1.0/experiment_lab/experiments/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       44 2024-03-04 14:43:06.000000 experiment-lab-1.1.0/experiment_lab/experiments/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.992227 experiment-lab-1.1.0/experiment_lab/experiments/examples/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       36 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1767 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/mc_pi_estimate.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1371 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/examples/random_waits.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.992624 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      120 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/__init__.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.993161 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      563 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2328 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/aggregators.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1103 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/post_processors.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1062 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/sample_filters.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1902 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/samplers.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1638 2024-04-03 18:52:52.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3212 2024-04-03 18:52:52.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      575 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.993779 experiment-lab-1.1.0/experiment_lab/experiments/rl/
+-rw-r--r--   0 rbhagat    (501) staff       (20)      255 2024-03-11 14:00:07.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1421 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/analysis.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1852 2024-03-13 20:27:53.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)    10546 2024-04-12 04:43:06.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/environment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     6267 2024-03-24 16:11:49.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      656 2024-04-09 22:28:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/rl/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.994278 experiment-lab-1.1.0/experiment_lab/experiments/supervised/
+-rw-r--r--   0 rbhagat    (501) staff       (20)       63 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/__init__.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3436 2024-03-12 21:19:35.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/config.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)     8526 2024-03-13 13:55:28.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/experiment.py
+-rw-r--r--   0 rbhagat    (501) staff       (20)      641 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/experiment_lab/experiments/supervised/main.py
+drwxr-xr-x   0 rbhagat    (501) staff       (20)        0 2024-04-12 04:43:36.994482 experiment-lab-1.1.0/experiment_lab.egg-info/
+-rw-r--r--   0 rbhagat    (501) staff       (20)     3949 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/PKG-INFO
+-rw-r--r--   0 rbhagat    (501) staff       (20)     2501 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/SOURCES.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)        1 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/dependency_links.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      237 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/entry_points.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)      223 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/requires.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)       15 2024-04-12 04:43:36.000000 experiment-lab-1.1.0/experiment_lab.egg-info/top_level.txt
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1200 2024-03-23 19:11:29.000000 experiment-lab-1.1.0/pyproject.toml
+-rw-r--r--   0 rbhagat    (501) staff       (20)       38 2024-04-12 04:43:36.995312 experiment-lab-1.1.0/setup.cfg
+-rw-r--r--   0 rbhagat    (501) staff       (20)     1030 2024-03-03 02:11:13.000000 experiment-lab-1.1.0/setup.py
```

### Comparing `experiment-lab-1.0.9/LICENCE` & `experiment-lab-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/PKG-INFO` & `experiment-lab-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.9
+Version: 1.1.0
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.9/README.md` & `experiment-lab-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/common/networks/blocks.py` & `experiment-lab-1.1.0/experiment_lab/common/networks/blocks.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/common/networks/mlp.py` & `experiment-lab-1.1.0/experiment_lab/common/networks/mlp.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/common/networks/network.py` & `experiment-lab-1.1.0/experiment_lab/common/networks/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
         Args:
             module_lst (Sequence[nn.Module]): The list of modules to apply before aggregation.
             aggregator (Callable[[torch.Tensor, torch.Tensor], torch.Tensor]): The aggregator to use on the tensors.
             output_module (nn.Module): The module to apply after aggregation.
         """
         super().__init__()
-        self.module_lst = module_lst
+        self.module_lst = nn.ModuleList(module_lst)
         self.aggregator = aggregator
         self.output_module = output_module
 
     def forward(self, xs: Sequence[torch.Tensor]) -> torch.Tensor:
         """The forward function of the aggregated network.
 
         Args:
@@ -129,15 +129,15 @@
 
         Args:
             input_module (nn.Module): The module to apply on the input.
             module_lst (Sequence[nn.Module]): The modules to apply after input_module has been applied.
         """
         super().__init__()
         self.input_module = input_module
-        self.module_lst = module_lst
+        self.module_lst = nn.ModuleList(module_lst)
 
     def forward(self, x: torch.Tensor) -> Sequence[torch.Tensor]:
         """The forward function of the multi output network
 
         Args:
             x (torch.Tensor): The input tensor.
```

### Comparing `experiment-lab-1.0.9/experiment_lab/common/resolvers/__init__.py` & `experiment-lab-1.1.0/experiment_lab/common/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/common/resolvers/list_resolvers.py` & `experiment-lab-1.1.0/experiment_lab/common/resolvers/list_resolvers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/common/utils/__init__.py` & `experiment-lab-1.1.0/experiment_lab/common/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/configs/mc/estimate_pi.yaml` & `experiment-lab-1.1.0/experiment_lab/configs/mc/estimate_pi.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/configs/rl/walker.yaml` & `experiment-lab-1.1.0/experiment_lab/configs/rl/walker.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/configs/supervised/fashion_mnist.yaml` & `experiment-lab-1.1.0/experiment_lab/configs/supervised/fashion_mnist.yaml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/core/base_analysis.py` & `experiment-lab-1.1.0/experiment_lab/core/base_analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 """Helper functions to analyze the results of experiments."""
 
 import abc
+import json
 from textwrap import indent
 from typing import Any, Dict, Tuple
 import pandas as pd
+from torch import Value
 import wandb
 import tqdm
+from hydra.core.hydra_config import HydraConfig
 import logging
+from pathlib import Path
+import glob
 
 from experiment_lab.core.base_config import BaseConfig
 
 
 logger = logging.getLogger(__name__)
 
 api = None
@@ -40,74 +45,98 @@
         self.cfg = cfg
 
     def load_data(self) -> Tuple[pd.DataFrame, Dict[str, Dict[str, Any]]]:
         """Function to load the run data of an experiment.
 
         Raises:
             ValueError: If wandb config is not specified, raise a ValueError.
+            ValueError: If load_from_output_dir is set to true without any outputs to load, raise a ValueError.
 
         Returns:
             Tuple[pd.DataFrame, Dict[str, Dict[str, Any]]]: The dataframe containing all the run data and the dict containing all the configs.
         """
-        if self.cfg.wandb is None:
-            raise ValueError("Not wandb config specified")
-        api = get_api_instance()
-        wandb_runs = api.runs(
-            path=self.cfg.wandb["project"],
-            filters={
-                "$and": [
-                    {"state": "finished"},
-                    {"config.experiment_name": self.cfg.experiment_name},
-                ]
-                + self.cfg.analysis.filters,
-            },
-            include_sweeps=False,
-        )
-
-        full_df = []
-
-        configs = {}
-
-        for wandb_run in tqdm.tqdm(wandb_runs):
-            if self.cfg.analysis.all_keys_per_step:
-                df = pd.DataFrame(
-                    wandb_run.scan_history(keys=self.cfg.analysis.wandb_keys),
-                )
-            else:
-                df = pd.DataFrame()
-                for key in self.cfg.analysis.wandb_keys:
-                    temp_df = pd.DataFrame(
-                        wandb_run.scan_history(keys=[key]),
+        if not self.cfg.analysis.load_from_output_dir:
+            if self.cfg.wandb is None:
+                raise ValueError("Not wandb config specified")
+            api = get_api_instance()
+            wandb_runs = api.runs(
+                path=self.cfg.wandb["project"],
+                filters={
+                    "$and": [
+                        {"state": "finished"},
+                        {"config.experiment_name": self.cfg.experiment_name},
+                    ]
+                    + self.cfg.analysis.filters,
+                },
+                include_sweeps=False,
+            )
+
+            full_df = []
+
+            configs = {}
+
+            for wandb_run in tqdm.tqdm(wandb_runs):
+                if self.cfg.analysis.all_keys_per_step:
+                    df = pd.DataFrame(
+                        wandb_run.scan_history(keys=self.cfg.analysis.wandb_keys),
+                    )
+                else:
+                    df = pd.DataFrame()
+                    for key in self.cfg.analysis.wandb_keys:
+                        temp_df = pd.DataFrame(
+                            wandb_run.scan_history(keys=[key]),
+                        )
+                        df = pd.merge(
+                            df, temp_df, left_index=True, right_index=True, how="outer"
+                        )
+                df["experiment_id"] = wandb_run.config["experiment_id"]
+                df["run_id"] = wandb_run.id
+                if wandb_run.config["experiment_id"] not in configs:
+                    configs[wandb_run.config["experiment_id"]] = wandb_run.config
+                if self.cfg.analysis.index is not None:
+                    df.set_index(
+                        ["experiment_id", "run_id", self.cfg.analysis.index],
+                        inplace=True,
+                    )
+                else:
+                    df.set_index(["experiment_id", "run_id"], append=True, inplace=True)
+                    df = df.reorder_levels([1, 2, 0])
+
+                full_df.append(df)
+
+            full_df = pd.concat(full_df)
+            full_df.sort_index(inplace=True)
+        else:
+            if self.cfg.analysis.output_dir_to_load_from is None:
+                root_output_dir = Path(self.output_directory).parent.parent.absolute()
+                glob_results = sorted(glob.glob(f"{root_output_dir}/*/*/run_data.pkl"))
+                if len(glob_results) == 0:
+                    raise ValueError(
+                        "Cannot load results from output directory since there are no other analysis runs."
                     )
-                    df = pd.merge(df, temp_df, left_index=True, right_index=True, how='outer')
-            df["experiment_id"] = wandb_run.config["experiment_id"]
-            df["run_id"] = wandb_run.id
-            if wandb_run.config["experiment_id"] not in configs:
-                configs[wandb_run.config["experiment_id"]] = wandb_run.config
-            if self.cfg.analysis.index is not None:
-                df.set_index(
-                    ["experiment_id", "run_id", self.cfg.analysis.index], inplace=True
-                )
+                output_dir_to_load_from = Path(glob_results[-1]).parent
             else:
-                df.set_index(["experiment_id", "run_id"], append=True, inplace=True)
-                df = df.reorder_levels([1, 2, 0])
-
-            full_df.append(df)
-
-        full_df = pd.concat(full_df)
-        full_df.sort_index(inplace=True)
+                output_dir_to_load_from = self.cfg.analysis.output_dir_to_load_from
+            full_df = pd.read_pickle(f"{output_dir_to_load_from}/run_data.pkl")
+            with open(f"{output_dir_to_load_from}/configs.json", "r") as f:
+                configs = json.load(f)
+
+        full_df.to_pickle(f"{self.output_directory}/run_data.pkl")
+        with open(f"{self.output_directory}/configs.json", "w") as f:
+            json.dump(configs, f, indent=4)
 
         return full_df, configs
 
     def _analyze_wrapper(self) -> Any:
         """A wrapper for the analyze function.
 
         Returns:
             Any: The results of the analysis.
         """
+        self.output_directory = HydraConfig.get().runtime.output_dir
         df, configs = self.load_data()
         results = self.analyze(df=df, configs=configs)
         logger.info(results)
         return results
 
     @abc.abstractmethod
     def analyze(self, df: pd.DataFrame, configs: Dict[str, Dict[str, Any]]) -> Any:
```

### Comparing `experiment-lab-1.0.9/experiment_lab/core/base_config.py` & `experiment-lab-1.1.0/experiment_lab/core/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 class AnalysisConfig:
     """Config for analysis of this experiment."""
 
     filters: List[Dict] = field(default_factory=lambda: [])
     wandb_keys: List[str] = field(default_factory=lambda: [])
     index: str | None = None
     all_keys_per_step: bool = False
+    load_from_output_dir: bool = False
+    output_dir_to_load_from: str | None = None
 
 
 @dataclass
 class BaseConfig:
     """Basic configuration for general experiment runs."""
 
     experiment_name: str | None = None
```

### Comparing `experiment-lab-1.0.9/experiment_lab/core/base_experiment.py` & `experiment-lab-1.1.0/experiment_lab/core/base_experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/core/runner.py` & `experiment-lab-1.1.0/experiment_lab/core/runner.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/examples/mc_pi_estimate.py` & `experiment-lab-1.1.0/experiment_lab/experiments/examples/mc_pi_estimate.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/examples/random_waits.py` & `experiment-lab-1.1.0/experiment_lab/experiments/examples/random_waits.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/__init__.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/__init__.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/aggregators.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/aggregators.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/post_processors.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/post_processors.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/sample_filters.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/sample_filters.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/components/samplers.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/components/samplers.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/config.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/experiment.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/monte_carlo/main.py` & `experiment-lab-1.1.0/experiment_lab/experiments/monte_carlo/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/rl/analysis.py` & `experiment-lab-1.1.0/experiment_lab/experiments/rl/analysis.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/rl/config.py` & `experiment-lab-1.1.0/experiment_lab/experiments/rl/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/rl/environment.py` & `experiment-lab-1.1.0/experiment_lab/experiments/rl/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,16 @@
             return _init
 
         env_fns = [make_env_fn(rank=i) for i in range(n_envs)]
 
         if start_method is None:
             start_method = "spawn" if "spawn" in mp.get_all_start_methods() else None
 
+        self.eval_env: ListEnv = make_env_fn(rank=n_envs)() # type: ignore
+
         super().__init__(env_fns=env_fns, start_method=start_method)
 
     def step_wait(self) -> VecEnvStepReturn:
         """Waits for the results of the step call and incremenets the environment idx if needed.
 
         Returns:
             VecEnvStepReturn: The step return.
@@ -285,12 +287,13 @@
             self.cur_env_idx < len(self.transfer_steps)
             and self.total_time_steps - self.last_incr
             > self.transfer_steps[self.cur_env_idx]
         ):
             self.last_incr = self.total_time_steps
             # Trigger the novelty if enough steps have passed
             transfer_injected: List[bool] = self.env_method("incr_env_idx")
+            self.eval_env.incr_env_idx()
             if np.any(transfer_injected):
                 self.cur_env_idx += 1
                 dones[:] = True
 
         return observations, rewards, dones, infos
```

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/rl/experiment.py` & `experiment-lab-1.1.0/experiment_lab/experiments/rl/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/rl/main.py` & `experiment-lab-1.1.0/experiment_lab/experiments/rl/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/supervised/config.py` & `experiment-lab-1.1.0/experiment_lab/experiments/supervised/config.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/supervised/experiment.py` & `experiment-lab-1.1.0/experiment_lab/experiments/supervised/experiment.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab/experiments/supervised/main.py` & `experiment-lab-1.1.0/experiment_lab/experiments/supervised/main.py`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/experiment_lab.egg-info/PKG-INFO` & `experiment-lab-1.1.0/experiment_lab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experiment-lab
-Version: 1.0.9
+Version: 1.1.0
 Summary: A suite of flexible experiments of a variety of different tasks.
 Author-email: Rishav Bhagat <rishavbhagat.cs@gmail.com>
 Project-URL: Repository, https://github.com/rishavb123/ExperimentLab
 Keywords: experiment,suite,lab
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `experiment-lab-1.0.9/experiment_lab.egg-info/SOURCES.txt` & `experiment-lab-1.1.0/experiment_lab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/pyproject.toml` & `experiment-lab-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `experiment-lab-1.0.9/setup.py` & `experiment-lab-1.1.0/setup.py`

 * *Files identical despite different names*

