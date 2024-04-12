# Comparing `tmp/rtrafactor-0.1.tar.gz` & `tmp/rtrafactor-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtrafactor-0.1.tar", last modified: Fri Apr 12 09:52:37 2024, max compression
+gzip compressed data, was "rtrafactor-0.2.tar", last modified: Fri Apr 12 10:26:27 2024, max compression
```

## Comparing `rtrafactor-0.1.tar` & `rtrafactor-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:52:37.743746 rtrafactor-0.1/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 09:52:37.743556 rtrafactor-0.1/PKG-INFO
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:52:37.742706 rtrafactor-0.1/rtrafactor/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:42:06.000000 rtrafactor-0.1/rtrafactor/__init__.py
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:42:17.000000 rtrafactor-0.1/rtrafactor/webconnect.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:52:37.743286 rtrafactor-0.1/rtrafactor.egg-info/
--rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 09:52:37.000000 rtrafactor-0.1/rtrafactor.egg-info/PKG-INFO
--rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 09:52:37.000000 rtrafactor-0.1/rtrafactor.egg-info/SOURCES.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 09:52:37.000000 rtrafactor-0.1/rtrafactor.egg-info/dependency_links.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 09:52:37.000000 rtrafactor-0.1/rtrafactor.egg-info/requires.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 09:52:37.000000 rtrafactor-0.1/rtrafactor.egg-info/top_level.txt
--rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 09:52:37.743794 rtrafactor-0.1/setup.cfg
--rw-r--r--   0 akhouriudit   (501) staff       (20)      482 2024-04-12 09:52:24.000000 rtrafactor-0.1/setup.py
-drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:52:37.743401 rtrafactor-0.1/tests/
--rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.1/tests/test_webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.733166 rtrafactor-0.2/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:26:27.732893 rtrafactor-0.2/PKG-INFO
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.731788 rtrafactor-0.2/rtrafactor/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:25:01.000000 rtrafactor-0.2/rtrafactor/__init__.py
+-rw-r--r--   0 akhouriudit   (501) staff       (20)     3289 2024-04-12 10:01:38.000000 rtrafactor-0.2/rtrafactor/webconnect.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.732582 rtrafactor-0.2/rtrafactor.egg-info/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      235 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/PKG-INFO
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      250 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/SOURCES.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        1 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/dependency_links.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       31 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/requires.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       11 2024-04-12 10:26:27.000000 rtrafactor-0.2/rtrafactor.egg-info/top_level.txt
+-rw-r--r--   0 akhouriudit   (501) staff       (20)       38 2024-04-12 10:26:27.733213 rtrafactor-0.2/setup.cfg
+-rw-r--r--   0 akhouriudit   (501) staff       (20)      483 2024-04-12 10:26:02.000000 rtrafactor-0.2/setup.py
+drwxr-xr-x   0 akhouriudit   (501) staff       (20)        0 2024-04-12 10:26:27.732704 rtrafactor-0.2/tests/
+-rw-r--r--   0 akhouriudit   (501) staff       (20)        0 2024-04-12 09:44:55.000000 rtrafactor-0.2/tests/test_webconnect.py
```

