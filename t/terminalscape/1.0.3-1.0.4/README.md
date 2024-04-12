# Comparing `tmp/terminalscape-1.0.3.tar.gz` & `tmp/terminalscape-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminalscape-1.0.3.tar", last modified: Fri Apr 12 14:09:06 2024, max compression
+gzip compressed data, was "terminalscape-1.0.4.tar", last modified: Fri Apr 12 14:54:19 2024, max compression
```

## Comparing `terminalscape-1.0.3.tar` & `terminalscape-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:06.864902 terminalscape-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 14:08:56.000000 terminalscape-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 14:09:06.864902 terminalscape-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 14:08:56.000000 terminalscape-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:09:06.864902 terminalscape-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-12 14:08:56.000000 terminalscape-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:06.860902 terminalscape-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-12 14:08:56.000000 terminalscape-1.0.3/src/Terminal_game.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:08:56.000000 terminalscape-1.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:09:06.864902 terminalscape-1.0.3/terminalscape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 14:09:06.000000 terminalscape-1.0.3/terminalscape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 14:09:06.000000 terminalscape-1.0.3/terminalscape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:09:06.000000 terminalscape-1.0.3/terminalscape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 14:09:06.000000 terminalscape-1.0.3/terminalscape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 14:09:06.000000 terminalscape-1.0.3/terminalscape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:19.884783 terminalscape-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 14:54:16.000000 terminalscape-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 14:54:19.884783 terminalscape-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 14:54:16.000000 terminalscape-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:54:19.884783 terminalscape-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-12 14:54:16.000000 terminalscape-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:19.884783 terminalscape-1.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-12 14:54:16.000000 terminalscape-1.0.4/src/Terminal_game.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:16.000000 terminalscape-1.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:54:19.884783 terminalscape-1.0.4/terminalscape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 14:54:19.000000 terminalscape-1.0.4/terminalscape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-12 14:54:19.000000 terminalscape-1.0.4/terminalscape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:54:19.000000 terminalscape-1.0.4/terminalscape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 14:54:19.000000 terminalscape-1.0.4/terminalscape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 14:54:19.000000 terminalscape-1.0.4/terminalscape.egg-info/top_level.txt
```

### Comparing `terminalscape-1.0.3/LICENSE` & `terminalscape-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terminalscape-1.0.3/PKG-INFO` & `terminalscape-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalscape
-Version: 1.0.3
+Version: 1.0.4
 Summary: Terminal-scape is a terminal-based game.
 Home-page: https://github.com/ImaledoShalom101/Terminal-scape
 Author: Imaledo David
 Author-email: shalomimaledo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `terminalscape-1.0.3/setup.py` & `terminalscape-1.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name="terminalscape",
-  version="1.0.3",
+  version="1.0.4",
   description="Terminal-scape is a terminal-based game.",
   long_description="Terminal-scape is a terminal-based game that engages programmers or any command line user during leisure time.",
   long_description_content_type="text/markdown",
   url="https://github.com/ImaledoShalom101/Terminal-scape",
   author="Imaledo David",
   author_email="shalomimaledo@gmail.com",
   packages=find_packages(),
@@ -14,11 +14,11 @@
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
   ],
   entry_points={
     'console_scripts': [
-      'tgmi = terminalscape.Terminal_game:commence',
+      'tgmi = terminalscape.src.Terminal_game:commence',
     ]
   },
 )
```

### Comparing `terminalscape-1.0.3/src/Terminal_game.py` & `terminalscape-1.0.4/src/Terminal_game.py`

 * *Files identical despite different names*

### Comparing `terminalscape-1.0.3/terminalscape.egg-info/PKG-INFO` & `terminalscape-1.0.4/terminalscape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminalscape
-Version: 1.0.3
+Version: 1.0.4
 Summary: Terminal-scape is a terminal-based game.
 Home-page: https://github.com/ImaledoShalom101/Terminal-scape
 Author: Imaledo David
 Author-email: shalomimaledo@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

