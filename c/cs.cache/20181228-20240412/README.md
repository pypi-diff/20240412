# Comparing `tmp/cs.cache-20181228.tar.gz` & `tmp/cs.cache-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs.cache-20181228.tar", last modified: Fri Dec 28 03:45:35 2018, max compression
+gzip compressed data, was "cs.cache-20240412.tar", last modified: Fri Apr 12 05:54:46 2024, max compression
```

## Comparing `cs.cache-20181228.tar` & `cs.cache-20240412.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2018-12-28 03:45:35.000000 cs.cache-20181228/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (508)       21 2018-12-28 03:45:28.000000 cs.cache-20181228/lib/python/cs/__init__.py
--rw-r--r--   0 cameron    (501) cameron    (508)     4960 2018-12-28 03:45:28.000000 cs.cache-20181228/lib/python/cs/cache.py
-drwxrwxr-x   0 cameron    (501) cameron    (508)        0 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs.cache.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (508)        1 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs.cache.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)     1161 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs.cache.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (508)      241 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs.cache.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)        3 2018-12-28 03:45:35.000000 cs.cache-20181228/lib/python/cs.cache.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (508)       19 2018-12-28 03:45:35.000000 cs.cache-20181228/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (508)     1161 2018-12-28 03:45:35.000000 cs.cache-20181228/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (508)       38 2018-12-28 03:45:35.000000 cs.cache-20181228/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (508)     1190 2018-12-28 03:45:35.000000 cs.cache-20181228/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.823222 cs.cache-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:54:43.000000 cs.cache-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4046 2024-04-12 05:54:46.822922 cs.cache-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3264 2024-04-12 05:54:43.000000 cs.cache-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.817482 cs.cache-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.818083 cs.cache-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.819962 cs.cache-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    11563 2024-04-12 05:54:29.000000 cs.cache-20240412/lib/python/cs/cache.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:54:46.822417 cs.cache-20240412/lib/python/cs.cache.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4046 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      118 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:54:46.000000 cs.cache-20240412/lib/python/cs.cache.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4525 2024-04-12 05:54:45.000000 cs.cache-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:54:46.823329 cs.cache-20240412/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

