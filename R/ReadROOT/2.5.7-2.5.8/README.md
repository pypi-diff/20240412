# Comparing `tmp/ReadROOT-2.5.7.tar.gz` & `tmp/ReadROOT-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReadROOT-2.5.7.tar", last modified: Fri Apr 12 11:27:00 2024, max compression
+gzip compressed data, was "ReadROOT-2.5.8.tar", last modified: Fri Apr 12 11:42:16 2024, max compression
```

## Comparing `ReadROOT-2.5.7.tar` & `ReadROOT-2.5.8.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.904644 ReadROOT-2.5.7/
--rw-rw-rw-   0        0        0    40377 2024-04-12 11:25:30.000000 ReadROOT-2.5.7/ErrorPropagation.py
--rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.5.7/IOClasses.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.196749 ReadROOT-2.5.7/Images/
--rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Calculate.png
--rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Clear.png
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.519750 ReadROOT-2.5.7/Images/CoMPASS/
--rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.5.7/Images/CoMPASS/Coincidence.png
--rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.5.7/Images/CoMPASS/Discriminator.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.5.7/Images/CoMPASS/EnergyCalibration.png
--rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.5.7/Images/CoMPASS/Input.png
--rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.5.7/Images/CoMPASS/Misc.png
--rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/CoMPASS/OpenGraph.png
--rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.5.7/Images/CoMPASS/QDC.png
--rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.5.7/Images/CoMPASS/Rejections.png
--rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.5.7/Images/CoMPASS/Spectra.png
--rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.5.7/Images/CoMPASS/Sync.png
--rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/CoMPASS/icon64x64.ico
--rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.5.7/Images/CoMPASS/icon64x64.png
--rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.5.7/Images/CompClear.png
--rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.5.7/Images/Disabled0.png
--rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.5.7/Images/Disabled1.png
--rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.5.7/Images/Disabled2.png
--rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.5.7/Images/Disabled3.png
--rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.5.7/Images/DisabledSelect.png
--rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.5.7/Images/DisabledSelectROI.png
--rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/EnergyHist.png
--rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.5.7/Images/EnergyvsEnergyHist.png
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.760897 ReadROOT-2.5.7/Images/Log/
--rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.5.7/Images/Log/0.png
--rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.5.7/Images/Log/1.png
--rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.5.7/Images/Log/2.png
--rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.5.7/Images/Log/3.png
--rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.5.7/Images/Log/4.png
--rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.5.7/Images/Log/5.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.5.7/Images/Log/6.png
--rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.5.7/Images/Log/7.png
--rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.5.7/Images/Log/8.png
--rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.5.7/Images/Log/9+.png
--rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.5.7/Images/Log/9.png
--rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/MCS Graph.png
--rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Off0.png
--rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Off1.png
--rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Off2.png
--rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Off3.png
--rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.5.7/Images/OffSelect.png
--rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/OffSelectROI.png
--rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/On0.png
--rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/On1.png
--rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/On2.png
--rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/On3.png
--rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.5.7/Images/OnSelect.png
--rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/OnSelectROI.png
--rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/OpenFolder.png
--rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/OpenFolderCompass.png
--rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/PSDHist.png
--rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/PSDvsEnergyHist.png
--rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/Plot.png
--rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/PlotCompass.png
--rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.5.7/Images/SaveCompass.png
--rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/SaveImage.png
--rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/TOFHist.png
--rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.5.7/Images/TOFvsEnergyHist.png
--rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.5.7/Images/TimeHist.png
--rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.5.7/Images/axis.png
--rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.5.7/Images/collapsed.png
--rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.5.7/Images/delete.png
--rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.5.7/Images/expanded.png
--rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.5.7/Images/file_config.png
--rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.5.7/Images/grid.png
--rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.5.7/Images/histogram.png
--rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.5.7/Images/info.png
--rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.5.7/Images/line.png
--rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.5.7/Images/save.png
--rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.5.7/Images/settings.png
--rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.5.7/Images/start.png
--rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.5.7/Images/stop.png
--rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.5.7/Images/time.png
--rw-rw-rw-   0        0        0     2787 2024-04-12 11:27:00.902500 ReadROOT-2.5.7/PKG-INFO
--rw-rw-rw-   0        0        0    11981 2024-03-17 16:38:14.000000 ReadROOT-2.5.7/QtClasses.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.865762 ReadROOT-2.5.7/ReadROOT.egg-info/
--rw-rw-rw-   0        0        0     2787 2024-04-12 11:26:58.000000 ReadROOT-2.5.7/ReadROOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2178 2024-04-12 11:26:58.000000 ReadROOT-2.5.7/ReadROOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 11:26:58.000000 ReadROOT-2.5.7/ReadROOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      191 2024-04-12 11:26:58.000000 ReadROOT-2.5.7/ReadROOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 11:26:58.000000 ReadROOT-2.5.7/ReadROOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7245 2023-06-08 18:12:55.000000 ReadROOT-2.5.7/ValidInputs.py
--rw-rw-rw-   0        0        0    11972 2023-09-12 16:41:14.000000 ReadROOT-2.5.7/XML_Parser.py
--rw-rw-rw-   0        0        0     4244 2024-04-12 11:26:35.000000 ReadROOT-2.5.7/__init__.py
--rw-rw-rw-   0        0        0      881 2023-07-19 17:15:14.000000 ReadROOT-2.5.7/config.json
--rw-rw-rw-   0        0        0    44649 2023-08-07 16:34:06.000000 ReadROOT-2.5.7/discord.mp3
--rw-rw-rw-   0        0        0     7990 2023-08-16 19:49:31.000000 ReadROOT-2.5.7/funcs.cpp
--rw-rw-rw-   0        0        0     2186 2023-08-16 19:53:47.000000 ReadROOT-2.5.7/funcs.hpp
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.878264 ReadROOT-2.5.7/merge/
--rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.5.7/merge/__init__.py
--rw-rw-rw-   0        0        0     6327 2023-07-19 16:22:00.000000 ReadROOT-2.5.7/merge/merge_root_files.py
--rw-rw-rw-   0        0        0    31875 2023-09-12 16:40:05.000000 ReadROOT-2.5.7/read_root.py
--rw-rw-rw-   0        0        0    79471 2023-09-12 16:37:07.000000 ReadROOT-2.5.7/read_root_gui.py
--rw-rw-rw-   0        0        0    98438 2024-04-12 11:26:35.000000 ReadROOT-2.5.7/read_root_gui_v2.py
--rw-rw-rw-   0        0        0     1369 2024-04-12 11:26:29.000000 ReadROOT-2.5.7/reload.py
--rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.5.7/root_plotter.py
--rw-rw-rw-   0        0        0       42 2024-04-12 11:27:00.906832 ReadROOT-2.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1600 2024-04-12 11:26:35.000000 ReadROOT-2.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 11:27:00.896558 ReadROOT-2.5.7/test/
--rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.5.7/test/test.py
--rw-rw-rw-   0        0        0      311 2023-09-12 16:26:23.000000 ReadROOT-2.5.7/test/test2.py
--rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.5.7/test/test_cpp.py
--rw-rw-rw-   0        0        0      110 2023-08-16 15:36:59.000000 ReadROOT-2.5.7/test/test_cpp_doc.py
--rw-rw-rw-   0        0        0      596 2023-08-16 17:23:41.000000 ReadROOT-2.5.7/wrap.cpp
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.466461 ReadROOT-2.5.8/
+-rw-rw-rw-   0        0        0    40541 2024-04-12 11:39:05.000000 ReadROOT-2.5.8/ErrorPropagation.py
+-rw-rw-rw-   0        0        0     5152 2023-06-14 20:31:08.000000 ReadROOT-2.5.8/IOClasses.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.283089 ReadROOT-2.5.8/Images/
+-rw-rw-rw-   0        0        0     1802 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Calculate.png
+-rw-rw-rw-   0        0        0     2340 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Clear.png
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.338721 ReadROOT-2.5.8/Images/CoMPASS/
+-rw-rw-rw-   0        0        0     2712 2023-05-23 14:31:42.000000 ReadROOT-2.5.8/Images/CoMPASS/Coincidence.png
+-rw-rw-rw-   0        0        0     2292 2023-05-23 14:18:04.000000 ReadROOT-2.5.8/Images/CoMPASS/Discriminator.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:27:57.000000 ReadROOT-2.5.8/Images/CoMPASS/EnergyCalibration.png
+-rw-rw-rw-   0        0        0     2492 2023-05-23 14:13:06.000000 ReadROOT-2.5.8/Images/CoMPASS/Input.png
+-rw-rw-rw-   0        0        0     2547 2023-05-23 14:32:49.000000 ReadROOT-2.5.8/Images/CoMPASS/Misc.png
+-rw-rw-rw-   0        0        0     1089 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/CoMPASS/OpenGraph.png
+-rw-rw-rw-   0        0        0     2499 2023-05-23 14:20:06.000000 ReadROOT-2.5.8/Images/CoMPASS/QDC.png
+-rw-rw-rw-   0        0        0     2282 2023-05-23 14:25:56.000000 ReadROOT-2.5.8/Images/CoMPASS/Rejections.png
+-rw-rw-rw-   0        0        0     2472 2023-05-23 14:23:25.000000 ReadROOT-2.5.8/Images/CoMPASS/Spectra.png
+-rw-rw-rw-   0        0        0     2264 2023-05-23 14:29:40.000000 ReadROOT-2.5.8/Images/CoMPASS/Sync.png
+-rw-rw-rw-   0        0        0    15934 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/CoMPASS/icon64x64.ico
+-rw-rw-rw-   0        0        0     3193 2023-06-14 13:48:49.000000 ReadROOT-2.5.8/Images/CoMPASS/icon64x64.png
+-rw-rw-rw-   0        0        0     1734 2023-06-12 19:05:08.000000 ReadROOT-2.5.8/Images/CompClear.png
+-rw-rw-rw-   0        0        0     1452 2023-06-08 20:53:51.000000 ReadROOT-2.5.8/Images/Disabled0.png
+-rw-rw-rw-   0        0        0     1201 2023-06-08 20:54:19.000000 ReadROOT-2.5.8/Images/Disabled1.png
+-rw-rw-rw-   0        0        0     1515 2023-06-08 20:54:35.000000 ReadROOT-2.5.8/Images/Disabled2.png
+-rw-rw-rw-   0        0        0     1566 2023-06-08 20:54:54.000000 ReadROOT-2.5.8/Images/Disabled3.png
+-rw-rw-rw-   0        0        0     1583 2023-06-21 19:30:21.000000 ReadROOT-2.5.8/Images/DisabledSelect.png
+-rw-rw-rw-   0        0        0     1994 2023-06-14 14:36:16.000000 ReadROOT-2.5.8/Images/DisabledSelectROI.png
+-rw-rw-rw-   0        0        0     1646 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/EnergyHist.png
+-rw-rw-rw-   0        0        0     1106 2023-06-12 18:27:14.000000 ReadROOT-2.5.8/Images/EnergyvsEnergyHist.png
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.378369 ReadROOT-2.5.8/Images/Log/
+-rw-rw-rw-   0        0        0      551 2023-07-04 16:52:34.000000 ReadROOT-2.5.8/Images/Log/0.png
+-rw-rw-rw-   0        0        0      476 2023-07-04 16:45:55.000000 ReadROOT-2.5.8/Images/Log/1.png
+-rw-rw-rw-   0        0        0      761 2023-07-04 16:46:51.000000 ReadROOT-2.5.8/Images/Log/2.png
+-rw-rw-rw-   0        0        0      818 2023-07-04 18:15:22.000000 ReadROOT-2.5.8/Images/Log/3.png
+-rw-rw-rw-   0        0        0      620 2023-07-04 18:16:09.000000 ReadROOT-2.5.8/Images/Log/4.png
+-rw-rw-rw-   0        0        0      835 2023-07-04 18:16:54.000000 ReadROOT-2.5.8/Images/Log/5.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:17:44.000000 ReadROOT-2.5.8/Images/Log/6.png
+-rw-rw-rw-   0        0        0      635 2023-07-04 18:18:20.000000 ReadROOT-2.5.8/Images/Log/7.png
+-rw-rw-rw-   0        0        0      822 2023-07-04 18:18:59.000000 ReadROOT-2.5.8/Images/Log/8.png
+-rw-rw-rw-   0        0        0      971 2023-07-04 18:24:12.000000 ReadROOT-2.5.8/Images/Log/9+.png
+-rw-rw-rw-   0        0        0      747 2023-07-04 18:19:41.000000 ReadROOT-2.5.8/Images/Log/9.png
+-rw-rw-rw-   0        0        0     4514 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/MCS Graph.png
+-rw-rw-rw-   0        0        0     1322 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Off0.png
+-rw-rw-rw-   0        0        0      937 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Off1.png
+-rw-rw-rw-   0        0        0     1343 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Off2.png
+-rw-rw-rw-   0        0        0     1370 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Off3.png
+-rw-rw-rw-   0        0        0      860 2023-06-21 19:30:00.000000 ReadROOT-2.5.8/Images/OffSelect.png
+-rw-rw-rw-   0        0        0     1718 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/OffSelectROI.png
+-rw-rw-rw-   0        0        0     1335 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/On0.png
+-rw-rw-rw-   0        0        0      926 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/On1.png
+-rw-rw-rw-   0        0        0     1336 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/On2.png
+-rw-rw-rw-   0        0        0     1366 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/On3.png
+-rw-rw-rw-   0        0        0      589 2023-06-21 19:29:10.000000 ReadROOT-2.5.8/Images/OnSelect.png
+-rw-rw-rw-   0        0        0     1737 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/OnSelectROI.png
+-rw-rw-rw-   0        0        0     1099 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/OpenFolder.png
+-rw-rw-rw-   0        0        0     1267 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/OpenFolderCompass.png
+-rw-rw-rw-   0        0        0     1224 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/PSDHist.png
+-rw-rw-rw-   0        0        0     1450 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/PSDvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1927 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/Plot.png
+-rw-rw-rw-   0        0        0     1242 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/PlotCompass.png
+-rw-rw-rw-   0        0        0     1404 2023-06-20 18:31:47.000000 ReadROOT-2.5.8/Images/SaveCompass.png
+-rw-rw-rw-   0        0        0     1461 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/SaveImage.png
+-rw-rw-rw-   0        0        0     2076 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/TOFHist.png
+-rw-rw-rw-   0        0        0     1140 2023-06-12 18:27:54.000000 ReadROOT-2.5.8/Images/TOFvsEnergyHist.png
+-rw-rw-rw-   0        0        0     1447 2022-12-02 19:45:45.000000 ReadROOT-2.5.8/Images/TimeHist.png
+-rw-rw-rw-   0        0        0      947 2023-05-17 22:43:58.000000 ReadROOT-2.5.8/Images/axis.png
+-rw-rw-rw-   0        0        0      463 2023-06-02 19:16:56.000000 ReadROOT-2.5.8/Images/collapsed.png
+-rw-rw-rw-   0        0        0      689 2023-05-17 22:35:31.000000 ReadROOT-2.5.8/Images/delete.png
+-rw-rw-rw-   0        0        0      458 2023-06-02 19:17:19.000000 ReadROOT-2.5.8/Images/expanded.png
+-rw-rw-rw-   0        0        0     1010 2023-05-17 19:25:44.000000 ReadROOT-2.5.8/Images/file_config.png
+-rw-rw-rw-   0        0        0      667 2023-05-17 22:56:43.000000 ReadROOT-2.5.8/Images/grid.png
+-rw-rw-rw-   0        0        0     1546 2023-05-23 15:50:13.000000 ReadROOT-2.5.8/Images/histogram.png
+-rw-rw-rw-   0        0        0      999 2023-05-17 20:52:54.000000 ReadROOT-2.5.8/Images/info.png
+-rw-rw-rw-   0        0        0      344 2023-05-17 22:44:20.000000 ReadROOT-2.5.8/Images/line.png
+-rw-rw-rw-   0        0        0      647 2023-05-17 22:35:02.000000 ReadROOT-2.5.8/Images/save.png
+-rw-rw-rw-   0        0        0     1712 2023-05-17 22:24:15.000000 ReadROOT-2.5.8/Images/settings.png
+-rw-rw-rw-   0        0        0     2094 2023-06-14 14:54:21.000000 ReadROOT-2.5.8/Images/start.png
+-rw-rw-rw-   0        0        0     1992 2023-06-14 14:53:58.000000 ReadROOT-2.5.8/Images/stop.png
+-rw-rw-rw-   0        0        0     1262 2023-05-23 15:51:24.000000 ReadROOT-2.5.8/Images/time.png
+-rw-rw-rw-   0        0        0     2787 2024-04-12 11:42:16.464215 ReadROOT-2.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11981 2024-03-17 16:38:14.000000 ReadROOT-2.5.8/QtClasses.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.433031 ReadROOT-2.5.8/ReadROOT.egg-info/
+-rw-rw-rw-   0        0        0     2787 2024-04-12 11:42:15.000000 ReadROOT-2.5.8/ReadROOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2178 2024-04-12 11:42:15.000000 ReadROOT-2.5.8/ReadROOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:42:15.000000 ReadROOT-2.5.8/ReadROOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      191 2024-04-12 11:42:15.000000 ReadROOT-2.5.8/ReadROOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 11:42:15.000000 ReadROOT-2.5.8/ReadROOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7245 2023-06-08 18:12:55.000000 ReadROOT-2.5.8/ValidInputs.py
+-rw-rw-rw-   0        0        0    11972 2023-09-12 16:41:14.000000 ReadROOT-2.5.8/XML_Parser.py
+-rw-rw-rw-   0        0        0     4244 2024-04-12 11:42:02.000000 ReadROOT-2.5.8/__init__.py
+-rw-rw-rw-   0        0        0      881 2023-07-19 17:15:14.000000 ReadROOT-2.5.8/config.json
+-rw-rw-rw-   0        0        0    44649 2023-08-07 16:34:06.000000 ReadROOT-2.5.8/discord.mp3
+-rw-rw-rw-   0        0        0     7990 2023-08-16 19:49:31.000000 ReadROOT-2.5.8/funcs.cpp
+-rw-rw-rw-   0        0        0     2186 2023-08-16 19:53:47.000000 ReadROOT-2.5.8/funcs.hpp
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.441539 ReadROOT-2.5.8/merge/
+-rw-rw-rw-   0        0        0      106 2023-06-19 15:42:39.000000 ReadROOT-2.5.8/merge/__init__.py
+-rw-rw-rw-   0        0        0     6327 2023-07-19 16:22:00.000000 ReadROOT-2.5.8/merge/merge_root_files.py
+-rw-rw-rw-   0        0        0    31875 2023-09-12 16:40:05.000000 ReadROOT-2.5.8/read_root.py
+-rw-rw-rw-   0        0        0    79471 2023-09-12 16:37:07.000000 ReadROOT-2.5.8/read_root_gui.py
+-rw-rw-rw-   0        0        0    98438 2024-04-12 11:42:02.000000 ReadROOT-2.5.8/read_root_gui_v2.py
+-rw-rw-rw-   0        0        0     1369 2024-04-12 11:42:01.000000 ReadROOT-2.5.8/reload.py
+-rw-rw-rw-   0        0        0     3531 2023-07-12 14:25:15.000000 ReadROOT-2.5.8/root_plotter.py
+-rw-rw-rw-   0        0        0       42 2024-04-12 11:42:16.467853 ReadROOT-2.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-04-12 11:42:02.000000 ReadROOT-2.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:42:16.459186 ReadROOT-2.5.8/test/
+-rw-rw-rw-   0        0        0       19 2023-05-25 14:27:41.000000 ReadROOT-2.5.8/test/test.py
+-rw-rw-rw-   0        0        0      311 2023-09-12 16:26:23.000000 ReadROOT-2.5.8/test/test2.py
+-rw-rw-rw-   0        0        0     2864 2023-06-14 19:53:55.000000 ReadROOT-2.5.8/test/test_cpp.py
+-rw-rw-rw-   0        0        0      110 2023-08-16 15:36:59.000000 ReadROOT-2.5.8/test/test_cpp_doc.py
+-rw-rw-rw-   0        0        0      596 2023-08-16 17:23:41.000000 ReadROOT-2.5.8/wrap.cpp
```

### Comparing `ReadROOT-2.5.7/ErrorPropagation.py` & `ReadROOT-2.5.8/ErrorPropagation.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,17 @@
         if kwargs == None:
             pass
     
     def __len__(self):
         return len(self.list)
     
     def __getitem__(self, item):
+        if isinstance(item, slice):
+            indices = range(*item.indices(len(self.list)))
+            return UList(ufloats=[self.list[i] for i in indices])
         return self.list[item]
 
     def __str__(self):
         string = ""
         for ufloat in self.list:
             string += str(ufloat) + ", "
         return string
```

### Comparing `ReadROOT-2.5.7/IOClasses.py` & `ReadROOT-2.5.8/IOClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Calculate.png` & `ReadROOT-2.5.8/Images/Calculate.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Clear.png` & `ReadROOT-2.5.8/Images/Clear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Coincidence.png` & `ReadROOT-2.5.8/Images/CoMPASS/Coincidence.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Discriminator.png` & `ReadROOT-2.5.8/Images/CoMPASS/Discriminator.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/EnergyCalibration.png` & `ReadROOT-2.5.8/Images/CoMPASS/EnergyCalibration.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Input.png` & `ReadROOT-2.5.8/Images/CoMPASS/Input.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Misc.png` & `ReadROOT-2.5.8/Images/CoMPASS/Misc.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/OpenGraph.png` & `ReadROOT-2.5.8/Images/CoMPASS/OpenGraph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/QDC.png` & `ReadROOT-2.5.8/Images/CoMPASS/QDC.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Rejections.png` & `ReadROOT-2.5.8/Images/CoMPASS/Rejections.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Spectra.png` & `ReadROOT-2.5.8/Images/CoMPASS/Spectra.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/Sync.png` & `ReadROOT-2.5.8/Images/CoMPASS/Sync.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/icon64x64.ico` & `ReadROOT-2.5.8/Images/CoMPASS/icon64x64.ico`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CoMPASS/icon64x64.png` & `ReadROOT-2.5.8/Images/CoMPASS/icon64x64.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/CompClear.png` & `ReadROOT-2.5.8/Images/CompClear.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Disabled0.png` & `ReadROOT-2.5.8/Images/Disabled0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Disabled1.png` & `ReadROOT-2.5.8/Images/Disabled1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Disabled2.png` & `ReadROOT-2.5.8/Images/Disabled2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Disabled3.png` & `ReadROOT-2.5.8/Images/Disabled3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/DisabledSelect.png` & `ReadROOT-2.5.8/Images/DisabledSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/DisabledSelectROI.png` & `ReadROOT-2.5.8/Images/DisabledSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/EnergyHist.png` & `ReadROOT-2.5.8/Images/EnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/EnergyvsEnergyHist.png` & `ReadROOT-2.5.8/Images/EnergyvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/0.png` & `ReadROOT-2.5.8/Images/Log/0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/2.png` & `ReadROOT-2.5.8/Images/Log/2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/3.png` & `ReadROOT-2.5.8/Images/Log/3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/4.png` & `ReadROOT-2.5.8/Images/Log/4.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/5.png` & `ReadROOT-2.5.8/Images/Log/5.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/6.png` & `ReadROOT-2.5.8/Images/Log/6.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/7.png` & `ReadROOT-2.5.8/Images/Log/7.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/8.png` & `ReadROOT-2.5.8/Images/Log/8.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/9+.png` & `ReadROOT-2.5.8/Images/Log/9+.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Log/9.png` & `ReadROOT-2.5.8/Images/Log/9.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/MCS Graph.png` & `ReadROOT-2.5.8/Images/MCS Graph.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Off0.png` & `ReadROOT-2.5.8/Images/Off0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Off1.png` & `ReadROOT-2.5.8/Images/Off1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Off2.png` & `ReadROOT-2.5.8/Images/Off2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Off3.png` & `ReadROOT-2.5.8/Images/Off3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OffSelect.png` & `ReadROOT-2.5.8/Images/OffSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OffSelectROI.png` & `ReadROOT-2.5.8/Images/OffSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/On0.png` & `ReadROOT-2.5.8/Images/On0.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/On1.png` & `ReadROOT-2.5.8/Images/On1.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/On2.png` & `ReadROOT-2.5.8/Images/On2.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/On3.png` & `ReadROOT-2.5.8/Images/On3.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OnSelect.png` & `ReadROOT-2.5.8/Images/OnSelect.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OnSelectROI.png` & `ReadROOT-2.5.8/Images/OnSelectROI.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OpenFolder.png` & `ReadROOT-2.5.8/Images/OpenFolder.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/OpenFolderCompass.png` & `ReadROOT-2.5.8/Images/OpenFolderCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/PSDHist.png` & `ReadROOT-2.5.8/Images/PSDHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/PSDvsEnergyHist.png` & `ReadROOT-2.5.8/Images/PSDvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/Plot.png` & `ReadROOT-2.5.8/Images/Plot.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/PlotCompass.png` & `ReadROOT-2.5.8/Images/PlotCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/SaveCompass.png` & `ReadROOT-2.5.8/Images/SaveCompass.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/SaveImage.png` & `ReadROOT-2.5.8/Images/SaveImage.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/TOFHist.png` & `ReadROOT-2.5.8/Images/TOFHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/TOFvsEnergyHist.png` & `ReadROOT-2.5.8/Images/TOFvsEnergyHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/TimeHist.png` & `ReadROOT-2.5.8/Images/TimeHist.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/axis.png` & `ReadROOT-2.5.8/Images/axis.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/delete.png` & `ReadROOT-2.5.8/Images/delete.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/file_config.png` & `ReadROOT-2.5.8/Images/file_config.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/grid.png` & `ReadROOT-2.5.8/Images/grid.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/histogram.png` & `ReadROOT-2.5.8/Images/histogram.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/info.png` & `ReadROOT-2.5.8/Images/info.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/save.png` & `ReadROOT-2.5.8/Images/save.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/settings.png` & `ReadROOT-2.5.8/Images/settings.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/start.png` & `ReadROOT-2.5.8/Images/start.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/stop.png` & `ReadROOT-2.5.8/Images/stop.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/Images/time.png` & `ReadROOT-2.5.8/Images/time.png`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/PKG-INFO` & `ReadROOT-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadROOT
-Version: 2.5.7
+Version: 2.5.8
 Summary: Easy GUI made to read ROOT files created by the CoMPASS software distribued by CAEN.
 Author: Chloé Legué
 Author-email: chloe.legue@mail.mcgill.ca
 Project-URL: Repository, https://github.com/Chujo58/ReadROOT
 Project-URL: Documentation, https://github.com/Chujo58/ReadROOT/wiki
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ReadROOT-2.5.7/QtClasses.py` & `ReadROOT-2.5.8/QtClasses.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/ReadROOT.egg-info/PKG-INFO` & `ReadROOT-2.5.8/ReadROOT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReadROOT
-Version: 2.5.7
+Version: 2.5.8
 Summary: Easy GUI made to read ROOT files created by the CoMPASS software distribued by CAEN.
 Author: Chloé Legué
 Author-email: chloe.legue@mail.mcgill.ca
 Project-URL: Repository, https://github.com/Chujo58/ReadROOT
 Project-URL: Documentation, https://github.com/Chujo58/ReadROOT/wiki
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ReadROOT-2.5.7/ReadROOT.egg-info/SOURCES.txt` & `ReadROOT-2.5.8/ReadROOT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/ValidInputs.py` & `ReadROOT-2.5.8/ValidInputs.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/XML_Parser.py` & `ReadROOT-2.5.8/XML_Parser.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/__init__.py` & `ReadROOT-2.5.8/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os, sys, matplotlib, json, difflib #type: ignore
 running_directory = os.getcwd() #This is to make the relative import work!
 path = os.path.dirname(os.path.abspath(__file__))
 os.chdir(path)
 sys.path.append(path) #FOR C++ TO WORK!
 
-__version__ = '2.5.7'
+__version__ = '2.5.8'
 
 from . import read_root
 from . import read_root_gui
 from . import read_root_gui_v2
 from . import IOClasses
 from . import QtClasses
 from . import root_plotter
```

### Comparing `ReadROOT-2.5.7/config.json` & `ReadROOT-2.5.8/config.json`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/discord.mp3` & `ReadROOT-2.5.8/discord.mp3`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/funcs.cpp` & `ReadROOT-2.5.8/funcs.cpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/funcs.hpp` & `ReadROOT-2.5.8/funcs.hpp`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/merge/merge_root_files.py` & `ReadROOT-2.5.8/merge/merge_root_files.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/read_root.py` & `ReadROOT-2.5.8/read_root.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/read_root_gui.py` & `ReadROOT-2.5.8/read_root_gui.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/read_root_gui_v2.py` & `ReadROOT-2.5.8/read_root_gui_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #----------------------------------------------------------------------------
 # Created by : Chloé Legué
 # Current version date : 2024/04/12
-# Version = 2.5.7
+# Version = 2.5.8
 #----------------------------------------------------------------------------
 """
 This code was made for the coincidence experiment at McGill University. 
 
 The code allows the user to choose a folder containing the results saved from the CoMPASS software from CAEN. This code should be used with the CAEN DT5751, or any other digitizer from CAEN that work in the same way.
 
 This code is able to reproduce the important graphs that the CoMPASS software makes like MCS Graph, Energy Histogram and TOF Histogram. Other graphs can be added if needed.
```

### Comparing `ReadROOT-2.5.7/reload.py` & `ReadROOT-2.5.8/reload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 import time, shutil, os
 version_date = datetime.now().strftime('%Y/%m/%d')
-version_number = "2.5.7"
+version_number = "2.5.8"
 
 with open("READme.md", "r") as f:
     read_me = f.readlines()
 
 with open("setup.py", "r") as f:
     setup = f.readlines()
```

### Comparing `ReadROOT-2.5.7/root_plotter.py` & `ReadROOT-2.5.8/root_plotter.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/setup.py` & `ReadROOT-2.5.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.5.7"
+__version__ = "2.5.8"
 
 from setuptools import setup
 
 description = open("READme.md").read()
 
 setup(
     name = "ReadROOT",
```

### Comparing `ReadROOT-2.5.7/test/test_cpp.py` & `ReadROOT-2.5.8/test/test_cpp.py`

 * *Files identical despite different names*

### Comparing `ReadROOT-2.5.7/wrap.cpp` & `ReadROOT-2.5.8/wrap.cpp`

 * *Files identical despite different names*

