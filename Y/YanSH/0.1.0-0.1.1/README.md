# Comparing `tmp/YanSH-0.1.0.tar.gz` & `tmp/YanSH-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YanSH-0.1.0.tar", last modified: Fri Apr 12 04:16:20 2024, max compression
+gzip compressed data, was "YanSH-0.1.1.tar", last modified: Fri Apr 12 06:00:10 2024, max compression
```

## Comparing `YanSH-0.1.0.tar` & `YanSH-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 04:16:20.632924 YanSH-0.1.0/
--rw-rw-rw-   0        0        0      243 2024-04-12 04:16:20.631912 YanSH-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-12 04:00:06.000000 YanSH-0.1.0/README.txt
-drwxrwxrwx   0        0        0        0 2024-04-12 04:16:20.631912 YanSH-0.1.0/YanSH.egg-info/
--rw-rw-rw-   0        0        0      243 2024-04-12 04:16:20.000000 YanSH-0.1.0/YanSH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2024-04-12 04:16:20.000000 YanSH-0.1.0/YanSH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 04:16:20.000000 YanSH-0.1.0/YanSH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-12 04:16:20.000000 YanSH-0.1.0/YanSH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 04:16:20.000000 YanSH-0.1.0/YanSH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 04:16:20.632924 YanSH-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      369 2024-04-12 03:49:23.000000 YanSH-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 06:00:10.873026 YanSH-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-04-12 05:09:42.000000 YanSH-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      236 2024-04-12 06:00:10.873026 YanSH-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-12 04:00:06.000000 YanSH-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 06:00:10.872012 YanSH-0.1.1/YanSH.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 06:00:10.000000 YanSH-0.1.1/YanSH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 06:00:10.873026 YanSH-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      344 2024-04-12 05:57:20.000000 YanSH-0.1.1/setup.py
```

