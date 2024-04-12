# Comparing `tmp/openjsoncanvas-1.0.3.tar.gz` & `tmp/openjsoncanvas-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-1.0.3.tar` & `openjsoncanvas-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.3/LICENSE
--rw-r--r--   0        0        0     2207 2024-04-12 13:30:02.375683 openjsoncanvas-1.0.3/README
--rw-r--r--   0        0        0     4801 2024-04-12 14:29:10.899541 openjsoncanvas-1.0.3/openjsoncanvas.py
--rw-r--r--   0        0        0      426 2024-04-12 14:28:41.830459 openjsoncanvas-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1939 2024-04-12 14:39:25.865517 openjsoncanvas-1.0.4/README
+-rw-r--r--   0        0        0     4801 2024-04-12 14:39:25.872516 openjsoncanvas-1.0.4/openjsoncanvas.py
+-rw-r--r--   0        0        0      426 2024-04-12 14:28:41.830459 openjsoncanvas-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.4/PKG-INFO
```

### Comparing `openjsoncanvas-1.0.3/LICENSE` & `openjsoncanvas-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.3/README` & `openjsoncanvas-1.0.4/README`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-Based on your provided Python implementation of the JsonCanvas format, here's a detailed README file. This README includes an overview, installation instructions, usage examples, and additional details that may be helpful for users of your project.
-
-```markdown
 # JsonCanvas Python Implementation
 
 This project provides a Python implementation of the [JsonCanvas format](https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md), designed to enable the creation, manipulation, and serialization of a structured canvas representation. It is built using Python's `dataclasses` for easy data management and supports various node types including Text, File, Link, Group, and Edge elements.
 
 ## Features
 
 - Define and manipulate canvas elements like Nodes and Edges.
@@ -58,8 +55,7 @@
 ## Contributing
 
 Contributions are welcome! Feel free to open issues or submit pull requests to our repository.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
-```
```

### Comparing `openjsoncanvas-1.0.3/openjsoncanvas.py` & `openjsoncanvas-1.0.4/openjsoncanvas.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import dataclasses
 import json
 import pathlib
 import re
 import typing
 import functools
 import pprint
-__version__: str = '1.0.3'
+__version__: str = '1.0.4'
 
 camel_to_name = lambda x: re.sub(r'(?<!^)(?=[A-Z])', '_', x).lower()
 
 @functools.lru_cache
 def get_leaf_subclass(cls, name):
     if cls.__subclasses__():
         for subcls in cls.__subclasses__():
```

### Comparing `openjsoncanvas-1.0.3/PKG-INFO` & `openjsoncanvas-1.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 Metadata-Version: 2.1
 Name: openjsoncanvas
-Version: 1.0.3
+Version: 1.0.4
 Summary: A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 Author: Alyce Osbourne
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/AlyceOsbourne/openjsoncanvas
 
-Based on your provided Python implementation of the JsonCanvas format, here's a detailed README file. This README includes an overview, installation instructions, usage examples, and additional details that may be helpful for users of your project.
-
-```markdown
 # JsonCanvas Python Implementation
 
 This project provides a Python implementation of the [JsonCanvas format](https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md), designed to enable the creation, manipulation, and serialization of a structured canvas representation. It is built using Python's `dataclasses` for easy data management and supports various node types including Text, File, Link, Group, and Edge elements.
 
 ## Features
 
 - Define and manipulate canvas elements like Nodes and Edges.
@@ -67,8 +64,8 @@
 ## Contributing
 
 Contributions are welcome! Feel free to open issues or submit pull requests to our repository.
 
 ## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
-```
+
```

