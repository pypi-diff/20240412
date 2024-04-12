# Comparing `tmp/pkscreener-0.44.20240410.253.tar.gz` & `tmp/pkscreener-0.44.20240412.254.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240410.253.tar", last modified: Wed Apr 10 22:22:30 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240412.254.tar", last modified: Fri Apr 12 00:44:40 2024, max compression
```

## Comparing `pkscreener-0.44.20240410.253.tar` & `pkscreener-0.44.20240412.254.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:22:30.038564 pkscreener-0.44.20240410.253/
--rw-rw-rw-   0        0        0     1086 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-04-10 22:22:30.038564 pkscreener-0.44.20240410.253/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 22:22:30.022962 pkscreener-0.44.20240410.253/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:22:30.038564 pkscreener-0.44.20240410.253/pkscreener/classes/
--rw-rw-rw-   0        0        0    10156 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    17333 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1536 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    24554 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9291 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2571 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    27488 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    10999 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    15888 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    17381 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8037 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    16886 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    48885 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   108935 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    44525 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4908 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    77641 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3681 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-04-10 22:22:19.000000 pkscreener-0.44.20240410.253/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     4935 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   110075 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/globals.py
--rw-rw-rw-   0        0        0      565 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    47815 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    16959 2024-04-10 22:18:29.000000 pkscreener-0.44.20240410.253/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:22:30.038564 pkscreener-0.44.20240410.253/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1250 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-04-10 22:22:29.000000 pkscreener-0.44.20240410.253/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-10 22:22:30.038564 pkscreener-0.44.20240410.253/setup.cfg
--rw-rw-rw-   0        0        0     4715 2024-04-10 22:18:30.000000 pkscreener-0.44.20240410.253/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/
+-rw-rw-rw-   0        0        0     1086 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.964645 pkscreener-0.44.20240412.254/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/pkscreener/classes/
+-rw-rw-rw-   0        0        0    10156 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    17333 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1536 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    24554 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9291 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2571 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    27550 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    10999 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    17214 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    17381 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8037 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    16886 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    48885 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   108935 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    44525 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4908 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    77670 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3681 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-04-12 00:44:31.000000 pkscreener-0.44.20240412.254/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     4935 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   111068 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      565 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    47815 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    18397 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:44:40.964645 pkscreener-0.44.20240412.254/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1250 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-04-12 00:44:40.000000 pkscreener-0.44.20240412.254/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-12 00:44:40.980271 pkscreener-0.44.20240412.254/setup.cfg
+-rw-rw-rw-   0        0        0     4715 2024-04-12 00:41:27.000000 pkscreener-0.44.20240412.254/setup.py
```

### Comparing `pkscreener-0.44.20240410.253/LICENSE` & `pkscreener-0.44.20240412.254/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/LICENSE-Others` & `pkscreener-0.44.20240412.254/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/PKG-INFO` & `pkscreener-0.44.20240412.254/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240410.253
+Version: 0.44.20240412.254
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240410.253.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.254.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240410.253/README.md` & `pkscreener-0.44.20240412.254/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/__init__.py` & `pkscreener-0.44.20240412.254/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/MenuOptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,18 +264,20 @@
 # This Class manages application menus
 class menus:
     
     @staticmethod
     def allMenus(topLevel="X",index=12):
         menuOptions = [topLevel]
         indexOptions =[index]
-        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,23,24,25]
-        scanSubOptions = {6:[1,2,3,4,5,6,{7:[1,2]}], 
-                          7:[1,2,{3:[1,2]},4,5,{6:[1,2,3]},7],
-                         21:[3,5,6,7,8,9]}
+        scanOptions = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,23,24,25]
+        scanSubOptions = {
+                            6:[1,2,3,4,5,6,{7:[1,2]},8,9],
+                            7:[1,2,{3:[1,2]},4,5,{6:[1,3]},7],
+                            # 21:[3,5,6,7,8,9]
+                         }
         runOptions = []
         for menuOption in menuOptions:
             for indexOption in indexOptions:
                 for scanOption in scanOptions:
                     if scanOption in scanSubOptions.keys():
                         for scanSubOption in scanSubOptions[scanOption]:
                             if isinstance(scanSubOption, dict):
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     SOFTWARE.
 
 """
 import copy
 import datetime
 import sys
 import os
+import numpy as np
 import pandas as pd
 import pkscreener.classes.Utility as Utility
 from pkscreener.classes.ConfigManager import parser, tools
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes import Archiver
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.PKPickler import PKPicklerDB
@@ -68,24 +69,30 @@
     allDailyCandles = None
     def getStockDataForSimulation():
         int_exists, int_cache_file = PKMarketOpenCloseAnalyser.ensureIntradayStockDataExists()
         daily_exists, daily_cache_file = PKMarketOpenCloseAnalyser.ensureDailyStockDataExists()
         updatedCandleData = PKMarketOpenCloseAnalyser.updatedCandleData
         allDailyCandles = PKMarketOpenCloseAnalyser.allDailyCandles
         if  (int_exists and daily_exists) and (updatedCandleData is None or allDailyCandles is None):
-            latestDailyCandle,allDailyCandles = PKMarketOpenCloseAnalyser.getLatestDailyCandleData(daily_cache_file)
+            allDailyCandles = PKMarketOpenCloseAnalyser.getLatestDailyCandleData(daily_cache_file)
             morningIntradayCandle = PKMarketOpenCloseAnalyser.getIntradayCandleFromMorning(int_cache_file)
-            updatedCandleData = PKMarketOpenCloseAnalyser.combineDailyStockDataWithMorningSimulation(latestDailyCandle,allDailyCandles,morningIntradayCandle)
-            Utility.tools.saveStockData(updatedCandleData,PKMarketOpenCloseAnalyser.configManager,0,False,False)
+            updatedCandleData = PKMarketOpenCloseAnalyser.combineDailyStockDataWithMorningSimulation(allDailyCandles,morningIntradayCandle)
+            # PKMarketOpenCloseAnalyser.updatedCandleData = updatedCandleData
+            # PKMarketOpenCloseAnalyser.allDailyCandles = allDailyCandles
+            Utility.tools.saveStockData(updatedCandleData,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
         return updatedCandleData, allDailyCandles
 
     def runOpenCloseAnalysis(updatedCandleData,allDailyCandles,screen_df,save_df,runOptionName=None):
         # stockListFromMorningTrade,morningIntraday_df = PKMarketOpenCloseAnalyser.simulateMorningTrade(updatedCandleData)
         # latest_daily_df = PKMarketOpenCloseAnalyser.runScanForStocksFromMorningTrade(stockListFromMorningTrade,allDailyCandles)
-        PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, allDailyCandles,runOptionName=runOptionName)
+        try:
+            PKMarketOpenCloseAnalyser.diffMorningCandleDataWithLatestDailyCandleData(screen_df,save_df, allDailyCandles,runOptionName=runOptionName)
+        except:
+            pass
+        Utility.tools.saveStockData(allDailyCandles,PKMarketOpenCloseAnalyser.configManager,1,False,False, True)
 
     def ensureIntradayStockDataExists():
         # Ensure that the intraday_stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
         if not exists:
             savedPeriod = PKMarketOpenCloseAnalyser.configManager.period
             savedDuration = PKMarketOpenCloseAnalyser.configManager.duration
@@ -105,22 +112,22 @@
 
     def ensureDailyStockDataExists():
         # Ensure that the stock_data_<date>.pkl file exists
         exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
         if not exists:
             print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
         # We should download a fresh copy anyways because we may have altered the existing copy in
-        # the previous run.
-        print(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
-        Utility.tools.loadStockData({},PKMarketOpenCloseAnalyser.configManager,False,'Y',False,False,None,isIntraday=False,forceRedownload=True)
-        exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=True)
-        if not exists:
-            print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
-            print(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d{colorText.END} and then run this menu option again.")
-            input("Press any key to continue...")
+        # the previous run. -- !!!! Not required if we saved at the end of last operation !!!!
+            print(f"[+] {colorText.GREEN}Trying to download {cache_file}{colorText.END}. Please wait ...")
+            Utility.tools.loadStockData({},PKMarketOpenCloseAnalyser.configManager,False,'Y',False,False,None,isIntraday=False,forceRedownload=True)
+            exists, cache_file = Utility.tools.afterMarketStockDataExists(intraday=False)
+            if not exists:
+                print(f"[+] {colorText.FAIL}{cache_file}{colorText.END} not found under {Archiver.get_user_outputs_dir()} !")
+                print(f"[+] Please run {colorText.FAIL}pkscreener{colorText.END}{colorText.GREEN} -a Y -e -d{colorText.END} and then run this menu option again.")
+                input("Press any key to continue...")
         return exists, cache_file
     
     def simulateMorningTrade(updatedCandleData):
         # 1. For each stock, remove the latest daily data for today from stock_data_<date>.pkl
         # 2. For each stock, only take the configManager.morninganalysiscandlenumber data rows
         #    and combine them as one candle - open for the earliest candle and close for the last candle,
         #    low and high will be the lowest and highest for in-between candles. Volume should be combined
@@ -130,28 +137,28 @@
         #    running in the morning. 
         # 5. Compare the stock prices from #4 with the removed row from #1 and show the diff.
         stockListFromMorningTrade = []
         morningIntraday_df = None
         return stockListFromMorningTrade, morningIntraday_df
     
     def getLatestDailyCandleData(daily_cache_file):
-        latestDailyCandle,allDailyCandles = None, None
+        allDailyCandles = None
         dailyDB = PKDailyStockDataDB(fileName=daily_cache_file)
         allDailyCandles = dailyDB.pickler.pickler.unpickle(fileName=dailyDB.pickler.fileName)
-        latestDailyCandle = {}
+        # latestDailyCandle = {}
         # stocks = list(allDailyCandles.keys())
         # for stock in stocks:
         #     try:
         #         df = pd.DataFrame(data=[allDailyCandles[stock]["data"][-1]],
         #                       columns=allDailyCandles[stock]["columns"],
         #                       index=[allDailyCandles[stock]["index"][-1]])
         #         latestDailyCandle[stock] = df.to_dict("split")
         #     except:
         #         continue
-        return latestDailyCandle,allDailyCandles
+        return allDailyCandles
     
     def getIntradayCandleFromMorning(int_cache_file):
         morningIntradayCandle = None
         intradayDB = PKIntradayStockDataDB(fileName=int_cache_file)
         allDailyIntradayCandles = intradayDB.pickler.pickler.unpickle(fileName=intradayDB.pickler.fileName)
         morningIntradayCandle = {}
         stocks = list(allDailyIntradayCandles.keys())
@@ -166,29 +173,45 @@
                 # We'd then combine the data from 9:15 to 9:57 as a single candle of 
                 # OHLCV and replace the last daily candle with this one candle to
                 # simulate the scan outcome from morning.
                 df = pd.DataFrame(data=allDailyIntradayCandles[stock]["data"],
                                 columns=allDailyIntradayCandles[stock]["columns"],
                                 index=allDailyIntradayCandles[stock]["index"])
                 df = df.head(numOfCandles)
-                df = df[df.index <=  f'{PKDateUtilities.tradingDate().strftime("%Y-%m-%d")} 09:57:00+05:30']
+                df = df[df.index <=  f'{PKDateUtilities.tradingDate().strftime(f"%Y-%m-%d")} 09:{15+PKMarketOpenCloseAnalyser.configManager.morninganalysiscandlenumber}:00+05:30']
                 if df is not None and len(df) > 0:
-                    combinedCandle = {"Open":df["Open"][0], "High":max(df["High"]), 
-                                    "Low":min(df["Low"]),"Close":df["Close"][-1],
+                    combinedCandle = {"Open":PKMarketOpenCloseAnalyser.getMorningOpen(df), "High":max(df["High"]), 
+                                    "Low":min(df["Low"]),"Close":PKMarketOpenCloseAnalyser.getMorningClose(df),
                                     "Adj Close":df["Adj Close"][-1],"Volume":sum(df["Volume"])}
                     tradingDate = PKDateUtilities.tradingDate()
                     timestamp = datetime.datetime.strptime(tradingDate.strftime("%Y-%m-%d hh:mm:ss"),"%Y-%m-%d hh:mm:ss")
                     df = pd.DataFrame([combinedCandle], columns=df.columns, index=[timestamp])
                     morningIntradayCandle[stock] = df.to_dict("split")
             except Exception as e:
                 print(f"{stock}:    {e}")
                 continue
         return morningIntradayCandle
 
-    def combineDailyStockDataWithMorningSimulation(latestDailyCandle,allDailyCandles,morningIntradayCandle):
+    def getMorningOpen(df):
+        open = df["Open"][0]
+        index = 0
+        while open is np.nan and index < len(df):
+            open = df["Open"][index + 1]
+            index += 1
+        return open
+    
+    def getMorningClose(df):
+        close = df["Close"][-1]
+        index = len(df)
+        while close is np.nan and index >= 0:
+            close = df["Close"][index - 1]
+            index -= 1
+        return close
+    
+    def combineDailyStockDataWithMorningSimulation(allDailyCandles,morningIntradayCandle):
         mutableAllDailyCandles = copy.deepcopy(allDailyCandles)
         stocks = list(mutableAllDailyCandles.keys())
         intradayStocks = list(morningIntradayCandle.keys())
         priceDict = {}
         listPriceDict = []
         for stock in stocks:
             try:
@@ -196,14 +219,17 @@
                 if stock in intradayStocks:
                     morningPrice = round(morningIntradayCandle[stock]["data"][0][3],2)
                     closePrice = round(mutableAllDailyCandles[stock]["data"][-1][3],2)
                     priceDict["Stock"] = stock
                     priceDict["Morning"] = morningPrice
                     priceDict["EoD"] = closePrice
                     listPriceDict.append(priceDict)
+                    # We basically need to replace today's candle with a single candle that has data from market open to the time
+                    # when we are taking as reference point in the morning. This is how it would have looked when running the scan 
+                    # in the morning hours.
                     mutableAllDailyCandles[stock]["data"] = mutableAllDailyCandles[stock]["data"][:-1] + [morningIntradayCandle[stock]["data"][0]]
                     mutableAllDailyCandles[stock]["index"] = mutableAllDailyCandles[stock]["index"][:-1] + morningIntradayCandle[stock]["index"]
                 else:
                     # We should ideally have all stocks from intraday and eod matching,
                     # but for whatever reason, if we don't have the stock, we should skip those
                     # stocks from analysis
                     del mutableAllDailyCandles[stock]
@@ -246,27 +272,26 @@
         save_df["EoDLTP"] = eodLTPs
         screen_df["EoDLTP"] = eodLTPs
         save_df["Diff"] = diff
         screen_df["Diff"] = diff
         columns = save_df.columns
         lastIndex = len(save_df)
         for col in columns:
-            if col in ["Stock", "LTP", "%Chng", "EoDLTP", "Diff","Pattern"]:
+            if col in ["Stock", "Pattern", "LTP", "EoDLTP", "Diff", "%Chng"]:
                 if col == "Stock":
                     save_df.loc[lastIndex,col] = "PORTFOLIO"
                 elif col == "Pattern":
                     save_df.loc[lastIndex,col] = runOptionName if runOptionName is not None else ""
                 elif col in ["LTP","EoDLTP", "Diff"]:
                     save_df.loc[lastIndex,col] = round(sum(save_df[col].dropna(inplace=False).astype(float)),2)
                 elif col == "%Chng":
                     change_pct = sum(save_df["Diff"].dropna(inplace=False).astype(float))*100/sum(save_df["LTP"].dropna(inplace=False).astype(float))
-                    save_df.loc[lastIndex,col] = round(change_pct,2)
+                    save_df.loc[lastIndex,col] = round(2*change_pct,2) # when summing above for LTP, the total of LTP gets summed up too. Hence *2 here.
             else:
                 save_df.loc[lastIndex,col] = ""
             screen_df.loc[lastIndex,col] = save_df.loc[lastIndex,col]
         save_df.set_index("Stock", inplace=True)
         screen_df.set_index("Stock", inplace=True)
         if 'index' in save_df.columns:
             save_df.drop('index', axis=1, inplace=True, errors="ignore")
         if 'index' in screen_df.columns:
             screen_df.drop('index', axis=1, inplace=True, errors="ignore")
-
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
         outputFolder = Archiver.get_user_outputs_dir()
         if downloadOnly:
             outputFolder = outputFolder.replace("results","actions-data-download")
             if not os.path.isdir(outputFolder):
                 os.makedirs(os.path.dirname(f"{outputFolder}{os.sep}"), exist_ok=True)
             configManager.deleteFileWithPattern(rootDir=outputFolder)
         cache_file = os.path.join(outputFolder, fileName)
-        if not os.path.exists(cache_file) or forceSave or (loadCount > 0 and len(stockDict) > (loadCount + 1)):
+        if not os.path.exists(cache_file) or forceSave or (loadCount >= 0 and len(stockDict) > (loadCount + 1)):
             try:
                 with open(cache_file, "wb") as f:
                     pickle.dump(stockDict.copy(), f, protocol=pickle.HIGHEST_PROTOCOL)
                     print(colorText.BOLD + colorText.GREEN + "=> Done." + colorText.END)
                 if downloadOnly:
                     Committer.execOSCommand(f"git add {cache_file} -f >/dev/null 2>&1")
             except pickle.PicklingError as e:  # pragma: no cover
@@ -893,15 +893,15 @@
             == configManager.period
             and ("1m" if isIntraday else ConfigManager.default_duration)
             == configManager.duration
         ) or forceRedownload:
             print(
                     colorText.BOLD
                     + colorText.FAIL
-                    + "[+] Market Stock Data is not cached.."
+                    + "[+] Market Stock Data is not cached, or forced to redownload .."
                     + colorText.END
                 )
             print(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] Downloading cache from server for faster processing, Please Wait.."
                 + colorText.END
@@ -1184,15 +1184,15 @@
             return (-100, 100)
 
     # Prompt for asking Volume ratio
     def promptVolumeMultiplier(volumeRatio=None):
         if volumeRatio is not None:
             return volumeRatio
         try:
-            volumeRatio = int(
+            volumeRatio = float(
                 input(
                     colorText.BOLD
                     + colorText.WARN
                     + "\n[+] Enter Min Volume ratio value (Default = 2.5): "
                     + colorText.END
                 )
             )
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/classes/keys.py` & `pkscreener-0.44.20240412.254/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/courbd.ttf` & `pkscreener-0.44.20240412.254/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/globals.py` & `pkscreener-0.44.20240412.254/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,29 +544,34 @@
             if reversalOption in [3]:
                 sortKey = ["Volume","MA-Signal"]
                 ascending = [False, False]
         elif executeOption == 23:
             sortKey = ["bbands_ulr_ratio_max5"]
             ascending = [False]
         try:
+            screenResults[sortKey] = screenResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+            saveResults[sortKey] = saveResults[sortKey].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
             screenResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
             saveResults.sort_values(by=sortKey, ascending=ascending, inplace=True)
-        except:
+        except Exception as e:
+            default_logger().debug(e, exc_info=True)
             pass
         columnsToBeDeleted = ["MFI","FVDiff","ConfDMADifference","bbands_ulr_ratio_max5"]
         for column in columnsToBeDeleted:
             if column in saveResults.columns:
                 saveResults.drop(column, axis=1, inplace=True, errors="ignore")
                 screenResults.drop(column, axis=1, inplace=True, errors="ignore")
-        screenResults.set_index("Stock", inplace=True)
-        saveResults.set_index("Stock", inplace=True)
+        if "Stock" in screenResults.columns:
+            screenResults.set_index("Stock", inplace=True)
+        if "Stock" in saveResults.columns:
+            saveResults.set_index("Stock", inplace=True)
         screenResults['Volume'] = screenResults['Volume'].astype(str)
         saveResults['Volume'] = saveResults['Volume'].astype(str)
         screenResults.loc[:, "Volume"] = screenResults.loc[:, "Volume"].apply(
-            lambda x: Utility.tools.formatRatio(float(x), volumeRatio)
+            lambda x: Utility.tools.formatRatio(float(x), volumeRatio) if len(str(x).strip()) > 0 else ''
         )
         saveResults.loc[:, "Volume"] = saveResults.loc[:, "Volume"].apply(
             lambda x: str(x) + "x"
         )
         screenResults.rename(
             columns={
                 "Trend": f"Trend({configManager.daysToLookback}Prds)",
@@ -1802,21 +1807,26 @@
 def removedUnusedColumns(screenResults, saveResults, dropAdditionalColumns=[], userArgs=None):
     periods = configManager.periodsRange
     if userArgs is not None and userArgs.backtestdaysago is not None and int(userArgs.backtestdaysago) < 22:
         dropAdditionalColumns.append("22-Pd %")
     summaryReturns = ("w.r.t. " + saveResults["Date"].iloc[0]) if "Date" in saveResults.columns else ""
     for period in periods:
         if saveResults is not None:
-            if f"LTP{period}" in saveResults.columns:
-                pdReturn = round(100*(sum(saveResults[f"LTP{period}"] * saveResults["MCapWt%"])-sum(saveResults["LTP"] * saveResults["MCapWt%"]))/sum(saveResults["LTP"] * saveResults["MCapWt%"]),1)
+            if f"LTP{period}" in saveResults.columns and "MCapWt%" in saveResults.columns:
+                pdLTP = saveResults[f"LTP{period}"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+                mktWeight = saveResults["MCapWt%"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+                ltp = saveResults[f"LTP"].replace("", np.nan).replace(np.inf, np.nan).replace(-np.inf, np.nan).astype(float)
+                pdReturn = round(100*(sum(pdLTP * mktWeight)-sum(ltp * mktWeight))/sum(ltp * mktWeight),1)
                           #round((sum(saveResults[f"LTP{period}"]) - sum(saveResults['LTP']))*100/sum(saveResults['LTP']),1)
                 if pdReturn > -500:
                     summaryReturns = f"{period}-Pd({pdReturn} %), {summaryReturns}"
             saveResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             saveResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
+            saveResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
+            screenResults.drop(f"MCapWt%", axis=1, inplace=True, errors="ignore")
             if len(dropAdditionalColumns) > 0:
                 for col in dropAdditionalColumns:
                     if col in saveResults.columns:
                         saveResults.drop(col, axis=1, inplace=True, errors="ignore")
         if screenResults is not None:
             screenResults.drop(f"LTP{period}", axis=1, inplace=True, errors="ignore")
             screenResults.drop(f"Growth{period}", axis=1, inplace=True, errors="ignore")
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240412.254/pkscreener/pkscreener.ini`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,9 @@
 backtestperiod = 120
 minimumvolume = 10000
 showunknowntrends = y
 backtestPeriodFactor = 1
 enablePortfolioCalculations = n
 showPastStrategyData = n
 maxbacktestwindow = 30
-morninganalysiscandlenumber=43
+morninganalysiscandlenumber=25
 morninganalysiscandleduration=1m
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240412.254/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240412.254/pkscreener/pkscreenercli.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,37 +271,60 @@
                 + colorText.FAIL
                 + "[+] Neither ta-lib nor pandas_ta was located. You need at least one of them to continue! \n[+] Please follow instructions from README file under PKScreener repo: https://github.com/pkjmesra/PKScreener"
                 + colorText.END
             )
             input("Press any key to try anyway...")
 
 def runApplication():
-    from pkscreener.globals import main
+    from pkscreener.globals import main, sendQuickScanResult
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
         optionalFinalOutcome_df = None
+        import pkscreener.classes.Utility as Utility
+        import pandas as pd
+        # Delete any existing data from the previous run.
+        configManager.deleteFileWithPattern(pattern="stock_data_*.pkl")
         for runOption in runOptions:
             args.options = runOption
             try:
                 optionalFinalOutcome_df = main(userArgs=args,optionalFinalOutcome_df=optionalFinalOutcome_df)
             except Exception as e:
                 print(e)
                 if args.log:
                     import traceback
                     traceback.print_exc()
         if optionalFinalOutcome_df is not None:
+            final_df = None
             df_grouped = optionalFinalOutcome_df.groupby("Stock")
             for stock, df_group in df_grouped:
                 if stock == "PORTFOLIO":
-                    print(df_group)
+                    if final_df is None:
+                        final_df = df_group[["Pattern","LTP","EoDLTP","Diff","%Chng"]]
+                    else:
+                        final_df = pd.concat([final_df, df_group[["Pattern","LTP","EoDLTP","Diff","%Chng"]]], axis=0)
+            mark_down = colorText.miniTabulator().tabulate(
+                                final_df,
+                                headers="keys",
+                                tablefmt=colorText.No_Pad_GridFormat,
+                                showindex = False
+                            ).encode("utf-8").decode(Utility.STD_ENCODING)
+            print(mark_down)
+            sendQuickScanResult(menuChoiceHierarchy="IntradayAnalysis",
+                                user="-1001785195297",
+                                tabulated_results=mark_down,
+                                markdown_results=mark_down,
+                                caption="IntradayAnalysis - Morning alert vs Market Close",
+                                pngName= f"PKS_IA_{PKDateUtilities.currentDateTime().strftime('%Y-%m-%d_%H:%M:%S')}",
+                                pngExtension= ".png"
+                                )
     else:
         main(userArgs=args)
 
 
 def pkscreenercli():
     global originalStdOut
     if sys.platform.startswith("darwin"):
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240412.254/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240410.253
+Version: 0.44.20240412.254
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240410.253.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240412.254.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.252/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240410.253/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240410.253/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240412.254/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240410.253/setup.py` & `pkscreener-0.44.20240412.254/setup.py`

 * *Files identical despite different names*

