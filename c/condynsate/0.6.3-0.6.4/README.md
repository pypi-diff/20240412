# Comparing `tmp/condynsate-0.6.3.tar.gz` & `tmp/condynsate-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.6.3.tar", last modified: Wed Apr  3 19:33:59 2024, max compression
+gzip compressed data, was "condynsate-0.6.4.tar", last modified: Fri Apr 12 20:04:34 2024, max compression
```

## Comparing `condynsate-0.6.3.tar` & `condynsate-0.6.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 19:33:59.469468 condynsate-0.6.3/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.3/LICENSE
--rw-rw-rw-   0        0        0     4875 2024-04-03 19:33:59.468468 condynsate-0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.3/README.md
--rw-rw-rw-   0        0        0     1439 2024-04-03 19:28:48.000000 condynsate-0.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 19:33:59.469468 condynsate-0.6.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 19:33:59.381360 condynsate-0.6.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:33:59.401360 condynsate-0.6.3/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-04-03 19:33:59.463467 condynsate-0.6.3/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.3/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.3/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.3/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.3/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.3/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.3/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-04-03 19:29:00.000000 condynsate-0.6.3/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.3/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.3/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   145850 2024-04-03 19:21:24.000000 condynsate-0.6.3/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.3/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.3/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-03 19:33:59.466468 condynsate-0.6.3/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4875 2024-04-03 19:33:59.000000 condynsate-0.6.3/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-04-03 19:33:59.000000 condynsate-0.6.3/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 19:33:59.000000 condynsate-0.6.3/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-03 19:33:59.000000 condynsate-0.6.3/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 19:33:59.000000 condynsate-0.6.3/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.760053 condynsate-0.6.4/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.4/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-12 20:04:34.744441 condynsate-0.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.4/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-12 20:03:40.000000 condynsate-0.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 20:04:34.760053 condynsate-0.6.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.665519 condynsate-0.6.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.681931 condynsate-0.6.4/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.744441 condynsate-0.6.4/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.4/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.4/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-12 20:03:30.000000 condynsate-0.6.4/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.4/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.4/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   145453 2024-04-12 19:30:44.000000 condynsate-0.6.4/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10805 2024-04-12 19:31:07.000000 condynsate-0.6.4/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    23281 2024-04-12 17:33:51.000000 condynsate-0.6.4/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.744441 condynsate-0.6.4/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.6.3/LICENSE` & `condynsate-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/PKG-INFO` & `condynsate-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.3
+Version: 0.6.4
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.3/README.md` & `condynsate-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/pyproject.toml` & `condynsate-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.6.3"
+version = "0.6.4"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.4/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.4/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.4/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/check.png` & `condynsate-0.6.4/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.4/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.4/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.4/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.4/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.4/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.4/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/animator.py` & `condynsate-0.6.4/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/keyboard.py` & `condynsate-0.6.4/src/condynsate/keyboard.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.3/src/condynsate/simulator.py` & `condynsate-0.6.4/src/condynsate/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,37 +134,37 @@
         self.urdf_objs = []
         
         # Keep track of all the arrows loaded into the visualizer
         self.lin_arr_map = {}
         self.ccw_arr_map = {}
         
         # Create a visualizer
-        if visualization:
+        self.visualization = visualization
+        if self.visualization:
             self.vis = Visualizer(grid_vis=False,axes_vis=False)
         else:
             self.vis=None
         
         # Create variables to keep track of visualizer frame rate
         self.visualization_fr = visualization_fr
         self.frame_time_target = 0.0
         self.prev_frame_time = -1.0 / self.visualization_fr
         self.vis_time_okay = True
         
         # Create an animator
-        if animation:
+        self.animation = animation
+        if self.animation:
             self.ani = Animator(fr=animation_fr)
         else:
             self.ani=None
             
         # Start the keyboard listener
         self.keyboard = keyboard
-        self.keyboard_running = False
         if self.keyboard:
             self.keys = Keys()
-            self.keyboard_running = True
         else:
             self.keys = None
         
         # Keep track if the simulation is done or not
         self.is_done = False
         
     
@@ -393,15 +393,15 @@
 
                 # Enable the force and torque sensor
                 self.set_joint_force_sensor(urdf_obj=urdf_obj,
                                             joint_name=joint_name,
                                             enable_sensor=True)
 
         # Add urdf objects to the visualizer if visualization is occuring
-        if isinstance(self.vis, Visualizer):
+        if self.visualization:
             if tex_path == None:
                 condynsate_path = Path(__file__).parents[0]
                 condynsate_path = condynsate_path.absolute().as_posix()
                 tex_path = condynsate_path + "/__assets__/check.png"
             self.add_urdf_to_visualizer(urdf_obj=urdf_obj,
                                         tex_path=tex_path)
 
@@ -1770,39 +1770,45 @@
             world coordinates.
 
         """
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
-        # Go through each link and update body com
-        weighted_pos = np.array([0., 0., 0.])
-        total_mass = 0.
-        for link_name in link_map:
-            link_id = link_map[link_name]
-            
-            # Get the mass of each link
-            mass = self.engine.getDynamicsInfo(urdf_id,link_id)[0]
-            
-            # Get the center of mass of each link
-            if link_id==-1:
-                pos = self.engine.getBasePositionAndOrientation(urdf_id)[0]
-            else:
-                pos = self.engine.getLinkState(urdf_id, link_id)[0]
-            pos = np.array(pos)
-            
-            # Update the center of mass parametersd
-            weighted_pos = weighted_pos + mass*pos
-            total_mass = total_mass + mass
-            
-        # Calculate the com
-        if total_mass > 0.:
-            com = weighted_pos / total_mass
+        # Get all link ids
+        link_ids = list(link_map.values())
+        base=False
+        if -1 in link_ids:
+            base=True
+            link_ids.remove(-1)
+        
+        # Get all the link positions
+        link_states = self.engine.getLinkStates(urdf_id, link_ids)
+        
+        # Retrieve the positions and masses for all links from the states
+        total_mass = 0.0
+        if base:
+            base_mass = self.engine.getDynamicsInfo(urdf_id,-1)[0]
+            total_mass += base_mass
+            masses = [base_mass]
+            link_poss = [self.engine.getBasePositionAndOrientation(urdf_id)[0]]
+        else:
+            masses = []
+            link_poss = []
+        for link_id, link_state in zip(link_ids, link_states):
+            link_mass = self.engine.getDynamicsInfo(urdf_id, link_id)[0]
+            total_mass += link_mass
+            masses.append(link_mass)
+            link_poss.append(link_state[0])
+        
+        # Get the CoM
+        if total_mass == 0:
+            com=np.array([0., 0., 0.])
         else:
-            com = np.array([0., 0., 0.])
+            com = np.dot(masses, link_poss) / total_mass
         return com
     
     
     ###########################################################################
     #EXTERNAL FORCE AND TORQUE APPLICATION
     ###########################################################################   
     def apply_force_to_link(self,
@@ -1862,16 +1868,17 @@
         if link_coords:
             f_inW = self._v_inB_to_vinW(urdf_obj, force)
         else:
             f_inW = np.array(force)
         
         # Apply the arrow offset to get the position of the base of the arrow
         # in world coords
-        if np.linalg.norm(f_inW) != 0:
-            f_inW_dirn = f_inW / np.linalg.norm(f_inW)
+        f_inW_norm = np.linalg.norm(f_inW)
+        if f_inW_norm != 0:
+            f_inW_dirn = f_inW / f_inW_norm
         else:
             f_inW_dirn = np.array([0., 0., 0.])
         arr_pos_inW = link_inW + arrow_offset*f_inW_dirn
         arr_pos_inW = tuple(arr_pos_inW.tolist())
         
         # Draw the force arrow
         self._draw_force_arrow(urdf_obj=urdf_obj,
@@ -1944,16 +1951,17 @@
             f_inW = np.array(force)
         
         # Get the center of mass of the body in world cooridnates
         com_inW = self.get_center_of_mass(urdf_obj)
         
         # Apply the arrow offset to get the position of the base of the arrow
         # in world coords
-        if np.linalg.norm(f_inW) != 0:
-            f_inW_dirn = f_inW / np.linalg.norm(f_inW)
+        f_inW_norm = np.linalg.norm(f_inW)
+        if f_inW_norm != 0:
+            f_inW_dirn = f_inW / f_inW_norm
         else:
             f_inW_dirn = np.array([0., 0., 0.])
         arr_pos_inW = com_inW + arrow_offset*f_inW_dirn
         arr_pos_inW = tuple(arr_pos_inW.tolist())
         
         # Draw the force arrow
         self._draw_force_arrow(urdf_obj=urdf_obj,
@@ -2022,16 +2030,17 @@
             t_inW = np.array(torque)
         
         # Get the center of mass of the body in world cooridnates
         com_inW = self.get_center_of_mass(urdf_obj)
         
         # Apply the arrow offset to get the position of the base of the arrow
         # in world coords
-        if np.linalg.norm(t_inW) != 0:
-            t_inW_dirn = t_inW / np.linalg.norm(t_inW)
+        t_inW_norm = np.linalg.norm(t_inW)
+        if t_inW_norm != 0:
+            t_inW_dirn = t_inW / t_inW_norm
         else:
             t_inW_dirn = np.array([0., 0., 0.])
         arr_pos_inW = com_inW + arrow_offset*t_inW_dirn
         arr_pos_inW = tuple(arr_pos_inW.tolist())
         
         # Draw the torque arrow
         self._draw_torque_arrow(urdf_obj=urdf_obj,
@@ -2091,28 +2100,26 @@
         None.
 
         """
         # If we cannot update the arrow, do nothing
         if not self.vis_time_okay and not force_update:
             return
         
+        # If the visualizer doesn't exist, leave
+        if not self.visualization:
+            return
+        
         # Get the URDF ID and combine with link name to get the key to the 
         # linear arrow map
         urdf_id = str(urdf_obj.urdf_id)
         urdf_force = urdf_id + "__" + force_name
         
-        # Make sure the visualizer exists and check the current status of the 
-        # arrow
-        vis_exists = isinstance(self.vis, Visualizer)
+        # Check the current status of the arrow
         arr_exists = urdf_force in self.lin_arr_map
-        
-        # If the visualizer doesn't exist, leave
-        if not vis_exists:
-            return
-        
+  
         # If show_arrow is set to false, and the visualizer and associated
         # force arrow exist, set the arrows visibility to false
         if (not show_arrow) and arr_exists:
             arr_name = str(self.lin_arr_map[urdf_force])
             self.vis.set_link_color(urdf_name = "Force Arrows",
                                     link_name = arr_name,
                                     link_geometry = self.lin_geom, 
@@ -2121,16 +2128,17 @@
                                     opacity = 0.0)
         
         # If show arrow is set to True and the visualizer exists, draw the
         # arrow at the position and orientation listed.
         if show_arrow:
             
             # Get the direction in which the force is applied
-            if np.linalg.norm(f_inW) != 0:
-                arr_dirn_inW = f_inW / np.linalg.norm(f_inW)
+            f_inW_norm = np.linalg.norm(f_inW)
+            if f_inW_norm != 0:
+                arr_dirn_inW = f_inW / f_inW_norm
             else:
                 arr_dirn_inW = np.array([0., 0., 0.])
                 
             # Get the orientation of the force arrow based on the direction
             # that it's pointing
             arr_xyzw_inW = get_rot_from_2_vecs([0,0,1], arr_dirn_inW)
             arr_wxyz_inW = xyzw_to_wxyz(arr_xyzw_inW)
@@ -2221,28 +2229,26 @@
         None.
 
         """
         # If we cannot update the arrow, do nothing
         if not self.vis_time_okay and not force_update:
             return
         
+        # If the visualizer doesn't exist, leave
+        if not self.visualization:
+            return
+        
         # Get the URDF ID and combine with link name to get the key to the 
         # ccw arrow map
         urdf_id = str(urdf_obj.urdf_id)
         urdf_torque = urdf_id + "__" + torque_name
         
-        # Make sure the visualizer exists and check the current status of the 
-        # arrow
-        vis_exists = isinstance(self.vis, Visualizer)
+        # Check the current status of the arrow
         arr_exists = urdf_torque in self.ccw_arr_map
         
-        # If the visualizer doesn't exist, leave
-        if not vis_exists:
-            return
-        
         # If show_arrow is set to false, and the visualizer and associated
         # torque arrow exist, set the arrows visibility to false
         if (not show_arrow) and arr_exists:
             arr_name = str(self.ccw_arr_map[urdf_torque])
             self.vis.set_link_color(urdf_name = "Torque Arrows",
                                     link_name = arr_name,
                                     link_geometry = self.ccw_geom, 
@@ -2251,16 +2257,17 @@
                                     opacity = 0.0)
         
         # If show arrow is set to True and the visualizer exists, draw the
         # arrow at the position and orientation listed.
         if show_arrow:
             
             # Get the direction in which the torque is applied
-            if np.linalg.norm(t_inW) != 0:
-                arr_dirn_inW = t_inW / np.linalg.norm(t_inW)
+            t_inW_norm = np.linalg.norm(t_inW)
+            if t_inW_norm != 0:
+                arr_dirn_inW = t_inW / t_inW_norm
             else:
                 arr_dirn_inW = np.array([0., 0., 0.])
                 
             # Get the orientation of the torque arrow based on the direction
             # that it's pointing
             arr_xyzw_inW = get_rot_from_2_vecs([0,0,1], arr_dirn_inW)
             arr_wxyz_inW = xyzw_to_wxyz(arr_xyzw_inW)
@@ -2341,15 +2348,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Extract the visual data from the urdf object in the simulator
         paths,names,scales,colors,poss,oris = self._get_urdf_vis_dat(urdf_obj)
         
         # Make the URDF name and format the texture path
         urdf_name = str(urdf_obj.urdf_id)
@@ -2410,15 +2417,15 @@
             
         Returns
         -------
         None.
 
         """
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Collect the visual data and urdf name
         paths,names,scales,colors,poss,oris = self._get_urdf_vis_dat(urdf_obj)
         urdf_name = str(urdf_obj.urdf_id)
         
         # Go through all links in urdf object and update their position
@@ -2556,15 +2563,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return    
         
         # If the link name doesn't exist, don't attempt to update it
         if not (link_name in urdf_obj.link_map):
             return
     
         # Get name and id data from urdf_obj
@@ -2623,15 +2630,15 @@
         # If the joint is invalid, do nothing
         if (joint_name in joint_map):
             joint_id = joint_map[joint_name]
         else:
             return
         
         # If there is no visualizer, do not color
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return    
         
         # Get the joint position
         state = self.get_joint_state(urdf_obj=urdf_obj,
                                      joint_name=joint_name)
         pos = state['position']
         
@@ -2691,15 +2698,15 @@
         # If the joint is invalid, do nothing
         if (joint_name in joint_map):
             joint_id = joint_map[joint_name]
         else:
             return
         
         # If there is no visualizer, do not color
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return    
         
         # Get the joint velocity
         state = self.get_joint_state(urdf_obj=urdf_obj,
                                      joint_name=joint_name)
         vel = state['velocity']
         
@@ -2761,15 +2768,15 @@
         # If the joint is invalid, do nothing
         if (joint_name in joint_map):
             joint_id = joint_map[joint_name]
         else:
             return
         
         # If there is no visualizer, do not color
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return    
         
         # Calculate the torque saturation and get the associated color
         sat = (torque - min_torque) / (max_torque - min_torque)
         sat = np.clip(sat, 0.0, 1.0)
         col = cmaps['coolwarm'](round(255*sat))[0:3]
         col = format_RGB(col,
@@ -2818,15 +2825,15 @@
         link_map = urdf_obj.link_map
     
         # If the link is invalid, do nothing
         if not (link_name in link_map):
             return
         
         # If there is no visualizer, do not color
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return    
         
         # Get the mass
         mass = self.get_link_mass(urdf_obj=urdf_obj,
                                   link_name=link_name)
         
         # Calculate the mass saturation and get the associated color
@@ -2886,15 +2893,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the camera transform
         else:
             self.vis.transform_camera(scale = scale,
                                       translate = translate,
                                       wxyz_quaternion = wxyz_quaternion,
@@ -2926,15 +2933,15 @@
     
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_background(top_color = top_color,
                                     bot_color = bot_color)
      
@@ -2962,15 +2969,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_spotlight(on = on,
                                    intensity = intensity,
                                    distance = distance)
@@ -3000,15 +3007,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_posx_pt_light(on = on,
                                        intensity = intensity,
                                        distance = distance)
@@ -3038,15 +3045,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_negx_pt_light(on = on,
                                        intensity = intensity,
                                        distance = distance)
@@ -3072,15 +3079,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_ambient_light(on = on,
                                        intensity = intensity)
             
@@ -3105,15 +3112,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no visualizer, do not attempt to update it
-        if not isinstance(self.vis, Visualizer):
+        if not self.visualization:
             return
         
         # Apply the background colors
         else:
             self.vis.set_fill_light(on = on,
                                        intensity = intensity)
         
@@ -3224,15 +3231,15 @@
             points, etc.).
         artist_inds : tuple of ints
             A tuple of integer identifiers that are unique to the artist
             created. This allows future interaction with these artists (adding
             data points, etc.).
         """
         # If there is no animator, do not attempt to add a plot to it
-        if not isinstance(self.ani, Animator):
+        if not self.animation:
             return
         
         # Add the plot data to the plot
         v1, v2 = self.ani.add_subplot(n_artists=n_artists,
                                       subplot_type=subplot_type,
                                       title=title,
                                       x_label=x_label,
@@ -3281,15 +3288,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no animator, do not attempt to update it
-        if not isinstance(self.ani, Animator):
+        if not self.animation:
             return
         
         # Update the plot
         self.ani.add_subplot_point(subplot_index=subplot_index,
                                    artist_index=artist_index,
                                    x=x,
                                    y=y)
@@ -3305,15 +3312,15 @@
 
         """
         # Do nothing if paused
         if self.paused:
             return
         
         # If there is no animator, do not attempt to update it
-        if not isinstance(self.ani, Animator):
+        if not self.animation:
             return
         
         self.ani.reset_plots()
         
         
     def open_animator_gui(self):
         """
@@ -3323,15 +3330,15 @@
 
         Returns
         -------
         None.
 
         """
         # Open the animator figure window if it exists
-        if isinstance(self.ani, Animator):
+        if self.animation:
             self.ani.create_figure()
         
         
     ###########################################################################
     #SIMULATION EXECUTION
     ###########################################################################
     def is_pressed(self,
@@ -3357,15 +3364,15 @@
         -------
         bool
             A boolean flag to indicate whether the desired key is pressed. If
             the keyboard is disabled, always returns False.
 
         """
         # Make sure that the keyboard exists
-        if (self.keyboard and isinstance(self.keys, Keys)):
+        if self.keyboard:
             return self.keys.is_pressed(key)
         else:
             return False
         
         
     def await_keypress(self,
                        key = "enter"):
@@ -3382,31 +3389,31 @@
 
         Returns
         -------
         None.
 
         """
         # Update the visualizer if it exists
-        if isinstance(self.vis, Visualizer):
+        if self.visualization:
             for urdf_obj in self.urdf_objs:
                 if urdf_obj.update_vis:
                     self._update_urdf_visual(urdf_obj)
         
         # If there is a keyboard
-        if (self.keyboard and isinstance(self.keys, Keys)):
+        if self.keyboard:
             # Tell user what to do
             print("PRESS "+key.upper()+" TO START SIMULATION.")
             print("PRESS ESC TO QUIT.")
             print("PRESS SPACE TO PAUSE/RESUME SIMULATION.")
             print("PRESS BACKSPACE TO RESET SIMULATION.")
             
             # Await keypress
             while True:
                 # Ensure so the GUI remains interactive
-                if isinstance(self.ani, Animator):
+                if self.animation:
                     self.ani.flush_events()
                     
                 # Termination condition
                 if self.is_pressed("esc"):
                     self.is_done = True
                     print("QUITTING...")
                     return
@@ -3417,15 +3424,15 @@
                     return
             
         # If there is not a keyboard, wait 1 second then return
         else:
             start_time = time.time()
             while (time.time() - start_time) < 1.0:
                 # Ensure so the GUI remains interactive
-                if isinstance(self.ani, Animator):
+                if self.animation:
                     self.ani.flush_events()
                 time.sleep(0.05)
             return
       
       
     def iterate_val(self,
                     curr_val,
@@ -3602,30 +3609,30 @@
         # Make sure that if there is not keyboard, the simulation only lasts
         # 10.0 seconds
         if (not self.keyboard) and (max_time == None):
             max_time = 10.0
 
         # If the keyboard is supposed to be running, but it is not,
         # terminate the simulation
-        if self.keyboard and isinstance(self.keys, Keys):
+        if self.keyboard:
             if not self.keys.running:
                 self.is_done = True
                 print("KEYBOARD LOST. QUITTING...")
                 return -2 # Return LOS end code
 
         # Collect keyboard IO for termination
         if self.is_pressed("esc"):
             self.is_done = True
             print("QUITTING...")
             return -1 # Return end code
 
         # Suspend if paused or resume if space is pressed
         if self.paused:
             time.sleep(0.05)
-            if isinstance(self.ani, Animator):
+            if self.animation:
                 self.ani.flush_events()
             if self.is_pressed("space"):
                 self.paused = False
                 print("RESUME")
                 time.sleep(0.2)
                 self.pause_elapsed_time += time.time()-self.pause_start_time
                 return 1 # Return end pause code
@@ -3651,28 +3658,27 @@
         # frame update
         frame_cond_1 = current_time >= self.frame_time_target
         frame_cond_2 = self.prev_frame_time < self.frame_time_target
         frame_cond_3 = self.prev_frame_time >= self.frame_time_target
         self.vis_time_okay = (frame_cond_1 and frame_cond_2) or frame_cond_3
     
         # Update the visualizer
-        vis_exists = isinstance(self.vis, Visualizer)
-        if self.vis_time_okay and update_vis and vis_exists:
+        if self.vis_time_okay and update_vis and self.visualization:
             
             # Keep track of number of frames and target frame time
             self.frame_time_target += + 1.0/self.visualization_fr
             self.prev_frame_time = current_time
                         
             # Update all urdfs
             for urdf_obj in self.urdf_objs:
                 if urdf_obj.update_vis:
                     self._update_urdf_visual(urdf_obj)
        
         # Update the animator if it exists
-        if update_ani and isinstance(self.ani, Animator):
+        if update_ani and self.animation:
             self.ani.step()
 
         # Calculate suspend time if running simulation in real time
         if real_time:
             # Get the amount of time to wait to place in real time
             time_to_wait = (self.prev_step_time + self.dt) - current_time
             self.prev_step_time = current_time
@@ -3681,15 +3687,15 @@
             if time_to_wait > 0:
                 time.sleep(time_to_wait)
 
         # Pause upon request
         if self.is_pressed("space"):
             self.pause_start_time = time.time()
             self.paused = True
-            if isinstance(self.ani, Animator):
+            if self.animation:
                 self.ani.flush_events()
             print("PAUSED")
             time.sleep(0.2)
             return 4 # Return start pause code
 
         # Check for max time
         if max_time != None:
```

### Comparing `condynsate-0.6.3/src/condynsate/utils.py` & `condynsate-0.6.4/src/condynsate/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 
 ###############################################################################
 #DEPENDENCIES
 ###############################################################################
 import numpy as np
-from pathlib import Path
+import os
 
 
 ###############################################################################
 #PUBLIC FUNCTIONS
 ###############################################################################
 def get_rot_from_2_vecs(vec1,
                         vec2):
@@ -75,15 +75,19 @@
 
     Returns
     -------
     wxyz_quaternion : array-like, size (4,)
         The Hamilton representation of the input JPL quaterion
 
     """
-    wxyz_quaternion = np.roll(xyzw_quaternion, 1)
+    wxyz_quaternion = np.array([xyzw_quaternion[3],
+                                xyzw_quaternion[0],
+                                xyzw_quaternion[1],
+                                xyzw_quaternion[2]])
+    #wxyz_quaternion = np.roll(xyzw_quaternion, 1)
     return wxyz_quaternion
 
 
 def wxyz_to_xyzw(wxyz_quaternion):
     """
     Converts a Hamilton quaternion (wxyz) to a JPL quaternion (xyzw)
 
@@ -94,15 +98,19 @@
 
     Returns
     -------
     xyzw_quaternion : array-like, size (4,)
         The JPL representation of the input Hamilton quaterion.
 
     """
-    xyzw_quaternion = np.roll(wxyz_quaternion, -1)
+    xyzw_quaternion = np.array([wxyz_quaternion[1],
+                                wxyz_quaternion[2],
+                                wxyz_quaternion[3],
+                                wxyz_quaternion[0]])
+    #xyzw_quaternion = np.roll(wxyz_quaternion, -1)
     return xyzw_quaternion
 
 
 def xyzw_quat_mult(q1, q2):
     """
     Gets the resultant JPL quaternion (xyzw) that arises from first 
     applying the q1 (xyzw) rotation then applying the q2 (xyzw) rotation.
@@ -249,15 +257,16 @@
 
     Returns
     -------
     formatted_path : string
         The formatted Windows path string.
 
     """
-    formatted_path = str(Path(unformatted_path))
+    formatted_path = os.path.abspath(unformatted_path)
+    #formatted_path = str(Path(unformatted_path))
     return formatted_path
     
 
 def format_RGB(unformatted_rgb,
                 range_to_255=True):
     """
     Converts unformatted rgb array-like objects to formatted rgb lists
```

### Comparing `condynsate-0.6.3/src/condynsate/visualizer.py` & `condynsate-0.6.4/src/condynsate/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 ###############################################################################
 #DEPENDENCIES
 ###############################################################################
 import numpy as np
 import meshcat
 import meshcat.geometry as geo
-import meshcat.transformations as tf
 from condynsate.utils import format_path, wxyz_from_euler
 
 
 ###############################################################################
 #VISUALIZER CLASS
 ###############################################################################
 class Visualizer():
@@ -251,19 +250,43 @@
         Returns
         -------
         transform : array-like, size (4,4)
             The resultant 4x4 3D affine transformation matrix.
 
         """
         # Get the scaling matrix based on the scale vector
+        scale_matrix = np.array([[scale[0], 0.0,      0.0,      0.0],
+                                 [0.0,      scale[1], 0.0,      0.0],
+                                 [0.0,      0.0,      scale[2], 0.0],
+                                 [0.0,      0.0,      0.0,      1.0]])
+        
         # Get the translation matrix based on the translation vector
+        translate_matrix = np.array([[1.0, 0.0, 0.0, translate[0]],
+                                     [0.0, 1.0, 0.0, translate[1]],
+                                     [0.0, 0.0, 1.0, translate[2]],
+                                     [0.0, 0.0, 0.0, 1.0]])
+        
         # Get the rotation matrix based on the wxyz quaternion
-        scale_matrix = np.diag(np.concatenate((scale, [1.0])))
-        translate_matrix = tf.translation_matrix(translate)
-        rotation_matrix = tf.quaternion_matrix(wxyz_quaternion)
+        w = wxyz_quaternion[0]
+        x = wxyz_quaternion[1]
+        y = wxyz_quaternion[2]
+        z = wxyz_quaternion[3]
+        xx = 2.*x*x
+        xy = 2.*x*y
+        xz = 2.*x*z
+        yy = 2.*y*y
+        yz = 2.*y*z
+        zz = 2.*z*z
+        wx = 2.*w*x
+        wy = 2.*w*y
+        wz = 2.*w*z
+        rotation_matrix = np.array([[1.-yy-zz, xy-wz, xz+wy, 0.],
+                                    [xy+wz, 1.-xx-zz, yz-wx, 0.],
+                                    [xz-wy, yz+wx, 1.-xx-yy, 0.],
+                                    [0., 0., 0., 1.]])
         
         # Calculate and return the total transformation matrix
         transform =  translate_matrix @ rotation_matrix @ scale_matrix
         return transform
 
 
     def apply_transform(self,
```

### Comparing `condynsate-0.6.3/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.4/src/condynsate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.3
+Version: 0.6.4
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.3/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.4/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

