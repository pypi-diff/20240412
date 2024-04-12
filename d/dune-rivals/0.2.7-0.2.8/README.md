# Comparing `tmp/dune_rivals-0.2.7.tar.gz` & `tmp/dune_rivals-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.7.tar", last modified: Fri Apr 12 20:53:25 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.8.tar", last modified: Fri Apr 12 21:07:12 2024, max compression
```

## Comparing `dune_rivals-0.2.7.tar` & `dune_rivals-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:53:25.510332 dune_rivals-0.2.7/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:53:25.509691 dune_rivals-0.2.7/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.7/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:53:25.509126 dune_rivals-0.2.7/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:53:25.000000 dune_rivals-0.2.7/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    10179 2024-04-12 20:52:55.000000 dune_rivals-0.2.7/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:53:20.000000 dune_rivals-0.2.7/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:53:25.510462 dune_rivals-0.2.7/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:07:12.182103 dune_rivals-0.2.8/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:07:12.181638 dune_rivals-0.2.8/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.8/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 21:07:12.181193 dune_rivals-0.2.8/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 21:07:12.000000 dune_rivals-0.2.8/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    10473 2024-04-12 21:06:32.000000 dune_rivals-0.2.8/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 21:07:06.000000 dune_rivals-0.2.8/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 21:07:12.182222 dune_rivals-0.2.8/setup.cfg
```

### Comparing `dune_rivals-0.2.7/dune_rivals.py` & `dune_rivals-0.2.8/dune_rivals.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 SPICE_FIELD_PROB = 0.01
 SPICE_FILE_SKEW = 0.7
 S3_FILE = 2
 OBJ_FILE = 1
 NUM_ACTORS = 4
 
 
-class BaseActor:
+class BaseRivalActor:
     """
     DO NOT MODIFY
 
     Base class with common functionality shared across all Fedaykin and Rival Actors.
     """
     def __init__(self, payload: str):
         self.payload = payload
         self.i = np.random.randint(0, MAP_DIM - 1)
         self.j = np.random.randint(0, MAP_DIM - 1)
         self.gamestate = ray.get_actor("GameState")
         self.spice_loc_map = None
         self.spice_file_map = None
         self.order_map = None
+        self.name = None
 
     def _destroy_spice_field(self) -> bool:
         """
         DO NOT MODIFY
 
         (Contributes to) destroy(ing) the spice field at location: (self.i, self.j)
 
@@ -48,49 +49,49 @@
           B. at least one Fedaykin preceding this one in the order_map has not yet
              called _destroy_spice_field() at this location
 
         The function returns True if the call to destroy the spice field is successful.
         """
         # if this isn't a spice field, incur a delay and return False
         if not self.spice_loc_map[(self.i, self.j)]:
-            print(f"Fedaykin{self.id} tried to destroy spice at {(self.i, self.j)}, but this is not a Spice location.")
-            print(f"Fedaykin{self.id} sleeping for {SLEEP_SECONDS_NOT_ON_SPICE} seconds")
+            print(f"{self.name} tried to destroy spice at {(self.i, self.j)}, but this is not a Spice location.")  # TODO: fix for h2h
+            print(f"{self.name} sleeping for {SLEEP_SECONDS_NOT_ON_SPICE} seconds")
             time.sleep(SLEEP_SECONDS_NOT_ON_SPICE)
             return False
 
         # if file is "on S3" simulate extra delay for the network request
         if self.spice_file_map[(self.i, self.j)] == S3_FILE:
-            print(f"Fedaykin{self.id} fetching spice field object from S3 for {(self.i, self.j)}")
+            print(f"{self.name} fetching spice field object from S3 for {(self.i, self.j)}")
             time.sleep(SLEEP_SECONDS_READ_FROM_S3)
         else:
-            print(f"Fedaykin{self.id} fetching spice field object from OBJECT STORE for {(self.i, self.j)}")
+            print(f"{self.name} fetching spice field object from OBJECT STORE for {(self.i, self.j)}")
 
         # get spice field object
-        spice_field_refs = ray.get(self.gamestate.get_spice_field_refs.remote("northern"))
+        spice_field_refs = ray.get(self.gamestate.get_spice_field_refs.remote("southern"))  # TODO: fix for h2h
         spice_field = ray.get(spice_field_refs[(self.i, self.j)])
 
         # check if spice field object can be written to
         write_order = self.order_map[(self.i, self.j)]
         try:
             write_idx = np.where(write_order == self.id)[0][0]
         except:
-            print(f"Fedaykin{self.id} tried to destroy spice at {(self.i, self.j)} but is not a valid destroyer ({list(write_order)})")
+            print(f"{self.name} tried to destroy spice at {(self.i, self.j)} but is not a valid destroyer ({list(write_order)})")
 
         if np.array_equal(spice_field["writes"], write_order[:write_idx]):
             spice_field["writes"].append(self.id)
             if np.array_equal(spice_field["writes"], write_order):
                 spice_field["payload"] = self.payload
-                print(f"Fedaykin{self.id} DESTROYED SPICE FIELD AT ({(self.i, self.j)})")
+                print(f"{self.name} DESTROYED SPICE FIELD AT ({(self.i, self.j)})")
             else:
-                print(f"Fedaykin{self.id} partially destroyed spice field at ({(self.i, self.j)})")
-            self.gamestate.update_spice_field_ref.remote(spice_field, self.i, self.j, "northern")
+                print(f"{self.name} partially destroyed spice field at ({(self.i, self.j)})")
+            self.gamestate.update_spice_field_ref.remote(spice_field, self.i, self.j, "southern")  # TODO: fix for h2h
             return True
 
         else:
-            print(f"Fedaykin{self.id} tried to destroy spice at {(self.i, self.j)} but current vs. destruction is: ({spice_writes}) vs. ({list(write_order)})")
+            print(f"{self.name} tried to destroy spice at {(self.i, self.j)} but current vs. destruction is: ({spice_field['writes']}) vs. ({list(write_order)})")
             return False
 
 
     def _ride_sandworm(self, new_i: int, new_j: int) -> None:
         """
         DO NOT MODIFY
 
@@ -110,56 +111,59 @@
 
         # update coordinates
         self.i = new_i
         self.j = new_j
 
 
 @ray.remote(num_cpus=0.1, resources={"worker3": 1e-4})
-class Noop12:
+class Noop12(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 12
+        self.name = "Noop12"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
 @ray.remote(num_cpus=0.1, resources={"worker4": 1e-4})
-class Noop34(BaseActor):
+class Noop34(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 34
+        self.name = "Noop34"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         pass
 
 
 ##############################################################################################
 ################################         Silly Goose          ################################
 ##############################################################################################
-# class BaseSillyGoose(BaseActor):
+# class BaseSillyGoose(BaseRivalActor):
 #     def __init__(self, payload: str):
 #         super().__init__(payload)
 
 #     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
 #         # set these state variables
 #         self.spice_loc_map = spice_loc_map
 #         self.spice_file_map = spice_file_map
 #         self.order_map = order_map
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose1", resources={"worker3": 1e-4})
-class SillyGoose1(BaseActor):
+class SillyGoose1(BaseRivalActor):
     """
     SillyGoose1 is the leader. It picks which spice field to target and moves all
     other Geese to that target. Once the necessary Geese arrive, it instructs the
     Geese to destroy spice in the specified order.
     """
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 1
+        self.name = "SillyGoose1"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
 
@@ -190,52 +194,55 @@
                     goose = ray.get_actor(f"SillyGoose{goose_id}")
                     ray.get(goose._destroy_spice_field.remote())
                 else:
                     ray.get(self._destroy_spice_field())
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
-class SillyGoose2(BaseActor):
+class SillyGoose2(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
+        self.name = "SillyGoose2"
     
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
         print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
-class SillyGoose3(BaseActor):
+class SillyGoose3(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
+        self.name = "SillyGoose3"
     
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
         print(f"SillyGoose{self.id} self.spice_loc_map is None?: {self.spice_loc_map is None}")
 
     def get_spice_loc_map(self):
         return self.spice_loc_map
 
 @ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
-class SillyGoose4(BaseActor):
+class SillyGoose4(BaseRivalActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
+        self.name = "SillyGoose4"
 
     def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
         print(f"SillyGoose{self.id} starting")
         # set these state variables
         self.spice_loc_map = spice_loc_map
         self.spice_file_map = spice_file_map
         self.order_map = order_map
```

