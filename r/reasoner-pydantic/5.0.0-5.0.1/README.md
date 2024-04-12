# Comparing `tmp/reasoner-pydantic-5.0.0.tar.gz` & `tmp/reasoner-pydantic-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-5.0.0.tar", last modified: Wed Apr 10 19:01:55 2024, max compression
+gzip compressed data, was "reasoner-pydantic-5.0.1.tar", last modified: Fri Apr 12 19:37:00 2024, max compression
```

## Comparing `reasoner-pydantic-5.0.0.tar` & `reasoner-pydantic-5.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 19:01:55.000000 reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 19:01:55.771062 reasoner-pydantic-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-10 19:01:53.000000 reasoner-pydantic-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.353155 reasoner-pydantic-5.0.1/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:37:00.353155 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 19:37:00.000000 reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:37:00.357155 reasoner-pydantic-5.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-12 19:36:57.000000 reasoner-pydantic-5.0.1/setup.py
```

### Comparing `reasoner-pydantic-5.0.0/PKG-INFO` & `reasoner-pydantic-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.0
+Version: 5.0.1
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.0/README.md` & `reasoner-pydantic-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/__init__.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/base_model.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/message.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Reasoner API models."""
 
 import copy
 import hashlib
 
 from typing import Optional, Callable
 
-from pydantic import constr, Field, parse_obj_as
+from pydantic import constr, Field, parse_obj_as, validator
 
 from .base_model import BaseModel
 from .utils import HashableSequence, HashableSet
 from .results import Result, Results
 from .qgraph import QueryGraph
 from .kgraph import KnowledgeGraph
 from .shared import LogEntry, LogLevel
@@ -204,24 +204,29 @@
 
 
 class Response(BaseModel):
     """Response."""
 
     message: Message = Field(..., title="message", nullable=False)
 
-    logs: Optional[HashableSequence[LogEntry]] = Field(..., nullable=False)
+    logs: Optional[HashableSequence[LogEntry]] = Field([], nullable=False)
 
     status: Optional[str] = Field(None, nullable=True)
 
     workflow: Optional[Workflow]
 
     class Config:
         title = "response"
         extra = "allow"
 
+    @validator("logs")
+    def prevent_none(cls, v):
+        assert v is not None
+        return v
+
     def parse_obj(obj, normalize=True):
         response = parse_obj_as(Response, obj)
         response.message = Message.parse_obj(obj["message"], normalize)
         return response
 
 
 class AsyncQueryResponse(BaseModel):
```

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/metakg.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/results.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/results.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/shared.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/utils.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic/workflow.py` & `reasoner-pydantic-5.0.1/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 5.0.0
+Version: 5.0.1
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Abrar Mesbah
 Author-email: amesbah@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-5.0.0/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-5.0.1/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-5.0.0/setup.py` & `reasoner-pydantic-5.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="5.0.0",
+    version="5.0.1",
     author="Abrar Mesbah",
     author_email="amesbah@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

