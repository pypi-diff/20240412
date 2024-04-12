# Comparing `tmp/egypt-0.0.1.tar.gz` & `tmp/egypt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egypt-0.0.1.tar", last modified: Thu Apr 11 07:51:15 2024, max compression
+gzip compressed data, was "egypt-0.0.2.tar", last modified: Fri Apr 12 09:36:36 2024, max compression
```

## Comparing `egypt-0.0.1.tar` & `egypt-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-11 07:51:15.368215 egypt-0.0.1/
--rw-r--r--   0 kimshan    (501) staff       (20)      116 2024-04-11 07:51:15.367731 egypt-0.0.1/PKG-INFO
-drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-11 07:51:15.359985 egypt-0.0.1/egypt/
--rw-r--r--   0 kimshan    (501) staff       (20)       60 2024-04-09 00:16:41.000000 egypt-0.0.1/egypt/__init__.py
--rw-r--r--   0 kimshan    (501) staff       (20)    15679 2024-04-11 02:48:12.000000 egypt-0.0.1/egypt/pyramid.py
-drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-11 07:51:15.362115 egypt-0.0.1/egypt.egg-info/
--rw-r--r--   0 kimshan    (501) staff       (20)      116 2024-04-11 07:51:15.000000 egypt-0.0.1/egypt.egg-info/PKG-INFO
--rw-r--r--   0 kimshan    (501) staff       (20)      261 2024-04-11 07:51:15.000000 egypt-0.0.1/egypt.egg-info/SOURCES.txt
--rw-r--r--   0 kimshan    (501) staff       (20)        1 2024-04-11 07:51:15.000000 egypt-0.0.1/egypt.egg-info/dependency_links.txt
--rw-r--r--   0 kimshan    (501) staff       (20)       10 2024-04-11 07:51:15.000000 egypt-0.0.1/egypt.egg-info/top_level.txt
-drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-11 07:51:15.366271 egypt-0.0.1/old/
--rw-r--r--   0 kimshan    (501) staff       (20)     4937 2024-04-08 11:32:04.000000 egypt-0.0.1/old/__init__.py
--rw-r--r--   0 kimshan    (501) staff       (20)     2732 2023-12-03 01:35:53.000000 egypt-0.0.1/old/fusion.py
--rw-r--r--   0 kimshan    (501) staff       (20)        0 2024-04-08 11:48:43.000000 egypt-0.0.1/old/new_pyramid.py
--rw-r--r--   0 kimshan    (501) staff       (20)     1589 2023-11-14 07:48:37.000000 egypt-0.0.1/old/plot.py
--rw-r--r--   0 kimshan    (501) staff       (20)    10485 2024-04-08 11:44:40.000000 egypt-0.0.1/old/pyramid.py
--rw-r--r--   0 kimshan    (501) staff       (20)     2630 2023-12-03 06:07:09.000000 egypt-0.0.1/old/source.py
--rw-r--r--   0 kimshan    (501) staff       (20)      370 2023-12-05 11:08:24.000000 egypt-0.0.1/old/test.py
--rw-r--r--   0 kimshan    (501) staff       (20)       38 2024-04-11 07:51:15.368314 egypt-0.0.1/setup.cfg
--rw-r--r--   0 kimshan    (501) staff       (20)      206 2024-04-11 07:49:09.000000 egypt-0.0.1/setup.py
+drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-12 09:36:36.411627 egypt-0.0.2/
+-rw-r--r--   0 kimshan    (501) staff       (20)      427 2024-04-12 09:36:36.410930 egypt-0.0.2/PKG-INFO
+drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-12 09:36:36.398658 egypt-0.0.2/egypt/
+-rw-r--r--   0 kimshan    (501) staff       (20)      653 2024-04-12 02:57:11.000000 egypt-0.0.2/egypt/__init__.py
+-rw-r--r--   0 kimshan    (501) staff       (20)    26082 2024-04-12 09:35:36.000000 egypt-0.0.2/egypt/pyramid.py
+drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-12 09:36:36.402496 egypt-0.0.2/egypt.egg-info/
+-rw-r--r--   0 kimshan    (501) staff       (20)      427 2024-04-12 09:36:36.000000 egypt-0.0.2/egypt.egg-info/PKG-INFO
+-rw-r--r--   0 kimshan    (501) staff       (20)      289 2024-04-12 09:36:36.000000 egypt-0.0.2/egypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kimshan    (501) staff       (20)        1 2024-04-12 09:36:36.000000 egypt-0.0.2/egypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kimshan    (501) staff       (20)       29 2024-04-12 09:36:36.000000 egypt-0.0.2/egypt.egg-info/requires.txt
+-rw-r--r--   0 kimshan    (501) staff       (20)       10 2024-04-12 09:36:36.000000 egypt-0.0.2/egypt.egg-info/top_level.txt
+drwxr-xr-x   0 kimshan    (501) staff       (20)        0 2024-04-12 09:36:36.409718 egypt-0.0.2/old/
+-rw-r--r--   0 kimshan    (501) staff       (20)     4937 2024-04-08 11:32:04.000000 egypt-0.0.2/old/__init__.py
+-rw-r--r--   0 kimshan    (501) staff       (20)     2732 2023-12-03 01:35:53.000000 egypt-0.0.2/old/fusion.py
+-rw-r--r--   0 kimshan    (501) staff       (20)        0 2024-04-08 11:48:43.000000 egypt-0.0.2/old/new_pyramid.py
+-rw-r--r--   0 kimshan    (501) staff       (20)     1589 2023-11-14 07:48:37.000000 egypt-0.0.2/old/plot.py
+-rw-r--r--   0 kimshan    (501) staff       (20)    10485 2024-04-08 11:44:40.000000 egypt-0.0.2/old/pyramid.py
+-rw-r--r--   0 kimshan    (501) staff       (20)     2630 2023-12-03 06:07:09.000000 egypt-0.0.2/old/source.py
+-rw-r--r--   0 kimshan    (501) staff       (20)      370 2023-12-05 11:08:24.000000 egypt-0.0.2/old/test.py
+-rw-r--r--   0 kimshan    (501) staff       (20)       38 2024-04-12 09:36:36.411822 egypt-0.0.2/setup.cfg
+-rw-r--r--   0 kimshan    (501) staff       (20)      985 2024-04-12 09:36:34.000000 egypt-0.0.2/setup.py
```

### Comparing `egypt-0.0.1/old/__init__.py` & `egypt-0.0.2/old/__init__.py`

 * *Files identical despite different names*

### Comparing `egypt-0.0.1/old/fusion.py` & `egypt-0.0.2/old/fusion.py`

 * *Files identical despite different names*

### Comparing `egypt-0.0.1/old/plot.py` & `egypt-0.0.2/old/plot.py`

 * *Files identical despite different names*

### Comparing `egypt-0.0.1/old/pyramid.py` & `egypt-0.0.2/old/pyramid.py`

 * *Files identical despite different names*

### Comparing `egypt-0.0.1/old/source.py` & `egypt-0.0.2/old/source.py`

 * *Files identical despite different names*

