# Comparing `tmp/Connectome-Utilities-0.4.6.tar.gz` & `tmp/Connectome-Utilities-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Connectome-Utilities-0.4.6.tar", last modified: Tue Oct 31 18:08:10 2023, max compression
+gzip compressed data, was "Connectome-Utilities-0.4.8.tar", last modified: Fri Apr 12 08:16:57 2024, max compression
```

## Comparing `Connectome-Utilities-0.4.6.tar` & `Connectome-Utilities-0.4.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.928591 Connectome-Utilities-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/AUTHORS.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.916591 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2023-10-31 18:08:10.000000 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-10-31 18:08:10.000000 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 18:08:10.000000 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-10-31 18:08:10.000000 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-31 18:08:10.000000 Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11353 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20272 2023-10-31 18:08:10.928591 Connectome-Utilities-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19296 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.916591 Connectome-Utilities-0.4.6/conntility/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.916591 Connectome-Utilities-0.4.6/conntility/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12378 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/analysis_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.916591 Connectome-Utilities-0.4.6/conntility/analysis/library/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/library/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3238 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/analysis/library/diffusion_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.920591 Connectome-Utilities-0.4.6/conntility/circuit_models/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29686 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/connection_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/input_spikes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.920591 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/extra_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/from_atlas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/grouping_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/make_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/sonata_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/tessellate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/circuit_models/sonata_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    91111 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/connectivity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.924591 Connectome-Utilities-0.4.6/conntility/flatmapping/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/flatmapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/flatmapping/_supersample_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/flatmapping/flatmap_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/flatmapping/supersampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/flatmapping/wm_recipe_utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.924591 Connectome-Utilities-0.4.6/conntility/io/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/io/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/io/sparse_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/io/synapse_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    10990 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.924591 Connectome-Utilities-0.4.6/conntility/randomization/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/randomization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.924591 Connectome-Utilities-0.4.6/conntility/subcellular/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/subcellular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16841 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/conntility/subcellular/neuron_morphology_path_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 18:08:10.928591 Connectome-Utilities-0.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 18:08:10.928591 Connectome-Utilities-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/tests/test_analysis_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7250 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/tests/test_connectivity_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-10-31 18:07:55.000000 Connectome-Utilities-0.4.6/tests/test_neuron_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.754089 Connectome-Utilities-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/AUTHORS.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.754089 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-12 08:16:57.000000 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-12 08:16:57.000000 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:16:57.000000 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-12 08:16:57.000000 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 08:16:57.000000 Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-04-12 08:16:57.754089 Connectome-Utilities-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.746089 Connectome-Utilities-0.4.8/conntility/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.746089 Connectome-Utilities-0.4.8/conntility/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12378 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/analysis_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.746089 Connectome-Utilities-0.4.8/conntility/analysis/library/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/library/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3238 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/analysis/library/diffusion_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/circuit_models/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29686 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/connection_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/input_spikes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/extra_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/from_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/grouping_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/make_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/sonata_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/tessellate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/circuit_models/sonata_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    93593 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/connectivity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/flatmapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/flatmapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/flatmapping/_supersample_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/flatmapping/flatmap_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/flatmapping/supersampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/flatmapping/wm_recipe_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/io/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/io/sparse_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/io/synapse_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10990 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/randomization/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/randomization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.750089 Connectome-Utilities-0.4.8/conntility/subcellular/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/subcellular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/conntility/subcellular/neuron_morphology_path_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:16:57.754089 Connectome-Utilities-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:16:57.754089 Connectome-Utilities-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/tests/test_analysis_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7250 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/tests/test_connectivity_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-12 08:16:52.000000 Connectome-Utilities-0.4.8/tests/test_neuron_groups.py
```

### Comparing `Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/PKG-INFO` & `Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Connectome-Utilities
-Version: 0.4.6
+Version: 0.4.8
 Summary: Complex network representation and analysis layer
 Author-email: "Blue Brain Project, EPFL" <conntility.645co@simplelogin.com>
 Project-URL: Homepage, https://github.com/BlueBrain/ConnectomeUtilities
 Project-URL: Bug Tracker, https://github.com/BlueBrain/ConnectomeUtilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Connectome-Utilities-0.4.6/Connectome_Utilities.egg-info/SOURCES.txt` & `Connectome-Utilities-0.4.8/Connectome_Utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/LICENSE` & `Connectome-Utilities-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/PKG-INFO` & `Connectome-Utilities-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Connectome-Utilities
-Version: 0.4.6
+Version: 0.4.8
 Summary: Complex network representation and analysis layer
 Author-email: "Blue Brain Project, EPFL" <conntility.645co@simplelogin.com>
 Project-URL: Homepage, https://github.com/BlueBrain/ConnectomeUtilities
 Project-URL: Bug Tracker, https://github.com/BlueBrain/ConnectomeUtilities/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Connectome-Utilities-0.4.6/README.md` & `Connectome-Utilities-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/analysis/__init__.py` & `Connectome-Utilities-0.4.8/conntility/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/analysis/analysis.py` & `Connectome-Utilities-0.4.8/conntility/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/analysis/analysis_decorators.py` & `Connectome-Utilities-0.4.8/conntility/analysis/analysis_decorators.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/analysis/clustering.py` & `Connectome-Utilities-0.4.8/conntility/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/analysis/library/diffusion_mapping.py` & `Connectome-Utilities-0.4.8/conntility/analysis/library/diffusion_mapping.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/__init__.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/connection_matrix.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/connection_matrix.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/input_spikes.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/input_spikes.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/extra_properties.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/extra_properties.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/from_atlas.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/from_atlas.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/grouping_config.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/grouping_config.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/loader.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/loader.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/make_groups.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/make_groups.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/sonata_extensions.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/sonata_extensions.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/neuron_groups/tessellate.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/neuron_groups/tessellate.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/circuit_models/sonata_helpers.py` & `Connectome-Utilities-0.4.8/conntility/circuit_models/sonata_helpers.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/connectivity.py` & `Connectome-Utilities-0.4.8/conntility/connectivity.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,15 +672,15 @@
         if mask is None:
             mask = np.ones(len(df), dtype=bool)
         elif hasattr(mask, "__call__"):
             mask = np.array(mask(df))
         else:
             mask = np.array(mask)
         passes_filter = np.ones(len(mask), dtype=bool)
-        passes_filter[mask.values] = filter_func(df.loc[mask], **kwargs)
+        passes_filter[mask] = filter_func(df.loc[mask], **kwargs)
         return self.subedges(passes_filter)
         
     def default(self, new_default_property, copy=True):
         """
         Set the default edge property to return. Used in obj.matrix, obj.dense_matrix, obj.array
 
         Args:
@@ -1375,14 +1375,73 @@
         self._edge_indices.to_hdf(fn, key=full_prefix + "/edge_indices")
 
         with h5py.File(fn, "a") as h5:
             data_grp = h5[full_prefix]
             data_grp.attrs["NEUROTOP_SHAPE"] = self._shape
             data_grp.attrs["NEUROTOP_DEFAULT_EDGE"] = self._default_edge
             data_grp.attrs["NEUROTOP_CLASS"] = "ConnectivityMatrix"
+    
+    def to_networkx(self, add_vertex_properties=True, add_edge_properties=True):
+        try:
+            import networkx
+        except ImportError:
+            print("This optional functionality requires installation of the networkx package!")
+            raise
+
+        if add_edge_properties:
+            G = networkx.DiGraph()
+            if add_vertex_properties:
+                for _r in self.vertices.iterrows():
+                    G.add_node(_r[0], **_r[1].to_dict())
+            else:
+                G.add_nodes_from(range(len(self)))
+            for _idx, _prop in zip(self._edge_indices.iterrows(), self.edges.iterrows()):
+                G.add_edge(_idx[1]["row"], _idx[1]["col"], **_prop[1].to_dict())
+        else:
+            G = networkx.DiGraph(self.matrix)
+            if add_vertex_properties:
+                for _r in self.vertices.iterrows():
+                    G.nodes[_r[0]].update(**_r[1].to_dict())
+        return G
+    
+    @classmethod
+    def from_networkx(cls, G):
+        try:
+            import networkx
+        except ImportError:
+            print("This optional functionality requires installation of the networkx package!")
+            raise
+
+        lst_vert_props = set([k for n in G.nodes for k in G.nodes[n].keys()])
+        lst_edge_props = set([k for n in G.edges for k in G.edges[n].keys()])
+
+        if len(lst_vert_props) == 0: verts = pd.DataFrame({}, index=range(len(G)))
+        else:
+            verts = [pd.Series(networkx.get_node_attributes(G, _prop), name=_prop)
+                    for _prop in lst_vert_props]
+            verts = pd.concat(verts, axis=1).reset_index(drop=True)
+            if "index" in lst_vert_props: verts = verts.set_index("index", drop=True)
+
+        if len(lst_edge_props) == 0:
+            edge_indices = pd.DataFrame(G.edges, columns=["row", "col"])
+            edges = pd.DataFrame(np.ones(len(edge_indices), dtype=bool), columns=["data"],
+                                 index=edge_indices.index)
+        else:
+            edges = [pd.Series(networkx.get_edge_attributes(G, _prop), name=_prop)
+                    for _prop in lst_edge_props]
+            edges = pd.concat(edges, axis=1)
+            edge_indices = edges.index.to_frame().reset_index(drop=True)
+            edge_indices.columns = ["row", "col"]
+            edges = edges.reset_index(drop=True)
+
+        return cls(edge_indices, edge_properties=edges,
+                   vertex_properties=verts, shape=(len(verts), len(verts)))
+
+
+
 
 
 def _update_load_config(load_cfg, sim_tgt):
     from .circuit_models.neuron_groups.grouping_config import _read_if_needed
     load_config = _read_if_needed(load_cfg)
     if load_config is None:
         load_config = {"loading": {"base_target": sim_tgt}}
```

### Comparing `Connectome-Utilities-0.4.6/conntility/flatmapping/_supersample_utility.py` & `Connectome-Utilities-0.4.8/conntility/flatmapping/_supersample_utility.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/flatmapping/flatmap_utility.py` & `Connectome-Utilities-0.4.8/conntility/flatmapping/flatmap_utility.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,28 +89,29 @@
     Locations that never hit the valid volume will return a flat location of (-1, -1).
     :param xyz: numpy.array, N x 3: coordinates in 3d space
     :param uvw: numpy.array, N x 3: directions in 3d space. Optional, can be None.
     :param fm: VoxelData: flatmap
     :param max_translation: float.
     :return: Flat locations of the xyz coordinates in the flatmap.
     """
-    solution = fm.lookup(xyz)
+    solution = fm.lookup(xyz, outer_value=-1)
     if uvw is not None and not numpy.all(solution > 0):
         # 1)
-        solution = fm.lookup(xyz + FIX_TRANSITION * uvw)
+        solution = fm.lookup(xyz + FIX_TRANSITION * uvw, outer_value=-1)
         if numpy.all(solution > 0):
             return solution
         else:
             # 2)
             fac = 0
             step = fm.voxel_dimensions[0] / 4
             tl_factors = numpy.zeros((len(uvw), 1))
-            solution = fm.lookup(xyz)
+            solution = fm.lookup(xyz, outer_value=-1)
             while numpy.any(solution < 0) and fac < max_translation:
                 try:
                     fac += step
                     to_update = numpy.any(solution < 0, axis=1)
                     tl_factors[to_update, 0] = fac
-                    solution[to_update, :] = fm.lookup(xyz[to_update, :] + tl_factors[to_update, :] * uvw[to_update, :])
+                    solution[to_update, :] = fm.lookup(xyz[to_update, :] + tl_factors[to_update, :] * uvw[to_update, :],
+                                                       outer_value=-1)
                 except VoxcellError:
                     break
     return solution
```

### Comparing `Connectome-Utilities-0.4.6/conntility/flatmapping/supersampling.py` & `Connectome-Utilities-0.4.8/conntility/flatmapping/supersampling.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/flatmapping/wm_recipe_utility.py` & `Connectome-Utilities-0.4.8/conntility/flatmapping/wm_recipe_utility.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/io/logging.py` & `Connectome-Utilities-0.4.8/conntility/io/logging.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/io/sparse_matrices.py` & `Connectome-Utilities-0.4.8/conntility/io/sparse_matrices.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/io/synapse_report.py` & `Connectome-Utilities-0.4.8/conntility/io/synapse_report.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/multi_scale.py` & `Connectome-Utilities-0.4.8/conntility/multi_scale.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/plugins.py` & `Connectome-Utilities-0.4.8/conntility/plugins.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/conntility/subcellular/neuron_morphology_path_distance.py` & `Connectome-Utilities-0.4.8/conntility/subcellular/neuron_morphology_path_distance.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/pyproject.toml` & `Connectome-Utilities-0.4.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Connectome-Utilities"
-version = "0.4.6"
+version = "0.4.8"
 authors = [
   { name="Blue Brain Project, EPFL", email="conntility.645co@simplelogin.com" },
 ]
 description = "Complex network representation and analysis layer"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `Connectome-Utilities-0.4.6/tests/test_analysis.py` & `Connectome-Utilities-0.4.8/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/tests/test_analysis_decorator.py` & `Connectome-Utilities-0.4.8/tests/test_analysis_decorator.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/tests/test_connectivity_matrix.py` & `Connectome-Utilities-0.4.8/tests/test_connectivity_matrix.py`

 * *Files identical despite different names*

### Comparing `Connectome-Utilities-0.4.6/tests/test_neuron_groups.py` & `Connectome-Utilities-0.4.8/tests/test_neuron_groups.py`

 * *Files identical despite different names*

