# Comparing `tmp/core-cdc-1.0.4.tar.gz` & `tmp/core-cdc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-cdc-1.0.4.tar", last modified: Sat Mar 30 19:09:36 2024, max compression
+gzip compressed data, was "core-cdc-1.0.5.tar", last modified: Fri Apr 12 03:04:57 2024, max compression
```

## Comparing `core-cdc-1.0.4.tar` & `core-cdc-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 19:09:36.675573 core-cdc-1.0.4/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2024-03-30 19:09:21.000000 core-cdc-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3122 2024-03-30 19:09:36.674573 core-cdc-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-03-30 19:09:21.000000 core-cdc-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 19:09:36.669573 core-cdc-1.0.4/core_cdc/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4115 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 19:09:36.671573 core-cdc-1.0.4/core_cdc/processors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4265 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3727 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/mongo_stream.py
--rw-rw-rw-   0 root         (0) root         (0)     3461 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/mssql.py
--rw-rw-rw-   0 root         (0) root         (0)     4246 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/mysql_binlog.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/processors/oracle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 19:09:36.673573 core-cdc-1.0.4/core_cdc/targets/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3825 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/base.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/kinesis.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/mysql.py
--rw-rw-rw-   0 root         (0) root         (0)     2608 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/snowflake.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/sns.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2024-03-30 19:09:21.000000 core-cdc-1.0.4/core_cdc/targets/sqs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 19:09:36.673573 core-cdc-1.0.4/core_cdc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3122 2024-03-30 19:09:36.000000 core-cdc-1.0.4/core_cdc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      615 2024-03-30 19:09:36.000000 core-cdc-1.0.4/core_cdc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 19:09:36.000000 core-cdc-1.0.4/core_cdc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      246 2024-03-30 19:09:36.000000 core-cdc-1.0.4/core_cdc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-30 19:09:36.000000 core-cdc-1.0.4/core_cdc.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-30 19:09:21.000000 core-cdc-1.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-30 19:09:36.675573 core-cdc-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-03-30 19:09:21.000000 core-cdc-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:04:57.873224 core-cdc-1.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2024-04-12 03:04:41.000000 core-cdc-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3122 2024-04-12 03:04:57.872224 core-cdc-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-04-12 03:04:41.000000 core-cdc-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:04:57.867224 core-cdc-1.0.5/core_cdc/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4115 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:04:57.869224 core-cdc-1.0.5/core_cdc/processors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4265 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3727 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/mongo_stream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3461 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/mssql.py
+-rw-rw-rw-   0 root         (0) root         (0)     4246 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/mysql_binlog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/processors/oracle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:04:57.871224 core-cdc-1.0.5/core_cdc/targets/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3825 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/kinesis.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/mysql.py
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/snowflake.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/sns.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2024-04-12 03:04:41.000000 core-cdc-1.0.5/core_cdc/targets/sqs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:04:57.871224 core-cdc-1.0.5/core_cdc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3122 2024-04-12 03:04:57.000000 core-cdc-1.0.5/core_cdc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-12 03:04:57.000000 core-cdc-1.0.5/core_cdc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:04:57.000000 core-cdc-1.0.5/core_cdc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-12 03:04:57.000000 core-cdc-1.0.5/core_cdc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 03:04:57.000000 core-cdc-1.0.5/core_cdc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-04-12 03:04:41.000000 core-cdc-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 03:04:57.873224 core-cdc-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-04-12 03:04:41.000000 core-cdc-1.0.5/setup.py
```

### Comparing `core-cdc-1.0.4/LICENSE` & `core-cdc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/PKG-INFO` & `core-cdc-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-cdc
-Version: 1.0.4
+Version: 1.0.5
 Summary: This project/library contains the core mechanism and resources for Change Data Capture services...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-cdc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: core-mixins==1.0.4
 Requires-Dist: core-tests==1.0.3
-Requires-Dist: core-aws==1.0.1
+Requires-Dist: core-aws==1.0.2
 Requires-Dist: core-db==2.0.2
 Provides-Extra: all
 Requires-Dist: core-db[all]==2.0.2; extra == "all"
 Requires-Dist: mysql-replication==1.0.7; extra == "all"
 Provides-Extra: mongo
 Requires-Dist: core-db[mongo]==2.0.2; extra == "mongo"
 Provides-Extra: mysql
```

### Comparing `core-cdc-1.0.4/README.md` & `core-cdc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/base.py` & `core-cdc-1.0.5/core_cdc/base.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/processors/base.py` & `core-cdc-1.0.5/core_cdc/processors/base.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/processors/mongo_stream.py` & `core-cdc-1.0.5/core_cdc/processors/mongo_stream.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/processors/mssql.py` & `core-cdc-1.0.5/core_cdc/processors/mssql.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/processors/mysql_binlog.py` & `core-cdc-1.0.5/core_cdc/processors/mysql_binlog.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/processors/oracle.py` & `core-cdc-1.0.5/core_cdc/processors/oracle.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/base.py` & `core-cdc-1.0.5/core_cdc/targets/base.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/kinesis.py` & `core-cdc-1.0.5/core_cdc/targets/kinesis.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/mysql.py` & `core-cdc-1.0.5/core_cdc/targets/mysql.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/snowflake.py` & `core-cdc-1.0.5/core_cdc/targets/snowflake.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/sns.py` & `core-cdc-1.0.5/core_cdc/targets/sns.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc/targets/sqs.py` & `core-cdc-1.0.5/core_cdc/targets/sqs.py`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/core_cdc.egg-info/PKG-INFO` & `core-cdc-1.0.5/core_cdc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-cdc
-Version: 1.0.4
+Version: 1.0.5
 Summary: This project/library contains the core mechanism and resources for Change Data Capture services...
 Author-email: Alejandro Cora González <alek.cora.glez@gmail.com>
 Maintainer: Alejandro Cora González
 License: MIT
 Project-URL: Homepage, https://gitlab.com/bytecode-solutions/core/core-cdc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -14,15 +14,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: core-mixins==1.0.4
 Requires-Dist: core-tests==1.0.3
-Requires-Dist: core-aws==1.0.1
+Requires-Dist: core-aws==1.0.2
 Requires-Dist: core-db==2.0.2
 Provides-Extra: all
 Requires-Dist: core-db[all]==2.0.2; extra == "all"
 Requires-Dist: mysql-replication==1.0.7; extra == "all"
 Provides-Extra: mongo
 Requires-Dist: core-db[mongo]==2.0.2; extra == "mongo"
 Provides-Extra: mysql
```

### Comparing `core-cdc-1.0.4/core_cdc.egg-info/SOURCES.txt` & `core-cdc-1.0.5/core_cdc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core-cdc-1.0.4/pyproject.toml` & `core-cdc-1.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "core-cdc"
 description = "This project/library contains the core mechanism and resources for Change Data Capture services..."
-version = "1.0.4"
+version = "1.0.5"
 
 authors = [
     {name = "Alejandro Cora González", email = "alek.cora.glez@gmail.com"}
 ]
 
 maintainers = [
     {name = "Alejandro Cora González"}
@@ -33,15 +33,15 @@
     "Intended Audience :: Developers",
     "Topic :: Utilities"
 ]
 
 dependencies = [
     "core-mixins==1.0.4",
     "core-tests==1.0.3",
-    "core-aws==1.0.1",
+    "core-aws==1.0.2",
     "core-db==2.0.2"
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/bytecode-solutions/core/core-cdc"
 
 [project.optional-dependencies]
```

