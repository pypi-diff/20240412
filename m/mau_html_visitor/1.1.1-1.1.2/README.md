# Comparing `tmp/mau_html_visitor-1.1.1.tar.gz` & `tmp/mau_html_visitor-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mau_html_visitor-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mau_html_visitor-1.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mau_html_visitor-1.1.1.tar` & `mau_html_visitor-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      328 2023-11-13 17:09:55.781826 mau_html_visitor-1.1.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-1.1.1/LICENSE
--rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-1.1.1/README.md
--rw-r--r--   0        0        0     6840 2023-11-13 17:09:55.781826 mau_html_visitor-1.1.1/mau_html_visitor/__init__.py
--rw-r--r--   0        0        0     1929 2023-11-13 17:09:55.781826 mau_html_visitor-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 mau_html_visitor-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      328 2023-11-13 17:09:55.781826 mau_html_visitor-1.1.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     1084 2023-08-14 21:18:34.423988 mau_html_visitor-1.1.2/LICENSE
+-rw-r--r--   0        0        0      982 2023-08-14 21:09:11.770701 mau_html_visitor-1.1.2/README.md
+-rw-r--r--   0        0        0     6840 2024-04-12 13:49:39.064573 mau_html_visitor-1.1.2/mau_html_visitor/__init__.py
+-rw-r--r--   0        0        0     1950 2024-04-12 13:52:29.413956 mau_html_visitor-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 mau_html_visitor-1.1.2/PKG-INFO
```

### Comparing `mau_html_visitor-1.1.1/LICENSE` & `mau_html_visitor-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-1.1.1/README.md` & `mau_html_visitor-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-1.1.1/mau_html_visitor/__init__.py` & `mau_html_visitor-1.1.2/mau_html_visitor/__init__.py`

 * *Files identical despite different names*

### Comparing `mau_html_visitor-1.1.1/pyproject.toml` & `mau_html_visitor-1.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mau_html_visitor"
-version = "1.1.1"
+version = "1.1.2"
 description = "A visitor for Mau that converts the AST into HTML"
 authors = [{name = "Leonardo Giordani", email = "giordani.leonardo@gmail.com"}]
 license = {file = "LICENSE"}
 classifiers = [
 "Development Status :: 5 - Production/Stable",
 "License :: OSI Approved :: MIT License",
 "Intended Audience :: Developers",
@@ -19,14 +19,15 @@
 "Programming Language :: Python :: 3.8",
 "Programming Language :: Python :: 3.9",
 "Programming Language :: Python :: 3.10",
 "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.7"
 dependencies = [
+"mau>=3.0.0,<4.0.0",
 "pygments",
 ]
 readme = "README.md"
 
 [project.urls]
 Home = "https://github.com/Project-Mau/mau-html-visitor"
```

### Comparing `mau_html_visitor-1.1.1/PKG-INFO` & `mau_html_visitor-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mau_html_visitor
-Version: 1.1.1
+Version: 1.1.2
 Summary: A visitor for Mau that converts the AST into HTML
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
 Requires-Dist: pygments
 Project-URL: Home, https://github.com/Project-Mau/mau-html-visitor
 Provides-Extra: development
 Provides-Extra: testing
 
 # Mau HTML Visitor
```

