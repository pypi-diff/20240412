# Comparing `tmp/fab-react-toolkit-0.3.7.tar.gz` & `tmp/fab-react-toolkit-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fab-react-toolkit-0.3.7.tar", last modified: Wed Apr 10 16:22:30 2024, max compression
+gzip compressed data, was "fab-react-toolkit-0.3.9.tar", last modified: Fri Apr 12 07:31:18 2024, max compression
```

## Comparing `fab-react-toolkit-0.3.7.tar` & `fab-react-toolkit-0.3.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.049234 fab-react-toolkit-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 16:22:30.049234 fab-react-toolkit-0.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.045234 fab-react-toolkit-0.3.7/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.045234 fab-react-toolkit-0.3.7/example/app/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/app/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/app/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/app/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/example/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.045234 fab-react-toolkit-0.3.7/fab_react_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.049234 fab-react-toolkit-0.3.7/fab_react_toolkit/api/
--rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/api/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/fab_react_toolkit/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 16:22:30.049234 fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-10 16:22:30.000000 fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-10 16:22:30.000000 fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 16:22:30.000000 fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 16:22:30.000000 fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-10 16:22:14.000000 fab-react-toolkit-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-10 16:22:30.049234 fab-react-toolkit-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/example/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/example/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/fab_react_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.036207 fab-react-toolkit-0.3.9/fab_react_toolkit/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20853 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/api/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12522 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/fab_react_toolkit/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 07:31:18.000000 fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-12 07:31:09.000000 fab-react-toolkit-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:31:18.040207 fab-react-toolkit-0.3.9/setup.cfg
```

### Comparing `fab-react-toolkit-0.3.7/LICENSE` & `fab-react-toolkit-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/PKG-INFO` & `fab-react-toolkit-0.3.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.7
+Version: 0.3.9
 Summary: A small example package
-Home-page: https://github.com/dttctcs/fab-react-toolkit
-Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Flask-AppBuilder<=4.3.10
```

### Comparing `fab-react-toolkit-0.3.7/example/app/__init__.py` & `fab-react-toolkit-0.3.9/example/app/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/example/app/apis.py` & `fab-react-toolkit-0.3.9/example/app/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/example/app/config.py` & `fab-react-toolkit-0.3.9/example/app/config.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/example/app/models.py` & `fab-react-toolkit-0.3.9/example/app/models.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/example/run.py` & `fab-react-toolkit-0.3.9/example/run.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/__init__.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/api/__init__.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/api/convert.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/api/convert.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/apis.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/apis.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/filters.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/filters.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit/views.py` & `fab-react-toolkit-0.3.9/fab_react_toolkit/views.py`

 * *Files identical despite different names*

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/PKG-INFO` & `fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: fab-react-toolkit
-Version: 0.3.7
+Version: 0.3.9
 Summary: A small example package
-Home-page: https://github.com/dttctcs/fab-react-toolkit
-Author: Datatactics GmbH
 Author-email: Matthias Leinweber <m.leinweber@datatactics.de>
 Project-URL: Homepage, https://github.com/dttctcs/fab-react-toolkit
 Project-URL: Issues, https://github.com/dttctcs/fab-react-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Flask-AppBuilder<=4.3.10
```

### Comparing `fab-react-toolkit-0.3.7/fab_react_toolkit.egg-info/SOURCES.txt` & `fab-react-toolkit-0.3.9/fab_react_toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 pyproject.toml
 requirements.txt
-setup.cfg
 example/readme.md
 example/requirements.txt
 example/run.py
 example/app/__init__.py
 example/app/apis.py
 example/app/config.py
 example/app/models.py
@@ -13,11 +12,12 @@
 fab_react_toolkit/apis.py
 fab_react_toolkit/filters.py
 fab_react_toolkit/interface.py
 fab_react_toolkit/views.py
 fab_react_toolkit.egg-info/PKG-INFO
 fab_react_toolkit.egg-info/SOURCES.txt
 fab_react_toolkit.egg-info/dependency_links.txt
+fab_react_toolkit.egg-info/requires.txt
 fab_react_toolkit.egg-info/top_level.txt
 fab_react_toolkit/api/__init__.py
 fab_react_toolkit/api/convert.py
 fab_react_toolkit/api/decorators.py
```

### Comparing `fab-react-toolkit-0.3.7/pyproject.toml` & `fab-react-toolkit-0.3.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
+dependencies = [
+    "Flask-AppBuilder <= 4.3.10"
+]
+
 [tool.setuptools_scm]
 root = ".."
 
 
 [project.urls]
 Homepage = "https://github.com/dttctcs/fab-react-toolkit"
 Issues = "https://github.com/dttctcs/fab-react-toolkit/issues"
```

