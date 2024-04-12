# Comparing `tmp/llama_index_experimental-0.1.2.tar.gz` & `tmp/llama_index_experimental-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_experimental-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_experimental-0.1.3.tar", max compression
```

## Comparing `llama_index_experimental-0.1.2.tar` & `llama_index_experimental-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0      262 2024-02-13 13:53:01.576384 llama_index_experimental-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-02-13 13:53:01.576473 llama_index_experimental-0.1.2/llama_index/experimental/__init__.py
--rw-r--r--   0        0        0      222 2024-02-13 13:53:01.576627 llama_index_experimental-0.1.2/llama_index/experimental/param_tuner/__init__.py
--rw-r--r--   0        0        0     9098 2024-02-13 13:53:01.576714 llama_index_experimental-0.1.2/llama_index/experimental/param_tuner/base.py
--rw-r--r--   0        0        0     1386 2024-02-22 03:29:21.920107 llama_index_experimental-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 llama_index_experimental-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      262 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/README.md
+-rw-r--r--   0        0        0      216 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/__init__.py
+-rw-r--r--   0        0        0     4640 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/exec_utils.py
+-rw-r--r--   0        0        0      222 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/param_tuner/__init__.py
+-rw-r--r--   0        0        0     9098 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/param_tuner/base.py
+-rw-r--r--   0        0        0      268 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/query_engine/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/query_engine/pandas/__init__.py
+-rw-r--r--   0        0        0     3011 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/query_engine/pandas/output_parser.py
+-rw-r--r--   0        0        0     7736 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/query_engine/pandas/pandas_query_engine.py
+-rw-r--r--   0        0        0      568 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/llama_index/experimental/query_engine/pandas/prompts.py
+-rw-r--r--   0        0        0     1386 2024-04-12 18:53:56.855891 llama_index_experimental-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 llama_index_experimental-0.1.3/PKG-INFO
```

### Comparing `llama_index_experimental-0.1.2/llama_index/experimental/param_tuner/base.py` & `llama_index_experimental-0.1.3/llama_index/experimental/param_tuner/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_experimental-0.1.2/pyproject.toml` & `llama_index_experimental-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index experimental package"
+exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-experimental"
 readme = "README.md"
-version = "0.1.2"
-exclude = ["**/BUILD"]
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.11.post1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_experimental-0.1.2/PKG-INFO` & `llama_index_experimental-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-experimental
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index experimental package
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Experimental
 
 This is the experimental LlamaIndex extension to core. Experimental features
 and classes can be found in this package. Features that reside in this project
```

