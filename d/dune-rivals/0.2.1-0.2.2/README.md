# Comparing `tmp/dune_rivals-0.2.1.tar.gz` & `tmp/dune_rivals-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.1.tar", last modified: Fri Apr 12 20:14:48 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.2.tar", last modified: Fri Apr 12 20:20:24 2024, max compression
```

## Comparing `dune_rivals-0.2.1.tar` & `dune_rivals-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:14:48.442823 dune_rivals-0.2.1/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:14:48.442408 dune_rivals-0.2.1/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.1/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:14:48.441959 dune_rivals-0.2.1/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:14:48.000000 dune_rivals-0.2.1/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)     8090 2024-04-12 20:13:23.000000 dune_rivals-0.2.1/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:14:44.000000 dune_rivals-0.2.1/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:14:48.442919 dune_rivals-0.2.1/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:20:24.122219 dune_rivals-0.2.2/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:20:24.121731 dune_rivals-0.2.2/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.2/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:20:24.121199 dune_rivals-0.2.2/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:20:24.000000 dune_rivals-0.2.2/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:20:24.000000 dune_rivals-0.2.2/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:20:24.000000 dune_rivals-0.2.2/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:20:24.000000 dune_rivals-0.2.2/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     8104 2024-04-12 20:18:29.000000 dune_rivals-0.2.2/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:20:16.000000 dune_rivals-0.2.2/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:20:24.122340 dune_rivals-0.2.2/setup.cfg
```

### Comparing `dune_rivals-0.2.1/dune_rivals.py` & `dune_rivals-0.2.2/dune_rivals.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,20 +155,20 @@
         # get spice locations and iterate over them to destroy spice
         out = np.where(spice_loc_map==1)
         for i, j in zip(out[0], out[1]):
             # move Geese that are needed to location (i,j)
             geese_ids = self.order_map[(i,j)]
             for goose_id in geese_ids:
                 goose = ray.get_actor(f"SillyGoose{goose_id}")
-                goose._ride_sandworm(i, j)
+                goose._ride_sandworm.remote(i, j)
 
             # destroy spice
             for goose_id in geese_ids:
                 goose = ray.get_actor(f"SillyGoose{goose_id}")
-                goose._destroy_spice_field(i, j)
+                goose._destroy_spice_field.remote(i, j)
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
 class SillyGoose2(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
```

