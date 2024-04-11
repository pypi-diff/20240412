# Comparing `tmp/replit_river-0.1.2.tar.gz` & `tmp/replit_river-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.2.tar", max compression
+gzip compressed data, was "replit_river-0.1.3.tar", max compression
```

## Comparing `replit_river-0.1.2.tar` & `replit_river-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.2/LICENSE
--rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.2/README.md
--rw-r--r--   0        0        0     1732 2024-04-11 21:07:11.137264 replit_river-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-11 21:05:27.020432 replit_river-0.1.2/replit_river/__init__.py
--rw-r--r--   0        0        0    18569 2024-04-11 21:02:04.035350 replit_river-0.1.2/replit_river/client.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.2/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.2/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13340 2024-04-11 18:24:00.535474 replit_river-0.1.2/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.2/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.2/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12604 2024-04-11 18:24:00.536045 replit_river-0.1.2/replit_river/codegen/server.py
--rw-r--r--   0        0        0      478 2024-04-11 18:33:34.741591 replit_river-0.1.2/replit_river/error_schema.py
--rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.2/replit_river/py.typed
--rw-r--r--   0        0        0    11973 2024-04-11 18:34:41.139263 replit_river-0.1.2/replit_river/rpc.py
--rw-r--r--   0        0        0     2152 2024-04-11 21:05:41.429562 replit_river-0.1.2/replit_river/seq_manager.py
--rw-r--r--   0        0        0     1340 2024-04-11 21:05:27.021060 replit_river-0.1.2/replit_river/server.py
--rw-r--r--   0        0        0    15581 2024-04-11 21:05:49.017905 replit_river-0.1.2/replit_river/transport.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 replit_river-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.3/README.md
+-rw-r--r--   0        0        0     1732 2024-04-11 23:14:12.690005 replit_river-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-11 21:05:27.020432 replit_river-0.1.3/replit_river/__init__.py
+-rw-r--r--   0        0        0    18569 2024-04-11 21:02:04.035350 replit_river-0.1.3/replit_river/client.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.3/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.3/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13364 2024-04-11 23:13:40.504294 replit_river-0.1.3/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.3/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.3/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12625 2024-04-11 23:14:02.519903 replit_river-0.1.3/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      478 2024-04-11 18:33:34.741591 replit_river-0.1.3/replit_river/error_schema.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.3/replit_river/py.typed
+-rw-r--r--   0        0        0    11973 2024-04-11 18:34:41.139263 replit_river-0.1.3/replit_river/rpc.py
+-rw-r--r--   0        0        0     2152 2024-04-11 21:05:41.429562 replit_river-0.1.3/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     1340 2024-04-11 21:05:27.021060 replit_river-0.1.3/replit_river/server.py
+-rw-r--r--   0        0        0    15581 2024-04-11 21:05:49.017905 replit_river-0.1.3/replit_river/transport.py
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 replit_river-0.1.3/PKG-INFO
```

### Comparing `replit_river-0.1.2/LICENSE` & `replit_river-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/README.md` & `replit_river-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/pyproject.toml` & `replit_river-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.2"
+version="0.1.3"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.2/replit_river/client.py` & `replit_river-0.1.3/replit_river/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/codegen/client.py` & `replit_river-0.1.3/replit_river/codegen/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,17 @@
     chunks: List[str] = [
         "# Code generated by river.codegen. DO NOT EDIT.",
         "from collections.abc import AsyncIterable, AsyncIterator",
         "import datetime",
         "from typing import Any, Dict, List, Literal, Optional, Mapping, Union, Tuple",
         "",
         "from pydantic import BaseModel, Field, parse_obj_as",
-        "from river.error_schema import RiverError",
+        "from replit_river.error_schema import RiverError",
         "",
-        "import river",
+        "import replit_river as replit",
         "",
     ]
     for schema in schemas:
         current_chunks: List[str] = [
             f"class {schema.name.title()}Service:",
             "  def __init__(self, client: river.Client):",
             "    self.client = client",
```

### Comparing `replit_river-0.1.2/replit_river/codegen/run.py` & `replit_river-0.1.3/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/codegen/schema.py` & `replit_river-0.1.3/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/codegen/server.py` & `replit_river-0.1.3/replit_river/codegen/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,17 @@
         "  d: Mapping[str, Any],",
         f") -> {module_name}_pb2.{m.name}:",
         f"  m = {module_name}_pb2.{m.name}()",
         "  if d is None:",
         "    return m",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         chunks.append(
             f"  if d.get('{to_camel_case(field.name)}') is not None:",
         )
@@ -153,17 +153,17 @@
     chunks = [
         f"def _{m.name}Encoder(",
         f"  e: {module_name}_pb2.{m.name}",
         ") -> Dict[str, Any]:",
         "  d: Dict[str, Any] = {}",
     ]
     # Non-oneof fields.
-    oneofs: DefaultDict[
-        int, List[descriptor_pb2.FieldDescriptorProto]
-    ] = collections.defaultdict(list)
+    oneofs: DefaultDict[int, List[descriptor_pb2.FieldDescriptorProto]] = (
+        collections.defaultdict(list)
+    )
     for field in m.field:
         if field.HasField("oneof_index"):
             oneofs[field.oneof_index].append(field)
             continue
         value: str
         if field.type_name == ".google.protobuf.Timestamp":
             value = f"_{field.name}.ToDatetime(tzinfo=datetime.timezone.utc)"
@@ -226,15 +226,15 @@
         "# Code generated by river.codegen. DO NOT EDIT.",
         "import datetime",
         "from typing import Any, Dict, Mapping, Tuple",
         "",
         "from google.protobuf import timestamp_pb2",
         "from google.protobuf.wrappers_pb2 import BoolValue",
         "",
-        "import river",
+        "import replit_river as replit",
         "",
         f"from . import {module_name}_pb2, {module_name}_pb2_grpc\n\n",
     ]
     for pd in fds.file:
 
         def _remove_namespace(name: str) -> str:
             return name.replace(f".{pd.package}.", "")
```

### Comparing `replit_river-0.1.2/replit_river/rpc.py` & `replit_river-0.1.3/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/seq_manager.py` & `replit_river-0.1.3/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/server.py` & `replit_river-0.1.3/replit_river/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/replit_river/transport.py` & `replit_river-0.1.3/replit_river/transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.2/PKG-INFO` & `replit_river-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.2
+Version: 0.1.3
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

