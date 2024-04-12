# Comparing `tmp/liom-toolkit-0.7.1.tar.gz` & `tmp/liom-toolkit-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liom-toolkit-0.7.1.tar", last modified: Fri Apr 12 14:21:40 2024, max compression
+gzip compressed data, was "liom-toolkit-0.7.2.tar", last modified: Fri Apr 12 14:32:59 2024, max compression
```

## Comparing `liom-toolkit-0.7.1.tar` & `liom-toolkit-0.7.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.269647 liom-toolkit-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.273647 liom-toolkit-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.273647 liom-toolkit-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.273647 liom-toolkit-0.7.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.277647 liom-toolkit-0.7.1/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.registration.register.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.registration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.registration.templating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.registration.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.segmentation.stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.utils.conversion.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.utils.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/liom_toolkit.utils.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/docs/source/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.277647 liom-toolkit-0.7.1/liom_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.277647 liom-toolkit-0.7.1/liom_toolkit/registration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/registration/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/registration/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/registration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.277647 liom-toolkit-0.7.1/liom_toolkit/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/plane_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/volume_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/cldice.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1013 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/make_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2808 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/predict_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/training.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8627 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/liom_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/liom_toolkit/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/visualization/slice_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/liom_toolkit/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/liom_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:21:40.000000 liom-toolkit-0.7.1/liom_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-12 14:21:40.000000 liom-toolkit-0.7.1/liom_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:21:40.000000 liom-toolkit-0.7.1/liom_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 14:21:40.000000 liom-toolkit-0.7.1/liom_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:21:40.000000 liom-toolkit-0.7.1/liom_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:21:40.281647 liom-toolkit-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 14:21:33.000000 liom-toolkit-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.724211 liom-toolkit-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.templating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.conversion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/plane_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/volume_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/cldice.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1013 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/make_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2808 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/predict_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8627 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/slice_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/setup.py
```

### Comparing `liom-toolkit-0.7.1/.github/workflows/main.yml` & `liom-toolkit-0.7.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/.gitignore` & `liom-toolkit-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/LICENSE` & `liom-toolkit-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/PKG-INFO` & `liom-toolkit-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.1
+Version: 0.7.2
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.7.1/README.md` & `liom-toolkit-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/docs/Makefile` & `liom-toolkit-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/docs/make.bat` & `liom-toolkit-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/docs/source/conf.py` & `liom-toolkit-0.7.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/docs/source/index.rst` & `liom-toolkit-0.7.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/registration/register.py` & `liom-toolkit-0.7.2/liom_toolkit/registration/register.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/registration/templating.py` & `liom-toolkit-0.7.2/liom_toolkit/registration/templating.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/registration/utils.py` & `liom-toolkit-0.7.2/liom_toolkit/registration/utils.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/plane_segmentation.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/plane_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/stats.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/stats.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/volume_segmentation.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/volume_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/cldice.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/cldice.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/data.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/data.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/loss.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/loss.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/make_dataset.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/make_dataset.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/model.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/model.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/predict_one.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/predict_one.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/training.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/training.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/utils.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/utils.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/segmentation/vseg/validation.py` & `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/validation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/utils/conversion.py` & `liom-toolkit-0.7.2/liom_toolkit/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit/utils/io.py` & `liom-toolkit-0.7.2/liom_toolkit/utils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import os
 import tempfile
 from typing import Callable, Union
 
 import ants
 import nrrd
 import numpy as np
 import zarr
 from dask import array as da
 from ome_zarr.dask_utils import resize as dask_resize
 from ome_zarr.io import parse_url
 from ome_zarr.reader import Node, Reader
 from ome_zarr.scale import Scaler, ArrayLike
 from ome_zarr.writer import write_labels
+from skimage.io import imsave
 from skimage.transform import resize
+from tqdm import tqdm
 
 from liom_toolkit.registration import download_allen_atlas
 from liom_toolkit.segmentation import segment_3d_brain
+from .utils import convert_to_png_for_saving
 
 
 def load_zarr(zarr_file: str) -> list[Node]:
     """
     Load a zarr file to an ANTs image.
 
     :param zarr_file: The zarr file to load.
@@ -514,7 +518,24 @@
         # Check for empy dict
         if node.metadata == {}:
             continue
 
         if node.metadata["name"] == name:
             return node
     return None
+
+
+def extract_zarr_to_png(zarr_file: str, target_dir: str) -> None:
+    node = load_zarr(zarr_file)[0]
+    volume = node.data[0]
+
+    # Create if not exists, empty if exists
+    if not os.path.exists(target_dir):
+        os.makedirs(target_dir)
+    else:
+        for file in os.listdir(target_dir):
+            os.remove(os.path.join(target_dir, file))
+
+    for z in tqdm(range(volume.shape[0])):
+        image = volume[z, :, :]
+        image = convert_to_png_for_saving(image)
+        imsave(f"{target_dir}/{str(z)}.png", image, check_contrast=False)
```

### Comparing `liom-toolkit-0.7.1/liom_toolkit/visualization/slice_extraction.py` & `liom-toolkit-0.7.2/liom_toolkit/visualization/slice_extraction.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/liom_toolkit.egg-info/PKG-INFO` & `liom-toolkit-0.7.2/liom_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.1
+Version: 0.7.2
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.7.1/liom_toolkit.egg-info/SOURCES.txt` & `liom-toolkit-0.7.2/liom_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.1/setup.py` & `liom-toolkit-0.7.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="liom-toolkit",
-    version="0.7.1",
+    version="0.7.2",
     author="Laboratoire d’Imagerie Optique et Moléculaire",
     author_email="frederic.lesage@polymtl.ca",
     packages=find_packages(),
     description="Package to support the research of LIOM.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/LIOMLab/liom-toolkit",
```

