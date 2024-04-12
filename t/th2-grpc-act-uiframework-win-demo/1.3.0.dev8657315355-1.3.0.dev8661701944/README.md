# Comparing `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355.tar.gz` & `tmp/th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355.tar", last modified: Fri Apr 12 05:15:55 2024, max compression
+gzip compressed data, was "dist/th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944.tar", last modified: Fri Apr 12 12:04:38 2024, max compression
```

## Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355.tar` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 05:14:29.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 05:14:29.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-12 05:14:29.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 05:15:30.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-12 05:14:29.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 05:15:55.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 05:15:54.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-12 12:03:17.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 12:03:18.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-12 12:03:17.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-12 12:04:14.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-12 12:03:17.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-12 12:04:38.000000 th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/top_level.txt
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/PKG-INFO` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2_grpc_act_uiframework_win_demo
-Version: 1.3.0.dev8657315355
+Version: 1.3.0.dev8661701944
 Summary: th2_grpc_act_uiframework_win_demo
 Home-page: https://github.com/th2-net/th2-grpc-act-uiframework-win-demo
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: ## th2-grpc-act-ui-framework-demo (1.3.0)
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/setup.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/u_i_framework_act_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo/uiframework_win_demo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: th2-grpc-act-uiframework-win-demo
-Version: 1.3.0.dev8657315355
+Version: 1.3.0.dev8661701944
 Summary: th2_grpc_act_uiframework_win_demo
 Home-page: https://github.com/th2-net/th2-grpc-act-uiframework-win-demo
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: ## th2-grpc-act-ui-framework-demo (1.3.0)
```

### Comparing `th2_grpc_act_uiframework_win_demo-1.3.0.dev8657315355/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt` & `th2_grpc_act_uiframework_win_demo-1.3.0.dev8661701944/th2_grpc_act_uiframework_win_demo.egg-info/SOURCES.txt`

 * *Files identical despite different names*
