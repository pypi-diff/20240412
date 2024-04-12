# Comparing `tmp/dbis-exc-manager-0.4.0.tar.gz` & `tmp/dbis-exc-manager-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-exc-manager-0.4.0.tar", last modified: Mon Apr  8 13:21:59 2024, max compression
+gzip compressed data, was "dbis-exc-manager-1.0.tar", last modified: Fri Apr 12 08:23:38 2024, max compression
```

## Comparing `dbis-exc-manager-0.4.0.tar` & `dbis-exc-manager-1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1315 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-06 09:26:04.000000 dbis-exc-manager-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-08 13:12:08.000000 dbis-exc-manager-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.149930 dbis-exc-manager-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1315 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      434 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      114 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-08 13:21:59.000000 dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/src/excmanager/
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/Task.py
--rw-rw-rw-   0 root         (0) root         (0)    10376 2024-04-08 13:03:55.000000 dbis-exc-manager-0.4.0/src/excmanager/Util.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/Version.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/src/excmanager/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4464 2024-04-08 13:03:55.000000 dbis-exc-manager-0.4.0/src/excmanager/scorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 13:21:59.153930 dbis-exc-manager-0.4.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1198 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_Task.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_Util.py
--rw-rw-rw-   0 root         (0) root         (0)     1832 2023-12-22 08:44:56.000000 dbis-exc-manager-0.4.0/tests/test_scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      514 2024-02-06 09:26:04.000000 dbis-exc-manager-1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-12 08:18:22.000000 dbis-exc-manager-1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:23:38.276491 dbis-exc-manager-1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1313 2024-04-12 08:23:38.000000 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      434 2024-04-12 08:23:38.000000 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 08:23:38.000000 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-12 08:23:38.000000 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-12 08:23:38.000000 dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/src/excmanager/
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/src/excmanager/Task.py
+-rw-rw-rw-   0 root         (0) root         (0)    10376 2024-04-08 13:03:55.000000 dbis-exc-manager-1.0/src/excmanager/Util.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/src/excmanager/Version.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/src/excmanager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2024-04-08 13:03:55.000000 dbis-exc-manager-1.0/src/excmanager/scorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 08:23:38.280491 dbis-exc-manager-1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/tests/test_Task.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/tests/test_Util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1832 2023-12-22 08:44:56.000000 dbis-exc-manager-1.0/tests/test_scorer.py
```

### Comparing `dbis-exc-manager-0.4.0/LICENSE` & `dbis-exc-manager-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/PKG-INFO` & `dbis-exc-manager-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-exc-manager
-Version: 0.4.0
+Version: 1.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-exercise-manager
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-exc-manager-0.4.0/README.md` & `dbis-exc-manager-1.0/README.md`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/pyproject.toml` & `dbis-exc-manager-1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-exc-manager"
-version = "0.4.0"
+version = "1.0"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "DBIS i5 RWTH Aachen", email = "dbis-vl@dbis.rwth-aachen.de " },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-exc-manager-0.4.0/src/dbis_exc_manager.egg-info/PKG-INFO` & `dbis-exc-manager-1.0/src/dbis_exc_manager.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-exc-manager
-Version: 0.4.0
+Version: 1.0
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: DBIS i5 RWTH Aachen <dbis-vl@dbis.rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis/dbis-exercise-manager
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-exc-manager-0.4.0/src/excmanager/Task.py` & `dbis-exc-manager-1.0/src/excmanager/Task.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/src/excmanager/Util.py` & `dbis-exc-manager-1.0/src/excmanager/Util.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/src/excmanager/scorer.py` & `dbis-exc-manager-1.0/src/excmanager/scorer.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/tests/test_Task.py` & `dbis-exc-manager-1.0/tests/test_Task.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/tests/test_Util.py` & `dbis-exc-manager-1.0/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `dbis-exc-manager-0.4.0/tests/test_scorer.py` & `dbis-exc-manager-1.0/tests/test_scorer.py`

 * *Files identical despite different names*

