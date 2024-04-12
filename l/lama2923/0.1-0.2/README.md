# Comparing `tmp/lama2923-0.1.tar.gz` & `tmp/lama2923-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.1.tar", last modified: Fri Apr 12 00:06:18 2024, max compression
+gzip compressed data, was "lama2923-0.2.tar", last modified: Fri Apr 12 00:48:33 2024, max compression
```

## Comparing `lama2923-0.1.tar` & `lama2923-0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 00:06:18.019606 lama2923-0.1/
--rw-rw-rw-   0        0        0       53 2024-04-12 00:06:18.016608 lama2923-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 00:06:18.013605 lama2923-0.1/lama2923.egg-info/
--rw-rw-rw-   0        0        0       53 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 00:06:17.000000 lama2923-0.1/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 00:06:18.019606 lama2923-0.1/setup.cfg
--rw-rw-rw-   0        0        0      321 2024-04-11 23:42:36.000000 lama2923-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:48:33.504184 lama2923-0.2/
+-rw-rw-rw-   0        0        0      108 2024-04-12 00:48:33.500182 lama2923-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 00:48:33.422183 lama2923-0.2/lama2923/
+-rw-rw-rw-   0        0        0       40 2024-04-12 00:38:07.000000 lama2923-0.2/lama2923/__init__.py
+-rw-rw-rw-   0        0        0    18561 2024-04-11 04:30:42.000000 lama2923-0.2/lama2923/main.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:48:33.495180 lama2923-0.2/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      108 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 00:48:33.000000 lama2923-0.2/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 00:48:33.505184 lama2923-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      388 2024-04-12 00:47:49.000000 lama2923-0.2/setup.py
```

