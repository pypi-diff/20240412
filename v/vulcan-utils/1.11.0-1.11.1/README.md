# Comparing `tmp/vulcan_utils-1.11.tar.gz` & `tmp/vulcan_utils-1.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.tar", last modified: Fri Apr 12 16:57:20 2024, max compression
+gzip compressed data, was "vulcan_utils-1.11.1.tar", last modified: Fri Apr 12 17:08:51 2024, max compression
```

## Comparing `vulcan_utils-1.11.tar` & `vulcan_utils-1.11.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:57:20.836839 vulcan_utils-1.11/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 16:57:12.000000 vulcan_utils-1.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 16:57:20.836839 vulcan_utils-1.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:57:20.836839 vulcan_utils-1.11/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-12 16:57:12.000000 vulcan_utils-1.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:57:20.832839 vulcan_utils-1.11/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 16:57:12.000000 vulcan_utils-1.11/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:57:20.836839 vulcan_utils-1.11/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 16:57:12.000000 vulcan_utils-1.11/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:57:20.836839 vulcan_utils-1.11/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 16:57:20.000000 vulcan_utils-1.11/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 16:57:20.000000 vulcan_utils-1.11/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:57:20.000000 vulcan_utils-1.11/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 16:57:20.000000 vulcan_utils-1.11/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 16:57:20.000000 vulcan_utils-1.11/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:08:51.581562 vulcan_utils-1.11.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 17:08:51.581562 vulcan_utils-1.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:08:51.581562 vulcan_utils-1.11.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:08:51.577562 vulcan_utils-1.11.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8236 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:08:51.577562 vulcan_utils-1.11.1/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9286 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-12 17:08:37.000000 vulcan_utils-1.11.1/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:08:51.581562 vulcan_utils-1.11.1/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-12 17:08:51.000000 vulcan_utils-1.11.1/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 17:08:51.000000 vulcan_utils-1.11.1/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:08:51.000000 vulcan_utils-1.11.1/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 17:08:51.000000 vulcan_utils-1.11.1/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 17:08:51.000000 vulcan_utils-1.11.1/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11/LICENSE` & `vulcan_utils-1.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/PKG-INFO` & `vulcan_utils-1.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.0
+Version: 1.11.1
 Summary: A utility package Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Utils
 Vulcan Utils is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan_utils-1.11/tests/test_decorator.py` & `vulcan_utils-1.11.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/tests/test_encoder.py` & `vulcan_utils-1.11.1/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/tests/test_formatter.py` & `vulcan_utils-1.11.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/tests/test_logger.py` & `vulcan_utils-1.11.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/tests/test_printable.py` & `vulcan_utils-1.11.1/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils/decorator.py` & `vulcan_utils-1.11.1/vulcan_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils/encoder.py` & `vulcan_utils-1.11.1/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils/formatter.py` & `vulcan_utils-1.11.1/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils/logger.py` & `vulcan_utils-1.11.1/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils/printable.py` & `vulcan_utils-1.11.1/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11/vulcan_utils.egg-info/PKG-INFO` & `vulcan_utils-1.11.1/vulcan_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.11.0
+Version: 1.11.1
 Summary: A utility package Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Utils
 Vulcan Utils is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

