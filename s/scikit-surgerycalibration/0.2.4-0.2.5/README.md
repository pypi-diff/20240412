# Comparing `tmp/scikit-surgerycalibration-0.2.4.tar.gz` & `tmp/scikit-surgerycalibration-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scikit-surgerycalibration-0.2.4.tar", last modified: Sat Feb 25 13:02:56 2023, max compression
+gzip compressed data, was "dist/scikit-surgerycalibration-0.2.5.tar", last modified: Fri Apr 12 20:33:32 2024, max compression
```

## Comparing `scikit-surgerycalibration-0.2.4.tar` & `scikit-surgerycalibration-0.2.5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/
--rwxr-xr-x   0 runner    (1001) docker     (123)      141 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/sphere_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/triangulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/pivot_calibration_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/pivot_calibration_command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/quaternion_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15486 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_cost_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)    22360 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_hand_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    20230 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41432 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/tests/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/tests/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/tests/algorithms/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/tests/algorithms/test_sphere_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-02-25 13:02:36.000000 scikit-surgerycalibration-0.2.4/tests/algorithms/test_triangulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/tests/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/ui/test_pivot_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 13:02:56.000000 scikit-surgerycalibration-0.2.4/tests/video/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_charuco_plus_chessboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_chessboard_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_data_param_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_hand_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)    13398 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_handeye_dots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_iterative.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_load_calib_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_precalib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/test_video_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/tests/video/video_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-02-25 13:02:44.000000 scikit-surgerycalibration-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      141 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11982 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/sphere_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12518 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/triangulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/pivot_calibration_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/pivot_calibration_command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/quaternion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_cost_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_mono.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_stereo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_hand_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25470 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20230 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41792 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/tests/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/tests/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/tests/algorithms/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/tests/algorithms/test_sphere_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-04-12 20:33:17.000000 scikit-surgerycalibration-0.2.5/tests/algorithms/test_triangulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/tests/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/ui/test_pivot_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:32.000000 scikit-surgerycalibration-0.2.5/tests/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_charuco_plus_chessboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9690 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_chessboard_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_data_param_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_hand_eye.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13454 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_handeye_dots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_load_calib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_precalib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/test_video_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/tests/video/video_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68611 2024-04-12 20:33:23.000000 scikit-surgerycalibration-0.2.5/versioneer.py
```

### Comparing `scikit-surgerycalibration-0.2.4/PKG-INFO` & `scikit-surgerycalibration-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgerycalibration
-Version: 0.2.4
+Version: 0.2.5
 Summary: scikit-surgerycalibration provides algorithms designed for the calibration of surgical instruments
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerycalibration 
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgerycalibration
         ===============================
```

### Comparing `scikit-surgerycalibration-0.2.4/README.rst` & `scikit-surgerycalibration-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/PKG-INFO` & `scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgerycalibration
-Version: 0.2.4
+Version: 0.2.5
 Summary: scikit-surgerycalibration provides algorithms designed for the calibration of surgical instruments
 Home-page: https://github.com/SciKit-Surgery/scikit-surgerycalibration 
 Author: Stephen Thompson
 Author-email: s.thompson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgerycalibration
         ===============================
```

### Comparing `scikit-surgerycalibration-0.2.4/scikit_surgerycalibration.egg-info/SOURCES.txt` & `scikit-surgerycalibration-0.2.5/scikit_surgerycalibration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/setup.py` & `scikit-surgerycalibration-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/pivot.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/pivot.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     for iter_counter in range(number_iterations):
         indexes = random.sample(population_of_indices,
                                 minimum_matrices_required)
         sample = tracking_matrices[indexes]
 
         try:
-            pointer_offset, pivot_location, _ = pivot_calibration(sample)
+            pointer_offset, pivot_location, _ = pivot_calibration_aos(sample)
         except ValueError:
             print("RANSAC, iteration " + str(iter_counter) + ", failed.")
             continue
 
         # Need to evaluate the number of inliers.
         # Slow, but it's written as a teaching exercise.
         number_of_inliers = 0
@@ -176,15 +176,15 @@
 
         # Keep the best model so far, based on the highest number of inliers.
         if percentage_inliers > concensus_threshold \
                 and number_of_inliers > highest_number_of_inliers:
             highest_number_of_inliers = number_of_inliers
             inlier_matrices = tracking_matrices[inlier_indices]
             best_pointer_offset, best_pivot_location, best_residual_error = \
-                pivot_calibration(inlier_matrices)
+                pivot_calibration_aos(inlier_matrices)
 
         # Early exit condition, as soon as we find model with enough fit.
         if percentage_inliers > concensus_threshold and early_exit:
             return best_pointer_offset, best_pivot_location, best_residual_error
 
     if best_pointer_offset is None:
         raise ValueError("Failed to find a model using RANSAC.")
```

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/sphere_fitting.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/sphere_fitting.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/algorithms/triangulate.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/algorithms/triangulate.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,34 +29,33 @@
 
     :return x_array:  [4x1] ndarray
     """
 
     # Build matrix A for homogeneous equation system Ax = 0
     # Assume X = (x,y,z,1), for Linear-LS method
     # Which turns it into a AX = B system, where A is 4x3, X is 3x1 and B is 4x1
-
     a_array = np.zeros((4, 3), dtype=np.double)
-    a_array[0, 0] = (u1_array[0] * p1_array[2, 0] - p1_array[0, 0]) / w1_const
-    a_array[0, 1] = (u1_array[0] * p1_array[2, 1] - p1_array[0, 1]) / w1_const
-    a_array[0, 2] = (u1_array[0] * p1_array[2, 2] - p1_array[0, 2]) / w1_const
-    a_array[1, 0] = (u1_array[1] * p1_array[2, 0] - p1_array[1, 0]) / w1_const
-    a_array[1, 1] = (u1_array[1] * p1_array[2, 1] - p1_array[1, 1]) / w1_const
-    a_array[1, 2] = (u1_array[1] * p1_array[2, 2] - p1_array[1, 2]) / w1_const
-    a_array[2, 0] = (u2_array[0] * p2_array[2, 0] - p2_array[0, 0]) / w2_const
-    a_array[2, 1] = (u2_array[0] * p2_array[2, 1] - p2_array[0, 1]) / w2_const
-    a_array[2, 2] = (u2_array[0] * p2_array[2, 2] - p2_array[0, 2]) / w2_const
-    a_array[3, 0] = (u2_array[1] * p2_array[2, 0] - p2_array[1, 0]) / w2_const
-    a_array[3, 1] = (u2_array[1] * p2_array[2, 1] - p2_array[1, 1]) / w2_const
-    a_array[3, 2] = (u2_array[1] * p2_array[2, 2] - p2_array[1, 2]) / w2_const
+    a_array[0, 0] = (u1_array[0][0] * p1_array[2, 0] - p1_array[0, 0]) / w1_const
+    a_array[0, 1] = (u1_array[0][0] * p1_array[2, 1] - p1_array[0, 1]) / w1_const
+    a_array[0, 2] = (u1_array[0][0] * p1_array[2, 2] - p1_array[0, 2]) / w1_const
+    a_array[1, 0] = (u1_array[1][0] * p1_array[2, 0] - p1_array[1, 0]) / w1_const
+    a_array[1, 1] = (u1_array[1][0] * p1_array[2, 1] - p1_array[1, 1]) / w1_const
+    a_array[1, 2] = (u1_array[1][0] * p1_array[2, 2] - p1_array[1, 2]) / w1_const
+    a_array[2, 0] = (u2_array[0][0] * p2_array[2, 0] - p2_array[0, 0]) / w2_const
+    a_array[2, 1] = (u2_array[0][0] * p2_array[2, 1] - p2_array[0, 1]) / w2_const
+    a_array[2, 2] = (u2_array[0][0] * p2_array[2, 2] - p2_array[0, 2]) / w2_const
+    a_array[3, 0] = (u2_array[1][0] * p2_array[2, 0] - p2_array[1, 0]) / w2_const
+    a_array[3, 1] = (u2_array[1][0] * p2_array[2, 1] - p2_array[1, 1]) / w2_const
+    a_array[3, 2] = (u2_array[1][0] * p2_array[2, 2] - p2_array[1, 2]) / w2_const
 
     b_array = np.zeros((4, 1), dtype=np.double)
-    b_array[0] = -(u1_array[0] * p1_array[2, 3] - p1_array[0, 3]) / w1_const
-    b_array[1] = -(u1_array[1] * p1_array[2, 3] - p1_array[1, 3]) / w1_const
-    b_array[2] = -(u2_array[0] * p2_array[2, 3] - p2_array[0, 3]) / w2_const
-    b_array[3] = -(u2_array[1] * p2_array[2, 3] - p2_array[1, 3]) / w2_const
+    b_array[0][0] = -(u1_array[0][0] * p1_array[2, 3] - p1_array[0, 3]) / w1_const
+    b_array[1][0] = -(u1_array[1][0] * p1_array[2, 3] - p1_array[1, 3]) / w1_const
+    b_array[2][0] = -(u2_array[0][0] * p2_array[2, 3] - p2_array[0, 3]) / w2_const
+    b_array[3][0] = -(u2_array[1][0] * p2_array[2, 3] - p2_array[1, 3]) / w2_const
 
     # start = time.time_ns()
     x_array = cv2.solve(a_array, b_array, flags=cv2.DECOMP_SVD)
     # x_array, _, _, _ = np.linalg.lstsq(a_array, b_array, rcond=-1) #Alternatively
     # print(f'{ time.time_ns() - start } nsecs')
 
     return x_array[1]  # for cv2.solve #x_array#for np.linalg.lstsq
@@ -85,31 +84,31 @@
     w2_const = 1
     x_array = np.zeros((4, 1), dtype=np.double)
     result = np.zeros((3, 1), dtype=np.double)
 
     # Hartley suggests 10 iterations at most
     for dummy_idx in range(10):
         x_array_ = _triangulate_point_using_svd(p1_array, p2_array, u1_array, u2_array, w1_const, w2_const)
-        x_array[0] = x_array_[0]
-        x_array[1] = x_array_[1]
-        x_array[2] = x_array_[2]
-        x_array[3] = 1.0
+        x_array[0][0] = x_array_[0][0]
+        x_array[1][0] = x_array_[1][0]
+        x_array[2][0] = x_array_[2][0]
+        x_array[3][0] = 1.0
 
         p2x1 = p1_array[2, :].dot(x_array)
         p2x2 = p2_array[2, :].dot(x_array)
         # p2x1 and p2x2 should not be zero to avoid RuntimeWarning: invalid value encountered in true_divide
         if (abs(w1_const - p2x1) <= epsilon and abs(w2_const - p2x2) <= epsilon):
             break
 
-        w1_const = p2x1
-        w2_const = p2x2
+        w1_const = p2x1[0]
+        w2_const = p2x2[0]
 
-    result[0] = x_array[0]
-    result[1] = x_array[1]
-    result[2] = x_array[2]
+    result[0][0] = x_array[0][0]
+    result[1][0] = x_array[1][0]
+    result[2][0] = x_array[2][0]
 
     return result
 
 
 def new_e2_array(e2_array, r2_array, left_to_right_trans_vector):
     """
 
@@ -118,18 +117,23 @@
 
     :param e2_array: [4x4] narray
     :param r2_array: = left_to_right_rotation_matrix: [3x3] narray
     :param left_to_right_trans_vector: [3x1] narray
 
     :return e2_array: [4x4] narray
     """
+    # While the specification is [3x1] which implies ndarray, the users
+    # may also pass in array (3,), ndarray (3, 1) or ndarray (1, 3).
+    # So, this will flatten all of them to the same array-like shape.
+    l_r = np.ravel(left_to_right_trans_vector)
+
     for row_idx in range(0, 3):
         for col_idx in range(0, 3):
             e2_array[row_idx, col_idx] = r2_array[row_idx, col_idx]
-        e2_array[row_idx, 3] = left_to_right_trans_vector[row_idx]
+        e2_array[row_idx, 3] = l_r[row_idx]
 
     return e2_array
 
 
 def l2r_to_p2d(p2d, l2r):
     """
 
@@ -227,17 +231,17 @@
         # Converting to normalised image points
         u1t = np.matmul(k1inv, u1_array)
         u2t = np.matmul(k2inv, u2_array)
 
         # array shapes for input args _iter_triangulate_point_w_svd( [3, 4]; [3, 4]; [3, 1]; [3, 1] )
         reconstructed_point = _iter_triangulate_point_w_svd(p1d, p2d, u1t, u2t)
 
-        output_points[dummy_index, 0] = reconstructed_point[0]
-        output_points[dummy_index, 1] = reconstructed_point[1]
-        output_points[dummy_index, 2] = reconstructed_point[2]
+        output_points[dummy_index, 0] = reconstructed_point[0][0]
+        output_points[dummy_index, 1] = reconstructed_point[1][0]
+        output_points[dummy_index, 2] = reconstructed_point[2][0]
 
     return output_points
 
 
 def triangulate_points_opencv(input_undistorted_points,
                               left_camera_intrinsic_params,
                               right_camera_intrinsic_params,
@@ -297,14 +301,14 @@
 
         # Converting to normalised image points
         u1t = np.matmul(k1inv, u1_array)
         u2t = np.matmul(k2inv, u2_array)
 
         # array shapes for input args cv2.triangulatePoints( [3, 4]; [3, 4]; [2, 1]; [2, 1] )
         reconstructed_point = cv2.triangulatePoints(p1mat, p2mat, u1t[:2], u2t[:2])
-        reconstructed_point /= reconstructed_point[3]  # Homogenize
+        reconstructed_point /= reconstructed_point[3][0]  # Homogenize
 
-        output_points[dummy_index, 0] = reconstructed_point[0]
-        output_points[dummy_index, 1] = reconstructed_point[1]
-        output_points[dummy_index, 2] = reconstructed_point[2]
+        output_points[dummy_index, 0] = reconstructed_point[0][0]
+        output_points[dummy_index, 1] = reconstructed_point[1][0]
+        output_points[dummy_index, 2] = reconstructed_point[2][0]
 
     return output_points
```

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/pivot_calibration_app.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/pivot_calibration_app.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/ui/pivot_calibration_command_line.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/ui/pivot_calibration_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/quaternion_utils.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/quaternion_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_cost_functions.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_cost_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,22 @@
     where we have a tracked calibration pattern, and assume the
     pattern2marker transform should remain fixed. Therefore we
     only optimise hand-eye. So, x_0 should be of length 6.
     """
     assert len(x_0) == 6
 
     rvec = np.zeros((3, 1))
-    rvec[0] = x_0[0]
-    rvec[1] = x_0[1]
-    rvec[2] = x_0[2]
+    rvec[0][0] = x_0[0]
+    rvec[1][0] = x_0[1]
+    rvec[2][0] = x_0[2]
 
     tvec = np.zeros((3, 1))
-    tvec[0] = x_0[3]
-    tvec[1] = x_0[4]
-    tvec[2] = x_0[5]
+    tvec[0][0] = x_0[3]
+    tvec[1][0] = x_0[4]
+    tvec[2][0] = x_0[5]
 
     h2e = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
     number_of_frames = len(object_points)
     rvecs = []
     tvecs = []
 
@@ -127,32 +127,32 @@
     where we have a tracked pattern. Both the
     pattern2marker and hand2eye are optimised.
     So, x_0 should be of length 12.
     """
     assert len(x_0) == 12
 
     rvec = np.zeros((3, 1))
-    rvec[0] = x_0[0]
-    rvec[1] = x_0[1]
-    rvec[2] = x_0[2]
+    rvec[0][0] = x_0[0]
+    rvec[1][0] = x_0[1]
+    rvec[2][0] = x_0[2]
 
     tvec = np.zeros((3, 1))
-    tvec[0] = x_0[3]
-    tvec[1] = x_0[4]
-    tvec[2] = x_0[5]
+    tvec[0][0] = x_0[3]
+    tvec[1][0] = x_0[4]
+    tvec[2][0] = x_0[5]
 
     p2m = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
-    rvec[0] = x_0[6]
-    rvec[1] = x_0[7]
-    rvec[2] = x_0[8]
-
-    tvec[0] = x_0[9]
-    tvec[1] = x_0[10]
-    tvec[2] = x_0[11]
+    rvec[0][0] = x_0[6]
+    rvec[1][0] = x_0[7]
+    rvec[2][0] = x_0[8]
+
+    tvec[0][0] = x_0[9]
+    tvec[1][0] = x_0[10]
+    tvec[2][0] = x_0[11]
 
     h2e = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
     number_of_frames = len(object_points)
     rvecs = []
     tvecs = []
 
@@ -190,32 +190,32 @@
     where we have an untracked pattern. Both the
     hand2eye and grid2world are optimised.
     So, x_0 should be of length 12.
     """
     assert len(x_0) == 12
 
     rvec = np.zeros((3, 1))
-    rvec[0] = x_0[0]
-    rvec[1] = x_0[1]
-    rvec[2] = x_0[2]
+    rvec[0][0] = x_0[0]
+    rvec[1][0] = x_0[1]
+    rvec[2][0] = x_0[2]
 
     tvec = np.zeros((3, 1))
-    tvec[0] = x_0[3]
-    tvec[1] = x_0[4]
-    tvec[2] = x_0[5]
+    tvec[0][0] = x_0[3]
+    tvec[1][0] = x_0[4]
+    tvec[2][0] = x_0[5]
 
     h2e = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
-    rvec[0] = x_0[6]
-    rvec[1] = x_0[7]
-    rvec[2] = x_0[8]
-
-    tvec[0] = x_0[9]
-    tvec[1] = x_0[10]
-    tvec[2] = x_0[11]
+    rvec[0][0] = x_0[6]
+    rvec[1][0] = x_0[7]
+    rvec[2][0] = x_0[8]
+
+    tvec[0][0] = x_0[9]
+    tvec[1][0] = x_0[10]
+    tvec[2][0] = x_0[11]
 
     g2w = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
     number_of_frames = len(object_points)
     rvecs = []
     tvecs = []
 
@@ -252,22 +252,22 @@
     where we have a tracked pattern. The handeye, intrinsics and
     distortion parameters are optimised.
     So, x_0 should be of length 6+4+5 = 15.
     """
     assert len(x_0) == 15
 
     rvec = np.zeros((3, 1))
-    rvec[0] = x_0[0]
-    rvec[1] = x_0[1]
-    rvec[2] = x_0[2]
+    rvec[0][0] = x_0[0]
+    rvec[1][0] = x_0[1]
+    rvec[2][0] = x_0[2]
 
     tvec = np.zeros((3, 1))
-    tvec[0] = x_0[3]
-    tvec[1] = x_0[4]
-    tvec[2] = x_0[5]
+    tvec[0][0] = x_0[3]
+    tvec[1][0] = x_0[4]
+    tvec[2][0] = x_0[5]
 
     h2e = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
     intrinsics = np.zeros((3, 3))
     intrinsics[0][0] = x_0[6]
     intrinsics[1][1] = x_0[7]
     intrinsics[0][2] = x_0[8]
```

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_data.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_data.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_base.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_base.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_mono.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_mono.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_driver_stereo.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_driver_stereo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_hand_eye.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_hand_eye.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_io.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_io.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_metrics.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_metrics.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_params.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_params.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_utils.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/sksurgerycalibration/video/video_calibration_wrapper.py` & `scikit-surgerycalibration-0.2.5/sksurgerycalibration/video/video_calibration_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,55 +155,55 @@
                     pattern_tracking_array,
                     method=cv2.CALIB_ROBOT_WORLD_HAND_EYE_SHAH
                     )
 
             # Now optimise p2m and h2e
             x_0 = np.zeros(12)
             rvec, tvec = vu.extrinsic_matrix_to_vecs(pattern2marker_matrix)
-            x_0[0] = rvec[0]
-            x_0[1] = rvec[1]
-            x_0[2] = rvec[2]
-            x_0[3] = tvec[0]
-            x_0[4] = tvec[1]
-            x_0[5] = tvec[2]
+            x_0[0] = rvec[0][0]
+            x_0[1] = rvec[1][0]
+            x_0[2] = rvec[2][0]
+            x_0[3] = tvec[0][0]
+            x_0[4] = tvec[1][0]
+            x_0[5] = tvec[2][0]
 
             rvec, tvec = vu.extrinsic_matrix_to_vecs(handeye_matrix)
-            x_0[6] = rvec[0]
-            x_0[7] = rvec[1]
-            x_0[8] = rvec[2]
-            x_0[9] = tvec[0]
-            x_0[10] = tvec[1]
-            x_0[11] = tvec[2]
+            x_0[6] = rvec[0][0]
+            x_0[7] = rvec[1][0]
+            x_0[8] = rvec[2][0]
+            x_0[9] = tvec[0][0]
+            x_0[10] = tvec[1][0]
+            x_0[11] = tvec[2][0]
 
             res = minimize(vcf.mono_proj_err_p2m_h2e, x_0,
                            args=(object_points,
                                  image_points,
                                  camera_matrix,
                                  camera_distortion,
                                  pattern_tracking_array,
                                  device_tracking_array
                                  ),
                            method='Powell',
                            )
 
             x_1 = res.x
-            rvec[0] = x_1[0]
-            rvec[1] = x_1[1]
-            rvec[2] = x_1[2]
-            tvec[0] = x_1[3]
-            tvec[1] = x_1[4]
-            tvec[2] = x_1[5]
+            rvec[0][0] = x_1[0]
+            rvec[1][0] = x_1[1]
+            rvec[2][0] = x_1[2]
+            tvec[0][0] = x_1[3]
+            tvec[1][0] = x_1[4]
+            tvec[2][0] = x_1[5]
             pattern2marker_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
-            rvec[0] = x_1[6]
-            rvec[1] = x_1[7]
-            rvec[2] = x_1[8]
-            tvec[0] = x_1[9]
-            tvec[1] = x_1[10]
-            tvec[2] = x_1[11]
+            rvec[0][0] = x_1[6]
+            rvec[1][0] = x_1[7]
+            rvec[2][0] = x_1[8]
+            tvec[0][0] = x_1[9]
+            tvec[1][0] = x_1[10]
+            tvec[2][0] = x_1[11]
             handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
         elif pattern2marker_matrix is not None \
                 and len(pattern_tracking_array) > 3 \
                 and pattern_tracking_array[0] is not None:
 
             handeye_matrix, _ = \
@@ -214,40 +214,40 @@
                     pattern_tracking_array,
                     method=cv2.CALIB_ROBOT_WORLD_HAND_EYE_SHAH
                     )
 
             # Now optimise just the h2e
             x_0 = np.zeros(6)
             rvec, tvec = vu.extrinsic_matrix_to_vecs(handeye_matrix)
-            x_0[0] = rvec[0]
-            x_0[1] = rvec[1]
-            x_0[2] = rvec[2]
-            x_0[3] = tvec[0]
-            x_0[4] = tvec[1]
-            x_0[5] = tvec[2]
+            x_0[0] = rvec[0][0]
+            x_0[1] = rvec[1][0]
+            x_0[2] = rvec[2][0]
+            x_0[3] = tvec[0][0]
+            x_0[4] = tvec[1][0]
+            x_0[5] = tvec[2][0]
 
             res = minimize(vcf.mono_proj_err_h2e, x_0,
                            args=(object_points,
                                  image_points,
                                  camera_matrix,
                                  camera_distortion,
                                  pattern_tracking_array,
                                  device_tracking_array,
                                  pattern2marker_matrix
                                  ),
                            method='Powell',
                            )
 
             x_1 = res.x
-            rvec[0] = x_1[0]
-            rvec[1] = x_1[1]
-            rvec[2] = x_1[2]
-            tvec[0] = x_1[3]
-            tvec[1] = x_1[4]
-            tvec[2] = x_1[5]
+            rvec[0][0] = x_1[0]
+            rvec[1][0] = x_1[1]
+            rvec[2][0] = x_1[2]
+            tvec[0][0] = x_1[3]
+            tvec[1][0] = x_1[4]
+            tvec[2][0] = x_1[5]
             handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
         else:
 
             handeye_matrix = \
                 he.calibrate_hand_eye_using_stationary_pattern(
                     rvecs,
@@ -258,20 +258,20 @@
     if do_bundle_adjust \
             and len(pattern_tracking_array) > 3 \
             and pattern_tracking_array[0] is not None:
 
         # Now optimise h2e, intrinsics, distortion
         x_0 = np.zeros(15)
         rvec, tvec = vu.extrinsic_matrix_to_vecs(handeye_matrix)
-        x_0[0] = rvec[0]
-        x_0[1] = rvec[1]
-        x_0[2] = rvec[2]
-        x_0[3] = tvec[0]
-        x_0[4] = tvec[1]
-        x_0[5] = tvec[2]
+        x_0[0] = rvec[0][0]
+        x_0[1] = rvec[1][0]
+        x_0[2] = rvec[2][0]
+        x_0[3] = tvec[0][0]
+        x_0[4] = tvec[1][0]
+        x_0[5] = tvec[2][0]
         x_0[6] = camera_matrix[0][0]
         x_0[7] = camera_matrix[1][1]
         x_0[8] = camera_matrix[0][2]
         x_0[9] = camera_matrix[1][2]
         x_0[10] = camera_distortion[0][0]
         x_0[11] = camera_distortion[0][1]
         x_0[12] = camera_distortion[0][2]
@@ -284,20 +284,20 @@
                              device_tracking_array,
                              pattern_tracking_array,
                              pattern2marker_matrix
                              ),
                        method='Powell',
                        )
         x_1 = res.x
-        rvec[0] = x_1[0]
-        rvec[1] = x_1[1]
-        rvec[2] = x_1[2]
-        tvec[0] = x_1[3]
-        tvec[1] = x_1[4]
-        tvec[2] = x_1[5]
+        rvec[0][0] = x_1[0]
+        rvec[1][0] = x_1[1]
+        rvec[2][0] = x_1[2]
+        tvec[0][0] = x_1[3]
+        tvec[1][0] = x_1[4]
+        tvec[2][0] = x_1[5]
         handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
         camera_matrix[0][0] = x_1[6]
         camera_matrix[1][1] = x_1[7]
         camera_matrix[0][2] = x_1[8]
         camera_matrix[1][2] = x_1[9]
         camera_distortion[0][0] = x_1[10]
@@ -699,28 +699,28 @@
                 and len(calibration_tracking_array) > 3 \
                 and calibration_tracking_array[0] is not None:
 
             # Now optimise p2m and h2e
             x_0 = np.zeros(12)
 
             rvec, tvec = vu.extrinsic_matrix_to_vecs(left_handeye_matrix)
-            x_0[0] = rvec[0]
-            x_0[1] = rvec[1]
-            x_0[2] = rvec[2]
-            x_0[3] = tvec[0]
-            x_0[4] = tvec[1]
-            x_0[5] = tvec[2]
+            x_0[0] = rvec[0][0]
+            x_0[1] = rvec[1][0]
+            x_0[2] = rvec[2][0]
+            x_0[3] = tvec[0][0]
+            x_0[4] = tvec[1][0]
+            x_0[5] = tvec[2][0]
 
             rvec, tvec = vu.extrinsic_matrix_to_vecs(left_pattern2marker_matrix)
-            x_0[6] = rvec[0]
-            x_0[7] = rvec[1]
-            x_0[8] = rvec[2]
-            x_0[9] = tvec[0]
-            x_0[10] = tvec[1]
-            x_0[11] = tvec[2]
+            x_0[6] = rvec[0][0]
+            x_0[7] = rvec[1][0]
+            x_0[8] = rvec[2][0]
+            x_0[9] = tvec[0][0]
+            x_0[10] = tvec[1][0]
+            x_0[11] = tvec[2][0]
 
             res = minimize(vcf.stereo_proj_err_h2e, x_0,
                            args=(common_object_pts,
                                  common_l_image_pts,
                                  common_r_image_pts,
                                  left_camera_matrix,
                                  left_camera_distortion,
@@ -739,43 +739,43 @@
             LOGGER.info("Stereo Handeye Re-Optimised p2m and h2e: success=%s",
                         str(res.success))
             LOGGER.info("Stereo Handeye Re-Optimised p2m and h2e: msg=%s",
                         str(res.message))
 
             x_1 = res.x
 
-            rvec[0] = x_1[0]
-            rvec[1] = x_1[1]
-            rvec[2] = x_1[2]
-            tvec[0] = x_1[3]
-            tvec[1] = x_1[4]
-            tvec[2] = x_1[5]
+            rvec[0][0] = x_1[0]
+            rvec[1][0] = x_1[1]
+            rvec[2][0] = x_1[2]
+            tvec[0][0] = x_1[3]
+            tvec[1][0] = x_1[4]
+            tvec[2][0] = x_1[5]
             left_handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
-            rvec[0] = x_1[6]
-            rvec[1] = x_1[7]
-            rvec[2] = x_1[8]
-            tvec[0] = x_1[9]
-            tvec[1] = x_1[10]
-            tvec[2] = x_1[11]
+            rvec[0][0] = x_1[6]
+            rvec[1][0] = x_1[7]
+            rvec[2][0] = x_1[8]
+            tvec[0][0] = x_1[9]
+            tvec[1][0] = x_1[10]
+            tvec[2][0] = x_1[11]
             left_pattern2marker_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
         elif override_pattern2marker is not None \
                 and len(calibration_tracking_array) > 3 \
                 and calibration_tracking_array[0] is not None:
 
             # Now optimise just the h2e
             x_0 = np.zeros(6)
             rvec, tvec = vu.extrinsic_matrix_to_vecs(left_handeye_matrix)
-            x_0[0] = rvec[0]
-            x_0[1] = rvec[1]
-            x_0[2] = rvec[2]
-            x_0[3] = tvec[0]
-            x_0[4] = tvec[1]
-            x_0[5] = tvec[2]
+            x_0[0] = rvec[0][0]
+            x_0[1] = rvec[1][0]
+            x_0[2] = rvec[2][0]
+            x_0[3] = tvec[0][0]
+            x_0[4] = tvec[1][0]
+            x_0[5] = tvec[2][0]
 
             res = minimize(vcf.stereo_proj_err_h2e, x_0,
                            args=(common_object_pts,
                                  common_l_image_pts,
                                  common_r_image_pts,
                                  left_camera_matrix,
                                  left_camera_distortion,
@@ -793,45 +793,45 @@
                         str(res.status))
             LOGGER.info("Stereo Handeye Re-Optimised h2e: success=%s",
                         str(res.success))
             LOGGER.info("Stereo Handeye Re-Optimised h2e: msg=%s",
                         str(res.message))
 
             x_1 = res.x
-            rvec[0] = x_1[0]
-            rvec[1] = x_1[1]
-            rvec[2] = x_1[2]
-            tvec[0] = x_1[3]
-            tvec[1] = x_1[4]
-            tvec[2] = x_1[5]
+            rvec[0][0] = x_1[0]
+            rvec[1][0] = x_1[1]
+            rvec[2][0] = x_1[2]
+            tvec[0][0] = x_1[3]
+            tvec[1][0] = x_1[4]
+            tvec[2][0] = x_1[5]
             left_handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
         # Now, final case, optimise handeye and stereo camera parameters.
         # This means hand-eye (6DOF), left intrinsics (4DOF), left
         # distortion (5DOF), right intrinsics (4DOF), right distortion (5DOF),
         # l2r (6DOF) = 30 DOF.
 
         x_0 = np.zeros(30)
 
         rvec, tvec = vu.extrinsic_matrix_to_vecs(left_handeye_matrix)
-        x_0[0] = rvec[0]
-        x_0[1] = rvec[1]
-        x_0[2] = rvec[2]
-        x_0[3] = tvec[0]
-        x_0[4] = tvec[1]
-        x_0[5] = tvec[2]
+        x_0[0] = rvec[0][0]
+        x_0[1] = rvec[1][0]
+        x_0[2] = rvec[2][0]
+        x_0[3] = tvec[0][0]
+        x_0[4] = tvec[1][0]
+        x_0[5] = tvec[2][0]
 
         l2r = skcm.construct_rigid_transformation(l2r_rmat, l2r_tvec)
         rvec, tvec = vu.extrinsic_matrix_to_vecs(l2r)
-        x_0[6] = rvec[0]
-        x_0[7] = rvec[1]
-        x_0[8] = rvec[2]
-        x_0[9] = tvec[0]
-        x_0[10] = tvec[1]
-        x_0[11] = tvec[2]
+        x_0[6] = rvec[0][0]
+        x_0[7] = rvec[1][0]
+        x_0[8] = rvec[2][0]
+        x_0[9] = tvec[0][0]
+        x_0[10] = tvec[1][0]
+        x_0[11] = tvec[2][0]
 
         x_0[12] = left_camera_matrix[0][0]
         x_0[13] = left_camera_matrix[1][1]
         x_0[14] = left_camera_matrix[0][2]
         x_0[15] = left_camera_matrix[1][2]
         x_0[16] = left_camera_distortion[0][0]
         x_0[17] = left_camera_distortion[0][1]
@@ -863,28 +863,28 @@
                     str(res.status))
         LOGGER.info("Stereo Handeye bundle adjustment: success=%s",
                     str(res.success))
         LOGGER.info("Stereo Handeye bundle adjustment: msg=%s",
                     str(res.message))
 
         x_1 = res.x
-        rvec[0] = x_1[0]
-        rvec[1] = x_1[1]
-        rvec[2] = x_1[2]
-        tvec[0] = x_1[3]
-        tvec[1] = x_1[4]
-        tvec[2] = x_1[5]
+        rvec[0][0] = x_1[0]
+        rvec[1][0] = x_1[1]
+        rvec[2][0] = x_1[2]
+        tvec[0][0] = x_1[3]
+        tvec[1][0] = x_1[4]
+        tvec[2][0] = x_1[5]
         left_handeye_matrix = vu.extrinsic_vecs_to_matrix(rvec, tvec)
 
-        rvec[0] = x_1[6]
-        rvec[1] = x_1[7]
-        rvec[2] = x_1[8]
-        tvec[0] = x_1[9]
-        tvec[1] = x_1[10]
-        tvec[2] = x_1[11]
+        rvec[0][0] = x_1[6]
+        rvec[1][0] = x_1[7]
+        rvec[2][0] = x_1[8]
+        tvec[0][0] = x_1[9]
+        tvec[1][0] = x_1[10]
+        tvec[2][0] = x_1[11]
         l2r = vu.extrinsic_vecs_to_matrix(rvec, tvec)
         l2r_rmat = l2r[0:3, 0:3]
         l2r_tvec = l2r[0:3, 3]
 
         left_camera_matrix[0][0] = x_1[12]
         left_camera_matrix[1][1] = x_1[13]
         left_camera_matrix[0][2] = x_1[14]
@@ -1004,20 +1004,20 @@
     Simply re-optimises the extrinsic parameters.
     :return: error, l_rvecs, l_tvecs
     """
     number_of_frames = len(common_object_points)
     number_of_parameters = 6 * number_of_frames
     x_0 = np.zeros(number_of_parameters)
     for i in range(0, number_of_frames):
-        x_0[i * 6 + 0] = l_rvecs[i][0]
-        x_0[i * 6 + 1] = l_rvecs[i][1]
-        x_0[i * 6 + 2] = l_rvecs[i][2]
-        x_0[i * 6 + 3] = l_tvecs[i][0]
-        x_0[i * 6 + 4] = l_tvecs[i][1]
-        x_0[i * 6 + 5] = l_tvecs[i][2]
+        x_0[i * 6 + 0] = l_rvecs[i][0][0]
+        x_0[i * 6 + 1] = l_rvecs[i][1][0]
+        x_0[i * 6 + 2] = l_rvecs[i][2][0]
+        x_0[i * 6 + 3] = l_tvecs[i][0][0]
+        x_0[i * 6 + 4] = l_tvecs[i][1][0]
+        x_0[i * 6 + 5] = l_tvecs[i][2][0]
 
     res = least_squares(vcf.stereo_2d_error_for_extrinsics, x_0,
                         args=(common_object_points,
                               common_left_image_points,
                               common_right_image_points,
                               override_left_intrinsics,
                               override_left_distortion,
@@ -1031,15 +1031,15 @@
 
     LOGGER.info("Stereo Re-Calibration: status=%s", str(res.status))
     LOGGER.info("Stereo Re-Calibration: success=%s", str(res.success))
     LOGGER.info("Stereo Re-Calibration: msg=%s", str(res.message))
 
     x_1 = res.x
     for i in range(0, number_of_frames):
-        l_rvecs[i][0] = x_1[i * 6 + 0]
-        l_rvecs[i][1] = x_1[i * 6 + 1]
-        l_rvecs[i][2] = x_1[i * 6 + 2]
-        l_tvecs[i][0] = x_1[i * 6 + 3]
-        l_tvecs[i][1] = x_1[i * 6 + 4]
-        l_tvecs[i][2] = x_1[i * 6 + 5]
+        l_rvecs[i][0][0] = x_1[i * 6 + 0]
+        l_rvecs[i][1][0] = x_1[i * 6 + 1]
+        l_rvecs[i][2][0] = x_1[i * 6 + 2]
+        l_tvecs[i][0][0] = x_1[i * 6 + 3]
+        l_tvecs[i][1][0] = x_1[i * 6 + 4]
+        l_tvecs[i][2][0] = x_1[i * 6 + 5]
 
     return res.fun, l_rvecs, l_tvecs
```

### Comparing `scikit-surgerycalibration-0.2.4/tests/algorithms/test_pivot.py` & `scikit-surgerycalibration-0.2.5/tests/algorithms/test_pivot.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/algorithms/test_sphere_fitting.py` & `scikit-surgerycalibration-0.2.5/tests/algorithms/test_sphere_fitting.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/algorithms/test_triangulate.py` & `scikit-surgerycalibration-0.2.5/tests/algorithms/test_triangulate.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_charuco_plus_chessboard.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_charuco_plus_chessboard.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_chessboard_calibration.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_chessboard_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_data_param_io.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_data_param_io.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_hand_eye.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_hand_eye.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_handeye_dots.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_handeye_dots.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                                            threshold_offset=threshold_offset
                                            )
 
     calibration_driver = sc.StereoVideoCalibrationDriver(left_pd,
                                                          right_pd,
                                                          minimum_points_per_frame)
 
-    for i in range(10):
+    for i in range(0,10,2): #issue 59, reduced number of frames used for test
         l_img, r_img, chessboard, scope = lcu.get_calib_data(calib_dir, i)
         num_points = calibration_driver.grab_data(l_img, r_img, scope, chessboard)
         print("Grabbed " + str(num_points) + " points")
 
     return calibration_driver
 
 
@@ -263,15 +263,15 @@
 
     # Projection error < 4, should be ok for a stereo laparoscope
     assert results_no_p2m_m[0] < 4
     assert results_with_p2m_m[0] < 4
 
     # Reconstruction error < 1mm
     assert results_no_p2m_m[1] < 1
-    assert results_with_p2m_m[1] < 1
+    assert results_with_p2m_m[1] < 1.2
 
 
 def test_tracked_vs_stationary():
     """
     Mainly to check code runs, as we don't yet have functional requirements.
     Unfortunately, below, the stationary pattern calibrations fail.
     I suspect there was not enough movement of the laparoscope.
```

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_iterative.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_iterative.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_load_calib_utils.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_load_calib_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_precalib.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_precalib.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/test_video_calibration.py` & `scikit-surgerycalibration-0.2.5/tests/video/test_video_calibration.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/tests/video/video_testing_utils.py` & `scikit-surgerycalibration-0.2.5/tests/video/video_testing_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgerycalibration-0.2.4/versioneer.py` & `scikit-surgerycalibration-0.2.5/versioneer.py`

 * *Files identical despite different names*

