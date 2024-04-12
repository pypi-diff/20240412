# Comparing `tmp/vale-3.3.1.0.tar.gz` & `tmp/vale-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vale-3.3.1.0.tar", last modified: Sat Mar 23 06:18:47 2024, max compression
+gzip compressed data, was "vale-3.4.1.tar", last modified: Fri Apr 12 19:42:02 2024, max compression
```

## Comparing `vale-3.3.1.0.tar` & `vale-3.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:18:47.472154 vale-3.3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-23 06:18:39.000000 vale-3.3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-23 06:18:39.000000 vale-3.3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-23 06:18:47.472154 vale-3.3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-03-23 06:18:39.000000 vale-3.3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-23 06:18:39.000000 vale-3.3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 06:18:47.472154 vale-3.3.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:18:47.472154 vale-3.3.1.0/vale/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 06:18:39.000000 vale-3.3.1.0/vale/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5083 2024-03-23 06:18:39.000000 vale-3.3.1.0/vale/main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-03-23 06:18:39.000000 vale-3.3.1.0/vale/vale_bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 06:18:47.472154 vale-3.3.1.0/vale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-23 06:18:47.000000 vale-3.3.1.0/vale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-23 06:18:47.000000 vale-3.3.1.0/vale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 06:18:47.000000 vale-3.3.1.0/vale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-23 06:18:47.000000 vale-3.3.1.0/vale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-23 06:18:47.000000 vale-3.3.1.0/vale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:42:02.619897 vale-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 19:41:55.000000 vale-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 19:41:55.000000 vale-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-12 19:42:02.619897 vale-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-12 19:41:55.000000 vale-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-12 19:41:55.000000 vale-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:42:02.619897 vale-3.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:42:02.615897 vale-3.4.1/vale/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:41:55.000000 vale-3.4.1/vale/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5083 2024-04-12 19:41:55.000000 vale-3.4.1/vale/main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      195 2024-04-12 19:41:55.000000 vale-3.4.1/vale/vale_bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:42:02.619897 vale-3.4.1/vale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-12 19:42:02.000000 vale-3.4.1/vale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 19:42:02.000000 vale-3.4.1/vale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:42:02.000000 vale-3.4.1/vale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 19:42:02.000000 vale-3.4.1/vale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 19:42:02.000000 vale-3.4.1/vale.egg-info/top_level.txt
```

### Comparing `vale-3.3.1.0/LICENSE` & `vale-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vale-3.3.1.0/PKG-INFO` & `vale-3.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 3.3.1.0
+Version: 3.4.1.0
 Summary: Install and use Vale (grammar & style check tool) in python environments.
 Author: Dani Perez
 License: MIT
 Project-URL: Homepage, https://github.com/daniperez/vale-python-package
 Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 ## Installation
 
 You can add `vale` package as a dependency in your `setup.py`,
 `requirements.txt` or `pyproject.toml` file depending on how are you managing
 dependencies. For example, in `requirements.txt`:
 
 ```shell
-vale==3.3.1
+vale==3.4.1
 ```
 
 The version of this Python package corresponds exactly to Vale's version.  That
 is, if you add `vale==2.20.0` as a dependency, Vale with that same version will
 be installed.  Note that **Vale as such is not included in this package but
 downloaded the first time you execute `vale`**.
```

### Comparing `vale-3.3.1.0/README.md` & `vale-3.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ## Installation
 
 You can add `vale` package as a dependency in your `setup.py`,
 `requirements.txt` or `pyproject.toml` file depending on how are you managing
 dependencies. For example, in `requirements.txt`:
 
 ```shell
-vale==3.3.1
+vale==3.4.1
 ```
 
 The version of this Python package corresponds exactly to Vale's version.  That
 is, if you add `vale==2.20.0` as a dependency, Vale with that same version will
 be installed.  Note that **Vale as such is not included in this package but
 downloaded the first time you execute `vale`**.
```

### Comparing `vale-3.3.1.0/pyproject.toml` & `vale-3.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [project]
 name="vale"
 # This version corresponds to the original Vale's version, plus a 4th number to
 # account for fixes to this package. That 4th number is needed because PyPi
 # doesn't allow to re-release or upload deleted versions, every uploaded
 # version must be unique.
-version = "3.3.1.0"
+version = "3.4.1.0"
 authors = [
   { name="Dani Perez"},
 ]
 description = "Install and use Vale (grammar & style check tool) in python environments."
 readme = "README.md"
 license = { text="MIT" }
 requires-python = ">=3.7"
```

### Comparing `vale-3.3.1.0/vale/main.py` & `vale-3.4.1/vale/main.py`

 * *Files identical despite different names*

### Comparing `vale-3.3.1.0/vale.egg-info/PKG-INFO` & `vale-3.4.1/vale.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vale
-Version: 3.3.1.0
+Version: 3.4.1.0
 Summary: Install and use Vale (grammar & style check tool) in python environments.
 Author: Dani Perez
 License: MIT
 Project-URL: Homepage, https://github.com/daniperez/vale-python-package
 Project-URL: Bug Tracker, https://github.com/daniperez/vale-python-package/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,15 +30,15 @@
 ## Installation
 
 You can add `vale` package as a dependency in your `setup.py`,
 `requirements.txt` or `pyproject.toml` file depending on how are you managing
 dependencies. For example, in `requirements.txt`:
 
 ```shell
-vale==3.3.1
+vale==3.4.1
 ```
 
 The version of this Python package corresponds exactly to Vale's version.  That
 is, if you add `vale==2.20.0` as a dependency, Vale with that same version will
 be installed.  Note that **Vale as such is not included in this package but
 downloaded the first time you execute `vale`**.
```

