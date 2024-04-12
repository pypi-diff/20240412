# Comparing `tmp/acetone-nnet-0.0.1.2.1.tar.gz` & `tmp/acetone-nnet-0.0.1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone-nnet-0.0.1.2.1.tar", last modified: Fri Apr 12 08:24:09 2024, max compression
+gzip compressed data, was "acetone-nnet-0.0.1.2.3.tar", last modified: Fri Apr 12 08:58:05 2024, max compression
```

## Comparing `acetone-nnet-0.0.1.2.1.tar` & `acetone-nnet-0.0.1.2.3.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.051218 acetone-nnet-0.0.1.2.1/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.1/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.1/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.1/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 08:24:09.050218 acetone-nnet-0.0.1.2.1/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.2.1/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1480 2024-04-12 08:23:45.000000 acetone-nnet-0.0.1.2.1/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 08:24:09.051218 acetone-nnet-0.0.1.2.1/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.037218 acetone-nnet-0.0.1.2.1/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.040218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2062 2024-04-12 08:23:27.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.042218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2028 2024-04-12 07:41:32.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.044218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2785 2024-04-12 07:12:16.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/AddBias.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.045218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1507 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1615 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4332 2024-04-12 06:45:56.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1512 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1627 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1626 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1523 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1522 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4006 2024-04-12 06:43:28.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.046218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3771 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3023 2024-04-12 06:45:45.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6157 2024-04-12 06:45:42.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5374 2024-04-12 06:45:37.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5502 2024-04-12 06:45:29.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2981 2024-04-12 06:43:20.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4587 2024-04-12 06:43:16.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2388 2024-04-12 06:43:08.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3941 2024-04-12 06:43:04.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8014 2024-04-12 06:42:52.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2276 2024-04-12 06:42:38.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3206 2024-04-12 06:42:25.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.047218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3355 2024-04-12 06:45:10.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3777 2024-04-12 06:45:04.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2598 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3812 2024-04-12 06:44:49.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4044 2024-04-12 06:44:38.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.047218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2057 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1890 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4903 2024-04-12 06:44:17.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.048218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7198 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10484 2024-04-12 06:44:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5035 2024-04-12 06:44:02.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4304 2024-04-12 06:43:50.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2184 2024-04-12 06:42:15.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3109 2024-04-12 07:37:02.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24524 2024-04-12 07:43:08.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.048218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.049218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.049218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17403 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.049218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6040 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.049218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26619 2024-04-12 07:12:47.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1456 2024-04-12 08:05:21.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2513 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.050218 acetone-nnet-0.0.1.2.1/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1233 2024-04-12 08:14:36.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/graph/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:24:09.050218 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3334 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 08:24:09.000000 acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.506166 acetone-nnet-0.0.1.2.3/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      388 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.3/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.3/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone-nnet-0.0.1.2.3/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 08:58:05.505165 acetone-nnet-0.0.1.2.3/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6210 2024-04-02 13:15:41.000000 acetone-nnet-0.0.1.2.3/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1480 2024-04-12 08:57:57.000000 acetone-nnet-0.0.1.2.3/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-12 08:58:05.506166 acetone-nnet-0.0.1.2.3/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.489165 acetone-nnet-0.0.1.2.3/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.493165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2146 2024-04-12 08:45:28.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2787 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3845 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.495165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4079 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2080 2024-04-12 08:35:06.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4092 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.497166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2771 2024-04-12 08:51:06.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/AddBias.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.499165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1463 2024-04-12 08:56:13.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1571 2024-04-12 08:56:21.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4321 2024-04-12 08:57:14.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1468 2024-04-12 08:56:27.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1584 2024-04-12 08:56:37.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1583 2024-04-12 08:56:46.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1479 2024-04-12 08:56:51.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1478 2024-04-12 08:56:59.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3992 2024-04-12 08:51:08.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.500166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3760 2024-04-12 08:54:55.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2991 2024-04-12 08:55:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6125 2024-04-12 08:55:44.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5332 2024-04-12 08:55:28.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5460 2024-04-12 08:55:12.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2967 2024-04-12 08:51:12.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4573 2024-04-12 08:51:15.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2374 2024-04-12 08:51:18.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-04-12 08:51:31.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8002 2024-04-12 08:51:39.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2264 2024-04-12 08:51:44.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3194 2024-04-12 08:51:51.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.501165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3330 2024-04-12 08:53:56.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3752 2024-04-12 08:54:11.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2587 2024-04-12 08:53:37.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3787 2024-04-12 08:54:26.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4019 2024-04-12 08:54:43.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.502165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2016 2024-04-12 08:53:28.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1849 2024-04-12 08:53:15.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4892 2024-04-12 08:52:58.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.502165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7187 2024-04-12 08:52:41.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10450 2024-04-12 08:52:31.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5001 2024-04-12 08:52:22.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4270 2024-04-12 08:52:08.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2172 2024-04-12 08:51:55.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3109 2024-04-12 07:37:02.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    23547 2024-04-12 08:48:42.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.503166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.503166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6286 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.503166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    16882 2024-04-12 08:45:16.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.504166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3765 2024-04-12 06:47:10.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5952 2024-04-12 08:46:16.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.504166 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    26619 2024-04-12 07:12:47.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4027 2024-04-12 08:46:25.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1521 2024-04-12 08:35:49.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2317 2024-04-12 08:39:56.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.505165 acetone-nnet-0.0.1.2.3/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1246 2024-04-12 08:36:01.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/graph/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-12 08:58:05.505165 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7490 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3334 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-12 08:58:05.000000 acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone-nnet-0.0.1.2.1/COPYING` & `acetone-nnet-0.0.1.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/LICENSE` & `acetone-nnet-0.0.1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/PKG-INFO` & `acetone-nnet-0.0.1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.2.1
+Version: 0.0.1.2.3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.2.1/README.md` & `acetone-nnet-0.0.1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/pyproject.toml` & `acetone-nnet-0.0.1.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "acetone-nnet"
-version = "0.0.1.2.1"
+version = "0.0.1.2.3"
 requires-python = ">=3.10"
 
 authors = [
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
     { name="Claire PAGETTI", email="Claire.Pagetti@onera.fr" },
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/__init__.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,39 +14,39 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import graph
+from acetone_nnet import graph
 from graph import (
     tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
 )
 
-import format_importer
+from acetone_nnet import format_importer
 from format_importer import (
     parser, load_json, load_nnet, load_onnx, JSON_from_keras_model
 )
 
-import code_generator
+from acetone_nnet import code_generator
 from code_generator import (
     CodeGenerator, Layer,
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
 )
 
-from cli_acetone import cli_acetone
-from cli_compare import cli_compare
-_cli = {cli_acetone, cli_compare}
+from acetone_nnet.cli_acetone import cli_acetone
+from acetone_nnet.cli_compare import cli_compare
+_cli = {"cli_acetone", "cli_compare"}
 
 __all__ = list(
     _cli,
     set(code_generator.__all__),
     set(format_importer.__all__),
     set(graph.__all__)
 )
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/cli_acetone.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/cli_compare.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/Layer.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/__init__.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,27 +14,27 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from code_generator.activation_functions import (
+from acetone_nnet.code_generator.activation_functions import (
     ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
 )
 _activationfunctions = {"ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip"}
 
-from code_generator.neural_network import CodeGenerator
+from acetone_nnet.code_generator.neural_network import CodeGenerator
 _codegenerator = {"CodeGenerator"}
 
 from code_generator.Layer import Layer
 _layer = {"Layer"}
 
-from code_generator import layers
-from code_generator.layers import (
+from acetone_nnet.code_generator import layers
+from acetone_nnet.code_generator.layers import (
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/activation_functions.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+import acetone_nnet as Layer
 import numpy as np
 import pystache
 
-class Add_Bias(Layer.Layer):
+class Add_Bias(Layer):
 
     def __init__(self, idx, size, biases,activation_function):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Add_Biass'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
 
 #Addition of several tensor
-class Add(Broadcast.Broadcast):
+class Add(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = 'Add'
         self.specific_operator = ' + '
     
     def forward_path_layer(self, inputs):
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,21 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
 
-#Return a tensor with where each position (f,i,j) contains the average of all the values at position (f,i,j) in each tensor
-class Average(Broadcast.Broadcast):
+import numpy as np
+
+#Return a tensor with where each position (f,i,j) contains the min of all the values at position (f,i,j) in each tensor
+class Minimum(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
-        self.name = 'Average'
-        self.specific_operator = ' + '
+        self.name = 'Minimum'
+        self.specific_operator = ', '
 
     def forward_path_layer(self, inputs):
-        output = inputs[0]
+        mini = inputs[0]
         for input in inputs[1:]:
-            output +=input 
-        return self.activation_function.compute(output/(len(inputs)))
+            mini = np.minimum(mini, input)
+        return self.activation_function.compute(mini)
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,24 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
+
 from abc import abstractmethod
 import pystache
 
 #The class of the Layers which compute operation with broadcast numpy style
 #attribut: none
 #input: a list of tensor
 #output: the resultant tensor
-class Broadcast(Layer.Layer):
+class Broadcast(Layer):
     def __init__(self, idx, size, input_shapes, output_shape,activation_function):
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.input_shapes = input_shapes
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,22 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
 
-#Division of several tensors
-class Divide(Broadcast.Broadcast):
+#Multiplication of several tensors
+class Multiply(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Divide'
-        self.specific_operator = '/'
+        self.name = 'Multiply'
+        self.specific_operator = '*'
     
     def forward_path_layer(self, inputs):
         output = inputs[0]
         for input in inputs[1:]:
-            output /= input
-        return self.activation_function.compute(output)
+            output *= input
+        return self.activation_function.compute(output)
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,20 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
+
 import numpy as np
 
 #Return a tensor with where each position (f,i,j) contains the max of all the values at position (f,i,j) in each tensor
-class Maximum(Broadcast.Broadcast):
+class Maximum(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
         self.name = 'Maximum'
         self.specific_operator = ', '
 
     def forward_path_layer(self, inputs):
         maxi = inputs[0]
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,22 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
-import numpy as np
+from acetone_nnet import Broadcast
 
-#Return a tensor with where each position (f,i,j) contains the min of all the values at position (f,i,j) in each tensor
-class Minimum(Broadcast.Broadcast):
+#Return a tensor with where each position (f,i,j) contains the average of all the values at position (f,i,j) in each tensor
+class Average(Broadcast):
     def __init__(self,**kwargs):
         super().__init__(**kwargs)
-        self.name = 'Minimum'
-        self.specific_operator = ', '
+        self.name = 'Average'
+        self.specific_operator = ' + '
 
     def forward_path_layer(self, inputs):
-        mini = inputs[0]
+        output = inputs[0]
         for input in inputs[1:]:
-            mini = np.minimum(mini, input)
-        return self.activation_function.compute(mini)
+            output +=input 
+        return self.activation_function.compute(output/(len(inputs)))
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,22 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
 
-#Multiplication of several tensors
-class Multiply(Broadcast.Broadcast):
+#Subtraction of several tensors
+class Subtract(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Multiply'
-        self.specific_operator = '*'
+        self.name = 'Subtract'
+        self.specific_operator = ' - '
     
     def forward_path_layer(self, inputs):
         output = inputs[0]
         for input in inputs[1:]:
-            output *= input
+            output -= input
         return self.activation_function.compute(output)
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,22 +14,22 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Broadcast_layers.Broadcast as Broadcast
+from acetone_nnet import Broadcast
 
-#Subtraction of several tensors
-class Subtract(Broadcast.Broadcast):
+#Division of several tensors
+class Divide(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Subtract'
-        self.specific_operator = ' - '
+        self.name = 'Divide'
+        self.specific_operator = '/'
     
     def forward_path_layer(self, inputs):
         output = inputs[0]
         for input in inputs[1:]:
-            output -= input
-        return self.activation_function.compute(output)
+            output /= input
+        return self.activation_function.compute(output)
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+import acetone_nnet as Layer
 import numpy as np
 import pystache
 
 #Concatenate two tensor alongside a given axis
 #attribut: axis alongside of which the concatenation will be done
 #input: a list of tensor to concatenate
 #output: the concatenated tensor 
-class Concatenate(Layer.Layer):
+class Concatenate(Layer):
     def __init__(self, idx, size, axis, input_shapes,output_shape,activation_function):
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shapes = input_shapes
         self.name = 'Concatenate'
         self.axis = axis
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
+
 import numpy as np
 from abc import abstractmethod
 
-class Conv2D(Layer.Layer):
+class Conv2D(Layer):
     
     def __init__(self, idx, conv_algorithm, size, padding, strides, kernel_h, kernel_w, dilation_rate, nb_filters, input_shape, output_shape, weights, biases, activation_function):
         super().__init__()
         self.conv_algorithm = conv_algorithm
         self.idx = idx
         self.size = size
         self.name = 'Conv2D'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Conv_layers.Conv2D as Conv2D
+from acetone_nnet import Conv2D
+
 import pystache
 
-class Conv2D_6loops(Conv2D.Conv2D):
+class Conv2D_6loops(Conv2D):
     """Implements Conv2D using the six-loops algorithm (direc conv)"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
    
     def generate_inference_code_layer(self):
         output_str = self.previous_layer[0].output_str
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Conv_layers.Conv2D as Conv2D
+from acetone_nnet import Conv2D
+
 import numpy as np
 import pystache
 
-class Conv2D_gemm(Conv2D.Conv2D):
+class Conv2D_gemm(Conv2D):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.patches_height = self.input_channels * self.kernel_h * self.kernel_w
         self.patches_width = self.output_height * self.output_width
         self.patches_size = self.patches_height * self.patches_width
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,20 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Conv_layers.Conv2D_gemm as Conv2D_gemm
+from acetone_nnet import Conv2D_gemm
+
 import numpy as np
 import pystache
 
-class Conv2D_indirect_gemm(Conv2D_gemm.Conv2D_gemm):
+class Conv2D_indirect_gemm(Conv2D_gemm):
     """Implements Conv2D using indirect im2col (or im2row) and GeMM"""
    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def create_ppatches(self):
         if (self.pad_right or self.pad_left or self.pad_bottom or self.pad_top):
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Conv_layers.Conv2D_gemm as Conv2D_gemm
+from acetone_nnet import Conv2D_gemm
+
 import numpy as np
 import pystache
 
-class Conv2D_std_gemm(Conv2D_gemm.Conv2D_gemm):
+class Conv2D_std_gemm(Conv2D_gemm):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.patches_height = self.input_channels * self.kernel_h * self.kernel_w
         self.patches_width = self.output_height * self.output_width
         self.patches_size = self.patches_height * self.patches_width
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+import acetone_nnet as Layer
 import numpy as np
 import pystache
 
-class Dense(Layer.Layer):
+class Dense(Layer):
 
     def __init__(self, idx, size, weights, biases, activation_function):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Dense'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,24 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+import acetone_nnet as Layer
 import numpy as np
 import pystache
 
 
 #Do the dotproduct of two tensors
 #atribut: the axis alongside of which the dot product will be done. if type(axis) == int, same axis for the two tensor. can be tuples of axis (element i of axis represent axis of tensor i)
 #input: two tensor
 #output: the resultant tensor 
-class Dot(Layer.Layer):
+class Dot(Layer):
     def __init__(self, idx, size, axis, input_shapes,output_shape,activation_function):
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shapes = input_shapes
         self.name = 'Dot'
         #we seek a tuple of axis
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+import acetone_nnet as Layer
 import pystache
 import numpy as np
 
-class Flatten(Layer.Layer):
+class Flatten(Layer):
 
     def __init__(self, idx, size, input_shape, data_format):
        
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
 import numpy as np
 import pystache
 
 #extract a list of subtensor from a given tensor
 #attribut: axis alongside of which the submatrix will be extracted (if the desired submatrix must have the height, width or channels of the parent tensor)
 #input: a tensor
 #output: a list of tensor
-class Gather(Layer.Layer):
+class Gather(Layer):
     
     def __init__(self, idx, size, axis,  indices, input_shape, output_shape,activation_function):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Gather'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
 import numpy as np
 import pystache
 
 #The layer which compute the general matrix multiplication
 #input: weight tesnsor W and bias tensor B, input tensor T. The tensor must be of 2D
 #data: alpha and beta constante used in the operation, transpo un tuple saying if the tensor T or W must be transposed before the operation
 #output: The result of the operation """alpha*T*W + beta*B"""
-class Gemm(Layer.Layer):
+class Gemm(Layer):
     def __init__(self, idx, size, alpha, beta, transA, transB, weights, bias, input_shape, output_shape,activation_function):
         super().__init__() 
         self.name = 'Gemm'
         self.idx = idx
         self.size = size
         
         self.alpha = [alpha]
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Input.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
 import pystache
 
-class InputLayer(Layer.Layer):
+class InputLayer(Layer):
 
     def __init__(self, idx, size, input_shape, data_format):
        
         super().__init__()
         self.idx = idx
         self.size = size
         self.input_shape = input_shape
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
 import numpy as np
 import pystache
 
-class MatMul(Layer.Layer):
+class MatMul(Layer):
 
     def __init__(self, idx, size, input_shape, weights, side, activation_function):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'MatMul'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pad_layers.Pad as Pad
+from acetone_nnet import Pad
+
 import pystache
 
 #The Constant mode of the Pad layers
 #Use a constant to fill paddings
-class Constant_Pad(Pad.Pad):
+class Constant_Pad(Pad):
     
     def __init__(self, idx, size, pads, constant_value, axes,input_shape,activation_function):
         super().__init__(idx, size, pads, constant_value, axes,input_shape,activation_function)
         self.mode = 'constant'
     
     def generate_inference_code_layer(self):
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pad_layers.Pad as Pad
+from acetone_nnet import Pad
+
 import pystache
 
 #The Edge mode of the Pad layers
 #Pads with the edge values of array.
-class Edge_pad(Pad.Pad):
+class Edge_pad(Pad):
     
     def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
         super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
         self.mode = 'edge'
 
 
     def write_padding(self):
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,26 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
+
 import numpy as np
 from abc import abstractmethod
 
 #The Pad Layers
 #Pad alongside each dimmensions
 #attribut: the mode of padding required
 #input: a tensor to be padded, the desired pads, the value of teh constant if mode == constant
 #output:the resized tensor
 ######################### cf https://onnx.ai/onnx/operators/onnx__Pad.html for the doc
-class Pad(Layer.Layer):
+class Pad(Layer):
     
     def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
         super().__init__()
         self.idx = idx
         self.size = size
         self.pads = pads
         self.constant_value = constant_value
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pad_layers.Pad as Pad
+from acetone_nnet import Pad
+
 import pystache
 
 #The Reflect mode of the Pad layers
 #Pads with the reflection of the vector mirrored on the first and last values of the vector along each axis.
-class Reflect_pad(Pad.Pad):
+class Reflect_pad(Pad):
     
     def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
         super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
         self.mode = 'reflect'
     
     def write_padding(self):
         mustach_hash = {}
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,22 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pad_layers.Pad as Pad
+from acetone_nnet import Pad
+
 import pystache
 
 #The Wrap mode of the Pad layers
 #Pads with the wrap of the vector along the axis. 
 #The first values are used to pad the end and the end values are used to pad the beginning.
-class Wrap_pad(Pad.Pad):
+class Wrap_pad(Pad):
     
     def __init__(self, idx, size, mode, pads, constant_value, axes, input_shape):
         super().__init__(idx, size, mode, pads, constant_value, axes, input_shape)
         self.mode = 'wrap'
     
     def write_padding(self):
         mustach_hash = {}
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pooling_layers.Pooling2D as Pooling2D
+from acetone_nnet import Pooling2D
+
 import numpy as np
 
-class AveragePooling2D(Pooling2D.Pooling2D):
+class AveragePooling2D(Pooling2D):
     def __init__(self, **kwds):
         super().__init__(**kwds)
         
         self.name = 'AveragePooling2D'
         self.pooling_function = np.mean
         self.local_var = 'sum'
         self.local_var_2 = 'count'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Pooling_layers.Pooling2D as Pooling2D
+from acetone_nnet import Pooling2D
+
 import numpy as np
 
-class MaxPooling2D(Pooling2D.Pooling2D):
+class MaxPooling2D(Pooling2D):
     def __init__(self, **kwds):
         super().__init__(**kwds)
         
         self.name = 'MaxPooling2D'
         self.pooling_function = np.amax
         self.local_var = 'max'
         self.output_var = self.local_var
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
+
 import numpy as np
 import pystache
 from abc import abstractmethod
 
-class Pooling2D(Layer.Layer):
+class Pooling2D(Layer):
     def __init__(self, idx, size, padding, strides, pool_size, input_shape, output_shape, activation_function,**kwargs):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.padding = padding
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,27 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
+
 from abc import abstractmethod
 
 #The resize Layers
 #Only Height and Width are resized
 #attribut: a lot of stuff
 #input: a tensor to be resized, the desired size or a scale to multiply the size by, the region of interest
 #output:the resized tensor
 ##############  https://onnx.ai/onnx/operators/onnx__Resize.html for more informations
 #The strategie is always to go throught the elements, find the coordinate in the original tensor 
 # and apply a transformation to the value in the original tensor to find the value to enter in the new tensor
-class Resize(Layer.Layer):
+class Resize(Layer):
     
     def __init__(self,idx,size,input_shape,activation_function,axes=[],coordinate_transformation_mode='half_pixel',exclude_outside=0,
                  keep_aspect_ratio_policy='stretch',boolean_resize = None,target_size=[],roi=[],extrapolation_value=0, 
                  nearest_mode = 'round_prefer_floor',cubic_coeff_a = -0.75):
         super().__init__()
         self.idx = idx
         if(type(nearest_mode) == bytes):
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Resize_layers.Resize as Resize
+from acetone_nnet import Resize
+
 import numpy as np
 import tensorflow as tf
 import pystache
 
 #The Cubic mode of the Resize layers
 #Use a (bi)cubic interpolation to find the new value
-class ResizeCubic(Resize.Resize):
+class ResizeCubic(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'cubic'
         self.template_dict = {'1D':'./templates/layers/Resize/template_ResizeCubic1D.c.tpl',
                               '2D':'./templates/layers/Resize/template_ResizeCubic2D.c.tpl'}
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Resize_layers.Resize as Resize
+from acetone_nnet import Resize
+
 import numpy as np
 import tensorflow as tf
 import pystache
 
 #The mode Linear of the Resize layers
 #The value in the output tensor are found thanks to a (bi)linear interpolation
-class ResizeLinear(Resize.Resize):
+class ResizeLinear(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode = 'linear'
         self.template_dict = {'1D':'./templates/layers/Resize/template_ResizeLinear1D.c.tpl',
                               '2D':'./templates/layers/Resize/template_ResizeLinear2D.c.tpl'}
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,23 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.layers.Resize_layers.Resize as Resize
+from acetone_nnet import Resize
+
 import tensorflow as tf
 import numpy as np
 import pystache
 
 #The mode Nearest of the Resize layers.
 #The value in the new tensor is found by applying an rounding operation
-class ResizeNearest(Resize.Resize):
+class ResizeNearest(Resize):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.mode='nearest'
         self.nearest_mode_mapping = {"round_prefer_floor":self.round_prefer_floor,
                                      "round_prefer_ceil":self.round_prefer_ceil,
                                      "floor":self.floor,
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,19 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-import code_generator.Layer as Layer
+from acetone_nnet import Layer
 import numpy as np
 import pystache
 
-class Softmax(Layer.Layer):
+class Softmax(Layer):
 
     def __init__(self, idx, size):
         
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = 'Softmax'
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/code_generator/neural_network.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,35 +20,21 @@
 
 import os
 import numpy as np
 from pathlib import Path
 from abc import ABC
 import pystache
 
-from format_importer.parser import parser
-
-from code_generator.layers.Dense import Dense
-from code_generator.layers.Dot import Dot
-from code_generator.layers.Softmax import Softmax
-from code_generator.layers.Gather import Gather
-from code_generator.layers.Gemm import Gemm
-from code_generator.layers.MatMul import MatMul
-from code_generator.layers.Pad_layers.Pad import Pad
-from code_generator.layers.Resize_layers.ResizeLinear import ResizeLinear
-from code_generator.layers.Resize_layers.ResizeNearest import ResizeNearest
-from code_generator.layers.Resize_layers.ResizeCubic import ResizeCubic
-from code_generator.layers.Conv_layers.Conv2D_6loops import Conv2D_6loops
-from code_generator.layers.Conv_layers.Conv2D_indirect_gemm import Conv2D_indirect_gemm
-from code_generator.layers.Conv_layers.Conv2D_std_gemm import Conv2D_std_gemm
-from code_generator.layers.Conv_layers.Conv2D import Conv2D
-from code_generator.layers.Concatenate import Concatenate
-from code_generator.layers.Pooling_layers.Pooling2D import Pooling2D
-from code_generator.layers.Pooling_layers.AveragePooling2D import AveragePooling2D
-from code_generator.layers.Pooling_layers.MaxPooling2D import MaxPooling2D
-from code_generator.layers.Broadcast_layers.Broadcast import Broadcast
+from acetone_nnet import(
+    Dense, Dot, Softmax, Gather, Gemm, MatMul, Pad, Concatenate, Broadcast,
+    ResizeCubic, ResizeLinear, ResizeNearest,
+    Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm, 
+    Pooling2D, MaxPooling2D, AveragePooling2D,
+    parser
+)
 
 class CodeGenerator(ABC):
 
     def __init__(self, file, test_dataset_file = None, function_name = 'inference', nb_tests = None, conv_algorithm = 'conv_gemm_optim', normalize = False,**kwargs):
 
         self.file = file
         self.test_dataset_file = test_dataset_file
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,24 @@
  ******************************************************************************
 """
 
 import json
 from itertools import islice
 import numpy as np
 
-import graph.graph_interpretor as graph
-
-from code_generator.layers.Pooling_layers import AveragePooling2D, MaxPooling2D
-from code_generator.layers.Conv_layers import Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm 
-from code_generator.layers.Pad_layers import ConstantPad
-from code_generator.layers.Broadcast_layers import Add, Multiply, Subtract, Divide, Maximum, Minimum, Average
-from code_generator.layers.Resize_layers import ResizeCubic, ResizeLinear, ResizeNearest
-from code_generator.layers import  Concatenate, Input, Dense, Softmax,  Dot, Flatten
-from code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH
+from acetone_nnet import (
+    AveragePooling2D, MaxPooling2D,
+    Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
+    Constant_Pad,
+    Add, Multiply, Subtract, Maximum, Minimum, Average,
+    ResizeCubic, ResizeLinear, ResizeNearest,
+    Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten,
+    Linear, ReLu, Sigmoid, TanH,
+    tri_topo
+)
 
 def create_actv_function_obj(activation_str):
 
         if activation_str == 'sigmoid':
             return Sigmoid()
         elif activation_str == 'relu':
             return ReLu()
@@ -44,32 +45,32 @@
             return Linear()
         elif activation_str == 'softmax':
             return Softmax()
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
-        return Conv2D_6loops.Conv2D_6loops(**kwargs)
+        return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
-        return Conv2D_std_gemm.Conv2D_std_gemm(**kwargs)   
+        return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
-        return Conv2D_indirect_gemm.Conv2D_indirect_gemm(**kwargs)
+        return Conv2D_indirect_gemm(**kwargs)
 
 def create_resize_obj(mode, **kwargs):
 
     if mode == 'bicubic':
-        return ResizeCubic.ResizeCubic(**kwargs)
+        return ResizeCubic(**kwargs)
     
     elif mode == 'bilinear':
-        return ResizeLinear.ResizeLinear(**kwargs)
+        return ResizeLinear(**kwargs)
     
     else:
-        return ResizeNearest.ResizeNearest(**kwargs)
+        return ResizeNearest(**kwargs)
 
 def load_json(file_to_parse, conv_algorithm):
         
         file = open(file_to_parse, 'r')
         model = json.load(file)
         data_format = model['config']['data_format'] 
 
@@ -85,15 +86,15 @@
 
         elif data_type == 'int':
             data_type = 'long int'
             data_type_py = np.int32
 
         layers = []
 
-        l_temp = Input.InputLayer(0, model['config']['layers'][0]['config']['size'], model['config']['layers'][0]['config']['input_shape'], data_format)
+        l_temp = InputLayer(0, model['config']['layers'][0]['config']['size'], model['config']['layers'][0]['config']['input_shape'], data_format)
 
         layers.append(l_temp)
 
         nb_softmax_layers = 0
 
         for idx, layer in list(islice(enumerate(model['config']['layers']), 1, None)):
             add_softmax_layer = False
@@ -109,15 +110,15 @@
                 weights = np.array(data_type_py(layer['weights']))
                 if(len(weights.shape) < 3):
                     for i in range(3-len(weights.shape)): 
                         weights = np.expand_dims(weights, axis=-1)
                 weights = np.moveaxis(weights, 2, 0)
                 if(len(weights.shape) < 4):
                     weights = np.expand_dims(weights, axis=0)
-                current_layer = Dense.Dense(idx=idx,
+                current_layer = Dense(idx=idx,
                                       size=layer['config']['units'],
                                       weights=np.array(data_type_py(layer['weights'])),
                                       biases=data_type_py(layer['biases']),
                                       activation_function=create_actv_function_obj(layer['config']['activation']))
             
             elif layer['class_name'] == 'Conv2D':
                 weights = np.array(data_type_py(layer['weights']))
@@ -140,97 +141,97 @@
                                                   input_shape = layer['config']['input_shape'],
                                                   output_shape = layer['config']['output_shape'],
                                                   weights = weights, 
                                                   biases = data_type_py(layer['biases']),
                                                   activation_function = create_actv_function_obj(layer['config']['activation']))
             
             elif layer['class_name'] == 'AveragePooling2D':
-                current_layer = AveragePooling2D.AveragePooling2D(idx = idx,
+                current_layer = AveragePooling2D(idx = idx,
                                                  size = layer['config']['size'],
                                                  padding = layer['config']['padding'],
                                                  strides = layer['config']['strides'][0],
                                                  pool_size = layer['config']['pool_size'][0],
                                                  input_shape = layer['config']['input_shape'],
                                                  output_shape = layer['config']['output_shape'],
                                                  activation_function = Linear())
             
             elif layer['class_name'] == 'MaxPooling2D':
-                current_layer = MaxPooling2D.MaxPooling2D(idx = idx,
+                current_layer = MaxPooling2D(idx = idx,
                                              size = layer['config']['size'],
                                              padding = layer['config']['padding'],
                                              strides = layer['config']['strides'][0],
                                              pool_size = layer['config']['pool_size'][0],
                                              input_shape = layer['config']['input_shape'],
                                              output_shape = layer['config']['output_shape'],
                                              activation_function = Linear())
             
             elif layer['class_name'] == 'Flatten':
-                current_layer = Flatten.Flatten(idx = idx,
+                current_layer = Flatten(idx = idx,
                                                 size = layer['config']['size'],
                                                 input_shape = layer['config']['input_shape'],
                                                 data_format = data_format)
             
             elif layer['class_name'] == 'Add':
-                current_layer = Add.Add(idx = layer['config']['idx'],
+                current_layer = Add(idx = layer['config']['idx'],
                                     size = layer['config']['size'],
                                     input_shapes = layer['config']['input_shape'],
                                     output_shape = layer['config']['output_shape'],
                                     activation_function = Linear())
 
             elif layer['class_name'] == 'Multiply':
-                current_layer = Multiply.Multiply(idx = layer['config']['idx'],
+                current_layer = Multiply(idx = layer['config']['idx'],
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Subtract':
-                current_layer = Subtract.Subtract(idx = layer['config']['idx'], 
+                current_layer = Subtract(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Concatenate':
                 axis = layer['config']['axis']
                 if(data_format == 'channels_last'):
                     if(axis == 3):
                         axis = 1
                     else:
                         axis = axis + 1
-                current_layer = Concatenate.Concatenate(idx = layer['config']['idx'], 
+                current_layer = Concatenate(idx = layer['config']['idx'], 
                                             size = layer['config']['size'],
                                             axis = axis, 
                                             input_shapes = layer['config']['input_shape'], 
                                             output_shape = layer['config']['output_shape'],
                                             activation_function=Linear())
             
             elif layer['class_name'] == 'Maximum':
-                current_layer = Maximum.Maximum(idx = layer['config']['idx'], 
+                current_layer = Maximum(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
                 
             elif layer['class_name'] == 'Minimum':
-                current_layer = Minimum.Minimum(idx = layer['config']['idx'], 
+                current_layer = Minimum(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Average':
-                current_layer = Average.Average(idx = layer['config']['idx'], 
+                current_layer = Average(idx = layer['config']['idx'], 
                                          size = layer['config']['size'], 
                                          input_shapes = layer['config']['input_shape'], 
                                          output_shape = layer['config']['output_shape'],
                                          activation_function= Linear())
             
             elif layer['class_name'] == 'Dot':
-                current_layer = Dot.Dot(idx = layer['config']['idx'],
+                current_layer = Dot(idx = layer['config']['idx'],
                                     size = layer['config']['size'],
                                     axis= layer['config']['axes'],
                                     input_shapes = layer['config']['input_shape'], 
                                     output_shape = layer['config']['output_shape'],
                                     activation_function = Linear())
             
             elif layer['class_name'] == 'UpSampling2D': # Need to make sure that the 'size' attribut of the Layer is renamed
@@ -257,15 +258,15 @@
             elif layer['class_name'] == 'ZeroPadding1D':
                 pads = layer['config']['padding']
                 if(type(pads) == int):
                     pads = [pads for i in range(8)]
                 else:
                     pads = [0,0,pads[0],0,0,0,pads[1],0]
 
-                current_layer = ConstantPad.Constant_Pad(idx = layer['config']['idx'],
+                current_layer = Constant_Pad(idx = layer['config']['idx'],
                                              size = layer['config']['size'],
                                              pads = pads,
                                              constant_value = 0,
                                              axes = [],
                                              input_shape = layer['config']['input_shape'],
                                              activation_function = Linear())
 
@@ -278,15 +279,15 @@
                         pad_top, pad_bottom = pads[0], pads[0]
                         pad_left, pad_right = pads[1], pads[1]
                     else:
                         pad_top, pad_bottom = pads[0][0], pads[0][1]
                         pad_left, pad_right = pads[1][0], pads[1][1]
                     pads = [0,0,pad_top,pad_left,0,0,pad_bottom,pad_right]
 
-                current_layer = ConstantPad.Constant_Pad(idx = layer['config']['idx'],
+                current_layer = Constant_Pad(idx = layer['config']['idx'],
                                              size = layer['config']['size'],
                                              pads = pads,
                                              constant_value = 0,
                                              axes = [],
                                              input_shape = layer['config']['input_shape'],
                                              activation_function = Linear())
             
@@ -318,12 +319,12 @@
                 nb_softmax_layers += 1
                 current_layer = Softmax.Softmax(idx+1, l_temp.size)
                 l_temp.next_layer.append(current_layer)
                 current_layer.previous_layer.append(l_temp)
                 l_temp = current_layer
                 layers.append(current_layer)
 
-        layers, listRoad, maxRoad, dict_cst = graph.tri_topo(layers)
+        layers, listRoad, maxRoad, dict_cst = tri_topo(layers)
         layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
         print("Finished model initialization.")    
         return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,19 +18,17 @@
  ******************************************************************************
 """
 
 
 import tensorflow as tf
 import numpy as np
 
-import format_importer.NNET_importer.nnet_normalize as nnet_normalize
+import acetone_nnet.format_importer.NNET_importer.nnet_normalize as nnet_normalize
 
-from code_generator.layers.Dense import Dense
-from code_generator.layers.Input import InputLayer
-from code_generator.activation_functions import Linear, ReLu
+from acetone_nnet import Dense, InputLayer, Linear, ReLu
 
 tf.keras.backend.set_floatx('float32')
 
 
 def load_nnet(file_to_parse, normalize):
     """
     Reads nnet networks from ACAS project and to pull it in .h5 format
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 import onnx
-from format_importer.ONNX_importer.create_layer import *
-from graph.graph_interpretor import tri_topo
+from acetone_nnet.format_importer.ONNX_importer.create_layer import *
+from acetone_nnet import tri_topo
 
 def load_onnx(file_to_parse, conv_algorithm):
     #Loading the model and adding value_info if it's not already in it 
     model = onnx.load(file_to_parse)
     if (not model.graph.value_info):
         model = onnx.shape_inference.infer_shapes(model)
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/__init__.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from format_importer.parser import parser
+from acetone_nnet.format_importer.parser import parser
 
-from format_importer.ONNX_importer.parser_ONNX import load_onnx
-from format_importer.JSON_importer.parser_JSON import load_json
-from format_importer.NNET_importer.parser_NNET import load_nnet
-from format_importer.H5_importer.JSON_from_keras_model import JSON_from_keras_model
+from acetone_nnet.format_importer.ONNX_importer.parser_ONNX import load_onnx
+from acetone_nnet.format_importer.JSON_importer.parser_JSON import load_json
+from acetone_nnet.format_importer.NNET_importer.parser_NNET import load_nnet
+from acetone_nnet.format_importer.H5_importer.JSON_from_keras_model import JSON_from_keras_model
 
 __all__ = list("parser", "load_json", "load_nnet", "load_onnx", "JSON_from_keras_model")
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/format_importer/parser.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/format_importer/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,15 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import keras
-from format_importer.JSON_importer.parser_JSON import load_json
-from format_importer.ONNX_importer.parser_ONNX import load_onnx
-from format_importer.NNET_importer.parser_NNET import load_nnet
-from format_importer.H5_importer.JSON_from_keras_model import JSON_from_keras_model
+from acetone_nnet import load_json, load_nnet, load_onnx, JSON_from_keras_model
 
 def get_path(file, new_type):
     new_path = ""
     list_path = file.split("/")
     file_name = list_path[-1].split(".")[0]
 
     for dir in list_path[:-1]:
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/graph/__init__.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/graph/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,10 +14,10 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from graph.graph_interpretor import tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
+from acetone_nnet.graph.graph_interpretor import tri_topo, updatepath, setNewpath, to_save, parcours_prof_topo
 
 __all__ = list("tri_topo", "updatepath", "setNewpath","to_save", "parcours_prof_topo")
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet/graph/graph_interpretor.py` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/PKG-INFO` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.0.1.2.1
+Version: 0.0.1.2.3
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone-nnet-0.0.1.2.1/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone-nnet-0.0.1.2.3/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

