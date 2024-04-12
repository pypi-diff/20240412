# Comparing `tmp/pyindrav2h-0.0.6.tar.gz` & `tmp/pyindrav2h-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyindrav2h-0.0.6.tar", last modified: Tue Apr  9 10:17:22 2024, max compression
+gzip compressed data, was "pyindrav2h-0.0.7.tar", last modified: Fri Apr 12 11:18:54 2024, max compression
```

## Comparing `pyindrav2h-0.0.6.tar` & `pyindrav2h-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-09 10:17:22.516010 pyindrav2h-0.0.6/
--rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.6/LICENSE
--rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-09 10:17:22.515393 pyindrav2h-0.0.6/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)     2655 2024-04-09 09:20:59.000000 pyindrav2h-0.0.6/README.md
--rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-09 10:16:23.000000 pyindrav2h-0.0.6/pyproject.toml
--rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-09 10:17:22.516141 pyindrav2h-0.0.6/setup.cfg
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-09 10:17:22.499534 pyindrav2h-0.0.6/src/
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-09 10:17:22.506467 pyindrav2h-0.0.6/src/pyindrav2h/
--rw-r--r--   0 paulmorris   (501) staff       (20)      202 2024-04-09 10:16:30.000000 pyindrav2h-0.0.6/src/pyindrav2h/__init__.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     3024 2024-04-09 09:20:59.000000 pyindrav2h-0.0.6/src/pyindrav2h/cli.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     5079 2024-04-09 09:20:59.000000 pyindrav2h-0.0.6/src/pyindrav2h/connection.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      736 2024-04-08 19:31:59.000000 pyindrav2h-0.0.6/src/pyindrav2h/exceptions.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      899 2024-04-09 09:20:59.000000 pyindrav2h-0.0.6/src/pyindrav2h/v2hclient.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     7037 2024-04-09 10:12:52.000000 pyindrav2h-0.0.6/src/pyindrav2h/v2hdevice.py
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-09 10:17:22.514500 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/
--rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/SOURCES.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/dependency_links.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/entry_points.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/requires.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-09 10:17:22.000000 pyindrav2h-0.0.6/src/pyindrav2h.egg-info/top_level.txt
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-12 11:18:54.715256 pyindrav2h-0.0.7/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.7/LICENSE
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-12 11:18:54.714290 pyindrav2h-0.0.7/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2655 2024-04-09 09:20:59.000000 pyindrav2h-0.0.7/README.md
+-rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-12 11:15:04.000000 pyindrav2h-0.0.7/pyproject.toml
+-rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-12 11:18:54.715511 pyindrav2h-0.0.7/setup.cfg
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-12 11:18:54.702196 pyindrav2h-0.0.7/src/
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-12 11:18:54.708446 pyindrav2h-0.0.7/src/pyindrav2h/
+-rw-r--r--   0 paulmorris   (501) staff       (20)      202 2024-04-12 11:15:04.000000 pyindrav2h-0.0.7/src/pyindrav2h/__init__.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     3024 2024-04-09 09:20:59.000000 pyindrav2h-0.0.7/src/pyindrav2h/cli.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     5079 2024-04-09 09:20:59.000000 pyindrav2h-0.0.7/src/pyindrav2h/connection.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      736 2024-04-08 19:31:59.000000 pyindrav2h-0.0.7/src/pyindrav2h/exceptions.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      899 2024-04-09 09:20:59.000000 pyindrav2h-0.0.7/src/pyindrav2h/v2hclient.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     7037 2024-04-12 11:16:58.000000 pyindrav2h-0.0.7/src/pyindrav2h/v2hdevice.py
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-12 11:18:54.713242 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4451 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/SOURCES.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/dependency_links.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/entry_points.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/requires.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-12 11:18:54.000000 pyindrav2h-0.0.7/src/pyindrav2h.egg-info/top_level.txt
```

### Comparing `pyindrav2h-0.0.6/LICENSE` & `pyindrav2h-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/PKG-INFO` & `pyindrav2h-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.6
+Version: 0.0.7
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyindrav2h-0.0.6/README.md` & `pyindrav2h-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/pyproject.toml` & `pyindrav2h-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyindrav2h"
-version = "0.0.6"
+version = "0.0.7"
 description = "API client and example CLI to interact with Indra V2H Chargers"
 readme = "README.md"
 authors = [{ name = "Paul Morris", email = "paul@creatingwake.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h/cli.py` & `pyindrav2h-0.0.7/src/pyindrav2h/cli.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h/connection.py` & `pyindrav2h-0.0.7/src/pyindrav2h/connection.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h/exceptions.py` & `pyindrav2h-0.0.7/src/pyindrav2h/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h/v2hclient.py` & `pyindrav2h-0.0.7/src/pyindrav2h/v2hclient.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h/v2hdevice.py` & `pyindrav2h-0.0.7/src/pyindrav2h/v2hdevice.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,151 +48,151 @@
         self.active = a
     
     @property
     def id(self):
         try:
             return self.active["id"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function id")
+            _LOGGER.debug(f"KeyError [{e}] in function id")
             return None
 
     @property
     def serial(self):
         try:
             return self.data["devices"][0]["deviceUID"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function serial")
+            _LOGGER.debug(f"KeyError [{e}] in function serial")
             return None
 
     @property
     def lastOn(self):
         try:
             return self.data["lastOn"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function lastOn")
+            _LOGGER.debug(f"KeyError [{e}] in function lastOn")
             return None
        
     @property
     def isActive(self):
         try:
             return self.data["devices"][0]["active"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function isActive")
+            _LOGGER.debug(f"KeyError [{e}] in function isActive")
             return None   
 
     @property
     def updateTime(self):
         try:
             return self.stats["time"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function updateTime")
+            _LOGGER.debug(f"KeyError [{e}] in function updateTime")
             return None     
 
     @property
     def isBoosting(self):
         try:
             return self.stats["isBoosting"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function isBoosting")
+            _LOGGER.debug(f"KeyError [{e}] in function isBoosting")
             return None
         
     @property
     def mode(self):
         try:
             return self.stats["mode"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function mode")
+            _LOGGER.debug(f"KeyError [{e}] in function mode")
             return None
         
     @property
     def state(self):
         try:
             return self.stats["state"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function state")
+            _LOGGER.debug(f"KeyError [{e}] in function state")
             return None
 
     @property
     def activeEnergyFromEv(self):
         try:
             return self.stats["data"]["activeEnergyFromEv"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function activeEnergyFromEv")
+            _LOGGER.debug(f"KeyError [{e}] in function activeEnergyFromEv")
             return None
 
     @property
     def activeEnergyToEv(self):
         try:
             return self.stats["data"]["activeEnergyToEv"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function activeEnergyToEv")
+            _LOGGER.debug(f"KeyError [{e}] in function activeEnergyToEv")
             return None
 
     @property
     def powerToEv(self):
         try:
             return self.stats["data"]["powerToEv"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function powerToEv")
+            _LOGGER.debug(f"KeyError [{e}] in function powerToEv")
             return None
 
     @property
     def houseLoad(self):
         try:
             return self.stats["data"]["ctClamp"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function houseLoad")
+            _LOGGER.debug(f"KeyError [{e}] in function houseLoad")
             return None
 
     @property
     def current(self):
         try:
             return self.stats["data"]["current"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function current")
+            _LOGGER.debug(f"KeyError [{e}] in function current")
             return None
 
     @property
     def voltage(self):
         try:
             return self.stats["data"]["voltage"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function voltage")
+            _LOGGER.debug(f"KeyError [{e}] in function voltage")
             return None
 
     @property
     def freq(self):
         try:
             return self.stats["data"]["freq"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function freq")
+            _LOGGER.debug(f"KeyError [{e}] in function freq")
             return None
 
     @property
     def temperature(self):
         try:
             return self.stats["data"]["temp"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function temperature")
+            _LOGGER.debug(f"KeyError [{e}] in function temperature")
             return None
 
     @property
     def soc(self):
         try:
             return self.stats["data"]["soc"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function soc")
+            _LOGGER.debug(f"KeyError [{e}] in function soc")
             return None
 
     @property
     def isInterrupted(self):
         try:
             return self.active["isInterrupted"]
         except KeyError as e:
-            _LOGGER.error(f"KeyError [{e}] in function isInterrupted")
+            _LOGGER.debug(f"KeyError [{e}] in function isInterrupted")
             return None
     
     
     def showDevice(self):
         ret = ""
         
         ret = ret + "--- Device info ---\n"
```

### Comparing `pyindrav2h-0.0.6/src/pyindrav2h.egg-info/PKG-INFO` & `pyindrav2h-0.0.7/src/pyindrav2h.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.6
+Version: 0.0.7
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

