# Comparing `tmp/cellfinder-1.1.2.tar.gz` & `tmp/cellfinder-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-1.1.2.tar", last modified: Fri Apr  5 10:44:13 2024, max compression
+gzip compressed data, was "cellfinder-1.1.3.tar", last modified: Fri Apr 12 16:04:04 2024, max compression
```

## Comparing `cellfinder-1.1.2.tar` & `cellfinder-1.1.3.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.167877 cellfinder-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.151877 cellfinder-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.github/workflows/test_include_guard.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-05 10:44:05.000000 cellfinder-1.1.2/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-05 10:44:05.000000 cellfinder-1.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 10:44:05.000000 cellfinder-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-05 10:44:05.000000 cellfinder-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-05 10:44:13.167877 cellfinder-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-05 10:44:05.000000 cellfinder-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.155876 cellfinder-1.1.2/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/cli_migration_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/classify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/cube_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/classify/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/config/cellfinder.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/detect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/classical_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/plane_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/plane/tile_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/setup_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/ball_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/detect/filters/volume/volume_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.159876 cellfinder-1.1.2/cellfinder/core/download/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/download/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/core/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/array_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/source_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/core/train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/train/train_yml.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/curation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/detect/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/detect_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/detect/thread_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/images/brainglobe.png
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/input_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.163877 cellfinder-1.1.2/cellfinder/napari/train/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/train/train_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 10:44:05.000000 cellfinder-1.1.2/cellfinder/napari/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:44:13.167877 cellfinder-1.1.2/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-05 10:44:13.000000 cellfinder-1.1.2/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 10:44:12.000000 cellfinder-1.1.2/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-05 10:44:05.000000 cellfinder-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:44:13.167877 cellfinder-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.178807 cellfinder-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.162807 cellfinder-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.github/workflows/test_include_guard.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-12 16:03:57.000000 cellfinder-1.1.3/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-12 16:03:57.000000 cellfinder-1.1.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-12 16:03:57.000000 cellfinder-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 16:03:57.000000 cellfinder-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-12 16:04:04.178807 cellfinder-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 16:03:57.000000 cellfinder-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/cli_migration_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.166807 cellfinder-1.1.3/cellfinder/core/classify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/cube_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/classify/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/config/cellfinder.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/detect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/classical_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/plane_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/plane/tile_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/setup_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/ball_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/detect/filters/volume/volume_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.170807 cellfinder-1.1.3/cellfinder/core/download/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/download/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/core/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/array_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/source_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/core/train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/train/train_yml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21447 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/curation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/detect/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/detect_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/detect/thread_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21216 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/images/brainglobe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/input_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder/napari/train/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/train/train_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-12 16:03:57.000000 cellfinder-1.1.3/cellfinder/napari/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:04:04.174807 cellfinder-1.1.3/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-12 16:04:04.000000 cellfinder-1.1.3/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 16:04:03.000000 cellfinder-1.1.3/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-12 16:03:57.000000 cellfinder-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:04:04.178807 cellfinder-1.1.3/setup.cfg
```

### Comparing `cellfinder-1.1.2/.github/workflows/test_and_deploy.yml` & `cellfinder-1.1.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/.github/workflows/test_include_guard.yaml` & `cellfinder-1.1.3/.github/workflows/test_include_guard.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/.gitignore` & `cellfinder-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/CITATION.cff` & `cellfinder-1.1.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/LICENSE` & `cellfinder-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/PKG-INFO` & `cellfinder-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
```

### Comparing `cellfinder-1.1.2/README.md` & `cellfinder-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/__init__.py` & `cellfinder-1.1.3/cellfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/cli_migration_warning.py` & `cellfinder-1.1.3/cellfinder/cli_migration_warning.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/classify/augment.py` & `cellfinder-1.1.3/cellfinder/core/classify/augment.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/classify/classify.py` & `cellfinder-1.1.3/cellfinder/core/classify/classify.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/classify/cube_generator.py` & `cellfinder-1.1.3/cellfinder/core/classify/cube_generator.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/classify/resnet.py` & `cellfinder-1.1.3/cellfinder/core/classify/resnet.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/classify/tools.py` & `cellfinder-1.1.3/cellfinder/core/classify/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/detect.py` & `cellfinder-1.1.3/cellfinder/core/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/classical_filter.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/classical_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/plane_filter.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/plane_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/plane/tile_walker.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/plane/tile_walker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/setup_filters.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/setup_filters.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/ball_filter.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/ball_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_detection.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_detection.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/structure_splitting.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/structure_splitting.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/detect/filters/volume/volume_filter.py` & `cellfinder-1.1.3/cellfinder/core/detect/filters/volume/volume_filter.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/download/cli.py` & `cellfinder-1.1.3/cellfinder/core/download/cli.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/download/download.py` & `cellfinder-1.1.3/cellfinder/core/download/download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import shutil
 import tarfile
 import urllib.request
+from pathlib import Path
 
 from brainglobe_utils.general.config import get_config_obj
 from brainglobe_utils.general.system import disk_free_gb
 
 from cellfinder.core.tools.source_files import (
     default_configuration_path,
     user_specific_configuration_path,
@@ -120,9 +121,12 @@
 
     with open(orig_config, "r") as in_conf:
         data = in_conf.readlines()
     for i, line in enumerate(data):
         data[i] = line.replace(
             f"model_path = '{orig_path}", f"model_path = '{new_model_path}"
         )
+
+    custom_config_path = Path(custom_config)
+    custom_config_path.parent.mkdir(parents=True, exist_ok=True)
     with open(custom_config, "w") as out_conf:
         out_conf.writelines(data)
```

### Comparing `cellfinder-1.1.2/cellfinder/core/download/models.py` & `cellfinder-1.1.3/cellfinder/core/download/models.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/main.py` & `cellfinder-1.1.3/cellfinder/core/main.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/IO.py` & `cellfinder-1.1.3/cellfinder/core/tools/IO.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/array_operations.py` & `cellfinder-1.1.3/cellfinder/core/tools/array_operations.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/geometry.py` & `cellfinder-1.1.3/cellfinder/core/tools/geometry.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/image_processing.py` & `cellfinder-1.1.3/cellfinder/core/tools/image_processing.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/prep.py` & `cellfinder-1.1.3/cellfinder/core/tools/prep.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/source_files.py` & `cellfinder-1.1.3/cellfinder/core/tools/source_files.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/system.py` & `cellfinder-1.1.3/cellfinder/core/tools/system.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/tf.py` & `cellfinder-1.1.3/cellfinder/core/tools/tf.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/tiff.py` & `cellfinder-1.1.3/cellfinder/core/tools/tiff.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/tools/tools.py` & `cellfinder-1.1.3/cellfinder/core/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/core/train/train_yml.py` & `cellfinder-1.1.3/cellfinder/core/train/train_yml.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/curation.py` & `cellfinder-1.1.3/cellfinder/napari/curation.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/detect/detect.py` & `cellfinder-1.1.3/cellfinder/napari/detect/detect.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/detect/detect_containers.py` & `cellfinder-1.1.3/cellfinder/napari/detect/detect_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/detect/thread_worker.py` & `cellfinder-1.1.3/cellfinder/napari/detect/thread_worker.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/images/brainglobe.png` & `cellfinder-1.1.3/cellfinder/napari/images/brainglobe.png`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/input_container.py` & `cellfinder-1.1.3/cellfinder/napari/input_container.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/napari.yaml` & `cellfinder-1.1.3/cellfinder/napari/napari.yaml`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/sample_data.py` & `cellfinder-1.1.3/cellfinder/napari/sample_data.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/train/train.py` & `cellfinder-1.1.3/cellfinder/napari/train/train.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/train/train_containers.py` & `cellfinder-1.1.3/cellfinder/napari/train/train_containers.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder/napari/utils.py` & `cellfinder-1.1.3/cellfinder/napari/utils.py`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder.egg-info/PKG-INFO` & `cellfinder-1.1.3/cellfinder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 1.1.2
+Version: 1.1.3
 Summary: Automated 3D cell detection in large microscopy images
 Author-email: "Adam Tyson, Christian Niedworok, Charly Rousseau" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/documentation/cellfinder/index.html
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/cellfinder/index.html
```

### Comparing `cellfinder-1.1.2/cellfinder.egg-info/SOURCES.txt` & `cellfinder-1.1.3/cellfinder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/cellfinder.egg-info/requires.txt` & `cellfinder-1.1.3/cellfinder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `cellfinder-1.1.2/pyproject.toml` & `cellfinder-1.1.3/pyproject.toml`

 * *Files identical despite different names*

