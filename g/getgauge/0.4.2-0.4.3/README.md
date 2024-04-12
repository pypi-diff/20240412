# Comparing `tmp/getgauge-0.4.2.tar.gz` & `tmp/getgauge-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getgauge-0.4.2.tar", last modified: Tue Feb 13 14:05:22 2024, max compression
+gzip compressed data, was "getgauge-0.4.3.tar", last modified: Fri Apr 12 04:58:44 2024, max compression
```

## Comparing `getgauge-0.4.2.tar` & `getgauge-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:05:22.782908 getgauge-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-13 14:05:11.486860 getgauge-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-13 14:05:22.782908 getgauge-0.4.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:05:22.782908 getgauge-0.4.2/getgauge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/impl_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 14:05:22.782908 getgauge-0.4.2/getgauge/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/messages/messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/messages/services_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    60546 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/messages/services_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/messages/spec_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/refactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/static_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-13 14:05:11.486860 getgauge-0.4.2/getgauge/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-13 14:05:22.482906 getgauge-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:44.188920 getgauge-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 04:58:30.000000 getgauge-0.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 04:58:30.000000 getgauge-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-12 04:58:44.188920 getgauge-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-12 04:58:30.000000 getgauge-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:44.184920 getgauge-0.4.3/getgauge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/impl_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:44.184920 getgauge-0.4.3/getgauge/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/messages/messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/messages/services_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60546 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/messages/services_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17111 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/messages/spec_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/refactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8807 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/static_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-12 04:58:30.000000 getgauge-0.4.3/getgauge/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:44.188920 getgauge-0.4.3/getgauge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-12 04:58:44.000000 getgauge-0.4.3/getgauge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 04:58:44.000000 getgauge-0.4.3/getgauge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 04:58:44.000000 getgauge-0.4.3/getgauge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-12 04:58:44.000000 getgauge-0.4.3/getgauge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 04:58:44.000000 getgauge-0.4.3/getgauge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 04:58:44.188920 getgauge-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 04:58:43.000000 getgauge-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 04:58:44.188920 getgauge-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    21196 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29360 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18936 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_static_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-12 04:58:30.000000 getgauge-0.4.3/tests/test_validate.py
```

### Comparing `getgauge-0.4.2/LICENSE.txt` & `getgauge-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/executor.py` & `getgauge-0.4.3/getgauge/executor.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/handlers.py` & `getgauge-0.4.3/getgauge/handlers.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/impl_loader.py` & `getgauge-0.4.3/getgauge/impl_loader.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/messages/messages_pb2.py` & `getgauge-0.4.3/getgauge/messages/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/messages/services_pb2.py` & `getgauge-0.4.3/getgauge/messages/services_pb2.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/messages/services_pb2_grpc.py` & `getgauge-0.4.3/getgauge/messages/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/messages/spec_pb2.py` & `getgauge-0.4.3/getgauge/messages/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/parser.py` & `getgauge-0.4.3/getgauge/parser.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/processor.py` & `getgauge-0.4.3/getgauge/processor.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/python.py` & `getgauge-0.4.3/getgauge/python.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/refactor.py` & `getgauge-0.4.3/getgauge/refactor.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/registry.py` & `getgauge-0.4.3/getgauge/registry.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/static_loader.py` & `getgauge-0.4.3/getgauge/static_loader.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/util.py` & `getgauge-0.4.3/getgauge/util.py`

 * *Files identical despite different names*

### Comparing `getgauge-0.4.2/getgauge/validator.py` & `getgauge-0.4.3/getgauge/validator.py`

 * *Files identical despite different names*

