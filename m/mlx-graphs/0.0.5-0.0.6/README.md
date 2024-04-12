# Comparing `tmp/mlx-graphs-0.0.5.tar.gz` & `tmp/mlx-graphs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx-graphs-0.0.5.tar", last modified: Sun Mar 17 10:53:15 2024, max compression
+gzip compressed data, was "mlx-graphs-0.0.6.tar", last modified: Fri Apr 12 08:26:27 2024, max compression
```

## Comparing `mlx-graphs-0.0.5.tar` & `mlx-graphs-0.0.6.tar`

### file list

```diff
@@ -1,63 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.059263 mlx-graphs-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-03-17 10:53:15.059263 mlx-graphs-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.051263 mlx-graphs-0.0.5/mlx_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.051263 mlx-graphs-0.0.5/mlx_graphs/data/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/data/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/data/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.051263 mlx-graphs-0.0.5/mlx_graphs/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/elliptic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/karate_club.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/ogb_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/planetoid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/qm7b.py
--rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/superpixel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/tu_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.051263 mlx-graphs-0.0.5/mlx_graphs/datasets/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/datasets/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.051263 mlx-graphs-0.0.5/mlx_graphs/loaders/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/loaders/dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.055263 mlx-graphs-0.0.5/mlx_graphs/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.055263 mlx-graphs-0.0.5/mlx_graphs/nn/conv/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/gat_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/gcn_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/gin_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/rel_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/sage_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/conv/simple_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/graph_network_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/message_passing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.055263 mlx-graphs-0.0.5/mlx_graphs/nn/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/nn/pooling/global_pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.055263 mlx-graphs-0.0.5/mlx_graphs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/array_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/mlx_graphs/utils/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 10:53:15.055263 mlx-graphs-0.0.5/mlx_graphs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-03-17 10:53:15.000000 mlx-graphs-0.0.5/mlx_graphs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-03-17 10:53:15.000000 mlx-graphs-0.0.5/mlx_graphs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 10:53:15.000000 mlx-graphs-0.0.5/mlx_graphs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-17 10:53:15.000000 mlx-graphs-0.0.5/mlx_graphs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 10:53:15.000000 mlx-graphs-0.0.5/mlx_graphs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-17 10:53:10.000000 mlx-graphs-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 10:53:15.059263 mlx-graphs-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.816249 mlx-graphs-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-04-12 08:26:27.816249 mlx-graphs-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.804249 mlx-graphs-0.0.6/mlx_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.804249 mlx-graphs-0.0.6/mlx_graphs/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/data/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.804249 mlx-graphs-0.0.6/mlx_graphs/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/elliptic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/karate_club.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/ogb_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8754 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/planetoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/qm7b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8291 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/superpixel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/tu_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.804249 mlx-graphs-0.0.6/mlx_graphs/datasets/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/datasets/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.804249 mlx-graphs-0.0.6/mlx_graphs/loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/loaders/dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.808249 mlx-graphs-0.0.6/mlx_graphs/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.808249 mlx-graphs-0.0.6/mlx_graphs/nn/conv/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/gat_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/gcn_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/gin_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13433 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/rel_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/sage_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/conv/simple_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/graph_network_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/message_passing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.808249 mlx-graphs-0.0.6/mlx_graphs/nn/norm/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/norm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/norm/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/norm/instance_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/norm/layer_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.808249 mlx-graphs-0.0.6/mlx_graphs/nn/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/nn/pooling/global_pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.808249 mlx-graphs-0.0.6/mlx_graphs/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/transforms/base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/transforms/normalize_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.812249 mlx-graphs-0.0.6/mlx_graphs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14898 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/mlx_graphs/utils/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:26:27.812249 mlx-graphs-0.0.6/mlx_graphs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9481 2024-04-12 08:26:27.000000 mlx-graphs-0.0.6/mlx_graphs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-04-12 08:26:27.000000 mlx-graphs-0.0.6/mlx_graphs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:26:27.000000 mlx-graphs-0.0.6/mlx_graphs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 08:26:27.000000 mlx-graphs-0.0.6/mlx_graphs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 08:26:27.000000 mlx-graphs-0.0.6/mlx_graphs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-12 08:26:18.000000 mlx-graphs-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:26:27.816249 mlx-graphs-0.0.6/setup.cfg
```

### Comparing `mlx-graphs-0.0.5/LICENSE` & `mlx-graphs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/PKG-INFO` & `mlx-graphs-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-graphs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Graph Neural Network library made for Apple Silicon
 Author: mlx-graphs contributors
 License: MIT License
         
         Copyright © 2024 mlx-graphs contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,17 @@
 Requires-Dist: fsspec==2024.2.0
 Requires-Dist: tqdm==4.66.1
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.6.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest==7.4.4; extra == "test"
 Requires-Dist: scipy==1.12.0; extra == "test"
+Requires-Dist: networkx==3.2.1; extra == "test"
+Requires-Dist: torch==2.2.0; extra == "test"
+Requires-Dist: torch_geometric==2.5.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: ipython==8.21.0; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.25.2; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx-gallery==0.15.0; extra == "docs"
```

### Comparing `mlx-graphs-0.0.5/README.md` & `mlx-graphs-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/data/batch.py` & `mlx-graphs-0.0.6/mlx_graphs/data/batch.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/data/collate.py` & `mlx-graphs-0.0.6/mlx_graphs/data/collate.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/data/data.py` & `mlx-graphs-0.0.6/mlx_graphs/data/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Literal, Optional, Union
 
 import mlx.core as mx
 import numpy as np
 
+from mlx_graphs.utils import has_isolated_nodes, has_self_loops
+from mlx_graphs.utils.topology import is_undirected
+
 
 class GraphData:
     """
     Represents a graph data object with optional features and labels.
 
     Args:
         edge_index: edge index representing the topology of
@@ -24,15 +27,15 @@
         graph_labels: Array of shape [1, num_graph_labels]
             containing the global labels of the graph.
         **kwargs: Additional keyword arguments to store any other custom attributes.
     """
 
     def __init__(
         self,
-        edge_index: Optional[mx.array] = None,
+        edge_index: mx.array,
         node_features: Optional[mx.array] = None,
         edge_features: Optional[mx.array] = None,
         graph_features: Optional[mx.array] = None,
         node_labels: Optional[mx.array] = None,
         edge_labels: Optional[mx.array] = None,
         graph_labels: Optional[mx.array] = None,
         **kwargs,
@@ -66,31 +69,26 @@
 
         Returns:
             A dictionary with all attributes of the `GraphData` object.
         """
         return {k: v for k, v in self.__dict__.items() if v is not None}
 
     @property
-    def num_nodes(self) -> Union[int, None]:
+    def num_nodes(self) -> int:
         """Number of nodes in the graph."""
         if self.node_features is not None:
             return self.node_features.shape[0]
-
-        # NOTE: This may be slow for large graphs
-        elif self.edge_index is not None:
-            return np.unique(self.edge_index).size
-        return None
+        else:
+            # NOTE: This may be slow for large graphs
+            return np.unique(np.array(self.edge_index, copy=False)).size
 
     @property
-    def num_edges(self) -> Union[int, None]:
+    def num_edges(self) -> int:
         """Number of edges in the graph"""
-        if self.edge_index is not None:
-            return self.edge_index.shape[1]
-
-        return None
+        return self.edge_index.shape[1]
 
     @property
     def num_node_classes(self) -> int:
         """Returns the number of node classes in the current graph."""
         return self._num_classes("node")
 
     @property
@@ -169,7 +167,24 @@
 
         Returns:
             Incrementing value for the given attribute or None.
         """
         if "index" in key:
             return self.num_nodes
         return None
+
+    def has_isolated_nodes(self) -> bool:
+        """Returns a boolean of whether the graph has isolated nodes or not
+        (i.e., nodes that don't have a link to any other nodes)"""
+        return has_isolated_nodes(self.edge_index, self.num_nodes)
+
+    def has_self_loops(self) -> bool:
+        """Returns a boolean of whether the graph contains self loops."""
+        return has_self_loops(self.edge_index)
+
+    def is_undirected(self) -> bool:
+        """Returns a boolean of whether the graph is undirected or not."""
+        return is_undirected(self.edge_index, self.edge_features)
+
+    def is_directed(self) -> bool:
+        """Returns a boolean of whether the graph is directed or not."""
+        return not self.is_undirected()
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs/data/utils.py` & `mlx-graphs-0.0.6/mlx_graphs/data/utils.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/dataset.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,20 +34,21 @@
             By default, no transformation is applied.
     """
 
     def __init__(
         self,
         name: str,
         base_dir: Optional[str] = None,
+        pre_transform: Optional[Callable] = None,
         transform: Optional[Callable] = None,
     ):
         self._name = name
         self._base_dir = base_dir if base_dir else DEFAULT_BASE_DIR
         self.transform = transform
-
+        self.pre_transform = pre_transform
         self.graphs: list[GraphData] = []
         self._load()
 
     @property
     def name(self) -> str:
         """
         Name of the dataset
@@ -130,14 +131,22 @@
             if os.path.exists(self.raw_path):
                 return
             os.makedirs(self.raw_path, exist_ok=True)
             print(f"Downloading {self.name} raw data ...", end=" ")
             self.download()
             print("Done")
 
+    def _process(self):
+        self.process()
+
+        if self.pre_transform:
+            print(f"Applying pre-transform to {self.name} data ...", end=" ")
+            self.graphs = [self.pre_transform(graph) for graph in self.graphs]
+            print("Done")
+
     def _save(self):
         if self._base_dir is not None and self.processed_path is not None:
             if not os.path.exists(self.processed_path):
                 os.makedirs(self.processed_path, exist_ok=True)
         print(f"Saving processed {self.name} data ...", end=" ")
         self.save()
         print("Done")
@@ -148,15 +157,15 @@
         try:
             print(f"Loading {self.name} data ...", end=" ")
             self.load()
             print("Done")
         except FileNotFoundError:
             self._download()
             print(f"Processing {self.name} raw data ...", end=" ")
-            self.process()
+            self._process()
             print("Done")
             self._save()
 
     def _num_classes(self, task: Literal["node", "edge", "graph"]) -> int:
         flattened_labels = [
             getattr(g, f"{task}_labels")
             for g in self.graphs
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/elliptic.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/elliptic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Callable, Optional
 
 import mlx.core as mx
 import numpy as np
 
 from mlx_graphs.data import GraphData
 from mlx_graphs.datasets.dataset import Dataset
 from mlx_graphs.datasets.utils import download, extract_archive
@@ -23,18 +23,35 @@
     flows, with two percent of nodes (4,545) labelled as illicit, and
     twenty-one percent of nodes (42,019) labelled as licit.
     The remaining transactions are unknown
 
     Args:
         base_dir: Directory where to store dataset files. Default is
             in the local directory ``.mlx_graphs_data/``.
+        pre_transform: A function/transform which
+            takes in a GraphData object and returns a transformed
+            version. The data will be transformed before saving to
+            the disk.
+        transforms: A function/transform that
+            takes in a graphData object and returns a transformed version
+            The data object will be transformed before every access
     """
 
-    def __init__(self, base_dir: Optional[str] = None):
-        super().__init__(name="ellipticBitcoin", base_dir=base_dir)
+    def __init__(
+        self,
+        base_dir: Optional[str] = None,
+        pre_transform: Optional[Callable] = None,
+        transform: Optional[Callable] = None,
+    ):
+        super().__init__(
+            name="ellipticBitcoin",
+            base_dir=base_dir,
+            pre_transform=pre_transform,
+            transform=transform,
+        )
 
     @property
     def raw_file_names(self):
         return [
             "elliptic_txs_features.csv",
             "elliptic_txs_edgelist.csv",
             "elliptic_txs_classes.csv",
@@ -95,8 +112,9 @@
         graph = GraphData(
             edge_index=edge_index_numpy_array,
             node_features=node_features_np,
             node_labels=y_numpy,
         )
         graph.train_mask = train_mask
         graph.test_mask = test_mask
+
         self.graphs = [graph]
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/karate_club.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/karate_club.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/ogb_dataset.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/ogb_dataset.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/planetoid.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/planetoid.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/qm7b.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/qm7b.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/superpixel.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/superpixel.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/tu_dataset.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/tu_dataset.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/utils/download.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/utils/download.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/datasets/utils/io.py` & `mlx-graphs-0.0.6/mlx_graphs/datasets/utils/io.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/loaders/dataloaders.py` & `mlx-graphs-0.0.6/mlx_graphs/loaders/dataloaders.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/conv/gat_conv.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/conv/gat_conv.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/conv/gcn_conv.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/conv/gcn_conv.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         if self._add_self_loops:
             edge_index = add_self_loops(edge_index)
 
         row, col = edge_index
 
         # Compute node degree normalization for the mean aggregation.
-        norm: mx.array = None
+        norm: Optional[mx.array] = None
         if normalize:
             deg = degree(col, node_features.shape[0], edge_weights=edge_weights)
             # NOTE : need boolean indexing in order to zero out inf values
             deg_inv_sqrt = invert_sqrt_degree(deg)
             norm = deg_inv_sqrt[row] * deg_inv_sqrt[col]
 
         # Compute messages and aggregate them with sum and norm.
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/conv/rel_conv.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/conv/rel_conv.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/conv/sage_conv.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/conv/sage_conv.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/conv/simple_conv.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/conv/simple_conv.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/graph_network_block.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/graph_network_block.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/linear.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/linear.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/message_passing.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/message_passing.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/nn/pooling/global_pooling.py` & `mlx-graphs-0.0.6/mlx_graphs/nn/pooling/global_pooling.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/array_ops.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/array_ops.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/fs.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/fs.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/scatter.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/scatter.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/sorting.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/topology.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/topology.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/transformations.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/transformations.py`

 * *Files 15% similar despite different names*

```diff
@@ -420,7 +420,86 @@
     """
     edge_index = remove_duplicate_directed_edges(edge_index)
 
     row, col = edge_index
     edge_index = mx.stack([col, row])
 
     return edge_index
+
+
+@validate_edge_index
+def get_isolated_nodes_mask(
+    edge_index: mx.array, num_nodes: int, complement: bool = True
+) -> mx.array:
+    """Returns a mask with isolated nodes set to ``False`` to filter them out if needed.
+
+    Args:
+        edge_index: Edge index from which to remove isolated nodes.
+        num_nodes: Number of nodes of the graph.
+        complement: Wether to filter isolated or non isolated nodes.
+
+    Returns:
+        A boolean mask of size ``num_nodes`` where ``True`` means the node isn't
+        isolated and ``False`` means it is.
+
+    Example:
+
+    .. code-block:: python
+
+        edge_index = mx.array([[0, 2, 0], [2, 0, 0]])
+        mask = get_isolated_nodes_mask(edge_index, 3)
+        >>> mx.array([0,2])
+        mask = get_isolated_nodes_mask(edge_index, 3, complement=False)
+        >>> mx.array([1])
+    """
+    edge_index = remove_self_loops(edge_index)
+    indices = np.unique(edge_index.reshape(-1))
+    if complement:
+        return mx.array(indices)
+
+    return mx.array(np.setdiff1d(np.arange(num_nodes), indices))
+
+
+@validate_edge_index
+def has_isolated_nodes(edge_index: mx.array, num_nodes: int) -> bool:
+    """Function to check for isolated nodes.
+    (i.e. nodes that don't have a link to any other nodes )
+
+    Args:
+        edge_index: Edge index on which to check for isolated nodes.
+
+    Returns:
+        A boolean of whether the graph has isolated nodes.
+
+    Example:
+
+    .. code-block:: python
+
+        edge_index = mx.array([[0, 2, 0], [2, 0, 0]])
+        has_self_loops(edge_index, 3)
+        >>> True
+
+    """
+    edge_index = remove_self_loops(edge_index)
+    return np.unique(edge_index.reshape(-1)).size < num_nodes
+
+
+@validate_edge_index
+def has_self_loops(edge_index: mx.array) -> bool:
+    """Function to check for self loops.
+
+    Args:
+        edge_index: Edge index on which to check for self loops.
+
+    Returns:
+        A boolean of whether the graph has self loops.
+
+    Example:
+
+    .. code-block:: python
+
+        edge_index = mx.array([[0, 2, 0], [2, 0, 0]])
+        has_self_loops(edge_index)
+        >>> True
+    """
+
+    return ((edge_index[0] == edge_index[1]).sum() > 0).item()
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs/utils/validators.py` & `mlx-graphs-0.0.6/mlx_graphs/utils/validators.py`

 * *Files identical despite different names*

### Comparing `mlx-graphs-0.0.5/mlx_graphs.egg-info/PKG-INFO` & `mlx-graphs-0.0.6/mlx_graphs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-graphs
-Version: 0.0.5
+Version: 0.0.6
 Summary: Graph Neural Network library made for Apple Silicon
 Author: mlx-graphs contributors
 License: MIT License
         
         Copyright © 2024 mlx-graphs contributors.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,14 +42,17 @@
 Requires-Dist: fsspec==2024.2.0
 Requires-Dist: tqdm==4.66.1
 Provides-Extra: dev
 Requires-Dist: pre-commit==3.6.0; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest==7.4.4; extra == "test"
 Requires-Dist: scipy==1.12.0; extra == "test"
+Requires-Dist: networkx==3.2.1; extra == "test"
+Requires-Dist: torch==2.2.0; extra == "test"
+Requires-Dist: torch_geometric==2.5.0; extra == "test"
 Provides-Extra: docs
 Requires-Dist: ipython==8.21.0; extra == "docs"
 Requires-Dist: sphinx==7.2.6; extra == "docs"
 Requires-Dist: sphinx-book-theme==1.1.0; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints==1.25.2; extra == "docs"
 Requires-Dist: nbsphinx==0.9.3; extra == "docs"
 Requires-Dist: sphinx-gallery==0.15.0; extra == "docs"
```

### Comparing `mlx-graphs-0.0.5/mlx_graphs.egg-info/SOURCES.txt` & `mlx-graphs-0.0.6/mlx_graphs.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,23 @@
 mlx_graphs/nn/conv/__init__.py
 mlx_graphs/nn/conv/gat_conv.py
 mlx_graphs/nn/conv/gcn_conv.py
 mlx_graphs/nn/conv/gin_conv.py
 mlx_graphs/nn/conv/rel_conv.py
 mlx_graphs/nn/conv/sage_conv.py
 mlx_graphs/nn/conv/simple_conv.py
+mlx_graphs/nn/norm/__init__.py
+mlx_graphs/nn/norm/batch_norm.py
+mlx_graphs/nn/norm/instance_norm.py
+mlx_graphs/nn/norm/layer_norm.py
 mlx_graphs/nn/pooling/__init__.py
 mlx_graphs/nn/pooling/global_pooling.py
+mlx_graphs/transforms/__init__.py
+mlx_graphs/transforms/base_transform.py
+mlx_graphs/transforms/normalize_features.py
 mlx_graphs/utils/__init__.py
 mlx_graphs/utils/array_ops.py
 mlx_graphs/utils/convert.py
 mlx_graphs/utils/fs.py
 mlx_graphs/utils/scatter.py
 mlx_graphs/utils/sorting.py
 mlx_graphs/utils/topology.py
```

### Comparing `mlx-graphs-0.0.5/pyproject.toml` & `mlx-graphs-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlx-graphs"
-version = "0.0.5"
+version = "0.0.6"
 description = "Graph Neural Network library made for Apple Silicon"
 authors = [{name="mlx-graphs contributors"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">= 3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -27,14 +27,17 @@
 [project.optional-dependencies]
 dev = [
   "pre-commit==3.6.0",
 ]
 test = [
   "pytest==7.4.4",
   "scipy==1.12.0",
+  "networkx==3.2.1",
+  "torch==2.2.0",
+  "torch_geometric==2.5.0",
 ]
 docs = [
   "ipython==8.21.0",
   "sphinx==7.2.6",
   "sphinx-book-theme==1.1.0",
   "sphinx-autodoc-typehints==1.25.2",
   "nbsphinx==0.9.3",
```

