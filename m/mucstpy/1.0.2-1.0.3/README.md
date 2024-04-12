# Comparing `tmp/mucstpy-1.0.2.tar.gz` & `tmp/mucstpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mucstpy-1.0.2.tar", last modified: Fri Apr 12 02:45:30 2024, max compression
+gzip compressed data, was "mucstpy-1.0.3.tar", last modified: Fri Apr 12 03:09:54 2024, max compression
```

## Comparing `mucstpy-1.0.2.tar` & `mucstpy-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 02:45:30.082616 mucstpy-1.0.2/
--rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      202 2024-04-12 02:45:30.081614 mucstpy-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.2/README.md
--rw-rw-rw-   0        0        0      916 2024-04-12 02:42:43.000000 mucstpy-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 02:45:30.082616 mucstpy-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 02:45:30.062067 mucstpy-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 02:45:30.076780 mucstpy-1.0.2/src/mucstpy/
--rw-rw-rw-   0        0        0     5199 2024-04-11 19:32:18.000000 mucstpy-1.0.2/src/mucstpy/MuCST.py
--rw-rw-rw-   0        0        0      142 2024-04-12 02:43:00.000000 mucstpy-1.0.2/src/mucstpy/__init__.py
--rw-rw-rw-   0        0        0     7947 2024-04-11 19:34:32.000000 mucstpy-1.0.2/src/mucstpy/image_feature.py
--rw-rw-rw-   0        0        0     2802 2024-03-30 05:57:39.000000 mucstpy-1.0.2/src/mucstpy/loss.py
--rw-rw-rw-   0        0        0    11501 2024-04-11 11:34:35.000000 mucstpy-1.0.2/src/mucstpy/model.py
--rw-rw-rw-   0        0        0    23997 2024-04-11 11:50:52.000000 mucstpy-1.0.2/src/mucstpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 02:45:30.081110 mucstpy-1.0.2/src/mucstpy.egg-info/
--rw-rw-rw-   0        0        0      202 2024-04-12 02:45:30.000000 mucstpy-1.0.2/src/mucstpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-04-12 02:45:30.000000 mucstpy-1.0.2/src/mucstpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 02:45:30.000000 mucstpy-1.0.2/src/mucstpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 02:45:30.000000 mucstpy-1.0.2/src/mucstpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 03:09:54.004595 mucstpy-1.0.3/
+-rw-rw-rw-   0        0        0     1066 2024-04-11 19:39:05.000000 mucstpy-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4209 2024-04-12 03:09:54.004091 mucstpy-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3472 2024-04-12 02:44:56.000000 mucstpy-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 03:09:54.003586 mucstpy-1.0.3/mucstpy.egg-info/
+-rw-rw-rw-   0        0        0     4209 2024-04-12 03:09:53.000000 mucstpy-1.0.3/mucstpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-12 03:09:53.000000 mucstpy-1.0.3/mucstpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       66 2024-04-12 03:09:53.000000 mucstpy-1.0.3/mucstpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2024-04-12 03:09:53.000000 mucstpy-1.0.3/mucstpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 03:09:53.000000 mucstpy-1.0.3/mucstpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      980 2024-04-12 03:09:30.000000 mucstpy-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 03:09:54.004595 mucstpy-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      991 2024-04-12 03:04:31.000000 mucstpy-1.0.3/setup.py
```

### Comparing `mucstpy-1.0.2/LICENSE` & `mucstpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mucstpy-1.0.2/README.md` & `mucstpy-1.0.3/README.md`

 * *Files identical despite different names*

