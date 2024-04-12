# Comparing `tmp/composio_lyzr-0.1.98.tar.gz` & `tmp/composio_lyzr-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_lyzr-0.1.98.tar", last modified: Fri Apr 12 15:21:48 2024, max compression
+gzip compressed data, was "composio_lyzr-0.1.99.tar", last modified: Fri Apr 12 15:24:47 2024, max compression
```

## Comparing `composio_lyzr-0.1.98.tar` & `composio_lyzr-0.1.99.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:21:48.719695 composio_lyzr-0.1.98/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:05:13.000000 composio_lyzr-0.1.98/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     2717 2024-04-12 15:21:48.719524 composio_lyzr-0.1.98/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2122 2024-04-12 15:05:51.000000 composio_lyzr-0.1.98/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:21:48.718416 composio_lyzr-0.1.98/composio_lyzr/
--rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 15:03:16.000000 composio_lyzr-0.1.98/composio_lyzr/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5498 2024-04-12 15:21:00.000000 composio_lyzr-0.1.98/composio_lyzr/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-04-12 13:36:37.000000 composio_lyzr-0.1.98/composio_lyzr/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:21:48.719339 composio_lyzr-0.1.98/composio_lyzr.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2717 2024-04-12 15:21:48.000000 composio_lyzr-0.1.98/composio_lyzr.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      323 2024-04-12 15:21:48.000000 composio_lyzr-0.1.98/composio_lyzr.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:21:48.000000 composio_lyzr-0.1.98/composio_lyzr.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       77 2024-04-12 15:21:48.000000 composio_lyzr-0.1.98/composio_lyzr.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       14 2024-04-12 15:21:48.000000 composio_lyzr-0.1.98/composio_lyzr.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      343 2024-04-12 15:21:08.000000 composio_lyzr-0.1.98/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:21:48.719734 composio_lyzr-0.1.98/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      838 2024-04-12 15:21:08.000000 composio_lyzr-0.1.98/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:47.047424 composio_lyzr-0.1.99/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:05:13.000000 composio_lyzr-0.1.99/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2717 2024-04-12 15:24:47.047215 composio_lyzr-0.1.99/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2122 2024-04-12 15:05:51.000000 composio_lyzr-0.1.99/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:47.045983 composio_lyzr-0.1.99/composio_lyzr/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 15:03:16.000000 composio_lyzr-0.1.99/composio_lyzr/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5498 2024-04-12 15:21:00.000000 composio_lyzr-0.1.99/composio_lyzr/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-04-12 13:36:37.000000 composio_lyzr-0.1.99/composio_lyzr/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:24:47.046997 composio_lyzr-0.1.99/composio_lyzr.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2717 2024-04-12 15:24:47.000000 composio_lyzr-0.1.99/composio_lyzr.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      323 2024-04-12 15:24:47.000000 composio_lyzr-0.1.99/composio_lyzr.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:24:47.000000 composio_lyzr-0.1.99/composio_lyzr.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       77 2024-04-12 15:24:47.000000 composio_lyzr-0.1.99/composio_lyzr.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       14 2024-04-12 15:24:47.000000 composio_lyzr-0.1.99/composio_lyzr.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      343 2024-04-12 15:24:05.000000 composio_lyzr-0.1.99/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:24:47.047481 composio_lyzr-0.1.99/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      838 2024-04-12 15:24:05.000000 composio_lyzr-0.1.99/setup.py
```

### Comparing `composio_lyzr-0.1.98/PKG-INFO` & `composio_lyzr-0.1.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.1.98
+Version: 0.1.99
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.98
+Requires-Dist: composio_core===0.1.99
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.1.98/README.md` & `composio_lyzr-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.1.98/composio_lyzr/composio_tool_spec.py` & `composio_lyzr-0.1.99/composio_lyzr/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.1.98/composio_lyzr/pydantic_utils.py` & `composio_lyzr-0.1.99/composio_lyzr/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.1.98/composio_lyzr.egg-info/PKG-INFO` & `composio_lyzr-0.1.99/composio_lyzr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.1.98
+Version: 0.1.99
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.98
+Requires-Dist: composio_core===0.1.99
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.1.98/setup.py` & `composio_lyzr-0.1.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_lyzr",
-    version="0.1.98",
+    version="0.1.99",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Lyzr workflow.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

