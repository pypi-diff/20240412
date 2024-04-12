# Comparing `tmp/db_sync_tool-kmi-2.9.1.tar.gz` & `tmp/db_sync_tool-kmi-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_sync_tool-kmi-2.9.1.tar", last modified: Wed May  4 14:28:45 2022, max compression
+gzip compressed data, was "db_sync_tool-kmi-2.9.2.tar", last modified: Wed May 11 13:12:39 2022, max compression
```

## Comparing `db_sync_tool-kmi-2.9.1.tar` & `db_sync_tool-kmi-2.9.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.185417 db_sync_tool-kmi-2.9.1/
--rw-r--r--   0 kmi        (501) staff       (20)    13870 2022-05-04 14:28:45.185187 db_sync_tool-kmi-2.9.1/PKG-INFO
--rw-r--r--   0 kmi        (501) staff       (20)    11029 2022-04-02 16:32:15.000000 db_sync_tool-kmi-2.9.1/README.md
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.180889 db_sync_tool-kmi-2.9.1/db_sync_tool/
--rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 17:28:42.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/__init__.py
--rw-r--r--   0 kmi        (501) staff       (20)    11038 2022-04-02 16:24:28.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/__main__.py
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.181395 db_sync_tool-kmi-2.9.1/db_sync_tool/database/
--rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 16:30:04.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/database/__init__.py
--rw-r--r--   0 kmi        (501) staff       (20)     7429 2022-04-01 16:06:25.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/database/process.py
--rw-r--r--   0 kmi        (501) staff       (20)     7658 2022-04-08 09:34:30.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/database/utility.py
--rw-r--r--   0 kmi        (501) staff       (20)      164 2022-05-04 14:28:17.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/info.py
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.182315 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/
--rw-r--r--   0 kmi        (501) staff       (20)        0 2021-04-13 17:44:57.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/__init__.py
--rw-r--r--   0 kmi        (501) staff       (20)     1481 2021-04-13 17:45:07.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/drupal.py
--rw-r--r--   0 kmi        (501) staff       (20)     1151 2021-04-13 17:45:26.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/laravel.py
--rw-r--r--   0 kmi        (501) staff       (20)     2562 2021-04-13 17:45:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/symfony.py
--rw-r--r--   0 kmi        (501) staff       (20)     2605 2022-03-06 12:21:09.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/typo3.py
--rw-r--r--   0 kmi        (501) staff       (20)     1444 2021-04-13 17:46:29.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/wordpress.py
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.183007 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/
--rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 16:45:51.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/__init__.py
--rw-r--r--   0 kmi        (501) staff       (20)     6553 2022-04-10 17:02:04.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/client.py
--rw-r--r--   0 kmi        (501) staff       (20)     4082 2022-02-13 19:19:48.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/rsync.py
--rw-r--r--   0 kmi        (501) staff       (20)     1188 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/system.py
--rw-r--r--   0 kmi        (501) staff       (20)     5872 2022-02-13 19:21:47.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/transfer.py
--rw-r--r--   0 kmi        (501) staff       (20)     3264 2021-08-31 09:01:29.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/remote/utility.py
--rw-r--r--   0 kmi        (501) staff       (20)     2087 2022-04-02 16:24:50.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/sync.py
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.184384 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/
--rw-r--r--   0 kmi        (501) staff       (20)        0 2020-10-20 17:39:22.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/__init__.py
--rw-r--r--   0 kmi        (501) staff       (20)     7987 2022-04-10 16:46:34.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/helper.py
--rw-r--r--   0 kmi        (501) staff       (20)     2558 2022-04-02 16:45:55.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/info.py
--rw-r--r--   0 kmi        (501) staff       (20)      869 2021-04-13 17:58:30.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/log.py
--rw-r--r--   0 kmi        (501) staff       (20)     8571 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/mode.py
--rw-r--r--   0 kmi        (501) staff       (20)     4592 2021-06-21 14:56:33.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/output.py
--rw-r--r--   0 kmi        (501) staff       (20)     6624 2022-03-06 12:10:26.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/parser.py
--rw-r--r--   0 kmi        (501) staff       (20)    17295 2022-05-04 14:27:06.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/system.py
--rw-r--r--   0 kmi        (501) staff       (20)     3530 2021-04-13 18:07:28.000000 db_sync_tool-kmi-2.9.1/db_sync_tool/utility/validation.py
-drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-04 14:28:45.185004 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/
--rw-r--r--   0 kmi        (501) staff       (20)    13870 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/PKG-INFO
--rw-r--r--   0 kmi        (501) staff       (20)     1106 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/SOURCES.txt
--rw-r--r--   0 kmi        (501) staff       (20)        1 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/dependency_links.txt
--rw-r--r--   0 kmi        (501) staff       (20)       61 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/entry_points.txt
--rw-r--r--   0 kmi        (501) staff       (20)      109 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/requires.txt
--rw-r--r--   0 kmi        (501) staff       (20)       13 2022-05-04 14:28:44.000000 db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/top_level.txt
--rw-r--r--   0 kmi        (501) staff       (20)       38 2022-05-04 14:28:45.185475 db_sync_tool-kmi-2.9.1/setup.cfg
--rw-r--r--   0 kmi        (501) staff       (20)     1554 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.1/setup.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.363721 db_sync_tool-kmi-2.9.2/
+-rw-r--r--   0 kmi        (501) staff       (20)    13870 2022-05-11 13:12:39.363552 db_sync_tool-kmi-2.9.2/PKG-INFO
+-rw-r--r--   0 kmi        (501) staff       (20)    11029 2022-04-02 16:32:15.000000 db_sync_tool-kmi-2.9.2/README.md
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.358576 db_sync_tool-kmi-2.9.2/db_sync_tool/
+-rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 17:28:42.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/__init__.py
+-rw-r--r--   0 kmi        (501) staff       (20)    11038 2022-04-02 16:24:28.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/__main__.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.359184 db_sync_tool-kmi-2.9.2/db_sync_tool/database/
+-rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 16:30:04.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/database/__init__.py
+-rw-r--r--   0 kmi        (501) staff       (20)     7429 2022-04-01 16:06:25.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/database/process.py
+-rw-r--r--   0 kmi        (501) staff       (20)     7659 2022-05-11 13:11:12.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/database/utility.py
+-rw-r--r--   0 kmi        (501) staff       (20)      164 2022-05-11 13:12:24.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/info.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.360276 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/
+-rw-r--r--   0 kmi        (501) staff       (20)        0 2021-04-13 17:44:57.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/__init__.py
+-rw-r--r--   0 kmi        (501) staff       (20)     1481 2021-04-13 17:45:07.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/drupal.py
+-rw-r--r--   0 kmi        (501) staff       (20)     1151 2021-04-13 17:45:26.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/laravel.py
+-rw-r--r--   0 kmi        (501) staff       (20)     2562 2021-04-13 17:45:44.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/symfony.py
+-rw-r--r--   0 kmi        (501) staff       (20)     2605 2022-03-06 12:21:09.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/typo3.py
+-rw-r--r--   0 kmi        (501) staff       (20)     1444 2021-04-13 17:46:29.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/wordpress.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.361003 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/
+-rw-r--r--   0 kmi        (501) staff       (20)        0 2020-11-26 16:45:51.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/__init__.py
+-rw-r--r--   0 kmi        (501) staff       (20)     6553 2022-04-10 17:02:04.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/client.py
+-rw-r--r--   0 kmi        (501) staff       (20)     4082 2022-02-13 19:19:48.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/rsync.py
+-rw-r--r--   0 kmi        (501) staff       (20)     1188 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/system.py
+-rw-r--r--   0 kmi        (501) staff       (20)     5872 2022-02-13 19:21:47.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/transfer.py
+-rw-r--r--   0 kmi        (501) staff       (20)     3264 2021-08-31 09:01:29.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/remote/utility.py
+-rw-r--r--   0 kmi        (501) staff       (20)     2087 2022-04-02 16:24:50.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/sync.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.362594 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/
+-rw-r--r--   0 kmi        (501) staff       (20)        0 2020-10-20 17:39:22.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/__init__.py
+-rw-r--r--   0 kmi        (501) staff       (20)     7987 2022-04-10 16:46:34.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/helper.py
+-rw-r--r--   0 kmi        (501) staff       (20)     2558 2022-04-02 16:45:55.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/info.py
+-rw-r--r--   0 kmi        (501) staff       (20)      869 2021-04-13 17:58:30.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/log.py
+-rw-r--r--   0 kmi        (501) staff       (20)     8571 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/mode.py
+-rw-r--r--   0 kmi        (501) staff       (20)     4592 2021-06-21 14:56:33.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/output.py
+-rw-r--r--   0 kmi        (501) staff       (20)     6624 2022-03-06 12:10:26.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/parser.py
+-rw-r--r--   0 kmi        (501) staff       (20)    17295 2022-05-04 14:27:06.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/system.py
+-rw-r--r--   0 kmi        (501) staff       (20)     3530 2021-04-13 18:07:28.000000 db_sync_tool-kmi-2.9.2/db_sync_tool/utility/validation.py
+drwxr-xr-x   0 kmi        (501) staff       (20)        0 2022-05-11 13:12:39.363343 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/
+-rw-r--r--   0 kmi        (501) staff       (20)    13870 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/PKG-INFO
+-rw-r--r--   0 kmi        (501) staff       (20)     1106 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/SOURCES.txt
+-rw-r--r--   0 kmi        (501) staff       (20)        1 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/dependency_links.txt
+-rw-r--r--   0 kmi        (501) staff       (20)       61 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/entry_points.txt
+-rw-r--r--   0 kmi        (501) staff       (20)      109 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/requires.txt
+-rw-r--r--   0 kmi        (501) staff       (20)       13 2022-05-11 13:12:39.000000 db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/top_level.txt
+-rw-r--r--   0 kmi        (501) staff       (20)       38 2022-05-11 13:12:39.363760 db_sync_tool-kmi-2.9.2/setup.cfg
+-rw-r--r--   0 kmi        (501) staff       (20)     1554 2022-04-10 15:45:11.000000 db_sync_tool-kmi-2.9.2/setup.py
```

### Comparing `db_sync_tool-kmi-2.9.1/PKG-INFO` & `db_sync_tool-kmi-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_sync_tool-kmi
-Version: 2.9.1
+Version: 2.9.2
 Summary: Synchronize a database from and to host systems.
 Home-page: https://github.com/jackd248/db-sync-tool
 Author: Konrad Michalik
 Author-email: support@konradmichalik.eu
 License: MIT
 Description: # db sync tool
```

### Comparing `db_sync_tool-kmi-2.9.1/README.md` & `db_sync_tool-kmi-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/__main__.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/database/process.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/database/process.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/database/utility.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/database/utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
     """
     Generate specific tables for export
     :return: String
     """
     if system.config['tables'] == '':
         return ''
 
-    _result = ''
+    _result = ' '
     _tables = system.config['tables'].split(',')
     for _table in _tables:
         _result += '\'' + _table + '\' '
     return _result
 
 
 def generate_mysql_credentials(client):
```

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/drupal.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/drupal.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/laravel.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/laravel.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/symfony.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/symfony.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/typo3.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/typo3.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/recipes/wordpress.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/recipes/wordpress.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/remote/client.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/remote/client.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/remote/rsync.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/remote/rsync.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/remote/system.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/remote/system.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/remote/transfer.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/remote/transfer.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/remote/utility.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/remote/utility.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/sync.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/sync.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/helper.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/helper.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/info.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/info.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/log.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/log.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/mode.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/mode.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/output.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/output.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/parser.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/parser.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/system.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/system.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool/utility/validation.py` & `db_sync_tool-kmi-2.9.2/db_sync_tool/utility/validation.py`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/PKG-INFO` & `db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-sync-tool-kmi
-Version: 2.9.1
+Version: 2.9.2
 Summary: Synchronize a database from and to host systems.
 Home-page: https://github.com/jackd248/db-sync-tool
 Author: Konrad Michalik
 Author-email: support@konradmichalik.eu
 License: MIT
 Description: # db sync tool
```

### Comparing `db_sync_tool-kmi-2.9.1/db_sync_tool_kmi.egg-info/SOURCES.txt` & `db_sync_tool-kmi-2.9.2/db_sync_tool_kmi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `db_sync_tool-kmi-2.9.1/setup.py` & `db_sync_tool-kmi-2.9.2/setup.py`

 * *Files identical despite different names*

