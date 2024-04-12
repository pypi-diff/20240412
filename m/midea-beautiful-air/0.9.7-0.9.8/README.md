# Comparing `tmp/midea-beautiful-air-0.9.7.tar.gz` & `tmp/midea-beautiful-air-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midea-beautiful-air-0.9.7.tar", last modified: Wed Apr  6 18:36:00 2022, max compression
+gzip compressed data, was "midea-beautiful-air-0.9.8.tar", last modified: Thu Apr  7 19:58:18 2022, max compression
```

## Comparing `midea-beautiful-air-0.9.7.tar` & `midea-beautiful-air-0.9.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 18:36:00.294228 midea-beautiful-air-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    12672 2022-04-06 18:36:00.294228 midea-beautiful-air-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11966 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 18:36:00.290228 midea-beautiful-air-0.9.7/midea_beautiful/
--rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25519 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/appliance.py
--rw-r--r--   0 runner    (1001) docker     (121)    14656 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    22690 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)    26237 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/command.py
--rw-r--r--   0 runner    (1001) docker     (121)    15911 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    34694 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/lan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/midea.py
--rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/scanner.py
--rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/midea_beautiful/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 18:36:00.294228 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12672 2022-04-06 18:35:59.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-04-06 18:36:00.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 18:35:59.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-06 18:35:59.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-06 18:36:00.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-06 18:36:00.000000 midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-06 18:36:00.294228 midea-beautiful-air-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-04-06 18:35:44.000000 midea-beautiful-air-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 19:58:18.379659 midea-beautiful-air-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    12672 2022-04-07 19:58:18.379659 midea-beautiful-air-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    11966 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 19:58:18.379659 midea-beautiful-air-0.9.8/midea_beautiful/
+-rw-r--r--   0 runner    (1001) docker     (121)     4307 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25519 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/appliance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14656 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22690 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26237 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/command.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15911 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34694 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/lan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/midea.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8106 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4113 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/midea_beautiful/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-07 19:58:18.379659 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12672 2022-04-07 19:58:17.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-04-07 19:58:18.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-07 19:58:17.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-07 19:58:18.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-07 19:58:18.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-04-07 19:58:18.000000 midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-04-07 19:58:18.379659 midea-beautiful-air-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-04-07 19:58:04.000000 midea-beautiful-air-0.9.8/setup.py
```

### Comparing `midea-beautiful-air-0.9.7/LICENSE` & `midea-beautiful-air-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/PKG-INFO` & `midea-beautiful-air-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-beautiful-air
-Version: 0.9.7
+Version: 0.9.8
 Summary: A library to control Midea appliances via the local network
 Home-page: https://github.com/nbogojevic/midea-beautiful-air
 Author: Nenad Bogojević
 Author-email: nenad.bogojevic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `midea-beautiful-air-0.9.7/README.md` & `midea-beautiful-air-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/__init__.py` & `midea-beautiful-air-0.9.8/midea_beautiful/__init__.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/appliance.py` & `midea-beautiful-air-0.9.8/midea_beautiful/appliance.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/cli.py` & `midea-beautiful-air-0.9.8/midea_beautiful/cli.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/cloud.py` & `midea-beautiful-air-0.9.8/midea_beautiful/cloud.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/command.py` & `midea-beautiful-air-0.9.8/midea_beautiful/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,26 +667,26 @@
     @property
     def horizontal_swing(self):
         """Horizontal swing mode active"""
         return (self.data[17] & 0x0011) >> 2
 
     @horizontal_swing.setter
     def horizontal_swing(self, mode: int):
-        self.data[17] &= ~0x0011  # Clear the mode bit
-        self.data[17] |= 0x1110011 if mode else 0
+        self.data[17] &= ~0b0011  # Clear the mode bit
+        self.data[17] |= 0b1110011 if mode else 0
 
     @property
     def vertical_swing(self):
         """Vertical swing mode active"""
-        return (self.data[17] & 0x1100) >> 2
+        return (self.data[17] & 0b1100) >> 2
 
     @vertical_swing.setter
     def vertical_swing(self, mode: int):
-        self.data[17] &= ~0x1100  # Clear the mode bit
-        self.data[17] |= 0x111100 if mode else 0
+        self.data[17] &= ~0b1100  # Clear the mode bit
+        self.data[17] |= 0b111100 if mode else 0
 
     @property
     def turbo_fan(self) -> bool:
         """Turbo fan mode on/off"""
         return self.data[18] & 0b00100000 != 0
 
     @turbo_fan.setter
```

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/crypto.py` & `midea-beautiful-air-0.9.8/midea_beautiful/crypto.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/exceptions.py` & `midea-beautiful-air-0.9.8/midea_beautiful/exceptions.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/lan.py` & `midea-beautiful-air-0.9.8/midea_beautiful/lan.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/midea.py` & `midea-beautiful-air-0.9.8/midea_beautiful/midea.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/scanner.py` & `midea-beautiful-air-0.9.8/midea_beautiful/scanner.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful/util.py` & `midea-beautiful-air-0.9.8/midea_beautiful/util.py`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/PKG-INFO` & `midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midea-beautiful-air
-Version: 0.9.7
+Version: 0.9.8
 Summary: A library to control Midea appliances via the local network
 Home-page: https://github.com/nbogojevic/midea-beautiful-air
 Author: Nenad Bogojević
 Author-email: nenad.bogojevic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `midea-beautiful-air-0.9.7/midea_beautiful_air.egg-info/SOURCES.txt` & `midea-beautiful-air-0.9.8/midea_beautiful_air.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/setup.cfg` & `midea-beautiful-air-0.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `midea-beautiful-air-0.9.7/setup.py` & `midea-beautiful-air-0.9.8/setup.py`

 * *Files identical despite different names*

