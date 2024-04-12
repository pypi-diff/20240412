# Comparing `tmp/fnschool-20240412.1309.2.tar.gz` & `tmp/fnschool-20240412.1947.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240412.1309.2.tar", last modified: Fri Apr 12 05:09:07 2024, max compression
+gzip compressed data, was "fnschool-20240412.1947.9.tar", last modified: Fri Apr 12 11:47:14 2024, max compression
```

## Comparing `fnschool-20240412.1309.2.tar` & `fnschool-20240412.1947.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.183568 fnschool-20240412.1309.2/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.1309.2/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-12 05:09:07.183568 fnschool-20240412.1309.2/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240412.1309.2/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.1309.2/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 05:09:07.183568 fnschool-20240412.1309.2/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.166571 fnschool-20240412.1309.2/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.172570 fnschool-20240412.1309.2/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.177569 fnschool-20240412.1309.2/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.1309.2/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/config.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.180568 fnschool-20240412.1309.2/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.1309.2/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.1309.2/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14625 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/canteen/profile.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.1309.2/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    97347 2024-04-12 05:05:42.000000 fnschool-20240412.1309.2/src/fnschool/canteen/workbook.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.180568 fnschool-20240412.1309.2/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.1309.2/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.1309.2/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.169571 fnschool-20240412.1309.2/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.167571 fnschool-20240412.1309.2/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.180568 fnschool-20240412.1309.2/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.168571 fnschool-20240412.1309.2/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.181568 fnschool-20240412.1309.2/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    12127 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.168571 fnschool-20240412.1309.2/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.181568 fnschool-20240412.1309.2/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.168571 fnschool-20240412.1309.2/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.181568 fnschool-20240412.1309.2/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.169571 fnschool-20240412.1309.2/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.182568 fnschool-20240412.1309.2/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 05:09:02.000000 fnschool-20240412.1309.2/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/log.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.1309.2/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 05:09:07.182568 fnschool-20240412.1309.2/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 05:09:07.000000 fnschool-20240412.1309.2/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.054263 fnschool-20240412.1947.9/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240412.1947.9/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-12 11:47:14.054263 fnschool-20240412.1947.9/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-03-07 05:13:02.000000 fnschool-20240412.1947.9/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240412.1947.9/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-04-12 11:47:14.054263 fnschool-20240412.1947.9/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.037263 fnschool-20240412.1947.9/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.043263 fnschool-20240412.1947.9/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      233 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       80 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.048263 fnschool-20240412.1947.9/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13523 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2036 2024-03-27 13:44:47.000000 fnschool-20240412.1947.9/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2031 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/config.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.050263 fnschool-20240412.1947.9/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   816213 2024-04-12 04:56:59.000000 fnschool-20240412.1947.9/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240412.1947.9/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14625 2024-04-12 06:11:32.000000 fnschool-20240412.1947.9/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1826 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1369 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/canteen/profile.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-04-12 03:08:37.000000 fnschool-20240412.1947.9/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98780 2024-04-12 11:33:17.000000 fnschool-20240412.1947.9/src/fnschool/canteen/workbook.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.051263 fnschool-20240412.1947.9/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240412.1947.9/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1088 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      952 2024-04-12 03:34:03.000000 fnschool-20240412.1947.9/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      828 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.040263 fnschool-20240412.1947.9/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.038263 fnschool-20240412.1947.9/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.051263 fnschool-20240412.1947.9/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.039263 fnschool-20240412.1947.9/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.051263 fnschool-20240412.1947.9/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    12193 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.039263 fnschool-20240412.1947.9/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.051263 fnschool-20240412.1947.9/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.039263 fnschool-20240412.1947.9/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.052263 fnschool-20240412.1947.9/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.040263 fnschool-20240412.1947.9/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.052263 fnschool-20240412.1947.9/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-04-12 11:47:09.000000 fnschool-20240412.1947.9/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)      452 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/log.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1200 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-04-11 23:50:02.000000 fnschool-20240412.1947.9/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-04-12 11:47:14.053263 fnschool-20240412.1947.9/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)     9963 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1129 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-04-12 11:47:14.000000 fnschool-20240412.1947.9/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240412.1309.2/LICENSE` & `fnschool-20240412.1947.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/PKG-INFO` & `fnschool-20240412.1947.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.1309.2
+Version: 20240412.1947.9
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240412.1309.2/pyproject.toml` & `fnschool-20240412.1947.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/bill.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/canteen.toml` & `fnschool-20240412.1947.9/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/config.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240412.1947.9/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240412.1947.9/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/food.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/path.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/profile.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/test.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/canteen/workbook.py` & `fnschool-20240412.1947.9/src/fnschool/canteen/workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -645,138 +645,176 @@
         time_nodes = sorted(
             [
                 tn
                 for tn in self.bill.get_time_nodes()
                 if tn[1].month == self.bill.month
             ]
         )
+        time_nodes_mm1 = sorted(
+            [
+                tn
+                for tn in self.bill.get_time_nodes()
+                if tn[1].month == self.bill.month - 1
+            ]
+        )
         t0, t1 = time_nodes[-1]
         cfoods = [
             f
             for f in self.food.get_foods()
-            if f.check_date.month == self.bill.month
+            if (
+                (
+                    f.check_date.month == self.bill.month
+                    or (
+                        self.bill.month
+                        in [d.month for d, c in f.consuming_list]
+                    )
+                )
+                and not f.is_negligible
+            )
         ]
-        cfood_names = list(set([f.name for f in cfoods]))
-        days_num = calendar.monthrange(t1.year, self.bill.month)[1]
+        food_names = list(set([f.name for f in cfoods]))
         wb = self.get_bill_workbook()
-
-        tn0_dm1 = time_nodes[0][0] + timedelta(days=-1)
+        tn0_dm1 = (
+            (time_nodes[0][0] + timedelta(days=-1))
+            if len(time_nodes_mm1) < 1
+            else (time_nodes_mm1[-1][1])
+        )
 
         rfoods = [
             f
             for f in self.food.get_foods()
             if (
                 f.get_remainder_by_time(tn0_dm1) > 0
-                and f.check_date <= time_nodes[-1][1]
+                and not f.is_negligible
+                and f.check_date.month < self.bill.month
             )
         ]
-        rfoods_names = list(set([f.name for f in rfoods]))
-        for rfood_name in rfoods_names:
-            sheet = self.get_food_sheet(rfood_name)
+
+        food_names = list(set([f.name for f in rfoods] + food_names))
+
+        sheet = None
+        for food_name in food_names:
+            sheet = self.get_food_sheet(food_name)
             form_index_range = self.get_food_form_index(sheet)
             index_start, index_end = form_index_range
-            entry_index = 0
-            for food in rfoods:
-                if food.name == rfood_name:
-                    row_index = index_start + entry_index
+
+            for row_index in range(index_start, index_end - 1):
+                for col_index in range(1, 14):
+                    sheet.cell(row_index, col_index).value = ""
+            row_index = index_start 
+            col_index = 1
+
+            _rfoods = [f for f in rfoods if f.name == food_name]
+            _cfoods = [f for f in cfoods if f.name == food_name]
+
+            self.unmerge_cells_of_sheet(sheet)
+
+            sheet.cell(index_start - 2, 1, f"{t1.year}年")
+
+           
+            if len(_rfoods) > 0:
+                for _row_index in range(index_start, index_start + len(_rfoods)):
+                    food = _rfoods[_row_index - index_start]
                     sheet.cell(
-                        row_index,
+                        _row_index,
                         3,
                         ("上年结转" if t1.month == 1 else "上月结转"),
                     )
-                    for col_index in [1, 2, 4, 5, 6, 7, 8, 9]:
-                        sheet.cell(row_index, col_index, "")
                     sheet.cell(row_index, 10, food.count)
                     sheet.cell(row_index, 11, food.unit_price)
                     sheet.cell(row_index, 12, food.count * food.unit_price)
+                    row_index = _row_index   
+            else:
+                sheet.cell(
+                    row_index,
+                    3,
+                    ("上年结转" if t1.month == 1 else "上月结转"),
+                )
+                
 
-                    entry_index += 1
-
-        for cfood_name in cfood_names:
-            entry_index = 0
-            sheet = self.get_food_sheet(cfood_name)
-            self.unmerge_cells_of_sheet(sheet)
-            index_range = self.get_food_form_day_index(sheet)
-            index_start, index_end = index_range
-            for day_n in range(1, days_num + 1):
-                time_node = datetime(t1.year, t1.month, day_n)
-                for food in [f for f in cfoods if (f.name == cfood_name)]:
-                    _dates = [d for d, c in food.consuming_list]
-                    if time_node in _dates:
-                        row_index = index_start + entry_index
-                        _date, _count = [
-                            [d, c]
-                            for d, c in food.consuming_list
-                            if d == time_node
-                        ][0]
-                        _remainder = food.count - sum(
-                            [
-                                c
-                                for d, c in food.consuming_list
-                                if d <= time_node
-                            ]
-                        )
-
-                        sheet.cell(row_index, 2, time_node.day)
-                        sheet.cell(row_index, 6, "")
-                        sheet.cell(row_index, 7, _count)
-                        sheet.cell(row_index, 8, food.unit_price)
-                        sheet.cell(row_index, 9, _count * food.unit_price)
-                        sheet.cell(row_index, 10, _remainder)
-                        sheet.cell(row_index, 11, food.unit_price)
-                        sheet.cell(row_index, 12, _remainder * food.unit_price)
-
-                        entry_index += 1
-
-                    if food.check_date == time_node:
-                        row_index = index_start + entry_index
+            row_index += 1
 
-                        sheet.cell(row_index, 2, time_node.day)
+            _cdates = []
+            for food in _cfoods:
+                if len(food.consuming_list) > 0:
+                    _cdates += [d for d, c in food.consuming_list]
+                _cdates.append(food.check_date)
+            _cdates = [d for d in _cdates if d.month == self.bill.month]
+            _cdates = sorted(list(set(_cdates)))
+            
+            consuming_n = 1
+            warehousing_n = 1
+            for cdate in _cdates:
+                for food in _cfoods:
+
+                    if food.check_date == cdate:
+                        sheet.cell(row_index, 1, cdate.month)
+                        sheet.cell(row_index, 2, cdate.day)
                         sheet.cell(row_index, 4, food.count)
                         sheet.cell(row_index, 5, food.unit_price)
                         sheet.cell(row_index, 6, food.count * food.unit_price)
                         sheet.cell(row_index, 9, "")
                         sheet.cell(row_index, 10, food.count)
                         sheet.cell(row_index, 11, food.unit_price)
                         sheet.cell(row_index, 12, food.count * food.unit_price)
+                        sheet.cell(row_index, 13, f"R{cdate.month:0>2}{warehousing_n:0>2}")
+                        warehousing_n += 1
 
-                        entry_index += 1
-
-                    if food.check_date == time_node or time_node in _dates:
                         if "合计" in str(sheet.cell(row_index + 1, 3).value):
                             sheet.insert_rows(row_index + 1, 1)
 
-            self.format_food_sheet(sheet)
+                        row_index += 1
 
-            food_names = list(set([f.name for f in self.food.get_foods()]))
+                    if cdate in [ d for d,__ in food.consuming_list]:
+                        _count = [c for d,c in food.consuming_list if d == cdate][0]
+                        _remainder = food.count - sum(
+                            [c for d, c in food.consuming_list if d <= cdate]
+                        )
+                        sheet.cell(row_index, 1, cdate.month)
+                        sheet.cell(row_index, 2, cdate.day)
+                        sheet.cell(row_index, 6, "")
+                        sheet.cell(row_index, 7, _count)
+                        sheet.cell(row_index, 8, food.unit_price)
+                        sheet.cell(row_index, 9, _count * food.unit_price)
+                        sheet.cell(row_index, 10, _remainder)
+                        sheet.cell(row_index, 11, food.unit_price)
+                        sheet.cell(row_index, 12, _remainder * food.unit_price)
+                        sheet.cell(row_index, 13, f"C{cdate.month:0>2}{consuming_n:0>2}")
+                        consuming_n += 1
 
-            wb = self.get_bill_workbook()
-            wb.active = sheet
+                        if "合计" in str(sheet.cell(row_index + 1, 3).value):
+                            sheet.insert_rows(row_index + 1, 1)
 
+                        row_index += 1
+
+            self.format_food_sheet(sheet)
             print_info(_("Sheet '%s' was updated.") % sheet.title)
 
-        for name in food_names:
+        wb.active = sheet
+
+        _food_names = list(set([f.name for f in self.food.get_foods()]))
+        for name in _food_names:
             if self.includes_sheet(name):
                 sheet = self.get_bill_sheet(name)
                 sheet.sheet_properties.tabColor = "0" * 8
 
         print_info(_("All food sheets have their tab colors reset."))
 
-        for name in cfood_names:
+        for name in food_names:
             sheet = self.get_food_sheet(name)
             sheet.sheet_properties.tabColor = secrets.token_hex(4)
 
         print_info(
             _("Food sheets [{0}] have their tab colors recolor.").format(
-                " ".join(cfood_names)
+                " ".join(food_names)
             )
         )
         print_info(
             _("Food sheets [{0}] have been updated.").format(
-                " ".join(cfood_names)
+                " ".join(food_names)
             )
         )
 
     def get_food_form_day_index(self, sheet):
         indexes = []
         for row in sheet.iter_rows(
             min_row=1, max_row=sheet.max_row, min_col=1, max_col=14
@@ -1254,17 +1292,17 @@
                 if not any(
                     [o == self.bill.profile.org_name for o in _org_names]
                 ):
                     print_warning(
                         (
                             _('Organization name read from {0} are "{1}",')
                             if len(_org_names) > 1
-                            else _('Organization name read from {0} is "{1}",')
+                            else _('Organization name read from {0} is "{1}", ')
                         ).format(wb_fpath, " | ".join(_org_names))
-                        + _('But organization name of {0} is "{1}".').format(
+                        + _('but organization name of {0} is "{1}".').format(
                             f"{self.profile.label}({self.profile.name})",
                             self.profile.org_name,
                         )
                     )
                     print_error(
                         _("'{wb_fpath}' was discarded.").format(
                             wb_fpath=wb_fpath
@@ -1321,15 +1359,19 @@
                         check_date = self.clean_quotation_marks(
                             row[food_check_date_index].value
                         )
 
                         check_date = (
                             datetime.strptime(check_date, "%Y-%m-%d")
                             if "-" in check_date
-                            else datetime.strptime(check_date, "%Y%d%m")
+                            else (
+                                datetime.strptime(check_date, "%Y/%m/%d")
+                                if "/" in check_date
+                                else datetime.strptime(check_date, "%Y%d%m")
+                            )
                         )
                         org_name = row[food_org_name_index].value
 
                         if org_name != self.bill.profile.org_name:
                             if not wb_fpath in self.excluded_purchase_sheets:
                                 self.excluded_purchase_sheets.append(wb_fpath)
                             continue
@@ -2610,14 +2652,15 @@
         file_path = file_path.split(os.sep)[-1]
         file_path = file_path[:-5] + f".{uuid.uuid4()}.xlsx"
         file_path = self.get_profile_copy_data_dpath() / file_path
 
         return file_path
 
     def copy_bill_workbook(self, wb_fpath=None):
+        print_info(_("Copying workbook..."))
         file_path = wb_fpath or self.get_random_bill_workbook_copy_fpath()
         wb = self.get_bill_workbook()
         wb.save(file_path)
         print_info(_("Workbook '%s' was saved.") % file_path)
         return file_path
 
     def get_bill_sheet(self, name):
```

### Comparing `fnschool-20240412.1309.2/src/fnschool/entry.py` & `fnschool-20240412.1947.9/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/external.py` & `fnschool-20240412.1947.9/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/language.py` & `fnschool-20240412.1947.9/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240412.1947.9/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-04-12 13:05+0800\n"
-"PO-Revision-Date: 2024-04-12 13:06+0800\n"
+"POT-Creation-Date: 2024-04-12 19:26+0800\n"
+"PO-Revision-Date: 2024-04-12 19:27+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: zh_Hans_CN <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -18,17 +18,14 @@
 
 msgid "'{wb_fpath}' was discarded."
 msgstr "“{wb_fpath}” 已被舍去。"
 
 msgid "All food sheets have their tab colors reset."
 msgstr "所有食材台账表标签颜色已被重置。"
 
-msgid "But organization name of {0} is \"{1}\"."
-msgstr "但是 “{0}” 的 机构名（学校名）是 “{1}”。"
-
 msgid "Canteen related functions."
 msgstr "Cateen 的相关函数。"
 
 msgid "Command line interface of fnschool."
 msgstr "“fnschool“ 的命令行接口。"
 
 msgid "Configuration file '%s' was copied to '%s'."
@@ -39,14 +36,17 @@
 
 msgid "Consuming records:"
 msgstr "消耗记录："
 
 msgid "Consumptions were read."
 msgstr "每日食材消耗已被读取。"
 
+msgid "Copying workbook..."
+msgstr "正在复制工作簿......"
+
 msgid "Default time nodes of {0} have been used."
 msgstr "{0} 的默认时间节点被使用。"
 
 msgid "Directory %s was created."
 msgstr "目录 “%s” 已创建。"
 
 msgid "Directory '%s' has been made."
@@ -195,16 +195,16 @@
 
 msgid "Organization name or school name"
 msgstr "组织名 或 学校名"
 
 msgid "Organization name read from {0} are \"{1}\","
 msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”，"
 
-msgid "Organization name read from {0} is \"{1}\","
-msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”，"
+msgid "Organization name read from {0} is \"{1}\", "
+msgstr "从 “{0}” 中读取到的 机构名（学校名）是 “{1}”， "
 
 msgid "Please add codes to get foods from your suppliers."
 msgstr "没有与这个供应商相关的解析代码，你可以添加代码。"
 
 msgid "Please design the consumptions of spreadsheet '{0}' ."
 msgstr "请给工作簿 “{0}” 设计每天的消耗。"
 
@@ -379,14 +379,17 @@
 
 msgid ""
 "You can fill in the monthly missing data to food sheets, they will be saved "
 "for next updating."
 msgstr ""
 "你可以把 食材台账表 里面没有更新的月份的数据更新了，这些数据会被保存下来的。"
 
+msgid "but organization name of {0} is \"{1}\"."
+msgstr "但是 “{0}” 的 机构名（学校名）是 “{1}”。"
+
 msgid "fnschool"
 msgstr "fnschool"
 
 msgid "line '%s' has been discarded."
 msgstr "行 “%s” 被舍去。"
 
 msgid "values length is less than %s."
```

### Comparing `fnschool-20240412.1309.2/src/fnschool/path.py` & `fnschool-20240412.1947.9/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool/test.py` & `fnschool-20240412.1947.9/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240412.1309.2/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240412.1947.9/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240412.1309.2
+Version: 20240412.1947.9
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240412.1309.2/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240412.1947.9/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

