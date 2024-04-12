# Comparing `tmp/geo_parameters-0.2.3.tar.gz` & `tmp/geo_parameters-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_parameters-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geo_parameters-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geo_parameters-0.2.3.tar` & `geo_parameters-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1776 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0     3140 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/.gitignore
--rw-r--r--   0        0        0     1079 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/LICENSE
--rw-r--r--   0        0        0     3386 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/README.md
--rw-r--r--   0        0        0       91 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/environment.yml
--rw-r--r--   0        0        0       90 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/__init__.py
--rw-r--r--   0        0        0      376 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/grid.py
--rw-r--r--   0        0        0     1967 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/metaparameter.py
--rw-r--r--   0        0        0     1298 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/ocean.py
--rw-r--r--   0        0        0     1124 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/parameter_funcs.py
--rw-r--r--   0        0        0    10727 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/wave.py
--rw-r--r--   0        0        0     1388 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/geo_parameters/wind.py
--rw-r--r--   0        0        0      450 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1810 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_doc.py
--rw-r--r--   0        0        0     1020 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_funcs.py
--rw-r--r--   0        0        0      808 2024-04-11 12:24:15.103904 geo_parameters-0.2.3/tests/test_names.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1776 2024-04-11 13:01:12.681566 geo_parameters-0.2.4/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     3140 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1079 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3386 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/README.md
+-rw-r--r--   0        0        0       91 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/environment.yml
+-rw-r--r--   0        0        0       90 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/grid.py
+-rw-r--r--   0        0        0     1967 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/metaparameter.py
+-rw-r--r--   0        0        0     1298 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/ocean.py
+-rw-r--r--   0        0        0     1124 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/parameter_funcs.py
+-rw-r--r--   0        0        0    10727 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/wave.py
+-rw-r--r--   0        0        0     1388 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/geo_parameters/wind.py
+-rw-r--r--   0        0        0      450 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     1810 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/tests/test_doc.py
+-rw-r--r--   0        0        0     1020 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/tests/test_funcs.py
+-rw-r--r--   0        0        0      808 2024-04-11 13:01:12.685566 geo_parameters-0.2.4/tests/test_names.py
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 geo_parameters-0.2.4/PKG-INFO
```

### Comparing `geo_parameters-0.2.3/.github/workflows/tests.yml` & `geo_parameters-0.2.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/.gitignore` & `geo_parameters-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/LICENSE` & `geo_parameters-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/README.md` & `geo_parameters-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/geo_parameters/metaparameter.py` & `geo_parameters-0.2.4/geo_parameters/metaparameter.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/geo_parameters/ocean.py` & `geo_parameters-0.2.4/geo_parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/geo_parameters/parameter_funcs.py` & `geo_parameters-0.2.4/geo_parameters/parameter_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/geo_parameters/wave.py` & `geo_parameters-0.2.4/geo_parameters/wave.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/geo_parameters/wind.py` & `geo_parameters-0.2.4/geo_parameters/wind.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/tests/test_doc.py` & `geo_parameters-0.2.4/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/tests/test_funcs.py` & `geo_parameters-0.2.4/tests/test_funcs.py`

 * *Files identical despite different names*

### Comparing `geo_parameters-0.2.3/tests/test_names.py` & `geo_parameters-0.2.4/tests/test_names.py`

 * *Files identical despite different names*

