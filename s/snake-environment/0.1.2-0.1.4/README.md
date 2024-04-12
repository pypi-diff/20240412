# Comparing `tmp/snake_environment-0.1.2.tar.gz` & `tmp/snake_environment-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snake_environment-0.1.2.tar", last modified: Fri Apr 12 18:00:07 2024, max compression
+gzip compressed data, was "snake_environment-0.1.4.tar", last modified: Fri Apr 12 18:05:06 2024, max compression
```

## Comparing `snake_environment-0.1.2.tar` & `snake_environment-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.015286 snake_environment-0.1.2/
--rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:00:07.013871 snake_environment-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      385 2024-04-12 17:25:27.000000 snake_environment-0.1.2/README.md
--rw-rw-rw-   0        0        0      708 2024-04-12 17:59:52.000000 snake_environment-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 18:00:07.015286 snake_environment-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.000406 snake_environment-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.004426 snake_environment-0.1.2/src/snake_environment/
--rw-rw-rw-   0        0        0       97 2024-04-12 17:51:42.000000 snake_environment-0.1.2/src/snake_environment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.011541 snake_environment-0.1.2/src/snake_environment/game/
--rw-rw-rw-   0        0        0       59 2024-04-12 17:59:11.000000 snake_environment-0.1.2/src/snake_environment/game/__init__.py
--rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.1.2/src/snake_environment/game/objects.py
--rw-rw-rw-   0        0        0     6705 2024-04-12 17:06:22.000000 snake_environment-0.1.2/src/snake_environment/game/snake_game.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.012573 snake_environment-0.1.2/src/snake_environment/helpers/
--rw-rw-rw-   0        0        0       56 2024-04-12 17:59:30.000000 snake_environment-0.1.2/src/snake_environment/helpers/__init__.py
--rw-rw-rw-   0        0        0      772 2024-04-12 17:06:22.000000 snake_environment-0.1.2/src/snake_environment/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-12 18:00:07.013871 snake_environment-0.1.2/src/snake_environment.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-04-12 18:00:06.000000 snake_environment-0.1.2/src/snake_environment.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2024-04-12 18:00:06.000000 snake_environment-0.1.2/src/snake_environment.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 18:00:06.000000 snake_environment-0.1.2/src/snake_environment.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-12 18:00:06.000000 snake_environment-0.1.2/src/snake_environment.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 18:00:06.000000 snake_environment-0.1.2/src/snake_environment.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.836873 snake_environment-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2024-04-12 17:28:29.000000 snake_environment-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1010 2024-04-12 18:05:06.836873 snake_environment-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-04-12 17:25:27.000000 snake_environment-0.1.4/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-12 18:04:56.000000 snake_environment-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 18:05:06.836873 snake_environment-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.825126 snake_environment-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.828781 snake_environment-0.1.4/src/snake_environment/
+-rw-rw-rw-   0        0        0      116 2024-04-12 18:04:39.000000 snake_environment-0.1.4/src/snake_environment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.834764 snake_environment-0.1.4/src/snake_environment/game/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:03.000000 snake_environment-0.1.4/src/snake_environment/game/__init__.py
+-rw-rw-rw-   0        0        0     2932 2024-04-12 14:05:08.000000 snake_environment-0.1.4/src/snake_environment/game/objects.py
+-rw-rw-rw-   0        0        0     6705 2024-04-12 17:06:22.000000 snake_environment-0.1.4/src/snake_environment/game/snake_game.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.835812 snake_environment-0.1.4/src/snake_environment/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-12 18:04:07.000000 snake_environment-0.1.4/src/snake_environment/helpers/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-04-12 17:06:22.000000 snake_environment-0.1.4/src/snake_environment/helpers/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-12 18:05:06.835812 snake_environment-0.1.4/src/snake_environment.egg-info/
+-rw-rw-rw-   0        0        0     1010 2024-04-12 18:05:06.000000 snake_environment-0.1.4/src/snake_environment.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2024-04-12 18:05:06.000000 snake_environment-0.1.4/src/snake_environment.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 18:05:06.000000 snake_environment-0.1.4/src/snake_environment.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 18:05:06.000000 snake_environment-0.1.4/src/snake_environment.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-12 18:05:06.000000 snake_environment-0.1.4/src/snake_environment.egg-info/top_level.txt
```

### Comparing `snake_environment-0.1.2/LICENSE` & `snake_environment-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.2/PKG-INFO` & `snake_environment-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.1.2
+Version: 0.1.4
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `snake_environment-0.1.2/pyproject.toml` & `snake_environment-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "snake_environment"
-version = "0.1.2"
+version = "0.1.4"
 authors = [
   { name="LPengulin", email="contact@pengulin.com" },
 ]
 description = "A simple snake environment with 18 states and 4 actions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `snake_environment-0.1.2/src/snake_environment/game/objects.py` & `snake_environment-0.1.4/src/snake_environment/game/objects.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.2/src/snake_environment/game/snake_game.py` & `snake_environment-0.1.4/src/snake_environment/game/snake_game.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.2/src/snake_environment/helpers/helpers.py` & `snake_environment-0.1.4/src/snake_environment/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `snake_environment-0.1.2/src/snake_environment.egg-info/PKG-INFO` & `snake_environment-0.1.4/src/snake_environment.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snake_environment
-Version: 0.1.2
+Version: 0.1.4
 Summary: A simple snake environment with 18 states and 4 actions
 Author-email: LPengulin <contact@pengulin.com>
 Project-URL: Homepage, https://github.com/LPengulin/Python_snake_environment
 Project-URL: Issues, https://github.com/LPengulin/Python_snake_environment/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

