# Comparing `tmp/kwe-0.1.0.tar.gz` & `tmp/kwe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwe-0.1.0.tar", max compression
+gzip compressed data, was "kwe-0.1.1.tar", max compression
```

## Comparing `kwe-0.1.0.tar` & `kwe-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,12 @@
--rw-r--r--   0        0        0      564 2024-04-12 01:15:24.225696 kwe-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-12 00:30:45.230392 kwe-0.1.0/kwe/__init__.py
--rw-r--r--   0        0        0      900 2024-04-12 01:15:54.128697 kwe-0.1.0/kwe/base.py
--rw-r--r--   0        0        0      186 2024-04-12 01:15:54.145052 kwe-0.1.0/kwe/constant.py
--rw-r--r--   0        0        0     3351 2024-04-12 01:15:54.155473 kwe-0.1.0/kwe/eda.py
--rw-r--r--   0        0        0      420 2024-04-12 01:15:54.195247 kwe-0.1.0/kwe/models/__init__.py
--rw-r--r--   0        0        0      876 2024-04-12 01:15:54.229523 kwe-0.1.0/kwe/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5339 2024-04-12 01:15:54.231119 kwe-0.1.0/kwe/models/__pycache__/graph.cpython-311.pyc
--rw-r--r--   0        0        0     8474 2024-04-12 01:15:54.237042 kwe-0.1.0/kwe/models/__pycache__/nn.cpython-311.pyc
--rw-r--r--   0        0        0     6907 2024-04-12 01:15:54.253499 kwe-0.1.0/kwe/models/__pycache__/statistics.cpython-311.pyc
--rw-r--r--   0        0        0     3619 2024-04-12 01:15:54.264159 kwe-0.1.0/kwe/models/graph.py
--rw-r--r--   0        0        0     4261 2024-04-12 01:15:54.265098 kwe-0.1.0/kwe/models/nn.py
--rw-r--r--   0        0        0     3919 2024-04-12 01:15:54.269459 kwe-0.1.0/kwe/models/statistics.py
--rw-r--r--   0        0        0     1443 2024-04-12 01:15:54.164415 kwe-0.1.0/kwe/process.py
--rw-r--r--   0        0        0      340 2024-04-12 01:15:42.244152 kwe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 kwe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2534 2024-04-12 01:33:47.000000 kwe-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 00:30:45.000000 kwe-0.1.1/kwe/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/base.py
+-rw-r--r--   0        0        0      186 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/constant.py
+-rw-r--r--   0        0        0     3351 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/eda.py
+-rw-r--r--   0        0        0      420 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/__init__.py
+-rw-r--r--   0        0        0     3619 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/graph.py
+-rw-r--r--   0        0        0     4261 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/nn.py
+-rw-r--r--   0        0        0     3919 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/statistics.py
+-rw-r--r--   0        0        0     1443 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/process.py
+-rw-r--r--   0        0        0      340 2024-04-12 01:54:48.130098 kwe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3079 1970-01-01 00:00:00.000000 kwe-0.1.1/PKG-INFO
```

### Comparing `kwe-0.1.0/kwe/base.py` & `kwe-0.1.1/kwe/base.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.0/kwe/eda.py` & `kwe-0.1.1/kwe/eda.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.0/kwe/models/graph.py` & `kwe-0.1.1/kwe/models/graph.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.0/kwe/models/nn.py` & `kwe-0.1.1/kwe/models/nn.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.0/kwe/models/statistics.py` & `kwe-0.1.1/kwe/models/statistics.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.0/kwe/process.py` & `kwe-0.1.1/kwe/process.py`

 * *Files identical despite different names*

