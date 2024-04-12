# Comparing `tmp/smartbetsAPI-1.2.6.tar.gz` & `tmp/smartbetsAPI-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartbetsAPI-1.2.6.tar", last modified: Wed Apr 10 16:39:51 2024, max compression
+gzip compressed data, was "smartbetsAPI-1.2.7.tar", last modified: Fri Apr 12 04:38:58 2024, max compression
```

## Comparing `smartbetsAPI-1.2.6.tar` & `smartbetsAPI-1.2.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:39:51.402396 smartbetsAPI-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-10 16:39:51.402396 smartbetsAPI-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 16:39:51.402396 smartbetsAPI-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:39:51.402396 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 16:39:51.000000 smartbetsAPI-1.2.6/smartbetsAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:39:51.402396 smartbetsAPI-1.2.6/smartbets_API/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/bet_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/bet_at_rest_api_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/bet_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/configuration_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6613 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/figure_harvester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/googler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/html_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/proxyh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-10 16:39:47.000000 smartbetsAPI-1.2.6/smartbets_API/tertiary_bet.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-12 04:38:58.792915 smartbetsAPI-1.2.7/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    35149 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.7/LICENSE
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11506 2024-04-12 04:38:58.792915 smartbetsAPI-1.2.7/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     9356 2024-04-12 04:35:47.000000 smartbetsAPI-1.2.7/README.md
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       38 2024-04-12 04:38:58.792915 smartbetsAPI-1.2.7/setup.cfg
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2414 2024-04-10 16:38:22.000000 smartbetsAPI-1.2.7/setup.py
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-12 04:38:58.789582 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11506 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      629 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)        1 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       70 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/entry_points.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      102 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/requires.txt
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       14 2024-04-12 04:38:58.000000 smartbetsAPI-1.2.7/smartbetsAPI.egg-info/top_level.txt
+drwxr-xr-x   0 smartwa   (1000) smartwa   (1001)        0 2024-04-12 04:38:58.789582 smartbetsAPI-1.2.7/smartbets_API/
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)      189 2024-04-12 04:35:47.000000 smartbetsAPI-1.2.7/smartbets_API/__init__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)       52 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.7/smartbets_API/__main__.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2050 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.7/smartbets_API/bet_analyzer.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2747 2024-04-10 15:00:40.000000 smartbetsAPI-1.2.7/smartbets_API/bet_at_rest_api_level.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)    11318 2024-04-10 16:38:22.000000 smartbetsAPI-1.2.7/smartbets_API/bet_common.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     4473 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.7/smartbets_API/configuration_handler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6613 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.7/smartbets_API/figure_harvester.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     3065 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.7/smartbets_API/googler.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6394 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.7/smartbets_API/html_fetcher.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     6806 2024-04-12 04:35:47.000000 smartbetsAPI-1.2.7/smartbets_API/interface.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     8859 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.7/smartbets_API/predictor.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     1851 2024-04-10 13:33:04.000000 smartbetsAPI-1.2.7/smartbets_API/proxyh.py
+-rw-r--r--   0 smartwa   (1000) smartwa   (1001)     2201 2024-04-10 09:28:50.000000 smartbetsAPI-1.2.7/smartbets_API/tertiary_bet.py
```

### Comparing `smartbetsAPI-1.2.6/LICENSE` & `smartbetsAPI-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/PKG-INFO` & `smartbetsAPI-1.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -41,15 +41,15 @@
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/pypi/v/smartbetsAPI?color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.6 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.7 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.6/README.md` & `smartbetsAPI-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1 align="center">smartbetsAPI</h1>
 <p align="center">
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/pypi/v/smartbetsAPI?color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
  
  > "Punter's choice" 
 
  Worldwide soccer-matches predictor with Fast-API and a package for integrating the scripts in your own [Python](https://python.org) code.
 
  ## Features
```

### Comparing `smartbetsAPI-1.2.6/setup.py` & `smartbetsAPI-1.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbetsAPI.egg-info/PKG-INFO` & `smartbetsAPI-1.2.7/smartbetsAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartbetsAPI
-Version: 1.2.6
+Version: 1.2.7
 Summary: Simple football prediction API
 Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa Caleb
 Maintainer-email: smartwacaleb@gmail.com
 License: GPL-3.0
@@ -41,15 +41,15 @@
 Requires-Dist: bs4==0.0.1
 Requires-Dist: Faker==15.3.4
 
 <h1 align="center">smartbetsAPI</h1>
 
 <p align="center">
 
- <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v1.2.6&color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
+ <a href="https://github.com/Simatwa/smartbetsAPI"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GPL-v3&label=License"/></a> <a href="https://pypi.org/project/smartbetsAPI"><img alt="PyPi" src="https://img.shields.io/pypi/v/smartbetsAPI?color=green"/></a> <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a> <a href="#"><img alt="Accuracy" src="https://img.shields.io/static/v1?logo=accuracy&label=Accuracy&message=55%&color=yellow"/></a> <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a> <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=100%&color=yellowgreen"/></a>  <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>  <a href="https://pepy.tech/project/smartbetsapi"><img src="https://static.pepy.tech/personalized-badge/smartbetsapi?period=total&units=international_system&left_color=grey&left_text=Downloads" alt="Downloads"></a></p><br>
 
  
 
  > "Punter's choice"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.6 Summary: Simple
+Metadata-Version: 2.1 Name: smartbetsAPI Version: 1.2.7 Summary: Simple
 football prediction API Home-page: https://github.com/Simatwa/smartbetsAPI
 Author: Smartwa Caleb Author-email: smartwacaleb@gmail.com Maintainer: Smartwa
 Caleb Maintainer-email: smartwacaleb@gmail.com License: GPL-3.0 Project-URL:
 Bug Report, https://github.com/Simatwa/smartbetsAPI/issues/new Project-URL:
 Homepage, https://github.com/Simatwa/smartbetsAPI Project-URL: Source Code,
 https://github.com/Simatwa/smartbetsAPI Project-URL: Issue Tracker, https://
 github.com/Simatwa/smartbetsAPI/issues Project-URL: Download, https://
```

### Comparing `smartbetsAPI-1.2.6/smartbetsAPI.egg-info/SOURCES.txt` & `smartbetsAPI-1.2.7/smartbetsAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/bet_analyzer.py` & `smartbetsAPI-1.2.7/smartbets_API/bet_analyzer.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/bet_at_rest_api_level.py` & `smartbetsAPI-1.2.7/smartbets_API/bet_at_rest_api_level.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/bet_common.py` & `smartbetsAPI-1.2.7/smartbets_API/bet_common.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/configuration_handler.py` & `smartbetsAPI-1.2.7/smartbets_API/configuration_handler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/figure_harvester.py` & `smartbetsAPI-1.2.7/smartbets_API/figure_harvester.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/googler.py` & `smartbetsAPI-1.2.7/smartbets_API/googler.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/html_fetcher.py` & `smartbetsAPI-1.2.7/smartbets_API/html_fetcher.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/interface.py` & `smartbetsAPI-1.2.7/smartbets_API/interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,18 +85,15 @@
         "name": "GNUv3",
         "url": "https://github.com/Simatwa/smartbetsAPI/blob/main/LICENSE?raw=true",
     },
     contact={
         "name": "Smartwa",
         "url": "https://github.com/Simatwa",
         "email": "simatwacaleb@proton.me",
-    },
-    docs_url="/v1/docs",
-    redoc_url="/v1/redoc",
-    # openapi_prefix="/v1",
+    }
 )
 
 v1_router = APIRouter(prefix="/v1", tags=["v1"])
 
 v1_auth_scheme = OAuth2PasswordBearer(
     tokenUrl="/v1/token", description="Token set at server launch."
 )
@@ -109,14 +106,25 @@
     - `net` : Use latest data from internet
     """
 
     home: str
     away: str
     net: bool = False
 
+    model_config = {
+        "json_schema_extra": {
+            "examples": [
+                {
+                    "home": "Arsenal",
+                    "away": "Manchester United",
+                    "net": False
+                }
+            ]
+        }
+    }
 
 class Prediction(BaseModel):
     """Match prediction
     - `g` :	Goal-average of the two teams
     - `gg` : Probability of both teams to score
     - `ov15` : Probability of having more than 2 goals
     - `ov25` : Probability of having more than 3 goals
@@ -131,24 +139,48 @@
     ov15: float
     ov25: float
     ov35: float
     choice: float
     result: str
     pick: str
 
+    model_config = {
+        "json_schema_extra": {
+            "examples": [
+                {
+                    "g": 10,
+                    "gg": 70,
+                    "ov15": 75,
+                    "ov25": 40,
+                    "ov35": 25,
+                    "choice": 55.56,
+                    "result": "1",
+                    "pick": "ov15"
+                }
+            ]
+        }
+    }
 
 class ServerStatus(BaseModel):
     """Checks server's running status
     - `is_alive` : Is server running?
     - `as_at` : Datetime when status was generated.
     """
 
     is_alive: bool = True
     as_at: datetime = datetime.utcnow()
 
+class TokenAuth(BaseModel):
+    """
+    - `access_token` : Token value.
+    - `token_type` : bearer
+    """
+    access_token:str
+    token_type:str
+
 
 def verify_token(token: Annotated[str, Depends(v1_auth_scheme)]):
     """Ensures token passed match the one set"""
     if token and token == args.token:
         return token
     else:
         raise HTTPException(
@@ -167,21 +199,19 @@
 @app.get("/status")
 def server_status() -> ServerStatus:
     """Check server running status"""
     return ServerStatus(as_at=datetime.utcnow())
 
 
 @v1_router.post("/token")
-def fetch_token(form_data: Annotated[OAuth2PasswordRequestForm, Depends()]):
-    """Fetch api token"""
+def fetch_token(form_data: Annotated[OAuth2PasswordRequestForm, Depends()]) -> TokenAuth:
+    """Fetch api token
+    """
     if form_data.username == args.username and form_data.password == args.token:
-        return {
-            "access_token": args.token,
-            "token_type": "bearer",
-        }
+        return TokenAuth(**{"access_token": args.token,"token_type": "bearer",})
     else:
         raise HTTPException(
             status_code=status.HTTP_401_UNAUTHORIZED,
             detail="Invalid username or password",
         )
```

### Comparing `smartbetsAPI-1.2.6/smartbets_API/predictor.py` & `smartbetsAPI-1.2.7/smartbets_API/predictor.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/proxyh.py` & `smartbetsAPI-1.2.7/smartbets_API/proxyh.py`

 * *Files identical despite different names*

### Comparing `smartbetsAPI-1.2.6/smartbets_API/tertiary_bet.py` & `smartbetsAPI-1.2.7/smartbets_API/tertiary_bet.py`

 * *Files identical despite different names*

