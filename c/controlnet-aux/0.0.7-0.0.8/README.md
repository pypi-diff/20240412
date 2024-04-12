# Comparing `tmp/controlnet_aux-0.0.7.tar.gz` & `tmp/controlnet_aux-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.7.tar", last modified: Tue Sep  5 12:21:31 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.8.tar", last modified: Fri Apr 12 08:22:28 2024, max compression
```

## Comparing `controlnet_aux-0.0.7.tar` & `controlnet_aux-0.0.8.tar`

### file list

```diff
@@ -1,201 +1,203 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/LICENSE.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5639 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4688 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8759 2023-09-05 12:19:03.000000 controlnet_aux-0.0.7/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.142105 controlnet_aux-0.0.7/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.146105 controlnet_aux-0.0.7/src/controlnet_aux/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      583 2023-09-05 12:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.146105 controlnet_aux-0.0.7/src/controlnet_aux/canny/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1353 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/dwpose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2996 2023-09-05 12:07:25.000000 controlnet_aux-0.0.7/src/controlnet_aux/dwpose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10660 2023-09-05 12:10:42.000000 controlnet_aux-0.0.7/src/controlnet_aux/dwpose/util.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4576 2023-09-05 12:07:58.000000 controlnet_aux-0.0.7/src/controlnet_aux/dwpose/wholebody.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/hed/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5732 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4371 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6241 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/Resnet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8547 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/Resnext_torch.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    22911 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/depthmap.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1122 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2029 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/net_tools.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16887 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/network_auxi.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3095 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10714 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1660 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    28960 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/networks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7404 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      136 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9364 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/base_options.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1062 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/test_options.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/util/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       83 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/util/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3110 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/util/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/lineart/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5805 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/lineart/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/lineart_anime/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8204 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/lineart_anime/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/mediapipe_face/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1944 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/mediapipe_face/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7118 2023-05-26 09:41:40.000000 controlnet_aux-0.0.7/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.150105 controlnet_aux-0.0.7/src/controlnet_aux/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3581 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2816 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24189 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3647 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.154105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.158105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.158105 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.158105 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9477 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12428 2023-09-05 12:08:59.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13491 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/face.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3210 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13742 2023-09-05 12:09:57.000000 controlnet_aux-0.0.7/src/controlnet_aux/open_pose/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.158105 controlnet_aux-0.0.7/src/controlnet_aux/pidi/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3131 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/pidi/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    21813 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/pidi/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6259 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/processor.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.158105 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3364 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/automatic_mask_generator.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4695 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/build_sam.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      419 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/image_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7283 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/sam.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24707 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    11633 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/predictor.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/amg.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/onnx.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/shuffle/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3330 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/shuffle/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5434 2023-06-27 19:48:39.000000 controlnet_aux-0.0.7/src/controlnet_aux/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2913 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.162105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/model_io.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16264 2023-09-05 12:00:44.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/config.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.166105 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/easydict/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-09-05 12:21:31.146105 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5639 2023-09-05 12:21:31.000000 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8960 2023-09-05 12:21:31.000000 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-09-05 12:21:31.000000 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-09-05 12:21:31.000000 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-09-05 12:21:31.000000 controlnet_aux-0.0.7/src/controlnet_aux.egg-info/top_level.txt
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.908465 controlnet_aux-0.0.8/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    11357 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/LICENSE.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6095 2024-04-12 08:22:28.908296 controlnet_aux-0.0.8/PKG-INFO
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4848 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/README.md
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       38 2024-04-12 08:22:28.908511 controlnet_aux-0.0.8/setup.cfg
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8785 2024-04-12 08:20:48.000000 controlnet_aux-0.0.8/setup.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.883269 controlnet_aux-0.0.8/src/
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.888376 controlnet_aux-0.0.8/src/controlnet_aux/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      582 2024-04-12 08:21:02.000000 controlnet_aux-0.0.8/src/controlnet_aux/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889364 controlnet_aux-0.0.8/src/controlnet_aux/canny/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1353 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/canny/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889858 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2996 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10660 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/util.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4576 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/dwpose/wholebody.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.890039 controlnet_aux-0.0.8/src/controlnet_aux/hed/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5791 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/hed/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.890207 controlnet_aux-0.0.8/src/controlnet_aux/leres/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4465 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.891222 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6241 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnet.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8547 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnext_torch.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    22911 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/depthmap.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1122 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2029 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/net_tools.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16887 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/network_auxi.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.891379 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892070 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3095 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10714 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1660 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    28960 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/networks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7404 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892468 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9364 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/base_options.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1062 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/test_options.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892769 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       83 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3110 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.892905 controlnet_aux-0.0.8/src/controlnet_aux/lineart/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5899 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/lineart/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893035 controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8263 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893285 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1944 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7118 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.893661 controlnet_aux-0.0.8/src/controlnet_aux/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3640 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5276 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/api.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.894660 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9242 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/blocks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3154 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/transforms.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    14625 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4582 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/midas/utils.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.894932 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2875 2024-04-12 08:17:04.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895314 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9678 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9180 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    24189 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/mlsd/utils.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895434 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3706 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.895802 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      597 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2980 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/baseline.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.896317 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    10480 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.897665 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2428 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5993 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.898884 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      206 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.899440 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4170 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2690 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2294 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4549 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3350 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12093 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    26514 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    59925 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2833 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15009 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      707 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       22 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2730 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5821 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2932 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      843 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4905 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1737 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1297 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6632 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1060 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5703 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900193 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     9606 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12428 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/body.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13491 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/face.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3210 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/hand.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8743 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13742 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/open_pose/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900441 controlnet_aux-0.0.8/src/controlnet_aux/pidi/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3190 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/pidi/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    21813 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/pidi/model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6259 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/processor.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.900950 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3364 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15148 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4695 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/build_sam.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902023 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      419 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1479 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/common.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    14420 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6615 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8594 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7283 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/sam.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    24707 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8397 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    11633 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/predictor.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902530 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      197 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12712 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/amg.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5812 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/onnx.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3972 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/transforms.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902661 controlnet_aux-0.0.8/src/controlnet_aux/shuffle/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3330 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/shuffle/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5434 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/util.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902786 controlnet_aux-0.0.8/src/controlnet_aux/zoe/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2972 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.902907 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903387 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903650 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    15248 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.903866 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    13757 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.904876 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.905962 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6909 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3436 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1045 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      333 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      931 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1576 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7284 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6899 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      367 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12792 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6099 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2709 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     5207 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8552 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7869 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     2390 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     7362 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.906572 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1153 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8693 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4838 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6733 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4163 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3438 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907033 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1270 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1587 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      556 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    12630 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907400 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1276 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1968 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16264 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907821 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     1154 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      624 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-r--r--   0 sayakpaul   (501) staff       (20)    16310 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.907963 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     3426 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.889199 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     6095 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/PKG-INFO
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     8989 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)        1 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)      136 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/requires.txt
+-rw-r--r--   0 sayakpaul   (501) staff       (20)       15 2024-04-12 08:22:28.000000 controlnet_aux-0.0.8/src/controlnet_aux.egg-info/top_level.txt
+drwxr-xr-x   0 sayakpaul   (501) staff       (20)        0 2024-04-12 08:22:28.908070 controlnet_aux-0.0.8/tests/
+-rw-r--r--   0 sayakpaul   (501) staff       (20)     4855 2024-04-12 08:17:05.000000 controlnet_aux-0.0.8/tests/test_controlnet_aux.py
```

### Comparing `controlnet_aux-0.0.7/LICENSE.txt` & `controlnet_aux-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/PKG-INFO` & `controlnet_aux-0.0.8/src/controlnet_aux.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 Metadata-Version: 2.1
-Name: controlnet_aux
-Version: 0.0.7
+Name: controlnet-aux
+Version: 0.0.8
 Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: torch
+Requires-Dist: importlib_metadata
+Requires-Dist: huggingface_hub
+Requires-Dist: scipy
+Requires-Dist: opencv-python-headless
+Requires-Dist: filelock
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: einops
+Requires-Dist: torchvision
+Requires-Dist: timm<=0.6.7
+Requires-Dist: scikit-image
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.6
+pip install controlnet-aux==0.0.7
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
@@ -132,8 +143,10 @@
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
 ```
 
+### Image resolution
 
+In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.7/README.md` & `controlnet_aux-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.6
+pip install controlnet-aux==0.0.7
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
@@ -106,7 +106,11 @@
 processed_image_leres = leres(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
 ```
+
+### Image resolution
+
+In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.7/setup.py` & `controlnet_aux-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,21 +78,21 @@
 # 2. once modified, run: `make deps_table_update` to update src/diffusers/dependency_versions_table.py
 _deps = [
     "Pillow",
     "torch",
     "numpy",
     "filelock",
     "importlib_metadata",
-    "opencv-python",
+    "opencv-python-headless",
     "scipy",
     "huggingface_hub",
     "einops",
-    "timm",
+    "timm<=0.6.7",
     "torchvision",
-    "scikit-image"
+    "scikit-image",
 ]
 
 # this is a lookup table with items like:
 #
 # tokenizers: "huggingface-hub==0.8.0"
 # packaging: "packaging"
 #
@@ -164,27 +164,27 @@
 extras = {}
 
 install_requires = [
     deps["torch"],
     deps["importlib_metadata"],
     deps["huggingface_hub"],
     deps["scipy"],
-    deps["opencv-python"],
+    deps["opencv-python-headless"],
     deps["filelock"],
     deps["numpy"],
     deps["Pillow"],
     deps["einops"],
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.7",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.8",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Auxillary models for controlnet",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 from .hed import HEDdetector
 from .leres import LeresDetector
 from .lineart import LineartDetector
 from .lineart_anime import LineartAnimeDetector
 from .midas import MidasDetector
 from .mlsd import MLSDdetector
@@ -11,8 +11,8 @@
 from .pidi import PidiNetDetector
 from .zoe import ZoeDetector
 
 from .canny import CannyDetector
 from .mediapipe_face import MediapipeFaceDetector
 from .segment_anything import SamDetector
 from .shuffle import ContentShuffleDetector
-from .dwpose import DWposeDetector
+from .dwpose import DWposeDetector
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/canny/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/dwpose/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/dwpose/util.py` & `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/dwpose/wholebody.py` & `controlnet_aux-0.0.8/src/controlnet_aux/dwpose/wholebody.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/hed/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,21 +57,21 @@
         return projection1, projection2, projection3, projection4, projection5
 
 class HEDdetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "ControlNetHED.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         netNetwork = ControlNetHED_Apache2()
         netNetwork.load_state_dict(torch.load(model_path, map_location='cpu'))
         netNetwork.float().eval()
 
         return cls(netNetwork)
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 
 class LeresDetector:
     def __init__(self, model, pix2pixmodel):
         self.model = model
         self.pix2pixmodel = pix2pixmodel
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, pix2pix_filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, pix2pix_filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "res101.pth"
         pix2pix_filename = pix2pix_filename or "latest_net_G.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
             
         checkpoint = torch.load(model_path, map_location=torch.device('cpu'))
 
         model = RelDepthModel(backbone='resnext101')
         model.load_state_dict(strip_prefix_if_present(checkpoint['depth_model'], "module."), strict=True)
         del checkpoint
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, pix2pix_filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, pix2pix_filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, pix2pix_filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         opt = TestOptions().parse()
         if not torch.cuda.is_available():
             opt.gpu_ids = []  # cpu mode
         pix2pixmodel = Pix2Pix4DepthModel(opt)
         pix2pixmodel.save_dir = os.path.dirname(model_path)
         pix2pixmodel.load_networks('latest')
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/Resnet.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/Resnext_torch.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/Resnext_torch.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/depthmap.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/depthmap.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/multi_depth_model_woauxi.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/net_tools.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/net_tools.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/leres/network_auxi.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/leres/network_auxi.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/base_model.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/base_model_hg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/networks.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/networks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/models/pix2pix4depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/base_options.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/base_options.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/options/test_options.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/options/test_options.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/leres/pix2pix/util/util.py` & `controlnet_aux-0.0.8/src/controlnet_aux/leres/pix2pix/util/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/lineart/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,24 +93,24 @@
 
 class LineartDetector:
     def __init__(self, model, coarse_model):
         self.model = model
         self.model_coarse = coarse_model
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, coarse_filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, coarse_filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "sk_model.pth"
         coarse_filename = coarse_filename or "sk_model2.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
             coarse_model_path = os.path.join(pretrained_model_or_path, coarse_filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
-            coarse_model_path = hf_hub_download(pretrained_model_or_path, coarse_filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
+            coarse_model_path = hf_hub_download(pretrained_model_or_path, coarse_filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         model = Generator(3, 1, 3)
         model.load_state_dict(torch.load(model_path, map_location=torch.device('cpu')))
         model.eval()
 
         coarse_model = Generator(3, 1, 3)
         coarse_model.load_state_dict(torch.load(coarse_model_path, map_location=torch.device('cpu')))
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/lineart_anime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,21 +114,21 @@
 
 
 class LineartAnimeDetector:
     def __init__(self, model):
         self.model = model
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "netG.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         norm_layer = functools.partial(nn.InstanceNorm2d, affine=False, track_running_stats=False)
         net = UnetGenerator(3, 1, 8, 64, norm_layer=norm_layer, use_dropout=False)
         ckpt = torch.load(model_path)
         for key in list(ckpt.keys()):
             if 'module.' in key:
                 ckpt[key.replace('module.', '')] = ckpt[key]
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mediapipe_face/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 
 class MidasDetector:
     def __init__(self, model):
         self.model = model
         
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, model_type="dpt_hybrid", filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, model_type="dpt_hybrid", filename=None, cache_dir=None, local_files_only=False):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
         else:
             filename = filename or "dpt_hybrid-midas-501f0c75.pt"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         model = MiDaSInference(model_type=model_type, model_path=model_path)
 
         return cls(model)
         
 
     def to(self, device):
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.8/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 class MLSDdetector:
     def __init__(self, model):
         self.model = model
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None, local_files_only=False):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
         else:
             filename = filename or "mlsd_large_512_fp32.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
         model.eval()
 
         return cls(model)
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.8/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 class NormalBaeDetector:
     def __init__(self, model):
         self.model = model
         self.norm = transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "scannet.pt"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         args = types.SimpleNamespace()
         args.mode = 'client'
         args.architecture = 'BN'
         args.pretrained = 'scannet'
         args.sampling_ratio = 0.4
         args.importance_ratio = 0.7
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux-0.0.8/src/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     """
     def __init__(self, body_estimation, hand_estimation=None, face_estimation=None):
         self.body_estimation = body_estimation
         self.hand_estimation = hand_estimation
         self.face_estimation = face_estimation
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, hand_filename=None, face_filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, hand_filename=None, face_filename=None, cache_dir=None, local_files_only=False):
 
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/body_pose_model.pth"
             hand_filename = hand_filename or "annotator/ckpts/hand_pose_model.pth"
             face_filename = face_filename or "facenet.pth"
 
             face_pretrained_model_or_path = "lllyasviel/Annotators"
@@ -96,17 +96,17 @@
             face_pretrained_model_or_path = pretrained_model_or_path
 
         if os.path.isdir(pretrained_model_or_path):
             body_model_path = os.path.join(pretrained_model_or_path, filename)
             hand_model_path = os.path.join(pretrained_model_or_path, hand_filename)
             face_model_path = os.path.join(face_pretrained_model_or_path, face_filename)
         else:
-            body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
-            hand_model_path = hf_hub_download(pretrained_model_or_path, hand_filename, cache_dir=cache_dir)
-            face_model_path = hf_hub_download(face_pretrained_model_or_path, face_filename, cache_dir=cache_dir)
+            body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
+            hand_model_path = hf_hub_download(pretrained_model_or_path, hand_filename, cache_dir=cache_dir, local_files_only=local_files_only)
+            face_model_path = hf_hub_download(face_pretrained_model_or_path, face_filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         body_estimation = Body(body_model_path)
         hand_estimation = Hand(hand_model_path)
         face_estimation = Face(face_model_path)
 
         return cls(body_estimation, hand_estimation, face_estimation)
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/face.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/open_pose/util.py` & `controlnet_aux-0.0.8/src/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/pidi/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 
 
 class PidiNetDetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "table5_pidinet.pth"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
 
         netNetwork = pidinet()
         netNetwork.load_state_dict({k.replace('module.', ''): v for k, v in torch.load(model_path)['state_dict'].items()})
         netNetwork.eval()
 
         return cls(netNetwork)
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/pidi/model.py` & `controlnet_aux-0.0.8/src/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/processor.py` & `controlnet_aux-0.0.8/src/controlnet_aux/processor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/automatic_mask_generator.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/build_sam.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/common.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/image_encoder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/mask_decoder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/sam.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/tiny_vit_sam.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/modeling/transformer.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/predictor.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/amg.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/onnx.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/segment_anything/utils/transforms.py` & `controlnet_aux-0.0.8/src/controlnet_aux/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/util.py` & `controlnet_aux-0.0.8/src/controlnet_aux/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 
 class ZoeDetector:
     def __init__(self, model):
         self.model = model
 
     @classmethod
-    def from_pretrained(cls, pretrained_model_or_path, model_type="zoedepth", filename=None, cache_dir=None):
+    def from_pretrained(cls, pretrained_model_or_path, model_type="zoedepth", filename=None, cache_dir=None, local_files_only=False):
         filename = filename or "ZoeD_M12_N.pt"
 
         if os.path.isdir(pretrained_model_or_path):
             model_path = os.path.join(pretrained_model_or_path, filename)
         else:
-            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir, local_files_only=local_files_only)
             
         conf = get_config(model_type, "infer")
         model_cls = ZoeDepth if model_type == "zoedepth" else ZoeDepthNK
         model = model_cls.build_from_config(conf)
         model.load_state_dict(torch.load(model_path, map_location=torch.device('cpu'))['model'])
         model.eval()
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/builder.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/depth_model.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/depth_model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/model_io.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/model_io.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/config.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py` & `controlnet_aux-0.0.8/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux.egg-info/PKG-INFO` & `controlnet_aux-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 Metadata-Version: 2.1
-Name: controlnet-aux
-Version: 0.0.7
+Name: controlnet_aux
+Version: 0.0.8
 Summary: Auxillary models for controlnet
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: torch
+Requires-Dist: importlib_metadata
+Requires-Dist: huggingface_hub
+Requires-Dist: scipy
+Requires-Dist: opencv-python-headless
+Requires-Dist: filelock
+Requires-Dist: numpy
+Requires-Dist: Pillow
+Requires-Dist: einops
+Requires-Dist: torchvision
+Requires-Dist: timm<=0.6.7
+Requires-Dist: scikit-image
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
 All credit & copyright goes to https://github.com/lllyasviel .
 
 ## Install
 
 ```
-pip install controlnet-aux==0.0.6
+pip install controlnet-aux==0.0.7
 ```
 
 To support DWPose which is dependent on MMDetection, MMCV and MMPose
 ```
 pip install -U openmim
 mim install mmengine
 mim install "mmcv>=2.0.1"
@@ -132,8 +143,10 @@
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
 processed_image_mediapipe_face = face_detector(img)
 processed_image_dwpose = dwpose(img)
 ```
 
+### Image resolution
 
+In order to maintain the image aspect ratio, `detect_resolution`, `image_resolution` and images sizes need to be using multiple of `64`.
```

### Comparing `controlnet_aux-0.0.7/src/controlnet_aux.egg-info/SOURCES.txt` & `controlnet_aux-0.0.8/src/controlnet_aux.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -148,8 +148,9 @@
 src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
 src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
 src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
 src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
 src/controlnet_aux/zoe/zoedepth/utils/__init__.py
 src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
 src/controlnet_aux/zoe/zoedepth/utils/config.py
-src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+tests/test_controlnet_aux.py
```

