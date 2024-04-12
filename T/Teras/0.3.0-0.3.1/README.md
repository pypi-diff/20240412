# Comparing `tmp/Teras-0.3.0.tar.gz` & `tmp/Teras-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Teras-0.3.0.tar", last modified: Wed Apr 10 14:42:57 2024, max compression
+gzip compressed data, was "Teras-0.3.1.tar", last modified: Fri Apr 12 08:28:17 2024, max compression
```

## Comparing `Teras-0.3.0.tar` & `Teras-0.3.1.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-10 14:42:46.000000 Teras-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-10 14:42:57.921204 Teras-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-10 14:42:46.000000 Teras-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/Teras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-10 14:42:57.000000 Teras-0.3.0/Teras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-10 14:42:46.000000 Teras-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-10 14:42:57.921204 Teras-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-10 14:42:46.000000 Teras-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/models/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.877204 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/gans/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/gans/pcgain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/generic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.881204 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/gans/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/gain_fit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/jaxgan.py
--rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain_fit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/jax/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/trainers/gain_trainer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/jax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.885204 Teras-0.3.0/teras/_src/backend/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/pcgain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/data_samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/data_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/tensorflow/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.889204 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/gans/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/gans/pcgain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.893204 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/backend/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/activation/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/categorical_extraction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_extraction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cls_token_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/continuous_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/continuous_extraction_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/generator_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ctgan/generator_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/cutmix_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.897204 Teras-0.3.0/teras/_src/layers/ft_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/layer_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/mixup.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/mixup_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/saint/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/encoder_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/projection_head.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/projection_head_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/reconstruction_head.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/saint/reconstruction_head_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/tabnet/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.901204 Teras-0.3.0/teras/_src/layers/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/encoder_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/encoder_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/layers/transformer/feedforward_layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/losses/tabnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/autoencoders/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/autoencoders/tvae/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/backbone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.905204 Teras-0.3.0/teras/_src/models/backbones/saint/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/saint/saint_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/tabnet/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/backbones/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/backbones/transformer/encoder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/gans/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.909204 Teras-0.3.0/teras/_src/models/gans/ctgan/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/ctgan/generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/gans/gain/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/discriminator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/gain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gain/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/gans/pcgain/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/pretrainers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/pretrainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/saint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/saint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.913204 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/models/tasks/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/ops/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/data_samplers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_samplers/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/preprocessing/data_transformers/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/ctgan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/data_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/gain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/preprocessing/data_transformers/tvae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/tasks/imputation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/testing/markers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/_src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/_src/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/api_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.917204 Teras-0.3.0/teras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:42:57.921204 Teras-0.3.0/teras/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 14:42:46.000000 Teras-0.3.0/teras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.981460 Teras-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-04-12 08:28:07.000000 Teras-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-12 08:28:17.977460 Teras-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-12 08:28:07.000000 Teras-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/Teras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-12 08:28:17.000000 Teras-0.3.1/Teras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11011 2024-04-12 08:28:17.000000 Teras-0.3.1/Teras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:28:17.000000 Teras-0.3.1/Teras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 08:28:17.000000 Teras-0.3.1/Teras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 08:28:07.000000 Teras-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:28:17.981460 Teras-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 08:28:07.000000 Teras-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.933460 Teras-0.3.1/teras/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/common/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/common/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/common/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7030 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.937460 Teras-0.3.1/teras/_src/backend/common/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/common/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/common/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/generic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.941460 Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15111 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/gain_fit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14369 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/jaxgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/gans/pcgain_fit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/jax/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/trainers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13241 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/trainers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/trainers/gain_trainer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/jax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.945460 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/data_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/data_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/tensorflow/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/tvae/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.949460 Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/gans/pcgain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.953460 Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/backend/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.953460 Teras-0.3.1/teras/_src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.953460 Teras-0.3.1/teras/_src/layers/activation/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/activation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/activation/gumbel_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/activation/gumbel_softmax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/categorical_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/categorical_embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/categorical_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/categorical_extraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cls_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cls_token_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cls_token_extraction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cls_token_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/continuous_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/continuous_extraction_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.957460 Teras-0.3.1/teras/_src/layers/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ctgan/discriminator_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ctgan/discriminator_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ctgan/generator_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ctgan/generator_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/cutmix_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.957460 Teras-0.3.1/teras/_src/layers/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ft_transformer/feature_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/ft_transformer/feature_tokenizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/layer_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/mixup_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.957460 Teras-0.3.1/teras/_src/layers/saint/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/encoder_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/multi_head_inter_sample_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/multi_head_inter_sample_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/projection_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/projection_head_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/reconstruction_head.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/saint/reconstruction_head_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.957460 Teras-0.3.1/teras/_src/layers/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tab_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tab_transformer/column_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tab_transformer/column_embedding_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.961460 Teras-0.3.1/teras/_src/layers/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/attentive_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/attentive_transformer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.961460 Teras-0.3.1/teras/_src/layers/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/transformer/encoder_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/transformer/encoder_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/transformer/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/layers/transformer/feedforward_layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.961460 Teras-0.3.1/teras/_src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/losses/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/losses/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/losses/tabnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.961460 Teras-0.3.1/teras/_src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.961460 Teras-0.3.1/teras/_src/models/autoencoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/autoencoders/tvae/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/encoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/tvae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/autoencoders/tvae/tvae_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/backbone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/ft_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/ft_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/ft_transformer/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/ft_transformer/ft_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/saint/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/saint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/saint/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/saint/saint_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/tab_transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tab_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6973 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tab_transformer/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tab_transformer/tab_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tabnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/tabnet/encoder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.965460 Teras-0.3.1/teras/_src/models/backbones/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/transformer/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/backbones/transformer/encoder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.969460 Teras-0.3.1/teras/_src/models/gans/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.969460 Teras-0.3.1/teras/_src/models/gans/ctgan/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/ctgan_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/discriminator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/ctgan/generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.969460 Teras-0.3.1/teras/_src/models/gans/gain/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/discriminator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/gain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gain/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.969460 Teras-0.3.1/teras/_src/models/gans/pcgain/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/pcgain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/pcgain/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/pcgain/classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/pcgain/pcgain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/gans/pcgain/pcgain_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/models/pretrainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/pretrainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/saint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/saint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tab_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tab_transformer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/decoder_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/tabnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/pretrainers/tabnet/tabnet_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/tasks/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/models/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/ops/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.973460 Teras-0.3.1/teras/_src/preprocessing/data_samplers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_samplers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_samplers/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/_src/preprocessing/data_transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24314 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_transformers/ctgan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_transformers/data_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_transformers/gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/preprocessing/data_transformers/tvae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/_src/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/tasks/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/tasks/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/_src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/testing/markers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/_src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/_src/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/api_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/data_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:28:17.977460 Teras-0.3.1/teras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-12 08:28:07.000000 Teras-0.3.1/teras/version.py
```

### Comparing `Teras-0.3.0/LICENSE` & `Teras-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/Teras.egg-info/SOURCES.txt` & `Teras-0.3.1/Teras.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 Teras.egg-info/PKG-INFO
 Teras.egg-info/SOURCES.txt
 Teras.egg-info/dependency_links.txt
 Teras.egg-info/top_level.txt
 teras/__init__.py
 teras/activations.py
```

### Comparing `Teras-0.3.0/pyproject.toml` & `Teras-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "keras>=3.1.1", "pandas", "numpy",
     "scikit-learn"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Teras"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Khawaja Abaid", email="khawaja.abaid@gmail.com" },
 ]
 description = "A Unified Deep Learning Library for Tabular Data"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `Teras-0.3.0/teras/__init__.py` & `Teras-0.3.1/teras/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/__init__.py` & `Teras-0.3.1/teras/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/activations.py` & `Teras-0.3.1/teras/_src/activations.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/activations_test.py` & `Teras-0.3.1/teras/_src/activations_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/api_export.py` & `Teras-0.3.1/teras/_src/api_export.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/__init__.py` & `Teras-0.3.1/teras/_src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/autoencoders/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/models/autoencoders/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/models/autoencoders/tvae/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/autoencoders/tvae/tvae.py` & `Teras-0.3.1/teras/_src/backend/common/models/autoencoders/tvae/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/ctgan.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/discriminator.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/ctgan/generator.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/ctgan/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/gain.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/gans/pcgain.py` & `Teras-0.3.1/teras/_src/backend/common/models/gans/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/pretrainers/saint.py` & `Teras-0.3.1/teras/_src/backend/common/models/pretrainers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tab_transformer.py` & `Teras-0.3.1/teras/_src/backend/common/models/pretrainers/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/common/models/pretrainers/tabnet.py` & `Teras-0.3.1/teras/_src/backend/common/models/pretrainers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/tvae/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/autoencoders/tvae/tvae.py` & `Teras-0.3.1/teras/_src/backend/jax/models/autoencoders/tvae/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/ctgan.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/discriminator.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/ctgan/generator.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/ctgan/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/gain.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/gain_fit_test.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/gain_fit_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/jaxgan.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/jaxgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/gans/pcgain_fit_test.py` & `Teras-0.3.1/teras/_src/backend/jax/models/gans/pcgain_fit_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/saint.py` & `Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tab_transformer.py` & `Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/models/pretrainers/tabnet.py` & `Teras-0.3.1/teras/_src/backend/jax/models/pretrainers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/trainers/__init__.py` & `Teras-0.3.1/teras/_src/backend/jax/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/trainers/ctgan.py` & `Teras-0.3.1/teras/_src/backend/jax/trainers/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/trainers/gain.py` & `Teras-0.3.1/teras/_src/backend/jax/trainers/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/jax/trainers/gain_trainer_test.py` & `Teras-0.3.1/teras/_src/backend/jax/trainers/gain_trainer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/tvae/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/autoencoders/tvae/tvae.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/autoencoders/tvae/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/ctgan.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/discriminator.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/ctgan/generator.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/ctgan/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/gain.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/gans/pcgain.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/gans/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/saint.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tab_transformer.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/models/pretrainers/tabnet.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/models/pretrainers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/preprocessing/data_samplers/__init__.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/preprocessing/data_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/utils.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/tensorflow/utils_test.py` & `Teras-0.3.1/teras/_src/backend/tensorflow/utils_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/tvae/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/autoencoders/tvae/tvae.py` & `Teras-0.3.1/teras/_src/backend/torch/models/autoencoders/tvae/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/ctgan.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/discriminator.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/ctgan/generator.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/ctgan/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/gain.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/gans/pcgain.py` & `Teras-0.3.1/teras/_src/backend/torch/models/gans/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/__init__.py` & `Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/saint.py` & `Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tab_transformer.py` & `Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/models/pretrainers/tabnet.py` & `Teras-0.3.1/teras/_src/backend/torch/models/pretrainers/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/backend/torch/utils.py` & `Teras-0.3.1/teras/_src/backend/torch/utils.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/data_utils.py` & `Teras-0.3.1/teras/_src/data_utils.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/__init__.py` & `Teras-0.3.1/teras/_src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/activation/__init__.py` & `Teras-0.3.1/teras/_src/layers/activation/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax.py` & `Teras-0.3.1/teras/_src/layers/activation/gumbel_softmax.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/activation/gumbel_softmax_test.py` & `Teras-0.3.1/teras/_src/layers/activation/gumbel_softmax_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/categorical_embedding.py` & `Teras-0.3.1/teras/_src/layers/categorical_embedding.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/categorical_embedding_test.py` & `Teras-0.3.1/teras/_src/layers/categorical_embedding_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/categorical_extraction.py` & `Teras-0.3.1/teras/_src/layers/categorical_extraction.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/categorical_extraction_test.py` & `Teras-0.3.1/teras/_src/layers/categorical_extraction_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/cls_token.py` & `Teras-0.3.1/teras/_src/layers/cls_token.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/cls_token_extraction.py` & `Teras-0.3.1/teras/_src/layers/cls_token_extraction.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/cls_token_extraction_test.py` & `Teras-0.3.1/teras/_src/layers/cls_token_extraction_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/cls_token_test.py` & `Teras-0.3.1/teras/_src/layers/cls_token_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/continuous_extraction.py` & `Teras-0.3.1/teras/_src/layers/continuous_extraction.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/continuous_extraction_test.py` & `Teras-0.3.1/teras/_src/layers/continuous_extraction_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/layers/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer.py` & `Teras-0.3.1/teras/_src/layers/ctgan/discriminator_layer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ctgan/discriminator_layer_test.py` & `Teras-0.3.1/teras/_src/layers/ctgan/discriminator_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ctgan/generator_layer.py` & `Teras-0.3.1/teras/_src/layers/ctgan/generator_layer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ctgan/generator_layer_test.py` & `Teras-0.3.1/teras/_src/layers/ctgan/generator_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/cutmix.py` & `Teras-0.3.1/teras/_src/layers/cutmix.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ft_transformer/__init__.py` & `Teras-0.3.1/teras/_src/layers/ft_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer.py` & `Teras-0.3.1/teras/_src/layers/ft_transformer/feature_tokenizer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/ft_transformer/feature_tokenizer_test.py` & `Teras-0.3.1/teras/_src/layers/ft_transformer/feature_tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/layer_list.py` & `Teras-0.3.1/teras/_src/layers/layer_list.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/mixup.py` & `Teras-0.3.1/teras/_src/layers/mixup.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/mixup_test.py` & `Teras-0.3.1/teras/_src/layers/mixup_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/__init__.py` & `Teras-0.3.1/teras/_src/layers/saint/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/embedding.py` & `Teras-0.3.1/teras/_src/layers/saint/embedding.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,7 +74,19 @@
             feature_embeddings = embedding_layer(feature)
             if len(ops.shape(feature_embeddings)) == 2:
                 feature_embeddings = ops.expand_dims(
                     feature_embeddings, axis=1)
             embeddings = ops.concatenate([embeddings, feature_embeddings],
                                          axis=1)
         return embeddings
+
+    def get_config(self):
+        config = super().get_config()
+        config.update({
+            "embedding_dim": self.embedding_dim,
+            "cardinalities": self.cardinalities
+        })
+        return config
+
+    @classmethod
+    def from_config(cls, config):
+        return cls(**config)
```

### Comparing `Teras-0.3.0/teras/_src/layers/saint/embedding_test.py` & `Teras-0.3.1/teras/_src/layers/saint/embedding_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/encoder_layer.py` & `Teras-0.3.1/teras/_src/layers/saint/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/encoder_layer_test.py` & `Teras-0.3.1/teras/_src/layers/saint/encoder_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention.py` & `Teras-0.3.1/teras/_src/layers/saint/multi_head_inter_sample_attention.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/multi_head_inter_sample_attention_test.py` & `Teras-0.3.1/teras/_src/layers/saint/multi_head_inter_sample_attention_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/projection_head.py` & `Teras-0.3.1/teras/_src/layers/saint/projection_head.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/projection_head_test.py` & `Teras-0.3.1/teras/_src/layers/saint/projection_head_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/reconstruction_head.py` & `Teras-0.3.1/teras/_src/layers/saint/reconstruction_head.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/saint/reconstruction_head_test.py` & `Teras-0.3.1/teras/_src/layers/saint/reconstruction_head_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tab_transformer/__init__.py` & `Teras-0.3.1/teras/_src/layers/tab_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding.py` & `Teras-0.3.1/teras/_src/layers/tab_transformer/column_embedding.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tab_transformer/column_embedding_test.py` & `Teras-0.3.1/teras/_src/layers/tab_transformer/column_embedding_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/__init__.py` & `Teras-0.3.1/teras/_src/layers/tabnet/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer.py` & `Teras-0.3.1/teras/_src/layers/tabnet/attentive_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/attentive_transformer_test.py` & `Teras-0.3.1/teras/_src/layers/tabnet/attentive_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer.py` & `Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer.py` & `Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_layer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_layer_test.py` & `Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/tabnet/feature_transformer_test.py` & `Teras-0.3.1/teras/_src/layers/tabnet/feature_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/transformer/__init__.py` & `Teras-0.3.1/teras/_src/layers/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/transformer/encoder_layer.py` & `Teras-0.3.1/teras/_src/layers/transformer/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/transformer/encoder_layer_test.py` & `Teras-0.3.1/teras/_src/layers/transformer/encoder_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/transformer/feedforward.py` & `Teras-0.3.1/teras/_src/layers/transformer/feedforward.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/layers/transformer/feedforward_layer_test.py` & `Teras-0.3.1/teras/_src/layers/transformer/feedforward_layer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/losses/__init__.py` & `Teras-0.3.1/teras/_src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/losses/ctgan.py` & `Teras-0.3.1/teras/_src/losses/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/losses/saint.py` & `Teras-0.3.1/teras/_src/losses/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/losses/tabnet.py` & `Teras-0.3.1/teras/_src/losses/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/__init__.py` & `Teras-0.3.1/teras/_src/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/__init__.py` & `Teras-0.3.1/teras/_src/models/autoencoders/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/__init__.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/decoder.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/decoder_test.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/decoder_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/encoder.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/encoder_test.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/encoder_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/autoencoders/tvae/tvae_test.py` & `Teras-0.3.1/teras/_src/models/autoencoders/tvae/tvae_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/backbone.py` & `Teras-0.3.1/teras/_src/models/backbones/backbone.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/ft_transformer/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/ft_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer.py` & `Teras-0.3.1/teras/_src/models/backbones/ft_transformer/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/ft_transformer/ft_transformer_test.py` & `Teras-0.3.1/teras/_src/models/backbones/ft_transformer/ft_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/saint/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/saint/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/saint/saint.py` & `Teras-0.3.1/teras/_src/models/backbones/saint/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/saint/saint_test.py` & `Teras-0.3.1/teras/_src/models/backbones/saint/saint_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tab_transformer/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/tab_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer.py` & `Teras-0.3.1/teras/_src/models/backbones/tab_transformer/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tab_transformer/tab_transformer_test.py` & `Teras-0.3.1/teras/_src/models/backbones/tab_transformer/tab_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tabnet/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/tabnet/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder.py` & `Teras-0.3.1/teras/_src/models/backbones/tabnet/encoder.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/tabnet/encoder_test.py` & `Teras-0.3.1/teras/_src/models/backbones/tabnet/encoder_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/transformer/__init__.py` & `Teras-0.3.1/teras/_src/models/backbones/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/transformer/encoder.py` & `Teras-0.3.1/teras/_src/models/backbones/transformer/encoder.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/backbones/transformer/encoder_test.py` & `Teras-0.3.1/teras/_src/models/backbones/transformer/encoder_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/__init__.py` & `Teras-0.3.1/teras/_src/models/gans/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/__init__.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/ctgan_test.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/ctgan_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/discriminator_test.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/discriminator_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/generator.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/ctgan/generator_test.py` & `Teras-0.3.1/teras/_src/models/gans/ctgan/generator_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/__init__.py` & `Teras-0.3.1/teras/_src/models/gans/gain/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/discriminator.py` & `Teras-0.3.1/teras/_src/models/gans/gain/discriminator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/discriminator_test.py` & `Teras-0.3.1/teras/_src/models/gans/gain/discriminator_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/gain.py` & `Teras-0.3.1/teras/_src/models/gans/gain/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/gain_test.py` & `Teras-0.3.1/teras/_src/models/gans/gain/gain_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/generator.py` & `Teras-0.3.1/teras/_src/models/gans/gain/generator.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gain/generator_test.py` & `Teras-0.3.1/teras/_src/models/gans/gain/generator_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/gan.py` & `Teras-0.3.1/teras/_src/models/gans/gan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/pcgain/__init__.py` & `Teras-0.3.1/teras/_src/models/gans/pcgain/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/pcgain/classifier.py` & `Teras-0.3.1/teras/_src/models/gans/pcgain/classifier.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/pcgain/classifier_test.py` & `Teras-0.3.1/teras/_src/models/gans/pcgain/classifier_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain.py` & `Teras-0.3.1/teras/_src/models/gans/pcgain/pcgain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/gans/pcgain/pcgain_test.py` & `Teras-0.3.1/teras/_src/models/gans/pcgain/pcgain_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/__init__.py` & `Teras-0.3.1/teras/_src/models/pretrainers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/pretrainer.py` & `Teras-0.3.1/teras/_src/models/pretrainers/pretrainer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/saint.py` & `Teras-0.3.1/teras/_src/models/pretrainers/saint.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/saint_test.py` & `Teras-0.3.1/teras/_src/models/pretrainers/saint_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tab_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tab_transformer_test.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tab_transformer_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/__init__.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tabnet/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tabnet/decoder.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/decoder_test.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tabnet/decoder_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tabnet/tabnet.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/pretrainers/tabnet/tabnet_test.py` & `Teras-0.3.1/teras/_src/models/pretrainers/tabnet/tabnet_test.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/tasks/__init__.py` & `Teras-0.3.1/teras/_src/models/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/models/tasks/classification.py` & `Teras-0.3.1/teras/_src/models/tasks/regression.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import keras
 
 from teras._src.models.tasks.task import Task
-from teras._src.typing import ActivationType
 from teras._src.api_export import teras_export
+from teras._src.typing import ActivationType
 
 
-@teras_export("teras.models.Classifier")
-class Classifier(Task):
+@teras_export("teras.models.Regressor")
+class Regressor(Task):
     """
-    Classifier class that provides a dense prediction head.
+    Regressor class that provides a dense prediction head.
 
     Args:
-        backbone: `keras.Model` instance, backbone is called on
+        backbone: `keras.Model` instance. Backbone is called on
             inputs followed by the dense head that produces predictions.
-        num_classes: int, number of classes to predict.
-        activation: str or callable, activation function to use for
-        outputs. Defaults to "softmax"
+        num_outputs: int, number of regression outputs to predict.
+        hidden_dim: int, hidden dimensionality of the dense head.
+            Defaults to 1024.
+        hidden_activation: str or callable, activation for the hidden layer.
+            Defaults to "relu".
     """
     def __init__(self,
                  backbone: keras.Model,
-                 num_classes: int,
-                 activation: ActivationType = "softmax",
+                 num_outputs: int,
+                 hidden_dim: int = 1024,
+                 hidden_activation: ActivationType = "relu",
                  **kwargs):
         inputs = backbone.input
         x = backbone(inputs)
         # In case the backbone outputs are of shape (None, a, b),
         # for instance in the case of transformer based models
         x = keras.layers.Flatten()(x)
-        outputs = keras.layers.Dense(num_classes,
-                                     activation=activation,
+        x = keras.layers.Dense(hidden_dim, activation=hidden_activation,
+                               name="hidden_layer_regression_head")(x)
+        outputs = keras.layers.Dense(num_outputs,
                                      name="predictions")(x)
         super().__init__(inputs, outputs, **kwargs)
 
         self.backbone = backbone
-        self.num_classes = num_classes
-        self.activation = activation
+        self.num_outputs = num_outputs
+        self.hidden_dim = hidden_dim
+        self.hidden_activation = hidden_activation
 
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "backbone": keras.layers.serialize(self.backbone),
-                "num_classes": self.num_classes,
-                "activation": self.activation
+                "num_outputs": self.num_outputs,
+                "hidden_dim": self.hidden_dim,
+                "hidden_activation": self.hidden_activation
             }
         )
```

### Comparing `Teras-0.3.0/teras/_src/models/tasks/task.py` & `Teras-0.3.1/teras/_src/models/tasks/task.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/ops/__init__.py` & `Teras-0.3.1/teras/_src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/ops/ops.py` & `Teras-0.3.1/teras/_src/ops/ops.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/__init__.py` & `Teras-0.3.1/teras/_src/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_samplers/__init__.py` & `Teras-0.3.1/teras/_src/preprocessing/data_samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_samplers/ctgan.py` & `Teras-0.3.1/teras/_src/preprocessing/data_samplers/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_samplers/tvae.py` & `Teras-0.3.1/teras/_src/preprocessing/data_samplers/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_transformers/__init__.py` & `Teras-0.3.1/teras/_src/preprocessing/data_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_transformers/ctgan.py` & `Teras-0.3.1/teras/_src/preprocessing/data_transformers/ctgan.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_transformers/data_transformer.py` & `Teras-0.3.1/teras/_src/preprocessing/data_transformers/data_transformer.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_transformers/gain.py` & `Teras-0.3.1/teras/_src/preprocessing/data_transformers/gain.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/preprocessing/data_transformers/tvae.py` & `Teras-0.3.1/teras/_src/preprocessing/data_transformers/tvae.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/tasks/__init__.py` & `Teras-0.3.1/teras/_src/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/tasks/generation.py` & `Teras-0.3.1/teras/_src/tasks/generation.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/tasks/imputation.py` & `Teras-0.3.1/teras/_src/tasks/imputation.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/testing/__init__.py` & `Teras-0.3.1/teras/_src/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/trainers/__init__.py` & `Teras-0.3.1/teras/_src/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/typing.py` & `Teras-0.3.1/teras/_src/typing.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/_src/utils.py` & `Teras-0.3.1/teras/_src/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,37 +3,43 @@
 import numpy as np
 from warnings import warn
 from teras._src.typing import DataFrameOrNdArray
 from teras._src.api_export import teras_export
 
 
 @teras_export("teras.utils.compute_cardinalities")
-def compute_cardinalities(x, categorical_idx):
+def compute_cardinalities(x, categorical_idx: list,
+                          ordinal_encoded: bool = True):
     """
     Compute cardinalities for features in the given dataset/dataframe.
     For numerical features, 0 is used as a placeholder.
 
     Args:
         x: Input dataset or dataframe.
         categorical_idx: list, a list of indices of categorical features
             in the given dataset.
+        ordinal_encoded: `bool`, Whether the categorical values have been
+            ordinal encoded. Defaults to True.
 
     Returns:
         A 1d numpy array of cardinalities of all features.
         For numerical features, a value of 0 is used.
     """
     if isinstance(x, pd.DataFrame):
         x = x.values
 
     cardinalities = np.array([], dtype=np.uint16)
     for idx in range(ops.shape(x)[1]):
         if idx in categorical_idx:
             feature = ops.convert_to_numpy(x[:, idx])
-            cardinalities = np.append(cardinalities,
-                                      (len(np.unique(feature))))
+            if ordinal_encoded:
+                num_categories = np.max(feature) + 1
+            else:
+                num_categories = len(np.unique(feature))
+            cardinalities = np.append(cardinalities, num_categories)
         else:
             # it's a numerical feature, in which case we append 0
             cardinalities = np.append(cardinalities, 0)
     return cardinalities
 
 
 @teras_export("teras.utils.get_metadata_for_embedding")
```

### Comparing `Teras-0.3.0/teras/activations.py` & `Teras-0.3.1/teras/activations.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/api_export.py` & `Teras-0.3.1/teras/api_export.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/data_utils.py` & `Teras-0.3.1/teras/data_utils.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/layers/__init__.py` & `Teras-0.3.1/teras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/losses/__init__.py` & `Teras-0.3.1/teras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/models/__init__.py` & `Teras-0.3.1/teras/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/ops/__init__.py` & `Teras-0.3.1/teras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/preprocessing/__init__.py` & `Teras-0.3.1/teras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/tasks/__init__.py` & `Teras-0.3.1/teras/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/typing.py` & `Teras-0.3.1/teras/typing.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/utils.py` & `Teras-0.3.1/teras/utils.py`

 * *Files identical despite different names*

### Comparing `Teras-0.3.0/teras/version.py` & `Teras-0.3.1/teras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 # Unique source of truth for the version number.
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 
 def version():
     return __version__
```

