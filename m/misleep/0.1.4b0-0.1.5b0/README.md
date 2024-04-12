# Comparing `tmp/misleep-0.1.4b0.tar.gz` & `tmp/misleep-0.1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misleep-0.1.4b0.tar", last modified: Wed Apr 10 11:16:59 2024, max compression
+gzip compressed data, was "misleep-0.1.5b0.tar", last modified: Fri Apr 12 08:03:00 2024, max compression
```

## Comparing `misleep-0.1.4b0.tar` & `misleep-0.1.5b0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.126028 misleep-0.1.4b0/
--rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.4b0/LICENSE
--rw-rw-rw-   0        0        0     2920 2024-04-10 11:16:59.125028 misleep-0.1.4b0/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2024-04-10 04:00:34.000000 misleep-0.1.4b0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.104028 misleep-0.1.4b0/misleep/
--rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.4b0/misleep/__init__.py
--rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.4b0/misleep/__main__.py
--rw-rw-rw-   0        0        0      508 2024-04-10 11:13:16.000000 misleep-0.1.4b0/misleep/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.109028 misleep-0.1.4b0/misleep/gui/
--rw-rw-rw-   0        0        0      340 2024-04-02 09:30:59.000000 misleep-0.1.4b0/misleep/gui/__init__.py
--rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.4b0/misleep/gui/about.py
--rw-rw-rw-   0        0        0     4633 2024-04-02 07:00:24.000000 misleep-0.1.4b0/misleep/gui/label_dialog.py
--rw-rw-rw-   0        0        0    53637 2024-04-10 11:12:01.000000 misleep-0.1.4b0/misleep/gui/main_window.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.111028 misleep-0.1.4b0/misleep/gui/resources/
--rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.4b0/misleep/gui/resources/__init__.py
--rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/gui/resources/entire_logo.png
--rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/gui/resources/logo.png
--rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.4b0/misleep/gui/resources/misleep.py
--rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/gui/resources/misleep.qrc
--rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.4b0/misleep/gui/show.py
--rw-rw-rw-   0        0        0     5893 2024-04-08 05:54:04.000000 misleep-0.1.4b0/misleep/gui/spec_window.py
--rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.4b0/misleep/gui/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.114028 misleep-0.1.4b0/misleep/gui/uis/
--rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/gui/uis/__init__.py
--rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/gui/uis/about_ui.py
--rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.4b0/misleep/gui/uis/label_dialog_ui.py
--rw-rw-rw-   0        0        0    23842 2024-04-08 05:30:54.000000 misleep-0.1.4b0/misleep/gui/uis/main_window_ui.py
--rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.4b0/misleep/gui/uis/spec_window_ui.py
--rw-rw-rw-   0        0        0      757 2024-04-02 06:53:09.000000 misleep-0.1.4b0/misleep/gui/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.116028 misleep-0.1.4b0/misleep/io/
--rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.4b0/misleep/io/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/io/annotation_io.py
--rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.4b0/misleep/io/base.py
--rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.4b0/misleep/io/signal_io.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.117028 misleep-0.1.4b0/misleep/preprocessing/
--rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.4b0/misleep/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.4b0/misleep/preprocessing/channel.py
--rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.4b0/misleep/preprocessing/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.120028 misleep-0.1.4b0/misleep/utils/
--rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.4b0/misleep/utils/__init__.py
--rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.4b0/misleep/utils/annotation.py
--rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/utils/only4gui.py
--rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.4b0/misleep/utils/others.py
--rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/utils/signals.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.122028 misleep-0.1.4b0/misleep/viz/
--rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.4b0/misleep/viz/__init__.py
--rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.4b0/misleep/viz/hypnogram.py
--rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.4b0/misleep/viz/signals.py
--rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.4b0/misleep/viz/spectral.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.106028 misleep-0.1.4b0/misleep.egg-info/
--rw-rw-rw-   0        0        0     2920 2024-04-10 11:16:59.000000 misleep-0.1.4b0/misleep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1340 2024-04-10 11:16:59.000000 misleep-0.1.4b0/misleep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 11:16:59.000000 misleep-0.1.4b0/misleep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-10 11:16:59.000000 misleep-0.1.4b0/misleep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 11:16:59.000000 misleep-0.1.4b0/misleep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 11:16:59.126028 misleep-0.1.4b0/setup.cfg
--rw-rw-rw-   0        0        0     2125 2024-04-10 11:13:05.000000 misleep-0.1.4b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 11:16:59.125028 misleep-0.1.4b0/test/
--rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.4b0/test/test_annotation_io.py
--rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.4b0/test/test_loadmat73.py
--rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.4b0/test/test_midata.py
--rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.4b0/test/test_show.py
--rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.4b0/test/test_signal_io.py
--rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.4b0/test/test_signals_viz.py
--rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.4b0/test/test_spectral_viz.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.909968 misleep-0.1.5b0/
+-rw-rw-rw-   0        0        0     1549 2024-03-05 06:19:17.000000 misleep-0.1.5b0/LICENSE
+-rw-rw-rw-   0        0        0     2968 2024-04-12 08:03:00.908969 misleep-0.1.5b0/PKG-INFO
+-rw-rw-rw-   0        0        0     1870 2024-04-10 04:00:34.000000 misleep-0.1.5b0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.885968 misleep-0.1.5b0/misleep/
+-rw-rw-rw-   0        0        0      215 2024-03-27 05:19:22.000000 misleep-0.1.5b0/misleep/__init__.py
+-rw-rw-rw-   0        0        0      167 2024-04-02 10:19:29.000000 misleep-0.1.5b0/misleep/__main__.py
+-rw-rw-rw-   0        0        0      532 2024-04-12 08:02:53.000000 misleep-0.1.5b0/misleep/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.891968 misleep-0.1.5b0/misleep/gui/
+-rw-rw-rw-   0        0        0      334 2024-04-12 06:13:32.000000 misleep-0.1.5b0/misleep/gui/__init__.py
+-rw-rw-rw-   0        0        0      808 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/gui/about.py
+-rw-rw-rw-   0        0        0    10976 2024-04-12 06:57:35.000000 misleep-0.1.5b0/misleep/gui/dialog.py
+-rw-rw-rw-   0        0        0    55821 2024-04-12 08:01:54.000000 misleep-0.1.5b0/misleep/gui/main_window.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.893968 misleep-0.1.5b0/misleep/gui/resources/
+-rw-rw-rw-   0        0        0       47 2024-04-02 09:32:49.000000 misleep-0.1.5b0/misleep/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0     9826 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/entire_logo.png
+-rw-rw-rw-   0        0        0     2670 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/logo.png
+-rw-rw-rw-   0        0        0    54154 2024-04-02 09:29:51.000000 misleep-0.1.5b0/misleep/gui/resources/misleep.py
+-rw-rw-rw-   0        0        0      121 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/resources/misleep.qrc
+-rw-rw-rw-   0        0        0      473 2024-04-08 05:55:10.000000 misleep-0.1.5b0/misleep/gui/show.py
+-rw-rw-rw-   0        0        0     5893 2024-04-12 06:40:33.000000 misleep-0.1.5b0/misleep/gui/spec_window.py
+-rw-rw-rw-   0        0        0     3177 2024-04-03 08:49:26.000000 misleep-0.1.5b0/misleep/gui/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.896969 misleep-0.1.5b0/misleep/gui/uis/
+-rw-rw-rw-   0        0        0      228 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/uis/__init__.py
+-rw-rw-rw-   0        0        0     2921 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/gui/uis/about_ui.py
+-rw-rw-rw-   0        0        0     2207 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/gui/uis/label_dialog_ui.py
+-rw-rw-rw-   0        0        0    24854 2024-04-12 06:48:24.000000 misleep-0.1.5b0/misleep/gui/uis/main_window_ui.py
+-rw-rw-rw-   0        0        0     4466 2024-04-08 05:30:56.000000 misleep-0.1.5b0/misleep/gui/uis/spec_window_ui.py
+-rw-rw-rw-   0        0        0     3048 2024-04-12 06:16:09.000000 misleep-0.1.5b0/misleep/gui/uis/transfer_result_dialog_ui.py
+-rw-rw-rw-   0        0        0     3441 2024-04-12 06:27:56.000000 misleep-0.1.5b0/misleep/gui/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.898969 misleep-0.1.5b0/misleep/io/
+-rw-rw-rw-   0        0        0      215 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/io/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/io/annotation_io.py
+-rw-rw-rw-   0        0        0    14995 2024-04-03 08:28:39.000000 misleep-0.1.5b0/misleep/io/base.py
+-rw-rw-rw-   0        0        0     4431 2024-04-08 12:27:01.000000 misleep-0.1.5b0/misleep/io/signal_io.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.900969 misleep-0.1.5b0/misleep/preprocessing/
+-rw-rw-rw-   0        0        0      163 2024-03-05 07:42:23.000000 misleep-0.1.5b0/misleep/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      338 2024-03-05 07:42:23.000000 misleep-0.1.5b0/misleep/preprocessing/channel.py
+-rw-rw-rw-   0        0        0     4898 2024-03-31 07:18:43.000000 misleep-0.1.5b0/misleep/preprocessing/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.903969 misleep-0.1.5b0/misleep/utils/
+-rw-rw-rw-   0        0        0      187 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/utils/__init__.py
+-rw-rw-rw-   0        0        0     1692 2024-04-02 07:16:03.000000 misleep-0.1.5b0/misleep/utils/annotation.py
+-rw-rw-rw-   0        0        0     2050 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/utils/only4gui.py
+-rw-rw-rw-   0        0        0        0 2024-04-01 05:02:43.000000 misleep-0.1.5b0/misleep/utils/others.py
+-rw-rw-rw-   0        0        0     2324 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/utils/signals.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.905968 misleep-0.1.5b0/misleep/viz/
+-rw-rw-rw-   0        0        0      211 2024-03-06 08:30:45.000000 misleep-0.1.5b0/misleep/viz/__init__.py
+-rw-rw-rw-   0        0        0     1164 2024-03-07 13:29:48.000000 misleep-0.1.5b0/misleep/viz/hypnogram.py
+-rw-rw-rw-   0        0        0     1668 2024-03-07 13:29:48.000000 misleep-0.1.5b0/misleep/viz/signals.py
+-rw-rw-rw-   0        0        0     1508 2024-03-13 06:17:48.000000 misleep-0.1.5b0/misleep/viz/spectral.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.887968 misleep-0.1.5b0/misleep.egg-info/
+-rw-rw-rw-   0        0        0     2968 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1379 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 08:03:00.000000 misleep-0.1.5b0/misleep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:03:00.909968 misleep-0.1.5b0/setup.cfg
+-rw-rw-rw-   0        0        0     2157 2024-04-12 08:02:06.000000 misleep-0.1.5b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:03:00.908969 misleep-0.1.5b0/test/
+-rw-rw-rw-   0        0        0      473 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_annotation_io.py
+-rw-rw-rw-   0        0        0      143 2024-04-03 07:20:46.000000 misleep-0.1.5b0/test/test_loadmat73.py
+-rw-rw-rw-   0        0        0     1828 2024-03-13 06:17:48.000000 misleep-0.1.5b0/test/test_midata.py
+-rw-rw-rw-   0        0        0      275 2024-03-28 08:11:15.000000 misleep-0.1.5b0/test/test_show.py
+-rw-rw-rw-   0        0        0     1376 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_signal_io.py
+-rw-rw-rw-   0        0        0      603 2024-03-07 13:29:48.000000 misleep-0.1.5b0/test/test_signals_viz.py
+-rw-rw-rw-   0        0        0     1253 2024-03-06 08:30:45.000000 misleep-0.1.5b0/test/test_spectral_viz.py
```

### Comparing `misleep-0.1.4b0/LICENSE` & `misleep-0.1.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/PKG-INFO` & `misleep-0.1.5b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.4b0
+Version: 0.1.5b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -23,14 +23,16 @@
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
 Requires-Dist: mat73
+Requires-Dist: pandas
+Requires-Dist: openpyxl
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
```

### Comparing `misleep-0.1.4b0/README.md` & `misleep-0.1.5b0/README.md`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/about.py` & `misleep-0.1.5b0/misleep/gui/about.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/main_window.py` & `misleep-0.1.5b0/misleep/gui/main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from misleep.preprocessing.spectral import spectrogram
 from misleep.io.base import MiData, MiAnnotation
 from misleep.io.signal_io import load_mat, load_edf
 from misleep.io.annotation_io import load_misleep_anno
 from misleep.gui.utils import create_new_mianno
 from misleep.utils.annotation import lst2group
 from misleep.gui.about import about_dialog
-from misleep.gui.label_dialog import label_dialog
+from misleep.gui.dialog import label_dialog, transferResult_dialog
 from misleep.gui.spec_window import SpecWindow
 from misleep.gui.uis.main_window_ui import Ui_MiSleep
 from misleep.preprocessing.spectral import spectrogram, spectrum, band_power
 from misleep.gui.thread import SaveThread
 
 
 class main_window(QMainWindow, Ui_MiSleep):
@@ -114,14 +114,17 @@
         # Initial about dialog and spec window
         self.about_dialog = about_dialog(version=self.config['gui']['version'],
                                          update_time=self.config['gui']['updatetime'])
         self.spec_window = SpecWindow()
         # Initial label dialog
         self.label_dialog = label_dialog(config=self.config)
 
+        # Initial transfer result dialog
+        self.transfer_result_dialog = transferResult_dialog()
+
         # Check wheher operation done and saved or not
         self.is_saved = True
 
         # Timer to auto save annotations
         self.save_timer = QTimer()
         self.save_timer.timeout.connect(self.auto_save)
 
@@ -129,14 +132,15 @@
 
     def init_qt(self):
         """Initial actions for qt widgets"""
         # Set triggers for toolBars
         self.AboutBar.actionTriggered[QAction].connect(self.about_bar_dispatcher)
         self.LoadBar.actionTriggered[QAction].connect(self.load_bar_dispatcher)
         self.SaveBar.actionTriggered[QAction].connect(self.save_bar_dispatcher)
+        self.ToolBar.actionTriggered[QAction].connect(self.tool_bar_dispatcher)
 
         # Spectrogram percentile change
         self.PercentileSpin.setValue(self.spectrogram_percentile)
         self.PercentileSpin.setRange(0, 100)
         self.PercentileSpin.valueChanged.connect(self.spec_percentile_change)
         # Spectrogram default channel
         self.DefaultCh4SpecBt.clicked.connect(self.default_ch4Spec)
@@ -204,14 +208,18 @@
         self.specSc.activated.connect(self.show_spec_window)
 
         # next page and previous page triggered by keyborad 
         self.next_pageSc = QShortcut(QKeySequence('right'), self)
         self.next_pageSc.activated.connect(self.next_page)
         self.previous_pageSc = QShortcut(QKeySequence('left'), self)
         self.previous_pageSc.activated.connect(self.previous_page)
+        self.next_epochSc = QShortcut(QKeySequence('down'), self)
+        self.next_epochSc.activated.connect(self.next_epoch)
+        self.previous_epochSc = QShortcut(QKeySequence('up'), self)
+        self.previous_epochSc.activated.connect(self.previous_epoch)
 
         # save labels
         self.SaveLabelBt.clicked.connect(self.save_anno)
         self.saveSc = QShortcut(QKeySequence('CTRL+s'), self)
         self.saveSc.activated.connect(self.save_anno)
 
         
@@ -247,14 +255,27 @@
         self.SaveLabelBt.setDisabled(status)
         self.MarkerRadio.setDisabled(status)
         self.NREMBt.setDisabled(status)
         self.DateTimeEdit.setDisabled(status)
         self.ShowRangeCombo.setDisabled(status)
         self.SaveBar.setDisabled(status)
         self.AboutBar.setDisabled(status)
+        self.ToolBar.setDisabled(status)
+        self.ScrollerBar.setDisabled(status)
+        self.nremSc.setEnabled(not status)
+        self.remSc.setEnabled(not status)
+        self.wakeSc.setEnabled(not status)
+        self.initSc.setEnabled(not status)
+        self.labelSc.setEnabled(not status)
+        self.specSc.setEnabled(not status)
+        self.next_pageSc.setEnabled(not status)
+        self.previous_pageSc.setEnabled(not status)
+        self.next_epochSc.setEnabled(not status)
+        self.previous_epochSc.setEnabled(not status)
+        # self.setShortcutEnabled(not status)
 
     def load_data(self):
         """Triggered by actionLoad_Data, get MiData"""
         data_path, _ = QFileDialog.getOpenFileName(
             self,
             "Select data file",
             f"{self.config['gui']['openpath']}",
@@ -489,15 +510,15 @@
                     range(
                         int(state[0] * self.midata.sf[each]),
                         int((state[1] + 1) * self.midata.sf[each]),
                     ),
                     -y_lim + y_shift,
                     y_lim + y_shift,
                     facecolor=self.state_color_dict[state[2]],
-                    alpha=0.1,
+                    alpha=float(self.config['gui']['statecolorbgalpha']),
                 )
         self.signal_ax[-1].xaxis.set_ticks(
             [
                 int(each * self.midata.sf[self.show_idx[-1]])
                 for each in range(0, self.show_duration + 1, 5)
             ],
             range(self.current_sec, self.current_sec + self.show_duration + 1, 5),
@@ -550,15 +571,15 @@
                     range(
                         int(replot_start * self.midata.sf[each]),
                         int(replot_end * self.midata.sf[each]),
                     ),
                     -y_lim + y_shift,
                     y_lim + y_shift,
                     facecolor=self.state_color_dict[state],
-                    alpha=0.1,
+                    alpha=float(self.config['gui']['statecolorbgalpha']),
                 )
         self.signal_figure.canvas.draw()
         self.signal_figure.canvas.flush_events()
     
 
     def spec_percentile_change(self):
         """Triggered by spectrogramPercentile change"""
@@ -756,17 +777,19 @@
         )
         self.hypo_ax.step(
             range(self.mianno.anno_length),
             self.mianno.sleep_state,
             where="mid",
             linewidth=1,
         )
-        self.hypo_ax.set_ylim(0, 4.5)
+
+        self.hypo_ax.set_ylim(0, len(list(self.state_map_dict.keys())))
         self.hypo_ax.set_xlim(0, self.total_seconds)
-        self.hypo_ax.yaxis.set_ticks([1, 2, 3, 4], ["NREM", "REM", "Wake", "INIT"])
+        self.hypo_ax.yaxis.set_ticks(list(self.state_map_dict.keys()), 
+                                     list(self.state_map_dict.values()))
         if self.StartEndRadio.isChecked():
             for each in self.start_end_ms:
                 self.hypo_ax.axvline(each, color="lime", alpha=1)
 
         if self.SleepStateRadio.isChecked():
             for each in self.start_end:
                 self.hypo_ax.axvline(each, color="lime", alpha=1)
@@ -938,14 +961,24 @@
     def scroller_change(self):
         """ScrollerBar value changed"""
         self.ScrollerBar.setDisabled(True)
         current_sec = self.ScrollerBar.value()
         self.redraw_all(second=current_sec)
         self.ScrollerBar.setEnabled(True)
 
+    def next_epoch(self):
+        """With down button, scroll to next epoch"""
+        current_sec = self.current_sec + 5
+        self.redraw_all(second=current_sec)
+
+    def previous_epoch(self):
+        """With up button, scroll to previous epoch"""
+        current_sec = self.current_sec - 5
+        self.redraw_all(second=current_sec)
+
     def next_page(self):
         """With -> button press, scroll to next page"""
         current_sec = self.current_sec + self.show_duration
         self.redraw_all(second=current_sec)
 
     def previous_page(self):
         """<- button"""
@@ -1300,14 +1333,28 @@
     def save_bar_dispatcher(self, signal):
         """Triggered by SaveBar action, save data, save annotation"""
         if signal.text() == "Save Data":
             pass
         if signal.text() == "Save Annotation":
             self.save_anno()
 
+    def tool_bar_dispatcher(self, signal):
+        """Triggered by ToolBar action, transfer result"""
+        if signal.text() == "Transfer Result":
+            self.transfer_result()
+
+    def transfer_result(self):
+        """Transfer result into file"""
+        self.transfer_result_dialog.exec_()
+        if self.label_dialog.closed:
+            return
+        self.transfer_result_dialog.transfer(config=self.config,
+                                             mianno=self.mianno,
+                                             ac_time=self.midata.time)
+
     def save_anno(self):
         """Save annotation into file"""
         save_thread = SaveThread(file=[self.mianno, self.midata], 
                                  file_path=self.anno_path)
         saved = save_thread.save_anno()
         if saved:
             self.is_saved = True
```

### Comparing `misleep-0.1.4b0/misleep/gui/resources/entire_logo.png` & `misleep-0.1.5b0/misleep/gui/resources/entire_logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/resources/logo.png` & `misleep-0.1.5b0/misleep/gui/resources/logo.png`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/resources/misleep.py` & `misleep-0.1.5b0/misleep/gui/resources/misleep.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/spec_window.py` & `misleep-0.1.5b0/misleep/gui/spec_window.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/thread.py` & `misleep-0.1.5b0/misleep/gui/thread.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/uis/about_ui.py` & `misleep-0.1.5b0/misleep/gui/uis/about_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/uis/label_dialog_ui.py` & `misleep-0.1.5b0/misleep/gui/uis/label_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/gui/uis/main_window_ui.py` & `misleep-0.1.5b0/misleep/gui/uis/main_window_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MiSleep(object):
     def setupUi(self, MiSleep):
         MiSleep.setObjectName("MiSleep")
-        MiSleep.resize(1445, 959)
-        font = QtGui.QFont()
-        font.setStyleStrategy(QtGui.QFont.PreferAntialias)
-        MiSleep.setFont(font)
+        MiSleep.resize(1445, 964)
         MiSleep.setFocusPolicy(QtCore.Qt.WheelFocus)
         icon = QtGui.QIcon()
         icon.addPixmap(QtGui.QPixmap(":/logo/logo.png"), QtGui.QIcon.Normal, QtGui.QIcon.Off)
         MiSleep.setWindowIcon(icon)
         MiSleep.setToolButtonStyle(QtCore.Qt.ToolButtonTextBesideIcon)
         MiSleep.setAnimated(True)
         MiSleep.setDocumentMode(True)
@@ -43,26 +40,26 @@
         self.HypnoArea.setWidget(self.scrollAreaWidgetContents_2)
         self.gridLayout_3.addWidget(self.HypnoArea, 2, 0, 1, 1)
         self.SignalArea = QtWidgets.QScrollArea(self.centralwidget)
         self.SignalArea.setMinimumSize(QtCore.QSize(700, 500))
         self.SignalArea.setWidgetResizable(True)
         self.SignalArea.setObjectName("SignalArea")
         self.scrollAreaWidgetContents = QtWidgets.QWidget()
-        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 1106, 753))
+        self.scrollAreaWidgetContents.setGeometry(QtCore.QRect(0, 0, 1106, 758))
         self.scrollAreaWidgetContents.setObjectName("scrollAreaWidgetContents")
         self.SignalArea.setWidget(self.scrollAreaWidgetContents)
         self.gridLayout_3.addWidget(self.SignalArea, 0, 0, 1, 1)
         self.ScrollerBar = QtWidgets.QScrollBar(self.centralwidget)
         self.ScrollerBar.setTracking(False)
         self.ScrollerBar.setOrientation(QtCore.Qt.Horizontal)
         self.ScrollerBar.setObjectName("ScrollerBar")
         self.gridLayout_3.addWidget(self.ScrollerBar, 1, 0, 1, 1)
         MiSleep.setCentralWidget(self.centralwidget)
         self.MetaDock = QtWidgets.QDockWidget(MiSleep)
-        self.MetaDock.setMinimumSize(QtCore.QSize(264, 112))
+        self.MetaDock.setMinimumSize(QtCore.QSize(288, 124))
         self.MetaDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.MetaDock.setObjectName("MetaDock")
         self.dockWidgetContents_3 = QtWidgets.QWidget()
         self.dockWidgetContents_3.setObjectName("dockWidgetContents_3")
         self.formLayout = QtWidgets.QFormLayout(self.dockWidgetContents_3)
         self.formLayout.setObjectName("formLayout")
         self.label_4 = QtWidgets.QLabel(self.dockWidgetContents_3)
@@ -242,15 +239,15 @@
         self.line_4.setFrameShape(QtWidgets.QFrame.VLine)
         self.line_4.setFrameShadow(QtWidgets.QFrame.Sunken)
         self.line_4.setObjectName("line_4")
         self.gridLayout_2.addWidget(self.line_4, 1, 1, 1, 1)
         self.AnnotationDock.setWidget(self.dockWidgetContents_5)
         MiSleep.addDockWidget(QtCore.Qt.DockWidgetArea(2), self.AnnotationDock)
         self.TimeDock = QtWidgets.QDockWidget(MiSleep)
-        self.TimeDock.setMinimumSize(QtCore.QSize(167, 148))
+        self.TimeDock.setMinimumSize(QtCore.QSize(197, 148))
         self.TimeDock.setAcceptDrops(False)
         self.TimeDock.setAutoFillBackground(True)
         self.TimeDock.setFeatures(QtWidgets.QDockWidget.DockWidgetFloatable|QtWidgets.QDockWidget.DockWidgetMovable)
         self.TimeDock.setAllowedAreas(QtCore.Qt.AllDockWidgetAreas)
         self.TimeDock.setObjectName("TimeDock")
         self.dockWidgetContents_7 = QtWidgets.QWidget()
         self.dockWidgetContents_7.setObjectName("dockWidgetContents_7")
@@ -306,37 +303,53 @@
         font = QtGui.QFont()
         font.setFamily("Arial")
         font.setPointSize(11)
         font.setStyleStrategy(QtGui.QFont.PreferAntialias)
         self.AboutBar.setFont(font)
         self.AboutBar.setObjectName("AboutBar")
         MiSleep.addToolBar(QtCore.Qt.TopToolBarArea, self.AboutBar)
+        self.ToolBar = QtWidgets.QToolBar(MiSleep)
+        font = QtGui.QFont()
+        font.setFamily("Arial")
+        font.setPointSize(11)
+        font.setStyleStrategy(QtGui.QFont.PreferAntialias)
+        self.ToolBar.setFont(font)
+        self.ToolBar.setObjectName("ToolBar")
+        MiSleep.addToolBar(QtCore.Qt.TopToolBarArea, self.ToolBar)
         self.actionLoad_Data = QtWidgets.QAction(MiSleep)
         self.actionLoad_Data.setObjectName("actionLoad_Data")
         self.actionLoad_Annotation = QtWidgets.QAction(MiSleep)
         self.actionLoad_Annotation.setObjectName("actionLoad_Annotation")
         self.actionShow = QtWidgets.QAction(MiSleep)
         self.actionShow.setObjectName("actionShow")
         self.actionSave_data = QtWidgets.QAction(MiSleep)
         self.actionSave_data.setObjectName("actionSave_data")
         self.actionSave_Annotation = QtWidgets.QAction(MiSleep)
         self.actionSave_Annotation.setObjectName("actionSave_Annotation")
         self.actionAbout = QtWidgets.QAction(MiSleep)
         self.actionAbout.setObjectName("actionAbout")
+        self.actionMerge_Data = QtWidgets.QAction(MiSleep)
+        self.actionMerge_Data.setObjectName("actionMerge_Data")
+        self.actionTransfer_Result = QtWidgets.QAction(MiSleep)
+        self.actionTransfer_Result.setObjectName("actionTransfer_Result")
         self.LoadBar.addAction(self.actionLoad_Data)
         self.LoadBar.addSeparator()
         self.LoadBar.addAction(self.actionLoad_Annotation)
         self.LoadBar.addSeparator()
         self.LoadBar.addAction(self.actionShow)
         self.LoadBar.addSeparator()
         self.SaveBar.addAction(self.actionSave_data)
         self.SaveBar.addSeparator()
         self.SaveBar.addAction(self.actionSave_Annotation)
         self.SaveBar.addSeparator()
         self.AboutBar.addAction(self.actionAbout)
+        self.ToolBar.addAction(self.actionMerge_Data)
+        self.ToolBar.addSeparator()
+        self.ToolBar.addAction(self.actionTransfer_Result)
+        self.ToolBar.addSeparator()
 
         self.retranslateUi(MiSleep)
         QtCore.QMetaObject.connectSlotsByName(MiSleep)
 
     def retranslateUi(self, MiSleep):
         _translate = QtCore.QCoreApplication.translate
         MiSleep.setWindowTitle(_translate("MiSleep", "MiSleep"))
@@ -380,14 +393,18 @@
         self.ShowRangeCombo.setItemText(2, _translate("MiSleep", "Show 5 minutes"))
         self.ShowRangeCombo.setItemText(3, _translate("MiSleep", "Show 30 minutes"))
         self.ShowRangeCombo.setItemText(4, _translate("MiSleep", "Show 1 hour"))
         self.CustomSecondsCheck.setText(_translate("MiSleep", "Custom seconds"))
         self.LoadBar.setWindowTitle(_translate("MiSleep", "LoadBar"))
         self.SaveBar.setWindowTitle(_translate("MiSleep", "SaveBar"))
         self.AboutBar.setWindowTitle(_translate("MiSleep", "toolBar"))
+        self.ToolBar.setWindowTitle(_translate("MiSleep", "toolBar"))
         self.actionLoad_Data.setText(_translate("MiSleep", "Load Data"))
         self.actionLoad_Annotation.setText(_translate("MiSleep", "Load Annotation"))
         self.actionShow.setText(_translate("MiSleep", "Show"))
         self.actionSave_data.setText(_translate("MiSleep", "Save Data"))
         self.actionSave_Annotation.setText(_translate("MiSleep", "Save Annotation"))
         self.actionAbout.setText(_translate("MiSleep", "About"))
+        self.actionMerge_Data.setText(_translate("MiSleep", "Merge Data"))
+        self.actionTransfer_Result.setText(_translate("MiSleep", "Transfer Result"))
+        self.actionTransfer_Result.setToolTip(_translate("MiSleep", "Transfer Result"))
 from misleep.gui.resources import misleep
```

### Comparing `misleep-0.1.4b0/misleep/gui/uis/spec_window_ui.py` & `misleep-0.1.5b0/misleep/gui/uis/spec_window_ui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/io/annotation_io.py` & `misleep-0.1.5b0/misleep/io/annotation_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/io/base.py` & `misleep-0.1.5b0/misleep/io/base.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/io/signal_io.py` & `misleep-0.1.5b0/misleep/io/signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/preprocessing/spectral.py` & `misleep-0.1.5b0/misleep/preprocessing/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/utils/annotation.py` & `misleep-0.1.5b0/misleep/utils/annotation.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/utils/only4gui.py` & `misleep-0.1.5b0/misleep/utils/only4gui.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/utils/signals.py` & `misleep-0.1.5b0/misleep/utils/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/viz/hypnogram.py` & `misleep-0.1.5b0/misleep/viz/hypnogram.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/viz/signals.py` & `misleep-0.1.5b0/misleep/viz/signals.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep/viz/spectral.py` & `misleep-0.1.5b0/misleep/viz/spectral.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/misleep.egg-info/PKG-INFO` & `misleep-0.1.5b0/misleep.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misleep
-Version: 0.1.4b0
+Version: 0.1.5b0
 Summary: MiSleep: Mice Sleep EEG/EMG visualization, scoring and analysis.
 Home-page: https://github.com/BryanWang0702/MiSleep/
 Download-URL: https://github.com/BryanWang0702/MiSleep/
 Author: Xueqiang Wang
 Author-email: swang@gmail.com
 Maintainer: Xueqiang Wang
 Maintainer-email: swang@gmail.com
@@ -23,14 +23,16 @@
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: matplotlib
 Requires-Dist: scipy
 Requires-Dist: pyedflib
 Requires-Dist: hdf5storage
 Requires-Dist: pyqt5
 Requires-Dist: mat73
+Requires-Dist: pandas
+Requires-Dist: openpyxl
 
 # MiSleep
 MiSleep is for EEG/EMG signal processing and visualization
 
 ![logo](resources/entire_logo.png)
 
 ## Get start
```

### Comparing `misleep-0.1.4b0/misleep.egg-info/SOURCES.txt` & `misleep-0.1.5b0/misleep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 misleep.egg-info/PKG-INFO
 misleep.egg-info/SOURCES.txt
 misleep.egg-info/dependency_links.txt
 misleep.egg-info/requires.txt
 misleep.egg-info/top_level.txt
 misleep/gui/__init__.py
 misleep/gui/about.py
-misleep/gui/label_dialog.py
+misleep/gui/dialog.py
 misleep/gui/main_window.py
 misleep/gui/show.py
 misleep/gui/spec_window.py
 misleep/gui/thread.py
 misleep/gui/utils.py
 misleep/gui/resources/__init__.py
 misleep/gui/resources/entire_logo.png
@@ -23,14 +23,15 @@
 misleep/gui/resources/misleep.py
 misleep/gui/resources/misleep.qrc
 misleep/gui/uis/__init__.py
 misleep/gui/uis/about_ui.py
 misleep/gui/uis/label_dialog_ui.py
 misleep/gui/uis/main_window_ui.py
 misleep/gui/uis/spec_window_ui.py
+misleep/gui/uis/transfer_result_dialog_ui.py
 misleep/io/__init__.py
 misleep/io/annotation_io.py
 misleep/io/base.py
 misleep/io/signal_io.py
 misleep/preprocessing/__init__.py
 misleep/preprocessing/channel.py
 misleep/preprocessing/spectral.py
```

### Comparing `misleep-0.1.4b0/setup.py` & `misleep-0.1.5b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 DISTNAME = "misleep"
 MAINTAINER = "Xueqiang Wang"
 MAINTAINER_EMAIL = "swang@gmail.com"
 URL = "https://github.com/BryanWang0702/MiSleep/"
 LICENSE = "BSD (3-clause)"
 DOWNLOAD_URL = "https://github.com/BryanWang0702/MiSleep/"
-VERSION = "0.1.4 Beta"
+VERSION = "0.1.5 Beta"
 
 INSTALL_REQUIRES = [
     "numpy>=1.18.1",
     "matplotlib",
     "scipy",
     "pyedflib",
     "hdf5storage",
     "pyqt5",
-    "mat73"
+    "mat73",
+    "pandas",
+    "openpyxl"
 ]
 
 PACKAGES = [
     "misleep",
 ]
 
 CLASSIFIERS = [
```

### Comparing `misleep-0.1.4b0/test/test_midata.py` & `misleep-0.1.5b0/test/test_midata.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/test/test_signal_io.py` & `misleep-0.1.5b0/test/test_signal_io.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/test/test_signals_viz.py` & `misleep-0.1.5b0/test/test_signals_viz.py`

 * *Files identical despite different names*

### Comparing `misleep-0.1.4b0/test/test_spectral_viz.py` & `misleep-0.1.5b0/test/test_spectral_viz.py`

 * *Files identical despite different names*

