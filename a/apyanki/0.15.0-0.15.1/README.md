# Comparing `tmp/apyanki-0.15.0.tar.gz` & `tmp/apyanki-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.0.tar", max compression
+gzip compressed data, was "apyanki-0.15.1.tar", max compression
```

## Comparing `apyanki-0.15.0.tar` & `apyanki-0.15.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.0/LICENSE.md
--rw-r--r--   0        0        0    11048 2024-04-11 17:16:35.753889 apyanki-0.15.0/README.md
--rw-r--r--   0        0        0     1550 2024-04-11 17:17:26.407557 apyanki-0.15.0/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.0/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16898 2024-04-11 17:01:51.868060 apyanki-0.15.0/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.0/src/apyanki/cards.py
--rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.0/src/apyanki/cli.py
--rw-r--r--   0        0        0     2021 2024-03-29 14:35:15.207533 apyanki-0.15.0/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.0/src/apyanki/console.py
--rw-r--r--   0        0        0     9117 2024-04-11 17:03:47.808825 apyanki-0.15.0/src/apyanki/fields.py
--rw-r--r--   0        0        0    23307 2024-04-11 17:08:37.727403 apyanki-0.15.0/src/apyanki/note.py
--rw-r--r--   0        0        0     2987 2024-04-11 17:11:39.668604 apyanki-0.15.0/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12006 1970-01-01 00:00:00.000000 apyanki-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-04-08 08:17:45.340180 apyanki-0.15.1/LICENSE.md
+-rw-r--r--   0        0        0    11048 2024-04-11 20:43:59.140388 apyanki-0.15.1/README.md
+-rw-r--r--   0        0        0     1550 2024-04-12 13:01:26.090626 apyanki-0.15.1/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16898 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14640 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2021 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-04-11 20:43:59.140388 apyanki-0.15.1/src/apyanki/console.py
+-rw-r--r--   0        0        0     9117 2024-04-11 20:43:59.143721 apyanki-0.15.1/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23307 2024-04-11 20:43:59.143721 apyanki-0.15.1/src/apyanki/note.py
+-rw-r--r--   0        0        0     2987 2024-04-11 20:43:59.143721 apyanki-0.15.1/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12006 1970-01-01 00:00:00.000000 apyanki-0.15.1/PKG-INFO
```

### Comparing `apyanki-0.15.0/LICENSE.md` & `apyanki-0.15.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/README.md` & `apyanki-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/pyproject.toml` & `apyanki-0.15.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.0"
+version = "0.15.1"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Environment :: Console",
 ]
 
 [project.urls]
-Homepage = "https://github.com/lervag/apy"
-Issues = "https://github.com/lervag/apy/issues"
+homepage = "https://github.com/lervag/apy"
+issues = "https://github.com/lervag/apy/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.2"
 click = "^8.1.3"
 markdown = "^3.4.3"
 readchar = "^4.0.5"
```

### Comparing `apyanki-0.15.0/src/apyanki/anki.py` & `apyanki-0.15.1/src/apyanki/anki.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/cards.py` & `apyanki-0.15.1/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/cli.py` & `apyanki-0.15.1/src/apyanki/cli.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/config.py` & `apyanki-0.15.1/src/apyanki/config.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/console.py` & `apyanki-0.15.1/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/fields.py` & `apyanki-0.15.1/src/apyanki/fields.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/note.py` & `apyanki-0.15.1/src/apyanki/note.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/src/apyanki/utilities.py` & `apyanki-0.15.1/src/apyanki/utilities.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.0/PKG-INFO` & `apyanki-0.15.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.0
+Version: 0.15.1
 Summary: CLI script for interacting with local Anki collection
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

