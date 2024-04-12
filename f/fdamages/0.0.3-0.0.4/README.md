# Comparing `tmp/fdamages-0.0.3.tar.gz` & `tmp/fdamages-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdamages-0.0.3.tar", last modified: Fri Apr 12 09:41:32 2024, max compression
+gzip compressed data, was "fdamages-0.0.4.tar", last modified: Fri Apr 12 09:42:34 2024, max compression
```

## Comparing `fdamages-0.0.3.tar` & `fdamages-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:41:32.987291 fdamages-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      469 2024-04-12 09:41:32.987291 fdamages-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 09:41:32.987291 fdamages-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      842 2024-04-12 09:41:30.000000 fdamages-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:41:32.979776 fdamages-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 09:41:32.982775 fdamages-0.0.3/src/fdamages/
--rw-rw-rw-   0        0        0        0 2024-04-12 09:29:34.000000 fdamages-0.0.3/src/fdamages/__init__.py
--rw-rw-rw-   0        0        0     1968 2024-04-12 08:29:52.000000 fdamages-0.0.3/src/fdamages/module_fdamage.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:41:32.986292 fdamages-0.0.3/src/fdamages.egg-info/
--rw-rw-rw-   0        0        0      469 2024-04-12 09:41:32.000000 fdamages-0.0.3/src/fdamages.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-12 09:41:32.000000 fdamages-0.0.3/src/fdamages.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:41:32.000000 fdamages-0.0.3/src/fdamages.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 09:41:32.000000 fdamages-0.0.3/src/fdamages.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 09:41:32.000000 fdamages-0.0.3/src/fdamages.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.360581 fdamages-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-12 09:29:34.000000 fdamages-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      469 2024-04-12 09:42:34.360077 fdamages-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-12 09:29:34.000000 fdamages-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-12 09:42:34.360581 fdamages-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      844 2024-04-12 09:42:32.000000 fdamages-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.350511 fdamages-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.354021 fdamages-0.0.4/src/fdamages/
+-rw-rw-rw-   0        0        0       41 2024-04-12 09:42:30.000000 fdamages-0.0.4/src/fdamages/__init__.py
+-rw-rw-rw-   0        0        0     1968 2024-04-12 08:29:52.000000 fdamages-0.0.4/src/fdamages/module_fdamage.py
+drwxrwxrwx   0        0        0        0 2024-04-12 09:42:34.359027 fdamages-0.0.4/src/fdamages.egg-info/
+-rw-rw-rw-   0        0        0      469 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-12 09:42:34.000000 fdamages-0.0.4/src/fdamages.egg-info/top_level.txt
```

### Comparing `fdamages-0.0.3/LICENSE` & `fdamages-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fdamages-0.0.3/setup.py` & `fdamages-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 PACKAGE_NAME = "fdamages"
 AUTHOR = "Valerio Luzzi"
 EMAIL = "valerio.luzzi@gecosistema.com"
 GITHUB = f"https://github.com/valluzzi/{PACKAGE_NAME}.git"
 DESCRIPTION = "A fdamage utility for reading damage functions"
 
 setup(
@@ -31,11 +31,12 @@
 
 
 
 
 
 
 
+
```

### Comparing `fdamages-0.0.3/src/fdamages/module_fdamage.py` & `fdamages-0.0.4/src/fdamages/module_fdamage.py`

 * *Files identical despite different names*

