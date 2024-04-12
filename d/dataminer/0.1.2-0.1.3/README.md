# Comparing `tmp/dataminer-0.1.2.tar.gz` & `tmp/dataminer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataminer-0.1.2.tar", last modified: Thu Apr 11 08:52:52 2024, max compression
+gzip compressed data, was "dataminer-0.1.3.tar", last modified: Fri Apr 12 03:34:49 2024, max compression
```

## Comparing `dataminer-0.1.2.tar` & `dataminer-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-11 08:51:19.000000 dataminer-0.1.2/LICENSE
--rw-r--r--   0 javaite   (1000) javaite   (1000)      520 2024-04-11 08:52:52.755700 dataminer-0.1.2/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/README.md
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.751700 dataminer-0.1.2/dataminer/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/__init__.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/dataminer/datax/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/job_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/datax/runner.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.755700 dataminer-0.1.2/dataminer/sqla/
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/__init__.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1624 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/engine_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/query_helpers.py
--rw-rw-r--   0 javaite   (1000) javaite   (1000)     1443 2024-04-11 08:51:19.000000 dataminer-0.1.2/dataminer/sqla/table_helpers.py
-drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-11 08:52:52.751700 dataminer-0.1.2/dataminer.egg-info/
--rw-r--r--   0 javaite   (1000) javaite   (1000)      520 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/PKG-INFO
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      421 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/SOURCES.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/dependency_links.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       11 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/requires.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-11 08:52:52.000000 dataminer-0.1.2/dataminer.egg-info/top_level.txt
--rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-11 08:52:52.755700 dataminer-0.1.2/setup.cfg
--rw-rw-r--   0 javaite   (1000) javaite   (1000)      705 2024-04-11 08:51:19.000000 dataminer-0.1.2/setup.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.246152 dataminer-0.1.3/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)    11357 2024-04-12 03:34:23.000000 dataminer-0.1.3/LICENSE
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-12 03:34:49.246152 dataminer-0.1.3/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/README.md
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/__init__.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer/datax/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     4302 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/job_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     3558 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/datax/runner.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.246152 dataminer-0.1.3/dataminer/sqla/
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/__init__.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1618 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/engine_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      332 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/query_helpers.py
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)     1443 2024-04-12 03:34:23.000000 dataminer-0.1.3/dataminer/sqla/table_helpers.py
+drwxrwxr-x   0 javaite   (1000) javaite   (1000)        0 2024-04-12 03:34:49.242152 dataminer-0.1.3/dataminer.egg-info/
+-rw-r--r--   0 javaite   (1000) javaite   (1000)      544 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/PKG-INFO
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      421 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/SOURCES.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)        1 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/dependency_links.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       20 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/requires.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       10 2024-04-12 03:34:49.000000 dataminer-0.1.3/dataminer.egg-info/top_level.txt
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)       38 2024-04-12 03:34:49.246152 dataminer-0.1.3/setup.cfg
+-rw-rw-r--   0 javaite   (1000) javaite   (1000)      725 2024-04-12 03:34:23.000000 dataminer-0.1.3/setup.py
```

### Comparing `dataminer-0.1.2/LICENSE` & `dataminer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.2/PKG-INFO` & `dataminer-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlalchemy
+Requires-Dist: oracledb
```

### Comparing `dataminer-0.1.2/dataminer/datax/job_helpers.py` & `dataminer-0.1.3/dataminer/datax/job_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.2/dataminer/datax/runner.py` & `dataminer-0.1.3/dataminer/datax/runner.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.2/dataminer/sqla/engine_helpers.py` & `dataminer-0.1.3/dataminer/sqla/engine_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from dataclasses import dataclass
 
-import cx_Oracle
+import oracledb
 from sqlalchemy import Engine, NullPool, create_engine
 
 
 @dataclass
 class EngineConfig:
     drivername: str
     host: str
@@ -20,20 +20,20 @@
     @staticmethod
     def create_engine(cfg: EngineConfig) -> Engine:
         _driver = cfg.drivername
         _username = cfg.username
         url = f"{cfg.drivername}://{cfg.username}:{cfg.password}@{cfg.host}:{cfg.port}/{cfg.database}"
 
         if re.search(r"oracle", _driver, re.IGNORECASE) and (
-                _username.lower() == "sys" or _username.lower() == "system"
+            _username.lower() == "sys" or _username.lower() == "system"
         ):
             return create_engine(
                 url,
                 poolclass=NullPool,
-                connect_args={"mode": cx_Oracle.SYSDBA},
+                connect_args={"mode": oracledb.SYSDBA},
             )
         else:
             return create_engine(url, poolclass=NullPool)
 
     @staticmethod
     def jdbc_from_engine(engine: Engine) -> str:
         dialect = engine.dialect.name
```

### Comparing `dataminer-0.1.2/dataminer/sqla/table_helpers.py` & `dataminer-0.1.3/dataminer/sqla/table_helpers.py`

 * *Files identical despite different names*

### Comparing `dataminer-0.1.2/dataminer.egg-info/PKG-INFO` & `dataminer-0.1.3/dataminer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: dataminer
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of data processing tools.
 Home-page: https://gitee.com/javaite_code/dataminer.git
 Author: javaite
 Author-email: javaite@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlalchemy
+Requires-Dist: oracledb
```

### Comparing `dataminer-0.1.2/setup.py` & `dataminer-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataminer',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     install_requires=[
         'sqlalchemy',
+        'oracledb',
     ],
     author='javaite',
     author_email='javaite@126.com',
     description='A set of data processing tools.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://gitee.com/javaite_code/dataminer.git',
```

