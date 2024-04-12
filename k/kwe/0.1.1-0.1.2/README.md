# Comparing `tmp/kwe-0.1.1.tar.gz` & `tmp/kwe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwe-0.1.1.tar", max compression
+gzip compressed data, was "kwe-0.1.2.tar", max compression
```

## Comparing `kwe-0.1.1.tar` & `kwe-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2534 2024-04-12 01:33:47.000000 kwe-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-12 00:30:45.000000 kwe-0.1.1/kwe/__init__.py
--rw-r--r--   0        0        0      900 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/base.py
--rw-r--r--   0        0        0      186 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/constant.py
--rw-r--r--   0        0        0     3351 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/eda.py
--rw-r--r--   0        0        0      420 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/__init__.py
--rw-r--r--   0        0        0     3619 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/graph.py
--rw-r--r--   0        0        0     4261 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/nn.py
--rw-r--r--   0        0        0     3919 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/models/statistics.py
--rw-r--r--   0        0        0     1443 2024-04-12 01:15:54.000000 kwe-0.1.1/kwe/process.py
--rw-r--r--   0        0        0      340 2024-04-12 01:54:48.130098 kwe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3079 1970-01-01 00:00:00.000000 kwe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2534 2024-04-12 01:33:47.000000 kwe-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 00:30:45.000000 kwe-0.1.2/kwe/__init__.py
+-rw-r--r--   0        0        0      900 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/base.py
+-rw-r--r--   0        0        0      186 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/constant.py
+-rw-r--r--   0        0        0     3351 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/eda.py
+-rw-r--r--   0        0        0      420 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/models/__init__.py
+-rw-r--r--   0        0        0     3619 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/models/graph.py
+-rw-r--r--   0        0        0     4261 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/models/nn.py
+-rw-r--r--   0        0        0     3919 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/models/statistics.py
+-rw-r--r--   0        0        0     1443 2024-04-12 01:15:54.000000 kwe-0.1.2/kwe/process.py
+-rw-r--r--   0        0        0      358 2024-04-12 02:55:56.650419 kwe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3118 1970-01-01 00:00:00.000000 kwe-0.1.2/PKG-INFO
```

### Comparing `kwe-0.1.1/README.md` & `kwe-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/base.py` & `kwe-0.1.2/kwe/base.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/eda.py` & `kwe-0.1.2/kwe/eda.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/models/graph.py` & `kwe-0.1.2/kwe/models/graph.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/models/nn.py` & `kwe-0.1.2/kwe/models/nn.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/models/statistics.py` & `kwe-0.1.2/kwe/models/statistics.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/kwe/process.py` & `kwe-0.1.2/kwe/process.py`

 * *Files identical despite different names*

### Comparing `kwe-0.1.1/PKG-INFO` & `kwe-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kwe
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: 윤성민
 Author-email: meetingstranger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datasets (>=2.18.0,<3.0.0)
+Requires-Dist: gensim (>=4.3.2,<5.0.0)
 Requires-Dist: keybert (>=0.8.4,<0.9.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 # KWE
```

