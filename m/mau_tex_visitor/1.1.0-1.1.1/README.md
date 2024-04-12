# Comparing `tmp/mau_tex_visitor-1.1.0.tar.gz` & `tmp/mau_tex_visitor-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau_tex_visitor-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau_tex_visitor-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau_tex_visitor-1.1.0.tar` & `mau_tex_visitor-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      225 2023-11-12 21:00:28.251216 mau_tex_visitor-1.1.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-15 11:48:05.519329 mau_tex_visitor-1.1.0/LICENSE
--rw-r--r--   0        0        0      890 2023-08-15 11:56:07.028986 mau_tex_visitor-1.1.0/README.md
--rw-r--r--   0        0        0     4172 2023-11-12 18:13:02.651948 mau_tex_visitor-1.1.0/mau_tex_visitor/__init__.py
--rw-r--r--   0        0        0     1911 2023-11-12 21:00:50.243335 mau_tex_visitor-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 mau_tex_visitor-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      225 2023-11-13 17:01:37.002662 mau_tex_visitor-1.1.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-15 11:48:05.519329 mau_tex_visitor-1.1.1/LICENSE
+-rw-r--r--   0        0        0      890 2023-08-15 11:56:07.028986 mau_tex_visitor-1.1.1/README.md
+-rw-r--r--   0        0        0     4172 2024-04-12 13:51:36.449526 mau_tex_visitor-1.1.1/mau_tex_visitor/__init__.py
+-rw-r--r--   0        0        0     1933 2024-04-12 13:52:23.605909 mau_tex_visitor-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1848 1970-01-01 00:00:00.000000 mau_tex_visitor-1.1.1/PKG-INFO
```

### Comparing `mau_tex_visitor-1.1.0/LICENSE` & `mau_tex_visitor-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mau_tex_visitor-1.1.0/README.md` & `mau_tex_visitor-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mau_tex_visitor-1.1.0/mau_tex_visitor/__init__.py` & `mau_tex_visitor-1.1.1/mau_tex_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mau_tex_visitor-1.1.0/pyproject.toml` & `mau_tex_visitor-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau_tex_visitor"
-version = "1.1.0"
+version = "1.1.1"
 description = "A visitor for Mau that converts the AST into TeX"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
@@ -18,15 +18,17 @@
 "Programming Language :: Python :: 3.7",
 "Programming Language :: Python :: 3.8",
 "Programming Language :: Python :: 3.9",
 "Programming Language :: Python :: 3.10",
 "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
-dependencies = []
+dependencies = [
+"mau>=3.0.0,<4.0.0",
+]
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/Project-Mau/mau-tex-visitor"
 
 [project.optional-dependencies]
 testing = []
```

### Comparing `mau_tex_visitor-1.1.0/PKG-INFO` & `mau_tex_visitor-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau_tex_visitor
-Version: 1.1.0
+Version: 1.1.1
 Summary: A visitor for Mau that converts the AST into TeX
 Author-email: Leonardo Giordani <giordani.leonardo@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: mau>=3.0.0,<4.0.0
 Project-URL: Home, https://github.com/Project-Mau/mau-tex-visitor
 Provides-Extra: development
 Provides-Extra: testing
 
 # Mau TeX Visitor
 
 This is a plugin for the [Mau](https://github.com/Project-Mau/mau) markup language. The plugin provides the conversion from Mau source to TeX.
```

