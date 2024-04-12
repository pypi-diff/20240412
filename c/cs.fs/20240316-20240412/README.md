# Comparing `tmp/cs.fs-20240316.tar.gz` & `tmp/cs.fs-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fs-20240316.tar", last modified: Sat Mar 16 06:35:55 2024, max compression
+gzip compressed data, was "cs.fs-20240412.tar", last modified: Fri Apr 12 05:22:15 2024, max compression
```

## Comparing `cs.fs-20240316.tar` & `cs.fs-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:35:55.488731 cs.fs-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:35:42.000000 cs.fs-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6584 2024-03-16 06:35:55.488359 cs.fs-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     6245 2024-03-16 06:35:45.000000 cs.fs-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:35:55.484055 cs.fs-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:35:55.484351 cs.fs-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:35:55.485743 cs.fs-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    12535 2024-03-16 06:35:31.000000 cs.fs-20240316/lib/python/cs/fs.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:35:55.487665 cs.fs-20240316/lib/python/cs.fs.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6584 2024-03-16 06:35:54.000000 cs.fs-20240316/lib/python/cs.fs.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-03-16 06:35:55.000000 cs.fs-20240316/lib/python/cs.fs.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:35:55.000000 cs.fs-20240316/lib/python/cs.fs.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       62 2024-03-16 06:35:55.000000 cs.fs-20240316/lib/python/cs.fs.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:35:55.000000 cs.fs-20240316/lib/python/cs.fs.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6988 2024-03-16 06:35:53.000000 cs.fs-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:35:55.488843 cs.fs-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.279561 cs.fs-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:22:03.000000 cs.fs-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7320 2024-04-12 05:22:15.279341 cs.fs-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     6506 2024-04-12 05:22:07.000000 cs.fs-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.276446 cs.fs-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.276669 cs.fs-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.277697 cs.fs-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    12685 2024-04-12 05:21:50.000000 cs.fs-20240412/lib/python/cs/fs.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:22:15.279002 cs.fs-20240412/lib/python/cs.fs.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7320 2024-04-12 05:22:14.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:22:14.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       62 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:22:15.000000 cs.fs-20240412/lib/python/cs.fs.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     7724 2024-04-12 05:22:13.000000 cs.fs-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:22:15.279646 cs.fs-20240412/setup.cfg
```

### Comparing `cs.fs-20240316/PKG-INFO` & `cs.fs-20240412/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20240316
+Version: 20240412
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -71,15 +71,33 @@
 - set `.fspath` to `self._resolve_fspath(fspath)`
 - set `._lock` to `lock` (or `threading.Lock()` if not specified)
 - return `True`
 On subsequent calls return `False`.
 
 ## Class `HasFSPath`
 
-An object with a `.fspath` attribute representing a filesystem location.
+A mixin for an object with a `.fspath` attribute representing a filesystem location.
+
+The `__init__` method just sets the `.fspath` attribute, and
+need not be called if the main class takes care of that itself.
+
+*Method `HasFSPath.fnmatch(self, fnglob)`*:
+Return a list of the names in `self.fspath` matching the glob `fnglob`.
+
+*Method `HasFSPath.listdir(self)`*:
+Return `os.listdir(self.fspath)`.
+
+*Method `HasFSPath.pathto(self, *subpaths)`*:
+The full path to `subpaths`, comprising a relative path
+below `self.fspath`.
+This is a shim for `os.path.join` which requires that all
+the `subpaths` be relative paths.
+
+*Property `HasFSPath.shortpath`*:
+The short version of `self.fspath`.
 
 ## Function `is_valid_rpath(rpath, log=None) -> bool`
 
 Test that `rpath` is a clean relative path with no funny business.
 
 This is a Boolean wrapper for `validate_rpath()`.
 
@@ -140,14 +158,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 * FSPathBasedSingleton: drop the default_factory parameter/attribute, let default_attr specify a callable.
 * Singleton._resolve_fspath: fix reference to class name.
```

### Comparing `cs.fs-20240316/README.md` & `cs.fs-20240412/lib/python/cs.fs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+Metadata-Version: 2.1
+Name: cs.fs
+Version: 20240412
+Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -53,15 +71,18 @@
 - set `.fspath` to `self._resolve_fspath(fspath)`
 - set `._lock` to `lock` (or `threading.Lock()` if not specified)
 - return `True`
 On subsequent calls return `False`.
 
 ## Class `HasFSPath`
 
-An object with a `.fspath` attribute representing a filesystem location.
+A mixin for an object with a `.fspath` attribute representing a filesystem location.
+
+The `__init__` method just sets the `.fspath` attribute, and
+need not be called if the main class takes care of that itself.
 
 *Method `HasFSPath.fnmatch(self, fnglob)`*:
 Return a list of the names in `self.fspath` matching the glob `fnglob`.
 
 *Method `HasFSPath.listdir(self)`*:
 Return `os.listdir(self.fspath)`.
 
@@ -137,14 +158,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 * FSPathBasedSingleton: drop the default_factory parameter/attribute, let default_attr specify a callable.
 * Singleton._resolve_fspath: fix reference to class name.
 
@@ -181,7 +205,8 @@
 * Add longpath and shortpath from cs.fileutils.
 * New is_clean_subpath(subpath).
 * New needdir(path).
 * New fnmatchdir(dirpath,fnglob) pulled out from HasFSPath.fnmatch(fnglob).
 
 *Release 20220327*:
 New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated.
+
```

### Comparing `cs.fs-20240316/lib/python/cs/fs.py` & `cs.fs-20240412/lib/python/cs/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from icontract import require
 
 from cs.deco import decorator
 from cs.obj import SingletonMixin
 from cs.pfx import pfx, pfx_call
 
-__version__ = '20240316'
+__version__ = '20240412'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -153,15 +153,18 @@
 def fnmatchdir(dirpath, fnglob):
   ''' Return a list of the names in `dirpath` matching the glob `fnglob`.
   '''
   return fnfilter(pfx_listdir(dirpath), fnglob)
 
 # pylint: disable=too-few-public-methods
 class HasFSPath:
-  ''' An object with a `.fspath` attribute representing a filesystem location.
+  ''' A mixin for an object with a `.fspath` attribute representing a filesystem location.
+
+      The `__init__` method just sets the `.fspath` attribute, and
+      need not be called if the main class takes care of that itself.
   '''
 
   def __init__(self, fspath):
     self.fspath = fspath
 
   def __str__(self):
     return f'{self.__class__.__name__}(fspath={self.shortpath})'
```

### Comparing `cs.fs-20240316/lib/python/cs.fs.egg-info/PKG-INFO` & `cs.fs-20240412/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-Metadata-Version: 2.1
-Name: cs.fs
-Version: 20240316
-Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -71,15 +53,33 @@
 - set `.fspath` to `self._resolve_fspath(fspath)`
 - set `._lock` to `lock` (or `threading.Lock()` if not specified)
 - return `True`
 On subsequent calls return `False`.
 
 ## Class `HasFSPath`
 
-An object with a `.fspath` attribute representing a filesystem location.
+A mixin for an object with a `.fspath` attribute representing a filesystem location.
+
+The `__init__` method just sets the `.fspath` attribute, and
+need not be called if the main class takes care of that itself.
+
+*Method `HasFSPath.fnmatch(self, fnglob)`*:
+Return a list of the names in `self.fspath` matching the glob `fnglob`.
+
+*Method `HasFSPath.listdir(self)`*:
+Return `os.listdir(self.fspath)`.
+
+*Method `HasFSPath.pathto(self, *subpaths)`*:
+The full path to `subpaths`, comprising a relative path
+below `self.fspath`.
+This is a shim for `os.path.join` which requires that all
+the `subpaths` be relative paths.
+
+*Property `HasFSPath.shortpath`*:
+The short version of `self.fspath`.
 
 ## Function `is_valid_rpath(rpath, log=None) -> bool`
 
 Test that `rpath` is a clean relative path with no funny business.
 
 This is a Boolean wrapper for `validate_rpath()`.
 
@@ -140,14 +140,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 * FSPathBasedSingleton: drop the default_factory parameter/attribute, let default_attr specify a callable.
 * Singleton._resolve_fspath: fix reference to class name.
 
@@ -184,8 +187,7 @@
 * Add longpath and shortpath from cs.fileutils.
 * New is_clean_subpath(subpath).
 * New needdir(path).
 * New fnmatchdir(dirpath,fnglob) pulled out from HasFSPath.fnmatch(fnglob).
 
 *Release 20220327*:
 New module cs.fs to contain more filesystem focussed functions than cs.fileutils, which is feeling a bit bloated.
-
```

### Comparing `cs.fs-20240316/pyproject.toml` & `cs.fs-20240412/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,43 +5,43 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20240316",
+    "cs.deco>=20240412",
     "cs.obj>=20220918",
-    "cs.pfx>=20230604",
+    "cs.pfx>=20240412",
     "icontract",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240316"
+version = "20240412"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -88,15 +88,33 @@
 - set `.fspath` to `self._resolve_fspath(fspath)`
 - set `._lock` to `lock` (or `threading.Lock()` if not specified)
 - return `True`
 On subsequent calls return `False`.
 
 ## Class `HasFSPath`
 
-An object with a `.fspath` attribute representing a filesystem location.
+A mixin for an object with a `.fspath` attribute representing a filesystem location.
+
+The `__init__` method just sets the `.fspath` attribute, and
+need not be called if the main class takes care of that itself.
+
+*Method `HasFSPath.fnmatch(self, fnglob)`*:
+Return a list of the names in `self.fspath` matching the glob `fnglob`.
+
+*Method `HasFSPath.listdir(self)`*:
+Return `os.listdir(self.fspath)`.
+
+*Method `HasFSPath.pathto(self, *subpaths)`*:
+The full path to `subpaths`, comprising a relative path
+below `self.fspath`.
+This is a shim for `os.path.join` which requires that all
+the `subpaths` be relative paths.
+
+*Property `HasFSPath.shortpath`*:
+The short version of `self.fspath`.
 
 ## Function `is_valid_rpath(rpath, log=None) -> bool`
 
 Test that `rpath` is a clean relative path with no funny business.
 
 This is a Boolean wrapper for `validate_rpath()`.
 
@@ -157,14 +175,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240412*:
+HasFSPath: explain that the __init__ is optional in the docstring.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240201*:
 * FSPathBasedSingleton: drop the default_factory parameter/attribute, let default_attr specify a callable.
 * Singleton._resolve_fspath: fix reference to class name.
```

