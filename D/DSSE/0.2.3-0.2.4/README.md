# Comparing `tmp/DSSE-0.2.3.tar.gz` & `tmp/DSSE-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSSE-0.2.3.tar", last modified: Tue Mar 12 18:07:01 2024, max compression
+gzip compressed data, was "DSSE-0.2.4.tar", last modified: Tue Mar 12 18:39:54 2024, max compression
```

## Comparing `DSSE-0.2.3.tar` & `DSSE-0.2.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/DSSE/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      222 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/__init__.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/DSSE/environment/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/environment/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      256 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/environment/constants.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14099 2024-03-12 17:33:18.000000 DSSE-0.2.3/DSSE/environment/env.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/DSSE/environment/generator/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/environment/generator/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      348 2024-03-12 17:31:43.000000 DSSE-0.2.3/DSSE/environment/generator/circle.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5394 2024-03-12 17:31:43.000000 DSSE-0.2.3/DSSE/environment/generator/dynamic_probability.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2651 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/environment/generator/person_movement.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4447 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/environment/pygame_interface.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/DSSE/tests/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/tests/__init__.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8368 2024-03-12 14:40:14.000000 DSSE-0.2.3/DSSE/tests/test_env.py
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      594 2024-03-12 17:31:43.000000 DSSE-0.2.3/DSSE/tests/test_matrix.py
-drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:07:01.545779 DSSE-0.2.3/DSSE.egg-info/
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:07:01.000000 DSSE-0.2.3/DSSE.egg-info/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      550 2024-03-12 18:07:01.000000 DSSE-0.2.3/DSSE.egg-info/SOURCES.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-03-12 18:07:01.000000 DSSE-0.2.3/DSSE.egg-info/dependency_links.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       51 2024-03-12 18:07:01.000000 DSSE-0.2.3/DSSE.egg-info/requires.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-03-12 18:07:01.000000 DSSE-0.2.3/DSSE.egg-info/top_level.txt
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       15 2024-03-12 14:40:14.000000 DSSE-0.2.3/MANIFEST.in
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:07:01.545779 DSSE-0.2.3/PKG-INFO
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14768 2024-03-12 14:40:14.000000 DSSE-0.2.3/README.md
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-03-12 18:07:01.545779 DSSE-0.2.3/setup.cfg
--rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1072 2024-03-12 18:06:40.000000 DSSE-0.2.3/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.778095 DSSE-0.2.4/DSSE/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      222 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/__init__.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      256 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/constants.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14099 2024-03-12 17:33:18.000000 DSSE-0.2.4/DSSE/environment/env.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/generator/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/generator/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      348 2024-03-12 17:31:43.000000 DSSE-0.2.4/DSSE/environment/generator/circle.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5394 2024-03-12 17:31:43.000000 DSSE-0.2.4/DSSE/environment/generator/dynamic_probability.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2651 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/generator/person_movement.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE/environment/imgs/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:38:11.000000 DSSE-0.2.4/DSSE/environment/imgs/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/imgs/drone.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/imgs/person-swimming.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4447 2024-03-12 14:40:14.000000 DSSE-0.2.4/DSSE/environment/pygame_interface.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 18:39:54.782095 DSSE-0.2.4/DSSE.egg-info/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      586 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       51 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/requires.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-03-12 18:39:54.000000 DSSE-0.2.4/DSSE.egg-info/top_level.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       15 2024-03-12 14:40:14.000000 DSSE-0.2.4/MANIFEST.in
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    15400 2024-03-12 18:39:54.782095 DSSE-0.2.4/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14768 2024-03-12 14:40:14.000000 DSSE-0.2.4/README.md
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-03-12 18:39:54.782095 DSSE-0.2.4/setup.cfg
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1227 2024-03-12 18:39:50.000000 DSSE-0.2.4/setup.py
```

### Comparing `DSSE-0.2.3/DSSE/environment/env.py` & `DSSE-0.2.4/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.3/DSSE/environment/generator/dynamic_probability.py` & `DSSE-0.2.4/DSSE/environment/generator/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.3/DSSE/environment/generator/person_movement.py` & `DSSE-0.2.4/DSSE/environment/generator/person_movement.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.3/DSSE/environment/pygame_interface.py` & `DSSE-0.2.4/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.3/DSSE.egg-info/PKG-INFO` & `DSSE-0.2.4/DSSE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.2.3
+Version: 0.2.4
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth
 License: MIT
 Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
 Platform: UNKNOWN
```

### Comparing `DSSE-0.2.3/DSSE.egg-info/SOURCES.txt` & `DSSE-0.2.4/DSSE.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 DSSE/environment/constants.py
 DSSE/environment/env.py
 DSSE/environment/pygame_interface.py
 DSSE/environment/generator/__init__.py
 DSSE/environment/generator/circle.py
 DSSE/environment/generator/dynamic_probability.py
 DSSE/environment/generator/person_movement.py
-DSSE/tests/__init__.py
-DSSE/tests/test_env.py
-DSSE/tests/test_matrix.py
+DSSE/environment/imgs/__init__.py
+DSSE/environment/imgs/drone.png
+DSSE/environment/imgs/person-swimming.png
```

### Comparing `DSSE-0.2.3/PKG-INFO` & `DSSE-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 0.2.3
+Version: 0.2.4
 Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
 Home-page: https://github.com/pfeinsper/drone-swarm-search
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth
 License: MIT
 Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz
 Keywords: Reinforcement Learning,AI,SAR,Multi Agent
 Platform: UNKNOWN
```

### Comparing `DSSE-0.2.3/README.md` & `DSSE-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `DSSE-0.2.3/setup.py` & `DSSE-0.2.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,35 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
-download_url = "https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz"
+download_url = (
+    "https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v0.2.2.tar.gz"
+)
 setup(
     name="DSSE",
-    version="0.2.3",
+    version="0.2.4",
     author="Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Joras Oliveira, Ricardo Ribeiro Rodrigues, Renato Lafrachi Falcao, Pedro Andrade, Fabricio Barth",
     description="An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pfeinsper/drone-swarm-search",
     license="MIT",
     keywords=["Reinforcement Learning", "AI", "SAR", "Multi Agent"],
     download_url=download_url,
+    packages=[
+        "DSSE",
+        "DSSE.environment",
+        "DSSE.environment.imgs",
+        "DSSE.environment.generator",
+    ],
     include_package_data=True,
-    packages=find_packages(),
+    package_data={"DSSE": ["environment/imgs/*.png"]},
     install_requires=[
         "numpy",
         "gymnasium",
         "pygame",
         "pettingzoo",
         "matplotlib",
         "numba",
```

