# Comparing `tmp/ehdtd_daemon-0.1.9.tar.gz` & `tmp/ehdtd_daemon-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd_daemon-0.1.9.tar", max compression
+gzip compressed data, was "ehdtd_daemon-0.2.0.tar", max compression
```

## Comparing `ehdtd_daemon-0.1.9.tar` & `ehdtd_daemon-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.1.9/LICENSE
--rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.1.9/README.md
--rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.1.9/ehdtd_daemon/__init__.py
--rw-r--r--   0        0        0    13429 2024-04-10 07:12:22.226535 ehdtd_daemon-0.1.9/ehdtd_daemon/aux_common_functions.py
--rw-r--r--   0        0        0    10216 2024-04-11 06:35:47.089007 ehdtd_daemon-0.1.9/ehdtd_daemon/bin/ehdtd_daemon.py
--rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.1.9/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
--rw-r--r--   0        0        0      751 2024-04-11 05:54:12.799790 ehdtd_daemon-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 ehdtd_daemon-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1105 2024-03-14 00:36:27.021823 ehdtd_daemon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3247 2024-04-05 07:59:22.246560 ehdtd_daemon-0.2.0/README.md
+-rw-r--r--   0        0        0      909 2024-03-25 01:56:22.544500 ehdtd_daemon-0.2.0/ehdtd_daemon/__init__.py
+-rw-r--r--   0        0        0    13429 2024-04-10 07:12:22.226535 ehdtd_daemon-0.2.0/ehdtd_daemon/aux_common_functions.py
+-rw-r--r--   0        0        0    10216 2024-04-11 06:35:47.089007 ehdtd_daemon-0.2.0/ehdtd_daemon/bin/ehdtd_daemon.py
+-rw-r--r--   0        0        0      589 2024-04-05 07:45:24.312229 ehdtd_daemon-0.2.0/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml
+-rw-r--r--   0        0        0      751 2024-04-12 13:38:40.519101 ehdtd_daemon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 ehdtd_daemon-0.2.0/PKG-INFO
```

### Comparing `ehdtd_daemon-0.1.9/LICENSE` & `ehdtd_daemon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/README.md` & `ehdtd_daemon-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/ehdtd_daemon/__init__.py` & `ehdtd_daemon-0.2.0/ehdtd_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/ehdtd_daemon/aux_common_functions.py` & `ehdtd_daemon-0.2.0/ehdtd_daemon/aux_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/ehdtd_daemon/bin/ehdtd_daemon.py` & `ehdtd_daemon-0.2.0/ehdtd_daemon/bin/ehdtd_daemon.py`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml` & `ehdtd_daemon-0.2.0/etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml`

 * *Files identical despite different names*

### Comparing `ehdtd_daemon-0.1.9/pyproject.toml` & `ehdtd_daemon-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ehdtd-daemon"
-version = "0.1.9"
+version = "0.2.0"
 description = "Daemon script for ehdtd package"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/rmalvarezkai/ehdtd_daemon"
 include = ["etc/ehdtd-daemon/ehdtd-daemon-config-sample.yaml"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-ehdtd = "^0.1.1"
 pyyaml = "^6.0.1"
 importlib = "^1.0.4"
 logging = "^0.4.9.6"
 psycopg2-binary = "^2.9.9"
 pymysql = "^1.1.0"
+ehdtd = "^0.2.0"
 
 [tool.poetry.scripts]
 ehdtd_daemon = 'ehdtd_daemon.bin.ehdtd_daemon:main'
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1.0"
 pytest = "^8.1.1"
```

### Comparing `ehdtd_daemon-0.1.9/PKG-INFO` & `ehdtd_daemon-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ehdtd-daemon
-Version: 0.1.9
+Version: 0.2.0
 Summary: Daemon script for ehdtd package
 Home-page: https://github.com/rmalvarezkai/ehdtd_daemon
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: ehdtd (>=0.1.1,<0.2.0)
+Requires-Dist: ehdtd (>=0.2.0,<0.3.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: logging (>=0.4.9.6,<0.5.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
```

