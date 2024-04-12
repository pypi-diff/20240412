# Comparing `tmp/snake_environment-0.1.6.tar.gz` & `tmp/snake_environment-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.1.6.tar", last modified: Fri Apr 12 18:07:44 2024, max compression
+gzip compressed data, was "snake_environment-0.1.8.tar", last modified: Fri Apr 12 18:12:55 2024, max compression
```

## Comparing `snake_environment-0.1.6.tar` & `snake_environment-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.100593 snake_environment-0.1.6/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:07:44.100593 snake_environment-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-12 17:25:27.000000 snake_environment-0.1.6/README.md
--rw-rw-rw-   0        0        0      708 2024-04-12 18:07:35.000000 snake_environment-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 18:07:44.100593 snake_environment-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.083740 snake_environment-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.088761 snake_environment-0.1.6/src/snake_environment/
--rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.1.6/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.097274 snake_environment-0.1.6/src/snake_environment/game/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.1.6/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.1.6/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     6705 2024-04-12 17:06:22.000000 snake_environment-0.1.6/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.099268 snake_environment-0.1.6/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.1.6/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      772 2024-04-12 17:06:22.000000 snake_environment-0.1.6/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:07:44.099268 snake_environment-0.1.6/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:07:44.000000 snake_environment-0.1.6/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-12 18:07:44.000000 snake_environment-0.1.6/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:07:44.000000 snake_environment-0.1.6/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 18:07:44.000000 snake_environment-0.1.6/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 18:07:44.000000 snake_environment-0.1.6/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.407910 snake_environment-0.1.8/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1010 2024-04-12 18:12:55.406421 snake_environment-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-12 17:25:27.000000 snake_environment-0.1.8/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-12 18:12:41.000000 snake_environment-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:12:55.407910 snake_environment-0.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.393394 snake_environment-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.397342 snake_environment-0.1.8/src/snake_environment/
+-rw-rw-rw-   0        0        0      118 2024-04-12 18:06:25.000000 snake_environment-0.1.8/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.403923 snake_environment-0.1.8/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.1.8/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.1.8/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     6679 2024-04-12 18:11:20.000000 snake_environment-0.1.8/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.404991 snake_environment-0.1.8/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.1.8/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      763 2024-04-12 18:11:57.000000 snake_environment-0.1.8/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:12:55.406421 snake_environment-0.1.8/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     1010 2024-04-12 18:12:55.000000 snake_environment-0.1.8/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-12 18:12:55.000000 snake_environment-0.1.8/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 18:12:55.000000 snake_environment-0.1.8/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 18:12:55.000000 snake_environment-0.1.8/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 18:12:55.000000 snake_environment-0.1.8/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.1.6/LICENSE` & `snake_environment-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.6/PKG-INFO` & `snake_environment-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.1.6
+Version: 0.1.8
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snake_environment-0.1.6/pyproject.toml` & `snake_environment-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.1.6"
+version = "0.1.8"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.1.6/src/snake_environment/game/objects.py` & `snake_environment-0.1.8/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.6/src/snake_environment/game/snake_game.py` & `snake_environment-0.1.8/src/snake_environment/game/snake_game.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pygame
 import random
 import numpy as np
-from src.snake_environment.game.objects import Snake, Food
+from .objects import Snake, Food
 
 WINDOW_WIDTH = 800
 WINDOW_HEIGHT = 600
 
 
 class SnakeGame:
     def __init__(self, render=False):
```

### Comparing `snake_environment-0.1.6/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.1.8/src/snake_environment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.1.6
+Version: 0.1.8
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

