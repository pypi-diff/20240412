# Comparing `tmp/fissure-engine-1.0.3.tar.gz` & `tmp/fissure-engine-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fissure-engine-1.0.3.tar", last modified: Wed Apr 10 21:10:59 2024, max compression
+gzip compressed data, was "fissure-engine-1.0.4.tar", last modified: Fri Apr 12 19:10:15 2024, max compression
```

## Comparing `fissure-engine-1.0.3.tar` & `fissure-engine-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.436918 fissure-engine-1.0.3/
--rw-rw-rw-   0        0        0      485 2024-04-10 21:10:59.435920 fissure-engine-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.428388 fissure-engine-1.0.3/fissure_engine/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.3/fissure_engine/__init__.py
--rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.3/fissure_engine/common.py
--rw-rw-rw-   0        0        0    17876 2024-04-10 21:09:47.000000 fissure-engine-1.0.3/fissure_engine/fissure_engine.py
-drwxrwxrwx   0        0        0        0 2024-04-10 21:10:59.434920 fissure-engine-1.0.3/fissure_engine.egg-info/
--rw-rw-rw-   0        0        0      485 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-10 21:10:59.000000 fissure-engine-1.0.3/fissure_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 21:10:59.436918 fissure-engine-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      749 2024-04-10 21:09:47.000000 fissure-engine-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:10:15.571688 fissure-engine-1.0.4/
+-rw-rw-rw-   0        0        0      485 2024-04-12 19:10:15.570682 fissure-engine-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-12 19:10:15.563691 fissure-engine-1.0.4/fissure_engine/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:22:54.000000 fissure-engine-1.0.4/fissure_engine/__init__.py
+-rw-rw-rw-   0        0        0    75962 2024-03-27 20:54:24.000000 fissure-engine-1.0.4/fissure_engine/common.py
+-rw-rw-rw-   0        0        0    17886 2024-04-12 19:09:48.000000 fissure-engine-1.0.4/fissure_engine/fissure_engine.py
+drwxrwxrwx   0        0        0        0 2024-04-12 19:10:15.569683 fissure-engine-1.0.4/fissure_engine.egg-info/
+-rw-rw-rw-   0        0        0      485 2024-04-12 19:10:15.000000 fissure-engine-1.0.4/fissure_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2024-04-12 19:10:15.000000 fissure-engine-1.0.4/fissure_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 19:10:15.000000 fissure-engine-1.0.4/fissure_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-12 19:10:15.000000 fissure-engine-1.0.4/fissure_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-12 19:10:15.000000 fissure-engine-1.0.4/fissure_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 19:10:15.571688 fissure-engine-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      749 2024-04-12 19:10:06.000000 fissure-engine-1.0.4/setup.py
```

### Comparing `fissure-engine-1.0.3/fissure_engine/common.py` & `fissure-engine-1.0.4/fissure_engine/common.py`

 * *Files identical despite different names*

### Comparing `fissure-engine-1.0.3/fissure_engine/fissure_engine.py` & `fissure-engine-1.0.4/fissure_engine/fissure_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     def __hash__(self):
         return hash((self.node, self.mission, self.planet, self.tileset, self.enemy,
                      self.era, self.tier, self.expiry, self.fissure_type, self.activation, self.duration))
 
 def get_fissure_type_identifier(fissure_type, emoji_dict):
     if fissure_type != FissureEngine.FISSURE_TYPE_NORMAL:
         short_identifier = ''.join(word[0] for word in fissure_type.split())
-        return emoji_dict.get(short_identifier, short_identifier)
+        return f"{emoji_dict.get(short_identifier, short_identifier)} "
     return ""
 
 class FissureEngine:
     FISSURE_TYPE_VOID_STORMS = 'Void Storms'
     FISSURE_TYPE_STEEL_PATH = 'Steel Path'
     FISSURE_TYPE_NORMAL = 'Normal'
     FISSURE_TYPES = [FISSURE_TYPE_VOID_STORMS, FISSURE_TYPE_STEEL_PATH, FISSURE_TYPE_NORMAL]
@@ -129,15 +129,15 @@
             emoji_dict (dict): A dictionary mapping fissure type short identifiers and eras to emojis.
 
         Returns:
             dict: A dictionary where each key is a field name and the corresponding value is a list of all values for that field from the list of Fissures, formatted according to the format string.
         """
         preprocess_functions = {
             "{era}": lambda
-                fissure: f"{get_fissure_type_identifier(fissure.fissure_type, emoji_dict)} {emoji_dict.get(fissure.era, '') if emoji_dict else ''} {fissure.era}",
+                fissure: f"{get_fissure_type_identifier(fissure.fissure_type, emoji_dict)}{emoji_dict.get(f"{fissure.era} ", '') if emoji_dict else ''}{fissure.era}",
             "{expiry}": lambda fissure: self.format_time_remaining(fissure.expiry, display_type)
         }
 
         def preprocess_format_string(format_string, fissure):
             for key, preprocess in preprocess_functions.items():
                 if key in format_string:
                     format_string = format_string.replace(key, preprocess(fissure))
```

### Comparing `fissure-engine-1.0.3/setup.py` & `fissure-engine-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
+VERSION = '1.0.4'
 DESCRIPTION = 'Engine for getting fissure information in Warframe.'
 LONG_DESCRIPTION = 'Engine for getting the current fissures for Warframe in a dictionary object.'
 
 
 setup(
     name='fissure-engine',
     version=VERSION,
```

