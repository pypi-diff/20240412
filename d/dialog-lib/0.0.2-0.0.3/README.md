# Comparing `tmp/dialog_lib-0.0.2.tar.gz` & `tmp/dialog_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog_lib-0.0.2.tar", max compression
+gzip compressed data, was "dialog_lib-0.0.3.tar", max compression
```

## Comparing `dialog_lib-0.0.2.tar` & `dialog_lib-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       98 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/README.md
--rw-r--r--   0        0        0        0 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/agents/__init__.py
--rw-r--r--   0        0        0     3238 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/agents/abstract.py
--rw-r--r--   0        0        0      117 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/db/__init__.py
--rw-r--r--   0        0        0     2642 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/db/memory.py
--rw-r--r--   0        0        0     1325 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/db/models.py
--rw-r--r--   0        0        0      398 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/db/utils.py
--rw-r--r--   0        0        0        0 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/embeddings/__init__.py
--rw-r--r--   0        0        0     1423 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/embeddings/generate.py
--rw-r--r--   0        0        0      148 2024-04-12 00:50:44.658414 dialog_lib-0.0.2/dialog_lib/main.py
--rw-r--r--   0        0        0      634 2024-04-12 00:50:44.662414 dialog_lib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      761 1970-01-01 00:00:00.000000 dialog_lib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       98 2024-04-12 01:02:46.532487 dialog_lib-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 01:02:46.532487 dialog_lib-0.0.3/dialog_lib/agents/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/agents/abstract.py
+-rw-r--r--   0        0        0      117 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/db/__init__.py
+-rw-r--r--   0        0        0     2642 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/db/memory.py
+-rw-r--r--   0        0        0     1325 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/db/models.py
+-rw-r--r--   0        0        0      398 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/db/utils.py
+-rw-r--r--   0        0        0        0 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/embeddings/__init__.py
+-rw-r--r--   0        0        0     1423 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/embeddings/generate.py
+-rw-r--r--   0        0        0      148 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/dialog_lib/main.py
+-rw-r--r--   0        0        0      627 2024-04-12 01:02:46.536488 dialog_lib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 dialog_lib-0.0.3/PKG-INFO
```

### Comparing `dialog_lib-0.0.2/dialog_lib/agents/abstract.py` & `dialog_lib-0.0.3/dialog_lib/agents/abstract.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.2/dialog_lib/db/memory.py` & `dialog_lib-0.0.3/dialog_lib/db/memory.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.2/dialog_lib/db/models.py` & `dialog_lib-0.0.3/dialog_lib/db/models.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.2/dialog_lib/embeddings/generate.py` & `dialog_lib-0.0.3/dialog_lib/embeddings/generate.py`

 * *Files identical despite different names*

### Comparing `dialog_lib-0.0.2/pyproject.toml` & `dialog_lib-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "dialog-lib"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Talkd.AI <foss@talkd.ai>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-langchain = "^0.1.16"
-langchain-openai = "^0.1.3"
+langchain = "0.1.7"
 SQLAlchemy = "^2.0.29"
-langchain-community = "^0.0.32"
 click = "^8.1.7"
 pgvector = "^0.2.5"
+langchain-openai = "^0.0.6"
+psycopg2-binary = "^2.9.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 black = "^24.3.0"
 pytest-mock = "^3.14.0"
 pytest-cov = "^5.0.0"
```

### Comparing `dialog_lib-0.0.2/PKG-INFO` & `dialog_lib-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dialog-lib
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 License: MIT
 Author: Talkd.AI
 Author-email: foss@talkd.ai
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: SQLAlchemy (>=2.0.29,<3.0.0)
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: langchain (>=0.1.16,<0.2.0)
-Requires-Dist: langchain-community (>=0.0.32,<0.0.33)
-Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
+Requires-Dist: langchain (==0.1.7)
+Requires-Dist: langchain-openai (>=0.0.6,<0.0.7)
 Requires-Dist: pgvector (>=0.2.5,<0.3.0)
+Requires-Dist: psycopg2-binary (>=2.9.9,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Dialog Library
 
 Base library for the [dialog-server](https://github.com/talkdai/dialog) project.
```

