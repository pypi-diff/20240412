# Comparing `tmp/cowbase-1.0.0.tar.gz` & `tmp/cowbase-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowbase-1.0.0.tar", last modified: Tue Apr  9 10:17:33 2024, max compression
+gzip compressed data, was "cowbase-1.0.1.tar", last modified: Fri Apr 12 08:52:43 2024, max compression
```

## Comparing `cowbase-1.0.0.tar` & `cowbase-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 10:17:33.590575 cowbase-1.0.0/
--rw-rw-rw-   0        0        0     1089 2024-04-04 19:01:24.000000 cowbase-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       41 2023-10-09 09:52:17.000000 cowbase-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2932 2024-04-09 10:17:33.588573 cowbase-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    15101 2024-04-09 09:59:23.000000 cowbase-1.0.0/README.md
--rw-rw-rw-   0        0        0     1571 2024-04-09 10:16:40.000000 cowbase-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 10:17:33.591577 cowbase-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2024-04-09 10:07:08.000000 cowbase-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:17:33.528237 cowbase-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-09 10:17:33.556555 cowbase-1.0.0/src/cowbase/
--rw-rw-rw-   0        0        0     1349 2024-04-09 10:00:02.000000 cowbase-1.0.0/src/cowbase/__init__.py
--rw-rw-rw-   0        0        0    16012 2024-01-05 10:26:39.000000 cowbase-1.0.0/src/cowbase/cowbase_m1.py
--rw-rw-rw-   0        0        0     8378 2023-10-10 14:13:30.000000 cowbase-1.0.0/src/cowbase/cowbase_m2.py
--rw-rw-rw-   0        0        0     8941 2023-10-10 14:13:44.000000 cowbase-1.0.0/src/cowbase/cowbase_m3.py
--rw-rw-rw-   0        0        0    54464 2024-04-03 14:40:58.000000 cowbase-1.0.0/src/cowbase/cowbase_m4.py
--rw-rw-rw-   0        0        0    21667 2023-11-16 09:24:30.000000 cowbase-1.0.0/src/cowbase/cowbase_m5.py
-drwxrwxrwx   0        0        0        0 2024-04-09 10:17:33.584573 cowbase-1.0.0/src/cowbase/utils/
--rw-rw-rw-   0        0        0     1959 2023-10-04 13:23:50.000000 cowbase-1.0.0/src/cowbase/utils/M1_restoreDB.sql
--rw-rw-rw-   0        0        0     7611 2023-09-05 13:24:47.000000 cowbase-1.0.0/src/cowbase/utils/M1_tableDict.json
--rw-rw-rw-   0        0        0     8243 2023-07-18 08:46:11.000000 cowbase-1.0.0/src/cowbase/utils/M2_tableDict.json
--rw-rw-rw-   0        0        0    27926 2023-12-05 09:54:53.000000 cowbase-1.0.0/src/cowbase/utils/M3_tableDict.json
--rw-rw-rw-   0        0        0     6293 2023-12-05 09:54:53.000000 cowbase-1.0.0/src/cowbase/utils/M4_sqlupdate.json
--rw-rw-rw-   0        0        0    33271 2024-04-03 14:42:23.000000 cowbase-1.0.0/src/cowbase/utils/M4_tableDict.json
--rw-rw-rw-   0        0        0      302 2023-06-14 14:57:08.000000 cowbase-1.0.0/src/cowbase/utils/config.toml
--rw-rw-rw-   0        0        0       92 2023-06-21 08:14:28.000000 cowbase-1.0.0/src/cowbase/utils/config_farm.toml
--rw-rw-rw-   0        0        0      315 2023-08-11 09:18:43.000000 cowbase-1.0.0/src/cowbase/utils/serverSettings.json
-drwxrwxrwx   0        0        0        0 2024-04-09 10:17:33.586571 cowbase-1.0.0/src/cowbase.egg-info/
--rw-rw-rw-   0        0        0     2932 2024-04-09 10:17:33.000000 cowbase-1.0.0/src/cowbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2024-04-09 10:17:33.000000 cowbase-1.0.0/src/cowbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 10:17:33.000000 cowbase-1.0.0/src/cowbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      522 2024-04-09 10:17:33.000000 cowbase-1.0.0/src/cowbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-09 10:17:33.000000 cowbase-1.0.0/src/cowbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 08:52:43.351451 cowbase-1.0.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-04 19:01:24.000000 cowbase-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       41 2023-10-09 09:52:17.000000 cowbase-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2932 2024-04-12 08:52:43.349452 cowbase-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    15101 2024-04-09 09:59:23.000000 cowbase-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1571 2024-04-12 08:52:27.000000 cowbase-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 08:52:43.351451 cowbase-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2024-04-09 10:07:08.000000 cowbase-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:52:43.301452 cowbase-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 08:52:43.320454 cowbase-1.0.1/src/cowbase/
+-rw-rw-rw-   0        0        0     1349 2024-04-09 10:00:02.000000 cowbase-1.0.1/src/cowbase/__init__.py
+-rw-rw-rw-   0        0        0    16012 2024-01-05 10:26:39.000000 cowbase-1.0.1/src/cowbase/cowbase_m1.py
+-rw-rw-rw-   0        0        0     8378 2023-10-10 14:13:30.000000 cowbase-1.0.1/src/cowbase/cowbase_m2.py
+-rw-rw-rw-   0        0        0     8941 2023-10-10 14:13:44.000000 cowbase-1.0.1/src/cowbase/cowbase_m3.py
+-rw-rw-rw-   0        0        0    54464 2024-04-03 14:40:58.000000 cowbase-1.0.1/src/cowbase/cowbase_m4.py
+-rw-rw-rw-   0        0        0    21476 2024-04-12 06:22:59.000000 cowbase-1.0.1/src/cowbase/cowbase_m5.py
+drwxrwxrwx   0        0        0        0 2024-04-12 08:52:43.344451 cowbase-1.0.1/src/cowbase/utils/
+-rw-rw-rw-   0        0        0     1959 2023-10-04 13:23:50.000000 cowbase-1.0.1/src/cowbase/utils/M1_restoreDB.sql
+-rw-rw-rw-   0        0        0     7611 2023-09-05 13:24:47.000000 cowbase-1.0.1/src/cowbase/utils/M1_tableDict.json
+-rw-rw-rw-   0        0        0     8243 2023-07-18 08:46:11.000000 cowbase-1.0.1/src/cowbase/utils/M2_tableDict.json
+-rw-rw-rw-   0        0        0    27926 2023-12-05 09:54:53.000000 cowbase-1.0.1/src/cowbase/utils/M3_tableDict.json
+-rw-rw-rw-   0        0        0     6293 2023-12-05 09:54:53.000000 cowbase-1.0.1/src/cowbase/utils/M4_sqlupdate.json
+-rw-rw-rw-   0        0        0    33271 2024-04-03 14:42:23.000000 cowbase-1.0.1/src/cowbase/utils/M4_tableDict.json
+-rw-rw-rw-   0        0        0      302 2023-06-14 14:57:08.000000 cowbase-1.0.1/src/cowbase/utils/config.toml
+-rw-rw-rw-   0        0        0       92 2023-06-21 08:14:28.000000 cowbase-1.0.1/src/cowbase/utils/config_farm.toml
+-rw-rw-rw-   0        0        0      315 2023-08-11 09:18:43.000000 cowbase-1.0.1/src/cowbase/utils/serverSettings.json
+drwxrwxrwx   0        0        0        0 2024-04-12 08:52:43.347451 cowbase-1.0.1/src/cowbase.egg-info/
+-rw-rw-rw-   0        0        0     2932 2024-04-12 08:52:43.000000 cowbase-1.0.1/src/cowbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      699 2024-04-12 08:52:43.000000 cowbase-1.0.1/src/cowbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 08:52:43.000000 cowbase-1.0.1/src/cowbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      522 2024-04-12 08:52:43.000000 cowbase-1.0.1/src/cowbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-12 08:52:43.000000 cowbase-1.0.1/src/cowbase.egg-info/top_level.txt
```

### Comparing `cowbase-1.0.0/LICENSE` & `cowbase-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/PKG-INFO` & `cowbase-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowbase
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for data processing of Automatic Milking System data
 Author-email: Martin Julius Gote <martin.gote@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2024 Martin Gote
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cowbase-1.0.0/README.md` & `cowbase-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/pyproject.toml` & `cowbase-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=62.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "cowbase"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python package for data processing of Automatic Milking System data"
 authors = [{ name = "Martin Julius Gote", email = "martin.gote@kuleuven.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
```

### Comparing `cowbase-1.0.0/src/cowbase/__init__.py` & `cowbase-1.0.1/src/cowbase/__init__.py`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/cowbase_m1.py` & `cowbase-1.0.1/src/cowbase/cowbase_m1.py`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/cowbase_m2.py` & `cowbase-1.0.1/src/cowbase/cowbase_m2.py`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/cowbase_m3.py` & `cowbase-1.0.1/src/cowbase/cowbase_m3.py`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/cowbase_m4.py` & `cowbase-1.0.1/src/cowbase/cowbase_m4.py`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/cowbase_m5.py` & `cowbase-1.0.1/src/cowbase/cowbase_m5.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,18 +366,14 @@
     """
     Returns connection to database, specify parameters in settings file
 
     Parameters
     ----------
     rootdir : str
         path to cowbase rootdir
-    farm_to_update : str
-        name of farm for which data is processed
-    anonymizeFarmlocation : bool
-        anonlymize farm location (in a radius of 5 km around original location)
     """
 
     settingsPath = os.path.join(rootdir, "config", "serverSettings.json")
 
     with open(settingsPath) as file:
         serverSettings = json.load(file)
```

### Comparing `cowbase-1.0.0/src/cowbase/utils/M1_restoreDB.sql` & `cowbase-1.0.1/src/cowbase/utils/M1_restoreDB.sql`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/utils/M1_tableDict.json` & `cowbase-1.0.1/src/cowbase/utils/M1_tableDict.json`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/utils/M2_tableDict.json` & `cowbase-1.0.1/src/cowbase/utils/M2_tableDict.json`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/utils/M3_tableDict.json` & `cowbase-1.0.1/src/cowbase/utils/M3_tableDict.json`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/utils/M4_sqlupdate.json` & `cowbase-1.0.1/src/cowbase/utils/M4_sqlupdate.json`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase/utils/M4_tableDict.json` & `cowbase-1.0.1/src/cowbase/utils/M4_tableDict.json`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase.egg-info/PKG-INFO` & `cowbase-1.0.1/src/cowbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowbase
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for data processing of Automatic Milking System data
 Author-email: Martin Julius Gote <martin.gote@kuleuven.be>
 License: MIT License
         
         Copyright (c) 2024 Martin Gote
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cowbase-1.0.0/src/cowbase.egg-info/SOURCES.txt` & `cowbase-1.0.1/src/cowbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cowbase-1.0.0/src/cowbase.egg-info/requires.txt` & `cowbase-1.0.1/src/cowbase.egg-info/requires.txt`

 * *Files identical despite different names*

