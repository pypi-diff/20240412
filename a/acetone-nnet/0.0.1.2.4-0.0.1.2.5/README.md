# Comparing `tmp/acetone-nnet-0.0.1.2.4.tar.gz` & `tmp/acetone-nnet-0.0.1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone-nnet-0.0.1.2.4.tar", last modified: Fri Apr 12 09:25:22 2024, max compression
+gzip compressed data, was "acetone-nnet-0.0.1.2.5.tar", last modified: Fri Apr 12 09:33:25 2024, max compression
```

## Comparing `acetone-nnet-0.0.1.2.4.tar` & `acetone-nnet-0.0.1.2.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.733577 acetone-nnet-0.0.1.2.4/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.4/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.4/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.4/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 09:25:22.732577 acetone-nnet-0.0.1.2.4/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.2.4/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1480 2024-04-12 09:25:02.000000 acetone-nnet-0.0.1.2.4/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 09:25:22.733577 acetone-nnet-0.0.1.2.4/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.716577 acetone-nnet-0.0.1.2.4/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.723577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2173 2024-04-12 09:05:13.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.725577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2024 2024-04-12 09:06:27.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.727577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2785 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.728577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1507 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1615 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4332 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1512 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1627 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1626 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1523 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1522 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4006 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.729577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3771 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6157 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5374 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5502 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2981 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4587 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2388 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3941 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8014 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2276 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3206 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.729577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3355 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3777 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2598 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3812 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4044 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.730577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2057 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4903 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.730577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7198 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10484 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5035 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4304 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2184 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2988 2024-04-12 09:13:07.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24524 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.731577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.731577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.731577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17403 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.731577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6040 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.732577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26619 2024-04-12 07:12:47.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1517 2024-04-12 09:05:52.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2513 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.732577 acetone-nnet-0.0.1.2.4/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1242 2024-04-12 09:24:45.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/graph/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:25:22.732577 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3334 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 09:25:22.000000 acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.913279 acetone-nnet-0.0.1.2.5/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.5/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.5/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.5/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 09:33:25.913279 acetone-nnet-0.0.1.2.5/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.2.5/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1480 2024-04-12 09:33:05.000000 acetone-nnet-0.0.1.2.5/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 09:33:25.913279 acetone-nnet-0.0.1.2.5/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.899278 acetone-nnet-0.0.1.2.5/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.902279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2074 2024-04-12 09:29:53.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.904279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1857 2024-04-12 09:31:09.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.906279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2785 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/AddBias.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.908279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1507 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1615 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4332 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1512 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1627 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1626 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1523 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1522 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4006 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.909279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3771 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6157 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5374 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5502 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2981 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4587 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2388 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3941 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8014 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2276 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3206 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.909279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3355 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3777 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2598 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3812 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4044 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.910279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2057 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4903 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.910279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7198 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10484 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5035 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4304 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2184 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2938 2024-04-12 09:32:31.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24524 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.911279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.911279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.911279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17403 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.911279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6040 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.912279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26619 2024-04-12 07:12:47.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1377 2024-04-12 09:32:58.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2513 2024-04-12 09:03:49.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.912279 acetone-nnet-0.0.1.2.5/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1224 2024-04-12 09:30:04.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/graph/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 09:33:25.913279 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3334 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 09:33:25.000000 acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone-nnet-0.0.1.2.4/COPYING` & `acetone-nnet-0.0.1.2.5/COPYING`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/LICENSE` & `acetone-nnet-0.0.1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/PKG-INFO` & `acetone-nnet-0.0.1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.2.4
+Version: 0.0.1.2.5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.2.4/README.md` & `acetone-nnet-0.0.1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/pyproject.toml` & `acetone-nnet-0.0.1.2.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acetone-nnet"
-version = "0.0.1.2.4"
+version = "0.0.1.2.5"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
```

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/__init__.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,39 +14,38 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import acetone_nnet.graph as graph
-from graph import (
+from . import graph
+from .graph import (
     tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
 )
 
-import acetone_nnet.format_importer as format_importer
-from format_importer import (
+from . import format_importer
+from .format_importer import (
     parser, load_json, load_nnet, load_onnx, JSON_from_keras_model
 )
 
-import acetone_nnet.code_generator as code_generator
-from code_generator import (
+from . import code_generator
+from .code_generator import (
     CodeGenerator, Layer,
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
 )
 
-from acetone_nnet.cli_acetone import cli_acetone
-from acetone_nnet.cli_compare import cli_compare
-_cli = {"cli_acetone", "cli_compare"}
+from .cli_acetone import cli_acetone
+from .cli_compare import cli_compare
 
 __all__ = (
-    _cli,
+    "cli_acetone", "cli_compare",
     set(code_generator.__all__),
     set(format_importer.__all__),
     set(graph.__all__)
 )
```

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/cli_acetone.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/cli_compare.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/Layer.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/__init__.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,34 +14,31 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from code_generator.activation_functions import (
+from .activation_functions import (
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
 )
-_activationfunctions = {"ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip"}
 
-from code_generator.neural_network import CodeGenerator
-_codegenerator = {"CodeGenerator"}
+from .neural_network import CodeGenerator
 
-from code_generator.Layer import Layer
-_layer = {"Layer"}
+from .Layer import Layer
 
-from code_generator import layers
-from code_generator.layers import (
+from . import layers
+from .layers import (
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
 
 __all__ = (
-    _activationfunctions,
-    _codegenerator,
-    _layer,
+    "CodeGenerator",
+    "ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip",
+    "Layer",
     set(layers.__all__)
 )
```

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/activation_functions.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Input.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/code_generator/neural_network.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/format_importer/parser.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/format_importer/parser.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/graph/__init__.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/graph/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,10 +14,10 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from acetone_nnet.graph.graph_interpretor import tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
+from .graph_interpretor import tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
 
 __all__ = ("tri_topo", "updatepath", "setNewpath","to_save", "parcours_prof_topo")
```

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet/graph/graph_interpretor.py` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/PKG-INFO` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.2.4
+Version: 0.0.1.2.5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.2.4/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone-nnet-0.0.1.2.5/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

