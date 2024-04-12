# Comparing `tmp/fnschool-20240412.2240.38.tar.gz` & `tmp/fnschool-20240412.2250.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240412.2240.38.tar", last modified: Fri Apr 12 14:40:42 2024, max compression
+gzip compressed data, was "fnschool-20240412.2250.49.tar", last modified: Fri Apr 12 14:50:54 2024, max compression
```

## Comparing `fnschool-20240412.2240.38.tar` & `fnschool-20240412.2250.49.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.660664 fnschool-20240412.2240.38/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.2240.38/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12299 2024-04-12 14:40:42.660664 fnschool-20240412.2240.38/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2334 2024-04-12 14:33:08.000000 fnschool-20240412.2240.38/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.2240.38/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 14:40:42.661664 fnschool-20240412.2240.38/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.643664 fnschool-20240412.2240.38/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.650664 fnschool-20240412.2240.38/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 14:40:38.000000 fnschool-20240412.2240.38/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.654664 fnschool-20240412.2240.38/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.2240.38/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.657664 fnschool-20240412.2240.38/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.2240.38/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.2240.38/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14985 2024-04-12 14:37:20.000000 fnschool-20240412.2240.38/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.2240.38/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    99108 2024-04-12 12:10:03.000000 fnschool-20240412.2240.38/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.657664 fnschool-20240412.2240.38/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.2240.38/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.2240.38/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.646664 fnschool-20240412.2240.38/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.644664 fnschool-20240412.2240.38/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.658664 fnschool-20240412.2240.38/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 14:40:37.000000 fnschool-20240412.2240.38/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.644664 fnschool-20240412.2240.38/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.658664 fnschool-20240412.2240.38/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    12605 2024-04-12 14:40:37.000000 fnschool-20240412.2240.38/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.645664 fnschool-20240412.2240.38/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.658664 fnschool-20240412.2240.38/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:40:37.000000 fnschool-20240412.2240.38/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.645664 fnschool-20240412.2240.38/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.659664 fnschool-20240412.2240.38/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:40:37.000000 fnschool-20240412.2240.38/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.646664 fnschool-20240412.2240.38/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.659664 fnschool-20240412.2240.38/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:40:37.000000 fnschool-20240412.2240.38/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.2240.38/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:40:42.659664 fnschool-20240412.2240.38/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12299 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 14:40:42.000000 fnschool-20240412.2240.38/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.033082 fnschool-20240412.2250.49/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.2250.49/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12297 2024-04-12 14:50:54.032082 fnschool-20240412.2250.49/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2332 2024-04-12 14:50:23.000000 fnschool-20240412.2250.49/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.2250.49/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 14:50:54.033082 fnschool-20240412.2250.49/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.015082 fnschool-20240412.2250.49/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.022082 fnschool-20240412.2250.49/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.027082 fnschool-20240412.2250.49/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.2250.49/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.029082 fnschool-20240412.2250.49/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.2250.49/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.2250.49/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14985 2024-04-12 14:37:20.000000 fnschool-20240412.2250.49/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/canteen/profile.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.2250.49/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    99108 2024-04-12 12:10:03.000000 fnschool-20240412.2250.49/src/fnschool/canteen/workbook.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.030082 fnschool-20240412.2250.49/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.2250.49/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.2250.49/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.018082 fnschool-20240412.2250.49/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.016082 fnschool-20240412.2250.49/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.030082 fnschool-20240412.2250.49/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.017082 fnschool-20240412.2250.49/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.030082 fnschool-20240412.2250.49/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    12605 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.017082 fnschool-20240412.2250.49/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.031082 fnschool-20240412.2250.49/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.017082 fnschool-20240412.2250.49/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.031082 fnschool-20240412.2250.49/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.018082 fnschool-20240412.2250.49/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.031082 fnschool-20240412.2250.49/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 14:50:49.000000 fnschool-20240412.2250.49/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.2250.49/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 14:50:54.032082 fnschool-20240412.2250.49/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12297 2024-04-12 14:50:53.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 14:50:54.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 14:50:53.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 14:50:53.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 14:50:53.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 14:50:53.000000 fnschool-20240412.2250.49/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240412.2240.38/LICENSE` & `fnschool-20240412.2250.49/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/PKG-INFO` & `fnschool-20240412.2250.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.2240.38
+Version: 20240412.2250.49
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -233,15 +233,15 @@
 
 ## How To Use
 
 ### Install Python3
 
 Ubuntu: 
 ```bash
-sudo apt-get install -U python3 python3-pip
+sudo apt-get install python3 python3-pip
 ```
 Windows:   
 Install Python3 from [www.python.org/getit](https://www.python.org/getit/).  
 
 ### Install fnschool and run it
 ```bash
 # install
@@ -262,14 +262,15 @@
 - [pandas](https://pandas.pydata.org/)  
 - [numpy](https://numpy.org/)  
 - [openpyxl](https://openpyxl.readthedocs.io/)  
 - [appdirs](http://github.com/ActiveState/appdirs)  
 
 
 ## Support
+
 Buy me a `coffee`:  
 
 ![Buy me a coffee](https://raw.githubusercontent.com/larryw3i/funingschool/master/Documentation/images/9237879a-f8d5-11ee-8411-23057db0a773.jpeg)
 
 ## License
 
 [GNU LESSER GENERAL PUBLIC LICENSE Version 3](https://github.com/larryw3i/funingschool/blob/master/LICENSE)
```

### Comparing `fnschool-20240412.2240.38/README.md` & `fnschool-20240412.2250.49/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 ## How To Use
 
 ### Install Python3
 
 Ubuntu: 
 ```bash
-sudo apt-get install -U python3 python3-pip
+sudo apt-get install python3 python3-pip
 ```
 Windows:   
 Install Python3 from [www.python.org/getit](https://www.python.org/getit/).  
 
 ### Install fnschool and run it
 ```bash
 # install
@@ -72,14 +72,15 @@
 - [pandas](https://pandas.pydata.org/)  
 - [numpy](https://numpy.org/)  
 - [openpyxl](https://openpyxl.readthedocs.io/)  
 - [appdirs](http://github.com/ActiveState/appdirs)  
 
 
 ## Support
+
 Buy me a `coffee`:  
 
 ![Buy me a coffee](https://raw.githubusercontent.com/larryw3i/funingschool/master/Documentation/images/9237879a-f8d5-11ee-8411-23057db0a773.jpeg)
 
 ## License
 
 [GNU LESSER GENERAL PUBLIC LICENSE Version 3](https://github.com/larryw3i/funingschool/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
                            _ç_®__ä_½__ä_¸_­_æ__ â¢ _E_n_g_l_i_s_h
  _K_e_y_ _F_e_a_t_u_r_e_s â¢ _H_o_w_ _T_o_ _U_s_e â¢ _D_o_w_n_l_o_a_d â¢ _C_r_e_d_i_t_s â¢ _R_e_l_a_t_e_d â¢ _L_i_c_e_n_s_e
 ![screenshot](https://raw.githubusercontent.com/larryw3i/funingschool/master/
 Documentation/images/9432e132-f8cd-11ee-8ee6-f37309efa64b.png) ## Key Features
 * Read food spreadsheets automatically. * The simplest and most straightforward
 `consuming sheets`. * Update sheets (warehousing, consuming, summing, etc)
 automatically. * Reduce calculation errors. * Easy to use. ## How To Use ###
-Install Python3 Ubuntu: ```bash sudo apt-get install -U python3 python3-pip ```
+Install Python3 Ubuntu: ```bash sudo apt-get install python3 python3-pip ```
 Windows: Install Python3 from [www.python.org/getit](https://www.python.org/
 getit/). ### Install fnschool and run it ```bash # install pip3 install -
 U fnschool # run fnschool-cli canteen mk_bill ``` > **Note** > Read the
 information it prompts carefully, which is the key to using it well. ## Credits
 This software uses the following open source packages: - [colorama](https://
 github.com/tartley/colorama) - [pandas](https://pandas.pydata.org/) - [numpy]
 (https://numpy.org/) - [openpyxl](https://openpyxl.readthedocs.io/) - [appdirs]
```

### Comparing `fnschool-20240412.2240.38/pyproject.toml` & `fnschool-20240412.2250.49/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/bill.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/canteen.toml` & `fnschool-20240412.2250.49/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/config.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240412.2250.49/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240412.2250.49/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/food.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/path.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/profile.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/test.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/canteen/workbook.py` & `fnschool-20240412.2250.49/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/entry.py` & `fnschool-20240412.2250.49/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/external.py` & `fnschool-20240412.2250.49/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/language.py` & `fnschool-20240412.2250.49/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240412.2250.49/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/path.py` & `fnschool-20240412.2250.49/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool/test.py` & `fnschool-20240412.2250.49/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.2240.38/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240412.2250.49/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.2240.38
+Version: 20240412.2250.49
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -233,15 +233,15 @@
 
 ## How To Use
 
 ### Install Python3
 
 Ubuntu: 
 ```bash
-sudo apt-get install -U python3 python3-pip
+sudo apt-get install python3 python3-pip
 ```
 Windows:   
 Install Python3 from [www.python.org/getit](https://www.python.org/getit/).  
 
 ### Install fnschool and run it
 ```bash
 # install
@@ -262,14 +262,15 @@
 - [pandas](https://pandas.pydata.org/)  
 - [numpy](https://numpy.org/)  
 - [openpyxl](https://openpyxl.readthedocs.io/)  
 - [appdirs](http://github.com/ActiveState/appdirs)  
 
 
 ## Support
+
 Buy me a `coffee`:  
 
 ![Buy me a coffee](https://raw.githubusercontent.com/larryw3i/funingschool/master/Documentation/images/9237879a-f8d5-11ee-8411-23057db0a773.jpeg)
 
 ## License
 
 [GNU LESSER GENERAL PUBLIC LICENSE Version 3](https://github.com/larryw3i/funingschool/blob/master/LICENSE)
```

### Comparing `fnschool-20240412.2240.38/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240412.2250.49/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

