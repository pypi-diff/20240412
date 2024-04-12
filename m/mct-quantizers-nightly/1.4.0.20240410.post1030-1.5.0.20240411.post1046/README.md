# Comparing `tmp/mct-quantizers-nightly-1.4.0.20240410.post1030.tar.gz` & `tmp/mct-quantizers-nightly-1.5.0.20240411.post1046.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.4.0.20240410.post1030.tar", last modified: Wed Apr 10 00:10:31 2024, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.5.0.20240411.post1046.tar", last modified: Thu Apr 11 00:10:48 2024, max compression
```

## Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030.tar` & `mct-quantizers-nightly-1.5.0.20240411.post1046.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.185199 mct-quantizers-nightly-1.4.0.20240410.post1030/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-10 00:10:31.185199 mct-quantizers-nightly-1.4.0.20240410.post1030/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.173199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.177199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.177199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.177199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.177199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.177199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.181198 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/onnxruntime_session_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/onnxruntime_validations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14196 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.181198 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.181198 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.181198 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-10 00:10:19.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 00:10:31.185199 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-10 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-10 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-10 00:10:31.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 00:10:31.185199 mct-quantizers-nightly-1.4.0.20240410.post1030/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-10 00:10:30.000000 mct-quantizers-nightly-1.4.0.20240410.post1030/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.210299 mct-quantizers-nightly-1.5.0.20240411.post1046/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 00:10:48.210299 mct-quantizers-nightly-1.5.0.20240411.post1046/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.198299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.198299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.202299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21750 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.202299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.202299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5421 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.202299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.206299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4680 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/onnxruntime_session_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/onnxruntime_validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14180 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.206299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.206299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10019 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11047 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.206299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15290 2024-04-11 00:10:35.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:10:48.210299 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-11 00:10:47.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-11 00:10:48.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:10:47.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 00:10:47.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-11 00:10:47.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 00:10:48.210299 mct-quantizers-nightly-1.5.0.20240411.post1046/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-11 00:10:46.000000 mct-quantizers-nightly-1.5.0.20240411.post1046/setup.py
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/LICENSE.md` & `mct-quantizers-nightly-1.5.0.20240411.post1046/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/PKG-INFO` & `mct-quantizers-nightly-1.5.0.20240411.post1046/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240410.post1030
+Version: 1.5.0.20240411.post1046
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/README.md` & `mct-quantizers-nightly-1.5.0.20240411.post1046/README.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 
 from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, BaseInferableQuantizer, mark_quantizer
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.keras.activation_quantization_holder import KerasActivationQuantizationHolder
 from mct_quantizers.pytorch.activation_quantization_holder import PytorchActivationQuantizationHolder
 from mct_quantizers.keras.load_model import keras_load_quantized_model
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/metadata.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/metadata.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from mct_quantizers.logger import Logger
 from mct_quantizers.common.metadata import verify_and_init_metadata
 
 
 if FOUND_TF:
     import tensorflow as tf
 
-    @tf.keras.saving.register_keras_serializable()
+    @tf.keras.utils.register_keras_serializable()
     class MetadataLayer(tf.keras.layers.Layer):
         """
         A layer for holding the metadata dictionary.
         """
         def __init__(self, metadata: Dict = None, **kwargs):
             self.metadata = metadata
             super(MetadataLayer, self).__init__(**kwargs)
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/metadata.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/metadata.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/onnxruntime_session_options.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/onnxruntime_session_options.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/onnxruntime_validations.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/onnxruntime_validations.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,16 @@
                 setattr(self, LAYER, module)
 
             self.weights_quantizers = weights_quantizers
             # Initialize positional weights:
             self.weight_values = weight_values if weight_values is not None else dict()
             for pos, weight_val in self.weight_values.items():
                 if not isinstance(weight_val, torch.Tensor):
-                    Logger.error(f'Positional weight at position {pos} should be either an ndarray or a tf.Tensor,'
-                                 f'but type is {type(weight_val)}')
+                    Logger.error(f'Positional weight at position {pos} should be a torch.Tensor, '
+                                 f'but type is {type(weight_val)}.')
 
             # Initialize functional module arguments. For examples, see the class description.
             self.op_call_args = [] if op_call_args is None else op_call_args
             self.op_call_kwargs = {} if op_call_kwargs is None else op_call_kwargs
             self.is_inputs_as_list = is_inputs_as_list
 
             # Sanity checks:
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/base_activation_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/base_weight_quantizer_autograd_function.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.4.0.20240410.post1030
+Version: 1.5.0.20240411.post1046
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel.
```

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.5.0.20240411.post1046/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.4.0.20240410.post1030/setup.py` & `mct-quantizers-nightly-1.5.0.20240411.post1046/setup.py`

 * *Files identical despite different names*

