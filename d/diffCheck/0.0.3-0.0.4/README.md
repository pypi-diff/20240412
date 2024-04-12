# Comparing `tmp/diffCheck-0.0.3.tar.gz` & `tmp/diffCheck-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.3.tar", last modified: Wed Apr 10 15:22:46 2024, max compression
+gzip compressed data, was "diffCheck-0.0.4.tar", last modified: Fri Apr 12 13:41:26 2024, max compression
```

## Comparing `diffCheck-0.0.3.tar` & `diffCheck-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.862109 diffCheck-0.0.3/
--rw-rw-rw-   0        0        0      806 2024-04-10 15:22:46.861610 diffCheck-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-07 14:57:49.000000 diffCheck-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.839573 diffCheck-0.0.3/diffCheck/
--rw-rw-rw-   0        0        0       21 2024-04-09 13:29:53.000000 diffCheck-0.0.3/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     9485 2024-04-10 15:13:00.000000 diffCheck-0.0.3/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0     7622 2024-04-09 13:40:15.000000 diffCheck-0.0.3/diffCheck/df_joint_detector.py
--rw-rw-rw-   0        0        0     4604 2024-04-08 14:43:34.000000 diffCheck-0.0.3/diffCheck/df_transformations.py
--rw-rw-rw-   0        0        0     4166 2024-04-08 14:44:50.000000 diffCheck-0.0.3/diffCheck/df_util.py
--rw-rw-rw-   0        0        0     1065 2024-04-10 15:14:55.000000 diffCheck-0.0.3/diffCheck/diffCheck_app.py
--rw-rw-rw-   0        0        0      202 2024-04-10 11:03:44.000000 diffCheck-0.0.3/diffCheck/test.py
-drwxrwxrwx   0        0        0        0 2024-04-10 15:22:46.860109 diffCheck-0.0.3/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-10 15:22:46.000000 diffCheck-0.0.3/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 15:22:46.862610 diffCheck-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      739 2024-04-09 13:29:53.000000 diffCheck-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.776529 diffCheck-0.0.4/
+-rw-rw-rw-   0        0        0      806 2024-04-12 13:41:26.776031 diffCheck-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.761529 diffCheck-0.0.4/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-12 13:41:19.000000 diffCheck-0.0.4/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7680 2024-04-12 13:20:49.000000 diffCheck-0.0.4/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.4/diffCheck/df_util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 13:41:26.774034 diffCheck-0.0.4/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 13:41:26.000000 diffCheck-0.0.4/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 13:41:26.777033 diffCheck-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      739 2024-04-12 13:41:21.000000 diffCheck-0.0.4/setup.py
```

### Comparing `diffCheck-0.0.3/PKG-INFO` & `diffCheck-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.3
+Version: 0.0.4
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.3/diffCheck/df_geometries.py` & `diffCheck-0.0.4/diffCheck/df_geometries.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import Rhino
 import Rhino.Geometry as rg
 
 import xml.etree.ElementTree as ET
 from xml.dom.minidom import parseString
 
-from df_joint_detector import JointDetector
+import diffCheck.df_joint_detector
 
 
 @dataclass
 class DFVertex:
     """
     This class represents a vertex, a simple container with 3 coordinates
     """
@@ -183,15 +183,15 @@
 
     @classmethod
     def from_brep(cls, brep):
         """
         Create a DFBeam from a RhinoBrep object.
         It also removes duplicates and creates a list of unique faces.
         """
-        faces = JointDetector(brep).run()
+        faces = diffCheck.df_joint_detector.JointDetector(brep).run()
         faces = list(set(faces))
         beam = cls("Beam", faces)
         return beam
 
     def __repr__(self):
         return f"Beam: {self.name}, Faces: {len(self.faces)}"
```

### Comparing `diffCheck-0.0.3/diffCheck/df_joint_detector.py` & `diffCheck-0.0.4/diffCheck/df_joint_detector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import Rhino
 import scriptcontext as sc
 import Rhino.Geometry as rg
 
 import typing
 from dataclasses import dataclass
 
-import df_util
-import df_transformations
-from df_geometries import DFVertex, DFFace
-
+import diffCheck.df_util
+import diffCheck.df_transformations
+from diffCheck.df_geometries import DFFace
 
 @dataclass
 class JointDetector():
     """
     This class is responsible for detecting joints in a brep
     """
     brep : Rhino.Geometry.Brep
@@ -34,18 +33,18 @@
 
             :return: a list of faces from joins and faces
         """
         ############################################################################
         # 1. Bring to XY, mamke AABB and get negative boolean difference
         ############################################################################
         # bring to plane xy
-        x_form = df_transformations.pln_2_pln_world_transform(self.brep)
+        x_form = diffCheck.df_transformations.pln_2_pln_world_transform(self.brep)
 
         # reverse the transformation
-        x_form_back = df_transformations.get_inverse_transformation(x_form)
+        x_form_back = diffCheck.df_transformations.get_inverse_transformation(x_form)
 
         # compute the bounding box and inflate to include butt joints typo
         bbox = self.brep.GetBoundingBox(True)
         diagonal = bbox.Diagonal
         scaling_factor = diagonal.Length / 10
         bbox.Inflate(scaling_factor, 0, 0)
         bbox_b = bbox.ToBrep()
@@ -70,15 +69,15 @@
             for f in b.Faces:
                 f_brep = f.ToBrep()
                 f = f_brep.Faces[0]
                 if not f.IsPlanar():
                     is_cut = False
                     is_hole = True
 
-                    b_faces = df_util.explode_brep(b)
+                    b_faces = diffCheck.df_util.explode_brep(b)
                     for b_face in b_faces:
                         if b_face.Faces[0].IsPlanar():
                             b_face_edges = b_face.Edges
                             for b_face_edge in b_face_edges:
                                 if not b_face_edge.IsClosed:
                                     is_mix = True
                                     is_hole = False
@@ -106,15 +105,15 @@
             # (1) explode
             # (2) seperate in tow list flat surfaces (cuts + cylinder's bases) and non flat surfaces (cylinders)
             # (3) cap each object in both lists
             # (4) boolunion every object in both lists
             # (5) check if closed, if it is 
             # ----------------------
             # (1) explode
-            faces_b = df_util.explode_brep(b)
+            faces_b = diffCheck.df_util.explode_brep(b)
 
             # (2) seperate in tow list flat surfaces (cuts + cylinder's bases) and non flat surfaces (cylinders)
             flat_faces_b = []
             non_flat_faces_b = []
             for f_b in faces_b:
                 if f_b.Faces[0].IsPlanar():
                     flat_faces_b.append(f_b)
```

### Comparing `diffCheck-0.0.3/diffCheck/df_transformations.py` & `diffCheck-0.0.4/diffCheck/df_transformations.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.3/diffCheck/df_util.py` & `diffCheck-0.0.4/diffCheck/df_util.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.3/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.4/diffCheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.3
+Version: 0.0.4
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
```

### Comparing `diffCheck-0.0.3/setup.py` & `diffCheck-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diffCheck',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     description='DiffCheck is a package to check the differences between two timber structures',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand',
     author_email='andrea.settimi@epfl.ch',
     url='https://github.com/diffCheckOrg/diffCheck',
```

