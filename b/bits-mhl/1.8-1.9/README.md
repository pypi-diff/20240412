# Comparing `tmp/bits-mhl-1.8.tar.gz` & `tmp/bits-mhl-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bits-mhl-1.8.tar", last modified: Wed Aug 29 21:03:27 2018, max compression
+gzip compressed data, was "dist/bits-mhl-1.9.tar", last modified: Thu Aug 30 02:48:07 2018, max compression
```

## Comparing `bits-mhl-1.8.tar` & `bits-mhl-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-29 21:03:27.000000 bits-mhl-1.8/
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)      968 2018-08-29 21:03:24.000000 bits-mhl-1.8/setup.py
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)       38 2018-08-29 21:03:27.000000 bits-mhl-1.8/setup.cfg
-drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)        8 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/requires.txt
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)        1 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/dependency_links.txt
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)        1 2018-08-24 04:50:21.000000 bits-mhl-1.8/bits_mhl.egg-info/not-zip-safe
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)      224 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/PKG-INFO
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)        5 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/top_level.txt
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)      264 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits_mhl.egg-info/SOURCES.txt
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)      224 2018-08-29 21:03:27.000000 bits-mhl-1.8/PKG-INFO
-drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits/
-drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-29 21:03:27.000000 bits-mhl-1.8/bits/mhl/
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)    13694 2018-08-29 21:03:24.000000 bits-mhl-1.8/bits/mhl/types.py
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)    21098 2018-08-28 20:08:06.000000 bits-mhl-1.8/bits/mhl/__init__.py
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)       65 2018-08-18 22:04:03.000000 bits-mhl-1.8/bits/__init__.py
--rw-r--r--   0 karlsson  (1000) karlsson  (1001)       35 2018-08-18 21:44:59.000000 bits-mhl-1.8/README.md
+drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-30 02:48:07.000000 bits-mhl-1.9/
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)      968 2018-08-30 02:47:28.000000 bits-mhl-1.9/setup.py
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)       38 2018-08-30 02:48:07.000000 bits-mhl-1.9/setup.cfg
+drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)        8 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/requires.txt
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)        1 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/dependency_links.txt
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)        1 2018-08-24 04:50:21.000000 bits-mhl-1.9/bits_mhl.egg-info/not-zip-safe
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)      224 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/PKG-INFO
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)        5 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/top_level.txt
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)      264 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits_mhl.egg-info/SOURCES.txt
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)      224 2018-08-30 02:48:07.000000 bits-mhl-1.9/PKG-INFO
+drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits/
+drwxr-sr-x   0 karlsson  (1000) karlsson  (1001)        0 2018-08-30 02:48:07.000000 bits-mhl-1.9/bits/mhl/
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)    13694 2018-08-29 21:03:24.000000 bits-mhl-1.9/bits/mhl/types.py
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)    21121 2018-08-30 02:47:28.000000 bits-mhl-1.9/bits/mhl/__init__.py
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)       65 2018-08-18 22:04:03.000000 bits-mhl-1.9/bits/__init__.py
+-rw-r--r--   0 karlsson  (1000) karlsson  (1001)       35 2018-08-18 21:44:59.000000 bits-mhl-1.9/README.md
```

### Comparing `bits-mhl-1.8/setup.py` & `bits-mhl-1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from setuptools import setup, find_packages
 
 
 setup(
     name='bits-mhl',
 
-    version='1.8',
+    version='1.9',
 
     description='BITS MHL',
     long_description='',
 
     author='Lukas Karlsson',
     author_email='karlsson@broadinstitute.org',
```

### Comparing `bits-mhl-1.8/bits/mhl/types.py` & `bits-mhl-1.9/bits/mhl/types.py`

 * *Files identical despite different names*

### Comparing `bits-mhl-1.8/bits/mhl/__init__.py` & `bits-mhl-1.9/bits/mhl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,16 @@
         self.types = self.get_types()
 
         # check for errors, warnings and duplicates
         self.check_lines()
         self.check_duplicates()
 
         # if we have people data, let's add emplids to all our host records
-        self.insert_emplids(people)
+        if people:
+            self.insert_emplids(people)
 
         # errors and warnings
         self.errors = self.get_errors()
         self.warnings = self.get_warnings()
 
     def check_commented(self):
         """Check all the commented rows in the file."""
```

