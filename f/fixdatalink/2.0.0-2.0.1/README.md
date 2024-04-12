# Comparing `tmp/fixdatalink-2.0.0.tar.gz` & `tmp/fixdatalink-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixdatalink-2.0.0.tar", last modified: Mon Feb 26 17:38:37 2024, max compression
+gzip compressed data, was "fixdatalink-2.0.1.tar", last modified: Tue Feb 27 10:38:14 2024, max compression
```

## Comparing `fixdatalink-2.0.0.tar` & `fixdatalink-2.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:38:37.796967 fixdatalink-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34464 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42467 2024-02-26 17:38:37.796967 fixdatalink-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:38:37.788967 fixdatalink-2.0.0/fixdatalink/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/analytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:38:37.792967 fixdatalink-2.0.0/fixdatalink/arrow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/arrow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/arrow/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/arrow/type_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/arrow/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/batch_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/collect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/remote_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/show_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/fixdatalink/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:38:37.792967 fixdatalink-2.0.0/fixdatalink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42467 2024-02-26 17:38:37.000000 fixdatalink-2.0.0/fixdatalink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-26 17:38:37.000000 fixdatalink-2.0.0/fixdatalink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 17:38:37.000000 fixdatalink-2.0.0/fixdatalink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-26 17:38:37.000000 fixdatalink-2.0.0/fixdatalink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 17:38:37.000000 fixdatalink-2.0.0/fixdatalink.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-02-26 17:35:14.000000 fixdatalink-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-26 17:38:37.796967 fixdatalink-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:38:14.620992 fixdatalink-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34464 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-02-27 10:38:14.620992 fixdatalink-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:38:14.612992 fixdatalink-2.0.1/fixdatalink/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/analytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:38:14.616992 fixdatalink-2.0.1/fixdatalink/arrow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/arrow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/arrow/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/arrow/type_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/arrow/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/batch_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/collect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/remote_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10898 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/fixdatalink/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:38:14.616992 fixdatalink-2.0.1/fixdatalink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-02-27 10:38:14.000000 fixdatalink-2.0.1/fixdatalink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-27 10:38:14.000000 fixdatalink-2.0.1/fixdatalink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 10:38:14.000000 fixdatalink-2.0.1/fixdatalink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-27 10:38:14.000000 fixdatalink-2.0.1/fixdatalink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-27 10:38:14.000000 fixdatalink-2.0.1/fixdatalink.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-27 10:34:54.000000 fixdatalink-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-27 10:38:14.620992 fixdatalink-2.0.1/setup.cfg
```

### Comparing `fixdatalink-2.0.0/LICENSE` & `fixdatalink-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/PKG-INFO` & `fixdatalink-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixdatalink
-Version: 2.0.0
+Version: 2.0.1
 Summary: Data Pipelines for Fix infrastructure data.
 Author: Some Engineering Inc.
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,15 +679,15 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
-Requires-Dist: fixclient>=2.0.0
+Requires-Dist: fixinventoryclient>=2.0.0
 Requires-Dist: fixinventorylib
 Requires-Dist: rich
 Requires-Dist: sqlalchemy
 Provides-Extra: snowflake
 Requires-Dist: snowflake-sqlalchemy; extra == "snowflake"
 Provides-Extra: mysql
 Requires-Dist: pymysql; extra == "mysql"
```

### Comparing `fixdatalink-2.0.0/fixdatalink/analytics.py` & `fixdatalink-2.0.1/fixdatalink/analytics.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/arrow/config.py` & `fixdatalink-2.0.1/fixdatalink/arrow/config.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/arrow/model.py` & `fixdatalink-2.0.1/fixdatalink/arrow/model.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/arrow/type_converter.py` & `fixdatalink-2.0.1/fixdatalink/arrow/type_converter.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/arrow/writer.py` & `fixdatalink-2.0.1/fixdatalink/arrow/writer.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/batch_stream.py` & `fixdatalink-2.0.1/fixdatalink/batch_stream.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/collect_plugins.py` & `fixdatalink-2.0.1/fixdatalink/collect_plugins.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/remote_graph.py` & `fixdatalink-2.0.1/fixdatalink/remote_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Iterator
 from typing import Optional, ClassVar
 
 from attr import define, field
-from fixclient import FixClient, JsObject
+from fixclient import FixInventoryClient, JsObject
 from fixlib.baseplugin import BaseCollectorPlugin
 from fixlib.baseresources import (
     BaseResource,
     Cloud,
     EdgeType,
     UnknownZone,
     UnknownRegion,
@@ -54,15 +54,15 @@
                 self.core_feedback.error(f"Unhandled exception in Remote Plugin: {ex}", log)
             else:
                 log.error(f"No CoreFeedback available! Unhandled exception in RemoteGraph Plugin: {ex}")
             raise
 
     def _collect_remote_graph(self) -> Graph:
         config: RemoteGraphConfig = Config.remote_graph
-        client = FixClient(config.fix_url, psk=config.psk)
+        client = FixInventoryClient(config.fix_url, psk=config.psk)
         search = config.search or "is(graph_root) -[2:]->"
         return self._collect_from_graph_iterator(client.search_graph(search, graph=config.graph))
 
     def _collect_from_graph_iterator(self, graph_iterator: Iterator[JsObject]) -> Graph:
         assert self.core_feedback, "No CoreFeedback available!"
         graph = Graph()
         lookup: Dict[str, BaseResource] = {}
```

### Comparing `fixdatalink-2.0.0/fixdatalink/schema_utils.py` & `fixdatalink-2.0.1/fixdatalink/schema_utils.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/show_progress.py` & `fixdatalink-2.0.1/fixdatalink/show_progress.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/snowflake.py` & `fixdatalink-2.0.1/fixdatalink/snowflake.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink/sql.py` & `fixdatalink-2.0.1/fixdatalink/sql.py`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink.egg-info/PKG-INFO` & `fixdatalink-2.0.1/fixdatalink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixdatalink
-Version: 2.0.0
+Version: 2.0.1
 Summary: Data Pipelines for Fix infrastructure data.
 Author: Some Engineering Inc.
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -679,15 +679,15 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
-Requires-Dist: fixclient>=2.0.0
+Requires-Dist: fixinventoryclient>=2.0.0
 Requires-Dist: fixinventorylib
 Requires-Dist: rich
 Requires-Dist: sqlalchemy
 Provides-Extra: snowflake
 Requires-Dist: snowflake-sqlalchemy; extra == "snowflake"
 Provides-Extra: mysql
 Requires-Dist: pymysql; extra == "mysql"
```

### Comparing `fixdatalink-2.0.0/fixdatalink.egg-info/SOURCES.txt` & `fixdatalink-2.0.1/fixdatalink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixdatalink-2.0.0/fixdatalink.egg-info/requires.txt` & `fixdatalink-2.0.1/fixdatalink.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 networkx
-fixclient>=2.0.0
+fixinventoryclient>=2.0.0
 fixinventorylib
 rich
 sqlalchemy
 
 [dev]
 pip-tools
 types_python_dateutil
```

### Comparing `fixdatalink-2.0.0/pyproject.toml` & `fixdatalink-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixdatalink"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{name="Some Engineering Inc."}]
 description = "Data Pipelines for Fix infrastructure data."
 license = {file="LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
@@ -25,15 +25,15 @@
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 keywords = ["data source", "data sink", "data synchronization", "data pipeline"]
 
 dependencies = [
     "networkx",
-    "fixclient>=2.0.0",
+    "fixinventoryclient>=2.0.0",
     "fixinventorylib",
     "rich",
     "sqlalchemy",
 ]
 
 [project.optional-dependencies]
```

### Comparing `fixdatalink-2.0.0/requirements-all.txt` & `fixdatalink-2.0.1/requirements-all.txt`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 pytest-cov==4.1.0
 pytest-runner==6.0.1
 python-dateutil==2.8.2
 pytz==2023.3.post1
 pyyaml==6.0.1
 requests==2.31.0
 fixinventory-plugin-example-collector==4.0.0a2
-fixclient==2.0.0
+fixinventoryclient==2.0.0
 fixinventorylib==4.0.0a1
 rich==13.7.0
 rsa==4.9
 s3transfer==0.10.0
 six==1.16.0
 snowflake-connector-python==3.0.4
 snowflake-sqlalchemy==1.5.1
```

### Comparing `fixdatalink-2.0.0/requirements.txt` & `fixdatalink-2.0.1/requirements.txt`

 * *Files 12% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 pyjwt==2.8.0
 pymysql==1.1.0
 pyopenssl==23.2.0
 python-dateutil==2.8.2
 pytz==2023.3.post1
 pyyaml==6.0.1
 requests==2.31.0
-fixclient==2.0.0
+fixinventoryclient==2.0.0
 fixinventorylib==4.0.0a1
 rich==13.7.0
 rsa==4.9
 s3transfer==0.10.0
 six==1.16.0
 snowflake-connector-python==3.0.4
 snowflake-sqlalchemy==1.5.1
```

