# Comparing `tmp/pes-innovation-lab-hunt-1.2.tar.gz` & `tmp/pes-innovation-lab-hunt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pes-innovation-lab-hunt-1.2.tar", last modified: Fri Apr 12 20:38:21 2024, max compression
+gzip compressed data, was "pes-innovation-lab-hunt-1.3.tar", last modified: Fri Apr 12 20:40:34 2024, max compression
```

## Comparing `pes-innovation-lab-hunt-1.2.tar` & `pes-innovation-lab-hunt-1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:38:21.951947 pes-innovation-lab-hunt-1.2/
--rw-r--r--   0 monish    (1000) monish    (1000)      289 2024-04-12 20:38:21.951947 pes-innovation-lab-hunt-1.2/PKG-INFO
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:38:21.950947 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt/
--rw-r--r--   0 monish    (1000) monish    (1000)      126 2024-04-10 20:28:53.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt/__init__.py
--rw-r--r--   0 monish    (1000) monish    (1000)     5234 2024-04-10 20:07:39.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt/hunt.py
-drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:38:21.951947 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt.egg-info/
--rw-r--r--   0 monish    (1000) monish    (1000)      289 2024-04-12 20:38:21.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt.egg-info/PKG-INFO
--rw-r--r--   0 monish    (1000) monish    (1000)      264 2024-04-12 20:38:21.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt.egg-info/SOURCES.txt
--rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-12 20:38:21.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt.egg-info/dependency_links.txt
--rw-r--r--   0 monish    (1000) monish    (1000)       24 2024-04-12 20:38:21.000000 pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt.egg-info/top_level.txt
--rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-12 20:38:21.951947 pes-innovation-lab-hunt-1.2/setup.cfg
--rw-r--r--   0 monish    (1000) monish    (1000)      512 2024-04-12 20:38:19.000000 pes-innovation-lab-hunt-1.2/setup.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:40:34.135827 pes-innovation-lab-hunt-1.3/
+-rw-r--r--   0 monish    (1000) monish    (1000)      294 2024-04-12 20:40:34.135827 pes-innovation-lab-hunt-1.3/PKG-INFO
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:40:34.134827 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt/
+-rw-r--r--   0 monish    (1000) monish    (1000)      126 2024-04-10 20:28:53.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt/__init__.py
+-rw-r--r--   0 monish    (1000) monish    (1000)     5234 2024-04-10 20:07:39.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt/hunt.py
+drwxr-xr-x   0 monish    (1000) monish    (1000)        0 2024-04-12 20:40:34.135827 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt.egg-info/
+-rw-r--r--   0 monish    (1000) monish    (1000)      294 2024-04-12 20:40:34.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt.egg-info/PKG-INFO
+-rw-r--r--   0 monish    (1000) monish    (1000)      264 2024-04-12 20:40:34.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt.egg-info/SOURCES.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)        1 2024-04-12 20:40:34.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt.egg-info/dependency_links.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)       24 2024-04-12 20:40:34.000000 pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt.egg-info/top_level.txt
+-rw-r--r--   0 monish    (1000) monish    (1000)       38 2024-04-12 20:40:34.135827 pes-innovation-lab-hunt-1.3/setup.cfg
+-rw-r--r--   0 monish    (1000) monish    (1000)      517 2024-04-12 20:40:32.000000 pes-innovation-lab-hunt-1.3/setup.py
```

### Comparing `pes-innovation-lab-hunt-1.2/pes_innovation_lab_hunt/hunt.py` & `pes-innovation-lab-hunt-1.3/pes_innovation_lab_hunt/hunt.py`

 * *Files identical despite different names*

### Comparing `pes-innovation-lab-hunt-1.2/setup.py` & `pes-innovation-lab-hunt-1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pes-innovation-lab-hunt',
-    version='1.2',
+    version='1.3',
     packages=find_packages(),
     install_requires=[],  # Add dependencies if any
     entry_points={},
     # Metadata
     author='PES Innovation Lab',
     author_email='innovationlab@pes.edu',
-    description='Hunt package',
+    description='2024 Hunt package',
     long_description="""
 # pes_innovation_lab_hunt
 
 ```python
 import pes_innovation_lab_hunt
 # poke around and find out!
```

