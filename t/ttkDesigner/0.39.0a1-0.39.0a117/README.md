# Comparing `tmp/ttkDesigner-0.39.0a1.tar.gz` & `tmp/ttkdesigner-0.39a117.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttkDesigner-0.39.0a1.tar", last modified: Thu Feb 22 14:04:20 2024, max compression
+gzip compressed data, was "ttkdesigner-0.39a117.tar", last modified: Fri Apr 12 16:42:04 2024, max compression
```

## Comparing `ttkDesigner-0.39.0a1.tar` & `ttkdesigner-0.39a117.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/
--rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-02-22 14:04:16.000000 ttkDesigner-0.39.0a1/LICENSE
--rw-r--r--   0 one       (1000) one       (1000)     2959 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     2094 2024-02-22 14:04:16.000000 ttkDesigner-0.39.0a1/README.md
--rw-rw-r--   0 one       (1000) one       (1000)       38 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/setup.cfg
--rw-rw-r--   0 one       (1000) one       (1000)     1407 2024-02-22 14:04:16.000000 ttkDesigner-0.39.0a1/setup.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.408336 ttkDesigner-0.39.0a1/ttkDesigner/
--rwxrwxr-x   0 one       (1000) one       (1000)     1215 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     1218 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/__main__.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.408336 ttkDesigner-0.39.0a1/ttkDesigner/app/
--rw-rw-r--   0 one       (1000) one       (1000)     1610 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     3305 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/about.py
--rw-rw-r--   0 one       (1000) one       (1000)     1351 2024-02-22 14:04:16.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/cfg.py
--rw-rw-r--   0 one       (1000) one       (1000)    24097 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/designer.py
--rw-rw-r--   0 one       (1000) one       (1000)     2159 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/main.py
--rw-rw-r--   0 one       (1000) one       (1000)    17565 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/menuBarEditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     8701 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/notepad.py
--rw-rw-r--   0 one       (1000) one       (1000)    13152 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/propertyeditor.py
--rw-rw-r--   0 one       (1000) one       (1000)     3714 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/quickexport.py
--rw-rw-r--   0 one       (1000) one       (1000)     9451 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/signalsloteditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/
--rw-rw-r--   0 one       (1000) one       (1000)     1897 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/__init__.py
--rw-rw-r--   0 one       (1000) one       (1000)     4431 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/supercontrol.py
--rw-rw-r--   0 one       (1000) one       (1000)     9725 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayout.py
--rw-rw-r--   0 one       (1000) one       (1000)    16614 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayoutgrid.py
--rw-rw-r--   0 one       (1000) one       (1000)     1481 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayouthbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     1479 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayoutvbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     4008 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superobj.py
--rw-rw-r--   0 one       (1000) one       (1000)    10223 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidget.py
--rw-rw-r--   0 one       (1000) one       (1000)     1849 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetabstractscrollarea.py
--rw-rw-r--   0 one       (1000) one       (1000)     5235 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetcontainer.py
--rw-rw-r--   0 one       (1000) one       (1000)     3516 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetframe.py
--rw-rw-r--   0 one       (1000) one       (1000)     1319 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetlist.py
--rw-rw-r--   0 one       (1000) one       (1000)     2305 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetmenubutton.py
--rw-rw-r--   0 one       (1000) one       (1000)     1701 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetradiobutton.py
--rw-rw-r--   0 one       (1000) one       (1000)     1697 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetsplitter.py
--rw-rw-r--   0 one       (1000) one       (1000)     1809 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgettextedit.py
--rw-rw-r--   0 one       (1000) one       (1000)     9941 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/treeinspector.py
--rw-rw-r--   0 one       (1000) one       (1000)     8824 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/widgetbox.py
--rw-rw-r--   0 one       (1000) one       (1000)     4791 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/app/windoweditor.py
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/ttkDesigner/tui/
--rw-rw-r--   0 one       (1000) one       (1000)     4550 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/tui/menuBarEditor.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     7841 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/tui/newWindow.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     3727 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/tui/quickExport.tui.json
--rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-02-22 14:00:52.000000 ttkDesigner-0.39.0a1/ttkDesigner/tui/quickImport.tui.json
-drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-02-22 14:04:20.412336 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/
--rw-r--r--   0 one       (1000) one       (1000)     2959 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1000) one       (1000)     1537 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1000) one       (1000)        1 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1000) one       (1000)       49 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/entry_points.txt
--rw-rw-r--   0 one       (1000) one       (1000)       35 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/requires.txt
--rw-rw-r--   0 one       (1000) one       (1000)       12 2024-02-22 14:04:20.000000 ttkDesigner-0.39.0a1/ttkDesigner.egg-info/top_level.txt
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/
+-rw-rw-r--   0 one       (1000) one       (1000)     1118 2024-04-12 16:42:00.000000 ttkdesigner-0.39a117/LICENSE
+-rw-r--r--   0 one       (1000) one       (1000)     3449 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     2100 2024-04-12 16:42:00.000000 ttkdesigner-0.39a117/README.md
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/setup.cfg
+-rw-rw-r--   0 one       (1000) one       (1000)     2705 2024-04-12 16:42:00.000000 ttkdesigner-0.39a117/setup.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/ttkDesigner/
+-rwxrwxr-x   0 one       (1000) one       (1000)     1215 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1218 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/__main__.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/ttkDesigner/app/
+-rw-rw-r--   0 one       (1000) one       (1000)     1610 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3305 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/about.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1353 2024-04-12 16:42:00.000000 ttkdesigner-0.39a117/ttkDesigner/app/cfg.py
+-rw-rw-r--   0 one       (1000) one       (1000)    23725 2024-03-29 23:15:44.000000 ttkdesigner-0.39a117/ttkDesigner/app/designer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2182 2024-02-27 17:36:09.000000 ttkdesigner-0.39a117/ttkDesigner/app/main.py
+-rw-rw-r--   0 one       (1000) one       (1000)    17565 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/menuBarEditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     8545 2024-02-29 11:36:39.000000 ttkdesigner-0.39a117/ttkDesigner/app/notepad.py
+-rw-rw-r--   0 one       (1000) one       (1000)    13152 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/propertyeditor.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3714 2024-01-11 10:32:39.000000 ttkdesigner-0.39a117/ttkDesigner/app/quickexport.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9451 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/signalsloteditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/ttkDesigner/app/superobj/
+-rw-rw-r--   0 one       (1000) one       (1000)     1897 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/__init__.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4431 2024-02-06 10:28:08.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/supercontrol.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9725 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayout.py
+-rw-rw-r--   0 one       (1000) one       (1000)    16614 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayoutgrid.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1481 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayouthbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1479 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayoutvbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4008 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superobj.py
+-rw-rw-r--   0 one       (1000) one       (1000)    10223 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidget.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1849 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetabstractscrollarea.py
+-rw-rw-r--   0 one       (1000) one       (1000)     5235 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetcontainer.py
+-rw-rw-r--   0 one       (1000) one       (1000)     3516 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetframe.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1319 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetlist.py
+-rw-rw-r--   0 one       (1000) one       (1000)     2305 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetmenubutton.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1701 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetradiobutton.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1697 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetsplitter.py
+-rw-rw-r--   0 one       (1000) one       (1000)     1809 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgettextedit.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9941 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/app/treeinspector.py
+-rw-rw-r--   0 one       (1000) one       (1000)     9160 2024-03-29 23:17:16.000000 ttkdesigner-0.39a117/ttkDesigner/app/widgetbox.py
+-rw-rw-r--   0 one       (1000) one       (1000)     4791 2024-02-04 11:52:54.000000 ttkdesigner-0.39a117/ttkDesigner/app/windoweditor.py
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/ttkDesigner/tui/
+-rw-rw-r--   0 one       (1000) one       (1000)     4550 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/tui/menuBarEditor.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     7841 2024-01-10 23:26:14.000000 ttkdesigner-0.39a117/ttkDesigner/tui/newWindow.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     3727 2023-12-14 10:00:21.000000 ttkdesigner-0.39a117/ttkDesigner/tui/quickExport.tui.json
+-rw-rw-r--   0 one       (1000) one       (1000)     2201 2024-01-11 10:32:39.000000 ttkdesigner-0.39a117/ttkDesigner/tui/quickImport.tui.json
+drwxrwxr-x   0 one       (1000) one       (1000)        0 2024-04-12 16:42:04.537133 ttkdesigner-0.39a117/ttkDesigner.egg-info/
+-rw-r--r--   0 one       (1000) one       (1000)     3449 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1000) one       (1000)     1537 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1000) one       (1000)        1 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       49 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       38 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/requires.txt
+-rw-rw-r--   0 one       (1000) one       (1000)       12 2024-04-12 16:42:04.000000 ttkdesigner-0.39a117/ttkDesigner.egg-info/top_level.txt
```

### Comparing `ttkDesigner-0.39.0a1/LICENSE` & `ttkdesigner-0.39a117/LICENSE`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/PKG-INFO` & `ttkdesigner-0.39a117/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.39.0a1
+Version: 0.39.0a117
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Terminals
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Terminals
+Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyTermTk>=0.39.0a
+Requires-Dist: pyTermTk>=0.39.0a116
 Requires-Dist: pyperclip
 Requires-Dist: Pillow
 
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
-![Python](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
+![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/ttkDesigner)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 [![screenshot](https://user-images.githubusercontent.com/8876552/236525667-dcdcec6e-1066-4294-bdb0-db98ef8850da.png)](https://pypi.org/project/ttkDesigner)
 
-## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/ttkDesigner)
+## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/ttkDesigner)
 
 **ttkDesigner** is the [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) tool for designing and building Text-based user interfaces ([TUI](https://en.wikipedia.org/wiki/Text-based_user_interface)s) with [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) Widgets. You can compose and customize your windows or dialogs in a what-you-see-is-what-you-get (WYSIWYG) manner, and test them interactively.
 
 Widgets and forms created with **ttkDesigner** integrate seamlessly with programmed code, using [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk)'s signals and slots mechanism, so that you can easily assign behavior to graphical elements. All properties set in **ttkDesigner** can be changed dynamically within the code.
 
 ## Features
 tbd
```

### Comparing `ttkDesigner-0.39.0a1/README.md` & `ttkdesigner-0.39a117/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
-![Python](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
+![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/ttkDesigner)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 [![screenshot](https://user-images.githubusercontent.com/8876552/236525667-dcdcec6e-1066-4294-bdb0-db98ef8850da.png)](https://pypi.org/project/ttkDesigner)
 
-## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/ttkDesigner)
+## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/ttkDesigner)
 
 **ttkDesigner** is the [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) tool for designing and building Text-based user interfaces ([TUI](https://en.wikipedia.org/wiki/Text-based_user_interface)s) with [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) Widgets. You can compose and customize your windows or dialogs in a what-you-see-is-what-you-get (WYSIWYG) manner, and test them interactively.
 
 Widgets and forms created with **ttkDesigner** integrate seamlessly with programmed code, using [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk)'s signals and slots mechanism, so that you can easily assign behavior to graphical elements. All properties set in **ttkDesigner** can be changed dynamically within the code.
 
 ## Features
 tbd
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/__init__.py` & `ttkdesigner-0.39a117/ttkDesigner/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/__main__.py` & `ttkdesigner-0.39a117/ttkDesigner/__main__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/__init__.py` & `ttkdesigner-0.39a117/ttkDesigner/app/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/about.py` & `ttkdesigner-0.39a117/ttkDesigner/app/about.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/cfg.py` & `ttkdesigner-0.39a117/ttkDesigner/app/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import os
 # import yaml
 
 class TTkDesignerCfg:
-    version="0.39.0-a1"
+    version="0.39.0-a117"
     name="ttkDesigner"
     cfgVersion = '1.0'
     pathCfg="."
     options={}
     maxsearches=200
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/designer.py` & `ttkdesigner-0.39a117/ttkDesigner/app/designer.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 from TermTk import pyTTkSlot, pyTTkSignal
 
 from TermTk import TTkWidget, TTkFrame, TTkButton, TTkLabel, TTkMenuButton
 from TermTk import TTkTabWidget
 from TermTk import TTkFileDialogPicker, TTkMessageBox
 
 from TermTk import TTkGridLayout, TTkVBoxLayout, TTkHBoxLayout
-from TermTk import TTkSplitter
+from TermTk import TTkSplitter, TTkAppTemplate, TTkMenuBarLayout
 from TermTk import TTkLogViewer, TTkKeyPressView
-from TermTk import TTkUiLoader, TTkUtil
+from TermTk import TTkUiLoader, TTkUiSignature, TTkUtil
 
 from .cfg  import *
 from .about import *
 from .widgetbox import WidgetBoxScrollArea
 from .windoweditor import WindowEditor
 from .treeinspector import TreeInspector
 from .propertyeditor import PropertyEditor
@@ -72,15 +72,15 @@
 #      │                     ║└─────────────────────────────┘║   Signal/Slot     │
 #      │                     ╟───────────────────────────────╢                   │
 #      │                     ║     LOG Viewer                ║   Editor          │
 #      │                     ║                               ║                   │
 #      └─────────────────────╨───────────────────────────────╨───────────────────┘
 #
 
-class TTkDesigner(TTkGridLayout):
+class TTkDesigner(TTkAppTemplate):
     __slots__ = ('_main', '_toolBar', '_fileNameLabel', '_modified',
                  '_sigslotEditor', '_treeInspector', '_windowEditor', '_notepad',
                  '_fileName', '_currentPath',
                  '_snapshot', '_snapId', '_snapSaved',
                  # Signals
                  'weModified', 'thingSelected', 'widgetNameChanged'
                  )
@@ -92,88 +92,77 @@
         self.thingSelected = pyTTkSignal(TTkWidget, TTkWidget)
         self.widgetNameChanged = pyTTkSignal(str, str)
 
         self.resetSnapshot()
 
         super().__init__(*args, **kwargs)
 
-        self.addWidget(mainSplit := TTkSplitter())
-        mainSplit.addItem(widgetBoxLayout := TTkVBoxLayout())
-        #mainSplit.addWidget(TTkButton(text='A',border=True))
-
-        # mainSplit.addWidget(sa := TTkScrollArea())
-        # sa.viewport().setLayout(TTkGridLayout())
-        # sa.viewport().layout().addWidget(WindowEditor())
+        appTemplate = self
 
         self._notepad = NotePad()
         self._main = TTkVBoxLayout()
         self._toolBar = TTkHBoxLayout()
         self._windowEditor = WindowEditor(self)
         self._sigslotEditor = SignalSlotEditor(self)
         self._treeInspector = TreeInspector(self, self._windowEditor.viewport())
         self._fileNameLabel = TTkLabel(text=f"( {self._fileName} )", alignment=TTkK.CENTER_ALIGN)
 
-        widgetBoxLayout.addWidget(topMenuFrame := TTkFrame(minHeight=1,maxHeight=1,border=False))
-        widgetBoxLayout.addWidget(WidgetBoxScrollArea(self))
+        appTemplate.setWidget(WidgetBoxScrollArea(self), TTkAppTemplate.LEFT, 25)
 
         self._main.addItem(self._toolBar)
         self._main.addWidget(self._windowEditor)
 
-        mainSplit.addWidget(centralSplit := TTkSplitter(orientation=TTkK.VERTICAL))
-        centralSplit.addWidget(self._main)
-        centralSplit.addWidget(bottonTabWidget := TTkTabWidget(border=False))
+        appTemplate.setItem(self._main, TTkAppTemplate.MAIN)
+        appTemplate.setWidget(bottonTabWidget := TTkTabWidget(border=False), TTkAppTemplate.BOTTOM, 8)
         # centralSplit.addWidget(TTkLogViewer())
         bottonTabWidget.addTab(self._sigslotEditor,'Signal/Slot Editor')
         bottonTabWidget.addTab(TTkLogViewer(),'Logs')
 
-        mainSplit.addWidget(rightSplit := TTkSplitter(orientation=TTkK.VERTICAL))
+        appTemplate.setWidget(rightSplit := TTkSplitter(orientation=TTkK.VERTICAL), TTkAppTemplate.RIGHT, 42)
 
         rightSplit.addItem(self._treeInspector)
         rightSplit.addItem(propertyEditor := PropertyEditor(), title="Property Editor")
         # rightSplit.addItem(self._sigslotEditor)
 
         self.thingSelected.connect(lambda _,s : s.pushSuperControlWidget() if s.hasControlWidget() else None)
         self.thingSelected.connect(propertyEditor.setDetail)
 
         self.weModified.connect(self._treeInspector.refresh)
         self.weModified.connect(self._takeSnapshot)
 
-        fileMenu = topMenuFrame.newMenubarTop().addMenu("&File")
+        appTemplate.setMenuBar(appMenuBar:=TTkMenuBarLayout(), TTkAppTemplate.LEFT)
+        fileMenu = appMenuBar.addMenu("&File")
         fileMenu.addMenu("&New").menuButtonClicked.connect(self.new)
         fileMenu.addMenu("&Open").menuButtonClicked.connect(self.open)
         fileMenu.addMenu("&Save").menuButtonClicked.connect(self.save)
         fileMenu.addMenu("Save &As...").menuButtonClicked.connect(self.saveAs)
         fileMenu.addSpacer()
         fileMenu.addMenu("&Import 🎁").menuButtonClicked.connect(self.importDictWin)
         fileMenu.addMenu("&Export 📦").menuButtonClicked.connect(self.quickExport)
         fileMenu.addSpacer()
         fileMenu.addMenu("E&xit").menuButtonClicked.connect(self.quit)
 
-        extraMenu = topMenuFrame.newMenubarTop().addMenu("E&dit")
+        extraMenu = appMenuBar.addMenu("E&dit")
         extraMenu.addMenu("&Undo (CTRL+Z)").menuButtonClicked.connect(self.undo)
         extraMenu.addMenu("&Redo (CTRL+Y)").menuButtonClicked.connect(self.redo)
         extraMenu.addSpacer()
         extraMenu.addMenu("&Scratchpad 📝").menuButtonClicked.connect(self.scratchpad)
         extraMenu.addMenu("&KeypressView").menuButtonClicked.connect(self.keypressview)
         extraMenu.addSpacer()
         extraMenu.addMenu("&Preview...").menuButtonClicked.connect(self.preview)
 
         def _showAbout(btn):
             TTkHelper.overlay(None, About(), 30,10)
         def _showAboutTTk(btn):
             TTkHelper.overlay(None, TTkAbout(), 30,10)
 
-        helpMenu = topMenuFrame.newMenubarTop().addMenu("&Help", alignment=TTkK.RIGHT_ALIGN)
+        helpMenu = appMenuBar.addMenu("&Help", alignment=TTkK.RIGHT_ALIGN)
         helpMenu.addMenu("About ...").menuButtonClicked.connect(_showAbout)
         helpMenu.addMenu("About ttk").menuButtonClicked.connect(_showAboutTTk)
 
-        w,_ = self.size()
-        mainSplit.setSizes([25,None,42])
-        centralSplit.setSizes([None,8])
-
         self._toolBar.addWidget(btnPreview := TTkButton(maxWidth=12, text='Preview...'))
         self._toolBar.addWidget(btnExport := TTkButton(maxWidth=17, text='Quick Export 📦'))
         self._toolBar.addWidget(btnColors  := TTkButton(maxWidth=11, checkable=True, text=
                             TTkString("▣",TTkColor.fg("#ff0000")) +
                             TTkString("▣",TTkColor.fg("#ffff00")) +
                             TTkString("▣",TTkColor.fg("#00ff00")) +
                             TTkString("▣",TTkColor.fg("#00ffff")) +
@@ -398,14 +387,15 @@
                 if m := re.match(r'^ *["\']([A-Za-z0-9+/]+[=]{0,2})["\' +]*$',_t):
                     ret += m.group(1)
                 elif not re.match(r'^ *$',_t): # exclude empty lines
                     return ""
             return ret
         newWindow = TTkUiLoader.loadFile(os.path.join(os.path.dirname(os.path.abspath(__file__)),"../tui/quickImport.tui.json"))
         te = newWindow.getWidgetByName("TextEdit")
+        @pyTTkSlot()
         def _importDict(te=te):
             text = te.toPlainText()
             if compressed := _probeCompressedText(text):
                 dd = TTkUtil.base64_deflate_2_obj(compressed)
             else:
                 try:
                     dd = eval(text)
@@ -461,15 +451,16 @@
     def _saveToFile(self, fileName):
         TTkLog.info(f"Saving to: {fileName}")
         self._updateFileName(fileName)
 
         tui = self._windowEditor.dumpDict()
         connections = self._sigslotEditor.dumpDict()
         newUI = {
-            'version':'2.0.0',
+            'type': TTkUiSignature,
+            'version':'2.0.2',
             'tui':tui,
             'connections':connections}
         jj =  json.dumps(newUI, indent=1)
 
         with open(fileName,'w') as fp:
             fp.write(jj)
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/main.py` & `ttkdesigner-0.39a117/ttkDesigner/app/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,36 +19,36 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import argparse
 
 from TermTk import TTk, TTkTheme, TTkTerm
-from TermTk import TTkVBoxLayout, TTkKeyPressView
+from TermTk import TTkGridLayout, TTkKeyPressView
 
 from .designer import TTkDesigner
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('filename', type=str, nargs='?', help='the file to open')
     parser.add_argument('-k', '--showkeys', action='store_true', help='display the keypresses and mouse interactions')
     args = parser.parse_args()
 
     TTkTheme.loadTheme( TTkTheme.NERD )
 
     root = TTk(
             title="TTk Designer",
             mouseTrack=True,
+            layout=TTkGridLayout(),
             sigmask=(
                 TTkTerm.Sigmask.CTRL_C |
                 TTkTerm.Sigmask.CTRL_Q |
                 TTkTerm.Sigmask.CTRL_S |
                 TTkTerm.Sigmask.CTRL_Z ))
 
+    root.layout().addWidget(_d:=TTkDesigner(fileName=args.filename))
+
     if args.showkeys:
-        root.setLayout(_l:=TTkVBoxLayout())
-        _l.addItem(TTkDesigner(fileName=args.filename))
-        _l.addWidget(TTkKeyPressView(maxHeight=3))
-    else:
-        root.setLayout(TTkDesigner(fileName=args.filename))
+        _d.setWidget(widget=TTkKeyPressView(maxHeight=3), position=_d.FOOTER, size=3)
+        _d.setFixed(fixed=True, position=_d.FOOTER)
 
     root.mainloop()
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/menuBarEditor.py` & `ttkdesigner-0.39a117/ttkDesigner/app/menuBarEditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/notepad.py` & `ttkdesigner-0.39a117/ttkDesigner/app/notepad.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,23 +121,23 @@
             if btn_strikethrough.isChecked():
                 color += ttk.TTkColor.STRIKETROUGH
             cursor = te.textCursor()
             cursor.applyColor(color)
             cursor.setColor(color)
             te.setFocus()
 
-        cb_fg.stateChanged.connect(lambda x: btn_fgColor.setEnabled(x==ttk.TTkK.Checked))
-        cb_bg.stateChanged.connect(lambda x: btn_bgColor.setEnabled(x==ttk.TTkK.Checked))
-        cb_fg.clicked.connect(lambda _: _setStyle())
-        cb_bg.clicked.connect(lambda _: _setStyle())
+        cb_fg.toggled.connect(btn_fgColor.setEnabled)
+        cb_bg.toggled.connect(btn_bgColor.setEnabled)
+        cb_fg.clicked.connect(_setStyle)
+        cb_bg.clicked.connect(_setStyle)
 
-        cb_linenumber.stateChanged.connect(lambda x: te.setLineNumber(x==ttk.TTkK.Checked))
+        cb_linenumber.toggled.connect(te.setLineNumber)
 
-        btn_fgColor.colorSelected.connect(lambda _: _setStyle())
-        btn_bgColor.colorSelected.connect(lambda _: _setStyle())
+        btn_fgColor.colorSelected.connect(_setStyle)
+        btn_bgColor.colorSelected.connect(_setStyle)
 
         btn_bold.clicked.connect(_setStyle)
         btn_italic.clicked.connect(_setStyle)
         btn_underline.clicked.connect(_setStyle)
         btn_strikethrough.clicked.connect(_setStyle)
 
         lineWrap.setCurrentIndex(0)
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/propertyeditor.py` & `ttkdesigner-0.39a117/ttkDesigner/app/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/quickexport.py` & `ttkdesigner-0.39a117/ttkDesigner/app/quickexport.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/signalsloteditor.py` & `ttkdesigner-0.39a117/ttkDesigner/app/signalsloteditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/__init__.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/__init__.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/supercontrol.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/supercontrol.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayout.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayout.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayoutgrid.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayoutgrid.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayouthbox.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayouthbox.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superlayoutvbox.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superlayoutvbox.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superobj.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superobj.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidget.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidget.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetabstractscrollarea.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetabstractscrollarea.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetcontainer.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetcontainer.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetframe.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetframe.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetlist.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetlist.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetmenubutton.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetmenubutton.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetradiobutton.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetradiobutton.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgetsplitter.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgetsplitter.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/superobj/superwidgettextedit.py` & `ttkdesigner-0.39a117/ttkDesigner/app/superobj/superwidgettextedit.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/treeinspector.py` & `ttkdesigner-0.39a117/ttkDesigner/app/treeinspector.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/widgetbox.py` & `ttkdesigner-0.39a117/ttkDesigner/app/widgetbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,29 @@
         "ComboBox"    : { "class":ttk.TTkComboBox,  "params":{'size':(20,1)} },
         "LineEdit"    : { "class":ttk.TTkLineEdit,  "params":{'size':(20,1)} },
         "TextEdit"    : { "class":ttk.TTkTextEdit,  "params":{'size':(20,5), 'readOnly':False, 'multiline':True } },
         "TextEditLine": { "class":ttk.TTkTextEdit,  "params":{'size':(20,1), 'readOnly':False, 'multiLine':False, 'maxHeight':1 } },
         "SpinBox"     : { "class":ttk.TTkSpinBox,   "params":{'size':(20,1)} },
         "H ScrollBar" : { "class":ttk.TTkScrollBar, "params":{'size':(10,1), "orientation":ttk.TTkK.HORIZONTAL} },
         "V ScrollBar" : { "class":ttk.TTkScrollBar, "params":{'size':(1,5),  "orientation":ttk.TTkK.VERTICAL} },
+        "H Slider"    : { "class":ttk.TTkSlider,    "params":{'size':(10,1), "orientation":ttk.TTkK.HORIZONTAL} },
+        "V Slider"    : { "class":ttk.TTkSlider,    "params":{'size':(1,5),  "orientation":ttk.TTkK.VERTICAL} },
     },
     'Widgets':{
         "Label"           : { "class":ttk.TTkLabel,          "params":{'size':(20,1), 'text':'Label'}},
         "List"            : { "class":ttk.TTkList,           "params":{'size':(20,5)}},
         # "List Widget"     : { "class":ttk.TTkListWidget,     "params":{'size':(20,5)}},
         "Scroll Area"     : { "class":ttk.TTkScrollArea,     "params":{'size':(20,5)}, "disabled": True},
         "Spacer"          : { "class":ttk.TTkSpacer,         "params":{'size':(10,5)}},
         "Tab Widget"      : { "class":ttk.TTkTabWidget,      "params":{'size':(20,3)}, "disabled": True},
         "Widget"          : { "class":ttk.TTkWidget,         "params":{'size':(20,5)}},
     },
     'Pickers':{
         "Color Picker"     : { "class":ttk.TTkColorButtonPicker, "params":{'size':( 6,3), 'border':True}},
+        "Color Picker Slim": { "class":ttk.TTkColorButtonPicker, "params":{'size':( 6,1), 'border':False}},
         "File Picker"      : { "class":ttk.TTkFileButtonPicker,  "params":{'size':(20,3), 'border':True}},
         "Date Picker"      : { "class":ttk.TTkButton, "params":{'size':(20,3)}, "disabled": True},
         "TtkString Picker" : { "class":ttk.TTkButton, "params":{'size':(20,3)}, "disabled": True},
     },
     'Debug':{
         "Log Viewer"       : { "class":ttk.TTkLogViewer,       "params":{'size':(60,10)}},
         "Input View"       : { "class":ttk.TTkKeyPressView,    "params":{'size':(60,3)}},
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/app/windoweditor.py` & `ttkdesigner-0.39a117/ttkDesigner/app/windoweditor.py`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/tui/menuBarEditor.tui.json` & `ttkdesigner-0.39a117/ttkDesigner/tui/menuBarEditor.tui.json`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/tui/newWindow.tui.json` & `ttkdesigner-0.39a117/ttkDesigner/tui/newWindow.tui.json`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/tui/quickExport.tui.json` & `ttkdesigner-0.39a117/ttkDesigner/tui/quickExport.tui.json`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner/tui/quickImport.tui.json` & `ttkdesigner-0.39a117/ttkDesigner/tui/quickImport.tui.json`

 * *Files identical despite different names*

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner.egg-info/PKG-INFO` & `ttkdesigner-0.39a117/ttkDesigner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 Metadata-Version: 2.1
 Name: ttkDesigner
-Version: 0.39.0a1
+Version: 0.39.0a117
 Summary: ttkDesigner is a terminal user interface designer for pyTermTk applications
 Home-page: https://github.com/ceccopierangiolieugenio/pyTermTk
 Author: Eugenio Parodi
 Author-email: ceccopierangiolieugenio@googlemail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Terminals
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Terminals
+Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyTermTk>=0.39.0a
+Requires-Dist: pyTermTk>=0.39.0a116
 Requires-Dist: pyperclip
 Requires-Dist: Pillow
 
 ![Linux](https://img.shields.io/badge/-Linux-grey?logo=linux)
 ![Usage](https://img.shields.io/badge/Usage-Terminal%20User%20Interface-yellow)
-![Python](https://img.shields.io/badge/Python-v3.8%5E-green?logo=python)
+![Python](https://img.shields.io/badge/Python-v3.9%5E-green?logo=python)
 ![pyTermTk_version](https://img.shields.io/github/v/tag/ceccopierangiolieugenio/pyTermTk?label=version)
 [![Test Status](https://img.shields.io/github/actions/workflow/status/ceccopierangiolieugenio/pyTermTk/testing.yml?branch=main&label=tests)](https://github.com/ceccopierangiolieugenio/pyTermTk/actions?query=workflow%3Atesting)
 [![pypi_version](https://img.shields.io/pypi/v/ttkDesigner?label=pypi)](https://pypi.org/project/ttkDesigner)
 [![pypi_version](https://img.shields.io/twitter/follow/Pier95886803?style=social&logo=twitter)](https://twitter.com/hashtag/pyTermTk?src=hashtag_click&f=live)
 
 [![screenshot](https://user-images.githubusercontent.com/8876552/236525667-dcdcec6e-1066-4294-bdb0-db98ef8850da.png)](https://pypi.org/project/ttkDesigner)
 
-## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/ttkDesigner)
+## [ttkDesigner](https://github.com/ceccopierangiolieugenio/pyTermTk/tree/main/tools/ttkDesigner)
 
 **ttkDesigner** is the [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) tool for designing and building Text-based user interfaces ([TUI](https://en.wikipedia.org/wiki/Text-based_user_interface)s) with [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk) Widgets. You can compose and customize your windows or dialogs in a what-you-see-is-what-you-get (WYSIWYG) manner, and test them interactively.
 
 Widgets and forms created with **ttkDesigner** integrate seamlessly with programmed code, using [pyTermTk](https://github.com/ceccopierangiolieugenio/pyTermTk)'s signals and slots mechanism, so that you can easily assign behavior to graphical elements. All properties set in **ttkDesigner** can be changed dynamically within the code.
 
 ## Features
 tbd
```

### Comparing `ttkDesigner-0.39.0a1/ttkDesigner.egg-info/SOURCES.txt` & `ttkdesigner-0.39a117/ttkDesigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

