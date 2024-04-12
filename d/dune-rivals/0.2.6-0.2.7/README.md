# Comparing `tmp/dune_rivals-0.2.6.tar.gz` & `tmp/dune_rivals-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.6.tar", last modified: Fri Apr 12 20:41:05 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.7.tar", last modified: Fri Apr 12 20:53:25 2024, max compression
```

## Comparing `dune_rivals-0.2.6.tar` & `dune_rivals-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:41:05.645703 dune_rivals-0.2.6/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:41:05.645290 dune_rivals-0.2.6/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.6/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:41:05.644864 dune_rivals-0.2.6/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9184 2024-04-12 20:40:42.000000 dune_rivals-0.2.6/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:41:01.000000 dune_rivals-0.2.6/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:41:05.645794 dune_rivals-0.2.6/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:53:25.510332 dune_rivals-0.2.7/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:53:25.509691 dune_rivals-0.2.7/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.7/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:53:25.509126 dune_rivals-0.2.7/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10179 2024-04-12 20:52:55.000000 dune_rivals-0.2.7/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:53:20.000000 dune_rivals-0.2.7/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:53:25.510462 dune_rivals-0.2.7/setup.cfg
```

### Comparing `dune_rivals-0.2.6/dune_rivals.py` & `dune_rivals-0.2.7/dune_rivals.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,14 +159,23 @@
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
+        # confirm that other actors have set variables
+        all_ready = False
+        while not all_ready:
+            all_ready = True
+            for id in [2, 3, 4]:
+                goose = ray.get_actor(f"SillyGoose{id}")
+                loc_map = ray.get(goose.get_spice_loc_map.remote())
+                all_ready = all_ready and (loc_map is not None)
+
         # get spice locations and iterate over them to destroy spice
         out = np.where(spice_loc_map==1)
         for i, j in zip(out[0], out[1]):
             # move Geese that are needed to location (i,j)
             geese_ids = self.order_map[(i,j)]
             for goose_id in geese_ids:
                 if goose_id != 1:
@@ -187,42 +196,57 @@
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
 class SillyGoose2(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
     
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
+        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
 class SillyGoose3(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
     
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
+        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
 class SillyGoose4(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
+        print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
+
+    def get_spice_loc_map(self):
+        return self.spice_loc_map
 
 ##############################################################################################
 ###############################         Glossu Rabban          ###############################
 ##############################################################################################
 
 
 ##############################################################################################
```

