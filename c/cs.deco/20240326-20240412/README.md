# Comparing `tmp/cs.deco-20240326.tar.gz` & `tmp/cs.deco-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.deco-20240326.tar", last modified: Tue Mar 26 06:36:33 2024, max compression
+gzip compressed data, was "cs.deco-20240412.tar", last modified: Fri Apr 12 02:38:42 2024, max compression
```

## Comparing `cs.deco-20240326.tar` & `cs.deco-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:36:33.806143 cs.deco-20240326/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-26 06:35:39.000000 cs.deco-20240326/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    22165 2024-03-26 06:36:33.805794 cs.deco-20240326/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    21426 2024-03-26 06:35:57.000000 cs.deco-20240326/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:36:33.801451 cs.deco-20240326/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:36:33.801747 cs.deco-20240326/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:36:33.803263 cs.deco-20240326/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    35713 2024-03-26 06:35:26.000000 cs.deco-20240326/lib/python/cs/deco.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:36:33.805305 cs.deco-20240326/lib/python/cs.deco.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    22165 2024-03-26 06:36:33.000000 cs.deco-20240326/lib/python/cs.deco.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      267 2024-03-26 06:36:33.000000 cs.deco-20240326/lib/python/cs.deco.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-26 06:36:33.000000 cs.deco-20240326/lib/python/cs.deco.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       22 2024-03-26 06:36:33.000000 cs.deco-20240326/lib/python/cs.deco.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-26 06:36:33.000000 cs.deco-20240326/lib/python/cs.deco.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    22584 2024-03-26 06:36:32.000000 cs.deco-20240326/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-26 06:36:33.806245 cs.deco-20240326/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:38:42.444450 cs.deco-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 02:37:51.000000 cs.deco-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    22239 2024-04-12 02:38:42.444080 cs.deco-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    21500 2024-04-12 02:38:08.000000 cs.deco-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:38:42.440345 cs.deco-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:38:42.440638 cs.deco-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:38:42.441906 cs.deco-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    35773 2024-04-12 02:37:33.000000 cs.deco-20240412/lib/python/cs/deco.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:38:42.443588 cs.deco-20240412/lib/python/cs.deco.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    22239 2024-04-12 02:38:41.000000 cs.deco-20240412/lib/python/cs.deco.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      267 2024-04-12 02:38:42.000000 cs.deco-20240412/lib/python/cs.deco.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 02:38:41.000000 cs.deco-20240412/lib/python/cs.deco.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       22 2024-04-12 02:38:42.000000 cs.deco-20240412/lib/python/cs.deco.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 02:38:42.000000 cs.deco-20240412/lib/python/cs.deco.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    22658 2024-04-12 02:38:41.000000 cs.deco-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 02:38:42.444559 cs.deco-20240412/setup.cfg
```

### Comparing `cs.deco-20240326/PKG-INFO` & `cs.deco-20240412/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.deco
-Version: 20240326
+Version: 20240412
 Summary: Assorted function decorators.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted function decorators.
 
-*Latest release 20240326*:
-default_params: update wrapper signature to mark the defaulted params as optional.
+*Latest release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
 
 ## Function `ALL(func)`
 
 Include this function's name in its module's `__all__` list.
 
 Example:
 
@@ -531,14 +531,17 @@
 
 *Note*: use of this decorator requires the `cs.pfx` module.
 
 # Release Log
 
 
 
+*Release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
+
 *Release 20240326*:
 default_params: update wrapper signature to mark the defaulted params as optional.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240314.1*:
```

### Comparing `cs.deco-20240326/README.md` & `cs.deco-20240412/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Assorted function decorators.
 
-*Latest release 20240326*:
-default_params: update wrapper signature to mark the defaulted params as optional.
+*Latest release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
 
 ## Function `ALL(func)`
 
 Include this function's name in its module's `__all__` list.
 
 Example:
 
@@ -513,14 +513,17 @@
 
 *Note*: use of this decorator requires the `cs.pfx` module.
 
 # Release Log
 
 
 
+*Release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
+
 *Release 20240326*:
 default_params: update wrapper signature to mark the defaulted params as optional.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240314.1*:
```

### Comparing `cs.deco-20240326/lib/python/cs/deco.py` & `cs.deco-20240412/lib/python/cs/deco.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 import time
 import traceback
 import typing
 
 from cs.gimmicks import warning
 
-__version__ = '20240326'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -149,14 +149,15 @@
       return decorate(func, *da, **dkw)
 
     # `func` is not supplied, collect the arguments supplied and return a
     # decorator which takes the subsequent callable and returns
     # `deco(func, *da, **kw)`.
     return lambda func: decorate(func, *da, **dkw)
 
+  metadeco.__name__ = getattr(deco, '__name__', repr(deco))
   metadeco.__doc__ = getattr(deco, '__doc__', '')
   metadeco.__module__ = getattr(deco, '__module__', None)
   return metadeco
 
 @decorator
 def contextdecorator(cmgrfunc):
   ''' A decorator for a context manager function `cmgrfunc`
```

### Comparing `cs.deco-20240326/lib/python/cs.deco.egg-info/PKG-INFO` & `cs.deco-20240412/lib/python/cs.deco.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.deco
-Version: 20240326
+Version: 20240412
 Summary: Assorted function decorators.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted function decorators.
 
-*Latest release 20240326*:
-default_params: update wrapper signature to mark the defaulted params as optional.
+*Latest release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
 
 ## Function `ALL(func)`
 
 Include this function's name in its module's `__all__` list.
 
 Example:
 
@@ -531,14 +531,17 @@
 
 *Note*: use of this decorator requires the `cs.pfx` module.
 
 # Release Log
 
 
 
+*Release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
+
 *Release 20240326*:
 default_params: update wrapper signature to mark the defaulted params as optional.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240314.1*:
```

### Comparing `cs.deco-20240326/pyproject.toml` & `cs.deco-20240412/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240326"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted function decorators.
 
-*Latest release 20240326*:
-default_params: update wrapper signature to mark the defaulted params as optional.
+*Latest release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
 
 ## Function `ALL(func)`
 
 Include this function's name in its module's `__all__` list.
 
 Example:
 
@@ -545,14 +545,17 @@
 
 *Note*: use of this decorator requires the `cs.pfx` module.
 
 # Release Log
 
 
 
+*Release 20240412*:
+@decorator: apply the decorated function name to the metadecorator.
+
 *Release 20240326*:
 default_params: update wrapper signature to mark the defaulted params as optional.
 
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240314.1*:
```

