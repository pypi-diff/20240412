# Comparing `tmp/curitz-0.9.20.tar.gz` & `tmp/curitz-0.9.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curitz-0.9.20.tar", last modified: Fri Mar 31 11:39:07 2023, max compression
+gzip compressed data, was "curitz-0.9.21.tar", last modified: Fri Apr 12 10:51:36 2024, max compression
```

## Comparing `curitz-0.9.20.tar` & `curitz-0.9.21.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.324931 curitz-0.9.20/
--rw-rw-r--   0 hm        (1000) hm        (1000)      113 2023-03-30 12:48:01.000000 curitz-0.9.20/.gitignore
--rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-03-30 12:48:01.000000 curitz-0.9.20/.pre-commit-config.yaml
--rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-03-30 12:48:01.000000 curitz-0.9.20/LICENSE
--rw-rw-r--   0 hm        (1000) hm        (1000)       45 2023-03-31 11:39:02.000000 curitz-0.9.20/MANIFEST.in
--rw-rw-r--   0 hm        (1000) hm        (1000)      424 2023-03-30 12:48:01.000000 curitz-0.9.20/Makefile
--rw-rw-r--   0 hm        (1000) hm        (1000)    14917 2023-03-31 11:39:07.324931 curitz-0.9.20/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)     1160 2023-03-30 12:48:01.000000 curitz-0.9.20/README.rst
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.324931 curitz-0.9.20/action_plugin/
--rw-rw-r--   0 hm        (1000) hm        (1000)     1296 2023-03-30 12:48:01.000000 curitz-0.9.20/action_plugin/demoplugin1.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1274 2023-03-30 12:48:01.000000 curitz-0.9.20/pyproject.toml
--rw-rw-r--   0 hm        (1000) hm        (1000)       38 2023-03-31 11:39:07.324931 curitz-0.9.20/setup.cfg
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.320931 curitz-0.9.20/src/
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.324931 curitz-0.9.20/src/curitz/
--rw-rw-r--   0 hm        (1000) hm        (1000)      780 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/__init__.py
--rw-rw-r--   0 hm        (1000) hm        (1000)       30 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/__main__.py
--rwxrwxr-x   0 hm        (1000) hm        (1000)    37195 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/cli.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     4138 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/culistbox.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     8957 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/textpad.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1244 2023-03-30 12:48:01.000000 curitz-0.9.20/src/curitz/timed_cache.py
--rw-rw-r--   0 hm        (1000) hm        (1000)      162 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz/version.py
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.324931 curitz-0.9.20/src/curitz.egg-info/
--rw-rw-r--   0 hm        (1000) hm        (1000)    14917 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/PKG-INFO
--rw-rw-r--   0 hm        (1000) hm        (1000)      544 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/SOURCES.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/dependency_links.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)       43 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/entry_points.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-03-31 11:32:24.000000 curitz-0.9.20/src/curitz.egg-info/not-zip-safe
--rw-rw-r--   0 hm        (1000) hm        (1000)       56 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/requires.txt
--rw-rw-r--   0 hm        (1000) hm        (1000)        7 2023-03-31 11:39:07.000000 curitz-0.9.20/src/curitz.egg-info/top_level.txt
-drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2023-03-31 11:39:07.324931 curitz-0.9.20/tests/
--rw-rw-r--   0 hm        (1000) hm        (1000)     2663 2023-03-30 12:48:01.000000 curitz-0.9.20/tests/test_script.py
--rw-rw-r--   0 hm        (1000) hm        (1000)     1328 2023-03-30 12:48:01.000000 curitz-0.9.20/tox.ini
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.229731 curitz-0.9.21/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      113 2023-03-30 12:48:01.000000 curitz-0.9.21/.gitignore
+-rw-rw-r--   0 hm        (1000) hm        (1000)      417 2023-03-30 12:48:01.000000 curitz-0.9.21/.pre-commit-config.yaml
+-rw-rw-r--   0 hm        (1000) hm        (1000)    11358 2023-03-30 12:48:01.000000 curitz-0.9.21/LICENSE
+-rw-rw-r--   0 hm        (1000) hm        (1000)       45 2023-03-31 11:39:02.000000 curitz-0.9.21/MANIFEST.in
+-rw-rw-r--   0 hm        (1000) hm        (1000)      424 2023-03-30 12:48:01.000000 curitz-0.9.21/Makefile
+-rw-r--r--   0 hm        (1000) hm        (1000)    16583 2024-04-12 10:51:36.229731 curitz-0.9.21/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2547 2024-03-15 08:43:51.000000 curitz-0.9.21/README.rst
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.225731 curitz-0.9.21/action_plugin/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1296 2023-03-30 12:48:01.000000 curitz-0.9.21/action_plugin/demoplugin1.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1342 2024-04-12 10:36:18.000000 curitz-0.9.21/pyproject.toml
+-rw-rw-r--   0 hm        (1000) hm        (1000)       38 2024-04-12 10:51:36.229731 curitz-0.9.21/setup.cfg
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.225731 curitz-0.9.21/src/
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.229731 curitz-0.9.21/src/curitz/
+-rw-rw-r--   0 hm        (1000) hm        (1000)      780 2023-03-30 12:48:01.000000 curitz-0.9.21/src/curitz/__init__.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)       30 2023-03-30 12:48:01.000000 curitz-0.9.21/src/curitz/__main__.py
+-rwxrwxr-x   0 hm        (1000) hm        (1000)    37195 2023-08-23 12:38:31.000000 curitz-0.9.21/src/curitz/cli.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     4138 2023-03-30 12:48:01.000000 curitz-0.9.21/src/curitz/culistbox.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     8957 2023-03-30 12:48:01.000000 curitz-0.9.21/src/curitz/textpad.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1244 2023-03-30 12:48:01.000000 curitz-0.9.21/src/curitz/timed_cache.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)      413 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz/version.py
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.229731 curitz-0.9.21/src/curitz.egg-info/
+-rw-r--r--   0 hm        (1000) hm        (1000)    16583 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/PKG-INFO
+-rw-rw-r--   0 hm        (1000) hm        (1000)      544 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/SOURCES.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/dependency_links.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)       43 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/entry_points.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        1 2023-08-23 12:15:16.000000 curitz-0.9.21/src/curitz.egg-info/not-zip-safe
+-rw-rw-r--   0 hm        (1000) hm        (1000)       64 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/requires.txt
+-rw-rw-r--   0 hm        (1000) hm        (1000)        7 2024-04-12 10:51:36.000000 curitz-0.9.21/src/curitz.egg-info/top_level.txt
+drwxrwxr-x   0 hm        (1000) hm        (1000)        0 2024-04-12 10:51:36.229731 curitz-0.9.21/tests/
+-rw-rw-r--   0 hm        (1000) hm        (1000)     2663 2023-03-30 12:48:01.000000 curitz-0.9.21/tests/test_script.py
+-rw-rw-r--   0 hm        (1000) hm        (1000)     1332 2024-03-15 08:44:08.000000 curitz-0.9.21/tox.ini
```

### Comparing `curitz-0.9.20/LICENSE` & `curitz-0.9.21/LICENSE`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/PKG-INFO` & `curitz-0.9.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: curitz
-Version: 0.9.20
-Summary: Curses interface to Zino
+Version: 0.9.21
+Summary: Python ncurses terminal client to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,28 +212,74 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: zinolib<1.0,>=0.9.23
+Requires-Dist: dnspython
+Provides-Extra: test
+Requires-Dist: tox; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 ======
 curitz
 ======
 
 Python curses package to interface with Zino.
 
 Split from internal project PyRitz on 2023-03-30.
 
+Configuration
+=============
+
+There needs to be a file ``.ritz.tcl``, conventionally placed in your
+home-directory.
+
+Example ``.ritz.tcl``::
+    set Secret ZINO1SERVERTOKEN_A
+    set User USERNAME_1
+    set Server my.zino.server.com
+    set Port 8001
+
+    set _Secret(ALTERNATE) ZINO1SERVERTOKEN_B
+    set _User(ALTERNATE) USERNAME_2
+    set _Server(ALTERNATE) alternative.zino.server.com
+    set _Port(ALTERNATE) 8001
+
+The top four lines configures the default server. ``Secret`` and ``User`` is
+created by the admin of the zino server. ``Server`` and ``Port`` hopefully
+needs no explanation.
+
+Running ``curitz`` without the ``-p``-argument would connect to
+"my.zino.server.com", authenticated as USER_1.
+
+The bottom four lines are optional. They are an example of how to configure
+alternative servers. Running ``curitz`` with the ``/-``-argument would connect
+to the alternative server::
+
+    ``$ curitz -p ALTERNATE``
+
+This would connect to "alternative.zino.server.com", authenticated as USER_2.
+
+Running
+=======
+
+After installingOnce it is on your path the terminal program ``curitz`` will be available to run.
+
+Run ``curitz -h`` for info about the available arguments.
+
 Testing
 =======
 
 This library is testable with unittests. When testing it starts a Zino emulator
 that reponds correctly to requests as the real server would do.
 
 If you have all currently supported pythons in your path, you can test them
@@ -258,14 +304,18 @@
 if installing from source or::
 
     pip install --user curitz
 
 if installing from Pypi. This should normally put the binary and library under
 ``.local`` on Linux.
 
+If you develop python programs other than curitz we recommend that you install
+with ``pipx``. curitz and its dependencies will then be stored on your user but
+separately from any other thing you are working on.
+
 Development
 ===========
 
 Some minimal pre-commit hooks are included, install by running
 ``pre-commit install``.
 
 See the file `.git-blame-ignore-revs` for commits to ignore when running
```

### Comparing `curitz-0.9.20/action_plugin/demoplugin1.py` & `curitz-0.9.21/action_plugin/demoplugin1.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/pyproject.toml` & `curitz-0.9.21/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "curitz"
-description = "Curses interface to Zino"
+description = "Python ncurses terminal client to Zino"
 authors = [{name="Runar Borge", email="runar.borge@sikt.no"}]
 maintainers = [{name="Uninett Opensource", email="opensource@uninett.no"}]
 readme = "README.rst"
 requires-python = ">=3.7"
 dependencies = [
-    "zinolib<0.10",
+    "zinolib>=0.9.23,<1.0",
     "dnspython",
 ]
 license = {file="LICENSE"}
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
     "tox",
```

### Comparing `curitz-0.9.20/src/curitz/__init__.py` & `curitz-0.9.21/src/curitz/__init__.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/src/curitz/cli.py` & `curitz-0.9.21/src/curitz/cli.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/src/curitz/culistbox.py` & `curitz-0.9.21/src/curitz/culistbox.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/src/curitz/textpad.py` & `curitz-0.9.21/src/curitz/textpad.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/src/curitz/timed_cache.py` & `curitz-0.9.21/src/curitz/timed_cache.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/src/curitz.egg-info/PKG-INFO` & `curitz-0.9.21/src/curitz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: curitz
-Version: 0.9.20
-Summary: Curses interface to Zino
+Version: 0.9.21
+Summary: Python ncurses terminal client to Zino
 Author-email: Runar Borge <runar.borge@sikt.no>
 Maintainer-email: Uninett Opensource <opensource@uninett.no>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -212,28 +212,74 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: zinolib<1.0,>=0.9.23
+Requires-Dist: dnspython
+Provides-Extra: test
+Requires-Dist: tox; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 ======
 curitz
 ======
 
 Python curses package to interface with Zino.
 
 Split from internal project PyRitz on 2023-03-30.
 
+Configuration
+=============
+
+There needs to be a file ``.ritz.tcl``, conventionally placed in your
+home-directory.
+
+Example ``.ritz.tcl``::
+    set Secret ZINO1SERVERTOKEN_A
+    set User USERNAME_1
+    set Server my.zino.server.com
+    set Port 8001
+
+    set _Secret(ALTERNATE) ZINO1SERVERTOKEN_B
+    set _User(ALTERNATE) USERNAME_2
+    set _Server(ALTERNATE) alternative.zino.server.com
+    set _Port(ALTERNATE) 8001
+
+The top four lines configures the default server. ``Secret`` and ``User`` is
+created by the admin of the zino server. ``Server`` and ``Port`` hopefully
+needs no explanation.
+
+Running ``curitz`` without the ``-p``-argument would connect to
+"my.zino.server.com", authenticated as USER_1.
+
+The bottom four lines are optional. They are an example of how to configure
+alternative servers. Running ``curitz`` with the ``/-``-argument would connect
+to the alternative server::
+
+    ``$ curitz -p ALTERNATE``
+
+This would connect to "alternative.zino.server.com", authenticated as USER_2.
+
+Running
+=======
+
+After installingOnce it is on your path the terminal program ``curitz`` will be available to run.
+
+Run ``curitz -h`` for info about the available arguments.
+
 Testing
 =======
 
 This library is testable with unittests. When testing it starts a Zino emulator
 that reponds correctly to requests as the real server would do.
 
 If you have all currently supported pythons in your path, you can test them
@@ -258,14 +304,18 @@
 if installing from source or::
 
     pip install --user curitz
 
 if installing from Pypi. This should normally put the binary and library under
 ``.local`` on Linux.
 
+If you develop python programs other than curitz we recommend that you install
+with ``pipx``. curitz and its dependencies will then be stored on your user but
+separately from any other thing you are working on.
+
 Development
 ===========
 
 Some minimal pre-commit hooks are included, install by running
 ``pre-commit install``.
 
 See the file `.git-blame-ignore-revs` for commits to ignore when running
```

### Comparing `curitz-0.9.20/src/curitz.egg-info/SOURCES.txt` & `curitz-0.9.21/src/curitz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/tests/test_script.py` & `curitz-0.9.21/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `curitz-0.9.20/tox.ini` & `curitz-0.9.21/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tox]
 envlist =
     clean
     mypy
-    py{37,38,39,310,311}
+    py{37,38,39,310,311,312}
     coverage-html
 skipsdist = True
 skip_missing_interpreters = True
 basepython = python3.10
 
 [testenv:clean]
 deps =
```

