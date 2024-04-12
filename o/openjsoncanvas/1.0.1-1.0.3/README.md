# Comparing `tmp/openjsoncanvas-1.0.1.tar.gz` & `tmp/openjsoncanvas-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-1.0.1.tar` & `openjsoncanvas-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.1/LICENSE
--rw-r--r--   0        0        0     2207 2024-04-12 13:30:02.375683 openjsoncanvas-1.0.1/README
--rw-r--r--   0        0        0     4799 2024-04-12 14:04:05.401592 openjsoncanvas-1.0.1/openjsoncanvas.py
--rw-r--r--   0        0        0      368 2024-04-12 13:08:22.206321 openjsoncanvas-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      321 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2207 2024-04-12 13:30:02.375683 openjsoncanvas-1.0.3/README
+-rw-r--r--   0        0        0     4801 2024-04-12 14:29:10.899541 openjsoncanvas-1.0.3/openjsoncanvas.py
+-rw-r--r--   0        0        0      426 2024-04-12 14:28:41.830459 openjsoncanvas-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.3/PKG-INFO
```

### Comparing `openjsoncanvas-1.0.1/LICENSE` & `openjsoncanvas-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.1/README` & `openjsoncanvas-1.0.3/README`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.1/openjsoncanvas.py` & `openjsoncanvas-1.0.3/openjsoncanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import dataclasses
 import json
 import pathlib
 import re
 import typing
 import functools
 import pprint
-__version__: str = '1.0.1'
+__version__: str = '1.0.3'
 
 camel_to_name = lambda x: re.sub(r'(?<!^)(?=[A-Z])', '_', x).lower()
 
 @functools.lru_cache
 def get_leaf_subclass(cls, name):
     if cls.__subclasses__():
         for subcls in cls.__subclasses__():
@@ -133,8 +133,8 @@
         return f'Canvas(\n  nodes=\n{nodes}\n  ,\n  edges=\n{edges}\n  \n)'
 
     
 if __name__ == '__main__':
     path = r"G:\vault\Wiki\Untitled.canvas"
     #canvas = Canvas.from_file(path)
     #print(canvas)
-    print(json.load(open(path)))
+    print(json.load(open(path)))
```

