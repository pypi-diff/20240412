# Comparing `tmp/preprocess-docs-0.0.2.tar.gz` & `tmp/preprocess-docs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocess-docs-0.0.2.tar", last modified: Thu Apr 11 18:08:05 2024, max compression
+gzip compressed data, was "preprocess-docs-0.0.3.tar", last modified: Fri Apr 12 03:52:27 2024, max compression
```

## Comparing `preprocess-docs-0.0.2.tar` & `preprocess-docs-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.493916 preprocess-docs-0.0.2/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/LICENSE
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-11 18:08:05.493762 preprocess-docs-0.0.2/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-11 18:07:33.000000 preprocess-docs-0.0.2/README.md
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.492863 preprocess-docs-0.0.2/preprocess/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       27 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/__init__.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      273 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/client.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      688 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/collection.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       39 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/query_result.py
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.493518 preprocess-docs-0.0.2/preprocess_docs.egg-info/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      278 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/SOURCES.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/dependency_links.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/top_level.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-11 18:08:05.493983 preprocess-docs-0.0.2/setup.cfg
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      667 2024-04-11 18:08:02.000000 preprocess-docs-0.0.2/setup.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.697692 preprocess-docs-0.0.3/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 03:51:18.000000 preprocess-docs-0.0.3/LICENSE
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 03:52:27.697524 preprocess-docs-0.0.3/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-12 03:51:17.000000 preprocess-docs-0.0.3/README.md
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.696032 preprocess-docs-0.0.3/preprocess/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       78 2024-04-12 03:51:25.000000 preprocess-docs-0.0.3/preprocess/__init__.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      685 2024-04-12 03:51:24.000000 preprocess-docs-0.0.3/preprocess/element.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1011 2024-04-12 03:51:27.000000 preprocess-docs-0.0.3/preprocess/html.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 03:52:27.696952 preprocess-docs-0.0.3/preprocess_docs.egg-info/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      284 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       15 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/requires.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-12 03:52:27.000000 preprocess-docs-0.0.3/preprocess_docs.egg-info/top_level.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-12 03:52:27.697762 preprocess-docs-0.0.3/setup.cfg
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      696 2024-04-12 03:52:07.000000 preprocess-docs-0.0.3/setup.py
```

### Comparing `preprocess-docs-0.0.2/LICENSE` & `preprocess-docs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.2/PKG-INFO` & `preprocess-docs-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.2/preprocess_docs.egg-info/PKG-INFO` & `preprocess-docs-0.0.3/preprocess_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.2
+Version: 0.0.3
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.2/setup.py` & `preprocess-docs-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="preprocess-docs",
-    version="0.0.2",
+    version="0.0.3",
     author="Eddy Jin",
     description="An open source document preprocessor for AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eddyjin1/preprocess",
     packages=setuptools.find_packages(),
-    install_requires = [],
+    install_requires = [
+      "beautifulsoup4",
+    ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

