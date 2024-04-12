# Comparing `tmp/objx-65.tar.gz` & `tmp/objx-70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "objx-65.tar", last modified: Wed Mar 20 12:34:02 2024, max compression
+gzip compressed data, was "objx-70.tar", last modified: Fri Apr 12 14:06:45 2024, max compression
```

## Comparing `objx-65.tar` & `objx-70.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-20 12:34:02.248506 objx-65/
--rw-r--r--   0 bart      (1000) bart      (1000)     1405 2024-03-20 12:34:02.248506 objx-65/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      880 2024-03-20 12:17:38.000000 objx-65/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-20 12:34:02.244506 objx-65/objx/
--rw-r--r--   0 bart      (1000) bart      (1000)     5315 2024-03-20 12:16:44.000000 objx-65/objx/__init__.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-03-20 12:34:02.248506 objx-65/objx.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     1405 2024-03-20 12:34:02.000000 objx-65/objx.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      186 2024-03-20 12:34:02.000000 objx-65/objx.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-20 12:34:02.000000 objx-65/objx.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-03-20 12:34:02.000000 objx-65/objx.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-03-20 12:34:02.000000 objx-65/objx.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      875 2024-03-18 08:20:23.000000 objx-65/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-03-20 12:34:02.248506 objx-65/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-18 08:20:23.000000 objx-65/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1406 2024-04-12 14:06:45.108174 objx-70/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      880 2024-04-06 11:08:24.000000 objx-70/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/objx/
+-rw-r--r--   0 bart      (1000) bart      (1000)      664 2024-04-12 14:05:42.000000 objx-70/objx/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-12 14:05:42.000000 objx-70/objx/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-12 14:05:42.000000 objx-70/objx/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3261 2024-04-12 14:05:42.000000 objx-70/objx/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      731 2024-04-12 14:05:42.000000 objx-70/objx/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-12 14:06:45.108174 objx-70/objx.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     1406 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      249 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        5 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-12 14:06:45.000000 objx-70/objx.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-12 14:06:38.000000 objx-70/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-12 14:06:45.108174 objx-70/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-06 11:08:24.000000 objx-70/setup.py
```

### Comparing `objx-65/PKG-INFO` & `objx-70/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: objx
-Version: 65
+Version: 70
 Summary: objects library
-Author-email: xobjectz <objx@proton.me>
+Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objx
 Project-URL: bugs, https://github.com/xobjectz/objx/issues
 Project-URL: source, https://github.com/xobjectz/objx
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
```

### Comparing `objx-65/README.rst` & `objx-70/README.rst`

 * *Files identical despite different names*

### Comparing `objx-65/objx/__init__.py` & `objx-70/objx/object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,57 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0613,E0101
+# pylint: disable=C,R,W0105
 
 
-"a clean namespace"
+"objects"
 
 
 import json
 import os
 import pathlib
 import _thread
 
 
 disklock = _thread.allocate_lock()
 
 
-def cdir(pth):
-    if os.path.exists(pth):
-        return
-    pth = pathlib.Path(pth)
-    os.makedirs(pth, exist_ok=True)
-
-
 class Object:
 
+    "Object"
+
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
     def __len__(self):
         return len(self.__dict__)
 
     def __str__(self):
         return str(self.__dict__)
 
 
 def construct(obj, *args, **kwargs):
+    "construct an object from provided arguments."
     if args:
         val = args[0]
         if isinstance(val, zip):
             update(obj, dict(val))
         elif isinstance(val, dict):
             update(obj, val)
         elif isinstance(val, Object):
             update(obj, vars(val))
     if kwargs:
         update(obj, kwargs)
 
 
 def edit(obj, setter, skip=False):
+    "edit an object from provided dict/dict-like."
     for key, val in items(setter):
         if skip and val == "":
             continue
         try:
             setattr(obj, key, int(val))
             continue
         except ValueError:
@@ -69,14 +66,15 @@
         elif val in ["False", "false"]:
             setattr(obj, key, False)
         else:
             setattr(obj, key, val)
 
 
 def fmt(obj, args=None, skip=None, plain=False):
+    "format an object to a printable string."
     if args is None:
         args = keys(obj)
     if skip is None:
         skip = []
     txt = ""
     for key in args:
         if key.startswith("__"):
@@ -92,141 +90,172 @@
             txt += f'{key}="{value}" '
         else:
             txt += f"{key}={value} "
     return txt.strip()
 
 
 def fqn(obj):
+    "return full qualified name of an object."
     kin = str(type(obj)).split()[-1][1:-2]
     if kin == "type":
         kin = obj.__name__
     return kin
 
 
 def items(obj):
+    "return the items of an object."
     if isinstance(obj, type({})):
         return obj.items()
     return obj.__dict__.items()
 
 
 def keys(obj):
+    "return keys of an object."
     if isinstance(obj, type({})):
         return obj.keys()
     return list(obj.__dict__.keys())
 
 
 def read(obj, pth):
+    "read an object from file path."
     with disklock:
         with open(pth, 'r', encoding='utf-8') as ofile:
             update(obj, load(ofile))
 
 
 def search(obj, selector):
+    "check if object matches provided values."
     res = False
     if not selector:
         return True
     for key, value in items(selector):
         val = getattr(obj, key, None)
         if str(value).lower() in str(val).lower():
             res = True
         else:
             res = False
             break
     return res
 
 
 def update(obj, data, empty=True):
+    "update an object."
     for key, value in items(data):
         if empty and not value:
             continue
         setattr(obj, key, value)
 
 
 def values(obj):
+    "return values of an object."
     return obj.__dict__.values()
 
 
 def write(obj, pth):
+    "write an object to disk."
     with disklock:
         cdir(os.path.dirname(pth))
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
+
+    "ObjectDecoder"
+
     def __init__(self, *args, **kwargs):
-        return json.JSONDecoder.__init__(self, *args)
+        json.JSONDecoder.__init__(self, *args, **kwargs)
 
     def decode(self, s, _w=None):
+        "decoding string to object."
         val = json.JSONDecoder.decode(self, s)
         if not val:
             val = {}
         return hook(val)
 
     def raw_decode(self, s, idx=0):
+        "decode partial string to object."
         return json.JSONDecoder.raw_decode(self, s, idx)
 
 
 def hook(objdict, typ=None):
+    "construct object from dict."
     if typ:
         obj = typ()
     else:
         obj = Object()
     construct(obj, objdict)
     return obj
 
 
 def load(fpt, *args, **kw):
+    "load object from file."
     kw["cls"] = ObjectDecoder
     kw["object_hook"] = hook
     return json.load(fpt, *args, **kw)
 
 
 def loads(string, *args, **kw):
+    "load object from string."
     kw["cls"] = ObjectDecoder
     kw["object_hook"] = hook
     return json.loads(string, *args, **kw)
 
 
 class ObjectEncoder(json.JSONEncoder):
 
+    "ObjectEncoder"
+
     def __init__(self, *args, **kwargs):
-        return json.JSONEncoder.__init__(self, *args, **kwargs)
+        json.JSONEncoder.__init__(self, *args, **kwargs)
 
     def default(self, o):
+        "return stringable value."
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
             return vars(o)
         if isinstance(o, list):
             return iter(o)
         if isinstance(o, (type(str), type(True), type(False), type(int), type(float))):
             return o
         try:
             return json.JSONEncoder.default(self, o)
         except TypeError:
             return o.__dict__
 
     def encode(self, o) -> str:
+        "encode object to string."
         return json.JSONEncoder.encode(self, o)
 
     def iterencode(self, o, _one_shot=False):
+        "loop over object to encode to string."
         return json.JSONEncoder.iterencode(self, o, _one_shot)
 
 
 def dump(*args, **kw):
+    "dump object to file."
     kw["cls"] = ObjectEncoder
     return json.dump(*args, **kw)
 
 
 def dumps(*args, **kw):
+    "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
+def cdir(pth):
+    "create directory."
+    if os.path.exists(pth):
+        return
+    pth = pathlib.Path(pth)
+    os.makedirs(pth, exist_ok=True)
+
+
 "interface"
 
 
 def __dir__():
     return (
         'Object',
         'construct',
```

### Comparing `objx-65/objx.egg-info/PKG-INFO` & `objx-70/objx.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: objx
-Version: 65
+Version: 70
 Summary: objects library
-Author-email: xobjectz <objx@proton.me>
+Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/objx
 Project-URL: bugs, https://github.com/xobjectz/objx/issues
 Project-URL: source, https://github.com/xobjectz/objx
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Public Domain
 Classifier: Operating System :: Unix
```

### Comparing `objx-65/pyproject.toml` & `objx-70/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "objx"
 description = "objects library"
-version = "65"
+version = "70"
 authors = [
-    {name = "xobjectz", email = "objx@proton.me"},
+    {name = "Bart Thate", email = "bthate@dds.nl"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
     'License :: Public Domain',
     'Operating System :: Unix',
```

