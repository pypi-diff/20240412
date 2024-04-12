# Comparing `tmp/THREEDYARD-0.1.tar.gz` & `tmp/THREEDYARD-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THREEDYARD-0.1.tar", last modified: Wed Apr  3 10:26:33 2024, max compression
+gzip compressed data, was "THREEDYARD-0.2.tar", last modified: Fri Apr 12 11:12:35 2024, max compression
```

## Comparing `THREEDYARD-0.1.tar` & `THREEDYARD-0.2.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:26:33.888947 THREEDYARD-0.1/
--rw-rw-rw-   0        0        0     1078 2024-04-03 10:10:04.000000 THREEDYARD-0.1/LICENSE
--rw-rw-rw-   0        0        0      205 2024-04-03 10:26:33.888947 THREEDYARD-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      141 2024-04-03 10:18:51.000000 THREEDYARD-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 10:26:33.879804 THREEDYARD-0.1/THREEDYARD/
--rw-rw-rw-   0        0        0     5384 2024-04-03 10:18:02.000000 THREEDYARD-0.1/THREEDYARD/THREEDYARD.py
--rw-rw-rw-   0        0        0        0 2024-04-03 07:10:49.000000 THREEDYARD-0.1/THREEDYARD/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:26:33.887437 THREEDYARD-0.1/THREEDYARD.egg-info/
--rw-rw-rw-   0        0        0      205 2024-04-03 10:26:33.000000 THREEDYARD-0.1/THREEDYARD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-03 10:26:33.000000 THREEDYARD-0.1/THREEDYARD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:26:33.000000 THREEDYARD-0.1/THREEDYARD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 10:26:33.000000 THREEDYARD-0.1/THREEDYARD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 10:26:33.888947 THREEDYARD-0.1/setup.cfg
--rw-rw-rw-   0        0        0      276 2024-04-03 10:15:58.000000 THREEDYARD-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 11:12:35.198849 THREEDYARD-0.2/
+-rw-rw-rw-   0        0        0     1078 2024-04-03 10:10:04.000000 THREEDYARD-0.2/LICENSE
+-rw-rw-rw-   0        0        0      664 2024-04-12 11:12:35.197850 THREEDYARD-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-03 10:18:51.000000 THREEDYARD-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 11:12:35.196852 THREEDYARD-0.2/THREEDYARD.egg-info/
+-rw-rw-rw-   0        0        0      664 2024-04-12 11:12:35.000000 THREEDYARD-0.2/THREEDYARD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-12 11:12:35.000000 THREEDYARD-0.2/THREEDYARD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:12:35.000000 THREEDYARD-0.2/THREEDYARD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-12 11:12:35.000000 THREEDYARD-0.2/THREEDYARD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 11:12:35.000000 THREEDYARD-0.2/THREEDYARD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 11:12:35.198849 THREEDYARD-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      741 2024-04-12 11:06:48.000000 THREEDYARD-0.2/setup.py
```

### Comparing `THREEDYARD-0.1/LICENSE` & `THREEDYARD-0.2/LICENSE`

 * *Files identical despite different names*

