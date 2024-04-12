# Comparing `tmp/underhill-0.1.tar.gz` & `tmp/underhill-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underhill-0.1.tar", last modified: Thu Apr 11 21:34:57 2024, max compression
+gzip compressed data, was "underhill-0.2.tar", last modified: Fri Apr 12 00:20:33 2024, max compression
```

## Comparing `underhill-0.1.tar` & `underhill-0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-11 21:34:57.661082 underhill-0.1/
--rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-11 21:34:57.660986 underhill-0.1/PKG-INFO
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-11 21:34:57.660287 underhill-0.1/packages/
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-11 21:34:57.660471 underhill-0.1/packages/underhill/
--rw-r--r--   0 josiah     (501) staff       (20)        0 2024-04-11 21:17:26.000000 underhill-0.1/packages/underhill/__init__.py
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-11 21:34:57.660853 underhill-0.1/packages/underhill.egg-info/
--rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-11 21:34:57.000000 underhill-0.1/packages/underhill.egg-info/PKG-INFO
--rw-r--r--   0 josiah     (501) staff       (20)      207 2024-04-11 21:34:57.000000 underhill-0.1/packages/underhill.egg-info/SOURCES.txt
--rw-r--r--   0 josiah     (501) staff       (20)        1 2024-04-11 21:34:57.000000 underhill-0.1/packages/underhill.egg-info/dependency_links.txt
--rw-r--r--   0 josiah     (501) staff       (20)       10 2024-04-11 21:34:57.000000 underhill-0.1/packages/underhill.egg-info/top_level.txt
--rw-r--r--   0 josiah     (501) staff       (20)       38 2024-04-11 21:34:57.661113 underhill-0.1/setup.cfg
--rw-r--r--   0 josiah     (501) staff       (20)      377 2024-04-11 21:22:36.000000 underhill-0.1/setup.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 00:20:33.742935 underhill-0.2/
+-rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-12 00:20:33.742824 underhill-0.2/PKG-INFO
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 00:20:33.741238 underhill-0.2/packages/
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 00:20:33.741575 underhill-0.2/packages/underhill/
+-rw-r--r--   0 josiah     (501) staff       (20)        0 2024-04-11 21:17:26.000000 underhill-0.2/packages/underhill/__init__.py
+-rw-r--r--   0 josiah     (501) staff       (20)     1936 2024-04-12 00:11:35.000000 underhill-0.2/packages/underhill/expedition.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 00:20:33.742363 underhill-0.2/packages/underhill.egg-info/
+-rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-12 00:20:33.000000 underhill-0.2/packages/underhill.egg-info/PKG-INFO
+-rw-r--r--   0 josiah     (501) staff       (20)      305 2024-04-12 00:20:33.000000 underhill-0.2/packages/underhill.egg-info/SOURCES.txt
+-rw-r--r--   0 josiah     (501) staff       (20)        1 2024-04-12 00:20:33.000000 underhill-0.2/packages/underhill.egg-info/dependency_links.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       36 2024-04-12 00:20:33.000000 underhill-0.2/packages/underhill.egg-info/requires.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       10 2024-04-12 00:20:33.000000 underhill-0.2/packages/underhill.egg-info/top_level.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       38 2024-04-12 00:20:33.742967 underhill-0.2/setup.cfg
+-rw-r--r--   0 josiah     (501) staff       (20)      508 2024-04-12 00:20:33.000000 underhill-0.2/setup.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 00:20:33.742469 underhill-0.2/test/
+-rw-r--r--   0 josiah     (501) staff       (20)      346 2024-04-12 00:16:28.000000 underhill-0.2/test/test_expedition.py
```

