# Comparing `tmp/dune_rivals-0.2.4.tar.gz` & `tmp/dune_rivals-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.4.tar", last modified: Fri Apr 12 20:26:30 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.5.tar", last modified: Fri Apr 12 20:38:18 2024, max compression
```

## Comparing `dune_rivals-0.2.4.tar` & `dune_rivals-0.2.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:26:30.933360 dune_rivals-0.2.4/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:26:30.932816 dune_rivals-0.2.4/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.4/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:26:30.932097 dune_rivals-0.2.4/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:26:30.000000 dune_rivals-0.2.4/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:26:30.000000 dune_rivals-0.2.4/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:26:30.000000 dune_rivals-0.2.4/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:26:30.000000 dune_rivals-0.2.4/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)     8159 2024-04-12 20:26:05.000000 dune_rivals-0.2.4/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:26:25.000000 dune_rivals-0.2.4/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:26:30.933465 dune_rivals-0.2.4/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:38:18.344839 dune_rivals-0.2.5/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:38:18.344403 dune_rivals-0.2.5/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.5/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:38:18.343916 dune_rivals-0.2.5/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9198 2024-04-12 20:38:00.000000 dune_rivals-0.2.5/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:38:13.000000 dune_rivals-0.2.5/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:38:18.344949 dune_rivals-0.2.5/setup.cfg
```

### Comparing `dune_rivals-0.2.4/dune_rivals.py` & `dune_rivals-0.2.5/dune_rivals.py`

 * *Files 19% similar despite different names*

```diff
@@ -131,27 +131,27 @@
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
 
 ##############################################################################################
 ################################         Silly Goose          ################################
 ##############################################################################################
-class BaseSillyGoose(BaseActor):
-    def __init__(self, payload: str):
-        super().__init__(payload)
-
-    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
-        # set these state variables
-        self.spice_loc_map = spice_loc_map
-        self.spice_file_map = spice_file_map
-        self.order_map = order_map
+# class BaseSillyGoose(BaseActor):
+#     def __init__(self, payload: str):
+#         super().__init__(payload)
+
+#     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+#         # set these state variables
+#         self.spice_loc_map = spice_loc_map
+#         self.spice_file_map = spice_file_map
+#         self.order_map = order_map
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose1", resources={"worker3": 1e-4})
-class SillyGoose1(BaseSillyGoose):
+class SillyGoose1(BaseActor):
     """
     SillyGoose1 is the leader. It picks which spice field to target and moves all
     other Geese to that target. Once the necessary Geese arrive, it instructs the
     Geese to destroy spice in the specified order.
     """
     def __init__(self, payload: str):
         super().__init__(payload)
@@ -165,41 +165,64 @@
 
         # get spice locations and iterate over them to destroy spice
         out = np.where(spice_loc_map==1)
         for i, j in zip(out[0], out[1]):
             # move Geese that are needed to location (i,j)
             geese_ids = self.order_map[(i,j)]
             for goose_id in geese_ids:
-                goose = ray.get_actor(f"SillyGoose{goose_id}")
-                goose._ride_sandworm.remote(i, j)
+                if goose_id != 1:
+                    goose = ray.get_actor(f"SillyGoose{goose_id}")
+                    goose._ride_sandworm.remote(i, j)
+                else:
+                    self._ride_sandworm.remote(i, j)
 
-            # destroy spice
+            # destroy spice in synchronous fashion
             for goose_id in geese_ids:
-                goose = ray.get_actor(f"SillyGoose{goose_id}")
-                goose._destroy_spice_field.remote()
+                if goose_id != 1:
+                    goose = ray.get_actor(f"SillyGoose{goose_id}")
+                    ray.get(goose._destroy_spice_field.remote())
+                else:
+                    ray.get(self._destroy_spice_field.remote())
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
-class SillyGoose2(BaseSillyGoose):
+class SillyGoose2(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
+    
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
-class SillyGoose3(BaseSillyGoose):
+class SillyGoose3(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
+    
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
-class SillyGoose4(BaseSillyGoose):
+class SillyGoose4(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
 
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        # set these state variables
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
 
 ##############################################################################################
 ###############################         Glossu Rabban          ###############################
 ##############################################################################################
 
 
 ##############################################################################################
```

