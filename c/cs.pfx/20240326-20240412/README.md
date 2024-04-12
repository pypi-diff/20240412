# Comparing `tmp/cs.pfx-20240326.tar.gz` & `tmp/cs.pfx-20240412.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.pfx-20240326.tar", last modified: Tue Mar 26 06:38:30 2024, max compression
+gzip compressed data, was "cs.pfx-20240412.tar", last modified: Fri Apr 12 02:40:15 2024, max compression
```

## Comparing `cs.pfx-20240326.tar` & `cs.pfx-20240412.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:38:30.148192 cs.pfx-20240326/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-26 06:38:02.000000 cs.pfx-20240326/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    12069 2024-03-26 06:38:30.147872 cs.pfx-20240326/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    11277 2024-03-26 06:38:11.000000 cs.pfx-20240326/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:38:30.143521 cs.pfx-20240326/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:38:30.143947 cs.pfx-20240326/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:38:30.145754 cs.pfx-20240326/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    21725 2024-03-26 06:37:49.000000 cs.pfx-20240326/lib/python/cs/pfx.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-26 06:38:30.147432 cs.pfx-20240326/lib/python/cs.pfx.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    12069 2024-03-26 06:38:29.000000 cs.pfx-20240326/lib/python/cs.pfx.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-03-26 06:38:30.000000 cs.pfx-20240326/lib/python/cs.pfx.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-26 06:38:29.000000 cs.pfx-20240326/lib/python/cs.pfx.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       71 2024-03-26 06:38:29.000000 cs.pfx-20240326/lib/python/cs.pfx.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-26 06:38:30.000000 cs.pfx-20240326/lib/python/cs.pfx.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    12505 2024-03-26 06:38:28.000000 cs.pfx-20240326/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-26 06:38:30.148292 cs.pfx-20240326/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:40:15.238829 cs.pfx-20240412/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 02:39:46.000000 cs.pfx-20240412/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12047 2024-04-12 02:40:15.238437 cs.pfx-20240412/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    11255 2024-04-12 02:39:55.000000 cs.pfx-20240412/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:40:15.234340 cs.pfx-20240412/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:40:15.234657 cs.pfx-20240412/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:40:15.236164 cs.pfx-20240412/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    21752 2024-04-12 02:39:35.000000 cs.pfx-20240412/lib/python/cs/pfx.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 02:40:15.237990 cs.pfx-20240412/lib/python/cs.pfx.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12047 2024-04-12 02:40:14.000000 cs.pfx-20240412/lib/python/cs.pfx.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      261 2024-04-12 02:40:15.000000 cs.pfx-20240412/lib/python/cs.pfx.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 02:40:14.000000 cs.pfx-20240412/lib/python/cs.pfx.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       71 2024-04-12 02:40:15.000000 cs.pfx-20240412/lib/python/cs.pfx.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 02:40:15.000000 cs.pfx-20240412/lib/python/cs.pfx.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    12483 2024-04-12 02:40:13.000000 cs.pfx-20240412/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 02:40:15.238932 cs.pfx-20240412/setup.cfg
```

### Comparing `cs.pfx-20240326/PKG-INFO` & `cs.pfx-20240412/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.pfx
-Version: 20240326
+Version: 20240412
 Summary: Easy context prefixes for messages.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,17 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Dynamic message prefixes providing execution context.
 
-*Latest release 20240326*:
-* Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
-* Pfx.prefixify_exception: do not modify .message if it is not a string.
+*Latest release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -268,14 +267,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
+
 *Release 20240326*:
 * Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
 * Pfx.prefixify_exception: do not modify .message if it is not a string.
 
 *Release 20230604*:
 @pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
```

### Comparing `cs.pfx-20240326/README.md` & `cs.pfx-20240412/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Dynamic message prefixes providing execution context.
 
-*Latest release 20240326*:
-* Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
-* Pfx.prefixify_exception: do not modify .message if it is not a string.
+*Latest release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -249,14 +248,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
+
 *Release 20240326*:
 * Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
 * Pfx.prefixify_exception: do not modify .message if it is not a string.
 
 *Release 20230604*:
 @pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
```

### Comparing `cs.pfx-20240326/lib/python/cs/pfx.py` & `cs.pfx-20240412/lib/python/cs/pfx.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 from cs.deco import decorator, contextdecorator, fmtdoc, logging_wrapper
 from cs.py.func import funcname, func_a_kw_fmt
 from cs.py3 import StringTypes, ustr, unicode
 
 from cs.x import X
 
-__version__ = '20240326'
+__version__ = '20240412'
 
 DISTINFO = {
     'description':
     "Easy context prefixes for messages.",
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
@@ -268,15 +268,15 @@
     '''
     cls._push(cls(msg, *a))
 
   def __exit__(self, exc_type, exc_value, _):
     _state = self._state
     if exc_value is not None:
       try:
-        exc_value._pfx_prefix
+        exc_value._pfx_prefix  # noqa: B018
       except AttributeError:
         exc_value._pfx_prefix = self._state.prefix
         # prevent outer Pfx wrappers from hacking stuff as well
         # now hack the exception attributes
         if not self.prefixify_exception(exc_value):
           True or print(
               "warning: %s: %s:%s: message not prefixed: dir=%r" % (
@@ -332,15 +332,15 @@
     return (
         current_prefix + DEFAULT_SEPARATOR +
         ustr(text, errors='replace'
              ).replace('\n', '\n  ' + current_prefix + DEFAULT_SEPARATOR)
     )
 
   @classmethod
-  def prefixify_exception(cls, e):
+  def prefixify_exception(cls, e):  # noqa: C901
     ''' Modify the supplied exception `e` with the current prefix.
         Return `True` if modified, `False` if unable to modify.
     '''
     current_prefix = cls._state.prefix
     did_prefix = False
     for attr in 'args', 'message', 'msg', 'reason', 'strerror':
       try:
@@ -352,15 +352,15 @@
       ovalue = value
       # special case various known exception type attributes
       if attr == 'args' and isinstance(e, OSError):
         # prefixify the first string
         value = list(value)
         for i, v in enumerate(value):
           if isinstance(v, str):
-            value = cls.prefixify(value)
+            value[i] = cls.prefixify(v)
             did_prefix = True
             break
         value = tuple(value)
       elif attr == 'args' and isinstance(e, LookupError):
         if (isinstance(value, tuple) and value):
           value0 = value[0]
           if (isinstance(value0, str) and value0.startswith("'")
```

### Comparing `cs.pfx-20240326/lib/python/cs.pfx.egg-info/PKG-INFO` & `cs.pfx-20240412/lib/python/cs.pfx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.pfx
-Version: 20240326
+Version: 20240412
 Summary: Easy context prefixes for messages.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,17 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Dynamic message prefixes providing execution context.
 
-*Latest release 20240326*:
-* Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
-* Pfx.prefixify_exception: do not modify .message if it is not a string.
+*Latest release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -268,14 +267,17 @@
 
     XX("NOTE!", "some message")
 
 # Release Log
 
 
 
+*Release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
+
 *Release 20240326*:
 * Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
 * Pfx.prefixify_exception: do not modify .message if it is not a string.
 
 *Release 20230604*:
 @pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
```

### Comparing `cs.pfx-20240326/pyproject.toml` & `cs.pfx-20240412/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,44 +5,43 @@
     { name = "Cameron Simpson", email = "cs@cskk.id.au" },
 ]
 keywords = [
     "python2",
     "python3",
 ]
 dependencies = [
-    "cs.deco>=20240326",
+    "cs.deco>=20240412",
     "cs.py.func>=20210913",
     "cs.py3>=20220523",
     "cs.x>=20240316",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 2",
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
 Dynamic message prefixes providing execution context.
 
-*Latest release 20240326*:
-* Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
-* Pfx.prefixify_exception: do not modify .message if it is not a string.
+*Latest release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
 
 The primary facility here is `Pfx`,
 a context manager which maintains a per thread stack of context prefixes.
 There are also decorators for functions.
 This stack is used to prefix logging messages and exception text with context.
 
 Usage is like this:
@@ -285,14 +284,17 @@
 
     XX(\"NOTE!\", \"some message\")
 
 # Release Log
 
 
 
+*Release 20240412*:
+Pfx.prefixify_exception: bugfix prefixification of sequences.
+
 *Release 20240326*:
 * Pfx.prefixify_exception: sanity check the types of the prefixed attributes, aids debugging.
 * Pfx.prefixify_exception: do not modify .message if it is not a string.
 
 *Release 20230604*:
 @pfx_method: handle methods with no __name__ (generally a misuse of the decorator).
```

