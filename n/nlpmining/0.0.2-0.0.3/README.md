# Comparing `tmp/nlpmining-0.0.2.tar.gz` & `tmp/nlpmining-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpmining-0.0.2.tar", last modified: Thu Apr 11 19:30:45 2024, max compression
+gzip compressed data, was "nlpmining-0.0.3.tar", last modified: Thu Apr 11 19:34:13 2024, max compression
```

## Comparing `nlpmining-0.0.2.tar` & `nlpmining-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 19:30:45.453703 nlpmining-0.0.2/
--rw-rw-rw-   0        0        0     1077 2024-04-11 18:56:18.000000 nlpmining-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      459 2024-04-11 19:30:45.453703 nlpmining-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      102 2024-04-11 18:57:55.000000 nlpmining-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 19:30:45.422883 nlpmining-0.0.2/nlpmining/
-drwxrwxrwx   0        0        0        0 2024-04-11 19:30:45.450575 nlpmining-0.0.2/nlpmining/src/
-drwxrwxrwx   0        0        0        0 2024-04-11 19:30:45.450575 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/
--rw-rw-rw-   0        0        0      459 2024-04-11 19:30:45.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2024-04-11 19:30:45.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 19:30:45.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 19:30:45.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-11 19:30:45.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    21171 2024-04-11 19:00:47.000000 nlpmining-0.0.2/nlpmining/src/nlpmining.py
--rw-rw-rw-   0        0        0       42 2024-04-11 19:30:45.456151 nlpmining-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1215 2024-04-11 19:30:28.000000 nlpmining-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 19:34:13.908250 nlpmining-0.0.3/
+-rw-rw-rw-   0        0        0     1077 2024-04-11 18:56:18.000000 nlpmining-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      459 2024-04-11 19:34:13.908250 nlpmining-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      102 2024-04-11 18:57:55.000000 nlpmining-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 19:34:13.876706 nlpmining-0.0.3/nlpmining/
+drwxrwxrwx   0        0        0        0 2024-04-11 19:34:13.908250 nlpmining-0.0.3/nlpmining/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 19:34:13.908250 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/
+-rw-rw-rw-   0        0        0      459 2024-04-11 19:34:13.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2024-04-11 19:34:13.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 19:34:13.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-11 19:34:13.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-11 19:34:13.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    21171 2024-04-11 19:00:47.000000 nlpmining-0.0.3/nlpmining/src/nlpmining.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 19:34:13.908250 nlpmining-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1215 2024-04-11 19:34:07.000000 nlpmining-0.0.3/setup.py
```

### Comparing `nlpmining-0.0.2/LICENSE.txt` & `nlpmining-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nlpmining-0.0.2/nlpmining/src/nlpmining.egg-info/SOURCES.txt` & `nlpmining-0.0.3/nlpmining/src/nlpmining.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlpmining-0.0.2/nlpmining/src/nlpmining.py` & `nlpmining-0.0.3/nlpmining/src/nlpmining.py`

 * *Files identical despite different names*

### Comparing `nlpmining-0.0.2/setup.py` & `nlpmining-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nlpmining",                     # This is the name of the package
-    version="0.0.2",                        # The initial release version
+    version="0.0.3",                        # The initial release version
     author="NLP Mining",                     # Full name of the author
     description="Text Preprocessing  package",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

