# Comparing `tmp/composio_langchain-0.1.90.tar.gz` & `tmp/composio_langchain-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.90.tar", last modified: Fri Apr 12 10:06:18 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.91.tar", last modified: Fri Apr 12 10:14:49 2024, max compression
```

## Comparing `composio_langchain-0.1.90.tar` & `composio_langchain-0.1.91.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:18.397496 composio_langchain-0.1.90/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.90/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 10:06:18.397298 composio_langchain-0.1.90/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.90/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:18.396339 composio_langchain-0.1.90/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 09:34:14.000000 composio_langchain-0.1.90/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5518 2024-04-12 01:13:56.000000 composio_langchain-0.1.90/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.90/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:18.397081 composio_langchain-0.1.90/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 10:06:18.000000 composio_langchain-0.1.90/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-12 10:06:18.000000 composio_langchain-0.1.90/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:06:18.000000 composio_langchain-0.1.90/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      149 2024-04-12 10:06:18.000000 composio_langchain-0.1.90/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-12 10:06:18.000000 composio_langchain-0.1.90/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      455 2024-04-12 10:06:05.000000 composio_langchain-0.1.90/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:06:18.397538 composio_langchain-0.1.90/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-12 10:06:05.000000 composio_langchain-0.1.90/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:49.003938 composio_langchain-0.1.91/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.91/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 10:14:49.003745 composio_langchain-0.1.91/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.91/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:49.002814 composio_langchain-0.1.91/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 09:34:14.000000 composio_langchain-0.1.91/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5518 2024-04-12 01:13:56.000000 composio_langchain-0.1.91/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.91/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:49.003555 composio_langchain-0.1.91/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-12 10:14:48.000000 composio_langchain-0.1.91/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-12 10:14:49.000000 composio_langchain-0.1.91/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:14:48.000000 composio_langchain-0.1.91/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      149 2024-04-12 10:14:48.000000 composio_langchain-0.1.91/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-12 10:14:48.000000 composio_langchain-0.1.91/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      455 2024-04-12 10:14:00.000000 composio_langchain-0.1.91/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:14:49.003977 composio_langchain-0.1.91/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-12 10:14:00.000000 composio_langchain-0.1.91/setup.py
```

### Comparing `composio_langchain-0.1.90/PKG-INFO` & `composio_langchain-0.1.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.90
+Version: 0.1.91
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.90
+Requires-Dist: composio_core===0.1.91
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.90/README.md` & `composio_langchain-0.1.91/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.90/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.91/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.90/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.91/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.90/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.91/composio_langchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.90
+Version: 0.1.91
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.90
+Requires-Dist: composio_core===0.1.91
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.90/setup.py` & `composio_langchain-0.1.91/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.90",
+    version="0.1.91",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```
