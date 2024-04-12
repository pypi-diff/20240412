# Comparing `tmp/nttl-0.3.0.tar.gz` & `tmp/nttl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nttl-0.3.0.tar", last modified: Wed Mar 27 09:44:30 2024, max compression
+gzip compressed data, was "nttl-0.3.1.tar", last modified: Fri Apr 12 20:08:37 2024, max compression
```

## Comparing `nttl-0.3.0.tar` & `nttl-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2024-03-27 09:44:30.884284 nttl-0.3.0/
--rw-r--r--   0 robertl   (1000) robertl   (1000)    32424 2024-01-15 06:28:31.000000 nttl-0.3.0/LICENSE
--rw-r--r--   0 robertl   (1000) robertl   (1000)    12698 2024-03-27 09:44:30.884284 nttl-0.3.0/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)    12403 2024-02-08 09:55:18.000000 nttl-0.3.0/README.md
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2024-03-27 09:44:30.880950 nttl-0.3.0/nttl/
--rw-r--r--   0 robertl   (1000) robertl   (1000)       65 2024-01-15 06:28:31.000000 nttl-0.3.0/nttl/__init__.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     5469 2024-02-27 07:36:47.000000 nttl-0.3.0/nttl/data.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     4857 2024-02-13 06:46:30.000000 nttl-0.3.0/nttl/dt.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)    11407 2024-03-27 09:37:57.000000 nttl-0.3.0/nttl/main.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)     9567 2024-03-01 07:08:09.000000 nttl-0.3.0/nttl/report.py
--rw-r--r--   0 robertl   (1000) robertl   (1000)       23 2024-03-27 09:40:34.000000 nttl-0.3.0/nttl/version.py
-drwxr-xr-x   0 robertl   (1000) robertl   (1000)        0 2024-03-27 09:44:30.884284 nttl-0.3.0/nttl.egg-info/
--rw-r--r--   0 robertl   (1000) robertl   (1000)    12698 2024-03-27 09:44:30.000000 nttl-0.3.0/nttl.egg-info/PKG-INFO
--rw-r--r--   0 robertl   (1000) robertl   (1000)      279 2024-03-27 09:44:30.000000 nttl-0.3.0/nttl.egg-info/SOURCES.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        1 2024-03-27 09:44:30.000000 nttl-0.3.0/nttl.egg-info/dependency_links.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       39 2024-03-27 09:44:30.000000 nttl-0.3.0/nttl.egg-info/entry_points.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)        5 2024-03-27 09:44:30.000000 nttl-0.3.0/nttl.egg-info/top_level.txt
--rw-r--r--   0 robertl   (1000) robertl   (1000)       50 2024-01-15 06:28:31.000000 nttl-0.3.0/pyproject.toml
--rw-r--r--   0 robertl   (1000) robertl   (1000)      541 2024-03-27 09:44:30.884284 nttl-0.3.0/setup.cfg
--rw-r--r--   0 robertl   (1000) robertl   (1000)       38 2024-01-15 06:28:31.000000 nttl-0.3.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 20:08:37.126795 nttl-0.3.1/
+-rw-r--r--   0 robert    (1000) robert    (1000)    32424 2024-01-13 09:52:28.000000 nttl-0.3.1/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)    12698 2024-04-12 20:08:37.126795 nttl-0.3.1/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)    12403 2024-02-02 22:05:17.000000 nttl-0.3.1/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 20:08:37.126795 nttl-0.3.1/nttl/
+-rw-r--r--   0 robert    (1000) robert    (1000)       65 2024-01-13 19:43:05.000000 nttl-0.3.1/nttl/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     5469 2024-02-20 07:46:00.000000 nttl-0.3.1/nttl/data.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4857 2024-04-09 19:32:24.000000 nttl-0.3.1/nttl/dt.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    11407 2024-04-09 19:32:24.000000 nttl-0.3.1/nttl/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9567 2024-04-09 19:32:24.000000 nttl-0.3.1/nttl/report.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2024-04-09 19:32:24.000000 nttl-0.3.1/nttl/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2024-04-12 20:08:37.126795 nttl-0.3.1/nttl.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)    12698 2024-04-12 20:08:37.000000 nttl-0.3.1/nttl.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      279 2024-04-12 20:08:37.000000 nttl-0.3.1/nttl.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2024-04-12 20:08:37.000000 nttl-0.3.1/nttl.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       39 2024-04-12 20:08:37.000000 nttl-0.3.1/nttl.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        5 2024-04-12 20:08:37.000000 nttl-0.3.1/nttl.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-08-26 10:08:17.000000 nttl-0.3.1/pyproject.toml
+-rw-r--r--   0 robert    (1000) robert    (1000)      541 2024-04-12 20:08:37.126795 nttl-0.3.1/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-08-26 10:08:39.000000 nttl-0.3.1/setup.py
```

### Comparing `nttl-0.3.0/LICENSE` & `nttl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nttl-0.3.0/PKG-INFO` & `nttl-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nttl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tiny time tracker for the commandline
 Home-page: https://vonshednob.cc/nttl/
 Author: R
 Author-email: contact+nttl@vonshednob.cc
 License: GPL version 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `nttl-0.3.0/README.md` & `nttl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nttl-0.3.0/nttl/data.py` & `nttl-0.3.1/nttl/data.py`

 * *Files identical despite different names*

### Comparing `nttl-0.3.0/nttl/dt.py` & `nttl-0.3.1/nttl/dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
                                                            month=now.month,
                                                            day=now.day)
     elif len(value) == 8:
         return datetime.datetime.strptime(value,
                                           '%H:%M:%S').replace(year=now.year,
                                                               month=now.month,
                                                               day=now.day)
-    elif len(value) == 17:
+    elif len(value) == 16:
         return datetime.datetime.strptime(value, '%Y-%m-%d %H:%M')
     elif len(value) == 19:
         return datetime.datetime.strptime(value, '%Y-%m-%d %H:%M:%S')
 
     raise ValueError(f"Don't know the time format '{value}'")
```

### Comparing `nttl-0.3.0/nttl/main.py` & `nttl-0.3.1/nttl/main.py`

 * *Files identical despite different names*

### Comparing `nttl-0.3.0/nttl/report.py` & `nttl-0.3.1/nttl/report.py`

 * *Files identical despite different names*

### Comparing `nttl-0.3.0/nttl.egg-info/PKG-INFO` & `nttl-0.3.1/nttl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nttl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tiny time tracker for the commandline
 Home-page: https://vonshednob.cc/nttl/
 Author: R
 Author-email: contact+nttl@vonshednob.cc
 License: GPL version 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `nttl-0.3.0/setup.cfg` & `nttl-0.3.1/setup.cfg`

 * *Files identical despite different names*

