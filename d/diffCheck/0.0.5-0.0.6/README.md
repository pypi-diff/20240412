# Comparing `tmp/diffCheck-0.0.5.tar.gz` & `tmp/diffCheck-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffCheck-0.0.5.tar", last modified: Fri Apr 12 13:57:07 2024, max compression
+gzip compressed data, was "diffCheck-0.0.6.tar", last modified: Fri Apr 12 14:42:56 2024, max compression
```

## Comparing `diffCheck-0.0.5.tar` & `diffCheck-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.535807 diffCheck-0.0.5/
--rw-rw-rw-   0        0        0      806 2024-04-12 13:57:07.534807 diffCheck-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.524805 diffCheck-0.0.5/diffCheck/
--rw-rw-rw-   0        0        0       21 2024-04-12 13:57:00.000000 diffCheck-0.0.5/diffCheck/__init__.py
--rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_geometries.py
--rw-rw-rw-   0        0        0     7680 2024-04-12 13:20:49.000000 diffCheck-0.0.5/diffCheck/df_joint_detector.py
--rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_transformations.py
--rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.5/diffCheck/df_util.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:57:07.533804 diffCheck-0.0.5/diffCheck.egg-info/
--rw-rw-rw-   0        0        0      806 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 13:57:07.000000 diffCheck-0.0.5/diffCheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 13:57:07.535807 diffCheck-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      820 2024-04-12 13:56:54.000000 diffCheck-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:42:56.262861 diffCheck-0.0.6/
+-rw-rw-rw-   0        0        0      806 2024-04-12 14:42:56.262359 diffCheck-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2024-04-12 08:02:49.000000 diffCheck-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 14:42:56.239852 diffCheck-0.0.6/diffCheck/
+-rw-rw-rw-   0        0        0       21 2024-04-12 14:42:45.000000 diffCheck-0.0.6/diffCheck/__init__.py
+-rw-rw-rw-   0        0        0     9504 2024-04-12 08:02:49.000000 diffCheck-0.0.6/diffCheck/df_geometries.py
+-rw-rw-rw-   0        0        0     7812 2024-04-12 14:41:11.000000 diffCheck-0.0.6/diffCheck/df_joint_detector.py
+-rw-rw-rw-   0        0        0     4604 2024-04-12 08:02:49.000000 diffCheck-0.0.6/diffCheck/df_transformations.py
+-rw-rw-rw-   0        0        0     4166 2024-04-12 08:02:49.000000 diffCheck-0.0.6/diffCheck/df_util.py
+drwxrwxrwx   0        0        0        0 2024-04-12 14:42:56.260858 diffCheck-0.0.6/diffCheck.egg-info/
+-rw-rw-rw-   0        0        0      806 2024-04-12 14:42:56.000000 diffCheck-0.0.6/diffCheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2024-04-12 14:42:56.000000 diffCheck-0.0.6/diffCheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 14:42:56.000000 diffCheck-0.0.6/diffCheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-12 14:42:56.000000 diffCheck-0.0.6/diffCheck.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-12 14:42:56.000000 diffCheck-0.0.6/diffCheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 14:42:56.262861 diffCheck-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      820 2024-04-12 14:42:45.000000 diffCheck-0.0.6/setup.py
```

### Comparing `diffCheck-0.0.5/PKG-INFO` & `diffCheck-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.5
+Version: 0.0.6
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
         
         DiffCheck is a plugin for Rhino/Grasshopper that allows the user to compare a 3D model with its scan. 
         
         More information to come
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `diffCheck-0.0.5/diffCheck/df_geometries.py` & `diffCheck-0.0.6/diffCheck/df_geometries.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.5/diffCheck/df_joint_detector.py` & `diffCheck-0.0.6/diffCheck/df_joint_detector.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import Rhino.Geometry as rg
 
 import typing
 from dataclasses import dataclass
 
 import diffCheck.df_util
 import diffCheck.df_transformations
-from diffCheck.df_geometries import DFFace
+import diffCheck.df_geometries
 
 @dataclass
 class JointDetector():
     """
     This class is responsible for detecting joints in a brep
     """
     brep : Rhino.Geometry.Brep
@@ -21,17 +21,17 @@
         self._cuts : typing.List[rg.Brep] = []
         # list of holes
         self._holes : typing.List[rg.Brep] = []
         # list of mixed joints (cuts+holes)
         self._mix : typing.List[rg.Brep]= []
 
         # list of DFFaces from joints and sides
-        self._faces : typing.List[DFFace] = []
+        self._faces : typing.List[diffCheck.df_geometries.DFFace] = []
 
-    def run(self) -> typing.List[DFFace]:
+    def run(self) -> typing.List[diffCheck.df_geometries.DFFace]:
         """
             Run the joint detector
 
             :return: a list of faces from joins and faces
         """
         ############################################################################
         # 1. Bring to XY, mamke AABB and get negative boolean difference
@@ -160,27 +160,27 @@
 
         # get all the medians of the faces of cuts only
         cuts_faces_centroids : typing.Dict[int, typing.List[rg.Point3d]] = {}
         for idx, b in enumerate(self._cuts):
             idx = idx + 1
             temp_face_centroids = []
             for f in b.Faces:
-                centroid = DFFace.compute_mass_center(f)
+                centroid = diffCheck.df_geometries.DFFace.compute_mass_center(f)
                 temp_face_centroids.append(centroid)
             cuts_faces_centroids[idx] = temp_face_centroids
 
         # compare with the brep medians faces to get the joint/sides's faces
         for f in self.brep.Faces:
-            centroid_2test = DFFace.compute_mass_center(f)
+            centroid_2test = diffCheck.df_geometries.DFFace.compute_mass_center(f)
             for key, centroids in cuts_faces_centroids.items():
                 is_joint = False
                 for centroid in centroids:
                     if centroid_2test.DistanceTo(centroid) < sc.doc.ModelAbsoluteTolerance:
-                        self._faces.append(DFFace.from_brep(f, key))
+                        self._faces.append(diffCheck.df_geometries.DFFace.from_brep(f, key))
                         is_joint = True
                         break
                 if is_joint:
                     break
             if not is_joint:
-                self._faces.append(DFFace.from_brep(f, None))
+                self._faces.append(diffCheck.df_geometries.DFFace.from_brep(f, None))
 
         return self._faces
```

### Comparing `diffCheck-0.0.5/diffCheck/df_transformations.py` & `diffCheck-0.0.6/diffCheck/df_transformations.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.5/diffCheck/df_util.py` & `diffCheck-0.0.6/diffCheck/df_util.py`

 * *Files identical despite different names*

### Comparing `diffCheck-0.0.5/diffCheck.egg-info/PKG-INFO` & `diffCheck-0.0.6/diffCheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: diffCheck
-Version: 0.0.5
+Version: 0.0.6
 Summary: DiffCheck is a package to check the differences between two timber structures
 Home-page: https://github.com/diffCheckOrg/diffCheck
 Author: Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand
 Author-email: andrea.settimi@epfl.ch
 License: UNKNOWN
 Description: # DiffCheck Grasshopper Plugin
         
         DiffCheck is a plugin for Rhino/Grasshopper that allows the user to compare a 3D model with its scan. 
         
         More information to come
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `diffCheck-0.0.5/setup.py` & `diffCheck-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='diffCheck',
-    version='0.0.5',
+    version='0.0.6',
     packages=['diffCheck'],
     install_requires=[
         'numpy',
         # other dependencies...
     ],
     description='DiffCheck is a package to check the differences between two timber structures',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Andrea Settimi, Damien Gilliard, Eleni Skevaki, Marirena Kladeftira, Julien Gamerro, Stefana Parascho, and Yves Weinand',
     author_email='andrea.settimi@epfl.ch',
     url='https://github.com/diffCheckOrg/diffCheck',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
     ],
 )
```

