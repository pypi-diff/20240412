# Comparing `tmp/acetone-nnet-0.0.1.dev2.tar.gz` & `tmp/acetone-nnet-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone-nnet-0.0.1.dev2.tar", last modified: Fri Apr 12 12:29:20 2024, max compression
+gzip compressed data, was "acetone-nnet-0.0.1.dev3.tar", last modified: Fri Apr 12 12:33:32 2024, max compression
```

## Comparing `acetone-nnet-0.0.1.dev2.tar` & `acetone-nnet-0.0.1.dev3.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.044193 acetone-nnet-0.0.1.dev2/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev2/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev2/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev2/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 12:29:20.043193 acetone-nnet-0.0.1.dev2/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.dev2/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1481 2024-04-12 12:29:12.000000 acetone-nnet-0.0.1.dev2/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 12:29:20.044193 acetone-nnet-0.0.1.dev2/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.026193 acetone-nnet-0.0.1.dev2/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.029193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-12 12:00:11.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.031193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4055 2024-04-12 11:42:25.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1857 2024-04-12 09:31:09.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.034193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2768 2024-04-12 11:57:51.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.036193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4317 2024-04-12 11:58:31.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3989 2024-04-12 11:57:49.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.037193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2986 2024-04-12 11:58:12.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6119 2024-04-12 11:50:48.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5332 2024-04-12 11:50:34.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5441 2024-04-12 11:50:07.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2964 2024-04-12 11:57:46.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-12 11:57:44.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2371 2024-04-12 11:57:41.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3924 2024-04-12 11:57:39.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7997 2024-04-12 11:57:36.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2259 2024-04-12 11:57:16.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3189 2024-04-12 11:57:12.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.038193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3322 2024-04-12 11:49:27.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3743 2024-04-12 11:49:07.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3779 2024-04-12 11:48:34.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4011 2024-04-12 11:48:17.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.039193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4888 2024-04-12 11:57:59.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.040193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10445 2024-04-12 11:47:27.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4995 2024-04-12 11:47:33.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4264 2024-04-12 11:47:40.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2167 2024-04-12 11:57:31.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:52:53.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23576 2024-04-12 11:42:15.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.040193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.041193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.041193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    16930 2024-04-12 12:28:19.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.042193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5903 2024-04-12 12:26:13.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.042193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26120 2024-04-12 12:25:42.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.042193 acetone-nnet-0.0.1.dev2/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:29:20.043193 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3254 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 12:29:20.000000 acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.645146 acetone-nnet-0.0.1.dev3/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev3/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev3/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.dev3/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 12:33:32.644146 acetone-nnet-0.0.1.dev3/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.dev3/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1481 2024-04-12 12:33:20.000000 acetone-nnet-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 12:33:32.645146 acetone-nnet-0.0.1.dev3/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.633146 acetone-nnet-0.0.1.dev3/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.635146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1770 2024-04-12 12:00:11.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.637146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4055 2024-04-12 11:42:25.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1857 2024-04-12 09:31:09.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.639146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2768 2024-04-12 11:57:51.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.640146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4317 2024-04-12 11:58:31.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3989 2024-04-12 11:57:49.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.641146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2986 2024-04-12 11:58:12.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6119 2024-04-12 11:50:48.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5332 2024-04-12 11:50:34.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5441 2024-04-12 11:50:07.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2964 2024-04-12 11:57:46.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-12 11:57:44.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2371 2024-04-12 11:57:41.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3924 2024-04-12 11:57:39.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7997 2024-04-12 11:57:36.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2259 2024-04-12 11:57:16.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3189 2024-04-12 11:57:12.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.642146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3322 2024-04-12 11:49:27.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3743 2024-04-12 11:49:07.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3779 2024-04-12 11:48:34.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4011 2024-04-12 11:48:17.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.642146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4888 2024-04-12 11:57:59.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.643146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10445 2024-04-12 11:47:27.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4995 2024-04-12 11:47:33.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4264 2024-04-12 11:47:40.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2167 2024-04-12 11:57:31.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:52:53.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23576 2024-04-12 11:42:15.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.643146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.643146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.643146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17154 2024-04-12 12:33:03.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.643146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6008 2024-04-12 12:31:18.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.644146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26621 2024-04-12 12:31:18.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.644146 acetone-nnet-0.0.1.dev3/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 12:33:32.644146 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7491 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3254 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 12:33:32.000000 acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone-nnet-0.0.1.dev2/COPYING` & `acetone-nnet-0.0.1.dev3/COPYING`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/LICENSE` & `acetone-nnet-0.0.1.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/PKG-INFO` & `acetone-nnet-0.0.1.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.dev2/README.md` & `acetone-nnet-0.0.1.dev3/README.md`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/pyproject.toml` & `acetone-nnet-0.0.1.dev3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acetone-nnet"
-version = "0.0.1.dev2"
+version = "0.0.1.dev3"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
```

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/__init__.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/cli_acetone.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/cli_compare.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/Layer.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/__init__.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/activation_functions.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Input.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/code_generator/neural_network.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,21 @@
 
 import json
 from itertools import islice
 import numpy as np
 
 from ...graph import graph_interpretor
 
-from ...code_generator import (
-    AveragePooling2D, MaxPooling2D,
-    Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
-    Constant_Pad,
-    Add, Multiply, Subtract, Maximum, Minimum, Average,
-    ResizeCubic, ResizeLinear, ResizeNearest,
-    Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten,
-    Linear, ReLu, Sigmoid, TanH)
+from ...code_generator.layers import AveragePooling2D, MaxPooling2D
+from ...code_generator.layers import Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm 
+from ...code_generator.layers import Constant_Pad
+from ...code_generator.layers import Add, Multiply, Subtract, Divide, Maximum, Minimum, Average
+from ...code_generator.layers import ResizeCubic, ResizeLinear, ResizeNearest
+from ...code_generator.layers import  Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten
+from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH
 
 def create_actv_function_obj(activation_str):
 
         if activation_str == 'sigmoid':
             return Sigmoid()
         elif activation_str == 'relu':
             return ReLu()
@@ -216,15 +215,15 @@
                 current_layer = Minimum(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Average':
-                current_layer = Average(idx = layer['config']['idx'], 
+                current_layer = Average.Average(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Dot':
                 current_layer = Dot(idx = layer['config']['idx'],
```

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 
 import tensorflow as tf
 import numpy as np
 
 from . import nnet_normalize
 
-from ...code_generator import Dense, InputLayer, Linear, ReLu
+from ...code_generator.layers.Dense import Dense
+from ...code_generator.layers.Input import InputLayer
+from ...code_generator.activation_functions import Linear, ReLu
 
 tf.keras.backend.set_floatx('float32')
 
 
 def load_nnet(file_to_parse, normalize):
     """
     Reads nnet networks from ACAS project and to pull it in .h5 format
```

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,58 +18,56 @@
  ******************************************************************************
 """
 
 
 import numpy as np
 import onnx
 
-from ...code_generator import (
-    AveragePooling2D, MaxPooling2D,
-    Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
-    Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
-    Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
-    ResizeCubic, ResizeLinear, ResizeNearest,
-    Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias,
-    )
+from ...code_generator.layers.Pooling_layers import AveragePooling2D, MaxPooling2D
+from ...code_generator.layers.Conv_layers import Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm 
+from ...code_generator.layers.Pad_layers import EdgePad, WrapPad, ReflectPad, ConstantPad
+from ...code_generator.layers.Broadcast_layers import Add, Multiply, Subtract, Divide, Maximum, Minimum, Average
+from ...code_generator.layers.Resize_layers import ResizeCubic, ResizeLinear, ResizeNearest
+from ...code_generator.layers import  Concatenate, Input, Softmax,  Dot, Gather, Gemm, MatMul, AddBias
 
 from ...code_generator import activation_functions
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
-        return Conv2D_6loops(**kwargs)
+        return Conv2D_6loops.Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
-        return Conv2D_std_gemm(**kwargs)   
+        return Conv2D_std_gemm.Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
-        return Conv2D_indirect_gemm(**kwargs)
+        return Conv2D_indirect_gemm.Conv2D_indirect_gemm(**kwargs)
         
 
 def create_resize_obj(mode, **kwargs):
     if mode == b'nearest':
-        return ResizeNearest(**kwargs)
+        return ResizeNearest.ResizeNearest(**kwargs)
     
     elif mode == b'linear':
-        return ResizeLinear(**kwargs)
+        return ResizeLinear.ResizeLinear(**kwargs)
     
     elif mode == b'cubic':
-        return ResizeCubic(**kwargs)
+        return ResizeCubic.ResizeCubic(**kwargs)
 
 def create_pad_obj(mode, **kwargs):
     if mode == b'constant':
-        return Constant_Pad(**kwargs)
+        return ConstantPad.Constant_Pad(**kwargs)
     elif mode == b'edge':
-        return Edge_pad(**kwargs)
+        return EdgePad.Edge_pad(**kwargs)
     elif mode == b'wrap':
-        return Wrap_pad(**kwargs)
+        return WrapPad.Wrap_pad(**kwargs)
     elif mode == b'reflect':
-        return Reflect_pad(**kwargs)
+        return ReflectPad.Reflect_pad(**kwargs)
 
 #Go find the constant named initialzer_name in model(an onnx model)
 def look_for_initializer(initializer_name,model):
     if (initializer_name == ''):
         return []
     for initializer in model.graph.initializer:
         if (initializer.name == initializer_name):
@@ -117,23 +115,23 @@
 
 #Create an input layers 
 def create_Input_Layer(input_layer,idx,dict_output):
         dict_output[input_layer.name] = idx
         output_shape = [input_layer.type.tensor_type.shape.dim[i].dim_value for i in range(len(input_layer.type.tensor_type.shape.dim))]
         size = find_size(output_shape)
         
-        return InputLayer(idx,size,output_shape,'channels_first')
+        return Input.InputLayer(idx,size,output_shape,'channels_first')
 
 #Create a layer Softmax
 def create_Softmax(node,idx,dict_input,dict_output,model):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Softmax(idx = idx,
+    return Softmax.Softmax(idx = idx,
                             size = size)
 
 
 #Create a layer Conv
 def create_Conv(node,idx,dict_input,dict_output,model,conv_algorithm):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
@@ -179,15 +177,15 @@
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
-    return Concatenate(idx,
+    return Concatenate.Concatenate(idx,
                                 size, 
                                 attributs['axis'],
                                 input_shapes,
                                 output_shape,
                                 activation_function= activation_functions.Linear())
     
 #Create a layer Resize
@@ -273,15 +271,15 @@
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     initializer = look_for_initializer(node.input[1],model)
-    return Gather(idx = idx,
+    return Gather.Gather(idx = idx,
                          size = size,
                          axis = attributs['axis'],
                          indices = onnx.numpy_helper.to_array(initializer),
                          input_shape = input_shape,
                          output_shape = output_shape,
                          activation_function = activation_functions.Linear())
 
@@ -302,15 +300,15 @@
         attributs['transA'] = 0
     if('transB' not in attributs):
         attributs['transB'] = 0
     if('alpha' not in attributs):
         attributs['alpha'] = 1.0
     if('beta' not in attributs):
         attributs['beta'] = 1.0
-    return Gemm(idx = idx,
+    return Gemm.Gemm(idx = idx,
                        size = size,
                        alpha = attributs['alpha'],
                        beta = attributs['beta'],
                        transA = attributs['transA'],
                        transB = attributs['transB'],
                        weights = onnx.numpy_helper.to_array(B_tensor),
                        bias = onnx.numpy_helper.to_array(C_tensor),
@@ -336,27 +334,27 @@
         if(left_tensor and not right_tensor):
             #the weigth is the right tensor:  MatMul(W,T)
             side = False
             weights = onnx.numpy_helper.to_array(left_tensor)
             weights = np.reshape(weights, (1,1,get_shape(node.input[0],model)[-1],output_shape[-1]))
             dict_input[idx] = [node.input[0]]
             input_shape = get_shape(node.input[0],model)
-        return MatMul(idx = idx,
+        return MatMul.MatMul(idx = idx,
                              size = size,
                              input_shape = input_shape,
                              weights = weights,
                              side = side,
                              activation_function = activation_functions.Linear())
     else:
         dict_input[idx] = node.input
         input_shapes =[]
         for input in node.input:
             input_shapes.append(get_shape(input,model))
         # to check
-        return Dot(idx = idx,
+        return Dot.Dot(idx = idx,
                        size = size,
                        axis = [-1,-2],
                        input_shapes = input_shapes,
                        output_shape = output_shape,
                        activation_function = activation_functions.Linear())
 
 ### Pooling layers ###
@@ -371,15 +369,15 @@
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = 1
     if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
-    return MaxPooling2D(idx = idx,
+    return MaxPooling2D.MaxPooling2D(idx = idx,
                                 size = size,
                                 padding =attributs['auto_pad'],
                                 strides = attributs['strides'][0],
                                 pool_size = attributs['kernel_shape'][0],
                                 input_shape = input_shape,
                                 output_shape = output_shape,
                                 activation_function = activation_functions.Linear())
@@ -394,15 +392,15 @@
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = 1
     if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
-    return AveragePooling2D(idx=idx,
+    return AveragePooling2D.AveragePooling2D(idx=idx,
                                    size=size, 
                                    padding=attributs['auto_pad'],
                                    strides=attributs['strides'][0], 
                                    pool_size=attributs['kernel_shape'][0], 
                                    input_shape=input_shape,
                                    output_shape=output_shape,
                                    activation_function = activation_functions.Linear())
@@ -410,15 +408,15 @@
 #Create a layer GlobalAveragePool
 def create_GlobalAveragePool(node,idx,dict_input,dict_output,model):
     input_shape = get_shape(node.input[0],model)
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return AveragePooling2D(idx = idx,
+    return AveragePooling2D.AveragePooling2D(idx = idx,
                                     size = size,
                                     padding = [0,0,0,0],
                                     strides = 0,
                                     pool_size = input_shape[2],
                                     input_shape = input_shape,
                                     output_shape = output_shape,
                                     activation_function = activation_functions.Linear())
@@ -433,116 +431,116 @@
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
     if(not right_tensor and not left_tensor):
         input_shapes =[]
         for input in node.input:
             input_shapes.append(get_shape(input,model))
         dict_input[idx] = node.input
-        return Add(idx=idx,
+        return Add.Add(idx=idx,
                         size=size,
                         input_shapes=input_shapes,
                         output_shape=output_shape,
                         activation_function= activation_functions.Linear())
     else:
         if(right_tensor):
             biases = onnx.numpy_helper.to_array(right_tensor)
             dict_input[idx] = [node.input[1]]
         elif(left_tensor):
             biases = onnx.numpy_helper.to_array(left_tensor)
             dict_input[idx] = [node.input[0]]
-        return Add_Bias(idx = idx,
+        return AddBias.Add_Bias(idx = idx,
                                   size = size,
                                   biases = biases,
                                   activation_function = activation_functions.Linear())
     
 #create a layer Div
 def create_Div(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Divide(idx=idx,
+    return Divide.Divide(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
 
 #create a layer Mul
 def create_Mul(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Multiply(idx=idx,
+    return Multiply.Multiply(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
 
 #create a layer Sub
 def create_Sub(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Subtract(idx=idx,
+    return Subtract.Subtract(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
     
 #create a layer Max
 def create_Max(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Maximum(idx=idx,
+    return Maximum.Maximum(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
 
 #create a layer Min
 def create_Min(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Minimum(idx=idx,
+    return Minimum.Minimum(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
 
 #create a layer Average
 def create_Avg(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
-    return Average(idx=idx,
+    return Average.Average(idx=idx,
                       size=size,
                       input_shapes=input_shapes,
                       output_shape=output_shape,
                       activation_function= activation_functions.Linear())
 
 ###### Dict of all the functions ######
 layer_type = {"Softmax":create_Softmax,
```

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/format_importer/parser.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet/graph/graph_interpretor.py` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/PKG-INFO` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.dev2/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone-nnet-0.0.1.dev3/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

