# Comparing `tmp/polymatheia-1.0.7.tar.gz` & `tmp/polymatheia-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatheia-1.0.7.tar", max compression
+gzip compressed data, was "polymatheia-1.0.8.tar", max compression
```

## Comparing `polymatheia-1.0.7.tar` & `polymatheia-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-01-12 09:16:02.452213 polymatheia-1.0.7/LICENSE.md
--rw-r--r--   0        0        0      858 2024-01-12 09:16:02.452213 polymatheia-1.0.7/README.md
--rw-r--r--   0        0        0     1227 2024-01-12 09:16:02.456213 polymatheia-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      264 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/__init__.py
--rw-r--r--   0        0        0    12729 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/data/__init__.py
--rw-r--r--   0        0        0    18076 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/data/reader.py
--rw-r--r--   0        0        0     9480 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/data/writer.py
--rw-r--r--   0        0        0     9098 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/filter.py
--rw-r--r--   0        0        0     8135 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/transform.py
--rw-r--r--   0        0        0      887 2024-01-12 09:16:02.456213 polymatheia-1.0.7/src/polymatheia/util.py
--rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 polymatheia-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-12 11:38:11.856775 polymatheia-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0      858 2024-04-12 11:38:11.856775 polymatheia-1.0.8/README.md
+-rw-r--r--   0        0        0     1227 2024-04-12 11:38:11.860776 polymatheia-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      264 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/__init__.py
+-rw-r--r--   0        0        0    12729 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/data/__init__.py
+-rw-r--r--   0        0        0    18076 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/data/reader.py
+-rw-r--r--   0        0        0     9480 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/data/writer.py
+-rw-r--r--   0        0        0     9098 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/filter.py
+-rw-r--r--   0        0        0     8135 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/transform.py
+-rw-r--r--   0        0        0      887 2024-04-12 11:38:11.860776 polymatheia-1.0.8/src/polymatheia/util.py
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 polymatheia-1.0.8/PKG-INFO
```

### Comparing `polymatheia-1.0.7/LICENSE.md` & `polymatheia-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/README.md` & `polymatheia-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/pyproject.toml` & `polymatheia-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polymatheia"
-version = "1.0.7"
+version = "1.0.8"
 description = "A python library to support digital archive metadata use"
 authors = ["Mark Hall <mark.hall@work.room3b.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://polymatheia.readthedocs.io"
 repository = "https://github.com/scmmmh/polymatheia"
 classifiers = [
```

### Comparing `polymatheia-1.0.7/src/polymatheia/data/__init__.py` & `polymatheia-1.0.8/src/polymatheia/data/__init__.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/src/polymatheia/data/reader.py` & `polymatheia-1.0.8/src/polymatheia/data/reader.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/src/polymatheia/data/writer.py` & `polymatheia-1.0.8/src/polymatheia/data/writer.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/src/polymatheia/filter.py` & `polymatheia-1.0.8/src/polymatheia/filter.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/src/polymatheia/transform.py` & `polymatheia-1.0.8/src/polymatheia/transform.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/src/polymatheia/util.py` & `polymatheia-1.0.8/src/polymatheia/util.py`

 * *Files identical despite different names*

### Comparing `polymatheia-1.0.7/PKG-INFO` & `polymatheia-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polymatheia
-Version: 1.0.7
+Version: 1.0.8
 Summary: A python library to support digital archive metadata use
 Home-page: https://polymatheia.readthedocs.io
 License: MIT
 Author: Mark Hall
 Author-email: mark.hall@work.room3b.eu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

