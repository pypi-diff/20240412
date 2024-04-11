# Comparing `tmp/dpd_lib-0.0.9.tar.gz` & `tmp/dpd_lib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpd_lib-0.0.9.tar", last modified: Wed Apr 10 18:03:28 2024, max compression
+gzip compressed data, was "dpd_lib-0.1.0.tar", last modified: Thu Apr 11 22:22:48 2024, max compression
```

## Comparing `dpd_lib-0.0.9.tar` & `dpd_lib-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/PYPI.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/dpd_lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 18:03:21.000000 dpd_lib-0.0.9/dpd_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/dpd_lib/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 18:03:21.000000 dpd_lib-0.0.9/dpd_lib/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/dpd_lib/client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8426 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/dpd_lib/client/influx.py
--rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/dpd_lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/dpd_lib/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/dpd_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2101 2024-04-10 18:03:28.000000 dpd_lib-0.0.9/dpd_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      313 2024-04-10 18:03:28.000000 dpd_lib-0.0.9/dpd_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 18:03:28.000000 dpd_lib-0.0.9/dpd_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2024-04-10 18:03:28.000000 dpd_lib-0.0.9/dpd_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-10 18:03:28.000000 dpd_lib-0.0.9/dpd_lib.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-10 18:02:48.000000 dpd_lib-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 18:03:28.488862 dpd_lib-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:22:48.190838 dpd_lib-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-11 22:22:48.190838 dpd_lib-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/PYPI.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:22:48.186838 dpd_lib-0.1.0/dpd_lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 22:22:39.000000 dpd_lib-0.1.0/dpd_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:22:48.186838 dpd_lib-0.1.0/dpd_lib/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 22:22:39.000000 dpd_lib-0.1.0/dpd_lib/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/dpd_lib/client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8426 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/dpd_lib/client/influx.py
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/dpd_lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/dpd_lib/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 22:22:48.186838 dpd_lib-0.1.0/dpd_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-04-11 22:22:48.000000 dpd_lib-0.1.0/dpd_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-11 22:22:48.000000 dpd_lib-0.1.0/dpd_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 22:22:48.000000 dpd_lib-0.1.0/dpd_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2024-04-11 22:22:48.000000 dpd_lib-0.1.0/dpd_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 22:22:48.000000 dpd_lib-0.1.0/dpd_lib.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      979 2024-04-11 22:22:00.000000 dpd_lib-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 22:22:48.190838 dpd_lib-0.1.0/setup.cfg
```

### Comparing `dpd_lib-0.0.9/PKG-INFO` & `dpd_lib-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.9/PYPI.md` & `dpd_lib-0.1.0/PYPI.md`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.9/dpd_lib/client/exceptions.py` & `dpd_lib-0.1.0/dpd_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.9/dpd_lib/client/influx.py` & `dpd_lib-0.1.0/dpd_lib/client/influx.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.9/dpd_lib/config.py` & `dpd_lib-0.1.0/dpd_lib/config.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.9/dpd_lib/models.py` & `dpd_lib-0.1.0/dpd_lib/models.py`

 * *Files identical despite different names*

### Comparing `dpd_lib-0.0.9/dpd_lib.egg-info/PKG-INFO` & `dpd_lib-0.1.0/dpd_lib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpd_lib
-Version: 0.0.9
+Version: 0.1.0
 Summary: A package for interacting with the USGS influx db
 Author-email: Noah Harper <nharper@usgs.gov>
 Project-URL: Homepage, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database
 Project-URL: Issues, https://code.usgs.gov/cvo-realtime-seismic/derived-project-database/-/issues
 Keywords: infrasound,seismic,usgs,volcanos
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `dpd_lib-0.0.9/pyproject.toml` & `dpd_lib-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=66.1.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpd_lib"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Noah Harper", email="nharper@usgs.gov" },
 ]
 description = "A package for interacting with the USGS influx db"
 readme = "PYPI.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
```

