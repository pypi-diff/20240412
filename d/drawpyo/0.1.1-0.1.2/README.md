# Comparing `tmp/drawpyo-0.1.1.tar.gz` & `tmp/drawpyo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drawpyo-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "drawpyo-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `drawpyo-0.1.1.tar` & `drawpyo-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     4781 2024-03-21 04:48:09.875927 drawpyo-0.1.1/README.md
--rw-r--r--   0        0        0      877 2024-04-02 23:44:43.159162 drawpyo-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      150 2024-04-02 23:44:43.159162 drawpyo-0.1.1/src/drawpyo/__init__.py
--rw-r--r--   0        0        0       99 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram/__init__.py
--rw-r--r--   0        0        0    10390 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram/base_diagram.py
--rw-r--r--   0        0        0    19912 2024-04-02 23:44:43.159162 drawpyo-0.1.1/src/drawpyo/diagram/edges.py
--rw-r--r--   0        0        0    20577 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram/objects.py
--rw-r--r--   0        0        0     6097 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram/text_format.py
--rw-r--r--   0        0        0       49 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram_types/__init__.py
--rw-r--r--   0        0        0     1042 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram_types/class_diagram.py
--rw-r--r--   0        0        0    20255 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/diagram_types/tree.py
--rw-r--r--   0        0        0     4551 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/file.py
--rw-r--r--   0        0        0     2176 2024-04-02 23:44:43.159162 drawpyo-0.1.1/src/drawpyo/formatting_database/edge_styles.toml
--rw-r--r--   0        0        0      217 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/formatting_database/line_styles.toml
--rw-r--r--   0        0        0     4839 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/page.py
--rw-r--r--   0        0        0     4737 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/shape_libraries/flowchart.toml
--rw-r--r--   0        0        0     2716 2024-04-02 00:14:21.541936 drawpyo-0.1.1/src/drawpyo/shape_libraries/general.toml
--rw-r--r--   0        0        0     3939 2024-04-02 23:44:43.159162 drawpyo-0.1.1/src/drawpyo/xml_base.py
--rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 drawpyo-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4781 2024-03-21 04:48:09.875927 drawpyo-0.1.2/README.md
+-rw-r--r--   0        0        0      877 2024-04-02 23:44:43.159162 drawpyo-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      150 2024-04-12 01:57:49.929102 drawpyo-0.1.2/src/drawpyo/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/__init__.py
+-rw-r--r--   0        0        0    10644 2024-04-12 01:56:48.484739 drawpyo-0.1.2/src/drawpyo/diagram/base_diagram.py
+-rw-r--r--   0        0        0    19912 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/diagram/edges.py
+-rw-r--r--   0        0        0    20577 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/objects.py
+-rw-r--r--   0        0        0     6097 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram/text_format.py
+-rw-r--r--   0        0        0       49 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/__init__.py
+-rw-r--r--   0        0        0     1042 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/class_diagram.py
+-rw-r--r--   0        0        0    20255 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/diagram_types/tree.py
+-rw-r--r--   0        0        0     4551 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/file.py
+-rw-r--r--   0        0        0     2176 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/formatting_database/edge_styles.toml
+-rw-r--r--   0        0        0      217 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/formatting_database/line_styles.toml
+-rw-r--r--   0        0        0     4839 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/page.py
+-rw-r--r--   0        0        0     4737 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/shape_libraries/flowchart.toml
+-rw-r--r--   0        0        0     2716 2024-04-02 00:14:21.541936 drawpyo-0.1.2/src/drawpyo/shape_libraries/general.toml
+-rw-r--r--   0        0        0     3939 2024-04-02 23:44:43.159162 drawpyo-0.1.2/src/drawpyo/xml_base.py
+-rw-r--r--   0        0        0     5442 1970-01-01 00:00:00.000000 drawpyo-0.1.2/PKG-INFO
```

### Comparing `drawpyo-0.1.1/README.md` & `drawpyo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/pyproject.toml` & `drawpyo-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram/base_diagram.py` & `drawpyo-0.1.2/src/drawpyo/diagram/base_diagram.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,20 @@
         import tomllib
 
         with open(file_name, "rb") as f:
             data = tomllib.load(f)
 
     for obj in data.values():
         if "inherit" in obj:
-            obj.update(data[obj["inherit"]])
+            # To make the inheritor styles take precedence the inherited
+            # object needs to be updated not the other way around. The copy is
+            # created, updated, and replaced.
+            new_obj = data[obj["inherit"]]
+            new_obj.update(obj)
+            obj = new_obj
 
     return data
 
 
 def style_str_from_dict(style_dict):
     """
     This function returns a concatenated style string from a style dictionary.
```

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram/edges.py` & `drawpyo-0.1.2/src/drawpyo/diagram/edges.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram/objects.py` & `drawpyo-0.1.2/src/drawpyo/diagram/objects.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram/text_format.py` & `drawpyo-0.1.2/src/drawpyo/diagram/text_format.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram_types/class_diagram.py` & `drawpyo-0.1.2/src/drawpyo/diagram_types/class_diagram.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/diagram_types/tree.py` & `drawpyo-0.1.2/src/drawpyo/diagram_types/tree.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/file.py` & `drawpyo-0.1.2/src/drawpyo/file.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/formatting_database/edge_styles.toml` & `drawpyo-0.1.2/src/drawpyo/formatting_database/edge_styles.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/page.py` & `drawpyo-0.1.2/src/drawpyo/page.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/shape_libraries/flowchart.toml` & `drawpyo-0.1.2/src/drawpyo/shape_libraries/flowchart.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/shape_libraries/general.toml` & `drawpyo-0.1.2/src/drawpyo/shape_libraries/general.toml`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/src/drawpyo/xml_base.py` & `drawpyo-0.1.2/src/drawpyo/xml_base.py`

 * *Files identical despite different names*

### Comparing `drawpyo-0.1.1/PKG-INFO` & `drawpyo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drawpyo
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python library for programmatically generating Draw.io charts.
 Keywords: draw.io,diagrams.net,diagrams
 Author-email: Xander Cesari <xander@merriman.industries>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```
