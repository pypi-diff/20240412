# Comparing `tmp/betterspread-0.2.1.tar.gz` & `tmp/betterspread-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterspread-0.2.1.tar", max compression
+gzip compressed data, was "betterspread-0.2.2.tar", max compression
```

## Comparing `betterspread-0.2.1.tar` & `betterspread-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      990 2024-03-06 13:50:58.175957 betterspread-0.2.1/README.md
--rw-r--r--   0        0        0      216 2024-03-06 23:15:52.699049 betterspread-0.2.1/betterspread/__init__.py
--rw-r--r--   0        0        0     2412 2024-04-01 21:56:52.317830 betterspread-0.2.1/betterspread/cell.py
--rw-r--r--   0        0        0      419 2024-03-06 13:50:58.176278 betterspread-0.2.1/betterspread/connection.py
--rw-r--r--   0        0        0     2085 2024-04-01 21:58:03.606643 betterspread-0.2.1/betterspread/row.py
--rw-r--r--   0        0        0     1552 2024-03-06 17:46:16.681869 betterspread-0.2.1/betterspread/sheet.py
--rw-r--r--   0        0        0     1114 2024-03-06 13:50:58.176550 betterspread-0.2.1/betterspread/style.py
--rw-r--r--   0        0        0     3076 2024-04-01 22:57:34.076604 betterspread-0.2.1/betterspread/tab.py
--rw-r--r--   0        0        0      581 2024-03-06 23:15:52.702121 betterspread-0.2.1/betterspread/utils.py
--rw-r--r--   0        0        0      661 2024-04-01 22:58:01.243178 betterspread-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 betterspread-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      990 2024-03-06 13:50:58.175957 betterspread-0.2.2/README.md
+-rw-r--r--   0        0        0      216 2024-03-06 23:15:52.699049 betterspread-0.2.2/betterspread/__init__.py
+-rw-r--r--   0        0        0     2412 2024-04-01 21:56:52.317830 betterspread-0.2.2/betterspread/cell.py
+-rw-r--r--   0        0        0      419 2024-03-06 13:50:58.176278 betterspread-0.2.2/betterspread/connection.py
+-rw-r--r--   0        0        0     2085 2024-04-01 21:58:03.606643 betterspread-0.2.2/betterspread/row.py
+-rw-r--r--   0        0        0     1552 2024-03-06 17:46:16.681869 betterspread-0.2.2/betterspread/sheet.py
+-rw-r--r--   0        0        0     1114 2024-03-06 13:50:58.176550 betterspread-0.2.2/betterspread/style.py
+-rw-r--r--   0        0        0     3076 2024-04-12 05:01:16.307958 betterspread-0.2.2/betterspread/tab.py
+-rw-r--r--   0        0        0      565 2024-04-12 05:10:02.773891 betterspread-0.2.2/betterspread/utils.py
+-rw-r--r--   0        0        0      661 2024-04-12 05:10:38.840743 betterspread-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 betterspread-0.2.2/PKG-INFO
```

### Comparing `betterspread-0.2.1/README.md` & `betterspread-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/betterspread/cell.py` & `betterspread-0.2.2/betterspread/cell.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/betterspread/row.py` & `betterspread-0.2.2/betterspread/row.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/betterspread/sheet.py` & `betterspread-0.2.2/betterspread/sheet.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/betterspread/style.py` & `betterspread-0.2.2/betterspread/style.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/betterspread/tab.py` & `betterspread-0.2.2/betterspread/tab.py`

 * *Files identical despite different names*

### Comparing `betterspread-0.2.1/pyproject.toml` & `betterspread-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "betterspread"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Md Shahriyar Alam <contact@shahriyar.dev>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.urls]
 homepage = "https://github.com/shahriyardx/betterspread"
```

### Comparing `betterspread-0.2.1/PKG-INFO` & `betterspread-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterspread
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 License: MIT
 Author: Md Shahriyar Alam
 Author-email: contact@shahriyar.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

