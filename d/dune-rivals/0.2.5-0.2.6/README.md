# Comparing `tmp/dune_rivals-0.2.5.tar.gz` & `tmp/dune_rivals-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.2.5.tar", last modified: Fri Apr 12 20:38:18 2024, max compression
+gzip compressed data, was "dune_rivals-0.2.6.tar", last modified: Fri Apr 12 20:41:05 2024, max compression
```

## Comparing `dune_rivals-0.2.5.tar` & `dune_rivals-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:38:18.344839 dune_rivals-0.2.5/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:38:18.344403 dune_rivals-0.2.5/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.5/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:38:18.343916 dune_rivals-0.2.5/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:38:18.000000 dune_rivals-0.2.5/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)     9198 2024-04-12 20:38:00.000000 dune_rivals-0.2.5/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:38:13.000000 dune_rivals-0.2.5/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:38:18.344949 dune_rivals-0.2.5/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:41:05.645703 dune_rivals-0.2.6/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:41:05.645290 dune_rivals-0.2.6/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.2.6/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-12 20:41:05.644864 dune_rivals-0.2.6/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-12 20:41:05.000000 dune_rivals-0.2.6/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)     9184 2024-04-12 20:40:42.000000 dune_rivals-0.2.6/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-12 20:41:01.000000 dune_rivals-0.2.6/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-12 20:41:05.645794 dune_rivals-0.2.6/setup.cfg
```

### Comparing `dune_rivals-0.2.5/dune_rivals.py` & `dune_rivals-0.2.6/dune_rivals.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,23 +169,23 @@
             # move Geese that are needed to location (i,j)
             geese_ids = self.order_map[(i,j)]
             for goose_id in geese_ids:
                 if goose_id != 1:
                     goose = ray.get_actor(f"SillyGoose{goose_id}")
                     goose._ride_sandworm.remote(i, j)
                 else:
-                    self._ride_sandworm.remote(i, j)
+                    self._ride_sandworm(i, j)
 
             # destroy spice in synchronous fashion
             for goose_id in geese_ids:
                 if goose_id != 1:
                     goose = ray.get_actor(f"SillyGoose{goose_id}")
                     ray.get(goose._destroy_spice_field.remote())
                 else:
-                    ray.get(self._destroy_spice_field.remote())
+                    ray.get(self._destroy_spice_field())
 
 
 @ray.remote(num_cpus=0.8, name="SillyGoose2", resources={"worker3": 1e-4})
 class SillyGoose2(BaseActor):
     def __init__(self, payload: str):
         super().__init__(payload)
         self.id = 2
```

