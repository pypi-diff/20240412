# Comparing `tmp/dune_rivals-0.2.tar.gz` & `tmp/dune_rivals-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.tar", last modified: Fri Apr 12 20:07:50 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.1.tar", last modified: Fri Apr 12 20:14:48 2024, max compression
```

## Comparing `dune_rivals-0.2.tar` & `dune_rivals-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:07:50.547628 dune_rivals-0.2/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:07:50.547212 dune_rivals-0.2/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:07:50.546760 dune_rivals-0.2/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:07:50.000000 dune_rivals-0.2/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)     7771 2024-04-12 20:02:16.000000 dune_rivals-0.2/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:07:35.000000 dune_rivals-0.2/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:07:50.547720 dune_rivals-0.2/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:14:48.442823 dune_rivals-0.2.1/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:14:48.442408 dune_rivals-0.2.1/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.1/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:14:48.441959 dune_rivals-0.2.1/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     8090 2024-04-12 20:13:23.000000 dune_rivals-0.2.1/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:14:44.000000 dune_rivals-0.2.1/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:14:48.442919 dune_rivals-0.2.1/setup.cfg
```

### Comparing `dune_rivals-0.2/dune_rivals.py` & `dune_rivals-0.2.1/dune_rivals.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,28 +169,35 @@
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
 class SillyGoose2(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
 
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        pass
 
 @ray.remote(num_cpus=0.8, name="SillyGoose3", resources={"worker4": 1e-4})
 class SillyGoose3(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 3
 
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        pass
 
 @ray.remote(num_cpus=0.8, name="SillyGoose4", resources={"worker4": 1e-4})
 class SillyGoose4(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 4
 
+    def start(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict):
+        pass
+
 
 ##############################################################################################
 ###############################         Glossu Rabban          ###############################
 ##############################################################################################
 
 
 ##############################################################################################
```

