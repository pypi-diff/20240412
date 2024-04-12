# Comparing `tmp/fnschool-20240412.1950.33.tar.gz` & `tmp/fnschool-20240412.2017.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240412.1950.33.tar", last modified: Fri Apr 12 11:50:37 2024, max compression
+gzip compressed data, was "fnschool-20240412.2017.13.tar", last modified: Fri Apr 12 12:17:17 2024, max compression
```

## Comparing `fnschool-20240412.1950.33.tar` & `fnschool-20240412.2017.13.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.601297 fnschool-20240412.1950.33/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.1950.33/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-12 11:50:37.601297 fnschool-20240412.1950.33/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240412.1950.33/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.1950.33/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 11:50:37.601297 fnschool-20240412.1950.33/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.584298 fnschool-20240412.1950.33/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.590298 fnschool-20240412.1950.33/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 11:50:33.000000 fnschool-20240412.1950.33/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.595298 fnschool-20240412.1950.33/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.1950.33/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.598297 fnschool-20240412.1950.33/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.1950.33/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.1950.33/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14625 2024-04-12 06:11:32.000000 fnschool-20240412.1950.33/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.1950.33/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    99112 2024-04-12 11:50:07.000000 fnschool-20240412.1950.33/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.598297 fnschool-20240412.1950.33/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.1950.33/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.1950.33/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.587298 fnschool-20240412.1950.33/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.586298 fnschool-20240412.1950.33/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.598297 fnschool-20240412.1950.33/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 11:50:32.000000 fnschool-20240412.1950.33/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.586298 fnschool-20240412.1950.33/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.599298 fnschool-20240412.1950.33/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    12193 2024-04-12 11:50:32.000000 fnschool-20240412.1950.33/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.586298 fnschool-20240412.1950.33/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.599298 fnschool-20240412.1950.33/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:50:32.000000 fnschool-20240412.1950.33/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.587298 fnschool-20240412.1950.33/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.599298 fnschool-20240412.1950.33/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:50:32.000000 fnschool-20240412.1950.33/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.587298 fnschool-20240412.1950.33/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.600298 fnschool-20240412.1950.33/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:50:32.000000 fnschool-20240412.1950.33/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.1950.33/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:50:37.600298 fnschool-20240412.1950.33/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 11:50:37.000000 fnschool-20240412.1950.33/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.590344 fnschool-20240412.2017.13/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.2017.13/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-12 12:17:17.589343 fnschool-20240412.2017.13/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240412.2017.13/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.2017.13/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 12:17:17.590344 fnschool-20240412.2017.13/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.573344 fnschool-20240412.2017.13/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.579344 fnschool-20240412.2017.13/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.584344 fnschool-20240412.2017.13/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.2017.13/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.586344 fnschool-20240412.2017.13/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.2017.13/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.2017.13/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14625 2024-04-12 06:11:32.000000 fnschool-20240412.2017.13/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/canteen/profile.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.2017.13/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    99108 2024-04-12 12:10:03.000000 fnschool-20240412.2017.13/src/fnschool/canteen/workbook.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.586344 fnschool-20240412.2017.13/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.2017.13/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.2017.13/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.576344 fnschool-20240412.2017.13/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.574344 fnschool-20240412.2017.13/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.587344 fnschool-20240412.2017.13/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.575344 fnschool-20240412.2017.13/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.587344 fnschool-20240412.2017.13/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    12193 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.575344 fnschool-20240412.2017.13/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.587344 fnschool-20240412.2017.13/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.576344 fnschool-20240412.2017.13/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.588343 fnschool-20240412.2017.13/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.576344 fnschool-20240412.2017.13/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.588343 fnschool-20240412.2017.13/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 12:17:13.000000 fnschool-20240412.2017.13/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.2017.13/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 12:17:17.589343 fnschool-20240412.2017.13/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)     9964 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 12:17:17.000000 fnschool-20240412.2017.13/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240412.1950.33/LICENSE` & `fnschool-20240412.2017.13/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/PKG-INFO` & `fnschool-20240412.2017.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.1950.33
+Version: 20240412.2017.13
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240412.1950.33/pyproject.toml` & `fnschool-20240412.2017.13/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/bill.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/canteen.toml` & `fnschool-20240412.2017.13/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/config.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240412.2017.13/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240412.2017.13/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/food.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/path.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/profile.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/test.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/canteen/workbook.py` & `fnschool-20240412.2017.13/src/fnschool/canteen/workbook.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,23 +719,23 @@
                         _row_index,
                         3,
                         ("上年结转" if t1.month == 1 else "上月结转"),
                     )
                     sheet.cell(row_index, 10, food.count)
                     sheet.cell(row_index, 11, food.unit_price)
                     sheet.cell(row_index, 12, food.count * food.unit_price)
-                    row_index = _row_index
+                    row_index += 1
             else:
                 sheet.cell(
                     row_index,
                     3,
                     ("上年结转" if t1.month == 1 else "上月结转"),
                 )
 
-            row_index += 1
+                row_index += 1
 
             _cdates = []
             for food in _cfoods:
                 if len(food.consuming_list) > 0:
                     _cdates += [d for d, c in food.consuming_list]
                 _cdates.append(food.check_date)
             _cdates = [d for d in _cdates if d.month == self.bill.month]
```

### Comparing `fnschool-20240412.1950.33/src/fnschool/entry.py` & `fnschool-20240412.2017.13/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/external.py` & `fnschool-20240412.2017.13/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/language.py` & `fnschool-20240412.2017.13/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240412.2017.13/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/path.py` & `fnschool-20240412.2017.13/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool/test.py` & `fnschool-20240412.2017.13/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1950.33/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240412.2017.13/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.1950.33
+Version: 20240412.2017.13
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240412.1950.33/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240412.2017.13/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

