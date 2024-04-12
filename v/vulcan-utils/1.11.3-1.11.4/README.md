# Comparing `tmp/vulcan_utils-1.11.3.tar.gz` & `tmp/vulcan_utils-1.11.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan_utils-1.11.3.tar", last modified: Fri Apr 12 19:17:07 2024, max compression
+gzip compressed data, was "vulcan_utils-1.11.4.tar", last modified: Fri Apr 12 20:21:44 2024, max compression
```

## Comparing `vulcan_utils-1.11.3.tar` & `vulcan_utils-1.11.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.871774 vulcan_utils-1.11.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.871774 vulcan_utils-1.11.3/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 19:16:59.000000 vulcan_utils-1.11.3/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:17:07.875774 vulcan_utils-1.11.3/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 19:17:07.000000 vulcan_utils-1.11.3/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       87 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9973 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 20:21:32.000000 vulcan_utils-1.11.4/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:21:44.236234 vulcan_utils-1.11.4/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-04-12 20:21:44.000000 vulcan_utils-1.11.4/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 20:21:44.000000 vulcan_utils-1.11.4/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:21:44.000000 vulcan_utils-1.11.4/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 20:21:44.000000 vulcan_utils-1.11.4/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 20:21:44.000000 vulcan_utils-1.11.4/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan_utils-1.11.3/LICENSE` & `vulcan_utils-1.11.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/tests/test_decorator.py` & `vulcan_utils-1.11.4/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/tests/test_encoder.py` & `vulcan_utils-1.11.4/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/tests/test_formatter.py` & `vulcan_utils-1.11.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/tests/test_logger.py` & `vulcan_utils-1.11.4/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/tests/test_printable.py` & `vulcan_utils-1.11.4/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/vulcan_utils/decorator.py` & `vulcan_utils-1.11.4/vulcan_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/vulcan_utils/encoder.py` & `vulcan_utils-1.11.4/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/vulcan_utils/formatter.py` & `vulcan_utils-1.11.4/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/vulcan_utils/logger.py` & `vulcan_utils-1.11.4/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan_utils-1.11.3/vulcan_utils/printable.py` & `vulcan_utils-1.11.4/vulcan_utils/printable.py`

 * *Files identical despite different names*

