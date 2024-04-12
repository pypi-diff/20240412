# Comparing `tmp/jemma-0.1.420.tar.gz` & `tmp/jemma-0.1.4200.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.420.tar", last modified: Thu Apr 11 01:36:10 2024, max compression
+gzip compressed data, was "jemma-0.1.4200.tar", last modified: Thu Apr 11 01:42:31 2024, max compression
```

## Comparing `jemma-0.1.420.tar` & `jemma-0.1.4200.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.785275 jemma-0.1.420/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-11 01:36:10.784601 jemma-0.1.420/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.420/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.757615 jemma-0.1.420/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-10 04:55:55.000000 jemma-0.1.420/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.764318 jemma-0.1.420/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.766093 jemma-0.1.420/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.769306 jemma-0.1.420/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.771416 jemma-0.1.420/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.773662 jemma-0.1.420/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.780982 jemma-0.1.420/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     7571 2024-04-11 01:32:04.000000 jemma-0.1.420/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     3651 2024-04-11 01:30:43.000000 jemma-0.1.420/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.783140 jemma-0.1.420/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.420/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-10 21:15:08.000000 jemma-0.1.420/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:36:10.763304 jemma-0.1.420/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      101 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-11 01:36:10.000000 jemma-0.1.420/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-11 01:36:10.785457 jemma-0.1.420/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      469 2024-04-11 01:35:14.000000 jemma-0.1.420/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.729297 jemma-0.1.4200/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-11 01:42:31.728765 jemma-0.1.4200/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.4200/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.703963 jemma-0.1.4200/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2311 2024-04-10 04:55:55.000000 jemma-0.1.4200/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.709159 jemma-0.1.4200/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.710503 jemma-0.1.4200/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15616 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.714103 jemma-0.1.4200/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.716210 jemma-0.1.4200/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.718634 jemma-0.1.4200/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.725451 jemma-0.1.4200/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4036 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     7571 2024-04-11 01:32:04.000000 jemma-0.1.4200/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     5439 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     3651 2024-04-11 01:30:43.000000 jemma-0.1.4200/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.727534 jemma-0.1.4200/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.4200/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2698 2024-04-10 21:15:08.000000 jemma-0.1.4200/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-11 01:42:31.708523 jemma-0.1.4200/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)      102 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       86 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-11 01:42:31.000000 jemma-0.1.4200/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-11 01:42:31.729454 jemma-0.1.4200/setup.cfg
+-rw-r--r--   0 tolitius   (503) staff       (20)      470 2024-04-11 01:42:24.000000 jemma-0.1.4200/setup.py
```

### Comparing `jemma-0.1.420/README.md` & `jemma-0.1.4200/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/huddle.py` & `jemma-0.1.4200/jemma/huddle.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/prompt/business/owner.py` & `jemma-0.1.4200/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/prompt/engineer/clarify.py` & `jemma-0.1.4200/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/prompt/engineer/code.py` & `jemma-0.1.4200/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/prompt/tester/test.py` & `jemma-0.1.4200/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/requirements/feature.py` & `jemma-0.1.4200/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/team/business_owner.py` & `jemma-0.1.4200/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/team/engineer.py` & `jemma-0.1.4200/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/team/project_manager.py` & `jemma-0.1.4200/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/team/tester.py` & `jemma-0.1.4200/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/thinker.py` & `jemma-0.1.4200/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/tools.py` & `jemma-0.1.4200/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma/work/flow.py` & `jemma-0.1.4200/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.420/jemma.egg-info/SOURCES.txt` & `jemma-0.1.4200/jemma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

