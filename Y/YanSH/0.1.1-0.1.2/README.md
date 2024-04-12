# Comparing `tmp/YanSH-0.1.1.tar.gz` & `tmp/YanSH-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YanSH-0.1.1.tar", last modified: Fri Apr 12 06:00:10 2024, max compression
+gzip compressed data, was "YanSH-0.1.2.tar", last modified: Fri Apr 12 06:15:41 2024, max compression
```

## Comparing `YanSH-0.1.1.tar` & `YanSH-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 06:00:10.873026 YanSH-0.1.1/
--rw-rw-rw-   0        0        0     1088 2024-04-12 05:09:42.000000 YanSH-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      236 2024-04-12 06:00:10.873026 YanSH-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-12 04:00:06.000000 YanSH-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 06:00:10.872012 YanSH-0.1.1/YanSH.egg-info/
--rw-rw-rw-   0        0        0      236 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      142 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 06:00:10.873026 YanSH-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      344 2024-04-12 05:57:20.000000 YanSH-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:41.075282 YanSH-0.1.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-12 05:09:42.000000 YanSH-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      236 2024-04-12 06:15:41.066226 YanSH-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-04-12 06:13:30.000000 YanSH-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:41.059122 YanSH-0.1.2/YanSH/
+-rw-rw-rw-   0        0        0     1969 2024-04-12 03:19:36.000000 YanSH-0.1.2/YanSH/Yan_def.py
+-rw-rw-rw-   0        0        0       14 2024-04-12 06:12:38.000000 YanSH-0.1.2/YanSH/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 06:15:41.065284 YanSH-0.1.2/YanSH.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-04-12 06:15:41.000000 YanSH-0.1.2/YanSH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-12 06:15:41.000000 YanSH-0.1.2/YanSH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 06:15:41.000000 YanSH-0.1.2/YanSH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 06:15:41.000000 YanSH-0.1.2/YanSH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 06:15:41.075282 YanSH-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      344 2024-04-12 06:15:39.000000 YanSH-0.1.2/setup.py
```

### Comparing `YanSH-0.1.1/LICENSE` & `YanSH-0.1.2/LICENSE`

 * *Files identical despite different names*

