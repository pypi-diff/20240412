# Comparing `tmp/liom-toolkit-0.7.2.tar.gz` & `tmp/liom-toolkit-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liom-toolkit-0.7.2.tar", last modified: Fri Apr 12 14:32:59 2024, max compression
+gzip compressed data, was "liom-toolkit-0.7.3.tar", last modified: Fri Apr 12 16:20:29 2024, max compression
```

## Comparing `liom-toolkit-0.7.2.tar` & `liom-toolkit-0.7.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.724211 liom-toolkit-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.728211 liom-toolkit-0.7.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.register.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.templating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.registration.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.conversion.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/liom_toolkit.utils.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/docs/source/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/registration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/registration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.732210 liom-toolkit-0.7.2/liom_toolkit/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/plane_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/volume_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/cldice.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/data.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1013 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/make_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2808 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/predict_one.py
--rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/training.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8627 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19091 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/slice_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/liom_toolkit/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/liom_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:32:59.000000 liom-toolkit-0.7.2/liom_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:32:59.736210 liom-toolkit-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 14:32:55.000000 liom-toolkit-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.268265 liom-toolkit-0.7.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.268265 liom-toolkit-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.268265 liom-toolkit-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.272265 liom-toolkit-0.7.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.272265 liom-toolkit-0.7.3/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.registration.register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.registration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.registration.templating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.registration.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.segmentation.stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.utils.conversion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.utils.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/liom_toolkit.utils.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/docs/source/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.272265 liom-toolkit-0.7.3/liom_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.276265 liom-toolkit-0.7.3/liom_toolkit/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/registration/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/registration/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/registration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.276265 liom-toolkit-0.7.3/liom_toolkit/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/plane_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/volume_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.276265 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/cldice.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1862 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1389 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/make_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4105 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4210 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/predict_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12942 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/liom_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19111 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/liom_toolkit/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/visualization/slice_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/liom_toolkit/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/liom_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 16:20:29.000000 liom-toolkit-0.7.3/liom_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-12 16:20:29.000000 liom-toolkit-0.7.3/liom_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:20:29.000000 liom-toolkit-0.7.3/liom_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 16:20:29.000000 liom-toolkit-0.7.3/liom_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 16:20:29.000000 liom-toolkit-0.7.3/liom_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:20:29.280265 liom-toolkit-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 16:20:25.000000 liom-toolkit-0.7.3/setup.py
```

### Comparing `liom-toolkit-0.7.2/.github/workflows/main.yml` & `liom-toolkit-0.7.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/.gitignore` & `liom-toolkit-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/LICENSE` & `liom-toolkit-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/PKG-INFO` & `liom-toolkit-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.2
+Version: 0.7.3
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.7.2/README.md` & `liom-toolkit-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/docs/Makefile` & `liom-toolkit-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/docs/make.bat` & `liom-toolkit-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/docs/source/conf.py` & `liom-toolkit-0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/docs/source/index.rst` & `liom-toolkit-0.7.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/registration/register.py` & `liom-toolkit-0.7.3/liom_toolkit/registration/register.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/registration/templating.py` & `liom-toolkit-0.7.3/liom_toolkit/registration/templating.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/registration/utils.py` & `liom-toolkit-0.7.3/liom_toolkit/registration/utils.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/plane_segmentation.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/plane_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/stats.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/stats.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/volume_segmentation.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/volume_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/predict_one.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/predict_one.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 import shutil
 
+from .model import VsegModel
 from .utils import *
 
 
-def predict_one(model, img_path, save_path, stride=256, width=256, norm=True, dev="cuda", patching=True):
-    """ Hyperparameters """
+def predict_one(model: VsegModel, img_path: str, save_path: str, stride: int = 256, width: int = 256, norm: bool = True,
+                dev: str = "cuda", patching: bool = True) -> np.ndarray:
+    """
+    Predict one image
+
+    :param model: The model to use for prediction
+    :type model: VsegModel
+    :param img_path: The path to the image to predict
+    :type img_path: str
+    :param save_path: The path to save the results
+    :type save_path: str
+    :param stride: The stride of the patches
+    :type stride: int
+    :param width: The width of the patches
+    :type width: int
+    :param norm: Normalize the images
+    :type norm: bool
+    :param dev: The device to use for prediction
+    :type dev: str
+    :param patching: Whether to use patching
+    :type patching: bool
+    :return: The predicted image
+    :rtype: np.ndarray
+    """
     if patching:
         H = width
         W = width
         size = (H, W)
         stride = stride
     else:
         image = imread(img_path)
@@ -87,15 +110,14 @@
                                              n_patches_by_row)
 
         y1 += 1
 
     inference = np.floor(inference)
     inference = (inference / inference.max() * 255).astype(np.uint8)
     inference = inference.astype(bool)
-    # inference = remove_small_objects(inference)
     inference = inference.astype(np.uint8) * 255
 
     save_inf = f"{save_path}/{image_id}_segmented.png"
     imsave(save_inf,
            inference, check_contrast=False)
 
     return inference
```

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/training.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/training.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,36 @@
+import torch.nn
 import wandb
 from skimage.color import label2rgb
 from torch.utils.data import DataLoader
 
 from .data import PatchDataset
 from .loss import DiceBCELoss
 from .model import VsegModel
 from .utils import *
 
 
-def train(model, loader, optimizer, loss_fn, device):
+def train(model: VsegModel, loader: DataLoader, optimizer: torch.optim.Optimizer, loss_fn: torch.nn.Module,
+          device: torch.device) -> (float, torch.Tensor, torch.Tensor, torch.Tensor):
+    """
+    Train the model for an epoch
+
+    :param model: The model to train
+    :type model: VsegModel
+    :param loader: The data loader
+    :type loader: torch.utils.data.DataLoader
+    :param optimizer: The optimizer
+    :type optimizer: torch.optim.Optimizer
+    :param loss_fn: The loss function
+    :type loss_fn: torch.nn.Module
+    :param device: The device to use for training
+    :type device: torch.device
+    :return: The loss, the true labels, the predicted labels, and the input
+    :rtype: (float, torch.Tensor, torch.Tensor, torch.Tensor)
+    """
     # Initialize epoch loss to 0
     epoch_loss = 0.0
 
     # Put in training mode 
     model.train()
 
     # Iterate over train-loader
@@ -27,15 +45,30 @@
         epoch_loss += loss.item()
 
     # Normalize cumulative loss for number of examples
     epoch_loss = epoch_loss / len(loader)
     return epoch_loss, y, y_pred, x
 
 
-def evaluate(model, loader, loss_fn, device):
+def evaluate(model: VsegModel, loader: DataLoader, loss_fn: torch.nn.Module, device: torch.device) -> (
+        float, torch.Tensor, torch.Tensor, torch.Tensor, float, float, float, float):
+    """
+    Evaluate the model for an epoch
+
+    :param model: The model to evaluate
+    :type model: VsegModel
+    :param loader: The data loader
+    :type loader: torch.utils.data.DataLoader
+    :param loss_fn: The loss function
+    :type loss_fn: torch.nn.Module
+    :param device: The device to use for evaluation
+    :type device: torch.device
+    :return: The loss, the true labels, the predicted labels, the input, and the metrics
+    :rtype: (float, torch.Tensor, torch.Tensor, torch.Tensor, float, float, float, float)
+    """
     # Initialize epoch loss to 0
     # Added metrics
     epoch_loss = 0.0
     f1 = 0.0
     accuracy = 0.0
     jaccard = 0.0
     recall = 0.0
@@ -67,15 +100,29 @@
         accuracy = accuracy / len(loader)
         jaccard = jaccard / len(loader)
         recall = recall / len(loader)
 
     return epoch_loss, y, y_pred, x, f1, accuracy, jaccard, recall
 
 
-def create_images(x, y, pred, num_images=4):
+def create_images(x: torch.Tensor, y: torch.Tensor, pred: torch.Tensor, num_images: int = 4) -> list[np.ndarray]:
+    """
+    Create images for visualization
+
+    :param x: The input tensor
+    :type x: torch.Tensor
+    :param y: The true labels
+    :type y: torch.Tensor
+    :param pred: The predicted labels
+    :type pred: torch.Tensor
+    :param num_images: The number of images to create
+    :type num_images: int
+    :return: The images
+    :rtype: List[np.ndarray]
+    """
     y_mask = y.cpu().detach().numpy()
     pred_mask = pred.cpu().detach().numpy()
     x = x.cpu().detach().numpy()
     images = []
     num_images = min(num_images, x.shape[0])
     i = 0
     while len(images) < num_images or i - 1 == x.shape[0]:
@@ -110,16 +157,33 @@
 
     labels = np.max([y_mask, diff_mask, pred_mask], axis=0)
     img = label2rgb(labels, image=img, colors=[[0, 0, 1], [0, 1, 0], [1, 0, 0]], alpha=0.3, bg_label=0,
                     bg_color=None)
     return img
 
 
-def train_model(dataset_dir="data/patches", dev="cuda", output_train="data/training", learning_rate=0.003673,
-                batch_size=35, epochs=62, config=None):
+def train_model(dataset_dir: str = "data/patches", dev: str = "cuda", output_train: str = "data/training",
+                learning_rate: float = 0.003673, batch_size: int = 35, epochs: int = 62) -> None:
+    """
+    Train the vessel segmentation model
+
+    :param dataset_dir: The directory of the dataset
+    :type dataset_dir: str
+    :param dev: The device to use for training
+    :type dev: str
+    :param output_train: The output directory for the training
+    :type output_train: str
+    :param learning_rate: The learning rate for the optimizer
+    :type learning_rate: float
+    :param batch_size: The batch size for training
+    :type batch_size: int
+    :param epochs: The number of epochs to train
+    :type epochs: int
+    :return: None
+    """
     # Setup training parameters and wandb run
     hyperparameter_defaults = dict(
         batch_size=batch_size,
         learning_rate=learning_rate,
         epochs=epochs)
 
     # Init wandb
@@ -234,16 +298,14 @@
 
     final_loss = pd.DataFrame(data=[train_losses, val_losses]).T
     final_loss.to_csv('final_metrics.csv', encoding='utf-8', index=False)
 
 
 if __name__ == "__main__":
     # Hardcoded for wandb sweeps
-    # dataset_dir = "/Users/frans/docker_data/confocal/vseg/patches"
-    # output = "/Users/frans/docker_data/confocal/vseg/training"
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-    dataset_dir = "/home/frans/code/vseg/data/patches"
-    output = "/home/frans/code/vseg/data/training"
+    dataset_dir = "vseg/data/patches"
+    output = "vseg/data/training"
 
     train_model(dataset_dir=dataset_dir,
                 dev=device,
                 output_train=output)
```

### Comparing `liom-toolkit-0.7.2/liom_toolkit/segmentation/vseg/validation.py` & `liom-toolkit-0.7.3/liom_toolkit/segmentation/vseg/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,64 @@
 import csv
 
 import matplotlib.pyplot as plt
 import numpy as np
 from skimage.io import imread
 
 from .cldice import cl_dice
+from .model import VsegModel
 from .predict_one import predict_one
 from .utils import calculate_metrics
 
 
-def show_diff(mask, prediction, output_path, id, acq) -> None:
+def show_diff(mask: np.ndarray, prediction: np.ndarray, output_path: str, id: str, acq: str) -> None:
     """
-       - Black: TN
-       - Red: FP
-       - Blue: FN
-       - White: TP
+    Show the difference between the mask and the prediction.
+    - Black: TN
+    - Red: FP
+    - Blue: FN
+    - White: TP
+
+    :param mask: The mask
+    :type mask: np.ndarray
+    :param prediction: The prediction
+    :type prediction: np.ndarray
+    :param output_path: The output path
+    :type output_path: str
+    :param id: The id of the image
+    :type id: str
+    :param acq: The acquisition of the image
+    :type acq: str
+    :return: None
     """
-
     mask = mask > 0.5
     prediction = prediction > 0.5
 
     red = prediction * 1.0
     blue = mask * 1.0
     green = (prediction & mask) * 1.0
 
     rgb = np.stack([red, green, blue], axis=2)
     plt.imsave(f"{output_path}/{acq}_{id}_comparison.png", rgb)
 
 
-def validate_model(model, img_list, save_path, device):
-    # img_list: list of image paths to validate. The mask has to be in the same folder
+def validate_model(model: VsegModel, img_list: list[np.ndarray], save_path: str, device: str) -> None:
+    """
+    Validate a model on a list of images.
+
+    :param model: The model to validate
+    :type model: VsegModel
+    :param img_list: list of image paths to validate. The mask has to be in the same folder
+    :type img_list: list[np.ndarray]
+    :param save_path: The path to save the results
+    :type save_path: str
+    :param device: The device to use for prediction
+    :type device: str
+    :return: None
+    """
     f1 = []
     recall = []
     accuracy = []
     jaccard = []
     cldice = []
     ids = []
```

### Comparing `liom-toolkit-0.7.2/liom_toolkit/utils/conversion.py` & `liom-toolkit-0.7.3/liom_toolkit/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit/utils/io.py` & `liom-toolkit-0.7.3/liom_toolkit/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ome_zarr.writer import write_labels
 from skimage.io import imsave
 from skimage.transform import resize
 from tqdm import tqdm
 
 from liom_toolkit.registration import download_allen_atlas
 from liom_toolkit.segmentation import segment_3d_brain
-from .utils import convert_to_png_for_saving
+from liom_toolkit.visualization import convert_to_png_for_saving
 
 
 def load_zarr(zarr_file: str) -> list[Node]:
     """
     Load a zarr file to an ANTs image.
 
     :param zarr_file: The zarr file to load.
```

### Comparing `liom-toolkit-0.7.2/liom_toolkit/visualization/slice_extraction.py` & `liom-toolkit-0.7.3/liom_toolkit/visualization/slice_extraction.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/liom_toolkit.egg-info/PKG-INFO` & `liom-toolkit-0.7.3/liom_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.7.2
+Version: 0.7.3
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `liom-toolkit-0.7.2/liom_toolkit.egg-info/SOURCES.txt` & `liom-toolkit-0.7.3/liom_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.7.2/setup.py` & `liom-toolkit-0.7.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="liom-toolkit",
-    version="0.7.2",
+    version="0.7.3",
     author="Laboratoire d’Imagerie Optique et Moléculaire",
     author_email="frederic.lesage@polymtl.ca",
     packages=find_packages(),
     description="Package to support the research of LIOM.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/LIOMLab/liom-toolkit",
```

