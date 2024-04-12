# Comparing `tmp/ktianc-0.3.0.tar.gz` & `tmp/ktianc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ktianc-0.3.0.tar", max compression
+gzip compressed data, was "ktianc-0.3.1.tar", max compression
```

## Comparing `ktianc-0.3.0.tar` & `ktianc-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      463 2024-04-12 01:49:56.837756 ktianc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2633 2024-04-02 06:15:47.144933 ktianc-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-03-26 07:29:13.734004 ktianc-0.3.0/src/__init__.py
--rw-r--r--   0        0        0      436 2024-04-12 01:49:00.528066 ktianc-0.3.0/src/main.py
--rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 ktianc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      473 2024-04-12 02:14:59.421547 ktianc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2633 2024-04-02 06:15:47.144933 ktianc-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-26 07:29:13.734004 ktianc-0.3.1/src/__init__.py
+-rw-r--r--   0        0        0      436 2024-04-12 01:49:00.528066 ktianc-0.3.1/src/main.py
+-rw-r--r--   0        0        0     2930 1970-01-01 00:00:00.000000 ktianc-0.3.1/PKG-INFO
```

### Comparing `ktianc-0.3.0/README.md` & `ktianc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ktianc-0.3.0/PKG-INFO` & `ktianc-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ktianc
-Version: 0.3.0
+Version: 0.3.1
 Summary: ktianc first package
 License: MIT
 Author: ktianc
 Author-email: 2445667550@qq.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

