# Comparing `tmp/featuring-data-0.0.2.tar.gz` & `tmp/featuring-data-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featuring-data-0.0.2.tar", last modified: Tue Feb 20 01:16:06 2024, max compression
+gzip compressed data, was "featuring-data-0.2.tar", last modified: Fri Apr 12 14:15:39 2024, max compression
```

## Comparing `featuring-data-0.0.2.tar` & `featuring-data-0.2.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-02-20 01:16:06.863483 featuring-data-0.0.2/
--rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring-data-0.0.2/LICENSE
--rw-r--r--   0 dancapellupo   (501) staff       (20)      769 2024-02-20 01:16:06.863277 featuring-data-0.0.2/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)      172 2024-02-15 18:59:58.000000 featuring-data-0.0.2/README.md
--rw-r--r--   0 dancapellupo   (501) staff       (20)      694 2024-02-20 01:14:59.000000 featuring-data-0.0.2/pyproject.toml
--rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-02-20 01:16:06.863533 featuring-data-0.0.2/setup.cfg
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-02-20 01:16:06.859660 featuring-data-0.0.2/src/
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-02-20 01:16:06.863077 featuring-data-0.0.2/src/featuring_data.egg-info/
--rw-r--r--   0 dancapellupo   (501) staff       (20)      769 2024-02-20 01:16:06.000000 featuring-data-0.0.2/src/featuring_data.egg-info/PKG-INFO
--rw-r--r--   0 dancapellupo   (501) staff       (20)      427 2024-02-20 01:16:06.000000 featuring-data-0.0.2/src/featuring_data.egg-info/SOURCES.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-02-20 01:16:06.000000 featuring-data-0.0.2/src/featuring_data.egg-info/dependency_links.txt
--rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-02-20 01:16:06.000000 featuring-data-0.0.2/src/featuring_data.egg-info/top_level.txt
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-02-20 01:16:06.861081 featuring-data-0.0.2/src/featuringdata/
--rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring-data-0.0.2/src/featuringdata/__init__.py
-drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-02-20 01:16:06.862218 featuring-data-0.0.2/src/featuringdata/featuresEDA/
--rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring-data-0.0.2/src/featuringdata/featuresEDA/__init__.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     8471 2024-02-19 03:03:02.000000 featuring-data-0.0.2/src/featuringdata/featuresEDA/_create_pdf_report.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     1863 2024-02-19 23:52:10.000000 featuring-data-0.0.2/src/featuringdata/featuresEDA/_features_eda.py
--rw-r--r--   0 dancapellupo   (501) staff       (20)     2191 2024-02-19 01:54:01.000000 featuring-data-0.0.2/src/featuringdata/featuresEDA/_initial_eda_functions.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.919911 featuring-data-0.2/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     1079 2024-02-15 19:01:48.000000 featuring-data-0.2/LICENSE
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      767 2024-04-12 14:15:39.919718 featuring-data-0.2/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      172 2024-02-15 18:59:58.000000 featuring-data-0.2/README.md
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      692 2024-04-12 14:15:23.000000 featuring-data-0.2/pyproject.toml
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       38 2024-04-12 14:15:39.919953 featuring-data-0.2/setup.cfg
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.913301 featuring-data-0.2/src/
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.919502 featuring-data-0.2/src/featuring_data.egg-info/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      767 2024-04-12 14:15:39.000000 featuring-data-0.2/src/featuring_data.egg-info/PKG-INFO
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      783 2024-04-12 14:15:39.000000 featuring-data-0.2/src/featuring_data.egg-info/SOURCES.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        1 2024-04-12 14:15:39.000000 featuring-data-0.2/src/featuring_data.egg-info/dependency_links.txt
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       14 2024-04-12 14:15:39.000000 featuring-data-0.2/src/featuring_data.egg-info/top_level.txt
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.914567 featuring-data-0.2/src/featuringdata/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)        0 2024-02-19 19:41:13.000000 featuring-data-0.2/src/featuringdata/__init__.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.916012 featuring-data-0.2/src/featuringdata/featureSelector/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       79 2024-03-26 00:18:12.000000 featuring-data-0.2/src/featuringdata/featureSelector/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)      819 2024-03-15 01:12:03.000000 featuring-data-0.2/src/featuringdata/featureSelector/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    24269 2024-03-25 22:49:10.000000 featuring-data-0.2/src/featuringdata/featureSelector/_features_select.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     4018 2024-03-18 02:12:33.000000 featuring-data-0.2/src/featuringdata/featureSelector/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    11861 2024-03-26 12:16:29.000000 featuring-data-0.2/src/featuringdata/featureSelector/_recursive_fit.py
+drwxr-xr-x   0 dancapellupo   (501) staff       (20)        0 2024-04-12 14:15:39.918988 featuring-data-0.2/src/featuringdata/featuresEDA/
+-rw-r--r--   0 dancapellupo   (501) staff       (20)       68 2024-02-19 23:39:34.000000 featuring-data-0.2/src/featuringdata/featuresEDA/__init__.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    13809 2024-04-11 22:48:40.000000 featuring-data-0.2/src/featuringdata/featuresEDA/_correlation.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    16529 2024-04-12 02:28:29.000000 featuring-data-0.2/src/featuringdata/featuresEDA/_create_pdf_report.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    21667 2024-04-12 02:32:28.000000 featuring-data-0.2/src/featuringdata/featuresEDA/_features_eda.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)    10430 2024-04-12 02:14:19.000000 featuring-data-0.2/src/featuringdata/featuresEDA/_generate_plots.py
+-rw-r--r--   0 dancapellupo   (501) staff       (20)     5258 2024-03-28 02:40:38.000000 featuring-data-0.2/src/featuringdata/featuresEDA/_initial_eda_functions.py
```

### Comparing `featuring-data-0.0.2/LICENSE` & `featuring-data-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featuring-data-0.0.2/PKG-INFO` & `featuring-data-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuring-data
-Version: 0.0.2
+Version: 0.2
 Summary: This package is designed to help anyone with a new dataset get started with EDA quickly.
 Author-email: "Daniel M. Capellupo" <daniel@dmcdatascience.com>
 Project-URL: Homepage, https://github.com/dancapellupo/featuring-data
 Project-URL: Issues, https://github.com/dancapellupo/featuring-data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `featuring-data-0.0.2/pyproject.toml` & `featuring-data-0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "featuring-data"
-version = "0.0.2"
+version = "0.2"
 authors = [
     { name="Daniel M. Capellupo", email="daniel@dmcdatascience.com" },
 ]
 description = "This package is designed to help anyone with a new dataset get started with EDA quickly."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `featuring-data-0.0.2/src/featuring_data.egg-info/PKG-INFO` & `featuring-data-0.2/src/featuring_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featuring-data
-Version: 0.0.2
+Version: 0.2
 Summary: This package is designed to help anyone with a new dataset get started with EDA quickly.
 Author-email: "Daniel M. Capellupo" <daniel@dmcdatascience.com>
 Project-URL: Homepage, https://github.com/dancapellupo/featuring-data
 Project-URL: Issues, https://github.com/dancapellupo/featuring-data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

