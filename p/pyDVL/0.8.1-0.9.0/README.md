# Comparing `tmp/pyDVL-0.8.1.tar.gz` & `tmp/pydvl-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDVL-0.8.1.tar", last modified: Fri Jan 26 09:48:19 2024, max compression
+gzip compressed data, was "pydvl-0.9.tar", last modified: Fri Apr 12 18:13:02 2024, max compression
```

## Comparing `pyDVL-0.8.1.tar` & `pydvl-0.9.tar`

### file list

```diff
@@ -1,95 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.600985 pyDVL-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-01-26 09:46:57.000000 pyDVL-0.8.1/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-26 09:46:57.000000 pyDVL-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-26 09:46:57.000000 pyDVL-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16995 2024-01-26 09:48:19.600985 pyDVL-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-01-26 09:46:57.000000 pyDVL-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     9828 2024-01-26 09:46:57.000000 pyDVL-0.8.1/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-26 09:46:57.000000 pyDVL-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-26 09:46:57.000000 pyDVL-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 09:48:19.600985 pyDVL-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-01-26 09:46:57.000000 pyDVL-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.584985 pyDVL-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pyDVL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16995 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-26 09:48:19.000000 pyDVL-0.8.1/src/pyDVL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pydvl/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pydvl/influence/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/base_influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    28282 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/influence_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pydvl/influence/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32956 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/torch/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    53897 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/torch/influence_function_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    17818 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/influence/torch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pydvl/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.588985 pyDVL-0.8.1/src/pydvl/parallel/backends/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/backends/joblib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/backends/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.592985 pyDVL-0.8.1/src/pydvl/parallel/futures/
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/futures/ray.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/parallel/map_reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.592985 pyDVL-0.8.1/src/pydvl/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/reporting/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/reporting/scores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.592985 pyDVL-0.8.1/src/pydvl/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.592985 pyDVL-0.8.1/src/pydvl/utils/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/caching/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15418 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/utils/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.596985 pyDVL-0.8.1/src/pydvl/value/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20366 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/games.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.596985 pyDVL-0.8.1/src/pydvl/value/least_core/
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/least_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12005 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/least_core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/least_core/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/least_core/naive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.596985 pyDVL-0.8.1/src/pydvl/value/loo/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/loo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/loo/loo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.596985 pyDVL-0.8.1/src/pydvl/value/oob/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/oob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/oob/oob.py
--rw-r--r--   0 runner    (1001) docker     (127)    31423 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21606 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/semivalues.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 09:48:19.596985 pyDVL-0.8.1/src/pydvl/value/shapley/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24188 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/classwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10847 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13573 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/montecarlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4880 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/owen.py
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/truncated.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/shapley/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    25508 2024-01-26 09:46:57.000000 pyDVL-0.8.1/src/pydvl/value/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.111592 pydvl-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-12 18:11:37.000000 pydvl-0.9/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 18:11:37.000000 pydvl-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 18:11:37.000000 pydvl-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-12 18:13:02.111592 pydvl-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9322 2024-04-12 18:11:37.000000 pydvl-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-12 18:11:37.000000 pydvl-0.9/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-12 18:11:37.000000 pydvl-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-12 18:11:37.000000 pydvl-0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:13:02.111592 pydvl-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-12 18:11:37.000000 pydvl-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.091592 pydvl-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pyDVL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11033 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:13:02.000000 pydvl-0.9/src/pyDVL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.095592 pydvl-0.9/src/pydvl/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/influence/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6599 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/base_influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28378 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/influence_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/influence/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38897 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64011 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/influence_function_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7532 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/pre_conditioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/influence/torch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/joblib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/backends/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/parallel/futures/
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15845 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/futures/ray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/parallel/map_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.099592 pydvl-0.9/src/pydvl/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/reporting/scores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/utils/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/caching/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25291 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10814 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/utils/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/value/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/games.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.103592 pydvl-0.9/src/pydvl/value/least_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12716 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/least_core/naive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/loo/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/loo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/loo/loo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/oob/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/oob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/oob/oob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31283 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17713 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33246 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/semivalues.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/src/pydvl/value/shapley/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/classwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/montecarlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/owen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/shapley/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28615 2024-04-12 18:11:37.000000 pydvl-0.9/src/pydvl/value/stopping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:13:02.107592 pydvl-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-12 18:11:37.000000 pydvl-0.9/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13182 2024-04-12 18:11:37.000000 pydvl-0.9/tests/test_results.py
```

### Comparing `pyDVL-0.8.1/COPYING.LESSER` & `pydvl-0.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/LICENSE` & `pydvl-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/README.md` & `pydvl-0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+Metadata-Version: 2.1
+Name: pyDVL
+Version: 0.9.0
+Summary: The Python Data Valuation Library
+Author: appliedAI Institute gGmbH
+Project-URL: Source, https://github.com/aai-institute/pydvl
+Project-URL: Documentation, https://pydvl.org
+Project-URL: TransferLab, https://transferlab.ai
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYING.LESSER
+Requires-Dist: pyDeprecate>=0.3.2
+Requires-Dist: numpy>=1.20
+Requires-Dist: pandas>=1.3
+Requires-Dist: scikit-learn
+Requires-Dist: scipy>=1.7.0
+Requires-Dist: cvxpy>=1.3.0
+Requires-Dist: joblib>=1.3.0
+Requires-Dist: cloudpickle
+Requires-Dist: tqdm
+Requires-Dist: matplotlib
+Provides-Extra: cupy
+Requires-Dist: cupy-cuda11x>=12.1.0; extra == "cupy"
+Provides-Extra: memcached
+Requires-Dist: pymemcache; extra == "memcached"
+Provides-Extra: influence
+Requires-Dist: torch>=2.0.0; extra == "influence"
+Requires-Dist: dask>=2023.5.0; extra == "influence"
+Requires-Dist: distributed>=2023.5.0; extra == "influence"
+Requires-Dist: zarr>=2.16.1; extra == "influence"
+Provides-Extra: ray
+Requires-Dist: ray>=0.8; extra == "ray"
+
 <p align="center" style="text-align:center;">
     <img alt="pyDVL Logo" src="https://raw.githubusercontent.com/aai-institute/pyDVL/develop/logo.svg" width="200"/>
 </p>
 
 <p align="center" style="text-align:center;">
     A library for data valuation.
 </p>
@@ -14,26 +59,29 @@
     <a href="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml"><img src="https://github.com/aai-institute/pyDVL/actions/workflows/main.yaml/badge.svg" alt="Build status" ></a>
     <a href="https://codecov.io/gh/aai-institute/pyDVL"><img src="https://codecov.io/gh/aai-institute/pyDVL/graph/badge.svg?token=VN7DNDE0FV"/></a>
     <a href="https://zenodo.org/badge/latestdoi/354117916"><img src="https://zenodo.org/badge/354117916.svg" alt="DOI"></a>
 </p>
 
 **pyDVL** collects algorithms for **Data Valuation** and **Influence Function** computation.
 
+Refer to the [Methods](https://pydvl.org/devel/getting-started/methods/)
+page of our documentation for a list of all implemented methods. 
+
 **Data Valuation** for machine learning is the task of assigning a scalar
 to each element of a training set which reflects its contribution to the final
 performance or outcome of some model trained on it. Some concepts of
 value depend on a specific model of interest, while others are model-agnostic.
 pyDVL focuses on model-dependent methods.
 
 <div align="center" style="text-align:center;">
     <img
         width="70%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
-        src="docs/value/img/mclc-best-removal-10k-natural.svg"
+        src="https://pydvl.org/devel/value/img/mclc-best-removal-10k-natural.svg"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Comparison of different data valuation methods
         on best sample removal.
     </p>
 </div>
@@ -44,15 +92,15 @@
 of training samples over individual test points.
 
 <div align="center" style="text-align:center;">
     <img
         width="70%"
         align="center"
         style="display: block; margin-left: auto; margin-right: auto;"
-        src="docs/assets/influence_functions_example.png"
+        src="https://pydvl.org/devel/examples/img/influence_functions_example.png"
         alt="best sample removal"
     />
     <p align="center" style="text-align:center;">
         Influences of input points with corrupted data.
         Highlighted points have flipped labels.
     </p>
 </div>
@@ -68,18 +116,22 @@
 You can also install the latest development version from
 [TestPyPI](https://test.pypi.org/project/pyDVL/):
 
 ```shell
 pip install pyDVL --index-url https://test.pypi.org/simple/
 ```
 
-pyDVL has also extra dependencies for certain functionalities (e.g. influence functions).
+pyDVL has also extra dependencies for certain functionalities, 
+e.g. for using influence functions run
+```shell
+$ pip install pyDVL[influence]
+```
 
 For more instructions and information refer to [Installing pyDVL
-](https://pydvl.org/stable/getting-started/installation/) in the
+](https://pydvl.org/stable/getting-started/#installation) in the
 documentation.
 
 # Usage
 
 In the following subsections, we will showcase the usage of pyDVL
 for Data Valuation and Influence Functions using simple examples.
 
@@ -252,79 +304,14 @@
 
 # Contributing
 
 Please open new issues for bugs, feature requests and extensions. You can read
 about the structure of the project, the toolchain and workflow in the [guide for
 contributions](CONTRIBUTING.md).
 
-# Papers
-
-We currently implement the following papers:
-
-## Data Valuation
-
-- Castro, Javier, Daniel Gómez, and Juan Tejada. [Polynomial Calculation of the
-  Shapley Value Based on Sampling](https://doi.org/10.1016/j.cor.2008.04.004).
-  Computers & Operations Research, Selected papers presented at the Tenth
-  International Symposium on Locational Decisions (ISOLDE X), 36, no. 5 (May 1,
-  2009): 1726–30.
-- Ghorbani, Amirata, and James Zou. [Data Shapley: Equitable Valuation of Data
-  for Machine Learning](http://proceedings.mlr.press/v97/ghorbani19c.html). In
-  International Conference on Machine Learning, 2242–51. PMLR, 2019.
-- Wang, Tianhao, Yu Yang, and Ruoxi Jia. 
-  [Improving Cooperative Game Theory-Based Data Valuation via Data Utility
-  Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv, 2022.
-- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo
-  Li, Ce Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific Data
-  Valuation for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
-  Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019): 1610–23.
-- Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm to Estimate
-  Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In 25th
-  International Conference on Pattern Recognition (ICPR 2020), 7992–99. IEEE,
-  2021.
-- Yan, T., and Procaccia, A. D. [If You Like Shapley Then You’ll Love the
-  Core](https://ojs.aaai.org/index.php/AAAI/article/view/16721). Proceedings of
-  the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759.
-- Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve
-  Gürel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient
-  Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/jia19a.html).
-  In 22nd International Conference on Artificial Intelligence and Statistics,
-  1167–76. PMLR, 2019.
-- Wang, Jiachen T., and Ruoxi Jia. [Data Banzhaf: A Robust Data Valuation
-  Framework for Machine Learning](https://doi.org/10.48550/arXiv.2205.15466).
-  arXiv, October 22, 2022.
-- Kwon, Yongchan, and James Zou. [Beta Shapley: A Unified and Noise-Reduced Data
-  Valuation Framework for Machine Learning](http://arxiv.org/abs/2110.14049).
-  In Proceedings of the 25th International Conference on Artificial Intelligence
-  and Statistics (AISTATS) 2022, Vol. 151. Valencia, Spain: PMLR, 2022.
-- Kwon, Yongchan, and James Zou. [Data-OOB: Out-of-Bag Estimate as a Simple and
-  Efficient Data Value](https://proceedings.mlr.press/v202/kwon23e.html). In
-  Proceedings of the 40th International Conference on Machine Learning, 18135–52.
-  PMLR, 2023.
-- Schoch, Stephanie, Haifeng Xu, and Yangfeng Ji. [CS-Shapley: Class-Wise
-  Shapley Values for Data Valuation in
-  Classification](https://openreview.net/forum?id=KTOcrOR5mQ9). In Proc. of the
-  Thirty-Sixth Conference on Neural Information Processing Systems (NeurIPS).
-  New Orleans, Louisiana, USA, 2022.
-
-## Influence Functions
-
-- Koh, Pang Wei, and Percy Liang. [Understanding Black-Box Predictions via
-  Influence Functions](http://proceedings.mlr.press/v70/koh17a.html). In
-  Proceedings of the 34th International Conference on Machine Learning,
-  70:1885–94. Sydney, Australia: PMLR, 2017.
-- Naman Agarwal, Brian Bullins, and Elad Hazan, [Second-Order Stochastic Optimization
-  for Machine Learning in Linear Time](https://www.jmlr.org/papers/v18/16-491.html),
-  Journal of Machine Learning Research 18 (2017): 1-40.
-- Schioppa, Andrea, Polina Zablotskaia, David Vilar, and Artem Sokolov. 
-  [Scaling Up Influence Functions](http://arxiv.org/abs/2112.03052). 
-  In Proceedings of the AAAI-22. arXiv, 2021.
-- James Martens, Roger Grosse, [Optimizing Neural Networks with Kronecker-factored Approximate Curvature](https://arxiv.org/abs/1503.05671), International Conference on Machine Learning (ICML), 2015.
-- George, Thomas, César Laurent, Xavier Bouthillier, Nicolas Ballas, Pascal Vincent, [Fast Approximate Natural Gradient Descent in a Kronecker-factored Eigenbasis](https://arxiv.org/abs/1806.03884), Advances in Neural Information Processing Systems 31,2018.
-  
 # License
 
 pyDVL is distributed under
 [LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0.html). A complete version can
 be found in two files: [here](LICENSE) and [here](COPYING.LESSER).
 
 All contributions will be distributed under this license.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,40 +1,65 @@
+Metadata-Version: 2.1 Name: pyDVL Version: 0.9.0 Summary: The Python Data
+Valuation Library Author: appliedAI Institute gGmbH Project-URL: Source, https:
+//github.com/aai-institute/pydvl Project-URL: Documentation, https://pydvl.org
+Project-URL: TransferLab, https://transferlab.ai Classifier: Development Status
+:: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Typing :: Typed Classifier: Operating
+System :: MacOS :: MacOS X Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX Classifier: License :: OSI Approved ::
+GNU Lesser General Public License v3 (LGPLv3) Description-Content-Type: text/
+markdown License-File: LICENSE License-File: COPYING.LESSER Requires-Dist:
+pyDeprecate>=0.3.2 Requires-Dist: numpy>=1.20 Requires-Dist: pandas>=1.3
+Requires-Dist: scikit-learn Requires-Dist: scipy>=1.7.0 Requires-Dist:
+cvxpy>=1.3.0 Requires-Dist: joblib>=1.3.0 Requires-Dist: cloudpickle Requires-
+Dist: tqdm Requires-Dist: matplotlib Provides-Extra: cupy Requires-Dist: cupy-
+cuda11x>=12.1.0; extra == "cupy" Provides-Extra: memcached Requires-Dist:
+pymemcache; extra == "memcached" Provides-Extra: influence Requires-Dist:
+torch>=2.0.0; extra == "influence" Requires-Dist: dask>=2023.5.0; extra ==
+"influence" Requires-Dist: distributed>=2023.5.0; extra == "influence"
+Requires-Dist: zarr>=2.16.1; extra == "influence" Provides-Extra: ray Requires-
+Dist: ray>=0.8; extra == "ray"
                                  [pyDVL Logo]
                          A library for data valuation.
  _[_P_y_P_I_]_[_V_e_r_s_i_o_n_]_[_d_o_c_u_m_e_n_t_a_t_i_o_n_]_[_L_i_c_e_n_s_e_]_[_B_u_i_l_d_ _s_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/
           _a_a_i_-_i_n_s_t_i_t_u_t_e_/_p_y_D_V_L_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_V_N_7_D_N_D_E_0_F_V_]_[_D_O_I_]
 **pyDVL** collects algorithms for **Data Valuation** and **Influence Function**
-computation. **Data Valuation** for machine learning is the task of assigning a
-scalar to each element of a training set which reflects its contribution to the
-final performance or outcome of some model trained on it. Some concepts of
-value depend on a specific model of interest, while others are model-agnostic.
-pyDVL focuses on model-dependent methods.
+computation. Refer to the [Methods](https://pydvl.org/devel/getting-started/
+methods/) page of our documentation for a list of all implemented methods.
+**Data Valuation** for machine learning is the task of assigning a scalar to
+each element of a training set which reflects its contribution to the final
+performance or outcome of some model trained on it. Some concepts of value
+depend on a specific model of interest, while others are model-agnostic. pyDVL
+focuses on model-dependent methods.
                              [best sample removal]
     Comparison of different data valuation methods on best sample removal.
 The **Influence Function** is an infinitesimal measure of the effect that
 single training points have over the parameters of a model, or any function
 thereof. In particular, in machine learning they are also used to compute the
 effect of training samples over individual test points.
                              [best sample removal]
 Influences of input points with corrupted data. Highlighted points have flipped
                                     labels.
 # Installation To install the latest release use: ```shell $ pip install pyDVL
 ``` You can also install the latest development version from [TestPyPI](https:/
 /test.pypi.org/project/pyDVL/): ```shell pip install pyDVL --index-url https://
 test.pypi.org/simple/ ``` pyDVL has also extra dependencies for certain
-functionalities (e.g. influence functions). For more instructions and
-information refer to [Installing pyDVL ](https://pydvl.org/stable/getting-
-started/installation/) in the documentation. # Usage In the following
-subsections, we will showcase the usage of pyDVL for Data Valuation and
-Influence Functions using simple examples. For more instructions and
-information refer to [Getting Started](https://pydvl.org/stable/getting-
-started/first-steps/) in the documentation. We provide several examples for
-data valuation (e.g. [Shapley Data Valuation](https://pydvl.org/stable/
-examples/shapley_basic_spotify/)) and for influence functions (e.g. [Influence
-Functions for Neural Networks](https://pydvl.org/stable/examples/
+functionalities, e.g. for using influence functions run ```shell $ pip install
+pyDVL[influence] ``` For more instructions and information refer to [Installing
+pyDVL ](https://pydvl.org/stable/getting-started/#installation) in the
+documentation. # Usage In the following subsections, we will showcase the usage
+of pyDVL for Data Valuation and Influence Functions using simple examples. For
+more instructions and information refer to [Getting Started](https://pydvl.org/
+stable/getting-started/first-steps/) in the documentation. We provide several
+examples for data valuation (e.g. [Shapley Data Valuation](https://pydvl.org/
+stable/examples/shapley_basic_spotify/)) and for influence functions (e.g.
+[Influence Functions for Neural Networks](https://pydvl.org/stable/examples/
 influence_imagenet/)) with details on the algorithms and their applications. ##
 Influence Functions For influence computation, follow these steps: 1. Import
 the necessary packages (The exact packages depend on your specific use case).
 ```python import torch from torch import nn from torch.utils.data import
 DataLoader, TensorDataset from pydvl.influence.torch import DirectInfluence
 from pydvl.influence.torch.util import NestedTorchCatAggregator,
 TorchNumpyConverter from pydvl.influence import SequentialInfluenceCalculator
@@ -87,65 +112,11 @@
 contains the indices and their values as well as other attributes. The higher
 the value for an index, the more important it is for the chosen model, dataset
 and scorer. 6. (Optional) Convert the valuation result to a dataframe and
 analyze and visualize the values. ```python df = values.to_dataframe
 (column="data_value") ``` # Contributing Please open new issues for bugs,
 feature requests and extensions. You can read about the structure of the
 project, the toolchain and workflow in the [guide for contributions]
-(CONTRIBUTING.md). # Papers We currently implement the following papers: ##
-Data Valuation - Castro, Javier, Daniel GÃ³mez, and Juan Tejada. [Polynomial
-Calculation of the Shapley Value Based on Sampling](https://doi.org/10.1016/
-j.cor.2008.04.004). Computers & Operations Research, Selected papers presented
-at the Tenth International Symposium on Locational Decisions (ISOLDE X), 36,
-no. 5 (May 1, 2009): 1726â30. - Ghorbani, Amirata, and James Zou. [Data
-Shapley: Equitable Valuation of Data for Machine Learning](http://
-proceedings.mlr.press/v97/ghorbani19c.html). In International Conference on
-Machine Learning, 2242â51. PMLR, 2019. - Wang, Tianhao, Yu Yang, and Ruoxi
-Jia. [Improving Cooperative Game Theory-Based Data Valuation via Data Utility
-Learning](https://doi.org/10.48550/arXiv.2107.06336). arXiv, 2022. - Jia,
-Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo Li, Ce
-Zhang, Costas Spanos, and Dawn Song. [Efficient Task-Specific Data Valuation
-for Nearest Neighbor Algorithms](https://doi.org/10.14778/3342263.3342637).
-Proceedings of the VLDB Endowment 12, no. 11 (1 July 2019): 1610â23. -
-Okhrati, Ramin, and Aldo Lipani. [A Multilinear Sampling Algorithm to Estimate
-Shapley Values](https://doi.org/10.1109/ICPR48806.2021.9412511). In 25th
-International Conference on Pattern Recognition (ICPR 2020), 7992â99. IEEE,
-2021. - Yan, T., and Procaccia, A. D. [If You Like Shapley Then Youâll Love
-the Core](https://ojs.aaai.org/index.php/AAAI/article/view/16721). Proceedings
-of the AAAI Conference on Artificial Intelligence, 35(6) (2021): 5751-5759. -
-Jia, Ruoxi, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve
-GÃ¼rel, Bo Li, Ce Zhang, Dawn Song, and Costas J. Spanos. [Towards Efficient
-Data Valuation Based on the Shapley Value](http://proceedings.mlr.press/v89/
-jia19a.html). In 22nd International Conference on Artificial Intelligence and
-Statistics, 1167â76. PMLR, 2019. - Wang, Jiachen T., and Ruoxi Jia. [Data
-Banzhaf: A Robust Data Valuation Framework for Machine Learning](https://
-doi.org/10.48550/arXiv.2205.15466). arXiv, October 22, 2022. - Kwon, Yongchan,
-and James Zou. [Beta Shapley: A Unified and Noise-Reduced Data Valuation
-Framework for Machine Learning](http://arxiv.org/abs/2110.14049). In
-Proceedings of the 25th International Conference on Artificial Intelligence and
-Statistics (AISTATS) 2022, Vol. 151. Valencia, Spain: PMLR, 2022. - Kwon,
-Yongchan, and James Zou. [Data-OOB: Out-of-Bag Estimate as a Simple and
-Efficient Data Value](https://proceedings.mlr.press/v202/kwon23e.html). In
-Proceedings of the 40th International Conference on Machine Learning,
-18135â52. PMLR, 2023. - Schoch, Stephanie, Haifeng Xu, and Yangfeng Ji. [CS-
-Shapley: Class-Wise Shapley Values for Data Valuation in Classification](https:
-//openreview.net/forum?id=KTOcrOR5mQ9). In Proc. of the Thirty-Sixth Conference
-on Neural Information Processing Systems (NeurIPS). New Orleans, Louisiana,
-USA, 2022. ## Influence Functions - Koh, Pang Wei, and Percy Liang.
-[Understanding Black-Box Predictions via Influence Functions](http://
-proceedings.mlr.press/v70/koh17a.html). In Proceedings of the 34th
-International Conference on Machine Learning, 70:1885â94. Sydney, Australia:
-PMLR, 2017. - Naman Agarwal, Brian Bullins, and Elad Hazan, [Second-Order
-Stochastic Optimization for Machine Learning in Linear Time](https://
-www.jmlr.org/papers/v18/16-491.html), Journal of Machine Learning Research 18
-(2017): 1-40. - Schioppa, Andrea, Polina Zablotskaia, David Vilar, and Artem
-Sokolov. [Scaling Up Influence Functions](http://arxiv.org/abs/2112.03052). In
-Proceedings of the AAAI-22. arXiv, 2021. - James Martens, Roger Grosse,
-[Optimizing Neural Networks with Kronecker-factored Approximate Curvature]
-(https://arxiv.org/abs/1503.05671), International Conference on Machine
-Learning (ICML), 2015. - George, Thomas, CÃ©sar Laurent, Xavier Bouthillier,
-Nicolas Ballas, Pascal Vincent, [Fast Approximate Natural Gradient Descent in a
-Kronecker-factored Eigenbasis](https://arxiv.org/abs/1806.03884), Advances in
-Neural Information Processing Systems 31,2018. # License pyDVL is distributed
-under [LGPL-3.0](https://www.gnu.org/licenses/lgpl-3.0.html). A complete
-version can be found in two files: [here](LICENSE) and [here](COPYING.LESSER).
-All contributions will be distributed under this license.
+(CONTRIBUTING.md). # License pyDVL is distributed under [LGPL-3.0](https://
+www.gnu.org/licenses/lgpl-3.0.html). A complete version can be found in two
+files: [here](LICENSE) and [here](COPYING.LESSER). All contributions will be
+distributed under this license.
```

### Comparing `pyDVL-0.8.1/pyproject.toml` & `pydvl-0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/setup.py` & `pydvl-0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 setup(
     name="pyDVL",
     package_dir={"": "src"},
     package_data={"pydvl": ["py.typed"]},
     packages=find_packages(where="src"),
     include_package_data=True,
-    version="0.8.1",
+    version="0.9.0",
     description="The Python Data Valuation Library",
     install_requires=[
         line
         for line in open("requirements.txt").readlines()
         if not line.startswith("--")
     ],
     setup_requires=["wheel"],
@@ -39,20 +39,21 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     ],
     project_urls={
         "Source": "https://github.com/aai-institute/pydvl",
-        "Documentation": "https://aai-institute.github.io/pyDVL",
-        "TransferLab": "https://transferlab.appliedai.de",
+        "Documentation": "https://pydvl.org",
+        "TransferLab": "https://transferlab.ai",
     },
     zip_safe=False,  # Needed for mypy to find py.typed
 )
```

### Comparing `pyDVL-0.8.1/src/pyDVL.egg-info/SOURCES.txt` & `pydvl-0.9/src/pyDVL.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 src/pyDVL.egg-info/PKG-INFO
 src/pyDVL.egg-info/SOURCES.txt
 src/pyDVL.egg-info/dependency_links.txt
 src/pyDVL.egg-info/not-zip-safe
 src/pyDVL.egg-info/requires.txt
 src/pyDVL.egg-info/top_level.txt
 src/pydvl/__init__.py
+src/pydvl/py.typed
 src/pydvl/influence/__init__.py
 src/pydvl/influence/array.py
 src/pydvl/influence/base_influence_function_model.py
 src/pydvl/influence/influence_calculator.py
 src/pydvl/influence/torch/__init__.py
 src/pydvl/influence/torch/functional.py
 src/pydvl/influence/torch/influence_function_model.py
+src/pydvl/influence/torch/pre_conditioner.py
 src/pydvl/influence/torch/util.py
 src/pydvl/parallel/__init__.py
 src/pydvl/parallel/backend.py
 src/pydvl/parallel/config.py
 src/pydvl/parallel/map_reduce.py
 src/pydvl/parallel/backends/__init__.py
 src/pydvl/parallel/backends/joblib.py
@@ -34,15 +36,14 @@
 src/pydvl/reporting/plots.py
 src/pydvl/reporting/scores.py
 src/pydvl/utils/__init__.py
 src/pydvl/utils/config.py
 src/pydvl/utils/dataset.py
 src/pydvl/utils/functional.py
 src/pydvl/utils/numeric.py
-src/pydvl/utils/parallel.py
 src/pydvl/utils/progress.py
 src/pydvl/utils/score.py
 src/pydvl/utils/status.py
 src/pydvl/utils/types.py
 src/pydvl/utils/utility.py
 src/pydvl/utils/caching/__init__.py
 src/pydvl/utils/caching/base.py
@@ -69,8 +70,10 @@
 src/pydvl/value/shapley/common.py
 src/pydvl/value/shapley/gt.py
 src/pydvl/value/shapley/knn.py
 src/pydvl/value/shapley/montecarlo.py
 src/pydvl/value/shapley/naive.py
 src/pydvl/value/shapley/owen.py
 src/pydvl/value/shapley/truncated.py
-src/pydvl/value/shapley/types.py
+src/pydvl/value/shapley/types.py
+tests/test_plugin.py
+tests/test_results.py
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/array.py` & `pydvl-0.9/src/pydvl/influence/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 types and NumPy arrays, aggregating blocks of data, and abstract representations of
 lazy arrays. Concrete implementations are provided for handling chunked lazy arrays
 (chunked in one resp. two dimensions), with support for efficient storage and retrieval
 using the Zarr library.
 """
 
 from abc import ABC, abstractmethod
-from typing import Callable, Generator, Generic, List, Optional, Tuple
+from typing import Callable, Generator, Generic, List, Optional, Tuple, Union
 
 import zarr
 from numpy.typing import NDArray
+from zarr.storage import StoreLike
 
 from .base_influence_function_model import TensorType
 
 
 class NumpyConverter(Generic[TensorType], ABC):
     """
     Base class for converting TensorType objects into numpy arrays and vice versa.
@@ -136,27 +137,28 @@
         """
         if aggregator is None:
             aggregator = ListAggregator()
         return aggregator(self.generator_factory())
 
     def to_zarr(
         self,
-        path_or_url: str,
+        path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
         overwrite: bool = False,
     ) -> Optional[zarr.Array]:
         """
         Converts the array into Zarr format, a storage format optimized for large
         arrays, and stores it at the specified path or URL. This method is suitable for
         scenarios where the data needs to be saved for later use or for large datasets
         requiring efficient storage.
 
         Args:
             path_or_url: The file path or URL where the Zarr array will be stored.
+                Also excepts instances of zarr stores.
             converter: A converter for transforming blocks into NumPy arrays
                 compatible with Zarr.
             return_stored: If True, the method returns the stored Zarr array; otherwise,
                 it returns None.
             overwrite: If True, overwrites existing data at the given path_or_url.
                 If False, an error is raised in case of existing data.
 
@@ -240,27 +242,28 @@
         """
         if aggregator is None:
             aggregator = NestedListAggregator()
         return aggregator(self.generator_factory())
 
     def to_zarr(
         self,
-        path_or_url: str,
+        path_or_url: Union[str, StoreLike],
         converter: NumpyConverter,
         return_stored: bool = False,
         overwrite: bool = False,
     ) -> Optional[zarr.Array]:
         """
         Converts the array into Zarr format, a storage format optimized for large
         arrays, and stores it at the specified path or URL. This method is suitable for
         scenarios where the data needs to be saved for later use or for large datasets
         requiring efficient storage.
 
         Args:
             path_or_url: The file path or URL where the Zarr array will be stored.
+                Also excepts instances of zarr stores.
             converter: A converter for transforming blocks into NumPy arrays
                 compatible with Zarr.
             return_stored: If True, the method returns the stored Zarr array;
                 otherwise, it returns None.
             overwrite: If True, overwrites existing data at the given path_or_url.
                 If False, an error is raised in case of existing data.
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/base_influence_function_model.py` & `pydvl-0.9/src/pydvl/influence/base_influence_function_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import Collection, Generic, Iterable, Optional, TypeVar
+from typing import Collection, Generic, Iterable, Optional, Type, TypeVar
 
 
 class InfluenceMode(str, Enum):
-    r"""
+    """
     Enum representation for the types of influence.
 
     Attributes:
         Up: [Approximating the influence of a point]
             [approximating-the-influence-of-a-point]
         Perturbation: [Perturbation definition of the influence score]
             [perturbation-definition-of-the-influence-score]
@@ -24,18 +26,18 @@
         super().__init__(
             f"Provided {mode=} is not supported. Choose one of InfluenceMode.Up "
             f"and InfluenceMode.Perturbation"
         )
 
 
 class NotFittedException(ValueError):
-    def __init__(self):
+    def __init__(self, object_type: Type):
         super().__init__(
-            f"Objects of type InfluenceFunctionModel must be fitted before calling "
-            f"influence methods. "
+            f"Objects of type {object_type} must be fitted before calling "
+            f"methods. "
             f"Call method fit with appropriate input."
         )
 
 
 class NotImplementedLayerRepresentationException(ValueError):
     def __init__(self, module_id: str):
         message = f"Only Linear layers are supported, but found module {module_id} requiring grad."
@@ -66,29 +68,29 @@
 
     @property
     @abstractmethod
     def is_fitted(self):
         """Override this, to expose the fitting status of the instance."""
 
     @abstractmethod
-    def fit(self, data: DataLoaderType):
+    def fit(self, data: DataLoaderType) -> InfluenceFunctionModel:
         """
         Override this method to fit the influence function model to training data,
         e.g. pre-compute hessian matrix or matrix decompositions
 
         Args:
             data:
 
         Returns:
             The fitted instance
         """
 
     def influence_factors(self, x: TensorType, y: TensorType) -> TensorType:
         if not self.is_fitted:
-            raise NotFittedException()
+            raise NotFittedException(type(self))
         return self._influence_factors(x, y)
 
     @abstractmethod
     def _influence_factors(self, x: TensorType, y: TensorType) -> TensorType:
         r"""
         Override this method to implement the approximation of
 
@@ -110,15 +112,15 @@
         x_test: TensorType,
         y_test: TensorType,
         x: Optional[TensorType] = None,
         y: Optional[TensorType] = None,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> TensorType:
         if not self.is_fitted:
-            raise NotFittedException()
+            raise NotFittedException(type(self))
         return self._influences(x_test, y_test, x, y, mode)
 
     @abstractmethod
     def _influences(
         self,
         x_test: TensorType,
         y_test: TensorType,
@@ -146,15 +148,15 @@
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
                 $\nabla_{theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{test}$
             y: optional label tensor to compute gradients
             mode: enum value of [InfluenceMode]
-                [pydvl.influence.base_influence_modl.InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             Tensor representing the element-wise scalar products for the provided batch
 
         """
 
     @abstractmethod
@@ -176,22 +178,22 @@
         \[ \langle z_{\text{test_factors}},
             \nabla_{x} \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle \]
 
         for the perturbation type influence case. The gradient is meant to be per sample
         of the batch $(x, y)$.
 
         Args:
-             z_test_factors: pre-computed array, approximating
+            z_test_factors: pre-computed array, approximating
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                 f_{\theta}(x_{\text{test}}))$
-             x: model input to use in the gradient computations
+            x: model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
-             y: label tensor to compute gradients
-             mode: enum value of [InfluenceMode]
-                [pydvl.influence.base_influence_modl.InfluenceMode]
+            y: label tensor to compute gradients
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             Tensor representing the element-wise scalar products for the provided batch
 
         """
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/influence_calculator.py` & `pydvl-0.9/src/pydvl/influence/influence_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 This module provides functionality for calculating influences for large amount of data.
 The computation is based on a chunk computation model in the form of an instance of
-[InfluenceFunctionModel][pydvl.influence.base_influence_model.InfluenceFunctionModel],
+[InfluenceFunctionModel][pydvl.influence.base_influence_function_model.InfluenceFunctionModel],
 which is mapped over collection of chunks.
 """
 
 import logging
 from functools import partial
 from typing import Generator, Iterable, Optional, Tuple, Type, Union
 
@@ -97,24 +97,24 @@
 class DaskInfluenceCalculator:
     """
     This class is designed to compute influences over
     [dask.array.Array][dask.array.Array] collections, leveraging the capabilities of
     Dask for distributed computing and parallel processing. It requires an influence
     computation model of type
     [InfluenceFunctionModel]
-    [pydvl.influence.base_influence_model.InfluenceFunctionModel],
+    [pydvl.influence.base_influence_function_model.InfluenceFunctionModel],
     which defines how influences are computed on a chunk of data.
     Essentially, this class functions by mapping the influence
     function model across the various chunks of a [dask.array.Array][dask.array.Array]
     collection.
 
     Args:
         influence_function_model: instance of type
             [InfluenceFunctionModel]
-            [pydvl.influence.base_influence_model.InfluenceFunctionModel], that
+            [pydvl.influence.base_influence_function_model.InfluenceFunctionModel], that
             specifies the computation logic for influence on data chunks. It's a pivotal
             part of the calculator, determining how influence is computed and applied
             across the data array.
         converter: A utility for converting numpy arrays to TensorType objects,
             facilitating the interaction between numpy arrays and the influence
             function model.
         client: This parameter accepts either of two types:
@@ -136,31 +136,31 @@
             scheduler), you can supply the [DisableClientSingleThreadCheck]
             [pydvl.influence.influence_calculator.DisableClientSingleThreadCheck] type.
 
     !!! Warning
         Make sure to set `threads_per_worker=1`, when using the distributed scheduler
         for computing, if your implementation of
         [InfluenceFunctionModel]
-        [pydvl.influence.base_influence_model.InfluenceFunctionModel]
+        [pydvl.influence.base_influence_function_model.InfluenceFunctionModel]
         is not thread-safe.
         ```python
         client = Client(threads_per_worker=1)
         ```
         For details on dask schedulers see the
         [official documentation](https://docs.dask.org/en/stable/scheduling.html).
 
     Example:
         ```python
         import torch
         from torch.utils.data import Dataset, DataLoader
         from pydvl.influence import DaskInfluenceCalculator
         from pydvl.influence.torch import CgInfluence
         from pydvl.influence.torch.util import (
-        torch_dataset_to_dask_array,
-        TorchNumpyConverter,
+            torch_dataset_to_dask_array,
+            TorchNumpyConverter,
         )
         from distributed import Client
 
         # Possible some out of memory large Dataset
         train_data_set: Dataset = LargeDataSet(...)
         test_data_set: Dataset = LargeDataSet(...)
 
@@ -328,16 +328,16 @@
                     f_{\theta}(x_{\text{test}}))$
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             [dask.array.Array][dask.array.Array] representing the element-wise scalar
                 products for the provided batch.
 
         """
 
@@ -453,16 +453,16 @@
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                     f_{\theta}(x_{\text{test}}))$
             x: optional model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.twice_differentiable.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
           [dask.array.Array][dask.array.Array] representing the element-wise scalar
             product of the provided batch
 
         """
         self._validate_aligned_chunking(x, y)
@@ -543,21 +543,21 @@
 class SequentialInfluenceCalculator:
     """
     This class serves as a simple wrapper for processing batches of data
     in a sequential manner. It is particularly useful in scenarios where parallel
     or distributed processing is not required or not feasible.
     The core functionality of this class is to apply a specified influence computation
     model, of type [InfluenceFunctionModel]
-    [pydvl.influence.base_influence_model.InfluenceFunctionModel], to batches of data
+    [pydvl.influence.base_influence_function_model.InfluenceFunctionModel], to batches of data
     one at a time.
 
     Args:
         influence_function_model: An instance of type
                 [InfluenceFunctionModel]
-                [pydvl.influence.base_influence_model.InfluenceFunctionModel], that
+                [pydvl.influence.base_influence_function_model.InfluenceFunctionModel], that
                 specifies the computation logic for influence on data chunks.
 
     Example:
         ```python
         from pydvl.influence import SequentialInfluenceCalculator
         from pydvl.influence.torch.util import (
         NestedTorchCatAggregator,
@@ -624,15 +624,14 @@
 
     def _influences_gen(
         self,
         test_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         train_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         mode: InfluenceMode,
     ) -> Generator[Generator[TensorType, None, None], None, None]:
-
         for x_test, y_test in iter(test_data_iterable):
             yield (
                 self.influence_function_model.influences(x_test, y_test, x, y, mode)
                 for x, y in iter(train_data_iterable)
             )
 
     def influences(
@@ -660,16 +659,16 @@
         Args:
             test_data_iterable: An iterable that returns tuples of tensors.
                 Each tuple consists of a pair of tensors (x, y), representing input data
                 and corresponding targets.
             train_data_iterable: An iterable that returns tuples of tensors.
                 Each tuple consists of a pair of tensors (x, y), representing input data
                 and corresponding targets.
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             A lazy data structure representing the chunks of the resulting tensor
 
         """
         nested_tensor_gen_factory = partial(
             self._influences_gen,
@@ -682,15 +681,14 @@
 
     def _influences_from_factors_gen(
         self,
         z_test_factors: Iterable[TensorType],
         train_data_iterable: Iterable[Tuple[TensorType, TensorType]],
         mode: InfluenceMode,
     ):
-
         for z_test_factor in iter(z_test_factors):
             if isinstance(z_test_factor, list) or isinstance(z_test_factor, tuple):
                 z_test_factor = z_test_factor[0]
             yield (
                 self.influence_function_model.influences_from_factors(
                     z_test_factor, x, y, mode
                 )
@@ -720,16 +718,16 @@
         Args:
             z_test_factors: Pre-computed iterable of tensors, approximating
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                     f_{\theta}(x_{\text{test}}))$
             train_data_iterable: An iterable that returns tuples of tensors.
                 Each tuple consists of a pair of tensors (x, y), representing input data
                 and corresponding targets.
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.twice_differentiable.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
           A lazy data structure representing the chunks of the resulting tensor
 
         """
         nested_tensor_gen = partial(
             self._influences_from_factors_gen,
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/torch/functional.py` & `pydvl-0.9/src/pydvl/influence/torch/functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 """
 
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass
 from functools import partial
-from typing import Callable, Dict, Optional, Tuple
+from typing import Callable, Dict, Optional, Tuple, Union
 
 import torch
 from scipy.sparse.linalg import ArpackNoConvergence
+from torch._C import _LinAlgError
 from torch.func import functional_call, grad, jvp, vjp
 from torch.utils.data import DataLoader
 
 from .util import align_structure, align_with_model, flatten_dimensions, to_model_device
 
 __all__ = [
     "create_hvp_function",
@@ -43,16 +44,19 @@
     "create_batch_hvp_function",
     "create_per_sample_loss_function",
     "create_per_sample_gradient_function",
     "create_matrix_jacobian_product_function",
     "create_per_sample_mixed_derivative_function",
     "model_hessian_low_rank",
     "LowRankProductRepresentation",
+    "randomized_nystroem_approximation",
+    "model_hessian_nystroem_approximation",
 ]
 
+
 logger = logging.getLogger(__name__)
 
 
 def hvp(
     func: Callable[[Dict[str, torch.Tensor]], torch.Tensor],
     params: Dict[str, torch.Tensor],
     vec: Dict[str, torch.Tensor],
@@ -164,16 +168,18 @@
     data_loader: DataLoader,
 ) -> Callable[[Dict[str, torch.Tensor]], torch.Tensor]:
     r"""
     Creates a function to compute the empirical loss of a given model
     on a given dataset. If we denote the model parameters with \( \theta \),
     the resulting function approximates:
 
-    \[ f(\theta) = \frac{1}{N}\sum_{i=1}^N
-        \operatorname{loss}(y_i, \operatorname{model}(\theta, x_i)) \]
+    \[
+        f(\theta) = \frac{1}{N}\sum_{i=1}^N
+        \operatorname{loss}(y_i, \operatorname{model}(\theta, x_i))
+    \]
 
     for a loss function $\operatorname{loss}$ and a model $\operatorname{model}$
     with model parameters $\theta$, where $N$ is the number of all elements provided
     by the data_loader.
 
     Args:
         model: The model for which the loss should be computed.
@@ -255,44 +261,44 @@
     the function [hvp][pydvl.influence.torch.functional.hvp].
 
     Args:
         model: A PyTorch module representing the model whose loss function's
             Hessian is to be computed.
         loss: A callable that takes the model's output and target as input and
             returns the scalar loss.
-        data_loader: A DataLoader instance that provides batches of data for calculating
-            the Hessian-vector product. Each batch from the DataLoader is assumed to
-            return a tuple where the first element
-            is the model's input and the second element is the target output.
-        precompute_grad: If True, the full data gradient is precomputed and kept
-            in memory, which can speed up the hessian vector product computation.
-            Set this to False, if you can't afford to keep an additional
-            parameter-sized vector in memory.
-        use_average: If True, the returned function uses batch-wise computation via
-            [batch_loss_function][pydvl.influence.torch.functional.batch_loss_function]
+        data_loader: A DataLoader instance that provides batches of data for
+            calculating the Hessian-vector product. Each batch from the
+            DataLoader is assumed to return a tuple where the first element is
+            the model's input and the second element is the target output.
+        precompute_grad: If `True`, the full data gradient is precomputed and
+            kept in memory, which can speed up the hessian vector product
+            computation. Set this to `False`, if you can't afford to keep the
+            full computation graph in memory.
+        use_average: If `True`, the returned function uses batch-wise
+            computation via
+            [a batch loss function][pydvl.influence.torch.functional.create_batch_loss_function]
             and averages the results.
-            If False, the function uses backpropagation on the full
-            [empirical_loss_function]
-            [pydvl.influence.torch.functional.empirical_loss_function],
-            which is more accurate than averaging the batch hessians,
-            but probably has a way higher memory usage.
+            If `False`, the function uses backpropagation on the full
+            [empirical loss function]
+            [pydvl.influence.torch.functional.create_empirical_loss_function],
+            which is more accurate than averaging the batch hessians, but
+            probably has a way higher memory usage.
         reverse_only: Whether to use only reverse-mode autodiff or
-            both forward- and reverse-mode autodiff.
-            Ignored if precompute_grad is True.
-        track_gradients: Whether to track gradients for the resulting tensor of the
-            hessian vector products.
+            both forward- and reverse-mode autodiff. Ignored if
+            `precompute_grad` is `True`.
+        track_gradients: Whether to track gradients for the resulting tensor of
+            the Hessian-vector products.
 
     Returns:
-        A function that takes a single argument, a vector, and returns the product of
-            the Hessian of the `loss` function with respect to the `model`'s parameters
-            and the input vector.
+        A function that takes a single argument, a vector, and returns the
+        product of the Hessian of the `loss` function with respect to the
+        `model`'s parameters and the input vector.
     """
 
     if precompute_grad:
-
         model_params = {k: p for k, p in model.named_parameters() if p.requires_grad}
 
         if use_average:
             model_dtype = next(p.dtype for p in model.parameters() if p.requires_grad)
             total_grad_xy = torch.empty(0, dtype=model_dtype)
             total_points = 0
             grad_func = torch.func.grad(create_batch_loss_function(model, loss))
@@ -404,43 +410,43 @@
     n_parameters = sum([p.numel() for p in params.values()])
     model_dtype = next((p.dtype for p in params.values()))
 
     flat_params = flatten_dimensions(params.values())
 
     if use_hessian_avg:
         n_samples = 0
-        hessian = to_model_device(
+        hessian_mat = to_model_device(
             torch.zeros((n_parameters, n_parameters), dtype=model_dtype), model
         )
         blf = create_batch_loss_function(model, loss)
 
         def flat_input_batch_loss_function(
             p: torch.Tensor, t_x: torch.Tensor, t_y: torch.Tensor
         ):
             return blf(align_with_model(p, model), t_x, t_y)
 
         for x, y in iter(data_loader):
             n_samples += x.shape[0]
-            hessian += x.shape[0] * torch.func.hessian(flat_input_batch_loss_function)(
-                flat_params, to_model_device(x, model), to_model_device(y, model)
-            )
+            hessian_mat += x.shape[0] * torch.func.hessian(
+                flat_input_batch_loss_function
+            )(flat_params, to_model_device(x, model), to_model_device(y, model))
 
-        hessian /= n_samples
+        hessian_mat /= n_samples
     else:
 
         def flat_input_empirical_loss(p: torch.Tensor):
             return create_empirical_loss_function(model, loss, data_loader)(
                 align_with_model(p, model)
             )
 
-        hessian = torch.func.jacrev(torch.func.jacrev(flat_input_empirical_loss))(
+        hessian_mat = torch.func.jacrev(torch.func.jacrev(flat_input_empirical_loss))(
             flat_params
         )
 
-    return hessian
+    return hessian_mat
 
 
 def create_per_sample_loss_function(
     model: torch.nn.Module, loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor]
 ) -> Callable[[Dict[str, torch.Tensor], torch.Tensor, torch.Tensor], torch.Tensor]:
     r"""
     Generates a function to compute per-sample losses using PyTorch's vmap,
@@ -768,14 +774,15 @@
     training_data: DataLoader,
     hessian_perturbation: float = 0.0,
     rank_estimate: int = 10,
     krylov_dimension: Optional[int] = None,
     tol: float = 1e-6,
     max_iter: Optional[int] = None,
     eigen_computation_on_gpu: bool = False,
+    precompute_grad: bool = False,
 ) -> LowRankProductRepresentation:
     r"""
     Calculates a low-rank approximation of the Hessian matrix of the model's
     loss function using the implicitly restarted Lanczos algorithm, i.e.
 
     \[ H_{\text{approx}} = V D V^T\]
 
@@ -803,28 +810,179 @@
             If not provided, it defaults to 10*model.n_parameters.
         eigen_computation_on_gpu: If True, tries to execute the eigen pair approximation
             on the provided device via cupy implementation.
             Make sure, that either your model is small enough or you use a
             small rank_estimate to fit your device's memory.
             If False, the eigen pair approximation is executed on the CPU by
             scipy wrapper to ARPACK.
+        precompute_grad: If True, the full data gradient is precomputed and kept
+            in memory, which can speed up the hessian vector product computation.
+            Set this to False, if you can't afford to keep the full computation graph
+            in memory.
 
     Returns:
         [LowRankProductRepresentation]
             [pydvl.influence.torch.functional.LowRankProductRepresentation]
             instance that contains the top (up until rank_estimate) eigenvalues
             and corresponding eigenvectors of the Hessian.
     """
-    raw_hvp = create_hvp_function(model, loss, training_data, use_average=True)
+    raw_hvp = create_hvp_function(
+        model, loss, training_data, use_average=True, precompute_grad=precompute_grad
+    )
     n_params = sum([p.numel() for p in model.parameters() if p.requires_grad])
     device = next(model.parameters()).device
     return lanzcos_low_rank_hessian_approx(
         hessian_vp=raw_hvp,
         matrix_shape=(n_params, n_params),
         hessian_perturbation=hessian_perturbation,
         rank_estimate=rank_estimate,
         krylov_dimension=krylov_dimension,
         tol=tol,
         max_iter=max_iter,
         device=device,
         eigen_computation_on_gpu=eigen_computation_on_gpu,
     )
+
+
+def randomized_nystroem_approximation(
+    mat_mat_prod: Union[torch.Tensor, Callable[[torch.Tensor], torch.Tensor]],
+    input_dim: int,
+    rank: int,
+    input_type: torch.dtype,
+    shift_func: Optional[Callable[[torch.Tensor], torch.Tensor]] = None,
+    mat_vec_device: torch.device = torch.device("cpu"),
+) -> LowRankProductRepresentation:
+    r"""
+    Given a matrix vector product function (representing a symmetric positive definite
+    matrix $A$ ), computes a random Nyström low rank approximation of
+    $A$ in factored form, i.e.
+
+    $$ A_{\text{nys}} = (A \Omega)(\Omega^T A \Omega)^{\dagger}(A \Omega)^T
+    = U \Sigma U^T $$
+
+    where $\Omega$ is a standard normal random matrix.
+
+    Args:
+        mat_mat_prod: A callable representing the matrix vector product
+        input_dim: dimension of the input for the matrix vector product
+        input_type: data_type of inputs
+        rank: rank of the approximation
+        shift_func: optional function for computing the stabilizing shift in the
+            construction of the randomized nystroem approximation, defaults to
+
+            $$ \sqrt{\operatorname{\text{input_dim}}} \cdot
+                \varepsilon(\operatorname{\text{input_type}}) \cdot \|A\Omega\|_2,$$
+
+            where $\varepsilon(\operatorname{\text{input_type}})$ is the value of the
+            machine precision corresponding to the data type.
+        mat_vec_device: device where the matrix vector product has to be executed
+
+    Returns:
+        object containing, $U$ and $\Sigma$
+    """
+
+    if shift_func is None:
+
+        def shift_func(x: torch.Tensor):
+            return (
+                torch.sqrt(torch.as_tensor(input_dim))
+                * torch.finfo(x.dtype).eps
+                * torch.linalg.norm(x)
+            )
+
+    _mat_mat_prod: Callable[[torch.Tensor], torch.Tensor]
+
+    if isinstance(mat_mat_prod, torch.Tensor):
+
+        def _mat_mat_prod(x: torch.Tensor):
+            return mat_mat_prod @ x
+
+    else:
+        _mat_mat_prod = mat_mat_prod
+
+    random_sample_matrix = torch.randn(
+        input_dim, rank, device=mat_vec_device, dtype=input_type
+    )
+    random_sample_matrix, _ = torch.linalg.qr(random_sample_matrix)
+
+    sketch_mat = _mat_mat_prod(random_sample_matrix)
+
+    shift = shift_func(sketch_mat)
+    sketch_mat += shift * random_sample_matrix
+    cholesky_mat = torch.matmul(random_sample_matrix.t(), sketch_mat)
+    try:
+        triangular_mat = torch.linalg.cholesky(cholesky_mat)
+    except _LinAlgError as e:
+        logger.warning(
+            f"Encountered error in cholesky decomposition: {e}.\n "
+            f"Increasing shift by smallest eigenvalue and re-compute"
+        )
+        eigen_vals, eigen_vectors = torch.linalg.eigh(cholesky_mat)
+        shift += torch.abs(torch.min(eigen_vals))
+        eigen_vals += shift
+        triangular_mat = torch.linalg.cholesky(
+            torch.mm(eigen_vectors, torch.mm(torch.diag(eigen_vals), eigen_vectors.T))
+        )
+
+    svd_input = torch.linalg.solve_triangular(
+        triangular_mat.t(), sketch_mat, upper=True, left=False
+    )
+    left_singular_vecs, singular_vals, _ = torch.linalg.svd(
+        svd_input, full_matrices=False
+    )
+    singular_vals = torch.clamp(singular_vals**2 - shift, min=0)
+
+    return LowRankProductRepresentation(singular_vals, left_singular_vecs)
+
+
+def model_hessian_nystroem_approximation(
+    model: torch.nn.Module,
+    loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
+    data_loader: DataLoader,
+    rank: int,
+    shift_func: Optional[Callable[[torch.Tensor], torch.Tensor]] = None,
+) -> LowRankProductRepresentation:
+    r"""
+    Given a model, loss and a data_loader, computes a random Nyström low rank approximation of
+    the corresponding Hessian matrix in factored form, i.e.
+
+    $$ H_{\text{nys}} = (H \Omega)(\Omega^T H \Omega)^{+}(H \Omega)^T
+    = U \Sigma U^T $$
+
+    Args:
+        model: A PyTorch model instance. The Hessian will be calculated with respect to
+            this model's parameters.
+        loss : A callable that computes the loss.
+        data_loader: A DataLoader instance that provides the model's training data.
+            Used in calculating the Hessian-vector products.
+        rank: rank of the approximation
+        shift_func: optional function for computing the stabilizing shift in the
+            construction of the randomized nystroem approximation, defaults to
+
+            $$ \sqrt{\operatorname{\text{input_dim}}} \cdot
+                \varepsilon(\operatorname{\text{input_type}}) \cdot \|A\Omega\|_2,$$
+
+            where $\varepsilon(\operatorname{\text{input_type}})$ is the value of the
+            machine precision corresponding to the data type.
+
+    Returns:
+        object containing, $U$ and $\Sigma$
+    """
+
+    model_hvp = create_hvp_function(
+        model, loss, data_loader, precompute_grad=False, use_average=True
+    )
+    device = next((p.device for p in model.parameters()))
+    dtype = next((p.dtype for p in model.parameters()))
+    in_dim = sum((p.numel() for p in model.parameters() if p.requires_grad))
+
+    def model_hessian_mat_mat_prod(x: torch.Tensor):
+        return torch.func.vmap(model_hvp, in_dims=1, randomness="same")(x).t()
+
+    return randomized_nystroem_approximation(
+        model_hessian_mat_mat_prod,
+        in_dim,
+        rank,
+        dtype,
+        shift_func=shift_func,
+        mat_vec_device=device,
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/torch/influence_function_model.py` & `pydvl-0.9/src/pydvl/influence/torch/influence_function_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     create_batch_hvp_function,
     create_hvp_function,
     create_matrix_jacobian_product_function,
     create_per_sample_gradient_function,
     create_per_sample_mixed_derivative_function,
     hessian,
     model_hessian_low_rank,
+    model_hessian_nystroem_approximation,
 )
+from .pre_conditioner import PreConditioner
 from .util import (
     EkfacRepresentation,
     empirical_cross_entropy_loss_fn,
     flatten_dimensions,
 )
 
 logger = logging.getLogger(__name__)
@@ -61,17 +63,24 @@
         )
         self._model_device = next(
             (p.device for p in model.parameters() if p.requires_grad)
         )
         self._model_params = {
             k: p.detach() for k, p in self.model.named_parameters() if p.requires_grad
         }
+        self._model_dtype = next(
+            (p.dtype for p in model.parameters() if p.requires_grad)
+        )
         super().__init__()
 
     @property
+    def model_dtype(self):
+        return self._model_dtype
+
+    @property
     def n_parameters(self):
         return self._n_parameters
 
     @property
     def is_thread_safe(self) -> bool:
         return False
 
@@ -107,39 +116,41 @@
         y: Optional[torch.Tensor] = None,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> torch.Tensor:
         r"""
         Compute the approximation of
 
         \[
-        \langle H^{-1}\nabla_{theta} \ell(y_{\text{test}}, f_{\theta}(x_{\text{test}})),
-            \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle
+        \langle H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
+        f_{\theta}(x_{\text{test}})), \nabla_{\theta} \ell(y, f_{\theta}(x))\rangle
         \]
 
         for the case of up-weighting influence, resp.
 
         \[
-        \langle H^{-1}\nabla_{theta} \ell(y_{\text{test}}, f_{\theta}(x_{\text{test}})),
+        \langle H^{-1}\nabla_{\theta} \ell(y_{\text{test}}, f_{\theta}(x_{\text{test}})),
             \nabla_{x} \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle
         \]
 
-        for the perturbation type influence case.
+        for the perturbation type influence case. For all input tensors it is assumed,
+        that the first dimension is the batch dimension (in case, you want to provide
+        a single sample z, call z.unsqueeze(0) if no batch dimension is present).
 
         Args:
             x_test: model input to use in the gradient computations
-                of $H^{-1}\nabla_{theta} \ell(y_{\text{test}},
+                of $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                     f_{\theta}(x_{\text{test}}))$
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
-                $\nabla_{theta}\ell(y, f_{\theta}(x))$,
-                resp. $\nabla_{x}\nabla_{theta}\ell(y, f_{\theta}(x))$,
+                $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
+                resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             Tensor representing the element-wise scalar products for the provided batch
 
         """
         t: torch.Tensor = super().influences(x_test, y_test, x, y, mode=mode)
         return t
@@ -148,22 +159,20 @@
         self,
         x_test: torch.Tensor,
         y_test: torch.Tensor,
         x: Optional[torch.Tensor] = None,
         y: Optional[torch.Tensor] = None,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> torch.Tensor:
-
         if not self.is_fitted:
             raise ValueError(
                 "Instance must be fitted before calling influence methods on it"
             )
 
         if x is None:
-
             if y is not None:
                 raise ValueError(
                     "Providing labels y, without providing model input x "
                     "is not supported"
                 )
 
             return self._symmetric_values(
@@ -208,15 +217,14 @@
         else:
             raise UnsupportedInfluenceModeException(mode)
         return values
 
     def _symmetric_values(
         self, x: torch.Tensor, y: torch.Tensor, mode: InfluenceMode
     ) -> torch.Tensor:
-
         grad = self._loss_grad(x, y)
         fac = self._solve_hvp(grad)
 
         if mode == InfluenceMode.Up:
             values = fac @ grad.T
         elif mode == InfluenceMode.Perturbation:
             values = self.influences_from_factors(fac, x, y, mode=mode)
@@ -227,27 +235,29 @@
     def influence_factors(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
         r"""
         Compute approximation of
 
         \[ H^{-1}\nabla_{\theta} \ell(y, f_{\theta}(x)) \]
 
         where the gradient is meant to be per sample of the batch $(x, y)$.
+        For all input tensors it is assumed,
+        that the first dimension is the batch dimension (in case, you want to provide
+        a single sample z, call z.unsqueeze(0) if no batch dimension is present).
 
         Args:
             x: model input to use in the gradient computations
             y: label tensor to compute gradients
 
         Returns:
             Tensor representing the element-wise inverse Hessian matrix vector products
 
         """
         return super().influence_factors(x, y)
 
     def _influence_factors(self, x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
-
         if not self.is_fitted:
             raise ValueError(
                 "Instance must be fitted before calling influence methods on it"
             )
 
         return self._solve_hvp(
             self._loss_grad(x.to(self.model_device), y.to(self.model_device))
@@ -268,26 +278,28 @@
 
         for the case of up-weighting influence, resp.
 
         \[ \langle z_{\text{test_factors}},
             \nabla_{x} \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle \]
 
         for the perturbation type influence case. The gradient is meant to be per sample
-        of the batch $(x, y)$.
+        of the batch $(x, y)$. For all input tensors it is assumed,
+        that the first dimension is the batch dimension (in case, you want to provide
+        a single sample z, call z.unsqueeze(0) if no batch dimension is present).
 
         Args:
-             z_test_factors: pre-computed tensor, approximating
+            z_test_factors: pre-computed tensor, approximating
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
-                    f_{\theta}(x_{\text{test}}))$
-             x: model input to use in the gradient computations
+                f_{\theta}(x_{\text{test}}))$
+            x: model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$
-             y: label tensor to compute gradients
-             mode: enum value of [InfluenceType]
-                [pydvl.influence.twice_differentiable.InfluenceType]
+            y: label tensor to compute gradients
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             Tensor representing the element-wise scalar products for the provided batch
 
         """
         if mode == InfluenceMode.Up:
             return (
@@ -322,15 +334,18 @@
 
 class DirectInfluence(TorchInfluenceFunctionModel):
     r"""
     Given a model and training data, it finds x such that \(Hx = b\),
     with \(H\) being the model hessian.
 
     Args:
-        model: instance of [torch.nn.Module][torch.nn.Module].
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
+        loss: A callable that takes the model's output and target as input and returns
+              the scalar loss.
         hessian_regularization: Regularization of the hessian.
     """
 
     def __init__(
         self,
         model: nn.Module,
         loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
@@ -346,22 +361,21 @@
         try:
             return self.hessian is not None
         except AttributeError:
             return False
 
     def fit(self, data: DataLoader) -> DirectInfluence:
         """
-        Compute the hessian matrix based on a provided dataloader
+        Compute the hessian matrix based on a provided dataloader.
 
         Args:
-            data: Instance of [torch.utils.data.Dataloader]
-                [torch.utils.data.Dataloader]
+            data: The data to compute the Hessian with.
 
         Returns:
-            The fitted instance
+            The fitted instance.
         """
         self.hessian = hessian(self.model, self.loss, data)
         return self
 
     @log_duration
     def influences(
         self,
@@ -393,20 +407,20 @@
                     f_{\theta}(x_{\text{test}}))$
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
-            [torch.nn.Tensor][torch.nn.Tensor] representing the element-wise
-                scalar products for the provided batch.
+            A tensor representing the element-wise scalar products for the
+                provided batch.
 
         """
         return super().influences(x_test, y_test, x, y, mode=mode)
 
     @log_duration
     def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
         return torch.linalg.solve(
@@ -426,38 +440,54 @@
     r"""
     Given a model and training data, it uses conjugate gradient to calculate the
     inverse of the Hessian Vector Product. More precisely, it finds x such that \(Hx =
     b\), with \(H\) being the model hessian. For more info, see
     [Conjugate Gradient][conjugate-gradient].
 
     Args:
-        model: Instance of [torch.nn.Module][torch.nn.Module].
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
         loss: A callable that takes the model's output and target as input and returns
               the scalar loss.
-        hessian_regularization: Regularization of the hessian.
+        hessian_regularization: Optional regularization parameter added
+            to the Hessian-vector product for numerical stability.
         x0: Initial guess for hvp. If None, defaults to b.
         rtol: Maximum relative tolerance of result.
         atol: Absolute tolerance of result.
         maxiter: Maximum number of iterations. If None, defaults to 10*len(b).
         progress: If True, display progress bars.
+        precompute_grad: If True, the full data gradient is precomputed and kept
+            in memory, which can speed up the hessian vector product computation.
+            Set this to False, if you can't afford to keep the full computation graph
+            in memory.
+        pre_conditioner: Optional pre-conditioner to improve convergence of conjugate
+            gradient method
+        use_block_cg: If True, use block variant of conjugate gradient method, which
+            solves several right hand sides simultaneously
 
     """
 
     def __init__(
         self,
         model: nn.Module,
         loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
         hessian_regularization: float = 0.0,
         x0: Optional[torch.Tensor] = None,
         rtol: float = 1e-7,
         atol: float = 1e-7,
         maxiter: Optional[int] = None,
         progress: bool = False,
+        precompute_grad: bool = False,
+        pre_conditioner: Optional[PreConditioner] = None,
+        use_block_cg: bool = False,
     ):
         super().__init__(model, loss)
+        self.use_block_cg = use_block_cg
+        self.pre_conditioner = pre_conditioner
+        self.precompute_grad = precompute_grad
         self.progress = progress
         self.maxiter = maxiter
         self.atol = atol
         self.rtol = rtol
         self.x0 = x0
         self.hessian_regularization = hessian_regularization
 
@@ -468,139 +498,268 @@
         try:
             return self.train_dataloader is not None
         except AttributeError:
             return False
 
     def fit(self, data: DataLoader) -> CgInfluence:
         self.train_dataloader = data
+        if self.pre_conditioner is not None:
+            hvp = create_hvp_function(
+                self.model,
+                self.loss,
+                self.train_dataloader,
+                precompute_grad=self.precompute_grad,
+            )
+
+            def model_hessian_mat_mat_prod(x: torch.Tensor):
+                return torch.func.vmap(hvp, in_dims=1, randomness="same")(x).t()
+
+            self.pre_conditioner.fit(
+                model_hessian_mat_mat_prod,
+                self.n_parameters,
+                self.model_dtype,
+                self.model_device,
+                self.hessian_regularization,
+            )
         return self
 
     @log_duration
     def influences(
         self,
         x_test: torch.Tensor,
         y_test: torch.Tensor,
         x: Optional[torch.Tensor] = None,
         y: Optional[torch.Tensor] = None,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> torch.Tensor:
         r"""
-        Compute approximation of
+        Compute an approximation of
 
         \[ \langle H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
             f_{\theta}(x_{\text{test}})),
             \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle, \]
 
         for the case of up-weighting influence, resp.
 
         \[ \langle H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
             f_{\theta}(x_{\text{test}})),
             \nabla_{x} \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle \]
 
-        for the perturbation type influence case. The approximate action of $H^{-1}$
-        is achieved via the [conjugate gradient method]
-        (https://en.wikipedia.org/wiki/Conjugate_gradient_method).
+        for the case of perturbation-type influence. The approximate action of
+        $H^{-1}$ is achieved via the [conjugate gradient
+        method](https://en.wikipedia.org/wiki/Conjugate_gradient_method).
 
         Args:
             x_test: model input to use in the gradient computations of
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                     f_{\theta}(x_{\text{test}}))$
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
-            [torch.nn.Tensor][torch.nn.Tensor] representing the element-wise
-                scalar products for the provided batch.
+            A tensor representing the element-wise scalar products for the
+                provided batch.
 
         """
         return super().influences(x_test, y_test, x, y, mode=mode)
 
     @log_duration
     def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
         if len(self.train_dataloader) == 0:
             raise ValueError("Training dataloader must not be empty.")
 
-        hvp = create_hvp_function(self.model, self.loss, self.train_dataloader)
+        if self.use_block_cg:
+            return self._solve_pbcg(rhs)
+
+        hvp = create_hvp_function(
+            self.model,
+            self.loss,
+            self.train_dataloader,
+            precompute_grad=self.precompute_grad,
+        )
 
         def reg_hvp(v: torch.Tensor):
             return hvp(v) + self.hessian_regularization * v.type(rhs.dtype)
 
+        y_norm = torch.linalg.norm(rhs, dim=0)
+
+        stopping_val = torch.clamp(self.rtol**2 * y_norm, min=self.atol**2)
+
         batch_cg = torch.zeros_like(rhs)
 
-        for idx, bi in enumerate(
-            tqdm(rhs, disable=not self.progress, desc="Conjugate gradient")
+        for idx, (bi, _tol) in enumerate(
+            tqdm(
+                zip(rhs, stopping_val),
+                disable=not self.progress,
+                desc="Conjugate gradient",
+            )
         ):
-            batch_result = self._solve_cg(
+            batch_result = self._solve_pcg(
                 reg_hvp,
                 bi,
+                tol=_tol,
                 x0=self.x0,
-                rtol=self.rtol,
-                atol=self.atol,
                 maxiter=self.maxiter,
             )
             batch_cg[idx] = batch_result
+
         return batch_cg
 
-    @staticmethod
-    def _solve_cg(
+    def _solve_pcg(
+        self,
         hvp: Callable[[torch.Tensor], torch.Tensor],
         b: torch.Tensor,
         *,
+        tol: float,
         x0: Optional[torch.Tensor] = None,
-        rtol: float = 1e-7,
-        atol: float = 1e-7,
         maxiter: Optional[int] = None,
     ) -> torch.Tensor:
         r"""
         Conjugate gradient solver for the Hessian vector product.
 
         Args:
             hvp: A callable Hvp, operating with tensors of size N.
             b: A vector or matrix, the right hand side of the equation \(Hx = b\).
             x0: Initial guess for hvp.
             rtol: Maximum relative tolerance of result.
             atol: Absolute tolerance of result.
             maxiter: Maximum number of iterations. If None, defaults to 10*len(b).
 
         Returns:
-            [torch.nn.Tensor][torch.nn.Tensor] representing the solution of \(Ax=b\).
+            A tensor with the solution of \(Ax=b\).
         """
 
         if x0 is None:
             x0 = torch.clone(b)
         if maxiter is None:
             maxiter = len(b) * 10
 
-        y_norm = torch.sum(torch.matmul(b, b)).item()
-        stopping_val = max([rtol**2 * y_norm, atol**2])
-
         x = x0
-        p = r = (b - hvp(x)).squeeze()
-        gamma = torch.sum(torch.matmul(r, r)).item()
+
+        r0 = b - hvp(x)
+
+        if self.pre_conditioner is not None:
+            p = z0 = self.pre_conditioner.solve(r0)
+        else:
+            p = z0 = r0
 
         for k in range(maxiter):
-            if gamma < stopping_val:
+            if torch.norm(r0) < tol:
                 break
-            Ap = hvp(p).squeeze()
-            alpha = gamma / torch.sum(torch.matmul(p, Ap)).item()
+            Ap = hvp(p)
+            alpha = torch.dot(r0, z0) / torch.dot(p, Ap)
             x += alpha * p
-            r -= alpha * Ap
-            gamma_ = torch.sum(torch.matmul(r, r)).item()
-            beta = gamma_ / gamma
-            gamma = gamma_
-            p = r + beta * p
+            r = r0 - alpha * Ap
+
+            if self.pre_conditioner is not None:
+                z = self.pre_conditioner.solve(r)
+            else:
+                z = r
+
+            beta = torch.dot(r, z) / torch.dot(r0, z0)
+
+            r0 = r
+            p = z + beta * p
+            z0 = z
 
         return x
 
+    def _solve_pbcg(
+        self,
+        rhs: torch.Tensor,
+    ):
+        hvp = create_hvp_function(
+            self.model,
+            self.loss,
+            self.train_dataloader,
+            precompute_grad=self.precompute_grad,
+        )
+
+        # The block variant of conjugate gradient is known to suffer from breakdown,
+        # due to the possibility of rank deficiency of the iterates of the parameter
+        # matrix P^tAP, which destabilizes the direct solver.
+        # The paper `Randomized Nyström Preconditioning,
+        # Frangella, Zachary and Tropp, Joel A. and Udell, Madeleine,
+        # SIAM J. Matrix Anal. Appl., 2023`
+        # proposes a simple orthogonalization pre-processing. However, we observed, that
+        # this stabilization only worked for double precision. We thus implement
+        # a different stabilization strategy described in
+        # `A breakdown-free block conjugate gradient method, Ji, Hao and Li, Yaohang,
+        # BIT Numerical Mathematics, 2017`
+
+        def mat_mat(x: torch.Tensor):
+            return torch.vmap(
+                lambda u: hvp(u) + self.hessian_regularization * u,
+                in_dims=1,
+                randomness="same",
+            )(x)
+
+        X = torch.clone(rhs.T)
+
+        R = (rhs - mat_mat(X)).T
+        Z = R if self.pre_conditioner is None else self.pre_conditioner.solve(R)
+        P, _, _ = torch.linalg.svd(Z, full_matrices=False)
+        active_indices = torch.as_tensor(list(range(X.shape[-1])), dtype=torch.long)
+
+        maxiter = self.maxiter if self.maxiter is not None else len(rhs) * 10
+        y_norm = torch.linalg.norm(rhs, dim=1)
+        tol = torch.clamp(self.rtol**2 * y_norm, min=self.atol**2)
+
+        # In the case the parameter dimension is smaller than the number of right
+        # hand sides, we do not shrink the indices due to resulting wrong
+        # dimensionality of the svd decomposition. We consider this an edge case, which
+        # does not need optimization
+        shrink_finished_indices = rhs.shape[0] <= rhs.shape[1]
+
+        for k in range(maxiter):
+            Q = mat_mat(P).T
+            p_t_ap = P.T @ Q
+            alpha = torch.linalg.solve(p_t_ap, P.T @ R)
+            X[:, active_indices] += P @ alpha
+            R -= Q @ alpha
+
+            B = torch.linalg.norm(R, dim=0)
+            non_finished_indices = torch.nonzero(B > tol)
+            num_remaining_indices = non_finished_indices.numel()
+            non_finished_indices = non_finished_indices.squeeze()
+
+            if num_remaining_indices == 1:
+                non_finished_indices = non_finished_indices.unsqueeze(-1)
+
+            if num_remaining_indices == 0:
+                break
+
+            # Reduce problem size by removing finished columns from the iteration
+            if shrink_finished_indices:
+                active_indices = active_indices[non_finished_indices]
+                R = R[:, non_finished_indices]
+                P = P[:, non_finished_indices]
+                Q = Q[:, non_finished_indices]
+                p_t_ap = p_t_ap[:, non_finished_indices][non_finished_indices, :]
+                tol = tol[non_finished_indices]
+
+            Z = R if self.pre_conditioner is None else self.pre_conditioner.solve(R)
+            beta = -torch.linalg.solve(p_t_ap, Q.T @ Z)
+            Z_tmp = Z + P @ beta
+
+            if Z_tmp.ndim == 1:
+                Z_tmp = Z_tmp.unsqueeze(-1)
+
+            # Orthogonalization search directions to stabilize the action of
+            # (P^tAP)^{-1}
+            P, _, _ = torch.linalg.svd(Z_tmp, full_matrices=False)
+
+        return X.T
+
 
 class LissaInfluence(TorchInfluenceFunctionModel):
     r"""
     Uses LISSA, Linear time Stochastic Second-Order Algorithm, to iteratively
     approximate the inverse Hessian. More precisely, it finds x s.t. \(Hx = b\),
     with \(H\) being the model's second derivative wrt. the parameters.
     This is done with the update
@@ -609,16 +768,20 @@
 
     where \(I\) is the identity matrix, \(d\) is a dampening term and \(s\) a scaling
     factor that are applied to help convergence. For details,
     see [Linear time Stochastic Second-Order Approximation (LiSSA)]
     [linear-time-stochastic-second-order-approximation-lissa]
 
     Args:
-        model: instance of [torch.nn.Module][torch.nn.Module].
-        hessian_regularization: Regularization of the hessian.
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
+        loss: A callable that takes the model's output and target as input and returns
+              the scalar loss.
+        hessian_regularization: Optional regularization parameter added
+            to the Hessian-vector product for numerical stability.
         maxiter: Maximum number of iterations.
         dampen: Dampening factor, defaults to 0 for no dampening.
         scale: Scaling factor, defaults to 10.
         h0: Initial guess for hvp.
         rtol: tolerance to use for early stopping
         progress: If True, display progress bars.
     """
@@ -655,15 +818,14 @@
 
     def fit(self, data: DataLoader) -> LissaInfluence:
         self.train_dataloader = data
         return self
 
     @log_duration
     def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
-
         h_estimate = self.h0 if self.h0 is not None else torch.clone(rhs)
 
         shuffled_training_data = DataLoader(
             self.train_dataloader.dataset,
             self.train_dataloader.batch_size,
             shuffle=True,
         )
@@ -688,15 +850,16 @@
         }
         b_hvp = torch.vmap(
             create_batch_hvp_function(self.model, self.loss),
             in_dims=(None, None, None, 0),
         )
         for _ in tqdm(range(self.maxiter), disable=not self.progress, desc="Lissa"):
             x, y = next(iter(shuffled_training_data))
-            # grad_xy = model.grad(x, y, create_graph=True)
+            x = x.to(self.model_device)
+            y = y.to(self.model_device)
             reg_hvp = (
                 lambda v: b_hvp(model_params, x, y, v) + self.hessian_regularization * v
             )
             residual = lissa_step(h_estimate, reg_hvp) - h_estimate
             h_estimate += residual
             if torch.isnan(h_estimate).any():
                 raise RuntimeError("NaNs in h_estimate. Increase scale or dampening.")
@@ -725,16 +888,18 @@
 
     where \(D\) is a diagonal matrix with the top (in absolute value) `rank_estimate`
     eigenvalues of the Hessian
     and \(V\) contains the corresponding eigenvectors.
     For more information, see [Arnoldi][arnoldi].
 
     Args:
-        model: Instance of [torch.nn.Module][torch.nn.Module].
-            The Hessian will be calculated with respect to this model's parameters.
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
+        loss: A callable that takes the model's output and target as input and returns
+              the scalar loss.
         hessian_regularization: Optional regularization parameter added
             to the Hessian-vector product for numerical stability.
         rank_estimate: The number of eigenvalues and corresponding eigenvectors
             to compute. Represents the desired rank of the Hessian approximation.
         krylov_dimension: The number of Krylov vectors to use for the Lanczos method.
             Defaults to min(model's number of parameters,
             max(2 times rank_estimate + 1, 20)).
@@ -744,36 +909,41 @@
             Ignored if `low_rank_representation` is provided.
         eigen_computation_on_gpu: If True, tries to execute the eigen pair approximation
             on the model's device
             via a cupy implementation. Ensure the model size or rank_estimate
             is appropriate for device memory.
             If False, the eigen pair approximation is executed on the CPU by the scipy
             wrapper to ARPACK.
+        precompute_grad: If True, the full data gradient is precomputed and kept
+            in memory, which can speed up the hessian vector product computation.
+            Set this to False, if you can't afford to keep the full computation graph
+            in memory.
     """
     low_rank_representation: LowRankProductRepresentation
 
     def __init__(
         self,
-        model,
-        loss,
+        model: nn.Module,
+        loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
         hessian_regularization: float = 0.0,
         rank_estimate: int = 10,
         krylov_dimension: Optional[int] = None,
         tol: float = 1e-6,
         max_iter: Optional[int] = None,
         eigen_computation_on_gpu: bool = False,
+        precompute_grad: bool = False,
     ):
-
         super().__init__(model, loss)
         self.hessian_regularization = hessian_regularization
         self.rank_estimate = rank_estimate
         self.tol = tol
         self.max_iter = max_iter
         self.krylov_dimension = krylov_dimension
         self.eigen_computation_on_gpu = eigen_computation_on_gpu
+        self.precompute_grad = precompute_grad
 
     @property
     def is_fitted(self):
         try:
             return self.low_rank_representation is not None
         except AttributeError:
             return False
@@ -783,117 +953,119 @@
         Fitting corresponds to the computation of the low rank decomposition
 
         \[ V D^{-1} V^T \]
 
         of the Hessian defined by the provided data loader.
 
         Args:
-            data: Instance of [torch.utils.data.Dataloader][torch.utils.data.Dataloader]
+            data: The data to compute the Hessian with.
 
         Returns:
-            The fitted instance
+            The fitted instance.
 
         """
         low_rank_representation = model_hessian_low_rank(
             self.model,
             self.loss,
             data,
             hessian_perturbation=0.0,  # regularization is applied, when computing values
             rank_estimate=self.rank_estimate,
             krylov_dimension=self.krylov_dimension,
             tol=self.tol,
             max_iter=self.max_iter,
             eigen_computation_on_gpu=self.eigen_computation_on_gpu,
+            precompute_grad=self.precompute_grad,
         )
         self.low_rank_representation = low_rank_representation.to(self.model_device)
         return self
 
     def _non_symmetric_values(
         self,
         x_test: torch.Tensor,
         y_test: torch.Tensor,
         x: torch.Tensor,
         y: torch.Tensor,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> torch.Tensor:
-
         if mode == InfluenceMode.Up:
             mjp = create_matrix_jacobian_product_function(
                 self.model, self.loss, self.low_rank_representation.projections.T
             )
             left = mjp(self.model_params, x_test, y_test)
 
-            regularized_eigenvalues = (
+            inverse_regularized_eigenvalues = 1.0 / (
                 self.low_rank_representation.eigen_vals + self.hessian_regularization
             )
 
-            right = torch.diag_embed(1.0 / regularized_eigenvalues) @ mjp(
+            right = mjp(
                 self.model_params, x, y
-            )
+            ) * inverse_regularized_eigenvalues.unsqueeze(-1)
             values = torch.einsum("ij, ik -> jk", left, right)
         elif mode == InfluenceMode.Perturbation:
             factors = self.influence_factors(x_test, y_test)
             values = self.influences_from_factors(factors, x, y, mode=mode)
         else:
             raise UnsupportedInfluenceModeException(mode)
         return values
 
     def _symmetric_values(
         self, x: torch.Tensor, y: torch.Tensor, mode: InfluenceMode
     ) -> torch.Tensor:
-
         if mode == InfluenceMode.Up:
             left = create_matrix_jacobian_product_function(
                 self.model, self.loss, self.low_rank_representation.projections.T
             )(self.model_params, x, y)
-            regularized_eigenvalues = (
+            inverse_regularized_eigenvalues = 1.0 / (
                 self.low_rank_representation.eigen_vals + self.hessian_regularization
             )
-            right = torch.diag_embed(1.0 / regularized_eigenvalues) @ left
+            right = left * inverse_regularized_eigenvalues.unsqueeze(-1)
             values = torch.einsum("ij, ik -> jk", left, right)
         elif mode == InfluenceMode.Perturbation:
             factors = self.influence_factors(x, y)
             values = self.influences_from_factors(factors, x, y, mode=mode)
         else:
             raise UnsupportedInfluenceModeException(mode)
         return values
 
     @log_duration
     def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
-
-        regularized_eigenvalues = (
+        inverse_regularized_eigenvalues = 1.0 / (
             self.low_rank_representation.eigen_vals + self.hessian_regularization
         )
 
+        projected_rhs = self.low_rank_representation.projections.t() @ rhs.t()
         result = self.low_rank_representation.projections @ (
-            torch.diag_embed(1.0 / regularized_eigenvalues)
-            @ (self.low_rank_representation.projections.t() @ rhs.t())
+            projected_rhs * inverse_regularized_eigenvalues.unsqueeze(-1)
         )
 
         return result.t()
 
     def to(self, device: torch.device):
         if self.is_fitted:
             self.low_rank_representation = self.low_rank_representation.to(device)
         return super().to(device)
 
 
 class EkfacInfluence(TorchInfluenceFunctionModel):
     r"""
-    Approximately solves the linear system Hx = b, where H is the Hessian of a model with the empirical
-    categorical cross entropy as loss function and b is the given right-hand side vector.
-    It employs the EK-FAC method [@george2018fast], which is based on the kronecker
-    factorization of the Hessian first introduced in [@martens2015optimizing].
+    Approximately solves the linear system Hx = b, where H is the Hessian of a model
+    with the empirical categorical cross entropy as loss function and b is the given
+    right-hand side vector.
+    It employs the EK-FAC method, which is based on the kronecker
+    factorization of the Hessian.
+
     Contrary to the other influence function methods, this implementation can only
     be used for classification tasks with a cross entropy loss function. However, it
     is much faster than the other methods and can be used efficiently for very large
-    datasets and models. For more information, see [Eigenvalue Corrected K-FAC][ekfac].
+    datasets and models. For more information,
+    see [Eigenvalue Corrected K-FAC][eigenvalue-corrected-k-fac].
 
     Args:
-        model: Instance of [torch.nn.Module][torch.nn.Module].
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
         update_diagonal: If True, the diagonal values in the ekfac representation are
             refitted from the training data after calculating the KFAC blocks.
             This provides a more accurate approximation of the Hessian, but it is
             computationally more expensive.
         hessian_regularization: Regularization of the hessian.
         progress: If True, display progress bars.
     """
@@ -903,15 +1075,14 @@
     def __init__(
         self,
         model: nn.Module,
         update_diagonal: bool = False,
         hessian_regularization: float = 0.0,
         progress: bool = False,
     ):
-
         super().__init__(model, torch.nn.functional.cross_entropy)
         self.hessian_regularization = hessian_regularization
         self.update_diagonal = update_diagonal
         self.active_layers = self._parse_active_layers()
         self.progress = progress
 
     @property
@@ -1219,41 +1390,40 @@
         self,
         x_test: torch.Tensor,
         y_test: torch.Tensor,
         x: Optional[torch.Tensor] = None,
         y: Optional[torch.Tensor] = None,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> Dict[str, torch.Tensor]:
-        """
+        r"""
         Compute the influence of the data on the test data for each layer of the model.
 
         Args:
             x_test: model input to use in the gradient computations of
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
                     f_{\theta}(x_{\text{test}}))$
             y_test: label tensor to compute gradients
             x: optional model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 if None, use $x=x_{\text{test}}$
             y: optional label tensor to compute gradients
-            mode: enum value of [InfluenceType]
-                [pydvl.influence.base_influence_model.InfluenceType]
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
             A dictionary containing the influence of the data on the test data for each
             layer of the model, with the layer name as key.
         """
         if not self.is_fitted:
             raise ValueError(
                 "Instance must be fitted before calling influence methods on it"
             )
 
         if x is None:
-
             if y is not None:
                 raise ValueError(
                     "Providing labels y, without providing model input x "
                     "is not supported"
                 )
 
             return self._symmetric_values_by_layer(
@@ -1276,18 +1446,18 @@
         )
 
     def influence_factors_by_layer(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
     ) -> Dict[str, torch.Tensor]:
-        """
+        r"""
         Computes the approximation of
 
-        \[H^{-1}\nabla_{\theta} \ell(y, f_{\theta}(x))\]
+        \[ H^{-1}\nabla_{\theta} \ell(y, f_{\theta}(x)) \]
 
         for each layer of the model separately.
 
         Args:
             x: model input to use in the gradient computations
             y: label tensor to compute gradients
 
@@ -1309,42 +1479,43 @@
     def influences_from_factors_by_layer(
         self,
         z_test_factors: Dict[str, torch.Tensor],
         x: torch.Tensor,
         y: torch.Tensor,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> Dict[str, torch.Tensor]:
-        """
+        r"""
         Computation of
 
         \[ \langle z_{\text{test_factors}},
             \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle \]
 
         for the case of up-weighting influence, resp.
 
         \[ \langle z_{\text{test_factors}},
             \nabla_{x} \nabla_{\theta} \ell(y, f_{\theta}(x)) \rangle \]
 
-        for the perturbation type influence case for each layer of the model separately.
-        The gradients are meant to be per sample of the batch $(x, y)$.
+        for the perturbation type influence case for each layer of the model
+        separately. The gradients are meant to be per sample of the batch $(x,
+        y)$.
 
         Args:
             z_test_factors: pre-computed tensor, approximating
                 $H^{-1}\nabla_{\theta} \ell(y_{\text{test}},
-                    f_{\theta}(x_{\text{test}}))$
-             x: model input to use in the gradient computations
+                f_{\theta}(x_{\text{test}}))$
+            x: model input to use in the gradient computations
                 $\nabla_{\theta}\ell(y, f_{\theta}(x))$,
                 resp. $\nabla_{x}\nabla_{\theta}\ell(y, f_{\theta}(x))$
-             y: label tensor to compute gradients
-             mode: enum value of [InfluenceType]
-                [pydvl.influence.twice_differentiable.InfluenceType]
+            y: label tensor to compute gradients
+            mode: enum value of [InfluenceMode]
+                [pydvl.influence.base_influence_function_model.InfluenceMode]
 
         Returns:
-            A dictionary containing the influence of the data on the test data for each
-            layer of the model, with the layer name as key.
+            A dictionary containing the influence of the data on the test data
+            for each layer of the model, with the layer name as key.
         """
         if mode == InfluenceMode.Up:
             total_grad = self._loss_grad(
                 x.to(self.model_device), y.to(self.model_device)
             )
             start_idx = 0
             influences = {}
@@ -1376,17 +1547,17 @@
         x_test: torch.Tensor,
         y_test: torch.Tensor,
         x: torch.Tensor,
         y: torch.Tensor,
         mode: InfluenceMode = InfluenceMode.Up,
     ) -> Dict[str, torch.Tensor]:
         """
-        Similar to _non_symmetric_values, but computes the influence for each layer
-        separately. Returns a dictionary containing the influence for each layer,
-        with the layer name as key.
+        Similar to `_non_symmetric_values`, but computes the influence for each
+        layer separately. Returns a dictionary containing the influence for each
+        layer, with the layer name as key.
         """
         if mode == InfluenceMode.Up:
             if x_test.shape[0] <= x.shape[0]:
                 fac = self.influence_factors_by_layer(x_test, y_test)
                 values = self.influences_from_factors_by_layer(fac, x, y, mode=mode)
             else:
                 fac = self.influence_factors_by_layer(x, y)
@@ -1400,15 +1571,15 @@
             raise UnsupportedInfluenceModeException(mode)
         return values
 
     def _symmetric_values_by_layer(
         self, x: torch.Tensor, y: torch.Tensor, mode: InfluenceMode
     ) -> Dict[str, torch.Tensor]:
         """
-        Similar to _symmetric_values, but computes the influence for each layer
+        Similar to `_symmetric_values`, but computes the influence for each layer
         separately. Returns a dictionary containing the influence for each layer,
         with the layer name as key.
         """
         grad = self._loss_grad(x, y)
         fac = self._solve_hvp_by_layer(
             grad, self.ekfac_representation, self.hessian_regularization
         )
@@ -1465,7 +1636,84 @@
             influences_by_reg_value[reg_value] = values
         return influences_by_reg_value
 
     def to(self, device: torch.device):
         if self.is_fitted:
             self.ekfac_representation.to(device)
         return super().to(device)
+
+
+class NystroemSketchInfluence(TorchInfluenceFunctionModel):
+    r"""
+    Given a model and training data, it uses a low-rank approximation of the Hessian
+    (derived via random projection Nyström approximation) in combination with
+    the [Sherman–Morrison–Woodbury
+    formula](https://en.wikipedia.org/wiki/Woodbury_matrix_identity) to
+    calculate the inverse of the Hessian Vector Product. More concrete, it
+    computes a low-rank approximation
+
+    \begin{align*}
+        H_{\text{nys}} &= (H\Omega)(\Omega^TH\Omega)^{+}(H\Omega)^T \\\
+                       &= U \Lambda U^T
+    \end{align*}
+
+    in factorized form and approximates the action of the inverse Hessian via
+
+    \[ (H_{\text{nys}} + \lambda I)^{-1} = U(\Lambda+\lambda I)U^T +
+        \frac{1}{\lambda}(I−UU^T). \]
+
+    Args:
+        model: A PyTorch model. The Hessian will be calculated with respect to
+            this model's parameters.
+        loss: A callable that takes the model's output and target as input and returns
+              the scalar loss.
+        hessian_regularization: Optional regularization parameter added
+            to the Hessian-vector product for numerical stability.
+        rank: rank of the low-rank approximation
+
+    """
+
+    low_rank_representation: LowRankProductRepresentation
+
+    def __init__(
+        self,
+        model: torch.nn.Module,
+        loss: Callable[[torch.Tensor, torch.Tensor], torch.Tensor],
+        hessian_regularization: float,
+        rank: int,
+    ):
+        super().__init__(model, loss)
+        self.hessian_regularization = hessian_regularization
+        self.rank = rank
+
+    def _solve_hvp(self, rhs: torch.Tensor) -> torch.Tensor:
+        regularized_eigenvalues = (
+            self.low_rank_representation.eigen_vals + self.hessian_regularization
+        )
+
+        proj_rhs = self.low_rank_representation.projections.t() @ rhs.t()
+        inverse_regularized_eigenvalues = 1.0 / regularized_eigenvalues
+        result = self.low_rank_representation.projections @ (
+            proj_rhs * inverse_regularized_eigenvalues.unsqueeze(-1)
+        )
+
+        if self.hessian_regularization > 0.0:
+            result += (
+                1.0
+                / self.hessian_regularization
+                * (rhs.t() - self.low_rank_representation.projections @ proj_rhs)
+            )
+
+        return result.t()
+
+    @property
+    def is_fitted(self):
+        try:
+            return self.low_rank_representation is not None
+        except AttributeError:
+            return False
+
+    def fit(self, data: DataLoader):
+        self.low_rank_representation = model_hessian_nystroem_approximation(
+            self.model, self.loss, data, self.rank
+        )
+        return self
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyDVL-0.8.1/src/pydvl/influence/torch/util.py` & `pydvl-0.9/src/pydvl/influence/torch/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     Dict,
     Generator,
     Iterable,
     List,
     Mapping,
     Optional,
     Tuple,
+    Type,
     Union,
 )
 
 import dask
 import numpy as np
 import torch
 from dask import array as da
@@ -131,40 +132,35 @@
     Raises:
         ValueError: If `target` cannot be harmonized to match `source`.
     """
 
     tangent_dict: Dict[str, torch.Tensor]
 
     if isinstance(target, dict):
-
         if list(target.keys()) != list(source.keys()):
             raise ValueError("The keys in 'target' do not match the keys in 'source'.")
 
         if [v.shape for v in target.values()] != [v.shape for v in source.values()]:
-
             raise ValueError(
                 "The shapes of the values in 'target' do not match the shapes "
                 "of the values in 'source'."
             )
 
         tangent_dict = target
 
     elif isinstance(target, tuple) or isinstance(target, list):
-
         if [v.shape for v in target] != [v.shape for v in source.values()]:
-
             raise ValueError(
                 "'target' is a tuple/list but its elements' shapes do not match "
                 "the shapes of the values in 'source'."
             )
 
         tangent_dict = dict(zip(source.keys(), target))
 
     elif isinstance(target, torch.Tensor):
-
         try:
             tangent_dict = dict(
                 zip(
                     source.keys(),
                     reshape_vector_to_tensors(
                         target, [p.shape for p in source.values()]
                     ),
@@ -245,15 +241,15 @@
     )
 
 
 def torch_dataset_to_dask_array(
     dataset: Dataset,
     chunk_size: int,
     total_size: Optional[int] = None,
-    resulting_dtype=np.float32,
+    resulting_dtype: Type[np.number] = np.float32,
 ) -> Tuple[da.Array, ...]:
     """
     Construct tuple of dask arrays from a PyTorch dataset, using dask.delayed
 
     Args:
         dataset: A PyTorch [dataset][torch.utils.data.Dataset]
         chunk_size: The size of the chunks for the resulting Dask arrays.
@@ -346,15 +342,14 @@
         for (start, stop) in chunk_indices
     ]
 
     delayed_arrays_dict: Dict[int, List[da.Array]] = {k: [] for k in range(len(sample))}
 
     for chunk, (start, stop) in zip(delayed_chunks, chunk_indices):
         for tensor_idx, sample_tensor in enumerate(sample):
-
             delayed_tensor = da.from_delayed(
                 dask.delayed(lambda t: t.cpu().numpy())(chunk[tensor_idx]),
                 shape=(stop - start, *sample_tensor.shape),
                 dtype=resulting_dtype,
             )
 
             delayed_arrays_dict[tensor_idx].append(delayed_tensor)
```

### Comparing `pyDVL-0.8.1/src/pydvl/parallel/__init__.py` & `pydvl-0.9/src/pydvl/parallel/futures/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,58 @@
-"""
-This module provides a common interface to parallelization backends. The list of
-supported backends is [here][pydvl.parallel.backends]. Backends can be
-selected with the `backend` argument of an instance of
-[ParallelConfig][pydvl.utils.config.ParallelConfig], as seen in the examples
-below.
-
-We use [executors][concurrent.futures.Executor] to submit tasks in parallel. The
-basic high-level pattern is
-
-```python
-from pydvl.parallel import init_executor, ParallelConfig
-
-config = ParallelConfig(backend="ray")
-with init_executor(max_workers=1, config=config) as executor:
-    future = executor.submit(lambda x: x + 1, 1)
-    result = future.result()
-assert result == 2
-```
-
-Running a map-reduce job is also easy:
-
-```python
-from pydvl.parallel import init_executor, ParallelConfig
-
-config = ParallelConfig(backend="joblib")
-with init_executor(config=config) as executor:
-    results = list(executor.map(lambda x: x + 1, range(5)))
-assert results == [1, 2, 3, 4, 5]
-```
-
-There is an alternative map-reduce implementation
-[MapReduceJob][pydvl.parallel.map_reduce.MapReduceJob] which internally
-uses joblib's higher level API with `Parallel()`
-"""
-# HACK to avoid circular imports
-from ..utils.types import *  # pylint: disable=wrong-import-order
-from .backend import *
-from .backends import *
-from .config import *
-from .futures import *
-from .map_reduce import *
-
-if len(BaseParallelBackend.BACKENDS) == 0:
-    raise ImportError("No parallel backend found. Please install ray or joblib.")
+from concurrent.futures import Executor
+from contextlib import contextmanager
+from typing import Generator, Optional
+
+from deprecate import deprecated
+
+from pydvl.parallel.backend import ParallelBackend
+from pydvl.parallel.config import ParallelConfig
+
+__all__ = ["init_executor"]
+
+
+# TODO: delete this function once it's made redundant in v0.10.0
+# This string for the benefit of deprecation searches:
+# remove_in="0.10.0"
+@contextmanager
+@deprecated(
+    target=None,
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
+def init_executor(
+    max_workers: Optional[int] = None,
+    config: ParallelConfig = ParallelConfig(),
+    **kwargs,
+) -> Generator[Executor, None, None]:
+    """Initializes a futures executor for the given parallel configuration.
+
+    Args:
+        max_workers: Maximum number of concurrent tasks.
+        config: instance of [ParallelConfig][pydvl.utils.config.ParallelConfig]
+            with cluster address, number of cpus, etc.
+        kwargs: Other optional parameter that will be passed to the executor.
+
+
+    ??? Examples
+        ``` python
+        from pydvl.parallel.futures import init_executor, ParallelConfig
+
+        config = ParallelConfig(backend="ray")
+        with init_executor(max_workers=1, config=config) as executor:
+            future = executor.submit(lambda x: x + 1, 1)
+            result = future.result()
+        assert result == 2
+        ```
+        ``` python
+        from pydvl.parallel.futures import init_executor
+        with init_executor() as executor:
+            results = list(executor.map(lambda x: x + 1, range(5)))
+        assert results == [1, 2, 3, 4, 5]
+        ```
+    """
+    try:
+        cls = ParallelBackend.BACKENDS[config.backend]
+        with cls.executor(max_workers=max_workers, config=config, **kwargs) as e:
+            yield e
+    except KeyError:
+        raise NotImplementedError(f"Unexpected parallel backend {config.backend}")
```

### Comparing `pyDVL-0.8.1/src/pydvl/parallel/futures/ray.py` & `pydvl-0.9/src/pydvl/parallel/futures/ray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 import logging
 import queue
 import sys
 import threading
 import time
 import types
 from concurrent.futures import Executor, Future
-from typing import Any, Callable, Optional, TypeVar
+from typing import Any, Callable, Optional, TypeVar, Union
 from weakref import WeakSet, ref
 
-import ray
+from deprecate import deprecated
 
+try:
+    import ray
+except ModuleNotFoundError as e:
+    raise ModuleNotFoundError(
+        f"Cannot use RayExecutor because ray was not installed. "
+        f"Make sure to install pyDVL using `pip install pyDVL[ray]`. \n"
+        f"Original error: {e}"
+    )
+
+from pydvl.parallel import CancellationPolicy
 from pydvl.parallel.config import ParallelConfig
 
 __all__ = ["RayExecutor"]
 
-from pydvl.parallel import CancellationPolicy
-
 T = TypeVar("T")
 
 logger = logging.getLogger(__name__)
 
 
 class RayExecutor(Executor):
     """Asynchronous executor using Ray that implements the concurrent.futures API.
 
-    It shouldn't be initialized directly. You should instead call
-    [init_executor()][pydvl.parallel.futures.init_executor].
-
     Args:
         max_workers: Maximum number of concurrent tasks. Each task can request
             itself any number of vCPUs. You must ensure the product of this
             value and the n_cpus_per_job parameter passed to submit() does not
             exceed available cluster resources. If set to `None`, it will
             default to the total number of vCPUs in the ray cluster.
-        config: instance of [ParallelConfig][pydvl.utils.config.ParallelConfig]
-            with cluster address, number of cpus, etc.
         cancel_futures: Select which futures will be cancelled when exiting this
             context manager. `Pending` is the default, which will cancel all
             pending futures, but not running ones, as done by
             [concurrent.futures.ProcessPoolExecutor][]. Additionally, `All`
             cancels all pending and running futures, and `None` doesn't cancel
             any. See [CancellationPolicy][pydvl.parallel.backend.CancellationPolicy]
     """
 
+    @deprecated(
+        target=True,
+        args_mapping={"config": None},
+        deprecated_in="0.9.0",
+        remove_in="0.10.0",
+    )
     def __init__(
         self,
         max_workers: Optional[int] = None,
         *,
-        config: ParallelConfig = ParallelConfig(),
-        cancel_futures: CancellationPolicy = CancellationPolicy.ALL,
+        config: Optional[ParallelConfig] = None,
+        cancel_futures: Union[CancellationPolicy, bool] = CancellationPolicy.ALL,
     ):
-        if config.backend != "ray":
-            raise ValueError(
-                f"Parallel backend must be set to 'ray' and not '{config.backend}'"
-            )
         if max_workers is not None:
             if max_workers <= 0:
                 raise ValueError("max_workers must be greater than 0")
             max_workers = max_workers
 
         if isinstance(cancel_futures, CancellationPolicy):
             self._cancel_futures = cancel_futures
         else:
             self._cancel_futures = (
                 CancellationPolicy.PENDING
                 if cancel_futures
                 else CancellationPolicy.NONE
             )
 
-        self.config = {"address": config.address, "logging_level": config.logging_level}
-        if config.address is None:
-            self.config["num_cpus"] = config.n_cpus_local
-
         if not ray.is_initialized():
-            ray.init(**self.config)
+            raise RuntimeError(
+                "Starting from v0.9.0, ray is no longer automatically initialized. "
+                "Please use `ray.init()` with the desired configuration "
+                "before using this class."
+            )
 
         self._max_workers = max_workers
         if self._max_workers is None:
             self._max_workers = int(ray._private.state.cluster_resources()["CPU"])
 
         self._shutdown = False
         self._shutdown_lock = threading.Lock()
```

### Comparing `pyDVL-0.8.1/src/pydvl/parallel/map_reduce.py` & `pydvl-0.9/src/pydvl/parallel/map_reduce.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 This module contains a wrapper around joblib's `Parallel()` class that makes it
 easy to run map-reduce jobs.
 
 !!! Deprecation notice
     This interface might be deprecated or changed in a future release before 1.0
 
 """
+import warnings
 from functools import reduce
 from itertools import accumulate, repeat
 from typing import Any, Collection, Dict, Generic, List, Optional, TypeVar, Union
 
+from deprecate import deprecated
 from joblib import Parallel, delayed
 from numpy.random import SeedSequence
 from numpy.typing import NDArray
 
 from ..utils.functional import maybe_add_argument
 from ..utils.types import MapFunction, ReduceFunction, Seed, ensure_seed_sequence
-from .backend import init_parallel_backend
+from .backend import ParallelBackend, _maybe_init_parallel_backend
 from .config import ParallelConfig
 
 __all__ = ["MapReduceJob"]
 
 T = TypeVar("T")
 R = TypeVar("R")
 
@@ -42,15 +44,20 @@
         map_func: Function that will be applied to the input chunks in each job.
         reduce_func: Function that will be applied to the results of
             `map_func` to reduce them.
         map_kwargs: Keyword arguments that will be passed to `map_func` in
             each job. Alternatively, one can use [functools.partial][].
         reduce_kwargs: Keyword arguments that will be passed to `reduce_func`
             in each job. Alternatively, one can use [functools.partial][].
-        config: Instance of [ParallelConfig][pydvl.utils.config.ParallelConfig]
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
             with cluster address, number of cpus, etc.
         n_jobs: Number of parallel jobs to run. Does not accept 0
 
     ??? Example
         A simple usage example with 2 jobs:
 
         ``` pycon
@@ -77,32 +84,40 @@
         ...     n_jobs=2,
         ... )
         >>> map_reduce_job()
         10
         ```
     """
 
+    @deprecated(
+        target=True,
+        args_mapping={"config": "config"},
+        deprecated_in="0.9.0",
+        remove_in="0.10.0",
+    )
     def __init__(
         self,
         inputs: Union[Collection[T], T],
         map_func: MapFunction[R],
         reduce_func: ReduceFunction[R] = identity,
+        parallel_backend: Optional[ParallelBackend] = None,
+        config: Optional[ParallelConfig] = None,
+        *,
         map_kwargs: Optional[Dict] = None,
         reduce_kwargs: Optional[Dict] = None,
-        config: ParallelConfig = ParallelConfig(),
-        *,
         n_jobs: int = -1,
         timeout: Optional[float] = None,
     ):
-        self.config = config
-        parallel_backend = init_parallel_backend(self.config)
+        parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
         self.parallel_backend = parallel_backend
 
         self.timeout = timeout
 
+        self._n_jobs = -1
         # This uses the setter defined below
         self.n_jobs = n_jobs
 
         self.inputs_ = inputs
 
         self.map_kwargs = map_kwargs if map_kwargs is not None else dict()
         self.reduce_kwargs = reduce_kwargs if reduce_kwargs is not None else dict()
@@ -120,25 +135,29 @@
         Args:
             seed: Either an instance of a numpy random number generator or a seed for
                 it.
 
         Returns:
              The result of the reduce function.
         """
-        parallel_kwargs: Dict[str, Any] = {"n_jobs": self.n_jobs}
-        if self.config.backend == "joblib":
-            parallel_kwargs["backend"] = "loky"
-        else:
-            parallel_kwargs["backend"] = self.config.backend
-        # In joblib the levels are reversed.
-        # 0 means no logging and 50 means log everything to stdout
-        if self.config.logging_level is not None:
-            parallel_kwargs["verbose"] = 50 - self.config.logging_level
         seed_seq = ensure_seed_sequence(seed)
-        with Parallel(**parallel_kwargs) as parallel:
+
+        if hasattr(self.parallel_backend, "_joblib_backend_name"):
+            backend = getattr(self.parallel_backend, "_joblib_backend_name")
+        else:
+            warnings.warn(
+                "Parallel backend "
+                f"{self.parallel_backend.__class__.__name__}. "
+                "should have a `_joblib_backend_name` attribute in order to work "
+                "property with MapReduceJob. "
+                "Defaulting to joblib loky backend"
+            )
+            backend = "loky"
+
+        with Parallel(backend=backend, prefer="processes") as parallel:
             chunks = self._chunkify(self.inputs_, n_chunks=self.n_jobs)
             map_results: List[R] = parallel(
                 delayed(self._map_func)(
                     next_chunk, job_id=j, seed=seed, **self.map_kwargs
                 )
                 for j, (next_chunk, seed) in enumerate(
                     zip(chunks, seed_seq.spawn(len(chunks)))
```

### Comparing `pyDVL-0.8.1/src/pydvl/reporting/plots.py` & `pydvl-0.9/src/pydvl/reporting/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,15 @@
     df: pd.DataFrame,
     *,
     level: float = 0.05,
     ax: Optional[plt.Axes] = None,
     title: Optional[str] = None,
     xlabel: Optional[str] = None,
     ylabel: Optional[str] = None,
+    prefix: Optional[str] = "data_value",
 ) -> plt.Axes:
     r"""Plots the shapley values, as returned from
     [compute_shapley_values][pydvl.value.shapley.common.compute_shapley_values],
     with error bars corresponding to an $\alpha$-level Normal confidence
     interval.
 
     Args:
@@ -256,17 +257,17 @@
 
     Returns:
         The axes created or used
     """
     if ax is None:
         _, ax = plt.subplots()
 
-    yerr = norm.ppf(1 - level / 2) * df["data_value_stderr"]
+    yerr = norm.ppf(1 - level / 2) * df[f"{prefix}_stderr"]
 
-    ax.errorbar(x=df.index, y=df["data_value"], yerr=yerr, fmt="o", capsize=6)
+    ax.errorbar(x=df.index, y=df[prefix], yerr=yerr, fmt="o", capsize=6)
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.set_title(title)
     plt.xticks(rotation=60)
     return ax
```

### Comparing `pyDVL-0.8.1/src/pydvl/reporting/scores.py` & `pydvl-0.9/src/pydvl/reporting/scores.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/__init__.py` & `pydvl-0.9/src/pydvl/utils/caching/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Caching of functions.
+"""This module provides caching of functions.
 
 PyDVL can cache (memoize) the computation of the utility function
 and speed up some computations for data valuation.
 
 !!! Warning
     Function evaluations are cached with a key based on the function's signature
     and code. This can lead to undesired cache hits, see [Cache reuse](#cache-reuse).
 
     Remember **not to reuse utility objects for different datasets**.
 
 # Configuration
 
 Caching is disabled by default but can be enabled easily,
-see [Setting up the cache](#setting-up-the-cache).
+see [Setting up the cache][getting-started-cache].
 When enabled, it will be added to any callable used to construct a
 [Utility][pydvl.utils.utility.Utility] (done with the wrap method of
 [CacheBackend][pydvl.utils.caching.base.CacheBackend]).
 Depending on the nature of the utility you might want to
 enable the computation of a running average of function values, see
 [Usage with stochastic functions](#usaage-with-stochastic-functions).
 You can see all configuration options under
@@ -34,27 +34,29 @@
   a disk-based cache backend that uses pickled values written to and read from disk.
   This is used to share cached values between processes in a single machine.
 - [MemcachedCacheBackend][pydvl.utils.caching.memcached.MemcachedCacheBackend]:
   a [Memcached](https://memcached.org/)-based cache backend that uses pickled values written to
   and read from a Memcached server. This is used to share cached values
   between processes across multiple machines.
 
-  **Note** This specific backend requires optional dependencies.
-  See [[installation#extras]] for more information)
+    !!! Info
+        This specific backend requires optional dependencies not installed by
+        default. See [Extra dependencies][installation-extras] for more
+        information.
 
 # Usage with stochastic functions
 
 In addition to standard memoization, the wrapped functions
 can compute running average and standard error of repeated evaluations
 for the same input. This can be useful for stochastic functions with high variance
 (e.g. model training for small sample sizes), but drastically reduces
 the speed benefits of memoization.
 
 This behaviour can be activated with the option
-[allow_repeated_evaluations][pydvl.utils.caching.config.CachedFuncConfig]..
+[allow_repeated_evaluations][pydvl.utils.caching.config.CachedFuncConfig].
 
 # Cache reuse
 
 When working directly with [CachedFunc][pydvl.utils.caching.base.CachedFunc],  it is
 essential to only cache pure functions. If they have any kind of state, either
 internal or external (e.g. a closure over some data that may change), then the
 cache will fail to notice this and the same value will be returned.
@@ -80,9 +82,13 @@
 functions distinct to the eyes of the cache. This can be avoided with the use of
 [ignore_args][pydvl.utils.caching.config.CachedFuncConfig] option in the configuration.
 
 """
 from .base import *
 from .config import *
 from .disk import *
-from .memcached import *
 from .memory import *
+
+try:
+    from .memcached import *
+except ModuleNotFoundError:
+    pass
```

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/base.py` & `pydvl-0.9/src/pydvl/utils/caching/base.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/config.py` & `pydvl-0.9/src/pydvl/utils/caching/config.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/disk.py` & `pydvl-0.9/src/pydvl/utils/caching/disk.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 
     Args:
         cache_dir: Base directory for cache storage.
 
     Attributes:
         cache_dir: Base directory for cache storage.
 
-    ??? Examples
-        ``` pycon
+    Example:
+        Basic usage:
+        ```pycon
         >>> from pydvl.utils.caching.disk import DiskCacheBackend
         >>> cache_backend = DiskCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> cache_backend.set("key", value)
         >>> cache_backend.get("key")
         42
         ```
 
-        ``` pycon
+        Callable wrapping:
+        ```pycon
         >>> from pydvl.utils.caching.disk import DiskCacheBackend
         >>> cache_backend = DiskCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> def foo(x: int):
         ...     return x + 1
         ...
```

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/memcached.py` & `pydvl-0.9/src/pydvl/utils/caching/memcached.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,21 @@
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, Optional, Tuple
 
 try:
     from pymemcache import MemcacheUnexpectedCloseError
     from pymemcache.client import Client, RetryingClient
     from pymemcache.serde import PickleSerde
+except ModuleNotFoundError as e:
+    raise ModuleNotFoundError(
+        f"Cannot use MemcachedCacheBackend because pymemcache was not installed. "
+        f"Make sure to install pyDVL using `pip install pyDVL[memcached]`. \n"
+        f"Original error: {e}"
+    )
 
-    PYMEMCACHE_INSTALLED = True
-except ImportError:
-    PYMEMCACHE_INSTALLED = False
 
 from .base import CacheBackend
 
 __all__ = ["MemcachedClientConfig", "MemcachedCacheBackend"]
 
 PICKLE_VERSION = 5  # python >= 3.8
 
@@ -46,38 +49,40 @@
     no_delay: bool = True
     serde: PickleSerde = PickleSerde(pickle_version=PICKLE_VERSION)
 
 
 class MemcachedCacheBackend(CacheBackend):
     """Memcached cache backend for the distributed caching of functions.
 
-    Implements the CacheBackend interface for a memcached based cache.
-    This allows sharing evaluations across processes and nodes in a cluster.
-    You can run memcached as a service, locally or remotely,
-    see [Setting up the cache](#setting-up-the-cache)
+    Implements the [CacheBackend][pydvl.utils.caching.base.CacheBackend]
+    interface for a memcached based cache. This allows sharing evaluations
+    across processes and nodes in a cluster. You can run memcached as a service,
+    locally or remotely, see [the caching documentation][getting-started-cache].
 
     Args:
         config: Memcached client configuration.
 
     Attributes:
         config: Memcached client configuration.
         client: Memcached client instance.
 
-    ??? Examples
-        ``` pycon
+    Example:
+        Basic usage:
+        ```pycon
         >>> from pydvl.utils.caching.memcached import MemcachedCacheBackend
         >>> cache_backend = MemcachedCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> cache_backend.set("key", value)
         >>> cache_backend.get("key")
         42
         ```
 
-        ``` pycon
+        Callable wrapping:
+        ```pycon
         >>> from pydvl.utils.caching.memcached import MemcachedCacheBackend
         >>> cache_backend = MemcachedCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> def foo(x: int):
         ...     return x + 1
         ...
@@ -99,19 +104,15 @@
 
     def __init__(self, config: MemcachedClientConfig = MemcachedClientConfig()) -> None:
         """Initialize memcached cache backend.
 
         Args:
             config: Memcached client configuration.
         """
-        if not PYMEMCACHE_INSTALLED:
-            raise ModuleNotFoundError(
-                "Cannot use MemcachedCacheBackend because pymemcache was not installed. "
-                "Make sure to install pyDVL using `pip install pyDVL[memcached]`"
-            )
+
         super().__init__()
         self.config = config
         self.client = self._connect(self.config)
 
     def get(self, key: str) -> Optional[Any]:
         """Get value from memcached.
```

### Comparing `pyDVL-0.8.1/src/pydvl/utils/caching/memory.py` & `pydvl-0.9/src/pydvl/utils/caching/memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     This allows sharing evaluations across threads in a single process.
 
     The implementation is not thread-safe.
 
     Attributes:
         cached_values: Dictionary used to store cached values.
 
-    ??? Examples
-        ``` pycon
+    Example:
+        Basic usage:
+        ```pycon
         >>> from pydvl.utils.caching.memory import InMemoryCacheBackend
         >>> cache_backend = InMemoryCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> cache_backend.set("key", value)
         >>> cache_backend.get("key")
         42
         ```
 
-        ``` pycon
+        Callable wrapping:
+        ```pycon
         >>> from pydvl.utils.caching.memory import InMemoryCacheBackend
         >>> cache_backend = InMemoryCacheBackend()
         >>> cache_backend.clear()
         >>> value = 42
         >>> def foo(x: int):
         ...     return x + 1
         ...
```

### Comparing `pyDVL-0.8.1/src/pydvl/utils/dataset.py` & `pydvl-0.9/src/pydvl/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/functional.py` & `pydvl-0.9/src/pydvl/utils/functional.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/numeric.py` & `pydvl-0.9/src/pydvl/utils/numeric.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/progress.py` & `pydvl-0.9/src/pydvl/utils/progress.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/score.py` & `pydvl-0.9/src/pydvl/utils/score.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/status.py` & `pydvl-0.9/src/pydvl/utils/status.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/utils/types.py` & `pydvl-0.9/src/pydvl/utils/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 __all__ = [
     "ensure_seed_sequence",
     "LossFunction",
     "IndexT",
     "NameT",
     "MapFunction",
-    "NoPublicConstructor",
     "ReduceFunction",
     "Seed",
     "SupervisedModel",
 ]
 
 IndexT = TypeVar("IndexT", bound=np.int_)
 NameT = TypeVar("NameT", np.object_, np.int_)
@@ -80,40 +79,14 @@
 
         Returns:
             The score of the model on `(x, y)`
         """
         pass
 
 
-class NoPublicConstructor(ABCMeta):
-    """Metaclass that ensures a private constructor
-
-    If a class uses this metaclass like this:
-
-        class SomeClass(metaclass=NoPublicConstructor):
-            pass
-
-    If you try to instantiate your class (`SomeClass()`),
-    a `TypeError` will be thrown.
-
-    Taken almost verbatim from:
-    [https://stackoverflow.com/a/64682734](https://stackoverflow.com/a/64682734)
-    """
-
-    def __call__(cls, *args, **kwargs):
-        raise TypeError(
-            f"{cls.__module__}.{cls.__qualname__} cannot be initialized directly. "
-            "Use the proper factory instead."
-        )
-
-    def create(cls, *args: Any, **kwargs: Any):
-        """Create an instance of the class"""
-        return super().__call__(*args, **kwargs)
-
-
 def ensure_seed_sequence(
     seed: Optional[Union[Seed, SeedSequence]] = None
 ) -> SeedSequence:
     """
     If the passed seed is a SeedSequence object then it is returned as is. If it is
     a Generator the internal protected seed sequence from the generator gets extracted.
     Otherwise, a new SeedSequence object is created from the passed (optional) seed.
```

### Comparing `pyDVL-0.8.1/src/pydvl/utils/utility.py` & `pydvl-0.9/src/pydvl/utils/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 computation of values. Please see the documentation on
 [Computing Data Values][computing-data-values] for more information.
 
 [Utility][pydvl.utils.utility.Utility] holds information about model,
 data and scoring function (the latter being what one usually understands
 under *utility* in the general definition of Shapley value).
 It is automatically cached across machines when the
-[cache is configured][setting-up-the-cache] and it is enabled upon construction.
+[cache is configured][getting-started-cache] and it is enabled upon construction.
 
 [DataUtilityLearning][pydvl.utils.utility.DataUtilityLearning] adds support
 for learning the scoring function to avoid repeated re-training
 of the model to compute the score.
 
 This module also contains derived `Utility` classes for toy games that are used
 for testing and for demonstration purposes.
@@ -61,16 +61,16 @@
     [cloned](https://scikit-learn.org/stable/modules/generated/sklearn.base.clone.html)
     if it is a Sci-Kit Learn model, otherwise a copy is created using
     [copy.deepcopy][]
 
     Since evaluating the scoring function requires retraining the model and that
     can be time-consuming, this class wraps it and caches the results of each
     execution. Caching is available both locally and across nodes, but must
-    always be enabled for your project first, see [Setting up the
-    cache][setting-up-the-cache].
+    always be enabled for your project first, see [the documentation][getting-started-cache]
+    and the [module documentation][pydvl.utils.caching].
 
     Attributes:
         model: The supervised model.
         data: An object containing the split data.
         scorer: A scoring function. If None, the `score()` method of the model
             will be used. See [score][pydvl.utils.score] for ways to create
             and compose scorers, in particular how to set default values and
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/games.py` & `pydvl-0.9/src/pydvl/value/games.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 This module provides several predefined games and, depending on the game,
 the corresponding Shapley values, Least Core values or both of them, for
 benchmarking purposes.
 
 ## References
 
-[^1]: <a name="castro_polynomial_2009"></a>Castro, J., Gómez, D. and Tejada, J., 2009.
-    [Polynomial calculation of the Shapley value based on sampling](http://www.sciencedirect.com/science/article/pii/S0305054808000804).
-    Computers & Operations Research, 36(5), pp.1726-1730.
+[^1]: <a name="castro_polynomial_2009"></a>Castro, J., Gómez, D. and Tejada,
+      J., 2009. [Polynomial calculation of the Shapley value based on
+      sampling](http://www.sciencedirect.com/science/article/pii/S0305054808000804).
+      Computers & Operations Research, 36(5), pp.1726-1730.
 
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from functools import lru_cache
 from typing import Iterable, Optional, Tuple
@@ -324,18 +325,18 @@
             variances=np.zeros_like(self.data.x_train),
             counts=np.zeros_like(self.data.x_train),
         )
         return result
 
 
 class ShoesGame(Game):
-    """Toy game that is used for testing and demonstration purposes.
+    r"""Toy game that is used for testing and demonstration purposes.
 
-    An shoes game defined in
-    (Castro et al., 2009)<sup><a href="#castro_polynomial_2009">1</a></sup>.
+    A shoes game defined in (Castro et al.,
+    2009)<sup><a href="#castro_polynomial_2009">1</a></sup>.
 
     In this game, some players have a left shoe and others a right shoe.
     Single shoes have a worth of zero while pairs have a worth of 1.
 
     The payoff of a coalition $S$ is:
 
     $${
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/least_core/__init__.py` & `pydvl-0.9/src/pydvl/value/least_core/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 !!! tip "New in version 0.4.0"
 
 This package holds all routines for the computation of Least Core data values.
 
-Please refer to [Data valuation][computing-data-values] for an overview.
+Please refer to [Data valuation][data-valuation] for an overview.
 
 In addition to the standard interface via
 [compute_least_core_values()][pydvl.value.least_core.compute_least_core_values], because computing the
 Least Core values requires the solution of a linear and a quadratic problem
 *after* computing all the utility values, there is the possibility of performing
 each step separately. This is useful when running multiple experiments: use
 [lc_prepare_problem()][pydvl.value.least_core.naive.lc_prepare_problem] or
@@ -49,15 +49,15 @@
     solver_options: Optional[dict] = None,
     progress: bool = False,
     **kwargs,
 ) -> ValuationResult:
     """Umbrella method to compute Least Core values with any of the available
     algorithms.
 
-    See [Data valuation][computing-data-values] for an overview.
+    See [Data valuation][data-valuation] for an overview.
 
     The following algorithms are available. Note that the exact method can only
     work with very small datasets and is thus intended only for testing.
 
     - `exact`: uses the complete powerset of the training set for the constraints
       [combinatorial_exact_shapley()][pydvl.value.shapley.naive.combinatorial_exact_shapley].
     - `montecarlo`:  uses the approximate Monte Carlo Least Core algorithm.
@@ -83,15 +83,15 @@
     """
 
     if mode == LeastCoreMode.MonteCarlo:
         # TODO fix progress showing in remote case
         progress = False
         if n_iterations is None:
             raise ValueError("n_iterations cannot be None for Monte Carlo Least Core")
-        return montecarlo_least_core(
+        return montecarlo_least_core(  # type: ignore
             u=u,
             n_iterations=n_iterations,
             n_jobs=n_jobs,
             progress=progress,
             non_negative_subsidy=non_negative_subsidy,
             solver_options=solver_options,
             **kwargs,
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/least_core/common.py` & `pydvl-0.9/src/pydvl/value/least_core/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import itertools
 import logging
 import warnings
 from typing import List, NamedTuple, Optional, Sequence, Tuple
 
 import cvxpy as cp
 import numpy as np
+from deprecate import deprecated
 from numpy.typing import NDArray
 
-from pydvl.parallel import MapReduceJob, ParallelConfig
+from pydvl.parallel import (
+    MapReduceJob,
+    ParallelBackend,
+    ParallelConfig,
+    _maybe_init_parallel_backend,
+)
 from pydvl.utils import Status, Utility
 from pydvl.value import ValuationResult
 
 __all__ = [
     "_solve_least_core_linear_program",
     "_solve_egalitarian_least_core_quadratic_program",
     "lc_solve_problem",
@@ -140,61 +146,75 @@
         values=values,
         subsidy=subsidy,
         stderr=None,
         data_names=u.data.data_names,
     )
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def lc_solve_problems(
     problems: Sequence[LeastCoreProblem],
     u: Utility,
     algorithm: str,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     n_jobs: int = 1,
     non_negative_subsidy: bool = True,
     solver_options: Optional[dict] = None,
     **options,
 ) -> List[ValuationResult]:
     """Solves a list of linear problems in parallel.
 
     Args:
         u: Utility.
         problems: Least Core problems to solve, as returned by
             [mclc_prepare_problem()][pydvl.value.least_core.montecarlo.mclc_prepare_problem].
         algorithm: Name of the valuation algorithm.
-        config: Object configuring parallel computation, with cluster address,
-            number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         n_jobs: Number of parallel jobs to run.
         non_negative_subsidy: If True, the least core subsidy $e$ is constrained
             to be non-negative.
         solver_options: Additional options to pass to the solver.
 
     Returns:
         List of solutions.
     """
 
     def _map_func(
         problems: List[LeastCoreProblem], *args, **kwargs
     ) -> List[ValuationResult]:
         return [lc_solve_problem(p, *args, **kwargs) for p in problems]
 
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
     map_reduce_job: MapReduceJob[
         "LeastCoreProblem", "List[ValuationResult]"
     ] = MapReduceJob(
         inputs=problems,
         map_func=_map_func,
         map_kwargs=dict(
             u=u,
             algorithm=algorithm,
             non_negative_subsidy=non_negative_subsidy,
             solver_options=solver_options,
             **options,
         ),
         reduce_func=lambda x: list(itertools.chain(*x)),
-        config=config,
+        parallel_backend=parallel_backend,
         n_jobs=n_jobs,
     )
     solutions = map_reduce_job()
 
     return solutions
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/least_core/montecarlo.py` & `pydvl-0.9/src/pydvl/value/least_core/montecarlo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 import logging
 import warnings
 from typing import Iterable, Optional
 
 import numpy as np
+from deprecate import deprecated
 from numpy.typing import NDArray
 from tqdm.auto import tqdm
 
-from pydvl.parallel import MapReduceJob, ParallelConfig, effective_n_jobs
+from pydvl.parallel import (
+    MapReduceJob,
+    ParallelBackend,
+    ParallelConfig,
+    _maybe_init_parallel_backend,
+)
 from pydvl.utils.numeric import random_powerset
 from pydvl.utils.types import Seed
 from pydvl.utils.utility import Utility
 from pydvl.value.least_core.common import LeastCoreProblem, lc_solve_problem
 from pydvl.value.result import ValuationResult
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = ["montecarlo_least_core", "mclc_prepare_problem"]
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def montecarlo_least_core(
     u: Utility,
     n_iterations: int,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     non_negative_subsidy: bool = False,
     solver_options: Optional[dict] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
 ) -> ValuationResult:
     r"""Computes approximate Least Core values using a Monte Carlo approach.
 
@@ -47,57 +60,85 @@
     * $m$ is the number of subsets that will be sampled and whose utility will
       be computed and used to compute the data values.
 
     Args:
         u: Utility object with model, data, and scoring function
         n_iterations: total number of iterations to use
         n_jobs: number of jobs across which to distribute the computation
-        config: Object configuring parallel computation, with cluster
-            address, number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         non_negative_subsidy: If True, the least core subsidy $e$ is constrained
             to be non-negative.
         solver_options: Dictionary of options that will be used to select a solver
             and to configure it. Refer to [cvxpy's
             documentation](https://www.cvxpy.org/tutorial/advanced/index.html#setting-solver-options)
             for all possible options.
         progress: If True, shows a tqdm progress bar
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         Object with the data values and the least core value.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
     problem = mclc_prepare_problem(
-        u, n_iterations, n_jobs=n_jobs, config=config, progress=progress, seed=seed
+        u,
+        n_iterations,
+        n_jobs=n_jobs,
+        parallel_backend=parallel_backend,
+        config=config,
+        progress=progress,
+        seed=seed,
     )
     return lc_solve_problem(
         problem,
         u=u,
         algorithm="montecarlo_least_core",
         non_negative_subsidy=non_negative_subsidy,
         solver_options=solver_options,
     )
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def mclc_prepare_problem(
     u: Utility,
     n_iterations: int,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
 ) -> LeastCoreProblem:
     """Prepares a linear problem by sampling subsets of the data. Use this to
     separate the problem preparation from the solving with
     [lc_solve_problem()][pydvl.value.least_core.common.lc_solve_problem]. Useful
     for parallel execution of multiple experiments.
 
     See
     [montecarlo_least_core][pydvl.value.least_core.montecarlo.montecarlo_least_core]
     for argument descriptions.
+
+    !!! note "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
     n = len(u.data)
 
     if n_iterations < n:
         warnings.warn(
             f"Number of iterations '{n_iterations}' is smaller the size of the dataset '{n}'. "
             f"This is not optimal because in the worst case we need at least '{n}' constraints "
@@ -108,23 +149,27 @@
         warnings.warn(
             f"Passed n_iterations is greater than the number subsets! "
             f"Setting it to 2^{n}",
             RuntimeWarning,
         )
         n_iterations = 2**n
 
-    iterations_per_job = max(1, n_iterations // effective_n_jobs(n_jobs, config))
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
+    iterations_per_job = max(
+        1, n_iterations // parallel_backend.effective_n_jobs(n_jobs)
+    )
 
     map_reduce_job: MapReduceJob["Utility", "LeastCoreProblem"] = MapReduceJob(
         inputs=u,
         map_func=_montecarlo_least_core,
         reduce_func=_reduce_func,
         map_kwargs=dict(n_iterations=iterations_per_job, progress=progress),
         n_jobs=n_jobs,
-        config=config,
+        parallel_backend=parallel_backend,
     )
 
     return map_reduce_job(seed=seed)
 
 
 def _montecarlo_least_core(
     u: Utility,
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/least_core/naive.py` & `pydvl-0.9/src/pydvl/value/least_core/naive.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/loo/loo.py` & `pydvl-0.9/src/pydvl/value/loo/loo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 from __future__ import annotations
 
 from concurrent.futures import FIRST_COMPLETED, Future, wait
+from typing import Optional
 
+from deprecate import deprecated
 from tqdm import tqdm
 
-from pydvl.parallel import ParallelConfig, effective_n_jobs, init_executor
+from pydvl.parallel import ParallelBackend, ParallelConfig, _maybe_init_parallel_backend
 from pydvl.utils import Utility
 from pydvl.value.result import ValuationResult
 
 __all__ = ["compute_loo"]
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def compute_loo(
     u: Utility,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = True,
 ) -> ValuationResult:
     r"""Computes leave one out value:
 
     $$v(i) = u(D) - u(D \setminus \{i\}) $$
 
     Args:
         u: Utility object with model, data, and scoring function
         progress: If True, display a progress bar
         n_jobs: Number of parallel jobs to use
-        config: Object configuring parallel computation, with cluster
-            address, number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: If True, display a progress bar
 
     Returns:
         Object with the data values.
 
     !!! tip "New in version 0.7.0"
         Renamed from `naive_loo` and added parallel computation.
-    """
 
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
+    """
     if len(u.data) < 3:
         raise ValueError("Dataset must have at least 2 elements")
 
     result = ValuationResult.zeros(
         algorithm="loo",
         indices=u.data.indices,
         data_names=u.data.data_names,
@@ -48,22 +66,23 @@
 
     all_indices = set(u.data.indices)
     total_utility = u(u.data.indices)
 
     def fun(idx: int) -> tuple[int, float]:
         return idx, total_utility - u(all_indices.difference({idx}))
 
-    max_workers = effective_n_jobs(n_jobs, config)
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+    max_workers = parallel_backend.effective_n_jobs(n_jobs)
     n_submitted_jobs = 2 * max_workers  # number of jobs in the queue
 
     # NOTE: this could be done with a simple executor.map(), but we want to
     # display a progress bar
 
-    with init_executor(
-        max_workers=max_workers, config=config, cancel_futures=True
+    with parallel_backend.executor(
+        max_workers=max_workers, cancel_futures=True
     ) as executor:
         pending: set[Future] = set()
         index_it = iter(u.data.indices)
 
         pbar = tqdm(disable=not progress, total=100, unit="%")
         while True:
             pbar.n = 100 * sum(result.counts) / len(u.data)
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/oob/oob.py` & `pydvl-0.9/src/pydvl/value/oob/oob.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/result.py` & `pydvl-0.9/src/pydvl/value/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 [ValuationResult.empty()][pydvl.value.result.ValuationResult.empty] creates an
 empty result object, which can be used as a starting point for adding results
 together. Empty results are discarded when added to other results. Finally,
 [ValuationResult.from_random()][pydvl.value.result.ValuationResult.from_random]
 samples random values uniformly.
 
 """
+
 from __future__ import annotations
 
 import collections.abc
 import logging
 from dataclasses import dataclass
 from functools import total_ordering
 from numbers import Integral
@@ -59,26 +60,22 @@
     Sequence,
     Union,
     cast,
     overload,
 )
 
 import numpy as np
+import pandas as pd
 from numpy.typing import NDArray
 
 from pydvl.utils.dataset import Dataset
 from pydvl.utils.numeric import running_moments
 from pydvl.utils.status import Status
 from pydvl.utils.types import IndexT, NameT, Seed
 
-try:
-    import pandas  # Try to import here for the benefit of mypy
-except ImportError:
-    pass
-
 __all__ = ["ValuationResult", "ValueItem"]
 
 logger = logging.getLogger(__name__)
 
 
 @total_ordering
 @dataclass
@@ -659,41 +656,40 @@
             self._values[pos],
             self._variances[pos],
             self._counts[pos],
         )
 
     def to_dataframe(
         self, column: Optional[str] = None, use_names: bool = False
-    ) -> pandas.DataFrame:
+    ) -> pd.DataFrame:
         """Returns values as a dataframe.
 
         Args:
             column: Name for the column holding the data value. Defaults to
                 the name of the algorithm used.
             use_names: Whether to use data names instead of indices for the
                 DataFrame's index.
 
         Returns:
             A dataframe with two columns, one for the values, with name
                 given as explained in `column`, and another with standard errors for
                 approximate algorithms. The latter will be named `column+'_stderr'`.
-        Raises:
-             ImportError: If pandas is not installed
         """
-        if not pandas:
-            raise ImportError("Pandas required for DataFrame export")
         column = column or self._algorithm
-        df = pandas.DataFrame(
+        df = pd.DataFrame(
             self._values[self._sort_positions],
-            index=self._names[self._sort_positions]
-            if use_names
-            else self._indices[self._sort_positions],
+            index=(
+                self._names[self._sort_positions]
+                if use_names
+                else self._indices[self._sort_positions]
+            ),
             columns=[column],
         )
         df[column + "_stderr"] = self.stderr[self._sort_positions]
+        df[column + "_updates"] = self.counts[self._sort_positions]
         return df
 
     @classmethod
     def from_random(
         cls,
         size: int,
         total: Optional[float] = None,
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/sampler.py` & `pydvl-0.9/src/pydvl/value/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 ## References
 
 [^1]: <a name="mitchell_sampling_2022"></a>Mitchell, Rory, Joshua Cooper, Eibe
       Frank, and Geoffrey Holmes. [Sampling Permutations for Shapley Value
       Estimation](http://jmlr.org/papers/v23/21-0439.html). Journal of Machine
       Learning Research 23, no. 43 (2022): 1–46.
+[^2]: <a name="wang_data_2023"></a>Wang, J.T. and Jia, R., 2023.
+    [Data Banzhaf: A Robust Data Valuation Framework for Machine Learning](https://proceedings.mlr.press/v206/wang23e.html).
+    In: Proceedings of The 26th International Conference on Artificial Intelligence and Statistics, pp. 6388-6421.
 
 """
 
 from __future__ import annotations
 
 import abc
 import math
@@ -68,29 +71,32 @@
 from numpy.typing import NDArray
 
 from pydvl.utils.numeric import powerset, random_subset, random_subset_of_size
 from pydvl.utils.types import IndexT, Seed
 
 __all__ = [
     "AntitheticSampler",
-    "DeterministicUniformSampler",
     "DeterministicPermutationSampler",
+    "DeterministicUniformSampler",
+    "MSRSampler",
     "PermutationSampler",
     "PowersetSampler",
     "RandomHierarchicalSampler",
-    "UniformSampler",
+    "SampleT",
+    "StochasticSampler",
     "StochasticSamplerMixin",
+    "UniformSampler",
 ]
 
 SampleT = Tuple[IndexT, NDArray[IndexT]]
 Sequence.register(np.ndarray)
 
 
 class PowersetSampler(abc.ABC, Iterable[SampleT], Generic[IndexT]):
-    """Samplers are custom iterables over subsets of indices.
+    r"""Samplers are custom iterables over subsets of indices.
 
     Calling ``iter()`` on a sampler returns an iterator over tuples of the form
     $(i, S)$, where $i$ is an index of interest, and $S \subset I \setminus \{i\}$
     is a subset of the complement of $i$.
 
     This is done in two nested loops, where the outer loop iterates over the set
     of indices, and the inner loop iterates over subsets of the complement of
@@ -308,14 +314,34 @@
     def weight(cls, n: int, subset_len: int) -> float:
         """Correction coming from Monte Carlo integration so that the mean of
         the marginals converges to the value: the uniform distribution over the
         powerset of a set with n-1 elements has mass 2^{n-1} over each subset."""
         return float(2 ** (n - 1)) if n > 0 else 1.0
 
 
+class MSRSampler(StochasticSamplerMixin, PowersetSampler[IndexT]):
+    """An iterator to perform sampling of random subsets.
+
+    This sampler does not return any index, it only returns subsets of the data.
+    This sampler is used in (Wang et. al.)<sup><a href="wang_data_2023">2</a></sup>.
+    """
+
+    def __iter__(self) -> Iterator[SampleT]:
+        if len(self) == 0:
+            return
+        while True:
+            subset = random_subset(self.indices, seed=self._rng)
+            yield None, subset
+            self._n_samples += 1
+
+    @classmethod
+    def weight(cls, n: int, subset_len: int) -> float:
+        return 1.0
+
+
 class AntitheticSampler(StochasticSamplerMixin, PowersetSampler[IndexT]):
     """An iterator to perform uniform random sampling of subsets, and their
     complements.
 
     Works as [UniformSampler][pydvl.value.sampler.UniformSampler], but for every
     tuple $(i,S)$, it subsequently returns $(i,S^c)$, where $S^c$ is the
     complement of the set $S$ in the set of indices, excluding $i$.
@@ -446,8 +472,9 @@
 # TODO Replace by Intersection[StochasticSamplerMixin, PowersetSampler[T]]
 # See https://github.com/python/typing/issues/213
 StochasticSampler = Union[
     UniformSampler[IndexT],
     PermutationSampler[IndexT],
     AntitheticSampler[IndexT],
     RandomHierarchicalSampler[IndexT],
+    MSRSampler[IndexT],
 ]
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/__init__.py` & `pydvl-0.9/src/pydvl/value/shapley/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/classwise.py` & `pydvl-0.9/src/pydvl/value/shapley/classwise.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 $$
 
 where $S_{y_i} \subseteq D_{y_i} \setminus \{i\}$ and $S_{-y_i} \subseteq
 D_{-y_i}$.
 
 !!! tip "Analysis of Class-wise Shapley"
     For a detailed analysis of the method, with comparison to other valuation
-    techniques, please refer to the [main
-    documentation](../../../../../value/classwise-shapley).
+    techniques, please refer to the [main documentation][class-wise-shapley].
 
 In practice, the quantity above is estimated using Monte Carlo sampling of
 the powerset and the set of index permutations. This results in the estimator
 
 $$
 v_u(i) = \frac{1}{K} \sum_k \frac{1}{L} \sum_l
 [u(\sigma^{(l)}_{:i} \cup \{i\} | S^{(k)} ) − u( \sigma^{(l)}_{:i} | S^{(k)})],
@@ -61,24 +60,20 @@
 import logging
 import numbers
 from concurrent.futures import FIRST_COMPLETED, Future, wait
 from copy import copy
 from typing import Callable, Optional, Set, Tuple, Union, cast
 
 import numpy as np
+from deprecate import deprecated
 from numpy.random import SeedSequence
 from numpy.typing import NDArray
 from tqdm import tqdm
 
-from pydvl.parallel import (
-    ParallelConfig,
-    effective_n_jobs,
-    init_executor,
-    init_parallel_backend,
-)
+from pydvl.parallel import ParallelBackend, ParallelConfig, _maybe_init_parallel_backend
 from pydvl.utils import (
     Dataset,
     Scorer,
     ScorerCallable,
     Seed,
     SupervisedModel,
     Utility,
@@ -235,25 +230,32 @@
             n_out_of_class = len(y_test) - n_in_class
             in_class_score *= n_in_class / (n_in_class + n_out_of_class)
             out_of_class_score *= n_out_of_class / (n_in_class + n_out_of_class)
 
         return in_class_score, out_of_class_score
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def compute_classwise_shapley_values(
     u: Utility,
     *,
     done: StoppingCriterion,
     truncation: TruncationPolicy,
     done_sample_complements: Optional[StoppingCriterion] = None,
     normalize_values: bool = True,
     use_default_scorer_value: bool = True,
     min_elements_per_label: int = 1,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
 ) -> ValuationResult:
     r"""
     Computes an approximate Class-wise Shapley value by sampling independent
     permutations of the index set for each label and index sets sampled from the
     powerset of the complement (with respect to the currently evaluated label),
@@ -261,16 +263,17 @@
 
     $$
     v_u(i) = \frac{1}{K} \sum_k \frac{1}{L} \sum_l
     [u(\sigma^{(l)}_{:i} \cup \{i\} | S^{(k)} ) − u( \sigma^{(l)}_{:i} | S^{(k)})],
     $$
 
     where $\sigma_{:i}$ denotes the set of indices in permutation sigma before
-    the position where $i$ appears and $S$ is a subset of the index set of all other
-    labels(see [[data-valuation]] for details).
+    the position where $i$ appears and $S$ is a subset of the index set of all
+    other labels (see [the main documentation][class-wise-shapley] for
+    details).
 
     Args:
         u: Utility object containing model, data, and scoring function. The
             scorer must be of type
             [ClasswiseScorer][pydvl.value.shapley.classwise.ClasswiseScorer].
         done: Function that checks whether the computation needs to stop.
         truncation: Callable function that decides whether to interrupt processing a
@@ -284,15 +287,21 @@
             for each permutation.
         use_default_scorer_value: The first set of indices is the sampled complement
             set. Unless not otherwise specified, the default scorer value is used for
             this. If it is set to false, the base score is calculated from the utility.
         min_elements_per_label: The minimum number of elements for each opposite
             label.
         n_jobs: Number of parallel jobs to run.
-        config: Parallel configuration.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display a progress bar.
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         ValuationResult object containing computed data values.
 
     !!! tip "New in version 0.7.1"
@@ -310,28 +319,30 @@
 
     if not isinstance(u.scorer, ClasswiseScorer):
         raise ValueError(
             "Please set a subclass of ClasswiseScorer object as scorer object of the"
             " utility. See scoring argument of Utility."
         )
 
-    parallel_backend = init_parallel_backend(config)
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
     u_ref = parallel_backend.put(u)
-    n_jobs = effective_n_jobs(n_jobs, config)
+    n_jobs = parallel_backend.effective_n_jobs(n_jobs)
     n_submitted_jobs = 2 * n_jobs
 
     pbar = tqdm(disable=not progress, position=0, total=100, unit="%")
     algorithm = "classwise_shapley"
     accumulated_result = ValuationResult.zeros(
         algorithm=algorithm, indices=u.data.indices, data_names=u.data.data_names
     )
     terminate_exec = False
     seed_sequence = ensure_seed_sequence(seed)
 
-    with init_executor(max_workers=n_jobs, config=config) as executor:
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
+    with parallel_backend.executor(max_workers=n_jobs) as executor:
         pending: Set[Future] = set()
         while True:
             completed_futures, pending = wait(
                 pending, timeout=60, return_when=FIRST_COMPLETED
             )
             for future in completed_futures:
                 accumulated_result += future.result()
@@ -375,15 +386,14 @@
     min_elements_per_label: int = 1,
     algorithm_name: str = "classwise_shapley",
     seed: Optional[SeedSequence] = None,
 ) -> ValuationResult:
     """Helper function for [compute_classwise_shapley_values()]
     [pydvl.value.shapley.classwise.compute_classwise_shapley_values].
 
-
     Args:
         u: Utility object containing model, data, and scoring function. The
             scorer must be of type [ClasswiseScorer]
             [pydvl.value.shapley.classwise.ClasswiseScorer].
         done_sample_complements: Function checking whether computation needs to stop.
             Otherwise, it will resample conditional sets until the stopping criterion is
             met.
@@ -395,14 +405,18 @@
         min_elements_per_label: The minimum number of elements for each opposite
             label.
         algorithm_name: For the results object.
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         ValuationResult object containing computed data values.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend configuration.
     """
     if done_sample_complements is None:
         done_sample_complements = MaxChecks(1)
 
     result = ValuationResult.zeros(
         algorithm=algorithm_name, indices=u.data.indices, data_names=u.data.data_names
     )
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/common.py` & `pydvl-0.9/src/pydvl/value/shapley/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 from pydvl.value.shapley.naive import (
     combinatorial_exact_shapley,
     permutation_exact_shapley,
 )
 from pydvl.value.shapley.owen import OwenAlgorithm, owen_sampling_shapley
 from pydvl.value.shapley.truncated import NoTruncation
 from pydvl.value.shapley.types import ShapleyMode
-from pydvl.value.stopping import MaxUpdates, StoppingCriterion
+from pydvl.value.stopping import MaxChecks, StoppingCriterion
 
 __all__ = ["compute_shapley_values"]
 
 
 def compute_shapley_values(
     u: Utility,
     *,
-    done: StoppingCriterion = MaxUpdates(100),
+    done: StoppingCriterion = MaxChecks(None),
     mode: ShapleyMode = ShapleyMode.TruncatedMontecarlo,
     n_jobs: int = 1,
     seed: Optional[Seed] = None,
     **kwargs,
 ) -> ValuationResult:
     """Umbrella method to compute Shapley values with any of the available
     algorithms.
 
-    See [[data-valuation]] for an overview.
+    See [Data valuation][data-valuation] for an overview.
 
     The following algorithms are available. Note that the exact methods can only
     work with very small datasets and are thus intended only for testing. Some
     algorithms also accept additional arguments, please refer to the
     documentation of each particular method.
 
     - `combinatorial_exact`: uses the combinatorial implementation of data
@@ -115,33 +115,33 @@
             truncation=truncation,
             n_jobs=n_jobs,
             seed=seed,
             progress=progress,
             **kwargs,
         )
     elif mode == ShapleyMode.CombinatorialMontecarlo:
-        return combinatorial_montecarlo_shapley(
+        return combinatorial_montecarlo_shapley(  # type: ignore
             u, done=done, n_jobs=n_jobs, seed=seed, progress=progress
         )
     elif mode == ShapleyMode.CombinatorialExact:
-        return combinatorial_exact_shapley(u, n_jobs=n_jobs, progress=progress)
+        return combinatorial_exact_shapley(u, n_jobs=n_jobs, progress=progress)  # type: ignore
     elif mode == ShapleyMode.PermutationExact:
         return permutation_exact_shapley(u, progress=progress)
     elif mode == ShapleyMode.Owen or mode == ShapleyMode.OwenAntithetic:
         if kwargs.get("n_samples") is None:
             raise ValueError("n_samples cannot be None for Owen methods")
         if kwargs.get("max_q") is None:
             raise ValueError("Owen Sampling requires max_q for the outer integral")
 
         method = (
             OwenAlgorithm.Standard
             if mode == ShapleyMode.Owen
             else OwenAlgorithm.Antithetic
         )
-        return owen_sampling_shapley(
+        return owen_sampling_shapley(  # type: ignore
             u,
             n_samples=int(kwargs.get("n_samples", -1)),
             max_q=int(kwargs.get("max_q", -1)),
             method=method,
             n_jobs=n_jobs,
             seed=seed,
         )
@@ -151,15 +151,15 @@
         n_samples = kwargs.pop("n_samples")
         if n_samples is None:
             raise ValueError("n_samples cannot be None for Group Testing")
         epsilon = kwargs.pop("epsilon")
         if epsilon is None:
             raise ValueError("Group Testing requires error bound epsilon")
         delta = kwargs.pop("delta", 0.05)
-        return group_testing_shapley(
+        return group_testing_shapley(  # type: ignore
             u,
             epsilon=float(epsilon),
             delta=delta,
             n_samples=int(n_samples),
             n_jobs=n_jobs,
             progress=progress,
             seed=seed,
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/gt.py` & `pydvl-0.9/src/pydvl/value/shapley/gt.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 !!! Warning
     This method is very inefficient. Potential improvements to the
     implementation notwithstanding, convergence seems to be very slow (in terms
     of evaluations of the utility required). We recommend other Monte Carlo
     methods instead.
 
-You can read more [in the documentation][computing-data-values].
+You can read more [in the documentation][data-valuation].
 
 !!! tip "New in version 0.4.0"
 
 ## References
 
 [^1]: <a name="jia_efficient_2019"></a>Jia, R. et al., 2019.
     [Towards Efficient Data Valuation Based on the Shapley
@@ -24,19 +24,25 @@
 """
 import logging
 from collections import namedtuple
 from typing import Iterable, Optional, Tuple, TypeVar, Union, cast
 
 import cvxpy as cp
 import numpy as np
+from deprecate import deprecated
 from numpy.random import SeedSequence
 from numpy.typing import NDArray
 from tqdm.auto import trange
 
-from pydvl.parallel import MapReduceJob, ParallelConfig, effective_n_jobs
+from pydvl.parallel import (
+    MapReduceJob,
+    ParallelBackend,
+    ParallelConfig,
+    _maybe_init_parallel_backend,
+)
 from pydvl.utils import Utility
 from pydvl.utils.numeric import random_subset_of_size
 from pydvl.utils.status import Status
 from pydvl.utils.types import Seed, ensure_seed_sequence
 from pydvl.value import ValuationResult
 
 __all__ = ["group_testing_shapley", "num_samples_eps_delta"]
@@ -160,25 +166,32 @@
         k = rng.choice(const.kk, size=1, p=const.q).item()
         s = random_subset_of_size(u.data.indices, k, seed=rng)
         uu[t] = u(s)
         betas[t, s] = 1
     return uu, betas
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def group_testing_shapley(
     u: Utility,
     n_samples: int,
     epsilon: float,
     delta: float,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
-    **options,
+    **options: dict,
 ) -> ValuationResult:
     """Implements group testing for approximation of Shapley values as described
     in (Jia, R. et al., 2019)<sup><a href="#jia_efficient_2019">1</a></sup>.
 
     !!! Warning
         This method is very inefficient. It requires several orders of magnitude
         more evaluations of the utility than others in
@@ -197,16 +210,21 @@
             to estimate this.
         epsilon: From the (ε,δ) sample bound. Use the same as for the
             estimation of `n_iterations`.
         delta: From the (ε,δ) sample bound. Use the same as for the
             estimation of `n_iterations`.
         n_jobs: Number of parallel jobs to use. Each worker performs a chunk
             of all tests (i.e. utility evaluations).
-        config: Object configuring parallel computation, with cluster
-            address, number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display progress bars for each job.
         seed: Either an instance of a numpy random number generator or a seed for it.
         options: Additional options to pass to
             [cvxpy.Problem.solve()](https://www.cvxpy.org/tutorial/advanced/index.html#solve-method-options).
             E.g. to change the solver (which defaults to `cvxpy.SCS`) pass
             `solver=cvxpy.CVXOPT`.
 
@@ -214,14 +232,19 @@
         Object with the data values.
 
     !!! tip "New in version 0.4.0"
 
     !!! tip "Changed in version 0.5.0"
         Changed the solver to cvxpy instead of scipy's linprog. Added the ability
         to pass arbitrary options to it.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
 
     n = len(u.data.indices)
 
     const = _constants(
         n=n,
         epsilon=epsilon,
@@ -231,15 +254,17 @@
     T = n_samples
     if T < const.T:
         log.warning(
             f"n_samples of {T} are below the required {const.T} for the "
             f"ε={epsilon:.02f} guarantee at δ={1 - delta:.02f} probability"
         )
 
-    samples_per_job = max(1, n_samples // effective_n_jobs(n_jobs, config))
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
+    samples_per_job = max(1, n_samples // parallel_backend.effective_n_jobs(n_jobs))
 
     def reducer(
         results_it: Iterable[Tuple[NDArray, NDArray]]
     ) -> Tuple[NDArray, NDArray]:
         return np.concatenate(list(x[0] for x in results_it)).astype(
             np.float_
         ), np.concatenate(list(x[1] for x in results_it)).astype(np.int_)
@@ -248,15 +273,15 @@
     map_reduce_seed_sequence, cvxpy_seed = tuple(seed_sequence.spawn(2))
 
     map_reduce_job: MapReduceJob[Utility, Tuple[NDArray, NDArray]] = MapReduceJob(
         u,
         map_func=_group_testing_shapley,
         reduce_func=reducer,
         map_kwargs=dict(n_samples=samples_per_job, progress=progress),
-        config=config,
+        parallel_backend=parallel_backend,
         n_jobs=n_jobs,
     )
     uu, betas = map_reduce_job(seed=map_reduce_seed_sequence)
 
     # Matrix of estimated differences. See Eqs. (3) and (4) in the paper.
     C = np.zeros(shape=(n, n))
     for i in range(n):
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/knn.py` & `pydvl-0.9/src/pydvl/value/shapley/knn.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/montecarlo.py` & `pydvl-0.9/src/pydvl/value/shapley/montecarlo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
 Monte Carlo approximations to Shapley Data values.
 
 !!! Warning
     You probably want to use the common interface provided by
-    [compute_shapley_values()][pydvl.value.shapley.compute_shapley_values] instead of directly using
-    the functions in this module.
+    [compute_shapley_values()][pydvl.value.shapley.compute_shapley_values]
+    instead of directly using the functions in this module.
 
 Because exact computation of Shapley values requires $\mathcal{O}(2^n)$
 re-trainings of the model, several Monte Carlo approximations are available. The
 first two sample from the powerset of the training data directly:
 [combinatorial_montecarlo_shapley()][pydvl.value.shapley.montecarlo.combinatorial_montecarlo_shapley]
 and [owen_sampling_shapley()][pydvl.value.shapley.owen.owen_sampling_shapley].
 The latter uses a reformulation in terms of a continuous extension of the
@@ -46,25 +46,25 @@
 import math
 import operator
 from concurrent.futures import FIRST_COMPLETED, Future, wait
 from functools import reduce
 from typing import Optional, Sequence, Union
 
 import numpy as np
+from deprecate import deprecated
 from numpy.random import SeedSequence
 from numpy.typing import NDArray
 from tqdm.auto import tqdm
 
 from pydvl.parallel import (
     CancellationPolicy,
     MapReduceJob,
+    ParallelBackend,
     ParallelConfig,
-    effective_n_jobs,
-    init_executor,
-    init_parallel_backend,
+    _maybe_init_parallel_backend,
 )
 from pydvl.utils.numeric import random_powerset
 from pydvl.utils.progress import repeat_indices
 from pydvl.utils.types import Seed, ensure_seed_sequence
 from pydvl.utils.utility import Utility
 from pydvl.value.result import ValuationResult
 from pydvl.value.shapley.truncated import NoTruncation, TruncationPolicy
@@ -77,25 +77,28 @@
 
 def _permutation_montecarlo_one_step(
     u: Utility,
     truncation: TruncationPolicy,
     algorithm_name: str,
     seed: Optional[Union[Seed, SeedSequence]] = None,
 ) -> ValuationResult:
-    """Helper function for [permutation_montecarlo_shapley()][pydvl.value.shapley.montecarlo.permutation_montecarlo_shapley].
+    """Helper function for
+    [permutation_montecarlo_shapley()][pydvl.value.shapley.montecarlo.permutation_montecarlo_shapley].
 
     Computes marginal utilities of each training sample in a randomly sampled
     permutation.
+
     Args:
         u: Utility object with model, data, and scoring function
         truncation: A callable which decides whether to interrupt
             processing a permutation and set all subsequent marginals to zero.
         algorithm_name: For the results object. Used internally by different
             variants of Shapley using this subroutine
-        seed: Either an instance of a numpy random number generator or a seed for it.
+        seed: Either an instance of a numpy random number generator or a seed
+            for it.
 
     Returns:
         An object with the results
     """
 
     result = ValuationResult.zeros(
         algorithm=algorithm_name, indices=u.data.indices, data_names=u.data.data_names
@@ -120,41 +123,48 @@
             f"{nans} NaN values in current permutation, ignoring. "
             "Consider setting a default value for the Scorer"
         )
         result = ValuationResult.empty(algorithm=algorithm_name)
     return result
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def permutation_montecarlo_shapley(
     u: Utility,
     done: StoppingCriterion,
     *,
     truncation: TruncationPolicy = NoTruncation(),
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
 ) -> ValuationResult:
     r"""Computes an approximate Shapley value by sampling independent
     permutations of the index set, approximating the sum:
 
     $$
     v_u(x_i) = \frac{1}{n!} \sum_{\sigma \in \Pi(n)}
     \tilde{w}( | \sigma_{:i} | )[u(\sigma_{:i} \cup \{i\}) − u(\sigma_{:i})],
     $$
 
     where $\sigma_{:i}$ denotes the set of indices in permutation sigma before
     the position where $i$ appears (see [[data-valuation]] for details).
 
-    This implements the method described in (Ghorbani and Zou, 2019)<sup><a href="#ghorbani_data_2019">1</a></sup>
-    with a double stopping criterion.
+    This implements the method described in (Ghorbani and Zou, 2019)<sup><a
+    href="#ghorbani_data_2019">1</a></sup> with a double stopping criterion.
 
-    .. todo::
-       Think of how to add Robin-Gelman or some other more principled stopping
-       criterion.
+    !!! Todo
+        Think of how to add Robin-Gelman or some other more principled stopping
+        criterion.
 
     Instead of naively implementing the expectation, we sequentially add points
     to coalitions from a permutation and incrementally compute marginal utilities.
     We stop computing marginals for a given permutation based on a
     [TruncationPolicy][pydvl.value.shapley.truncated.TruncationPolicy].
     (Ghorbani and Zou, 2019)<sup><a href="#ghorbani_data_2019">1</a></sup>
     mention two policies: one that stops after a certain
@@ -172,47 +182,55 @@
     Args:
         u: Utility object with model, data, and scoring function.
         done: function checking whether computation must stop.
         truncation: An optional callable which decides whether to interrupt
             processing a permutation and set all subsequent marginals to
             zero. Typically used to stop computation when the marginal is small.
         n_jobs: number of jobs across which to distribute the computation.
-        config: Object configuring parallel computation, with cluster address,
-            number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display a progress bar.
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         Object with the data values.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
     algorithm = "permutation_montecarlo_shapley"
 
-    parallel_backend = init_parallel_backend(config)
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
     u = parallel_backend.put(u)
-    max_workers = effective_n_jobs(n_jobs, config)
+    max_workers = parallel_backend.effective_n_jobs(n_jobs)
     n_submitted_jobs = 2 * max_workers  # number of jobs in the executor's queue
 
     seed_sequence = ensure_seed_sequence(seed)
     result = ValuationResult.zeros(
         algorithm=algorithm, indices=u.data.indices, data_names=u.data.data_names
     )
 
     pbar = tqdm(disable=not progress, total=100, unit="%")
 
-    with init_executor(
-        max_workers=max_workers, config=config, cancel_futures=CancellationPolicy.ALL
+    with parallel_backend.executor(
+        max_workers=max_workers, cancel_futures=CancellationPolicy.ALL
     ) as executor:
         pending: set[Future] = set()
         while True:
             pbar.n = 100 * done.completion()
             pbar.refresh()
 
-            completed, pending = wait(
-                pending, timeout=config.wait_timeout, return_when=FIRST_COMPLETED
-            )
+            completed, pending = wait(pending, timeout=1.0, return_when=FIRST_COMPLETED)
             for future in completed:
                 result += future.result()
                 # we could check outside the loop, but that means more
                 # submissions if the stopping criterion is unstable
                 if done(result):
                     return result
 
@@ -281,32 +299,39 @@
         s = next(random_powerset(subset, n_samples=1, seed=rng))
         marginal = (u({idx}.union(s)) - u(s)) / math.comb(n - 1, len(s))
         result.update(idx, correction * marginal)
 
     return result
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def combinatorial_montecarlo_shapley(
     u: Utility,
     done: StoppingCriterion,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None,
 ) -> ValuationResult:
     r"""Computes an approximate Shapley value using the combinatorial
     definition:
 
     $$v_u(i) = \frac{1}{n} \sum_{S \subseteq N \setminus \{i\}}
     \binom{n-1}{ | S | }^{-1} [u(S \cup \{i\}) − u(S)]$$
 
     This consists of randomly sampling subsets of the power set of the training
     indices in [u.data][pydvl.utils.utility.Utility], and computing their
-    marginal utilities. See [Data valuation][computing-data-values] for details.
+    marginal utilities. See [Data valuation][data-valuation] for details.
 
     Note that because sampling is done with replacement, the approximation is
     poor even for $2^{m}$ subsets with $m>n$, even though there are $2^{n-1}$
     subsets for each $i$. Prefer
     [permutation_montecarlo_shapley()][pydvl.value.shapley.montecarlo.permutation_montecarlo_shapley].
 
     Parallelization is done by splitting the set of indices across processes and
@@ -314,25 +339,36 @@
 
     Args:
         u: Utility object with model, data, and scoring function
         done: Stopping criterion for the computation.
         n_jobs: number of parallel jobs across which to distribute the
             computation. Each worker receives a chunk of
             [indices][pydvl.utils.dataset.Dataset.indices]
-        config: Object configuring parallel computation, with cluster address,
-            number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display progress bars for each job.
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         Object with the data values.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
 
     map_reduce_job: MapReduceJob[NDArray, ValuationResult] = MapReduceJob(
         u.data.indices,
         map_func=_combinatorial_montecarlo_shapley,
         reduce_func=lambda results: reduce(operator.add, results),
         map_kwargs=dict(u=u, done=done, progress=progress),
         n_jobs=n_jobs,
-        config=config,
+        parallel_backend=parallel_backend,
     )
     return map_reduce_job(seed=seed)
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/naive.py` & `pydvl-0.9/src/pydvl/value/shapley/naive.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,50 @@
+r"""
+This module implements exact Shapley values using either the combinatorial or
+permutation definition.
+
+The exact computation of $n$ values takes $\mathcal{O}(2^n)$ evaluations of the
+utility and is therefore only possible for small datasets. For larger datasets,
+consider using any of the approximations, such as [Monte
+Carlo][pydvl.value.shapley.montecarlo], or proxy models like
+[kNN][pydvl.value.shapley.knn].
+
+See [Data valuation][data-valuation] for details.
+"""
+
 import math
 import warnings
 from itertools import permutations
-from typing import List
+from typing import List, Optional
 
 import numpy as np
+from deprecate import deprecated
 from numpy.typing import NDArray
 from tqdm.auto import tqdm
 
-from pydvl.parallel import MapReduceJob, ParallelConfig
+from pydvl.parallel import (
+    MapReduceJob,
+    ParallelBackend,
+    ParallelConfig,
+    _maybe_init_parallel_backend,
+)
 from pydvl.utils import Utility, powerset
 from pydvl.utils.status import Status
 from pydvl.value.result import ValuationResult
 
 __all__ = ["permutation_exact_shapley", "combinatorial_exact_shapley"]
 
 
 def permutation_exact_shapley(u: Utility, *, progress: bool = True) -> ValuationResult:
     r"""Computes the exact Shapley value using the formulation with permutations:
 
-    $$v_u(x_i) = \frac{1}{n!} \sum_{\sigma \in \Pi(n)} [u(\sigma_{i-1} \cup {i}) − u(\sigma_{i})].$$
+    $$v_u(x_i) = \frac{1}{n!} \sum_{\sigma \in \Pi(n)} [u(\sigma_{i-1}
+    \cup {i}) − u(\sigma_{i})].$$
 
-    See [Data valuation][computing-data-values] for details.
+    See [Data valuation][data-valuation] for details.
 
     When the length of the training set is > 10 this prints a warning since the
     computation becomes too expensive. Used mostly for internal testing and
     simple use cases. Please refer to the [Monte Carlo
     approximations][pydvl.value.shapley.montecarlo] for practical applications.
 
     Args:
@@ -85,60 +105,80 @@
             total=2 ** (n - 1),
             position=0,
         ):
             local_values[i] += (u({i}.union(s)) - u(s)) / math.comb(n - 1, len(s))  # type: ignore
     return local_values / n
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def combinatorial_exact_shapley(
     u: Utility,
     *,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
 ) -> ValuationResult:
     r"""Computes the exact Shapley value using the combinatorial definition.
 
-    $$v_u(i) = \frac{1}{n} \sum_{S \subseteq N \setminus \{i\}} \binom{n-1}{ | S | }^{-1} [u(S \cup \{i\}) − u(S)].$$
+    $$v_u(i) = \frac{1}{n} \sum_{S \subseteq N \setminus \{i\}}
+    \binom{n-1}{ | S | }^{-1} [u(S \cup \{i\}) − u(S)].$$
 
-    See [Data valuation][computing-data-values] for details.
+    See [Data valuation][data-valuation] for details.
 
     !!! Note
         If the length of the training set is > n_jobs*20 this prints a warning
-        because the computation is very expensive. Used mostly for internal testing
-        and simple use cases. Please refer to the
-        [Monte Carlo][pydvl.value.shapley.montecarlo] approximations for practical
-        applications.
+        because the computation is very expensive. Used mostly for internal
+        testing and simple use cases. Please refer to the
+        [Monte Carlo][pydvl.value.shapley.montecarlo] approximations for
+        practical applications.
 
     Args:
         u: Utility object with model, data, and scoring function
         n_jobs: Number of parallel jobs to use
-        config: Object configuring parallel computation, with cluster address,
-            number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display progress bars for each job.
 
     Returns:
         Object with the data values.
+
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
     """
     # Arbitrary choice, will depend on time required, caching, etc.
     if len(u.data) // n_jobs > 20:
         warnings.warn(
             f"Large dataset! Computation requires 2^{len(u.data)} calls to model.fit()"
         )
 
     def reduce_fun(results: List[NDArray]) -> NDArray:
         return np.array(results).sum(axis=0)  # type: ignore
 
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
     map_reduce_job: MapReduceJob[NDArray, NDArray] = MapReduceJob(
         u.data.indices,
         map_func=_combinatorial_exact_shapley,
         map_kwargs=dict(u=u, progress=progress),
         reduce_func=reduce_fun,
         n_jobs=n_jobs,
-        config=config,
+        parallel_backend=parallel_backend,
     )
     values = map_reduce_job()
     return ValuationResult(
         algorithm="combinatorial_exact_shapley",
         status=Status.Converged,
         values=values,
         data_names=u.data.data_names,
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/owen.py` & `pydvl-0.9/src/pydvl/value/shapley/owen.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,40 @@
 
 import operator
 from enum import Enum
 from functools import reduce
 from typing import Optional, Sequence
 
 import numpy as np
+from deprecate import deprecated
 from numpy.typing import NDArray
 
-from pydvl.parallel import MapReduceJob, ParallelConfig
+from pydvl.parallel import (
+    MapReduceJob,
+    ParallelBackend,
+    ParallelConfig,
+    _maybe_init_parallel_backend,
+)
 from pydvl.utils import Utility, random_powerset
 from pydvl.utils.progress import repeat_indices
 from pydvl.utils.types import Seed
 from pydvl.value import ValuationResult
 from pydvl.value.stopping import MinUpdates
 
 __all__ = ["OwenAlgorithm", "owen_sampling_shapley"]
 
 
 class OwenAlgorithm(Enum):
+    """Choices for the Owen sampling method.
+
+    Attributes:
+        Standard: Use q ∈ [0, 1]
+        Antithetic: Use q ∈ [0, 0.5] and correlated samples
+    """
+
     Standard = "standard"
     Antithetic = "antithetic"
 
 
 def _owen_sampling_shapley(
     indices: Sequence[int],
     u: Utility,
@@ -95,22 +108,29 @@
         # TODO: investigate whether this or other quadrature rules are better
         #  than a simple average
         # result.update(idx, (e[:-1] + e[1:]).sum() / (2 * max_q))
 
     return result
 
 
+@deprecated(
+    target=True,
+    args_mapping={"config": "config"},
+    deprecated_in="0.9.0",
+    remove_in="0.10.0",
+)
 def owen_sampling_shapley(
     u: Utility,
     n_samples: int,
     max_q: int,
     *,
     method: OwenAlgorithm = OwenAlgorithm.Standard,
     n_jobs: int = 1,
-    config: ParallelConfig = ParallelConfig(),
+    parallel_backend: Optional[ParallelBackend] = None,
+    config: Optional[ParallelConfig] = None,
     progress: bool = False,
     seed: Optional[Seed] = None
 ) -> ValuationResult:
     r"""Owen sampling of Shapley values as described in
     (Okhrati and Lipani, 2021)<sup><a href="#okhrati_multilinear_2021">1</a></sup>.
 
     This function computes a Monte Carlo approximation to
@@ -150,37 +170,49 @@
         method: Selects the algorithm to use, see the description. Either
             [OwenAlgorithm.Full][pydvl.value.shapley.owen.OwenAlgorithm] for
             $q \in [0,1]$ or
             [OwenAlgorithm.Halved][pydvl.value.shapley.owen.OwenAlgorithm] for
             $q \in [0,0.5]$ and correlated samples
         n_jobs: Number of parallel jobs to use. Each worker receives a chunk
             of the total of `max_q` values for q.
-        config: Object configuring parallel computation, with cluster address,
-            number of cpus, etc.
+        parallel_backend: Parallel backend instance to use
+            for parallelizing computations. If `None`,
+            use [JoblibParallelBackend][pydvl.parallel.backends.JoblibParallelBackend] backend.
+            See the [Parallel Backends][pydvl.parallel.backends] package
+            for available options.
+        config: (**DEPRECATED**) Object configuring parallel computation,
+            with cluster address, number of cpus, etc.
         progress: Whether to display progress bars for each job.
         seed: Either an instance of a numpy random number generator or a seed for it.
 
     Returns:
         Object with the data values.
 
     !!! tip "New in version 0.3.0"
 
     !!! tip "Changed in version 0.5.0"
         Support for parallel computation and enable antithetic sampling.
 
+    !!! tip "Changed in version 0.9.0"
+        Deprecated `config` argument and added a `parallel_backend`
+        argument to allow users to pass the Parallel Backend instance
+        directly.
+
     """
+    parallel_backend = _maybe_init_parallel_backend(parallel_backend, config)
+
     map_reduce_job: MapReduceJob[NDArray, ValuationResult] = MapReduceJob(
         u.data.indices,
         map_func=_owen_sampling_shapley,
         reduce_func=lambda results: reduce(operator.add, results),
         map_kwargs=dict(
             u=u,
             method=OwenAlgorithm(method),
             n_samples=n_samples,
             max_q=max_q,
             progress=progress,
         ),
         n_jobs=n_jobs,
-        config=config,
+        parallel_backend=parallel_backend,
     )
 
     return map_reduce_job(seed=seed)
```

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/truncated.py` & `pydvl-0.9/src/pydvl/value/shapley/truncated.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/shapley/types.py` & `pydvl-0.9/src/pydvl/value/shapley/types.py`

 * *Files identical despite different names*

### Comparing `pyDVL-0.8.1/src/pydvl/value/stopping.py` & `pydvl-0.9/src/pydvl/value/stopping.py`

 * *Files 14% similar despite different names*

```diff
@@ -111,38 +111,43 @@
 
 
 ## References
 
 [^1]: <a name="ghorbani_data_2019"></a>Ghorbani, A., Zou, J., 2019.
     [Data Shapley: Equitable Valuation of Data for Machine Learning](https://proceedings.mlr.press/v97/ghorbani19c.html).
     In: Proceedings of the 36th International Conference on Machine Learning, PMLR, pp. 2242–2251.
+[^2]: <a name="wang_data_2023"></a>Wang, J.T. and Jia, R., 2023.
+    [Data Banzhaf: A Robust Data Valuation Framework for Machine Learning](https://proceedings.mlr.press/v206/wang23e.html).
+    In: Proceedings of The 26th International Conference on Artificial Intelligence and Statistics, pp. 6388-6421.
 """
 
 from __future__ import annotations
 
 import abc
 import logging
 from time import time
 from typing import Callable, Optional, Protocol, Type
 
 import numpy as np
 from numpy.typing import NDArray
+from scipy.stats import spearmanr
 
 from pydvl.utils import Status
 from pydvl.value import ValuationResult
 
 __all__ = [
     "make_criterion",
     "AbsoluteStandardError",
     "StoppingCriterion",
     "MaxChecks",
     "MaxUpdates",
     "MinUpdates",
     "MaxTime",
     "HistoryDeviation",
+    "RankCorrelation",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 class StoppingCriterionCallable(Protocol):
     """Signature for a stopping criterion"""
@@ -165,41 +170,38 @@
 
     Instances of `StoppingCriterion` can be composed with the binary operators
     `&` (*and*), and `|` (*or*), following the truth tables of
     [Status][pydvl.utils.status.Status]. The unary operator `~` (*not*) is
     also supported. These boolean operations act according to the following
     rules:
 
-    - The results of [_check][pydvl.value.stopping.StoppingCriterion._check] are
-      combined with the operator. See [Status][pydvl.utils.status.Status] for
-      the truth tables.
+    - The results of `check()` are combined with the operator. See
+      [Status][pydvl.utils.status.Status] for the truth tables.
     - The results of
       [converged][pydvl.value.stopping.StoppingCriterion.converged] are combined
       with the operator (returning another boolean array).
     - The [completion][pydvl.value.stopping.StoppingCriterion.completion]
       method returns the min, max, or the complement to 1 of the completions of
       the operands, for AND, OR and NOT respectively. This is required for cases
       where one of the criteria does not keep track of the convergence of single
       values, e.g. [MaxUpdates][pydvl.value.stopping.MaxUpdates], because
       [completion][pydvl.value.stopping.StoppingCriterion.completion] by
       default returns the mean of the boolean convergence array.
 
     # Subclassing
 
-    Subclassing this class requires implementing a
-    [_check][pydvl.value.stopping.StoppingCriterion._check] method that
+    Subclassing this class requires implementing a `check()` method that
     returns a [Status][pydvl.utils.status.Status] object based on a given
     [ValuationResult][pydvl.value.result.ValuationResult]. This method should
-    update the attribute [_converged][pydvl.value.stopping.StoppingCriterion._converged],
-    which is a boolean array indicating whether the value for each index has
-    converged. When this does not make sense for a particular stopping criterion,
+    update the attribute `_converged`, which is a boolean array indicating
+    whether the value for each index has converged.
+    When this does not make sense for a particular stopping criterion,
     [completion][pydvl.value.stopping.StoppingCriterion.completion] should be
     overridden to provide an overall completion value, since its default
-    implementation attempts to compute the mean of
-    [_converged][pydvl.value.stopping.StoppingCriterion._converged].
+    implementation attempts to compute the mean of `_converged`.
 
     Args:
         modify_result: If `True` the status of the input
             [ValuationResult][pydvl.value.result.ValuationResult] is modified in
             place after the call.
     """
 
@@ -229,27 +231,27 @@
 
     @property
     def converged(self) -> NDArray[np.bool_]:
         """Returns a boolean array indicating whether the values have converged
         for each data point.
 
         Inheriting classes must set the `_converged` attribute in their
-        [_check][pydvl.value.stopping.StoppingCriterion._check].
+        `check()`.
 
         Returns:
             A boolean array indicating whether the values have converged for
             each data point.
         """
         return self._converged
 
     def __str__(self):
         return type(self).__name__
 
     def __call__(self, result: ValuationResult) -> Status:
-        """Calls [_check][pydvl.value.stopping.StoppingCriterion._check], maybe updating the result."""
+        """Calls `check()`, maybe updating the result."""
         if len(result) == 0:
             logger.warning(
                 "At least one iteration finished but no results where generated. "
                 "Please check that your scorer and utility return valid numbers."
             )
         status = self._check(result)
         if self.modify_result:  # FIXME: this is not nice
@@ -622,7 +624,90 @@
         return Status.Pending
 
     def reset(self):
         self._memory = None  # type: ignore
 
     def __str__(self):
         return f"HistoryDeviation(n_steps={self.n_steps}, rtol={self.rtol})"
+
+
+class RankCorrelation(StoppingCriterion):
+    r"""A check for stability of Spearman correlation between checks.
+
+    When the change in rank correlation between two successive iterations is
+    below a given threshold, the computation is terminated.
+    The criterion computes the Spearman correlation between two successive iterations.
+    The Spearman correlation uses the ordering indices of the given values and
+    correlates them. This means it focuses on the order of the elements instead of their
+    exact values. If the order stops changing (meaning the Banzhaf semivalues estimates
+    converge), the criterion stops the algorithm.
+
+    This criterion is used in (Wang et. al.)<sup><a href="wang_data_2023">2</a></sup>.
+
+    Args:
+        rtol: Relative tolerance for convergence ($\epsilon$ in the formula)
+        modify_result: If `True`, the status of the input
+            [ValuationResult][pydvl.value.result.ValuationResult] is modified in
+            place after the call.
+        burn_in: The minimum number of iterations before checking for
+            convergence. This is required because the first correlation is
+            meaningless.
+
+    !!! tip "Added in 0.9.0"
+    """
+
+    def __init__(
+        self,
+        rtol: float,
+        burn_in: int,
+        modify_result: bool = True,
+    ):
+        super().__init__(modify_result=modify_result)
+        if rtol <= 0 or rtol >= 1:
+            raise ValueError("rtol must be in (0, 1)")
+        self.rtol = rtol
+        self.burn_in = burn_in
+        self._memory: NDArray[np.float_] | None = None
+        self._corr = 0.0
+        self._completion = 0.0
+        self._iterations = 0
+
+    def _check(self, r: ValuationResult) -> Status:
+        self._iterations += 1
+        if self._memory is None:
+            self._memory = r.values.copy()
+            self._converged = np.full(len(r), False)
+            return Status.Pending
+
+        corr = spearmanr(self._memory, r.values)[0]
+        self._memory = r.values.copy()
+        self._update_completion(corr)
+        if (
+            np.isclose(corr, self._corr, rtol=self.rtol)
+            and self._iterations > self.burn_in
+        ):
+            self._converged = np.full(len(r), True)
+            logger.debug(
+                f"RankCorrelation has converged with {corr=} in iteration {self._iterations}"
+            )
+            return Status.Converged
+        self._corr = np.nan_to_num(corr, nan=0.0)
+        return Status.Pending
+
+    def _update_completion(self, corr: float) -> None:
+        if np.isnan(corr):
+            self._completion = 0.0
+        elif not np.isclose(corr, self._corr, rtol=self.rtol):
+            self._completion = corr
+            # self.rtol / np.abs(corr - self._corr) might be another option
+        else:
+            self._completion = 1.0
+
+    def completion(self) -> float:
+        return self._completion
+
+    def reset(self):
+        self._memory = None  # type: ignore
+        self._corr = 0.0
+
+    def __str__(self):
+        return f"RankCorrelation(rtol={self.rtol})"
```

