# Comparing `tmp/caustic.lexer-1.0.0.post1.tar.gz` & `tmp/caustic.lexer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.lexer-1.0.0.post1.tar", last modified: Fri Apr 12 20:06:15 2024, max compression
+gzip compressed data, was "caustic.lexer-1.0.1.tar", last modified: Fri Apr 12 21:13:23 2024, max compression
```

## Comparing `caustic.lexer-1.0.0.post1.tar` & `caustic.lexer-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:06:15.354023 caustic.lexer-1.0.0.post1/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.0.0.post1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     6488 2024-04-12 20:06:15.354023 caustic.lexer-1.0.0.post1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)     5550 2024-04-12 20:05:35.000000 caustic.lexer-1.0.0.post1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1000 2024-04-12 20:05:15.000000 caustic.lexer-1.0.0.post1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 20:06:15.354023 caustic.lexer-1.0.0.post1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:06:15.347356 caustic.lexer-1.0.0.post1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:06:15.347356 caustic.lexer-1.0.0.post1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:06:15.350689 caustic.lexer-1.0.0.post1/src/caustic/lexer/
--rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/basic_compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5521 2024-04-12 19:58:35.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/compiler.py
--rw-r--r--   0 shae      (1000) shae      (1000)    12964 2024-04-12 17:20:19.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/nodes.py
--rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/serialize.py
--rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.0.0.post1/src/caustic/lexer/util.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 20:06:15.354023 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     6488 2024-04-12 20:06:15.000000 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      416 2024-04-12 20:06:15.000000 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 20:06:15.000000 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 20:06:15.000000 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 20:06:15.000000 caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 21:13:23.533889 caustic.lexer-1.0.1/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.lexer-1.0.1/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     6588 2024-04-12 21:13:23.530556 caustic.lexer-1.0.1/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     5656 2024-04-12 21:04:34.000000 caustic.lexer-1.0.1/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1089 2024-04-12 21:11:51.000000 caustic.lexer-1.0.1/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-12 21:13:23.533889 caustic.lexer-1.0.1/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 21:13:23.520556 caustic.lexer-1.0.1/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 21:13:23.520556 caustic.lexer-1.0.1/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 21:13:23.530556 caustic.lexer-1.0.1/src/caustic/lexer/
+-rw-r--r--   0 shae      (1000) shae      (1000)     1676 2024-04-12 19:53:10.000000 caustic.lexer-1.0.1/src/caustic/lexer/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6676 2024-04-11 20:33:02.000000 caustic.lexer-1.0.1/src/caustic/lexer/basic_compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     5521 2024-04-12 19:58:35.000000 caustic.lexer-1.0.1/src/caustic/lexer/compiler.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1362 2024-04-11 22:20:05.000000 caustic.lexer-1.0.1/src/caustic/lexer/grammar.cag
+-rw-r--r--   0 shae      (1000) shae      (1000)    12964 2024-04-12 17:20:19.000000 caustic.lexer-1.0.1/src/caustic/lexer/nodes.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3237 2024-04-12 20:06:13.000000 caustic.lexer-1.0.1/src/caustic/lexer/precompiled_nodes.pkl
+-rw-r--r--   0 shae      (1000) shae      (1000)     2538 2024-04-12 16:47:14.000000 caustic.lexer-1.0.1/src/caustic/lexer/serialize.py
+-rw-r--r--   0 shae      (1000) shae      (1000)      666 2024-04-12 19:54:11.000000 caustic.lexer-1.0.1/src/caustic/lexer/util.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-12 21:13:23.530556 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     6588 2024-04-12 21:13:23.000000 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      486 2024-04-12 21:13:23.000000 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-12 21:13:23.000000 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-12 21:13:23.000000 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-12 21:13:23.000000 caustic.lexer-1.0.1/src/caustic.lexer.egg-info/top_level.txt
```

### Comparing `caustic.lexer-1.0.0.post1/LICENSE` & `caustic.lexer-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/PKG-INFO` & `caustic.lexer-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -188,7 +188,11 @@
 - Completely reworked compiler caching
 - Removed `$import` pragma
 - Moved `WHITESPACE_PATT` to `.util`
 - Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
 
 ### 1.0.0-1
 - Fixed an inaccuracy in README
+
+## 1.0.1
+- Added builtin `grammar.cag` to package
+- Added precompiled `precompiled_nodes.pkl` to package
```

### Comparing `caustic.lexer-1.0.0.post1/README.md` & `caustic.lexer-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -164,7 +164,11 @@
 - Completely reworked compiler caching
 - Removed `$import` pragma
 - Moved `WHITESPACE_PATT` to `.util`
 - Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
 
 ### 1.0.0-1
 - Fixed an inaccuracy in README
+
+## 1.0.1
+- Added builtin `grammar.cag` to package
+- Added precompiled `precompiled_nodes.pkl` to package
```

### Comparing `caustic.lexer-1.0.0.post1/pyproject.toml` & `caustic.lexer-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.lexer"
-version = "1.0.0-1"
+version = "1.0.1"
 dependencies = [
     "buffer-matcher >= 0.1.1",
 ]
 requires-python = ">=3.12"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Grammar compilation for Caustic"
@@ -27,7 +27,10 @@
 [project.urls]
 Homepage = "https://codeberg.org/Caustic/CausticLexer"
 Issues = "https://codeberg.org/Caustic/CausticLexer/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools.package-data]
+"caustic.lexer" = ["grammar.cag", "precompiled_nodes.pkl"]
```

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/__init__.py` & `caustic.lexer-1.0.1/src/caustic/lexer/__init__.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/basic_compiler.py` & `caustic.lexer-1.0.1/src/caustic/lexer/basic_compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/compiler.py` & `caustic.lexer-1.0.1/src/caustic/lexer/compiler.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/nodes.py` & `caustic.lexer-1.0.1/src/caustic/lexer/nodes.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/serialize.py` & `caustic.lexer-1.0.1/src/caustic/lexer/serialize.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic/lexer/util.py` & `caustic.lexer-1.0.1/src/caustic/lexer/util.py`

 * *Files identical despite different names*

### Comparing `caustic.lexer-1.0.0.post1/src/caustic.lexer.egg-info/PKG-INFO` & `caustic.lexer-1.0.1/src/caustic.lexer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.lexer
-Version: 1.0.0.post1
+Version: 1.0.1
 Summary: Grammar compilation for Caustic
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticLexer
 Project-URL: Issues, https://codeberg.org/Caustic/CausticLexer/issues
 Keywords: caustic,language,parser,lexer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -188,7 +188,11 @@
 - Completely reworked compiler caching
 - Removed `$import` pragma
 - Moved `WHITESPACE_PATT` to `.util`
 - Changed `nodes.Node.NO_RETURN` to singleton(ish) `util.NO_MATCH`
 
 ### 1.0.0-1
 - Fixed an inaccuracy in README
+
+## 1.0.1
+- Added builtin `grammar.cag` to package
+- Added precompiled `precompiled_nodes.pkl` to package
```

