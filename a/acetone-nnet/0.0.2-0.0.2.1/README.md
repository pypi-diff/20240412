# Comparing `tmp/acetone-nnet-0.0.2.tar.gz` & `tmp/acetone-nnet-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone-nnet-0.0.2.tar", last modified: Thu Apr 11 13:54:18 2024, max compression
+gzip compressed data, was "acetone-nnet-0.0.2.1.tar", last modified: Thu Apr 11 14:09:38 2024, max compression
```

## Comparing `acetone-nnet-0.0.2.tar` & `acetone-nnet-0.0.2.1.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.970951 acetone-nnet-0.0.2/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7486 2024-04-11 13:54:18.969951 acetone-nnet-0.0.2/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.2/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-11 13:52:38.000000 acetone-nnet-0.0.2/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-11 13:54:18.970951 acetone-nnet-0.0.2/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.934951 acetone-nnet-0.0.2/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.960951 acetone-nnet-0.0.2/src/acetone-nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-10 09:23:46.000000 acetone-nnet-0.0.2/src/acetone-nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-08 07:08:56.000000 acetone-nnet-0.0.2/src/acetone-nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.961951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-08 14:47:29.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-02 08:42:49.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.962951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-09 06:42:46.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/AddBiase.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.963951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1507 2024-04-10 12:03:05.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1615 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4336 2024-04-10 06:30:50.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1512 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1627 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1626 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1523 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1522 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4008 2024-04-09 06:42:58.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.964951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3771 2024-04-10 06:54:54.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3025 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-04-08 14:37:52.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5376 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5514 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2983 2024-04-11 07:58:51.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4591 2024-04-09 06:43:05.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2390 2024-04-11 07:55:39.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3943 2024-04-09 06:43:10.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8026 2024-04-09 06:43:13.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2278 2024-04-11 08:30:13.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3208 2024-04-11 08:40:52.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.965951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3359 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3785 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2598 2024-04-09 06:42:22.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3820 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4052 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.965951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2057 2024-03-27 15:28:31.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-03-27 15:30:33.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4905 2024-04-09 06:41:46.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.966951 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7198 2024-04-09 06:42:47.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10492 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5043 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4308 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2186 2024-04-09 06:43:24.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24546 2024-04-11 12:46:53.000000 acetone-nnet-0.0.2/src/acetone-nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.966951 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.966951 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 08:21:19.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.966951 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17403 2024-04-11 08:16:46.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.967951 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3781 2024-03-26 13:37:47.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6040 2024-04-11 12:46:41.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.967951 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26622 2024-04-11 06:53:14.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-02 10:01:57.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2513 2024-04-10 08:40:40.000000 acetone-nnet-0.0.2/src/acetone-nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.967951 acetone-nnet-0.0.2/src/acetone-nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-09 08:00:06.000000 acetone-nnet-0.0.2/src/acetone-nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 13:54:18.969951 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7486 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3131 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-11 13:54:18.000000 acetone-nnet-0.0.2/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.677318 acetone-nnet-0.0.2.1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2.1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2.1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.2.1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7488 2024-04-11 14:09:38.677318 acetone-nnet-0.0.2.1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.2.1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1478 2024-04-11 14:08:39.000000 acetone-nnet-0.0.2.1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-11 14:09:38.677318 acetone-nnet-0.0.2.1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.667318 acetone-nnet-0.0.2.1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.668318 acetone-nnet-0.0.2.1/src/acetone-nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1047 2024-04-11 14:08:08.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-10 09:23:46.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-08 07:08:56.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.669318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-08 14:47:29.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-02 08:42:49.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.670318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-09 06:42:46.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/AddBiase.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.671318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1507 2024-04-10 12:03:05.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1615 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4336 2024-04-10 06:30:50.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1512 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1627 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1626 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1523 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1522 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4008 2024-04-09 06:42:58.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.672318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3771 2024-04-10 06:54:54.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3025 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6165 2024-04-08 14:37:52.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5376 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5514 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2983 2024-04-11 07:58:51.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4591 2024-04-09 06:43:05.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2390 2024-04-11 07:55:39.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3943 2024-04-09 06:43:10.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8026 2024-04-09 06:43:13.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2278 2024-04-11 08:30:13.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3208 2024-04-11 08:40:52.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.673318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3359 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3785 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2598 2024-04-09 06:42:22.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3820 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4052 2024-04-08 14:39:35.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/WrapPad.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.673318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2057 2024-03-27 15:28:31.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-03-27 15:30:33.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4905 2024-04-09 06:41:46.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.674318 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7198 2024-04-09 06:42:47.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10492 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5043 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4308 2024-04-08 14:41:25.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2186 2024-04-09 06:43:24.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24546 2024-04-11 12:46:53.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.674318 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.674318 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 08:21:19.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.675318 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17403 2024-04-11 08:16:46.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.675318 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3781 2024-03-26 13:37:47.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6040 2024-04-11 12:46:41.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.675318 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26622 2024-04-11 06:53:14.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-02 10:01:57.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2513 2024-04-10 08:40:40.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.675318 acetone-nnet-0.0.2.1/src/acetone-nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-09 08:00:06.000000 acetone-nnet-0.0.2.1/src/acetone-nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-11 14:09:38.676318 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7488 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3160 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-11 14:09:38.000000 acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone-nnet-0.0.2/COPYING` & `acetone-nnet-0.0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/LICENSE` & `acetone-nnet-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/PKG-INFO` & `acetone-nnet-0.0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.2/README.md` & `acetone-nnet-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/pyproject.toml` & `acetone-nnet-0.0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acetone-nnet"
-version = "0.0.2"
+version = "0.0.2.1"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
```

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/cli_acetone.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/cli_compare.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/Layer.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/activation_functions.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/AddBiase.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/AddBiase.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Concatenate.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Dense.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Dot.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Flatten.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Gather.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Gemm.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Input.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/MatMul.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/layers/Softmax.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/code_generator/neural_network.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/ONNX_importer/create_layer.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/format_importer/parser.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone-nnet/graph/graph_interpretor.py` & `acetone-nnet-0.0.2.1/src/acetone-nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.2/src/acetone_nnet.egg-info/PKG-INFO` & `acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.2/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone-nnet-0.0.2.1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 AUTHORS.md
 COPYING
 LICENSE
 README.md
 pyproject.toml
+src/acetone-nnet/__init__.py
 src/acetone-nnet/cli_acetone.py
 src/acetone-nnet/cli_compare.py
 src/acetone-nnet/code_generator/Layer.py
 src/acetone-nnet/code_generator/activation_functions.py
 src/acetone-nnet/code_generator/neural_network.py
 src/acetone-nnet/code_generator/layers/AddBiase.py
 src/acetone-nnet/code_generator/layers/Concatenate.py
```

