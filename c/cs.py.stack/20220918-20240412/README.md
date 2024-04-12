# Comparing `tmp/cs.py.stack-20220918.tar.gz` & `tmp/cs.py.stack-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.py.stack-20220918.tar", last modified: Sat Sep 17 23:07:11 2022, max compression
+gzip compressed data, was "cs.py.stack-20240412.tar", last modified: Fri Apr 12 02:36:05 2024, max compression
```

## Comparing `cs.py.stack-20220918.tar` & `cs.py.stack-20240412.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.367881 cs.py.stack-20220918/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2022-09-17 23:06:54.000000 cs.py.stack-20220918/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     2772 2022-09-17 23:07:11.368006 cs.py.stack-20220918/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     1887 2022-09-17 23:06:56.000000 cs.py.stack-20220918/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.364624 cs.py.stack-20220918/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.364856 cs.py.stack-20220918/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.364964 cs.py.stack-20220918/lib/python/cs/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.367628 cs.py.stack-20220918/lib/python/cs/py/
--rw-r--r--   0 cameron    (501) cameron    (502)     2418 2022-09-17 23:06:46.000000 cs.py.stack-20220918/lib/python/cs/py/stack.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2022-09-17 23:07:11.367352 cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     2772 2022-09-17 23:07:11.000000 cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      265 2022-09-17 23:07:11.000000 cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2022-09-17 23:07:11.000000 cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2022-09-17 23:07:11.000000 cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     2908 2022-09-17 23:07:02.000000 cs.py.stack-20220918/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)      837 2022-09-17 23:07:11.368565 cs.py.stack-20220918/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2022-09-17 23:06:56.000000 cs.py.stack-20220918/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.439509 cs.py.stack-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 02:35:56.000000 cs.py.stack-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3063 2024-04-12 02:36:05.439226 cs.py.stack-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     2248 2024-04-12 02:35:59.000000 cs.py.stack-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.435899 cs.py.stack-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.436197 cs.py.stack-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.436305 cs.py.stack-20240412/lib/python/cs/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.438792 cs.py.stack-20240412/lib/python/cs/py/
+-rw-r--r--   0 cameron    (501) cameron    (502)     4253 2024-04-12 02:35:39.000000 cs.py.stack-20240412/lib/python/cs/py/stack.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:36:05.438467 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3063 2024-04-12 02:36:04.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      246 2024-04-12 02:36:05.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 02:36:04.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 02:36:05.000000 cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3373 2024-04-12 02:36:03.000000 cs.py.stack-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 02:36:05.439605 cs.py.stack-20240412/setup.cfg
```

### Comparing `cs.py.stack-20220918/PKG-INFO` & `cs.py.stack-20240412/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,55 @@
-Metadata-Version: 2.1
-Name: cs.py.stack
-Version: 20220918
-Summary: Convenience functions for the python execution stack.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
-
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20220918*:
-caller(): return None if the frame offset is out of range.
+*Latest release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
 * `-1`: caller, this function
 * `-2`: invoker, who wants to know the caller
 * `-3`: the calling function of the invoker
 
 The default `from_index` value is `-3`.
 
-## Class `Frame(Frame, builtins.tuple)`
-
-A `namedtuple` for stack frame contents.
-
 ## Function `frames()`
 
 Return the current stack as a list of `Frame` objects.
 
-## Function `stack_dump(fp=None, indent=0, Fs=None, skip=None)`
+## Function `stack_dump(f=None, indent=0, frames=None, skip=None, select=None, format_frame=None)`
 
-Recite current or supplied stack to `fp`, default `sys.stderr`.
+Recite current or supplied stack to `f`, default `sys.stderr`.
 
 Parameters:
-* `fp`: the output file object, default `sys.stderr`
+* `f`: the output file object, default `sys.stderr`
 * `indent`: how many spaces to indent the stack lines, default `0`
-* `Fs`: the stack `Frame`s to write,
+* `frames`: the stack `Frame`s to write,
   default obtained from the current stack
-* `skip`: the number of `Frame`s to trim from the end of `Fs`;
-  if `Fs` is `None` this defaults to `2` to trim the `Frame`s
+* `skip`: the number of `Frame`s to trim from the end of `frames`;
+  if `frames` is `None` this defaults to `2` to trim the `Frame`s
   for the `stack_dump` function and its call to `frames()`,
   otherwise the default is `0` to use the supplied `Frame`s as is
+* `select`: if not `None`, select particular frames;
+  if `select` is a `str` it must be present in the frame filename;
+  otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
+
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
 
 *Release 20220429*:
 caller: return None if the stack index is out of range.
 
 *Release 20190812*:
```

### Comparing `cs.py.stack-20220918/lib/python/cs.py.stack.egg-info/PKG-INFO` & `cs.py.stack-20240412/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 Metadata-Version: 2.1
 Name: cs.py.stack
-Version: 20220918
+Version: 20240412
 Summary: Convenience functions for the python execution stack.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20220918*:
-caller(): return None if the frame offset is out of range.
+*Latest release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
 * `-1`: caller, this function
 * `-2`: invoker, who wants to know the caller
 * `-3`: the calling function of the invoker
 
 The default `from_index` value is `-3`.
 
-## Class `Frame(Frame, builtins.tuple)`
-
-A `namedtuple` for stack frame contents.
-
 ## Function `frames()`
 
 Return the current stack as a list of `Frame` objects.
 
-## Function `stack_dump(fp=None, indent=0, Fs=None, skip=None)`
+## Function `stack_dump(f=None, indent=0, frames=None, skip=None, select=None, format_frame=None)`
 
-Recite current or supplied stack to `fp`, default `sys.stderr`.
+Recite current or supplied stack to `f`, default `sys.stderr`.
 
 Parameters:
-* `fp`: the output file object, default `sys.stderr`
+* `f`: the output file object, default `sys.stderr`
 * `indent`: how many spaces to indent the stack lines, default `0`
-* `Fs`: the stack `Frame`s to write,
+* `frames`: the stack `Frame`s to write,
   default obtained from the current stack
-* `skip`: the number of `Frame`s to trim from the end of `Fs`;
-  if `Fs` is `None` this defaults to `2` to trim the `Frame`s
+* `skip`: the number of `Frame`s to trim from the end of `frames`;
+  if `frames` is `None` this defaults to `2` to trim the `Frame`s
   for the `stack_dump` function and its call to `frames()`,
   otherwise the default is `0` to use the supplied `Frame`s as is
+* `select`: if not `None`, select particular frames;
+  if `select` is a `str` it must be present in the frame filename;
+  otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
+
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
 
 *Release 20220429*:
 caller: return None if the stack index is out of range.
 
 *Release 20190812*:
@@ -79,7 +82,8 @@
 Add stack_dump().
 
 *Release 20150115*:
 PyPI metadata fixups.
 
 *Release 20150111*:
 Tag for initial PyPI release of cs.py.stack.
+
```

### Comparing `cs.py.stack-20220918/pyproject.toml` & `cs.py.stack-20240412/lib/python/cs.py.stack.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,82 +1,74 @@
-[project]
-name = "cs.py.stack"
-description = "Convenience functions for the python execution stack."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = []
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 2",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20220918"
+Metadata-Version: 2.1
+Name: cs.py.stack
+Version: 20240412
+Summary: Convenience functions for the python execution stack.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 I find the supplied python traceback facilities quite awkward.
 These functions provide convenient facilities.
 
-*Latest release 20220918*:
-caller(): return None if the frame offset is out of range.
+*Latest release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
 
 ## Function `caller(frame_index=-3)`
 
 Return the `Frame` of the caller's caller.
 Returns `None` if `frame_index` is out of range.
 
 Useful `frame_index` values:
 * `-1`: caller, this function
 * `-2`: invoker, who wants to know the caller
 * `-3`: the calling function of the invoker
 
 The default `from_index` value is `-3`.
 
-## Class `Frame(Frame, builtins.tuple)`
-
-A `namedtuple` for stack frame contents.
-
 ## Function `frames()`
 
 Return the current stack as a list of `Frame` objects.
 
-## Function `stack_dump(fp=None, indent=0, Fs=None, skip=None)`
+## Function `stack_dump(f=None, indent=0, frames=None, skip=None, select=None, format_frame=None)`
 
-Recite current or supplied stack to `fp`, default `sys.stderr`.
+Recite current or supplied stack to `f`, default `sys.stderr`.
 
 Parameters:
-* `fp`: the output file object, default `sys.stderr`
+* `f`: the output file object, default `sys.stderr`
 * `indent`: how many spaces to indent the stack lines, default `0`
-* `Fs`: the stack `Frame`s to write,
+* `frames`: the stack `Frame`s to write,
   default obtained from the current stack
-* `skip`: the number of `Frame`s to trim from the end of `Fs`;
-  if `Fs` is `None` this defaults to `2` to trim the `Frame`s
+* `skip`: the number of `Frame`s to trim from the end of `frames`;
+  if `frames` is `None` this defaults to `2` to trim the `Frame`s
   for the `stack_dump` function and its call to `frames()`,
   otherwise the default is `0` to use the supplied `Frame`s as is
+* `select`: if not `None`, select particular frames;
+  if `select` is a `str` it must be present in the frame filename;
+  otherwise `select(frame)` must be true
 
 # Release Log
 
 
 
+*Release 20240412*:
+* stack_dump: new select parameter to pick interesting frames for the listing.
+* Provide StackSummary and FrameSummary if Python too old.
+
 *Release 20220918*:
 caller(): return None if the frame offset is out of range.
 
 *Release 20220429*:
 caller: return None if the stack index is out of range.
 
 *Release 20190812*:
@@ -89,17 +81,9 @@
 *Release 20160827*:
 Add stack_dump().
 
 *Release 20150115*:
 PyPI metadata fixups.
 
 *Release 20150111*:
-Tag for initial PyPI release of cs.py.stack."""
-content-type = "text/markdown"
+Tag for initial PyPI release of cs.py.stack.
 
-[build-system]
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-build-backend = "setuptools.build_meta"
```

