# Comparing `tmp/openjsoncanvas-1.0.5.tar.gz` & `tmp/openjsoncanvas-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openjsoncanvas-1.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openjsoncanvas-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openjsoncanvas-1.0.5.tar` & `openjsoncanvas-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-1.0.5/LICENSE
--rw-r--r--   0        0        0     1937 2024-04-12 14:50:57.072592 openjsoncanvas-1.0.5/README
--rw-r--r--   0        0        0     4801 2024-04-12 14:51:16.153080 openjsoncanvas-1.0.5/openjsoncanvas.py
--rw-r--r--   0        0        0      426 2024-04-12 14:28:41.830459 openjsoncanvas-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     2239 1970-01-01 00:00:00.000000 openjsoncanvas-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-12 12:47:53.175260 openjsoncanvas-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1937 2024-04-12 14:50:57.072592 openjsoncanvas-2.0.0/README
+-rw-r--r--   0        0        0     3460 2024-04-12 16:38:06.883788 openjsoncanvas-2.0.0/openjsoncanvas.py
+-rw-r--r--   0        0        0      468 2024-04-12 16:39:57.422261 openjsoncanvas-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-12 16:05:15.952512 openjsoncanvas-2.0.0/run.py
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 openjsoncanvas-2.0.0/PKG-INFO
```

### Comparing `openjsoncanvas-1.0.5/LICENSE` & `openjsoncanvas-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.5/README` & `openjsoncanvas-2.0.0/README`

 * *Files identical despite different names*

### Comparing `openjsoncanvas-1.0.5/PKG-INFO` & `openjsoncanvas-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: openjsoncanvas
-Version: 1.0.5
+Version: 2.0.0
 Summary: A python implementation of the JsonCanvas format: https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md
 Author: Alyce Osbourne
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: pydantic
 Project-URL: Home, https://github.com/AlyceOsbourne/openjsoncanvas
 
 # JsonCanvas Python Implementation
 
 This project provides a Python implementation of the [JsonCanvas format](https://github.com/obsidianmd/jsoncanvas/blob/main/spec/1.0.md), designed to enable the creation, manipulation, and serialization of a structured canvas representation. It is built using Python's `dataclasses` for easy data management and supports various node types including Text, File, Link, Group, and Edge elements.
 
 ## Features
```

