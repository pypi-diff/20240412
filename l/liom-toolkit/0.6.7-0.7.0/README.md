# Comparing `tmp/liom-toolkit-0.6.7.tar.gz` & `tmp/liom-toolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liom-toolkit-0.6.7.tar", last modified: Mon Mar 25 14:58:15 2024, max compression
+gzip compressed data, was "liom-toolkit-0.7.0.tar", last modified: Fri Apr 12 14:12:17 2024, max compression
```

## Comparing `liom-toolkit-0.6.7.tar` & `liom-toolkit-0.7.0.tar`

### file list

```diff
@@ -1,61 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.123930 liom-toolkit-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.127930 liom-toolkit-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.127930 liom-toolkit-0.6.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.127930 liom-toolkit-0.6.7/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.131930 liom-toolkit-0.6.7/docs/source/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.registration.register.rst
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.registration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.registration.templating.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.registration.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.rst
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.segmentation.stats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.utils.conversion.rst
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.utils.io.rst
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/liom_toolkit.utils.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/docs/source/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.131930 liom-toolkit-0.6.7/liom_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.131930 liom-toolkit-0.6.7/liom_toolkit/registration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/registration/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/registration/templating.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/registration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.131930 liom-toolkit-0.6.7/liom_toolkit/segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/segmentation/plane_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/segmentation/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/segmentation/volume_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/liom_toolkit/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/liom_toolkit/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/visualization/slice_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/liom_toolkit/visualization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/liom_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-25 14:58:15.000000 liom-toolkit-0.6.7/liom_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-25 14:58:15.000000 liom-toolkit-0.6.7/liom_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:58:15.000000 liom-toolkit-0.6.7/liom_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-25 14:58:15.000000 liom-toolkit-0.6.7/liom_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 14:58:15.000000 liom-toolkit-0.6.7/liom_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:58:15.135930 liom-toolkit-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-25 14:58:09.000000 liom-toolkit-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.840724 liom-toolkit-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.840724 liom-toolkit-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.844724 liom-toolkit-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.844724 liom-toolkit-0.7.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.844724 liom-toolkit-0.7.0/docs/source/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.registration.register.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.registration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.registration.templating.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.registration.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.segmentation.plane_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.segmentation.stats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.segmentation.volume_segmentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.utils.conversion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.utils.io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/liom_toolkit.utils.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/docs/source/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.844724 liom-toolkit-0.7.0/liom_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.848724 liom-toolkit-0.7.0/liom_toolkit/registration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17232 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/registration/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15544 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/registration/templating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/registration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.848724 liom-toolkit-0.7.0/liom_toolkit/segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/plane_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12429 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/volume_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.848724 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      810 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/data.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1013 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      750 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/make_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2808 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3517 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/predict_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8627 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/segmentation/vseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/liom_toolkit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14517 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/liom_toolkit/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/visualization/slice_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/liom_toolkit/visualization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/liom_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-12 14:12:17.000000 liom-toolkit-0.7.0/liom_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-12 14:12:17.000000 liom-toolkit-0.7.0/liom_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:12:17.000000 liom-toolkit-0.7.0/liom_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 14:12:17.000000 liom-toolkit-0.7.0/liom_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 14:12:17.000000 liom-toolkit-0.7.0/liom_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:12:17.852724 liom-toolkit-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-12 14:12:13.000000 liom-toolkit-0.7.0/setup.py
```

### Comparing `liom-toolkit-0.6.7/.github/workflows/main.yml` & `liom-toolkit-0.7.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/.gitignore` & `liom-toolkit-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/LICENSE` & `liom-toolkit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/PKG-INFO` & `liom-toolkit-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.6.7
+Version: 0.7.0
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -17,14 +17,21 @@
 Requires-Dist: zarr
 Requires-Dist: h5py
 Requires-Dist: pynrrd
 Requires-Dist: PyWavelets
 Requires-Dist: SimpleITK
 Requires-Dist: allensdk
 Requires-Dist: dask
+Requires-Dist: opencv-python
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: wandb
+Requires-Dist: patchify
+Requires-Dist: natsort
+Requires-Dist: albumentations
 
 # Liom Toolkit
 
 This package supports the research being done by the [Laboratoire d’Imagerie Optique et Moléculaire](https://liom.ca) at
 Polytechnique Montréal. It hosts a collection of scripts used to process and analyze data collected by the lab.
 
 [![Build and Publish Toolkit](https://github.com/LIOMLab/liom-toolkit/actions/workflows/main.yml/badge.svg)](https://github.com/LIOMLab/liom-toolkit/actions/workflows/main.yml) [![Documentation Status](https://readthedocs.org/projects/liom-toolkit/badge/?version=latest)](https://liom-toolkit.readthedocs.io/en/latest/?badge=latest)
@@ -37,23 +44,33 @@
 pip install liom-toolkit
 ```
 
 ## Requirements
 
 The package requires the following packages to be installed and will attempt to install them using installation:
 
-- antspyx
-- allensdk
+- antspyx 
+- tqdm
 - scikit-image
 - ome-zarr
 - nibabel
 - zarr
 - h5py
 - pynrrd
+- PyWavelets
 - SimpleITK
+- allensdk
+- dask
+- opencv-python
+- torch
+- torchvision
+- wandb
+- patchify
+- natsort
+- albumentations
 
 To create an anaconda environment with all the required packages, run the following commands:
 
 ```bash
 conda create -n <name>
 conda activate <name>
 conda install python=3.10
```

### Comparing `liom-toolkit-0.6.7/README.md` & `liom-toolkit-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,33 @@
 pip install liom-toolkit
 ```
 
 ## Requirements
 
 The package requires the following packages to be installed and will attempt to install them using installation:
 
-- antspyx
-- allensdk
+- antspyx 
+- tqdm
 - scikit-image
 - ome-zarr
 - nibabel
 - zarr
 - h5py
 - pynrrd
+- PyWavelets
 - SimpleITK
+- allensdk
+- dask
+- opencv-python
+- torch
+- torchvision
+- wandb
+- patchify
+- natsort
+- albumentations
 
 To create an anaconda environment with all the required packages, run the following commands:
 
 ```bash
 conda create -n <name>
 conda activate <name>
 conda install python=3.10
```

### Comparing `liom-toolkit-0.6.7/docs/Makefile` & `liom-toolkit-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/docs/make.bat` & `liom-toolkit-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/docs/source/conf.py` & `liom-toolkit-0.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/docs/source/index.rst` & `liom-toolkit-0.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/registration/register.py` & `liom-toolkit-0.7.0/liom_toolkit/registration/register.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/registration/templating.py` & `liom-toolkit-0.7.0/liom_toolkit/registration/templating.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/registration/utils.py` & `liom-toolkit-0.7.0/liom_toolkit/registration/utils.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/segmentation/plane_segmentation.py` & `liom-toolkit-0.7.0/liom_toolkit/segmentation/plane_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/segmentation/stats.py` & `liom-toolkit-0.7.0/liom_toolkit/segmentation/stats.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/segmentation/volume_segmentation.py` & `liom-toolkit-0.7.0/liom_toolkit/segmentation/volume_segmentation.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/utils/conversion.py` & `liom-toolkit-0.7.0/liom_toolkit/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/utils/io.py` & `liom-toolkit-0.7.0/liom_toolkit/utils/io.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit/visualization/slice_extraction.py` & `liom-toolkit-0.7.0/liom_toolkit/visualization/slice_extraction.py`

 * *Files identical despite different names*

### Comparing `liom-toolkit-0.6.7/liom_toolkit.egg-info/PKG-INFO` & `liom-toolkit-0.7.0/liom_toolkit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liom-toolkit
-Version: 0.6.7
+Version: 0.7.0
 Summary: Package to support the research of LIOM.
 Home-page: https://github.com/LIOMLab/liom-toolkit
 Author: Laboratoire d’Imagerie Optique et Moléculaire
 Author-email: frederic.lesage@polymtl.ca
 License: GPLv3+
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -17,14 +17,21 @@
 Requires-Dist: zarr
 Requires-Dist: h5py
 Requires-Dist: pynrrd
 Requires-Dist: PyWavelets
 Requires-Dist: SimpleITK
 Requires-Dist: allensdk
 Requires-Dist: dask
+Requires-Dist: opencv-python
+Requires-Dist: torch
+Requires-Dist: torchvision
+Requires-Dist: wandb
+Requires-Dist: patchify
+Requires-Dist: natsort
+Requires-Dist: albumentations
 
 # Liom Toolkit
 
 This package supports the research being done by the [Laboratoire d’Imagerie Optique et Moléculaire](https://liom.ca) at
 Polytechnique Montréal. It hosts a collection of scripts used to process and analyze data collected by the lab.
 
 [![Build and Publish Toolkit](https://github.com/LIOMLab/liom-toolkit/actions/workflows/main.yml/badge.svg)](https://github.com/LIOMLab/liom-toolkit/actions/workflows/main.yml) [![Documentation Status](https://readthedocs.org/projects/liom-toolkit/badge/?version=latest)](https://liom-toolkit.readthedocs.io/en/latest/?badge=latest)
@@ -37,23 +44,33 @@
 pip install liom-toolkit
 ```
 
 ## Requirements
 
 The package requires the following packages to be installed and will attempt to install them using installation:
 
-- antspyx
-- allensdk
+- antspyx 
+- tqdm
 - scikit-image
 - ome-zarr
 - nibabel
 - zarr
 - h5py
 - pynrrd
+- PyWavelets
 - SimpleITK
+- allensdk
+- dask
+- opencv-python
+- torch
+- torchvision
+- wandb
+- patchify
+- natsort
+- albumentations
 
 To create an anaconda environment with all the required packages, run the following commands:
 
 ```bash
 conda create -n <name>
 conda activate <name>
 conda install python=3.10
```

### Comparing `liom-toolkit-0.6.7/liom_toolkit.egg-info/SOURCES.txt` & `liom-toolkit-0.7.0/liom_toolkit.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -34,14 +34,22 @@
 liom_toolkit/registration/register.py
 liom_toolkit/registration/templating.py
 liom_toolkit/registration/utils.py
 liom_toolkit/segmentation/__init__.py
 liom_toolkit/segmentation/plane_segmentation.py
 liom_toolkit/segmentation/stats.py
 liom_toolkit/segmentation/volume_segmentation.py
+liom_toolkit/segmentation/vseg/__init__.py
+liom_toolkit/segmentation/vseg/data.py
+liom_toolkit/segmentation/vseg/loss.py
+liom_toolkit/segmentation/vseg/make_dataset.py
+liom_toolkit/segmentation/vseg/model.py
+liom_toolkit/segmentation/vseg/predict_one.py
+liom_toolkit/segmentation/vseg/training.py
+liom_toolkit/segmentation/vseg/utils.py
 liom_toolkit/utils/__init__.py
 liom_toolkit/utils/conversion.py
 liom_toolkit/utils/io.py
 liom_toolkit/utils/utils.py
 liom_toolkit/visualization/__init__.py
 liom_toolkit/visualization/slice_extraction.py
 liom_toolkit/visualization/utils.py
```

### Comparing `liom-toolkit-0.6.7/setup.py` & `liom-toolkit-0.7.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="liom-toolkit",
-    version="0.6.7",
+    version="0.7.0",
     author="Laboratoire d’Imagerie Optique et Moléculaire",
     author_email="frederic.lesage@polymtl.ca",
     packages=find_packages(),
     description="Package to support the research of LIOM.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/LIOMLab/liom-toolkit",
     license='GPLv3+',
     license_files=['LICENSE'],
     python_requires='>=3.10',
-    install_requires=['antspyx', 'tqdm', 'scikit-image', 'ome-zarr==0.8.2', 'nibabel', 'zarr', 'h5py', 'pynrrd', 'PyWavelets',
-                      'SimpleITK', 'allensdk', 'dask']
+    install_requires=['antspyx', 'tqdm', 'scikit-image', 'ome-zarr==0.8.2', 'nibabel', 'zarr', 'h5py', 'pynrrd',
+                      'PyWavelets', 'SimpleITK', 'allensdk', 'dask', 'opencv-python', 'torch', 'torchvision', 'wandb',
+                      'patchify', 'natsort', 'albumentations']
 )
```

