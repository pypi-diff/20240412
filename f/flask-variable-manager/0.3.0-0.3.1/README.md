# Comparing `tmp/flask-variable-manager-0.3.0.tar.gz` & `tmp/flask-variable-manager-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-variable-manager-0.3.0.tar", last modified: Wed Apr 10 08:25:30 2024, max compression
+gzip compressed data, was "flask-variable-manager-0.3.1.tar", last modified: Fri Apr 12 14:35:37 2024, max compression
```

## Comparing `flask-variable-manager-0.3.0.tar` & `flask-variable-manager-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/extension/variable_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/flask_variable_manager/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-10 08:25:30.000000 flask-variable-manager-0.3.0/flask_variable_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-10 08:25:25.000000 flask-variable-manager-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:25:30.167675 flask-variable-manager-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7101 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/extension/variable_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/flask_variable_manager/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 14:35:37.000000 flask-variable-manager-0.3.1/flask_variable_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-12 14:35:30.000000 flask-variable-manager-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:35:37.170586 flask-variable-manager-0.3.1/setup.cfg
```

### Comparing `flask-variable-manager-0.3.0/LICENSE` & `flask-variable-manager-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.0/PKG-INFO` & `flask-variable-manager-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: flask==2.3.3
+Requires-Dist: flask==3.0.3
 Requires-Dist: Jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: flasgger==0.9.7b2; extra == "dev"
 Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
 
 # Flask Variable Manager
```

### Comparing `flask-variable-manager-0.3.0/README.md` & `flask-variable-manager-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.0/flask_variable_manager/extension/variable_manager.py` & `flask-variable-manager-0.3.1/flask_variable_manager/extension/variable_manager.py`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.0/flask_variable_manager/tests/test_vm.py` & `flask-variable-manager-0.3.1/flask_variable_manager/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `flask-variable-manager-0.3.0/flask_variable_manager.egg-info/PKG-INFO` & `flask-variable-manager-0.3.1/flask_variable_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Flask
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: flask==2.3.3
+Requires-Dist: flask==3.0.3
 Requires-Dist: Jinja2==3.1.3
 Provides-Extra: dev
 Requires-Dist: flasgger==0.9.7b2; extra == "dev"
 Requires-Dist: build==1.2.1; extra == "dev"
 Requires-Dist: twine==5.0.0; extra == "dev"
 
 # Flask Variable Manager
```

### Comparing `flask-variable-manager-0.3.0/pyproject.toml` & `flask-variable-manager-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ['flask_variable_manager*']
 
 [project]
 name = "flask-variable-manager"
-version = "0.3.0"
+version = "0.3.1"
 description = "Create a variable manager in flask, enter values in python, and use values on the jinja template."
 authors = [
     { name = "minwook-shin", email = "minwook0106@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Framework :: Flask"
 ]
 dependencies = [
-    "flask==2.3.3",
+    "flask==3.0.3",
     "Jinja2==3.1.3"
 ]
 
 [project.optional-dependencies]
 dev = [
     "flasgger==0.9.7b2",
     "build==1.2.1",
```

