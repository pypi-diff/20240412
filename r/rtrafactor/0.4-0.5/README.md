# Comparing `tmp/rtrafactor-0.4.tar.gz` & `tmp/rtrafactor-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrafactor-0.4.tar", last modified: Fri Apr 12 10:43:21 2024, max compression
+gzip compressed data, was "rtrafactor-0.5.tar", last modified: Fri Apr 12 10:54:47 2024, max compression
```

## Comparing `rtrafactor-0.4.tar` & `rtrafactor-0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187794 rtrafactor-0.4/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:43:21.187571 rtrafactor-0.4/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.186409 rtrafactor-0.4/rtrafactor/
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.4/rtrafactor/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.4/rtrafactor/webconnect.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187260 rtrafactor-0.4/rtrafactor.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:43:21.187838 rtrafactor-0.4/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:43:09.000000 rtrafactor-0.4/setup.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187393 rtrafactor-0.4/tests/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.4/tests/test_webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:54:47.534288 rtrafactor-0.5/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:54:47.534088 rtrafactor-0.5/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:54:47.533096 rtrafactor-0.5/rtrafactor/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.5/rtrafactor/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:53:48.000000 rtrafactor-0.5/rtrafactor/setup.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.5/rtrafactor/webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:54:47.533779 rtrafactor-0.5/rtrafactor.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:54:47.000000 rtrafactor-0.5/rtrafactor.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      270 2024-04-12 10:54:47.000000 rtrafactor-0.5/rtrafactor.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:54:47.000000 rtrafactor-0.5/rtrafactor.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:54:47.000000 rtrafactor-0.5/rtrafactor.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:54:47.000000 rtrafactor-0.5/rtrafactor.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:54:47.534340 rtrafactor-0.5/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:54:42.000000 rtrafactor-0.5/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:54:47.533913 rtrafactor-0.5/tests/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.5/tests/test_webconnect.py
```

### Comparing `rtrafactor-0.4/rtrafactor/__init__.py` & `rtrafactor-0.5/rtrafactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rtrafactor-0.4/rtrafactor/webconnect.py` & `rtrafactor-0.5/rtrafactor/webconnect.py`

 * *Files identical despite different names*

