# Comparing `tmp/rtrafactor-0.3.tar.gz` & `tmp/rtrafactor-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrafactor-0.3.tar", last modified: Fri Apr 12 10:39:21 2024, max compression
+gzip compressed data, was "rtrafactor-0.4.tar", last modified: Fri Apr 12 10:43:21 2024, max compression
```

## Comparing `rtrafactor-0.3.tar` & `rtrafactor-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.662244 rtrafactor-0.3/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:39:21.662047 rtrafactor-0.3/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661065 rtrafactor-0.3/rtrafactor/
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.3/rtrafactor/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.3/rtrafactor/webconnect.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661770 rtrafactor-0.3/rtrafactor.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:39:21.000000 rtrafactor-0.3/rtrafactor.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:39:21.662292 rtrafactor-0.3/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:36:29.000000 rtrafactor-0.3/setup.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:39:21.661898 rtrafactor-0.3/tests/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.3/tests/test_webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187794 rtrafactor-0.4/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:43:21.187571 rtrafactor-0.4/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.186409 rtrafactor-0.4/rtrafactor/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3193 2024-04-12 10:38:43.000000 rtrafactor-0.4/rtrafactor/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.4/rtrafactor/webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187260 rtrafactor-0.4/rtrafactor.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:43:21.000000 rtrafactor-0.4/rtrafactor.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:43:21.187838 rtrafactor-0.4/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:43:09.000000 rtrafactor-0.4/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:43:21.187393 rtrafactor-0.4/tests/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.4/tests/test_webconnect.py
```

### Comparing `rtrafactor-0.3/rtrafactor/__init__.py` & `rtrafactor-0.4/rtrafactor/__init__.py`

 * *Files identical despite different names*

### Comparing `rtrafactor-0.3/rtrafactor/webconnect.py` & `rtrafactor-0.4/rtrafactor/webconnect.py`

 * *Files identical despite different names*

