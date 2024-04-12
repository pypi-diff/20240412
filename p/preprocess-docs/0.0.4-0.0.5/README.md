# Comparing `tmp/preprocess-docs-0.0.4.tar.gz` & `tmp/preprocess-docs-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preprocess-docs-0.0.4.tar", last modified: Fri Apr 12 04:38:47 2024, max compression
+gzip compressed data, was "preprocess-docs-0.0.5.tar", last modified: Fri Apr 12 05:14:19 2024, max compression
```

## Comparing `preprocess-docs-0.0.4.tar` & `preprocess-docs-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.281505 preprocess-docs-0.0.4/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 03:51:18.000000 preprocess-docs-0.0.4/LICENSE
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 04:38:47.281336 preprocess-docs-0.0.4/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-12 03:51:17.000000 preprocess-docs-0.0.4/README.md
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.280217 preprocess-docs-0.0.4/preprocess/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       78 2024-04-12 03:51:25.000000 preprocess-docs-0.0.4/preprocess/__init__.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      685 2024-04-12 04:35:52.000000 preprocess-docs-0.0.4/preprocess/element.py
--rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 04:35:47.000000 preprocess-docs-0.0.4/preprocess/html.py
-drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 04:38:47.281091 preprocess-docs-0.0.4/preprocess_docs.egg-info/
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/PKG-INFO
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      284 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/SOURCES.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/dependency_links.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       15 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/requires.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-12 04:38:47.000000 preprocess-docs-0.0.4/preprocess_docs.egg-info/top_level.txt
--rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-12 04:38:47.281571 preprocess-docs-0.0.4/setup.cfg
--rw-r--r--   0 edchin   (404365) primarygroup (89939)      696 2024-04-12 04:38:35.000000 preprocess-docs-0.0.4/setup.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 05:14:19.519540 preprocess-docs-0.0.5/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 03:51:18.000000 preprocess-docs-0.0.5/LICENSE
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 05:14:19.519294 preprocess-docs-0.0.5/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      310 2024-04-12 03:51:17.000000 preprocess-docs-0.0.5/README.md
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 05:14:19.518248 preprocess-docs-0.0.5/preprocess/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       99 2024-04-12 04:57:22.000000 preprocess-docs-0.0.5/preprocess/__init__.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      685 2024-04-12 04:35:52.000000 preprocess-docs-0.0.5/preprocess/element.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)     1065 2024-04-12 04:35:47.000000 preprocess-docs-0.0.5/preprocess/html.py
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      217 2024-04-12 05:03:12.000000 preprocess-docs-0.0.5/preprocess/pdf.py
+drwxr-xr-x   0 edchin   (404365) primarygroup (89939)        0 2024-04-12 05:14:19.519060 preprocess-docs-0.0.5/preprocess_docs.egg-info/
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      722 2024-04-12 05:14:19.000000 preprocess-docs-0.0.5/preprocess_docs.egg-info/PKG-INFO
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      302 2024-04-12 05:14:19.000000 preprocess-docs-0.0.5/preprocess_docs.egg-info/SOURCES.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)        1 2024-04-12 05:14:19.000000 preprocess-docs-0.0.5/preprocess_docs.egg-info/dependency_links.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       28 2024-04-12 05:14:19.000000 preprocess-docs-0.0.5/preprocess_docs.egg-info/requires.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       11 2024-04-12 05:14:19.000000 preprocess-docs-0.0.5/preprocess_docs.egg-info/top_level.txt
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)       38 2024-04-12 05:14:19.519596 preprocess-docs-0.0.5/setup.cfg
+-rw-r--r--   0 edchin   (404365) primarygroup (89939)      718 2024-04-12 05:13:59.000000 preprocess-docs-0.0.5/setup.py
```

### Comparing `preprocess-docs-0.0.4/LICENSE` & `preprocess-docs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.4/PKG-INFO` & `preprocess-docs-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.4
+Version: 0.0.5
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.4/preprocess/element.py` & `preprocess-docs-0.0.5/preprocess/element.py`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.4/preprocess/html.py` & `preprocess-docs-0.0.5/preprocess/html.py`

 * *Files identical despite different names*

### Comparing `preprocess-docs-0.0.4/preprocess_docs.egg-info/PKG-INFO` & `preprocess-docs-0.0.5/preprocess_docs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preprocess-docs
-Version: 0.0.4
+Version: 0.0.5
 Summary: An open source document preprocessor for AI.
 Home-page: https://github.com/eddyjin1/preprocess
 Author: Eddy Jin
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `preprocess-docs-0.0.4/setup.py` & `preprocess-docs-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="preprocess-docs",
-    version="0.0.4",
+    version="0.0.5",
     author="Eddy Jin",
     description="An open source document preprocessor for AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eddyjin1/preprocess",
     packages=setuptools.find_packages(),
     install_requires = [
       "beautifulsoup4",
+      "pdfminer.six",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

