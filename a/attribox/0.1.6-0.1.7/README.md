# Comparing `tmp/attribox-0.1.6.tar.gz` & `tmp/attribox-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribox-0.1.6.tar", last modified: Wed Apr 10 09:06:35 2024, max compression
+gzip compressed data, was "attribox-0.1.7.tar", last modified: Fri Apr 12 16:39:41 2024, max compression
```

## Comparing `attribox-0.1.6.tar` & `attribox-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-10 09:06:23.000000 attribox-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-10 09:06:35.528988 attribox-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-10 09:06:23.000000 attribox-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-10 09:06:32.000000 attribox-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-10 09:06:35.528988 attribox-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.524988 attribox-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/src/attribox/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_abstract_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_attri_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_delayed_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_this_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-10 09:06:23.000000 attribox-0.1.6/src/attribox/_typed_descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 09:06:35.528988 attribox-0.1.6/src/attribox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 09:06:35.000000 attribox-0.1.6/src/attribox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:39:41.141435 attribox-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 16:39:25.000000 attribox-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-12 16:39:41.141435 attribox-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-12 16:39:25.000000 attribox-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-12 16:39:37.000000 attribox-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-12 16:39:41.141435 attribox-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:39:41.137435 attribox-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:39:41.141435 attribox-0.1.7/src/attribox/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 16:39:25.000000 attribox-0.1.7/src/attribox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-12 16:39:25.000000 attribox-0.1.7/src/attribox/_abstract_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-12 16:39:26.000000 attribox-0.1.7/src/attribox/_attri_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-12 16:39:26.000000 attribox-0.1.7/src/attribox/_delayed_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-12 16:39:26.000000 attribox-0.1.7/src/attribox/_this_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-12 16:39:26.000000 attribox-0.1.7/src/attribox/_typed_descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:39:41.141435 attribox-0.1.7/src/attribox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-12 16:39:41.000000 attribox-0.1.7/src/attribox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 16:39:41.000000 attribox-0.1.7/src/attribox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:39:41.000000 attribox-0.1.7/src/attribox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 16:39:41.000000 attribox-0.1.7/src/attribox.egg-info/top_level.txt
```

### Comparing `attribox-0.1.6/LICENSE` & `attribox-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/PKG-INFO` & `attribox-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.6
+Version: 0.1.7
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
```

### Comparing `attribox-0.1.6/README.md` & `attribox-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/pyproject.toml` & `attribox-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=68.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "attribox"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Allows for deferred instantiation of class attributes."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `attribox-0.1.6/setup.cfg` & `attribox-0.1.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = attribox
-version = 0.1.6
+version = 0.1.7
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = Class attributes as descriptors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AsgerJon/attribox
 classifiers =
```

### Comparing `attribox-0.1.6/src/attribox/__init__.py` & `attribox-0.1.7/src/attribox/__init__.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/src/attribox/_abstract_descriptor.py` & `attribox-0.1.7/src/attribox/_abstract_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/src/attribox/_attri_box.py` & `attribox-0.1.7/src/attribox/_attri_box.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 """AttriBox subclasses the TypedDescriptor class and incorporates
 syntactic sugar for setting the inner class, and for the inner object
 creation. """
 #  MIT Licence
 #  Copyright (c) 2024 Asger Jon Vistisen
 from __future__ import annotations
 
-from typing import Self, Any
+import sys
+from typing import Any
 
 from icecream import ic
 from vistutils.text import monoSpace
 from vistutils.waitaminute import typeMsg
 
 from attribox import TypedDescriptor, scope, this
 
+if sys.version_info.minor < 11:
+  from typing_extensions import Self
+else:
+  from typing import Self
+
+
 ic.configureOutput(includeContext=True, )
 
 
 class AttriBox(TypedDescriptor):
   """AttriBox subclasses the TypedDescriptor class and incorporates
   syntactic sugar for setting the inner class, and for the inner object
   creation. """
```

### Comparing `attribox-0.1.6/src/attribox/_delayed_descriptor.py` & `attribox-0.1.7/src/attribox/_delayed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/src/attribox/_this_scope.py` & `attribox-0.1.7/src/attribox/_this_scope.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/src/attribox/_typed_descriptor.py` & `attribox-0.1.7/src/attribox/_typed_descriptor.py`

 * *Files identical despite different names*

### Comparing `attribox-0.1.6/src/attribox.egg-info/PKG-INFO` & `attribox-0.1.7/src/attribox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribox
-Version: 0.1.6
+Version: 0.1.7
 Summary: Allows for deferred instantiation of class attributes.
 Home-page: https://github.com/AsgerJon/attribox
 Author: Asger Jon Vistisen
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/attribox
 Project-URL: Bug Tracker, https://github.com/AsgerJon/attribox
 Classifier: Programming Language :: Python :: 3
```

