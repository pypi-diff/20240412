# Comparing `tmp/dpq-0.1.1.tar.gz` & `tmp/dpq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpq-0.1.1.tar", max compression
+gzip compressed data, was "dpq-0.1.2.tar", max compression
```

## Comparing `dpq-0.1.1.tar` & `dpq-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3693 2024-04-12 07:53:08.845937 dpq-0.1.1/README.md
--rw-r--r--   0        0        0       23 2024-04-09 07:16:40.852521 dpq-0.1.1/dpq/__init__.py
--rw-r--r--   0        0        0     5420 2024-04-12 15:14:34.552495 dpq-0.1.1/dpq/dpq.py
--rw-r--r--   0        0        0      420 2024-04-12 15:18:46.396089 dpq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4234 1970-01-01 00:00:00.000000 dpq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3693 2024-04-12 07:53:08.845937 dpq-0.1.2/README.md
+-rw-r--r--   0        0        0       23 2024-04-09 07:16:40.852521 dpq-0.1.2/dpq/__init__.py
+-rw-r--r--   0        0        0     5420 2024-04-12 15:14:34.552495 dpq-0.1.2/dpq/dpq.py
+-rw-r--r--   0        0        0      428 2024-04-12 15:35:38.538565 dpq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 dpq-0.1.2/PKG-INFO
```

### Comparing `dpq-0.1.1/README.md` & `dpq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dpq-0.1.1/dpq/dpq.py` & `dpq-0.1.2/dpq/dpq.py`

 * *Files identical despite different names*

### Comparing `dpq-0.1.1/PKG-INFO` & `dpq-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: dpq
-Version: 0.1.1
+Version: 0.1.2
 Summary: dpq is an open-source python library that makes prompt-based data processing and feature engineering easy.
 License: Apache-2.0
 Author: dpq
 Author-email: dpq.code@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # dpq: data. prompt. query.
```

