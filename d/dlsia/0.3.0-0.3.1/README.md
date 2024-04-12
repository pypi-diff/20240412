# Comparing `tmp/dlsia-0.3.0.tar.gz` & `tmp/dlsia-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlsia-0.3.0.tar", last modified: Tue Aug  8 19:57:38 2023, max compression
+gzip compressed data, was "dist/dlsia-0.3.1.tar", last modified: Fri Apr 12 03:11:43 2024, max compression
```

## Comparing `dlsia-0.3.0.tar` & `dlsia-0.3.1.tar`

### file list

```diff
@@ -1,96 +1,104 @@
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      137 2023-08-08 19:46:38.000000 dlsia-0.3.0/AUTHORS.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2964 2023-08-08 19:46:38.000000 dlsia-0.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      269 2023-08-08 19:46:38.000000 dlsia-0.3.0/HISTORY.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1554 2023-08-08 19:46:38.000000 dlsia-0.3.0/LICENSE
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      305 2023-08-08 19:46:38.000000 dlsia-0.3.0/MANIFEST.in
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8725 2023-08-08 19:57:38.818181 dlsia-0.3.0/PKG-INFO
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8108 2023-08-08 19:46:38.000000 dlsia-0.3.0/README.md
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.810181 dlsia-0.3.0/dlsia/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      166 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/__init__.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/__init__.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/conformalize/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/conformalize/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5950 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/conformalize/conformalize_segmentation.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      695 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/corcoef.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    17502 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/custom_losses.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16714 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/helpers.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1219 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/inference_scripts.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/networks/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      241 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2761 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/aggnet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5586 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/baggins.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3670 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/graph_utils.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16443 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msae.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7937 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msd_graph_tools.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9229 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdae.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    19515 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdnet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14317 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/msdnet2.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5130 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/scale_up_down.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    21540 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sms1d.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    23139 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sms3d.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36366 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/smsnet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    25596 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/sparsenet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2812 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/squashnet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    26668 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/tunet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    41863 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/tunet3plus.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4466 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/networks/unet.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    31241 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/train_scripts.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/core/utils/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3503 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/agg_utils.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3121 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/feature_extraction.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2750 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/latent_space_viewer.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2794 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/randomized_data_loader.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3201 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/core/utils/simple_instance_segmenter.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/test_data/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/__init__.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/test_data/two_d/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    12261 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/build_test_data.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2128 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/diffusion_model.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14578 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7409 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d_time.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9088 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/random_shapes.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7450 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/torch_hdf5_loader.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      143 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/test_data/two_d/tst.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/tutorials/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/tutorials/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      615 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/tutorials/copy_all.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia/viz_tools/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/__init__.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5874 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/draw_sparse_network.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4149 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/plot_autoencoder_image_classification.py
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7218 2023-08-08 19:46:38.000000 dlsia-0.3.0/dlsia/viz_tools/plots.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/dlsia.egg-info/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8725 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/PKG-INFO
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2313 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/SOURCES.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/dependency_links.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-08-08 19:47:52.000000 dlsia-0.3.0/dlsia.egg-info/not-zip-safe
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      445 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/requires.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        6 2023-08-08 19:57:38.000000 dlsia-0.3.0/dlsia.egg-info/top_level.txt
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/docs/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      606 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/Makefile
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2672 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/conf.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.814181 dlsia-0.3.0/docs/images/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36602 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/Autoencoder_fig.png
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    48762 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/MSDNet_fig.png
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    42098 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/RMSNet_fig.png
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    62953 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/UNet_fig.png
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    47397 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/images/dlsia.png
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3417 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/index.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      772 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/make.bat
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/docs/source/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      431 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.conformalize.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2013 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.networks.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1095 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.core.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      252 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      256 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.test_data.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1652 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.test_data.two_d.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      357 2023-08-08 19:46:38.000000 dlsia-0.3.0/docs/source/dlsia.viz_tools.rst
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      444 2023-08-08 19:46:38.000000 dlsia-0.3.0/requirements.txt
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      388 2023-08-08 19:57:38.818181 dlsia-0.3.0/setup.cfg
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1637 2023-08-08 19:57:24.000000 dlsia-0.3.0/setup.py
-drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2023-08-08 19:57:38.818181 dlsia-0.3.0/tests/
--rw-rw-r--   0 pzwart    (1000) pzwart    (1000)       40 2023-08-08 19:46:38.000000 dlsia-0.3.0/tests/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      137 2023-01-26 19:45:35.000000 dlsia-0.3.1/AUTHORS.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2964 2023-01-26 19:56:56.000000 dlsia-0.3.1/CONTRIBUTING.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      368 2024-04-12 03:08:23.000000 dlsia-0.3.1/HISTORY.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1554 2023-08-08 04:08:59.000000 dlsia-0.3.1/LICENSE
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      305 2023-01-26 19:45:35.000000 dlsia-0.3.1/MANIFEST.in
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    10636 2024-04-12 03:11:43.399469 dlsia-0.3.1/PKG-INFO
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8108 2023-08-08 04:10:08.000000 dlsia-0.3.1/README.md
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.395469 dlsia-0.3.1/dlsia/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      147 2024-04-12 03:08:56.000000 dlsia-0.3.1/dlsia/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.395469 dlsia-0.3.1/dlsia/core/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/core/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.395469 dlsia-0.3.1/dlsia/core/conformalize/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/core/conformalize/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5950 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/core/conformalize/conformalize_segmentation.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      695 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/core/corcoef.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    20330 2024-01-04 02:50:02.000000 dlsia-0.3.1/dlsia/core/custom_losses.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16714 2023-04-28 20:41:48.000000 dlsia-0.3.1/dlsia/core/helpers.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1219 2023-01-26 19:48:04.000000 dlsia-0.3.1/dlsia/core/inference_scripts.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/core/networks/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      241 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/core/networks/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2761 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/core/networks/aggnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5578 2024-04-12 03:06:11.000000 dlsia-0.3.1/dlsia/core/networks/baggins.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     8545 2024-04-11 05:49:14.000000 dlsia-0.3.1/dlsia/core/networks/construct_sms_ensemble.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3670 2023-01-26 19:48:05.000000 dlsia-0.3.1/dlsia/core/networks/graph_utils.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3590 2023-10-11 23:24:13.000000 dlsia-0.3.1/dlsia/core/networks/grey2color.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    16443 2023-05-09 18:07:26.000000 dlsia-0.3.1/dlsia/core/networks/msae.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7937 2023-01-26 19:56:56.000000 dlsia-0.3.1/dlsia/core/networks/msd_graph_tools.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9229 2023-01-26 20:45:26.000000 dlsia-0.3.1/dlsia/core/networks/msdae.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    19515 2023-01-27 18:50:50.000000 dlsia-0.3.1/dlsia/core/networks/msdnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14317 2023-04-28 20:41:48.000000 dlsia-0.3.1/dlsia/core/networks/msdnet2.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    12437 2023-09-05 20:58:51.000000 dlsia-0.3.1/dlsia/core/networks/orthonet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2203 2023-05-15 22:45:12.000000 dlsia-0.3.1/dlsia/core/networks/random_autoencoder.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5130 2023-01-26 19:48:05.000000 dlsia-0.3.1/dlsia/core/networks/scale_up_down.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    21540 2023-07-02 03:41:02.000000 dlsia-0.3.1/dlsia/core/networks/sms1d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    23026 2023-12-21 17:37:30.000000 dlsia-0.3.1/dlsia/core/networks/sms3d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36366 2023-03-20 22:05:58.000000 dlsia-0.3.1/dlsia/core/networks/smsnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    25596 2023-05-15 23:02:30.000000 dlsia-0.3.1/dlsia/core/networks/sparsenet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3232 2023-10-11 21:56:53.000000 dlsia-0.3.1/dlsia/core/networks/squashnet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    27074 2023-09-07 23:08:50.000000 dlsia-0.3.1/dlsia/core/networks/tunet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    41863 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/core/networks/tunet3plus.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4466 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/core/networks/unet.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    44255 2024-04-11 05:49:14.000000 dlsia-0.3.1/dlsia/core/train_scripts.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/core/utils/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/core/utils/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3503 2023-01-26 20:44:47.000000 dlsia-0.3.1/dlsia/core/utils/agg_utils.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5888 2024-03-21 06:06:54.000000 dlsia-0.3.1/dlsia/core/utils/blur.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2760 2024-03-21 23:02:57.000000 dlsia-0.3.1/dlsia/core/utils/downsample.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3466 2023-10-09 19:26:22.000000 dlsia-0.3.1/dlsia/core/utils/feature_extraction.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2750 2023-01-26 19:48:04.000000 dlsia-0.3.1/dlsia/core/utils/latent_space_viewer.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2794 2023-06-07 20:49:33.000000 dlsia-0.3.1/dlsia/core/utils/randomized_data_loader.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3201 2023-01-26 19:48:04.000000 dlsia-0.3.1/dlsia/core/utils/simple_instance_segmenter.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      735 2024-03-22 19:56:02.000000 dlsia-0.3.1/dlsia/core/utils/sparse_tools.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/test_data/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/test_data/__init__.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/test_data/two_d/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/test_data/two_d/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    12261 2023-01-26 20:53:30.000000 dlsia-0.3.1/dlsia/test_data/two_d/build_test_data.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2128 2023-01-26 19:48:04.000000 dlsia-0.3.1/dlsia/test_data/two_d/diffusion_model.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    14578 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/test_data/two_d/noisy_gauss_2d.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7409 2023-01-26 20:53:30.000000 dlsia-0.3.1/dlsia/test_data/two_d/noisy_gauss_2d_time.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     9088 2023-01-26 19:48:04.000000 dlsia-0.3.1/dlsia/test_data/two_d/random_shapes.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7450 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/test_data/two_d/torch_hdf5_loader.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      143 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/test_data/two_d/tst.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/tutorials/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/tutorials/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      615 2023-01-26 20:24:44.000000 dlsia-0.3.1/dlsia/tutorials/copy_all.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/dlsia/viz_tools/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        0 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/viz_tools/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     5874 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/viz_tools/draw_sparse_network.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     4149 2023-01-26 19:45:35.000000 dlsia-0.3.1/dlsia/viz_tools/plot_autoencoder_image_classification.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     7218 2023-02-15 23:17:39.000000 dlsia-0.3.1/dlsia/viz_tools/plots.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.395469 dlsia-0.3.1/dlsia.egg-info/
+-rw-r--r--   0 pzwart    (1000) pzwart    (1000)    10636 2024-04-12 03:11:43.000000 dlsia-0.3.1/dlsia.egg-info/PKG-INFO
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2575 2024-04-12 03:11:43.000000 dlsia-0.3.1/dlsia.egg-info/SOURCES.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2024-04-12 03:11:43.000000 dlsia-0.3.1/dlsia.egg-info/dependency_links.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        1 2023-12-28 02:08:35.000000 dlsia-0.3.1/dlsia.egg-info/not-zip-safe
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      504 2024-04-12 03:11:43.000000 dlsia-0.3.1/dlsia.egg-info/requires.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)        6 2024-04-12 03:11:43.000000 dlsia-0.3.1/dlsia.egg-info/top_level.txt
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/docs/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      606 2023-01-31 22:14:16.000000 dlsia-0.3.1/docs/Makefile
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2672 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/conf.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/docs/images/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    36602 2023-01-26 19:45:35.000000 dlsia-0.3.1/docs/images/Autoencoder_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    48762 2023-01-26 19:45:35.000000 dlsia-0.3.1/docs/images/MSDNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    42098 2023-01-26 19:45:35.000000 dlsia-0.3.1/docs/images/RMSNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    62953 2023-01-26 19:45:35.000000 dlsia-0.3.1/docs/images/UNet_fig.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)    47397 2023-01-26 22:56:36.000000 dlsia-0.3.1/docs/images/dlsia.png
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     3417 2023-08-07 18:08:49.000000 dlsia-0.3.1/docs/index.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      772 2023-01-26 19:45:35.000000 dlsia-0.3.1/docs/make.bat
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/docs/source/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      431 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.core.conformalize.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     2013 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.core.networks.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1095 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.core.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      252 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      256 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.test_data.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1652 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.test_data.two_d.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      357 2023-02-15 23:17:39.000000 dlsia-0.3.1/docs/source/dlsia.viz_tools.rst
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      504 2024-04-11 05:49:14.000000 dlsia-0.3.1/requirements.txt
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)      388 2024-04-12 03:11:43.399469 dlsia-0.3.1/setup.cfg
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1637 2024-04-12 03:08:03.000000 dlsia-0.3.1/setup.py
+drwxrwxr-x   0 pzwart    (1000) pzwart    (1000)        0 2024-04-12 03:11:43.399469 dlsia-0.3.1/tests/
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)       40 2023-01-26 19:45:35.000000 dlsia-0.3.1/tests/__init__.py
+-rw-rw-r--   0 pzwart    (1000) pzwart    (1000)     1324 2024-04-07 03:19:53.000000 dlsia-0.3.1/tests/test_blur.py
```

### Comparing `dlsia-0.3.0/CONTRIBUTING.rst` & `dlsia-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/LICENSE` & `dlsia-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/PKG-INFO` & `dlsia-0.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: dlsia
-Version: 0.3.0
-Summary: Deep Learning for Scientif Image Analysis
-Home-page: https://github.com/phzwart/dlsia/
-Author: Petrus H. Zwart, Eric J. Roberts
-Author-email: PHZwart@lbl.gov, EJroberts@lbl.gov
-License: BSD License
-Keywords: dlsia
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ![logo](docs/images/dlsia.png 'the logo')
 
 
 # Welcome to dlsia's documentation!
 
 <a style="text-decoration:none !important;" href="https://dlsia.readthedocs.io/en/latest/" alt="website"><img src="https://img.shields.io/readthedocs/dlsia" /></a>
 <a style="text-decoration:none !important;" href="https://opensource.org/licenses/MIT" alt="License"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
```

### Comparing `dlsia-0.3.0/dlsia/core/conformalize/conformalize_segmentation.py` & `dlsia-0.3.1/dlsia/core/conformalize/conformalize_segmentation.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/corcoef.py` & `dlsia-0.3.1/dlsia/core/corcoef.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/custom_losses.py` & `dlsia-0.3.1/dlsia/core/custom_losses.py`

 * *Files 11% similar despite different names*

```diff
@@ -422,14 +422,82 @@
         Returns:
             torch.Tensor: The combined loss with base loss and TV norm regularization.
         """
         base_loss = self.base_loss_fn(input, target)
         tv_loss = self.tv_norm(input)
         return base_loss + tv_loss
 
+class CombinedLossWithTVNorm3D(nn.Module):
+    """
+    A custom loss function combining a base loss and total variation (TV) norm regularization.
+
+    Args:
+        base_loss_fn (torch.nn.Module): The base loss function for the primary task.
+        tv_weights (torch.Tensor): Weights to control the impact of the TV regularization on each channel.
+
+    Attributes:
+        tv_weights (torch.Tensor): Weights to control the impact of the TV regularization on each channel.
+        base_loss_fn (torch.nn.Module): The base loss function for the primary task.
+
+    Methods:
+        tv_norm(input_tensor):
+            Calculates the total variation norm regularization for the input tensor.
+
+        forward(input, target):
+            Computes the combined loss with the base loss and TV norm regularization.
+
+    Example:
+        base_loss_fn = torch.nn.MSELoss()
+        tv_weights = torch.tensor([0.1, 0.2, 0.3])  # Example TV weights for 3 channels
+        combined_loss = CombinedLossWithTVNorm(base_loss_fn, tv_weights)
+    """
+
+    def __init__(self, base_loss_fn, tv_weights):
+        super(CombinedLossWithTVNorm3D, self).__init__()
+        self.tv_weights = tv_weights
+        self.base_loss_fn = base_loss_fn
+
+    def tv_norm(self, input_tensor):
+        """
+        Calculate the total variation norm regularization for the input tensor.
+
+        Args:
+            input_tensor (torch.Tensor): The input tensor to compute the TV norm for.
+
+        Returns:
+            torch.Tensor: The total variation norm regularization.
+        """
+        batch_size, channels, z, y, x = input_tensor.shape
+        sm = nn.Softmax(dim=1)
+        sm_input_tensor = sm(input_tensor)
+        diff_i = torch.abs(sm_input_tensor[:, :, 1:, :, :] - sm_input_tensor[:, :, :-1, :, :])
+        diff_j = torch.abs(sm_input_tensor[:, :, :, 1:, :] - sm_input_tensor[:, :, :, :-1, :])
+        diff_k = torch.abs(sm_input_tensor[:, :, :, :, 1:] - sm_input_tensor[:, :, :, :, :-1])
+
+        # Applying the weights for each channel
+        diff_i = (diff_i * self.tv_weights.view(1, channels, 1, 1, 1)).sum()
+        diff_j = (diff_j * self.tv_weights.view(1, channels, 1, 1, 1)).sum()
+        diff_k = (diff_k * self.tv_weights.view(1, channels, 1, 1, 1)).sum()
+
+        return (diff_i + diff_j + diff_k) / (batch_size * z * y * x)
+
+    def forward(self, input, target):
+        """
+        Compute the combined loss with the base loss and TV norm regularization.
+
+        Args:
+            input (torch.Tensor): The model's predicted output.
+            target (torch.Tensor): The ground truth target.
+
+        Returns:
+            torch.Tensor: The combined loss with base loss and TV norm regularization.
+        """
+        base_loss = self.base_loss_fn(input, target)
+        tv_loss = self.tv_norm(input)
+        return base_loss + tv_loss
 
 def tst():
     """
     Defines and test several Mixed Scale Dense Networks consisting of 2D
     convolutions, provides a printout of the network, and checks to make
     sure tensors pass through the network
     """
```

### Comparing `dlsia-0.3.0/dlsia/core/helpers.py` & `dlsia-0.3.1/dlsia/core/helpers.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/inference_scripts.py` & `dlsia-0.3.1/dlsia/core/inference_scripts.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/aggnet.py` & `dlsia-0.3.1/dlsia/core/networks/aggnet.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/baggins.py` & `dlsia-0.3.1/dlsia/core/networks/baggins.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             if self.model_type == "classification":
                 norma = torch.sum(mean, dim=1).unsqueeze(1)
                 mean = mean / norma
                 std = std / norma
             if not return_std:
                 return mean
             return mean, std / np.sqrt(N)
-        
+
 
 class autoencoder_labeling_model_baggin(nn.Module):
     """
     Bagg a number of models
     """
 
     def __init__(self, models, returns_normalized=False):
```

### Comparing `dlsia-0.3.0/dlsia/core/networks/graph_utils.py` & `dlsia-0.3.1/dlsia/core/networks/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/msae.py` & `dlsia-0.3.1/dlsia/core/networks/msae.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/msd_graph_tools.py` & `dlsia-0.3.1/dlsia/core/networks/msd_graph_tools.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/msdae.py` & `dlsia-0.3.1/dlsia/core/networks/msdae.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/msdnet.py` & `dlsia-0.3.1/dlsia/core/networks/msdnet.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/msdnet2.py` & `dlsia-0.3.1/dlsia/core/networks/msdnet2.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/scale_up_down.py` & `dlsia-0.3.1/dlsia/core/networks/scale_up_down.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/sms1d.py` & `dlsia-0.3.1/dlsia/core/networks/sms1d.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/sms3d.py` & `dlsia-0.3.1/dlsia/core/networks/sms3d.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,14 @@
 from collections import OrderedDict
 from dlsia.core.networks import msd_graph_tools
 from dlsia.core.networks import smsnet
 from dlsia.core.networks import graph_utils
 from dlsia.core.networks import scale_up_down
 from torch.nn import Conv3d
 
-
-# from SMSNet import sort_and_rename, buildSMSnodechannels
-# from SMSNet import edges_source_sink_list, buildSMSdilations
-
-
 def Conv3DReLU(in_channels,
                out_channels,
                conv_kernel_size,
                dilation_size,
                stride,
                output_padding,
                padding_mode="reflect"):
@@ -137,14 +132,30 @@
     :param out_channels: not used
     :return: the identity operator
     """
     function = nn.Identity()
     return function
 
 
+def aggregate(node_layer_accumulator, this_node, data):
+        """
+        Aggregate the data in place
+        :param node_layer_accumulator: a lit of lists
+        :param this_node: where we place stuff
+        :param data: the data to add
+        """
+        if node_layer_accumulator[this_node] is None:
+            node_layer_accumulator[this_node] = data
+        else:
+            node_layer_accumulator[this_node] = \
+                torch.cat([node_layer_accumulator[this_node], data], 1)
+        return node_layer_accumulator
+
+
+
 class SMSNet3D(nn.Module):
     """
     A Sparse Mixed Scale Network, 3D
     """
 
     def __init__(self,
                  in_channels,
@@ -193,44 +204,19 @@
         self.edge_list, \
         self.source, \
         self.hidden, \
         self.sink = smsnet.edges_source_sink_list(self.network_graph)
 
         self.node_layer_accumulator = OrderedDict()
         self.action_list = []
-        for node in self.channel_count:
-            self.node_layer_accumulator[node] = []
 
         self.build_network()
 
         self.return_before_last_layer_ = False
 
-    def aggregate(self, this_node, data):
-        """
-        Aggregate the data in place
-
-        :param this_node:
-        :param data:
-        """
-
-        if self.node_layer_accumulator[this_node] is None:
-            self.node_layer_accumulator[this_node] = data
-        else:
-            self.node_layer_accumulator[this_node] = \
-                torch.cat([self.node_layer_accumulator[this_node], data], 1)
-
-    def reset(self):
-        """
-        Simple reset
-        :return: None
-        :rtype: None
-        """
-        for node in self.node_layer_accumulator:
-            self.node_layer_accumulator[node] = None
-
     def build_network(self):
         """
         Put the network and its operations together
         """
         # the first thing to do is always the first_action
         # we choose tho keep the dimensions intact (for now)
         # self.add_module('on_input', self.first_action(self.in_channels,
@@ -290,16 +276,14 @@
                 what_now = ('Edge_%s_%s' % (from_here, to_there), from_here, to_there)
                 self.action_list.append(what_now)
 
         last_node = next(reversed(self.channel_count))
         last_action_in = self.channel_count[last_node]
         last_action_out = self.out_channels
 
-        self.node_layer_accumulator[last_node] = None
-
         self.action_list.append(('Last_Action', last_node, None))
 
         if self.last_action is None:
             self.add_module('Last_Action', nn.Identity())
         else:
             self.add_module('Last_Action', self.last_action(last_action_in,
                                                             last_action_out,
@@ -309,28 +293,33 @@
     def forward(self, x):
         """
         The forward method
 
         :param x: The data
         :return: the resulting tensor after it has been passed through the network
         """
-        self.reset()
-        self.aggregate(0, x)
+
+        node_layer_accumulator = OrderedDict()
+        for node in self.channel_count:
+            node_layer_accumulator[node] = None
+        last_node = next(reversed(self.channel_count))
+        node_layer_accumulator[last_node] = None
+
+        aggregate(node_layer_accumulator, 0, x)
 
         for action_pair in self.action_list[:-1]:
             action, from_here, to_there = action_pair
-            data_in = self.node_layer_accumulator[from_here]
+            data_in = node_layer_accumulator[from_here]
             data_out = self._modules[action](data_in)
-            self.aggregate(to_there, data_out)
+            aggregate(node_layer_accumulator, to_there, data_out)
 
         action, from_here, to_there = self.action_list[-1]
-
-        data_in = self.node_layer_accumulator[from_here]
-
+        data_in = node_layer_accumulator[from_here]
         data_out = self._modules[action](data_in)
+
         if self.return_before_last_layer_:
             return data_in, data_out
         return data_out
 
     def topology_dict(self):
         """
         Get all parameters needed to build this network
```

### Comparing `dlsia-0.3.0/dlsia/core/networks/smsnet.py` & `dlsia-0.3.1/dlsia/core/networks/smsnet.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/sparsenet.py` & `dlsia-0.3.1/dlsia/core/networks/sparsenet.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/squashnet.py` & `dlsia-0.3.1/dlsia/core/networks/squashnet.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,7 +82,20 @@
     def save_network_parameters(self, name=None):
         network_dict = OrderedDict()
         network_dict["topo_dict"] = self.topology_dict()
         network_dict["state_dict"] = self.state_dict()
         if name is None:
             return network_dict
         torch.save(network_dict, name)
+
+def Squashnet_from_file_SMS(filename):
+    network_dict = torch.load(filename, map_location=torch.device('cpu'))
+    SMSObj = smsnet.SMSNet(**network_dict["topo_dict_spatial"])
+    SMSObj.load_state_dict(network_dict["state_dict_spatial"])
+
+    FCNet = FCNetwork(**network_dict["topo_dict_squash"])
+    FCNet.load_state_dict(network_dict["state_dict_squash"])
+
+    result = SquashNet(FCNet, SMSObj)
+    return result
+
+
```

### Comparing `dlsia-0.3.0/dlsia/core/networks/tunet.py` & `dlsia-0.3.1/dlsia/core/networks/tunet.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,15 @@
                  growth_rate=2,
                  hidden_rate=1,
                  conv_kernel=nn.Conv2d,
                  kernel_down=nn.MaxPool2d,
                  kernel_up=nn.ConvTranspose2d,
                  normalization=nn.BatchNorm2d,
                  activation=nn.ReLU(),
+                 final_activation = None,
                  conv_kernel_size=3,
                  maxpool_kernel_size=2,
                  dilation=1
                  ):
         """
         Construct a tuneable UNet
 
@@ -237,14 +238,16 @@
                           nn.ConvTranspose3d
         :param normalization: PyTorch normalization class applied to each
                               layer. Passed as class without parentheses since
                               we need a different instance per layer.
                               ex) normalization=nn.BatchNorm2d
         :param activation: torch.nn class instance or list of torch.nn class
                            instances
+        :param final_activation: torch.nn class instance or list of torch.nn class
+                           instances
         :param conv_kernel_size: The size of the convolutional kernel we use
         :param maxpool_kernel_size: The size of the max pooling/transposed
                                     convolutional kernel we use in
                                     encoder/decoder paths. Default is 2.
         :param stride: The stride we want to use. Controls contraction/growth
                        rates of spatial dimensions (x and y) in encoder/decoder
                        paths. Default is 2.
@@ -280,14 +283,20 @@
             self.normalization = normalization
         else:
             self.normalization = None
         if activation is not None:
             self.activation = activation
         else:
             self.activation = None
+
+        if final_activation is not None:
+            self.final_activation = final_activation
+        else:
+            self.final_activation = None
+
         self.return_final_layer_ = False
 
         # we now need to get the sizing charts sorted
         self.sizing_chart = []
         for N in self.image_shape:
             self.sizing_chart.append(unet_sizing_chart(N=N,
                                                        depth=self.depth,
@@ -557,15 +566,16 @@
             x = self._modules[self.step_up[ii]](x)
             x = torch.cat((self.partials_encoder[ii], x), dim=1)
             x = self._modules[self.decoders[ii]](x)
 
         x = self._modules[self.step_up[0]](x)
         x = torch.cat((self.partials_encoder[0], x), dim=1)
         x_out = self._modules[self.decoders[0]](x)
-
+        if self.final_activation is not None:
+            return self.final_activation(x_out)
         return x_out
 
     def topology_dict(self):
         """
         Get all parameters needed to build this network
 
         :return: An orderdict with all parameters needed
```

### Comparing `dlsia-0.3.0/dlsia/core/networks/tunet3plus.py` & `dlsia-0.3.1/dlsia/core/networks/tunet3plus.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/networks/unet.py` & `dlsia-0.3.1/dlsia/core/networks/unet.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/train_scripts.py` & `dlsia-0.3.1/dlsia/core/train_scripts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import torch
 import torch.nn.utils
 from dlsia.core import corcoef
 from torchmetrics import F1Score
-
+import pandas as pd
+import logging
 
 def segmentation_metrics(preds, target, missing_label=-1, are_probs=True, num_classes=None):
     """
     Computes a variety of F1 scores.
     See : https://towardsdatascience.com/micro-macro-weighted-averages-of-f1-score-clearly-explained-b603420b292f
 
     Parameters
@@ -260,14 +261,349 @@
                "F1 validation micro": F1_validation_trace_micro,
                "F1 validation macro": F1_validation_trace_macro,
                "Best model index": best_index}
 
     net.load_state_dict(best_state_dict)
     return net, results
 
+## 20240320, Trainer() added by xchong ##
+class Trainer():
+    def __init__(self, net, trainloader, validationloader, NUM_EPOCHS,
+                       criterion, optimizer, device, dvclive=None,
+                       savepath=None, saveevery=None,
+                       scheduler=None, show=0,
+                       use_amp=False, clip_value=None):
+
+
+        """
+        Loop through epochs passing images to be segmented on a pixel-by-pixel
+        basis.
+
+        :param net: input network
+        :param trainloader: data loader with training data
+        :param validationloader: data loader with validation data
+        :param NUM_EPOCHS: number of epochs
+        :param criterion: target function
+        :param optimizer: optimization engine
+        :param device: the device where we calculate things
+        :param dvclive: use dvclive object to save metrics
+        :param savepath: filepath in which we save networks intermittently
+        :param saveevery: integer n for saving network every n epochs
+        :param scheduler: an optional schedular. can be None
+        :param show: print stats every n-th epoch
+        :param use_amp: use pytorch automatic mixed precision
+        :param clip_value: value for gradient clipping. Can be None.
+        :return: A network and run summary stats
+        """
+
+        self.net = net
+        self.trainloader = trainloader
+        self.validationloader = validationloader
+        self.NUM_EPOCHS = NUM_EPOCHS
+        self.criterion = criterion
+        self.optimizer = optimizer
+        self.device = device
+        self.dvclive = dvclive
+        self.savepath = savepath
+        self.saveevery = saveevery
+        self.scheduler = scheduler
+        self.show = show
+        self.use_amp = use_amp
+        self.clip_value = clip_value
+
+        self.train_loss = []
+        self.F1_train_trace_micro = []
+        self.F1_train_trace_macro = []
+
+          
+
+        # Skip validation steps if False or None loaded
+        if self.validationloader is False:
+            self.validationloader = None
+        if self.validationloader is not None:
+            self.validation_loss = []
+            self.F1_validation_trace_micro = []
+            self.F1_validation_trace_macro = []
+
+        self.best_score = 1e10
+        self.best_index = 0
+        self.best_state_dict = None
+
+        if self.savepath is not None:
+            if self.saveevery is None:
+                self.saveevery = 1
+
+        self.losses = pd.DataFrame()
+
+    # Save Loss
+    def save_loss(self,
+            epoch,
+            loss,
+            F1_micro,
+            F1_macro,
+            val_loss=None,
+            F1_val_micro=None,
+            F1_val_macro=None,
+            ):
+        if self.validationloader is not None:
+            table = pd.DataFrame(
+                {
+                    'epoch': [epoch],
+                    'loss': [loss], 
+                    'val_loss': [val_loss], 
+                    'F1_micro': [F1_micro], 
+                    'F1_macro': [F1_macro],
+                    'F1_val_micro': [F1_val_micro],
+                    'F1_val_macro': [F1_val_macro]
+                }
+            )
+        
+        else:
+            table = pd.DataFrame(
+                {
+                    'epoch': [epoch],
+                    'loss': [loss], 
+                    'F1_micro': [F1_micro], 
+                    'F1_macro': [F1_macro]
+                }
+            )
+
+        return table
+    
+    # Save metrics by dvclive
+    def save_dvc(self):
+        if self.dvclive is not None:
+            self.dvclive.log_metric("train/loss", self.train_loss[-1])
+            self.dvclive.log_metric("train/F1_micro", self.F1_train_trace_micro[-1])
+            self.dvclive.log_metric("train/F1_macro", self.F1_train_trace_macro[-1])
+            if self.validationloader is not None:
+                self.dvclive.log_metric("val/loss", self.validation_loss[-1])
+                self.dvclive.log_metric("val/F1_micro", self.F1_validation_trace_micro[-1])
+                self.dvclive.log_metric("val/F1_macro", self.F1_validation_trace_macro[-1])
+            self.dvclive.next_step()           
+        return True
+    
+    def train_one_epoch(self, epoch):
+        print(
+                f"*****  memory allocated at epoch {epoch} is {torch.cuda.memory_allocated(0)}"
+        )
+        running_train_loss = 0.0
+        running_F1_train_micro = 0.0
+        running_F1_train_macro = 0.0
+        tot_train = 0.0
+
+        if self.validationloader is not None:
+            running_validation_loss = 0.0
+            running_F1_validation_micro = 0.0
+            running_F1_validation_macro = 0.0
+            tot_val = 0.0
+        count = 0
+
+        for data in self.trainloader:
+            count += 1
+            noisy, target = data  # load noisy and target images
+            N_train = noisy.shape[0]
+            tot_train += N_train
+
+            noisy = noisy.type(torch.FloatTensor)
+            target = target.type(torch.LongTensor)
+            noisy = noisy.to(self.device)
+            target = target.to(self.device)
+
+            if self.criterion.__class__.__name__ == 'CrossEntropyLoss':
+                target = target.type(torch.LongTensor)
+                target = target.to(self.device).squeeze(1)
+
+            if self.use_amp is False:
+                # forward pass, compute loss and accuracy
+                output = self.net(noisy)
+                loss = self.criterion(output, target)
+
+                # backpropagation
+                self.optimizer.zero_grad()
+                loss.backward()
+            else:
+                scaler = torch.cuda.amp.GradScaler()
+                with torch.cuda.amp.autocast():
+                    # forward pass, compute loss and accuracy
+                    output = self.net(noisy)
+                    loss = self.criterion(output, target)
+
+                # backpropagation
+                self.optimizer.zero_grad()
+                scaler.scale(loss).backward()
+
+                # update the parameters
+                scaler.step(self.optimizer)
+                scaler.update()
+
+            # update the parameters
+            if self.clip_value is not None:
+                torch.nn.utils.clip_grad_value_(self.net.parameters(), self.clip_value)
+            self.optimizer.step()
+
+
+            tmp_micro, tmp_macro = segmentation_metrics(output, target)
+
+            running_F1_train_micro += tmp_micro.item()
+            running_F1_train_macro += tmp_macro.item()
+            running_train_loss += loss.item()
+        if self.scheduler is not None:
+            self.scheduler.step()
+
+        # compute validation step
+        if self.validationloader is not None:
+            with torch.no_grad():
+                for x, y in self.validationloader:
+                    x = x.type(torch.FloatTensor)
+                    y = y.type(torch.LongTensor)
+                    x = x.to(self.device)
+                    y = y.to(self.device)
+                    N_val = y.shape[0]
+                    tot_val += N_val
+                    if self.criterion.__class__.__name__ == 'CrossEntropyLoss':
+                        y = y.type(torch.LongTensor)
+                        y = y.to(self.device).squeeze(1)
+
+                    # forward pass, compute validation loss and accuracy
+                    if self.use_amp is False:
+                        yhat = self.net(x)
+                        val_loss = self.criterion(yhat, y)
+                    else:
+                        with torch.cuda.amp.autocast():
+                            yhat = self.net(x)
+                            val_loss = self.criterion(yhat, y)
+
+                    tmp_micro, tmp_macro = segmentation_metrics(yhat, y)
+                    running_F1_validation_micro += tmp_micro.item()
+                    running_F1_validation_macro += tmp_macro.item()
+
+                    # update running validation loss and accuracy
+                    running_validation_loss += val_loss.item()
+
+        loss = running_train_loss / len(self.trainloader)
+        F1_micro = running_F1_train_micro / len(self.trainloader)
+        F1_macro = running_F1_train_macro / len(self.trainloader)
+        self.train_loss.append(loss)
+        self.F1_train_trace_micro.append(F1_micro)
+        self.F1_train_trace_macro.append(F1_macro)
+
+        val_loss = None
+        if self.validationloader is not None:
+            val_loss = running_validation_loss / len(self.validationloader)
+            F1_val_micro = running_F1_validation_micro / len(self.validationloader)
+            F1_val_macro = running_F1_validation_macro / len(self.validationloader)
+            self.validation_loss.append(val_loss)
+            self.F1_validation_trace_micro.append(F1_val_micro)
+            self.F1_validation_trace_macro.append(F1_val_macro)
+
+        print(f'Epoch: {epoch}')
+
+        # Note: This is a very temporary solution to address the single frame mask case.
+        if self.validationloader is None:
+            F1_val_micro = None
+            F1_val_macro = None
+
+        table = self.save_loss(
+                epoch,
+                loss,
+                F1_micro,
+                F1_macro,
+                val_loss=val_loss,
+                F1_val_micro=F1_val_micro,
+                F1_val_macro=F1_val_macro,
+                )
+        
+        self.losses = pd.concat([self.losses, table])
+       
+
+        if self.show != 0:
+            learning_rates = []
+            for param_group in self.optimizer.param_groups:
+                learning_rates.append(param_group["lr"])
+            mean_learning_rate = np.mean(np.array(learning_rates))
+            if np.mod(epoch + 1, self.show) == 0:
+                if self.validationloader is not None:
+                    logging.info(
+                        f"Epoch {epoch + 1} of {self.NUM_EPOCHS} | Learning rate {mean_learning_rate:4.3e}"
+                    )
+                    logging.info(
+                        f"   Training Loss: {loss:.4e} | Validation Loss: {val_loss:.4e}"
+                    )
+                    logging.info(
+                        f"   Micro Training F1: {F1_micro:.4f} | Micro Validation F1: {F1_val_micro:.4f}"
+                    )
+                    logging.info(
+                        f"   Macro Training F1: {F1_macro:.4f} | Macro Validation F1: {F1_val_macro:.4f}"
+                    )
+                else:
+                    logging.info(
+                        f"Epoch {epoch + 1} of {self.NUM_EPOCHS} | Learning rate {mean_learning_rate:4.3e}"
+                    )
+                    logging.info(
+                        f"   Training Loss: {loss:.4e} | Micro Training F1: {F1_micro:.4f} "
+                        + "| Macro Training F1: {F1_macro:.4f}"
+                    )
+
+        if epoch == 0:
+            self.best_state_dict = self.net.state_dict()
+            if self.validationloader is not None:
+                self.best_score = val_loss
+            else:
+                self.best_score = loss
+
+        if self.validationloader is not None:
+            if val_loss < self.best_score:
+                self.best_state_dict = self.net.state_dict()
+                self.best_index = epoch
+                self.best_score = val_loss
+        else:
+            if loss < self.best_score:
+                self.best_state_dict = self.net.state_dict()
+                self.best_index = epoch
+                self.best_score = loss
+
+            if self.savepath is not None:
+                torch.save(self.best_state_dict, self.savepath + "/net_best")
+                logging.info("Best network found and saved")
+                logging.info("")
+
+        if self.savepath is not None:
+            if np.mod(epoch + 1, self.saveevery) == 0:
+                torch.save(self.net.state_dict(), self.savepath + "/net_checkpoint")
+                logging.info("Network intermittently saved")
+                logging.info("")
+
+        return True
+
+    def train_segmentation(self):
+
+        for epoch in range(self.NUM_EPOCHS):
+            self.train_one_epoch(epoch)
+            self.save_dvc()
+            
+        if self.validationloader is None:
+            self.validation_loss = []
+            self.F1_validation_trace_micro = []
+            self.F1_validation_trace_macro = []
+
+        results = {
+            "Training loss": self.train_loss,
+            "Validation loss": self.validation_loss,
+            "F1 training micro": self.F1_train_trace_micro,
+            "F1 training macro": self.F1_train_trace_macro,
+            "F1 validation micro": self.F1_validation_trace_micro,
+            "F1 validation macro": self.F1_validation_trace_macro,
+            "Best model index": self.best_index,
+        }
+
+        self.net.load_state_dict(self.best_state_dict)
+        self.losses.to_parquet(self.savepath + "/losses.parquet", engine="pyarrow")
+        return self.net, results
+## 20240320, Trainer() class added by xchong ##
 
 train_labeling = train_segmentation
 
 
 def regression_metrics(preds, target):
     """
     Compute a pearson correlation coefficient.
@@ -458,15 +794,15 @@
     return net, results
 
 
 def train_autoencoder(net, trainloader, validationloader, NUM_EPOCHS,
                       criterion, optimizer, device,
                       savepath=None, saveevery=None,
                       scheduler=None, use_amp=False,
-                      show=0, clip_value=None):
+                      show=0, clip_value=None, mask=None):
     """
     Loop through epochs passing dirty images to net.
 
     :param net: input network
     :param trainloader: data loader with training data
     :param validationloader: data loader with validation data
     :param NUM_EPOCHS: number of epochs
@@ -478,14 +814,16 @@
     :param scheduler: an optional schedular. can be None
     :param show: print stats every n-th epoch
     :param use_amp: use pytorch automatic mixed precision
     :param clip_value: value for gradient clipping. Can be None.
     :return: A network and run summary stats.
     """
 
+    if mask is None:
+        mask = 1.0
     train_loss = []
     validation_loss = []
     CC_train_trace = []
     CC_validation_trace = []
 
     best_score = 1e10
     best_index = 0
@@ -513,25 +851,25 @@
 
             noisy = noisy.type(torch.FloatTensor)
             noisy = noisy.to(device)
 
             if use_amp is False:
                 # forward pass, compute loss and accuracy
                 output = net(noisy)
-                loss = criterion(output, noisy)
+                loss = criterion(output*mask, noisy*mask)
 
                 # backpropagation
                 optimizer.zero_grad()
                 loss.backward()
             else:
                 scaler = torch.cuda.amp.GradScaler()
                 with torch.cuda.amp.autocast():
                     # forward pass, compute loss and accuracy
                     output = net(noisy)
-                    loss = criterion(output, noisy)
+                    loss = criterion(output*mask, noisy*mask)
 
                 # backpropagation
                 optimizer.zero_grad()
                 scaler.scale(loss).backward()
 
                 # update the parameters
                 scaler.step(optimizer)
@@ -559,19 +897,19 @@
 
                 N_val = x.shape[0]
                 tot_val += N_val
 
                 # forward pass, compute validation loss and accuracy
                 if use_amp is False:
                     yhat = net(x)
-                    val_loss = criterion(yhat, x)
+                    val_loss = criterion(yhat*mask, x*mask)
                 else:
                     with torch.cuda.amp.autocast():
                         yhat = net(x)
-                        val_loss = criterion(yhat, x)
+                        val_loss = criterion(yhat*mask, x*mask)
 
                 tmp = regression_metrics(yhat, x)
                 running_CC_validation_val += tmp.item()  # *N_val
 
                 # update running validation loss and accuracy
                 running_validation_loss += val_loss.item()
```

### Comparing `dlsia-0.3.0/dlsia/core/utils/agg_utils.py` & `dlsia-0.3.1/dlsia/core/utils/agg_utils.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/utils/feature_extraction.py` & `dlsia-0.3.1/dlsia/core/utils/feature_extraction.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,23 +69,31 @@
             if self.normalize is True:
                 means = torch.mean(feature, dim=(0, 1))
                 stds = torch.std(feature, dim=(0, 1))
                 feature = (feature - means) / stds
                 #feature = self.normal_cdf(feature)
             features.append(feature.unsqueeze(0))
         features = torch.cat(features, dim=0)
-        result = torch.concatenate( [images, einops.rearrange(features, "N Y X C -> N C Y X") ], dim=1 )
+        m = torch.mean(images, dim=(0,-2,-1)).unsqueeze(0).unsqueeze(-1).unsqueeze(-1)
+        s = torch.std(images, dim=(0,-2,-1)).unsqueeze(0).unsqueeze(-1).unsqueeze(-1)
+        print(m.shape, s.shape, images.shape)
+        images = (images-m)/s
+        features = einops.rearrange(features, "N Y X C -> N C Y X")
+        result = torch.concatenate( [images, features], dim=1 )
         return result
 
     def process(self, images):
         if len(images.shape)==4:
             return self._process_2d(images)
         if len(images.shape) == 5:
             return self._process_3d(images)
 
+    def __call__(self, images):
+        return self.process(images)
+
 
 if __name__ == "__main__":
     img = torch.Tensor(np.random.random((2,1,100,100)))
     obj = feature_extractor(100,100,20)
     tmp = obj.process(img)
```

### Comparing `dlsia-0.3.0/dlsia/core/utils/latent_space_viewer.py` & `dlsia-0.3.1/dlsia/core/utils/latent_space_viewer.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/utils/randomized_data_loader.py` & `dlsia-0.3.1/dlsia/core/utils/randomized_data_loader.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/core/utils/simple_instance_segmenter.py` & `dlsia-0.3.1/dlsia/core/utils/simple_instance_segmenter.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/build_test_data.py` & `dlsia-0.3.1/dlsia/test_data/two_d/build_test_data.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/diffusion_model.py` & `dlsia-0.3.1/dlsia/test_data/two_d/diffusion_model.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d.py` & `dlsia-0.3.1/dlsia/test_data/two_d/noisy_gauss_2d.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/noisy_gauss_2d_time.py` & `dlsia-0.3.1/dlsia/test_data/two_d/noisy_gauss_2d_time.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/random_shapes.py` & `dlsia-0.3.1/dlsia/test_data/two_d/random_shapes.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/test_data/two_d/torch_hdf5_loader.py` & `dlsia-0.3.1/dlsia/test_data/two_d/torch_hdf5_loader.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/tutorials/copy_all.py` & `dlsia-0.3.1/dlsia/tutorials/copy_all.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/viz_tools/draw_sparse_network.py` & `dlsia-0.3.1/dlsia/viz_tools/draw_sparse_network.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/viz_tools/plot_autoencoder_image_classification.py` & `dlsia-0.3.1/dlsia/viz_tools/plot_autoencoder_image_classification.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia/viz_tools/plots.py` & `dlsia-0.3.1/dlsia/viz_tools/plots.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/dlsia.egg-info/PKG-INFO` & `dlsia-0.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,260 +1,259 @@
 Metadata-Version: 2.1
 Name: dlsia
-Version: 0.3.0
+Version: 0.3.1
 Summary: Deep Learning for Scientif Image Analysis
 Home-page: https://github.com/phzwart/dlsia/
 Author: Petrus H. Zwart, Eric J. Roberts
 Author-email: PHZwart@lbl.gov, EJroberts@lbl.gov
 License: BSD License
+Description: ![logo](docs/images/dlsia.png 'the logo')
+        
+        
+        # Welcome to dlsia's documentation!
+        
+        <a style="text-decoration:none !important;" href="https://dlsia.readthedocs.io/en/latest/" alt="website"><img src="https://img.shields.io/readthedocs/dlsia" /></a>
+        <a style="text-decoration:none !important;" href="https://opensource.org/licenses/MIT" alt="License"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
+        <a style="text-decoration:none !important;" href="https://img.shields.io/github/commit-activity/m/phzwart/dlsia" alt="License"><img src="https://img.shields.io/github/commit-activity/m/phzwart/dlsia" /></a>
+        ![GitHub contributors](https://img.shields.io/github/contributors/phzwart/dlsia)
+        ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/phzwart/dlsia)
+        
+        dlsia (Deep Learning for Scientific Image Analysis) provides easy access to a number of segmentation and denoising
+        methods using convolution neural networks. The tools available are build for 
+        microscopy and synchrotron-imaging/scattering data in mind, but can be used 
+        elsewhere as well.
+        
+        The easiest way to start playing with the code is to install dlsia and 
+        perform denoising/segmenting using custom neural networks in our tutorial 
+        notebooks located in the dlsia/tutorials folder.
+        
+        ## Install dlsia
+        
+        We offer several methods for installation. 
+        
+        ### pip: Python package installer
+        
+        We are currently working on a stable release.
+        
+        ### From source
+        
+        dlsia may be directly downloaded and installed into your machine by 
+        cloning the public repository into an empty directory using:
+        
+        ```console
+        $ git clone https://github.com/phzwart/dlsia.git
+        ```
+        
+        Once cloned, move to the newly minted dlsia directory and install 
+        dlsia using:
+        
+        ```console
+        $ cd dlsia
+        $ pip install -e .
+        ```
+        
+        ### Further documentation & tutorial download
+        
+        For more in-depth documentation and end-to-end training workflows, please 
+        visit our 
+        [readthedocs](https://dlsia.readthedocs.io/en/latest/index.html) page 
+        for more support. To download only the tutorials in a new folder, use the 
+        following terminal input for a sparse git checkout:
+        
+        ```console
+        mkdir dlsiaTutorials
+        cd dlsiaTutorials
+        git init
+        git config core.sparseCheckout true
+        git remote add -f origin https://github.com/phzwart/dlsia.git
+        echo "dlsia/tutorials/*" > .git/info/sparse-checkout
+        git checkout main
+        ```
+        
+        ## Getting started
+        
+        We start with some basic imports - we import a network and some training 
+        scripts:
+        
+        ```python
+        from dlsia.core.networks import msdnet
+        from dlsia.core import train_scripts
+        ```
+        
+        ### Mixed-Scale dense networks (MSDNet)
+        
+        ![msdnet](docs/images/MSDNet_fig.png 'msdnet fig')
+        
+        
+        A plain 2d mixed-scale dense network is constructed as follows:
+        
+        ```python
+        from dlsia.core.networks import msdnet
+        
+        msdnet_model = msdnet.MixedScaleDenseNetwork(in_channels=1,
+                                                     out_channels=1,
+                                                     num_layers=20,
+                                                     max_dilation=10)
+        ```
+        
+        while 3d network types for volumetric images can be built passing in equivalent 
+        kernels for 3 dimensions:
+        
+        ```python
+        import torch
+        from torch import nn
+        
+        msdnet3d_model = msdnet.MixedScaleDenseNetwork(in_channels=1,
+                                                       out_channels=1,
+                                                       num_layers=20,
+                                                       max_dilation=10,
+                                                       normalization=nn.BatchNorm3d,
+                                                       convolution=nn.Conv3d)
+        ```
+        
+        Note that each instance of a convolution operator is followed by ReLU 
+        activation and batch normalization. To turn these off, simply pass in the 
+        parameters
+        
+        ```python
+        activation=None,
+        normalization=None
+        ```
+        
+        ### Sparse mixed-scale dense network (SMSNet)
+        
+        ![smsnet](docs/images/RMSNet_fig.png 'smsnet fig')
+        
+        
+        The dlsia suite also provides ways and means to build random, sparse mixed 
+        scale networks. SMSNets contain more sparsely connected nodes than a standard 
+        MSDNet and are useful to alleviate overfitting and multi-network aggregation. 
+        Controlling sparsity is possible, see full documentation for more details.
+        
+        ```python
+        from dlsia.core.networks import smsnet
+        
+        smsnet_model = smsnet.random_SMS_network(in_channels=1,
+                                                 out_channels=1,
+                                                 layers=20,
+                                                 dilation_choices=[1, 2, 4, 8],
+                                                 hidden_out_channels=[1, 2, 3])
+        ```
+        ### Tunable U-Nets
+        
+        ![tunet](docs/images/UNet_fig.png 'tunet fig')
+        
+        An alternative network choice is to construct a UNet. Classic U-Nets can easily 
+        explode in the number of parameters it requires; here we make it a bit easier 
+        to tune desired architecture-governing parameters:
+        
+        ```python
+        from dlsia.core.networks import tunet
+        
+        tunet_model = tunet.TUNet(image_shape=(64, 128),
+                                  in_channels=1,
+                                  out_channels=4,
+                                  base_channels=4,
+                                  depth=3,
+                                  growth_rate=1.5)
+        ```
+        
+        ## Training
+        
+        ### Data preparation
+        
+        To prep data for training, we make liberal use of PyTorch DataLoader 
+        classes. This allows for easy handling of data in the training process and 
+        automates the iterative loading of batch sizes.
+        
+        In the example below, we take pair two numpy arrays of shape ```[num_images, 
+        num_channels, x_size, y_size]``` consisting of training images and masks, convert 
+        them into PyTorch tensors, then initialize the DataLoader class.
+        
+        ```python
+        import torch
+        from torch.utils.data import TensorDataset, DataLoader
+        
+        train_data = TensorDataset(torch.Tensor(training_imgs), 
+                                   torch.Tensor(training_masks))
+        
+        train_loader_params = {'batch_size': 20,
+                               'shuffle': True}
+        
+        train_loader = DataLoader(train_data, **train_loader_params)
+        ```
+        
+        ### Training loop
+        
+        Once your DataLoaders are constructed, the training of these networks is as 
+        simple as defining a torch.nn optimizer, and calling the training script:
+        
+        ```python
+        from torch import optim, nn
+        from dlsia.core import helpers, train_scripts
+        
+        criterion = nn.CrossEntropyLoss()   # For segmenting
+        optimizer = optim.Adam(tunet_model.parameters(), lr=1e-2)
+        
+        device = helpers.get_device()
+        tunet_model = tunet_model.to(device)
+        
+        tunet_model, results = train_scripts.train_segmentation(net=tunet_model,
+                                                                trainloader=train_loader,
+                                                                validationloader=test_loader,
+                                                                NUM_EPOCHS=epochs, 
+                                                                criterion=criterion,
+                                                                optimizer=optimizer,
+                                                                device=device,
+                                                                show=1)
+        ```
+        
+        The output of the training scripts is the trained network and a dictionary with 
+        training losses and evaluation metrics. You can view them as follows:
+        
+        ```python
+        from dlsia.viz_tools import plots
+        
+        fig = plots.plot_training_results_segmentation(results)
+        fig.show()
+        ```
+        
+        ## Saving and loading models
+        
+        Each dlsia network library contains submodules for saving trained 
+        networks and loading them from file. Using the conventional PyTorch ```.pt ``` 
+        model file extension, the TUNet above may be saved with
+        
+        ```python
+        savepath = 'this_tunet.pt'
+        tunet_model.save_network_parameters(savepath)
+        ```
+        
+        and reloaded for future use with
+        
+        ```python
+        copy_of_tunet = tunet.TUNetwork_from_file(savepath)
+        ```
+        
+        ## License and Legal Stuff
+        
+        This software has been developed from funds that originate from the US tax 
+        payer and is free for academics. Please have a look at the license agreement 
+        for more details. Commercial usage will require some extra steps. Please 
+        contact ipo@lbl.gov for more details.
+        
+        ## Final Thoughts
+        
+        This documentation is far from complete, but have some notebooks as part of the codebase, which could provide a good
+        entry point.
+        
+        More to come!
+        
 Keywords: dlsia
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
-![logo](docs/images/dlsia.png 'the logo')
-
-
-# Welcome to dlsia's documentation!
-
-<a style="text-decoration:none !important;" href="https://dlsia.readthedocs.io/en/latest/" alt="website"><img src="https://img.shields.io/readthedocs/dlsia" /></a>
-<a style="text-decoration:none !important;" href="https://opensource.org/licenses/MIT" alt="License"><img src="https://img.shields.io/badge/license-MIT-blue.svg" /></a>
-<a style="text-decoration:none !important;" href="https://img.shields.io/github/commit-activity/m/phzwart/dlsia" alt="License"><img src="https://img.shields.io/github/commit-activity/m/phzwart/dlsia" /></a>
-![GitHub contributors](https://img.shields.io/github/contributors/phzwart/dlsia)
-![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/phzwart/dlsia)
-
-dlsia (Deep Learning for Scientific Image Analysis) provides easy access to a number of segmentation and denoising
-methods using convolution neural networks. The tools available are build for 
-microscopy and synchrotron-imaging/scattering data in mind, but can be used 
-elsewhere as well.
-
-The easiest way to start playing with the code is to install dlsia and 
-perform denoising/segmenting using custom neural networks in our tutorial 
-notebooks located in the dlsia/tutorials folder.
-
-## Install dlsia
-
-We offer several methods for installation. 
-
-### pip: Python package installer
-
-We are currently working on a stable release.
-
-### From source
-
-dlsia may be directly downloaded and installed into your machine by 
-cloning the public repository into an empty directory using:
-
-```console
-$ git clone https://github.com/phzwart/dlsia.git
-```
-
-Once cloned, move to the newly minted dlsia directory and install 
-dlsia using:
-
-```console
-$ cd dlsia
-$ pip install -e .
-```
-
-### Further documentation & tutorial download
-
-For more in-depth documentation and end-to-end training workflows, please 
-visit our 
-[readthedocs](https://dlsia.readthedocs.io/en/latest/index.html) page 
-for more support. To download only the tutorials in a new folder, use the 
-following terminal input for a sparse git checkout:
-
-```console
-mkdir dlsiaTutorials
-cd dlsiaTutorials
-git init
-git config core.sparseCheckout true
-git remote add -f origin https://github.com/phzwart/dlsia.git
-echo "dlsia/tutorials/*" > .git/info/sparse-checkout
-git checkout main
-```
-
-## Getting started
-
-We start with some basic imports - we import a network and some training 
-scripts:
-
-```python
-from dlsia.core.networks import msdnet
-from dlsia.core import train_scripts
-```
-
-### Mixed-Scale dense networks (MSDNet)
-
-![msdnet](docs/images/MSDNet_fig.png 'msdnet fig')
-
-
-A plain 2d mixed-scale dense network is constructed as follows:
-
-```python
-from dlsia.core.networks import msdnet
-
-msdnet_model = msdnet.MixedScaleDenseNetwork(in_channels=1,
-                                             out_channels=1,
-                                             num_layers=20,
-                                             max_dilation=10)
-```
-
-while 3d network types for volumetric images can be built passing in equivalent 
-kernels for 3 dimensions:
-
-```python
-import torch
-from torch import nn
-
-msdnet3d_model = msdnet.MixedScaleDenseNetwork(in_channels=1,
-                                               out_channels=1,
-                                               num_layers=20,
-                                               max_dilation=10,
-                                               normalization=nn.BatchNorm3d,
-                                               convolution=nn.Conv3d)
-```
-
-Note that each instance of a convolution operator is followed by ReLU 
-activation and batch normalization. To turn these off, simply pass in the 
-parameters
-
-```python
-activation=None,
-normalization=None
-```
-
-### Sparse mixed-scale dense network (SMSNet)
-
-![smsnet](docs/images/RMSNet_fig.png 'smsnet fig')
-
-
-The dlsia suite also provides ways and means to build random, sparse mixed 
-scale networks. SMSNets contain more sparsely connected nodes than a standard 
-MSDNet and are useful to alleviate overfitting and multi-network aggregation. 
-Controlling sparsity is possible, see full documentation for more details.
-
-```python
-from dlsia.core.networks import smsnet
-
-smsnet_model = smsnet.random_SMS_network(in_channels=1,
-                                         out_channels=1,
-                                         layers=20,
-                                         dilation_choices=[1, 2, 4, 8],
-                                         hidden_out_channels=[1, 2, 3])
-```
-### Tunable U-Nets
-
-![tunet](docs/images/UNet_fig.png 'tunet fig')
-
-An alternative network choice is to construct a UNet. Classic U-Nets can easily 
-explode in the number of parameters it requires; here we make it a bit easier 
-to tune desired architecture-governing parameters:
-
-```python
-from dlsia.core.networks import tunet
-
-tunet_model = tunet.TUNet(image_shape=(64, 128),
-                          in_channels=1,
-                          out_channels=4,
-                          base_channels=4,
-                          depth=3,
-                          growth_rate=1.5)
-```
-
-## Training
-
-### Data preparation
-
-To prep data for training, we make liberal use of PyTorch DataLoader 
-classes. This allows for easy handling of data in the training process and 
-automates the iterative loading of batch sizes.
-
-In the example below, we take pair two numpy arrays of shape ```[num_images, 
-num_channels, x_size, y_size]``` consisting of training images and masks, convert 
-them into PyTorch tensors, then initialize the DataLoader class.
-
-```python
-import torch
-from torch.utils.data import TensorDataset, DataLoader
-
-train_data = TensorDataset(torch.Tensor(training_imgs), 
-                           torch.Tensor(training_masks))
-
-train_loader_params = {'batch_size': 20,
-                       'shuffle': True}
-
-train_loader = DataLoader(train_data, **train_loader_params)
-```
-
-### Training loop
-
-Once your DataLoaders are constructed, the training of these networks is as 
-simple as defining a torch.nn optimizer, and calling the training script:
-
-```python
-from torch import optim, nn
-from dlsia.core import helpers, train_scripts
-
-criterion = nn.CrossEntropyLoss()   # For segmenting
-optimizer = optim.Adam(tunet_model.parameters(), lr=1e-2)
-
-device = helpers.get_device()
-tunet_model = tunet_model.to(device)
-
-tunet_model, results = train_scripts.train_segmentation(net=tunet_model,
-                                                        trainloader=train_loader,
-                                                        validationloader=test_loader,
-                                                        NUM_EPOCHS=epochs, 
-                                                        criterion=criterion,
-                                                        optimizer=optimizer,
-                                                        device=device,
-                                                        show=1)
-```
-
-The output of the training scripts is the trained network and a dictionary with 
-training losses and evaluation metrics. You can view them as follows:
-
-```python
-from dlsia.viz_tools import plots
-
-fig = plots.plot_training_results_segmentation(results)
-fig.show()
-```
-
-## Saving and loading models
-
-Each dlsia network library contains submodules for saving trained 
-networks and loading them from file. Using the conventional PyTorch ```.pt ``` 
-model file extension, the TUNet above may be saved with
-
-```python
-savepath = 'this_tunet.pt'
-tunet_model.save_network_parameters(savepath)
-```
-
-and reloaded for future use with
-
-```python
-copy_of_tunet = tunet.TUNetwork_from_file(savepath)
-```
-
-## License and Legal Stuff
-
-This software has been developed from funds that originate from the US tax 
-payer and is free for academics. Please have a look at the license agreement 
-for more details. Commercial usage will require some extra steps. Please 
-contact ipo@lbl.gov for more details.
-
-## Final Thoughts
-
-This documentation is far from complete, but have some notebooks as part of the codebase, which could provide a good
-entry point.
-
-More to come!
```

### Comparing `dlsia-0.3.0/dlsia.egg-info/SOURCES.txt` & `dlsia-0.3.1/dlsia.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,35 +21,42 @@
 dlsia/core/inference_scripts.py
 dlsia/core/train_scripts.py
 dlsia/core/conformalize/__init__.py
 dlsia/core/conformalize/conformalize_segmentation.py
 dlsia/core/networks/__init__.py
 dlsia/core/networks/aggnet.py
 dlsia/core/networks/baggins.py
+dlsia/core/networks/construct_sms_ensemble.py
 dlsia/core/networks/graph_utils.py
+dlsia/core/networks/grey2color.py
 dlsia/core/networks/msae.py
 dlsia/core/networks/msd_graph_tools.py
 dlsia/core/networks/msdae.py
 dlsia/core/networks/msdnet.py
 dlsia/core/networks/msdnet2.py
+dlsia/core/networks/orthonet.py
+dlsia/core/networks/random_autoencoder.py
 dlsia/core/networks/scale_up_down.py
 dlsia/core/networks/sms1d.py
 dlsia/core/networks/sms3d.py
 dlsia/core/networks/smsnet.py
 dlsia/core/networks/sparsenet.py
 dlsia/core/networks/squashnet.py
 dlsia/core/networks/tunet.py
 dlsia/core/networks/tunet3plus.py
 dlsia/core/networks/unet.py
 dlsia/core/utils/__init__.py
 dlsia/core/utils/agg_utils.py
+dlsia/core/utils/blur.py
+dlsia/core/utils/downsample.py
 dlsia/core/utils/feature_extraction.py
 dlsia/core/utils/latent_space_viewer.py
 dlsia/core/utils/randomized_data_loader.py
 dlsia/core/utils/simple_instance_segmenter.py
+dlsia/core/utils/sparse_tools.py
 dlsia/test_data/__init__.py
 dlsia/test_data/two_d/__init__.py
 dlsia/test_data/two_d/build_test_data.py
 dlsia/test_data/two_d/diffusion_model.py
 dlsia/test_data/two_d/noisy_gauss_2d.py
 dlsia/test_data/two_d/noisy_gauss_2d_time.py
 dlsia/test_data/two_d/random_shapes.py
@@ -73,8 +80,9 @@
 docs/source/dlsia.core.conformalize.rst
 docs/source/dlsia.core.networks.rst
 docs/source/dlsia.core.rst
 docs/source/dlsia.rst
 docs/source/dlsia.test_data.rst
 docs/source/dlsia.test_data.two_d.rst
 docs/source/dlsia.viz_tools.rst
-tests/__init__.py
+tests/__init__.py
+tests/test_blur.py
```

### Comparing `dlsia-0.3.0/docs/Makefile` & `dlsia-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/conf.py` & `dlsia-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/images/Autoencoder_fig.png` & `dlsia-0.3.1/docs/images/Autoencoder_fig.png`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/images/MSDNet_fig.png` & `dlsia-0.3.1/docs/images/MSDNet_fig.png`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/images/RMSNet_fig.png` & `dlsia-0.3.1/docs/images/RMSNet_fig.png`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/images/UNet_fig.png` & `dlsia-0.3.1/docs/images/UNet_fig.png`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/images/dlsia.png` & `dlsia-0.3.1/docs/images/dlsia.png`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/index.rst` & `dlsia-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/make.bat` & `dlsia-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/source/dlsia.core.networks.rst` & `dlsia-0.3.1/docs/source/dlsia.core.networks.rst`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/source/dlsia.core.rst` & `dlsia-0.3.1/docs/source/dlsia.core.rst`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/docs/source/dlsia.test_data.two_d.rst` & `dlsia-0.3.1/docs/source/dlsia.test_data.two_d.rst`

 * *Files identical despite different names*

### Comparing `dlsia-0.3.0/setup.py` & `dlsia-0.3.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     keywords='dlsia',
     name='dlsia',
     packages=find_packages(include=['dlsia', 'dlsia.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/phzwart/dlsia/',
-    version='0.3.0',
+    version='0.3.1',
     zip_safe=False,
 )
```

