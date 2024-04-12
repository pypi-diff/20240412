# Comparing `tmp/messari-1.0.0.tar.gz` & `tmp/messari-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/messari-1.0.0.tar", last modified: Tue Nov 24 10:35:43 2020, max compression
+gzip compressed data, was "messari-2.0.0.tar", last modified: Fri Apr 12 13:21:47 2024, max compression
```

## Comparing `messari-1.0.0.tar` & `messari-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 10:35:43.987740 messari-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     5020 2020-11-24 10:35:43.987740 messari-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3544 2020-11-24 10:35:34.000000 messari-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 10:35:43.987740 messari-1.0.0/messari/
--rw-r--r--   0 runner    (1001) docker     (116)      221 2020-11-24 10:35:34.000000 messari-1.0.0/messari/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      319 2020-11-24 10:35:34.000000 messari-1.0.0/messari/__version__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9398 2020-11-24 10:35:34.000000 messari-1.0.0/messari/messari.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-24 10:35:43.987740 messari-1.0.0/messari.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5020 2020-11-24 10:35:43.000000 messari-1.0.0/messari.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      234 2020-11-24 10:35:43.000000 messari-1.0.0/messari.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-24 10:35:43.000000 messari-1.0.0/messari.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2020-11-24 10:35:43.000000 messari-1.0.0/messari.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2020-11-24 10:35:43.000000 messari-1.0.0/messari.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-11-24 10:35:43.987740 messari-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1078 2020-11-24 10:35:34.000000 messari-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-12 13:21:38.000000 messari-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 13:21:47.437520 messari-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-12 13:21:38.000000 messari-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.433520 messari-2.0.0/messari/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-12 13:21:38.000000 messari-2.0.0/messari/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-12 13:21:38.000000 messari-2.0.0/messari/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-12 13:21:38.000000 messari-2.0.0/messari/messari.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/messari.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 13:21:47.000000 messari-2.0.0/messari.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 13:21:47.437520 messari-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-12 13:21:38.000000 messari-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 13:21:47.437520 messari-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-12 13:21:38.000000 messari-2.0.0/tests/test_messari.py
```

### Comparing `messari-1.0.0/setup.py` & `messari-2.0.0/setup.py`

 * *Files identical despite different names*

