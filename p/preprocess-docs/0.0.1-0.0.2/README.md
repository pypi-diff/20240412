# Comparing `tmp/preprocess-docs-0.0.1.tar.gz` & `tmp/preprocess-docs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocess-docs-0.0.1.tar", last modified: Thu Apr 11 18:05:36 2024, max compression
+gzip compressed data, was "preprocess-docs-0.0.2.tar", last modified: Thu Apr 11 18:08:05 2024, max compression
```

## Comparing `preprocess-docs-0.0.1.tar` & `preprocess-docs-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:05:36.448842 preprocess-docs-0.0.1/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-11 17:35:45.000000 preprocess-docs-0.0.1/LICENSE
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      707 2024-04-11 18:05:36.448608 preprocess-docs-0.0.1/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      308 2024-04-11 18:04:46.000000 preprocess-docs-0.0.1/README.md
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:05:36.447110 preprocess-docs-0.0.1/preprocess/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       27 2024-04-11 17:35:45.000000 preprocess-docs-0.0.1/preprocess/__init__.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      273 2024-04-11 17:35:45.000000 preprocess-docs-0.0.1/preprocess/client.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      688 2024-04-11 17:35:45.000000 preprocess-docs-0.0.1/preprocess/collection.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       39 2024-04-11 17:35:45.000000 preprocess-docs-0.0.1/preprocess/query_result.py
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:05:36.447788 preprocess-docs-0.0.1/preprocess_docs.egg-info/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      707 2024-04-11 18:05:36.000000 preprocess-docs-0.0.1/preprocess_docs.egg-info/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      278 2024-04-11 18:05:36.000000 preprocess-docs-0.0.1/preprocess_docs.egg-info/SOURCES.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-11 18:05:36.000000 preprocess-docs-0.0.1/preprocess_docs.egg-info/dependency_links.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-11 18:05:36.000000 preprocess-docs-0.0.1/preprocess_docs.egg-info/top_level.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-11 18:05:36.448918 preprocess-docs-0.0.1/setup.cfg
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      654 2024-04-11 18:05:12.000000 preprocess-docs-0.0.1/setup.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.493916 preprocess-docs-0.0.2/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/LICENSE
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-11 18:08:05.493762 preprocess-docs-0.0.2/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-11 18:07:33.000000 preprocess-docs-0.0.2/README.md
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.492863 preprocess-docs-0.0.2/preprocess/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       27 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/__init__.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      273 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/client.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      688 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/collection.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       39 2024-04-11 17:35:45.000000 preprocess-docs-0.0.2/preprocess/query_result.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-11 18:08:05.493518 preprocess-docs-0.0.2/preprocess_docs.egg-info/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      278 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-11 18:08:05.000000 preprocess-docs-0.0.2/preprocess_docs.egg-info/top_level.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-11 18:08:05.493983 preprocess-docs-0.0.2/setup.cfg
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      667 2024-04-11 18:08:02.000000 preprocess-docs-0.0.2/setup.py
```

### Comparing `preprocess-docs-0.0.1/LICENSE` & `preprocess-docs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.1/PKG-INFO` & `preprocess-docs-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.1
-Summary: A document preprocessor for AI.
+Version: 0.0.2
+Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # preprocess
 
-An open source vector embeddings database.
+An open source document preprocessor for AI.
 https://www.preprocess.net
 
 https://pypi.org/project/preprocess-docs/
 
 ```python
 pip install preprocess-docs
 ```
```

### Comparing `preprocess-docs-0.0.1/preprocess/collection.py` & `preprocess-docs-0.0.2/preprocess/collection.py`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.1/preprocess_docs.egg-info/PKG-INFO` & `preprocess-docs-0.0.2/preprocess_docs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.1
-Summary: A document preprocessor for AI.
+Version: 0.0.2
+Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # preprocess
 
-An open source vector embeddings database.
+An open source document preprocessor for AI.
 https://www.preprocess.net
 
 https://pypi.org/project/preprocess-docs/
 
 ```python
 pip install preprocess-docs
 ```
```

### Comparing `preprocess-docs-0.0.1/setup.py` & `preprocess-docs-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="preprocess-docs",
-    version="0.0.1",
+    version="0.0.2",
     author="Eddy Jin",
-    description="A document preprocessor for AI.",
+    description="An open source document preprocessor for AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eddyjin1/preprocess",
     packages=setuptools.find_packages(),
     install_requires = [],
     classifiers=[
         "Programming Language :: Python :: 3",
```

