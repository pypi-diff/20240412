# Comparing `tmp/endersutils-0.5.1.tar.gz` & `tmp/endersutils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endersutils-0.5.1.tar", last modified: Fri Apr 12 10:47:39 2024, max compression
+gzip compressed data, was "endersutils-0.5.2.tar", last modified: Fri Apr 12 10:57:36 2024, max compression
```

## Comparing `endersutils-0.5.1.tar` & `endersutils-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.435753 endersutils-0.5.1/
--rw-rw-rw-   0        0        0      824 2024-04-12 10:47:39.434749 endersutils-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-03-10 11:14:59.000000 endersutils-0.5.1/README.md
--rw-rw-rw-   0        0        0      701 2024-04-12 10:46:43.000000 endersutils-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 10:47:39.435753 endersutils-0.5.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.360221 endersutils-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.366552 endersutils-0.5.1/src/endersutils/
--rw-rw-rw-   0        0        0     1094 2024-03-10 11:09:16.000000 endersutils-0.5.1/src/endersutils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.408548 endersutils-0.5.1/src/endersutils/el_classes/
--rw-rw-rw-   0        0        0     1107 2023-12-12 18:27:06.000000 endersutils-0.5.1/src/endersutils/el_classes/component.py
--rw-rw-rw-   0        0        0     2872 2024-01-08 18:14:30.000000 endersutils-0.5.1/src/endersutils/el_classes/game.py
--rw-rw-rw-   0        0        0     2978 2024-03-10 08:44:22.000000 endersutils-0.5.1/src/endersutils/el_classes/gameobjects.py
--rw-rw-rw-   0        0        0     2999 2024-03-10 08:49:22.000000 endersutils-0.5.1/src/endersutils/el_classes/physics.py
--rw-rw-rw-   0        0        0     3004 2024-04-12 10:45:34.000000 endersutils-0.5.1/src/endersutils/el_classes/player.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.422482 endersutils-0.5.1/src/endersutils/el_funcs/
--rw-rw-rw-   0        0        0      325 2024-01-08 17:58:03.000000 endersutils-0.5.1/src/endersutils/el_funcs/getallindir.py
--rw-rw-rw-   0        0        0      339 2024-03-10 08:48:11.000000 endersutils-0.5.1/src/endersutils/el_funcs/getobjectsbyclass.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.432710 endersutils-0.5.1/src/endersutils/el_globs/
--rw-rw-rw-   0        0        0       41 2024-03-10 09:05:53.000000 endersutils-0.5.1/src/endersutils/el_globs/globs.py
-drwxrwxrwx   0        0        0        0 2024-04-12 10:47:39.433744 endersutils-0.5.1/src/endersutils.egg-info/
--rw-rw-rw-   0        0        0      824 2024-04-12 10:47:39.000000 endersutils-0.5.1/src/endersutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2024-04-12 10:47:39.000000 endersutils-0.5.1/src/endersutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 10:47:39.000000 endersutils-0.5.1/src/endersutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-12 10:47:39.000000 endersutils-0.5.1/src/endersutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.387027 endersutils-0.5.2/
+-rw-rw-rw-   0        0        0      824 2024-04-12 10:57:36.386025 endersutils-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-03-10 11:14:59.000000 endersutils-0.5.2/README.md
+-rw-rw-rw-   0        0        0      701 2024-04-12 10:56:51.000000 endersutils-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-12 10:57:36.387027 endersutils-0.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.353913 endersutils-0.5.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.356867 endersutils-0.5.2/src/endersutils/
+-rw-rw-rw-   0        0        0     1099 2024-04-12 10:51:17.000000 endersutils-0.5.2/src/endersutils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.379027 endersutils-0.5.2/src/endersutils/el_classes/
+-rw-rw-rw-   0        0        0     1107 2023-12-12 18:27:06.000000 endersutils-0.5.2/src/endersutils/el_classes/component.py
+-rw-rw-rw-   0        0        0     2872 2024-01-08 18:14:30.000000 endersutils-0.5.2/src/endersutils/el_classes/game.py
+-rw-rw-rw-   0        0        0     2978 2024-03-10 08:44:22.000000 endersutils-0.5.2/src/endersutils/el_classes/gameobjects.py
+-rw-rw-rw-   0        0        0     2999 2024-03-10 08:49:22.000000 endersutils-0.5.2/src/endersutils/el_classes/physics.py
+-rw-rw-rw-   0        0        0     3004 2024-04-12 10:45:34.000000 endersutils-0.5.2/src/endersutils/el_classes/player.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.384024 endersutils-0.5.2/src/endersutils/el_funcs/
+-rw-rw-rw-   0        0        0      325 2024-01-08 17:58:03.000000 endersutils-0.5.2/src/endersutils/el_funcs/getallindir.py
+-rw-rw-rw-   0        0        0      339 2024-03-10 08:48:11.000000 endersutils-0.5.2/src/endersutils/el_funcs/getobjectsbyclass.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.385024 endersutils-0.5.2/src/endersutils/el_globs/
+-rw-rw-rw-   0        0        0       41 2024-03-10 09:05:53.000000 endersutils-0.5.2/src/endersutils/el_globs/globs.py
+drwxrwxrwx   0        0        0        0 2024-04-12 10:57:36.385024 endersutils-0.5.2/src/endersutils.egg-info/
+-rw-rw-rw-   0        0        0      824 2024-04-12 10:57:36.000000 endersutils-0.5.2/src/endersutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-04-12 10:57:36.000000 endersutils-0.5.2/src/endersutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 10:57:36.000000 endersutils-0.5.2/src/endersutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-12 10:57:36.000000 endersutils-0.5.2/src/endersutils.egg-info/top_level.txt
```

### Comparing `endersutils-0.5.1/PKG-INFO` & `endersutils-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endersutils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Some utility commands that aren't really too useful but I use them a lot.
 Author-email: EnderGames <business.endergames@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12.0,>=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `endersutils-0.5.1/pyproject.toml` & `endersutils-0.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "pygame",
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "endersutils"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="EnderGames", email="business.endergames@gmail.com" },
 ]
 description = "Some utility commands that aren't really too useful but I use them a lot."
 readme = "README.md"
 requires-python = ">=3.0.0, <3.12.0"
 classifiers = [
```

### Comparing `endersutils-0.5.1/src/endersutils/__init__.py` & `endersutils-0.5.2/src/endersutils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,9 +20,9 @@
         self.gameobjects = gameobjects.GameObject
         self.physics = physics.Physics
         self.player = player.Player
 
 # The main class used, although other instances can be made!
 eu = EndersUtils()
 
-if eu.intversion not in versions:
+if eu.getNumVersion() not in versions:
     raise ImportError(f"EndersUtils - Version {eu.getNumVersion()} is not up to date! Please use any of the following versions: {versions}")
```

### Comparing `endersutils-0.5.1/src/endersutils/el_classes/component.py` & `endersutils-0.5.2/src/endersutils/el_classes/component.py`

 * *Files identical despite different names*

### Comparing `endersutils-0.5.1/src/endersutils/el_classes/game.py` & `endersutils-0.5.2/src/endersutils/el_classes/game.py`

 * *Files identical despite different names*

### Comparing `endersutils-0.5.1/src/endersutils/el_classes/gameobjects.py` & `endersutils-0.5.2/src/endersutils/el_classes/gameobjects.py`

 * *Files identical despite different names*

### Comparing `endersutils-0.5.1/src/endersutils/el_classes/physics.py` & `endersutils-0.5.2/src/endersutils/el_classes/physics.py`

 * *Files identical despite different names*

### Comparing `endersutils-0.5.1/src/endersutils/el_classes/player.py` & `endersutils-0.5.2/src/endersutils/el_classes/player.py`

 * *Files identical despite different names*

### Comparing `endersutils-0.5.1/src/endersutils.egg-info/PKG-INFO` & `endersutils-0.5.2/src/endersutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endersutils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Some utility commands that aren't really too useful but I use them a lot.
 Author-email: EnderGames <business.endergames@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <3.12.0,>=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `endersutils-0.5.1/src/endersutils.egg-info/SOURCES.txt` & `endersutils-0.5.2/src/endersutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

