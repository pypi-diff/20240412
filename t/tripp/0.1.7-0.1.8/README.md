# Comparing `tmp/tripp-0.1.7.tar.gz` & `tmp/tripp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripp-0.1.7.tar", max compression
+gzip compressed data, was "tripp-0.1.8.tar", max compression
```

## Comparing `tripp-0.1.7.tar` & `tripp-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,11 @@
--rw-r--r--   0        0        0        0 2023-07-06 12:44:27.112960 tripp-0.1.7/README.md
--rw-r--r--   0        0        0      443 2024-02-21 16:32:38.194447 tripp-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     8108 2024-02-21 16:32:15.275827 tripp-0.1.7/tripp/Trajectory.py
--rw-r--r--   0        0        0        0 2023-05-12 12:04:06.000000 tripp-0.1.7/tripp/__init__.py
--rw-r--r--   0        0        0     4775 2023-10-13 11:20:29.017801 tripp-0.1.7/tripp/edit_pdb.py
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 tripp-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-09 14:03:48.874947 tripp-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1397 2024-04-09 14:03:48.875120 tripp-0.1.8/README.md
+-rw-r--r--   0        0        0      469 2024-04-12 09:50:41.826672 tripp-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     8118 2024-04-09 15:07:38.243777 tripp-0.1.8/tripp/Trajectory.py
+-rw-r--r--   0        0        0     5231 2024-04-12 08:45:27.285532 tripp-0.1.8/tripp/Visualization.py
+-rw-r--r--   0        0        0      210 2024-04-10 12:16:57.816361 tripp-0.1.8/tripp/__init__.py
+-rw-r--r--   0        0        0    11753 2024-04-09 14:04:18.121635 tripp-0.1.8/tripp/color_palettes.py
+-rw-r--r--   0        0        0     5454 2024-04-11 13:00:42.597583 tripp-0.1.8/tripp/edit_pdb.py
+-rw-r--r--   0        0        0     1292 2024-04-09 14:04:18.121985 tripp-0.1.8/tripp/model_pka_values.py
+-rw-r--r--   0        0        0     3019 2024-04-12 09:44:23.895197 tripp-0.1.8/tripp/visualise_pka.py
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 tripp-0.1.8/PKG-INFO
```

### Comparing `tripp-0.1.7/tripp/Trajectory.py` & `tripp-0.1.8/tripp/Trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
     @release_date  : $release_date
     @version       : $release_version
     @author        : Christos Matsingos
     
     This file is part of the TrIPP software
     (https://github.com/fornililab/TrIPP).
-    Copyright (c) 2023 Christos Matsingos and Arianna Fornili.
+    Copyright (c) 2024 Christos Matsingos, Ka Fu Man and Arianna Fornili.
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, version 3.
 
     This program is distributed in the hope that it will be useful, but
     WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -167,8 +167,7 @@
             # Create asynchronous jobs that will be submitted once a processor is ready
             job = pool.apply_async(self.loop_function, args=(output_file, index, extract_surface_data, chain, mutation,))
             jobs.append(job)
         # Submit jobs
         results = [job.get() for job in jobs]
         pool.close()
         self.sort_data(output_file, extract_surface_data, mutation) #Sorting the data only once after all calculations are done, rather than at the end of each job.
-
```

### Comparing `tripp-0.1.7/tripp/edit_pdb.py` & `tripp-0.1.8/tripp/edit_pdb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 """
     @release_date  : $release_date
     @version       : $release_version
-    @author        : Christos Matsingos
+    @author        : Christos Matsingos, Ka Fu Man 
     
     This file is part of the TrIPP software
     (https://github.com/fornililab/TrIPP).
-    Copyright (c) 2023 Christos Matsingos and Arianna Fornili.
+    Copyright (c) 2024 Christos Matsingos, Ka Fu Man and Arianna Fornili.
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, version 3.
 
     This program is distributed in the hope that it will be useful, but
     WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
     General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program. If not, see <http://www.gnu.org/licenses/>.
 """
 
-def edit_pdb(pdbfile):
+
+def edit_pdb(pdbfile): 
+
+
+    """ 
+    Function that edits pdb file naming of residues so that it is compatible 
+    with PROPKA. 
+    """ 
+
+
     with open(pdbfile, 'r') as file: 
         data = file.read() 
-        corrected_amino_acids = { 
+        corrected_amino_acids = { #contains residue names recognised by MDAnalysis and associates them with residue names recognised by PROPKA 
             'ALAD' : 'ALA', 
             'ARGN' : 'ARG ', 
             'ASN1' : 'ASN ', 
             'ASPH' : 'ASP ', 
             'ASPP' : 'ASP ',  
             'CALA' : 'ALA ', 
             'CARG' : 'ARG ', 
@@ -100,22 +109,34 @@
             'HIE' : 'HIS', 
             'HIP' : 'HIS', 
             'HSD' : 'HIS', 
             'HSE' : 'HIS', 
             'HSP' : 'HIS', 
             'LYN' : 'LYS', 
             'LSN' : 'LYS', 
-            'MSE' : 'MET'
+            'MSE' : 'MET',
+            'OC1' : 'O  ', #added so that the atom name is changed for residues that are part of the C-ter (GROMACS)
+            'OC2' : 'OXT',
+            'OT1' : 'O  ', #added so that the atom name is changed for residues that are part of the C-ter 
+            'OT2' : 'OXT' 
             }
         for correction in corrected_amino_acids: 
             data = data.replace(correction, corrected_amino_acids[correction])
     with open(pdbfile, 'w') as file: 
         file.write(data)
 
 def mutate(temp_name, mutation): 
+
+
+    """ 
+    Function that deletes all atoms of a residue except for a methyl group. The 
+    residue is then rename to alanine. 
+    """ 
+
+    
     if type(mutation) == int:
         mutation = [mutation] 
     else: 
         mutation = mutation 
     residue_type = [] 
     lines = [] 
     changed_lines = []
```

