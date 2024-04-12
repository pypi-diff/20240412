# Comparing `tmp/optioner-1.4.9.tar.gz` & `tmp/optioner-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.9.tar", last modified: Fri Apr 12 17:12:33 2024, max compression
+gzip compressed data, was "optioner-1.5.tar", last modified: Fri Apr 12 17:23:43 2024, max compression
```

## Comparing `optioner-1.4.9.tar` & `optioner-1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 17:12:28.000000 optioner-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-12 17:12:33.126826 optioner-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-12 17:12:28.000000 optioner-1.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 17:12:28.000000 optioner-1.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:12:33.126826 optioner-1.4.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.122826 optioner-1.4.9/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:28.000000 optioner-1.4.9/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/src/optioner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 17:12:33.000000 optioner-1.4.9/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-12 17:12:28.000000 optioner-1.4.9/src/optioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:12:33.126826 optioner-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_compulsory_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ifthisthennotthat.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ifthisthennotthat_vigorous.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 17:12:28.000000 optioner-1.4.9/tests/test_ignore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:43.802945 optioner-1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-12 17:23:39.000000 optioner-1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-12 17:23:43.802945 optioner-1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-12 17:23:39.000000 optioner-1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 17:23:39.000000 optioner-1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:23:43.802945 optioner-1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:43.802945 optioner-1.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:39.000000 optioner-1.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:43.802945 optioner-1.5/src/optioner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-12 17:23:43.000000 optioner-1.5/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 17:23:43.000000 optioner-1.5/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:23:43.000000 optioner-1.5/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 17:23:43.000000 optioner-1.5/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-04-12 17:23:39.000000 optioner-1.5/src/optioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:23:43.802945 optioner-1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-12 17:23:39.000000 optioner-1.5/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-12 17:23:39.000000 optioner-1.5/tests/test_compulsory_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-12 17:23:39.000000 optioner-1.5/tests/test_ifthisthennotthat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-12 17:23:39.000000 optioner-1.5/tests/test_ifthisthennotthat_vigorous.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 17:23:39.000000 optioner-1.5/tests/test_ignore.py
```

### Comparing `optioner-1.4.9/LICENSE` & `optioner-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.9/PKG-INFO` & `optioner-1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.9
+Version: 1.5
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: GitHub, https://github.com/d33pster/optioner
 Project-URL: Issues, https://github.com/d33pster/optioner/issues
 Project-URL: Documentation, https://d33pster.github.io/optioner/
 Keywords: d33pster,optioner,argument-parser,argument,parser,argparse
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.9 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.5 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -15,16 +15,16 @@
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: GitHub, https://github.com/d33pster/
 optioner Project-URL: Issues, https://github.com/d33pster/optioner/issues
 Project-URL: Documentation, https://d33pster.github.io/optioner/ Keywords:
 d33pster,optioner,argument-parser,argument,parser,argparse Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
 [![Continuous Deployment](https://github.com/d33pster/optioner/actions/
 workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/
```

### Comparing `optioner-1.4.9/README.md` & `optioner-1.5/README.md`

 * *Files identical despite different names*

### Comparing `optioner-1.4.9/pyproject.toml` & `optioner-1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.9"
+version = "1.5"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
```

### Comparing `optioner-1.4.9/src/optioner.egg-info/PKG-INFO` & `optioner-1.5/src/optioner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.9
+Version: 1.5
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -26,15 +26,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: GitHub, https://github.com/d33pster/optioner
 Project-URL: Issues, https://github.com/d33pster/optioner/issues
 Project-URL: Documentation, https://d33pster.github.io/optioner/
 Keywords: d33pster,optioner,argument-parser,argument,parser,argparse
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.9 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.5 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -15,16 +15,16 @@
 EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
 OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE. Project-URL: GitHub, https://github.com/d33pster/
 optioner Project-URL: Issues, https://github.com/d33pster/optioner/issues
 Project-URL: Documentation, https://d33pster.github.io/optioner/ Keywords:
 d33pster,optioner,argument-parser,argument,parser,argparse Classifier:
-Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools Classifier:
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: Topic :: Software Development :: Build Tools Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.9 Description-Content-Type: text/markdown License-File: LICENSE # optioner
 [![Continuous Deployment](https://github.com/d33pster/optioner/actions/
 workflows/cont-dep.yml/badge.svg)](https://github.com/d33pster/optioner/
```

### Comparing `optioner-1.4.9/src/optioner.py` & `optioner-1.5/src/optioner.py`

 * *Files identical despite different names*

### Comparing `optioner-1.4.9/tests/test_basic.py` & `optioner-1.5/tests/test_basic.py`

 * *Files identical despite different names*

