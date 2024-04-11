# Comparing `tmp/pysros-23.7.2.tar.gz` & `tmp/pysros-24.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysros-23.7.2.tar", last modified: Fri Sep  1 18:44:11 2023, max compression
+gzip compressed data, was "pysros-24.3.1.tar", last modified: Fri Mar 15 21:34:56 2024, max compression
```

## Comparing `pysros-23.7.2.tar` & `pysros-24.3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 18:44:11.174342 pysros-23.7.2/
--rw-r--r--   0 runner    (1001) docker     (999)    17026 2023-09-01 18:43:57.000000 pysros-23.7.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (999)     4055 2023-09-01 18:44:11.174342 pysros-23.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     3330 2023-09-01 18:43:57.000000 pysros-23.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 18:44:11.170342 pysros-23.7.2/pysros/
--rw-r--r--   0 runner    (1001) docker     (999)      154 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     8806 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)     2858 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3479 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/identifier.py
--rw-r--r--   0 runner    (1001) docker     (999)    58908 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/management.py
--rw-r--r--   0 runner    (1001) docker     (999)    20965 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/model.py
--rw-r--r--   0 runner    (1001) docker     (999)    31735 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (999)      827 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/model_path.py
--rw-r--r--   0 runner    (1001) docker     (999)    21083 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/model_walker.py
--rw-r--r--   0 runner    (1001) docker     (999)    26085 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/pprint.py
--rw-r--r--   0 runner    (1001) docker     (999)    48039 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/request_data.py
--rw-r--r--   0 runner    (1001) docker     (999)     1883 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/singleton.py
--rw-r--r--   0 runner    (1001) docker     (999)     3411 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (999)    12009 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (999)    17361 2023-09-01 18:43:57.000000 pysros-23.7.2/pysros/yang_type.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-01 18:44:11.170342 pysros-23.7.2/pysros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4055 2023-09-01 18:44:11.000000 pysros-23.7.2/pysros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-09-01 18:44:11.000000 pysros-23.7.2/pysros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-01 18:44:11.000000 pysros-23.7.2/pysros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       29 2023-09-01 18:44:11.000000 pysros-23.7.2/pysros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        7 2023-09-01 18:44:11.000000 pysros-23.7.2/pysros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-01 18:44:11.174342 pysros-23.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1074 2023-09-01 18:43:57.000000 pysros-23.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    17026 2024-03-15 21:34:52.000000 pysros-24.3.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-15 21:34:56.686829 pysros-24.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-03-15 21:34:52.000000 pysros-24.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/pysros/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20797 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32703 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/model_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64049 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/request_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41970 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-03-15 21:34:52.000000 pysros-24.3.1/pysros/yang_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 21:34:56.686829 pysros-24.3.1/pysros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-15 21:34:56.000000 pysros-24.3.1/pysros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 21:34:56.686829 pysros-24.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-15 21:34:52.000000 pysros-24.3.1/setup.py
```

### Comparing `pysros-23.7.2/LICENSE.md` & `pysros-24.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysros-23.7.2/PKG-INFO` & `pysros-24.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.7.2
+Version: 24.3.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
-License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
+License: Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ncclient~=0.6.12
+Requires-Dist: lxml~=4.9.2
 
 # Python 3 for Nokia Service Router Operating System (pySROS) #
 
 ## Overview ##
 
 The pySROS libraries provide a model-driven management interface for
 Python developers to integrate with supported Nokia routers
```

### Comparing `pysros-23.7.2/README.md` & `pysros-24.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pysros-23.7.2/pysros/exceptions.py` & `pysros-24.3.1/pysros/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # Copyright 2021-2023 Nokia
 
-__all__ = ("SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError", )
+__all__ = (
+    "SrosMgmtError", "InvalidPathError", "ModelProcessingError",
+    "InternalError", "SrosConfigConflictError",
+    "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError",
+)
 
 __doc__ = """This module contains exceptions for error handling within pySROS.
 
 .. reviewed by PLM 20211201
 .. reviewed by TechComms 20211202
 """
 
@@ -18,78 +22,86 @@
     * invalid objects are passed to the operation e.g. :py:meth:`pysros.management.Datastore.set`
 
     .. Reviewed by PLM 20210625
     .. Reviewed by TechComms 20210630
     """
     pass
 
+
 class InvalidPathError(Exception):
     """Exception raised when a path provided by the user:
 
     * is empty
     * fails to parse
     * does not point to an existing object
     * is missing list keys that must be provided
 
     .. Reviewed by PLM 20210625
     .. Reviewed by TechComms 20210630
     """
     pass
 
+
 class ModelProcessingError(Exception):
     """Exception raised when an error occurs during processing of the YANG model (schema) when:
 
     * a YANG file cannot be found
     * a YANG file is malformed
 
     .. Reviewed by PLM 20210625
     .. Reviewed by TechComms 20210630
     """
     pass
 
+
 class InternalError(Exception):
     """Exception raised for broader issues when:
 
     * schema creation fails and this unfinished schema is utilized
 
     .. Reviewed by PLM 20210625
     .. Reviewed by TechComms 20210630
     """
     pass
 
+
 class SrosConfigConflictError(Exception):
     """Exception raised when a configuration commit failed due to conflicts
     between the ``candidate`` datastore and the ``baseline`` datastore.
     Retrying the configuration operation usually resolves the situation.
     If retrying does not resolve the issue, the connection should be closed using
     :py:meth:`pysros.management.Connection.disconnect` and the operation
     restarted to make a new connection.
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     pass
 
+
 class ActionTerminatedIncompleteError(Exception):
     """Exception raised when an operation (also known as an action)
     completes with a ``terminated-incomplete`` status.
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     pass
 
+
 class JsonDecodeError(Exception):
     """Exception raised when parsing json input fail."""
     pass
 
+
 class XmlDecodeError(Exception):
     """Exception raised when parsing xml input fail."""
     pass
 
+
 def make_exception(arg, **kwarg):
     """Create an exception.
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     return arg[0](arg[1].format(**kwarg))
```

### Comparing `pysros-23.7.2/pysros/identifier.py` & `pysros-24.3.1/pysros/identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # Copyright 2021-2023 Nokia
 
 import re
 
 from .errors import *
+from .errors import make_exception
 from .singleton import _Singleton
 
+
 class LazyBindModule(metaclass=_Singleton):
     def __str__(self):
         return f"{self.__class__.__name__}()"
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return self is other
 
+
 class NoModule(metaclass=_Singleton):
     def __str__(self):
         return f"{self.__class__.__name__}()"
 
     def __hash__(self):
         return id(self)
 
     def __eq__(self, other):
         return self is other
 
+
 class Identifier:
     """Class to hold prefix-name pair for single YANG entry"""
     __slots__ = "_name", "_prefix"
 
     def __init__(self, module, name: str):
         assert ':' not in name
         if isinstance(module, str):
@@ -43,42 +47,45 @@
     @staticmethod
     def builtin(name: str):
         return Identifier(NoModule(), name)
 
     def is_builtin(self):
         return self._prefix is NoModule()
 
-
     def is_lazy_bound(self):
         return self._prefix is LazyBindModule()
 
     @staticmethod
-    def from_yang_string(s:str, default_module, prefix_module_mapping:dict):
+    def from_yang_string(s: str, default_module, prefix_module_mapping: dict):
         if ":" not in s:
             return Identifier(default_module, s)
         if s.count(":") != 1:
             raise make_exception(pysros_err_can_have_one_semicolon)
         prefix, name = s.split(":")
         if prefix not in prefix_module_mapping:
-            raise make_exception(pysros_err_unknown_prefix_for_name, prefix=prefix, name=name)
+            raise make_exception(
+                pysros_err_unknown_prefix_for_name,
+                prefix=prefix,
+                name=name
+            )
         return Identifier(prefix_module_mapping[prefix], name)
 
     @staticmethod
-    def from_model_string(s:str):
+    def from_model_string(s: str):
         if ":" not in s:
             return Identifier.lazy_bound(s)
         if s.count(":") != 1:
             raise make_exception(pysros_err_can_have_one_semicolon)
         return Identifier(*s.split(":"))
 
     def __hash__(self):
         return hash((self.prefix, self.name))
 
     def __str__(self):
-        return  f"""{(str(self.prefix)+":") if self.prefix != NoModule() else ""}{self.name}"""
+        return f"""{(str(self.prefix)+":") if self.prefix != NoModule() else ""}{self.name}"""
 
     def __repr__(self):
         if self.prefix is NoModule():
             return f"""Identifier.builtin({self.name!r})"""
         if self.prefix is LazyBindModule():
             return f"""Identifier.lazy_bound({self.name!r})"""
         return f"""Identifier({self.prefix!r}, {self.name!r})"""
@@ -89,17 +96,18 @@
         elif type(other) == str:
             if ":" in other:
                 return self == Identifier.from_model_string(other)
             return self.name == other
         return False
 
     def __ne__(self, other):
-        return not(self == other)
+        return not (self == other)
 
     _IDENTIFIER_RE = re.compile(r'[a-zA-Z_][a-zA-Z0-9_\-.]*')
+
     def is_valid(self) -> bool:
         def valid_identifier(x):
             return bool(Identifier._IDENTIFIER_RE.fullmatch(x))
         return (valid_identifier(self._name) and
                 (self._prefix is LazyBindModule()
                 or self._prefix is NoModule()
                 or valid_identifier(self._prefix)))
@@ -111,8 +119,7 @@
     @property
     def name(self):
         return self._name
 
     @property
     def model_string(self):
         return f"{self.prefix+':' if self.prefix else ''}{self.name}"
-
```

### Comparing `pysros-23.7.2/pysros/management.py` & `pysros-24.3.1/pysros/management.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,23 +15,27 @@
 from enum import Enum, auto
 from typing import NamedTuple, Tuple
 
 from lxml import etree
 from ncclient import manager
 from ncclient.operations.rpc import RPCError as nc_RPCError
 from ncclient.transport.errors import TransportError as nc_TransportError
-from ncclient.xml_ import new_ele, new_ele_nsmap, to_ele
+from ncclient.xml_ import new_ele_nsmap, to_ele
 
 from .errors import *
+from .errors import (ActionTerminatedIncompleteError, SrosMgmtError,
+                     XmlDecodeError, make_exception)
 from .model import Model
 from .model_builder import ModelBuilder
-from .model_walker import FilteredDataModelWalker, ActionInputFilteredDataModelWalker, ActionOutputFilteredDataModelWalker
-from .request_data import RequestData, COMMON_NAMESPACES
+from .model_walker import (ActionInputFilteredDataModelWalker,
+                           ActionOutputFilteredDataModelWalker,
+                           FilteredDataModelWalker)
+from .request_data import COMMON_NAMESPACES, RequestData
 from .singleton import Empty
-from .wrappers import Container, Leaf, LeafList
+from .wrappers import Container, LeafList, Annotation
 
 __all__ = ("connect", "sros", "Connection", "Datastore", "Empty", "SrosMgmtError", "InvalidPathError", "ModelProcessingError", "InternalError", "SrosConfigConflictError", "ActionTerminatedIncompleteError", "JsonDecodeError", "XmlDecodeError", )
 __doc__ = """This module contains basic primitives for managing an SR OS node.
 It contains functions to obtain and manipulate configuration and state data.
 
 .. reviewed by PLM 20210624
 .. reviewed by TechComms 20210713
@@ -135,18 +139,21 @@
 
     .. reviewed by PLM 20220621
     .. reviewed by TechComms 20220624
     """
     if transport != "netconf":
         raise make_exception(pysros_err_invalid_transport)
     return Connection(host=host, port=port, username=username, password=password,
-                      device_params={'name': 'sros'}, manager_params={'timeout': timeout},
-                      nc_params={'capabilities':['urn:nokia.com:nc:pysros:pc']}, hostkey_verify=hostkey_verify,
+                      device_params={'name': 'sros'},
+                      manager_params={'timeout': timeout},
+                      nc_params={'capabilities': ['urn:nokia.com:nc:pysros:pc']},
+                      hostkey_verify=hostkey_verify,
                       yang_directory=yang_directory, rebuild=rebuild)
 
+
 def sros():
     """Determine whether the execution environment is an SR OS node
 
     :return: True if the application is executed on an SR OS node, False otherwise.
     :rtype: bool
 
     .. code-block:: python
@@ -166,14 +173,15 @@
 
 
     .. reviewed by PLM 20210625
     .. reviewed by TechComms 20210713
     """
     return False
 
+
 class Connection:
     """An object representing a connection to an SR OS device.
     This object is transport agnostic and manages the connection whether the application
     is run on the SR OS node or remotely.
 
     .. warning::
         You **should not** create this class directly. Please use :func:`~pysros.management.connect`
@@ -188,66 +196,78 @@
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
 
     def __init__(self, *args, yang_directory, rebuild, **kwargs):
         try:
-            self._nc        = manager.connect_ssh(*args, **kwargs)
+            self._nc = manager.connect_ssh(*args, **kwargs)
         except Exception as e:
-            raise make_exception(pysros_err_could_not_create_conn, reason=e) from None
-
-        self.running                = Datastore(self, 'running')
-        self.candidate              = Datastore(self, 'candidate')
+            raise make_exception(
+                pysros_err_could_not_create_conn, reason=e
+            ) from None
+
+        self.running = Datastore(self, 'running')
+        self.candidate = Datastore(self, 'candidate')
+
+        self.yang_directory = yang_directory
+        self.rebuild = rebuild
+        self._models = self._get_yang_models()
+        self._ns_map = types.MappingProxyType({model.name: model.namespace for model in self._models})
+        self._ns_map_rev = {v: k for k, v in self._ns_map.items()}
+        self._mod_revs = {model.name: model.revision for model in self._models}
+        self.root, self.metadata = self._get_root(self._models)
+        self._metadata_map = {i.name.model_string: i for i in self.metadata}
+        self._metadata_map_no_module = {}
+        self.debug = False
+        self.intensive_checks = False
 
-        self.yang_directory         = yang_directory
-        self.rebuild                = rebuild
-        self._models                = self._get_yang_models()
-        self._ns_map                = types.MappingProxyType({model.name: model.namespace for model in self._models})
-        self._ns_map_rev            = {v : k for k, v in self._ns_map.items()}
-        self._mod_revs              = {model.name: model.revision for model in self._models}
-        self.root                   = self._get_root(self._models)
-        self.debug                  = False
+        for v in self.metadata:
+            self._metadata_map_no_module.setdefault(v.name.name, []).append(v)
 
     def _get_root(self, modules):
         hasher = hashlib.sha256()
-        yangs = sorted(modules, key = lambda m: m.name)
+        yangs = sorted(modules, key=lambda m: m.name)
         hasher.update(b"Schema ver 5\n")
+        hasher.update(b"Schema features\nBEGIN\n")
+        hasher.update(b"ANNOTATIONS\n")
+        hasher.update(b"END\n")
         for m in yangs:
             hasher.update(f"mod:{m.name};rev:{m.revision};".encode())
-            for sm in sorted(m.submodules, key = lambda sm: sm.name):
+            for sm in sorted(m.submodules, key=lambda sm: sm.name):
                 hasher.update(f" smod:{sm.name};srev:{sm.revision};".encode())
         cache_dir = pathlib.Path.home() / '.pysros' / 'cache'
         cache_name_txt = f"model_{base64.b32encode(hasher.digest()).decode('utf-8')}.ver"
         cache_name = cache_dir / cache_name_txt
 
         if not self.rebuild:
             with contextlib.suppress(FileNotFoundError):
                 with cache_name.open("rb") as f:
-                    return Model(pickle.load(f), 0, None)
+                    storage, metadata = pickle.load(f)
+                    return (Model(storage, 0, None), metadata)
 
         # attempt to pickle. If load fails, we need to create a new tree
         model_builder = ModelBuilder(self._yang_getter, self._ns_map)
         for mod in yangs:
             model_builder.register_yang(mod.name)
         model_builder.process_all_yangs()
 
-        cache_dir.mkdir(mode=0o755, exist_ok=True, parents = True)
+        cache_dir.mkdir(mode=0o755, exist_ok=True, parents=True)
         # write to temp file instead of locking file
         # make hard link to correct name before close + unlink
-        with tempfile.NamedTemporaryFile("wb", dir = cache_dir, prefix = "temp_", delete=False) as f:
+        with tempfile.NamedTemporaryFile("wb", dir=cache_dir, prefix="temp_", delete=False) as f:
             try:
-                pickle.dump(model_builder.root._storage, f)
+                pickle.dump((model_builder.root._storage, model_builder.metadata), f)
             except:
                 with contextlib.suppress(FileNotFoundError):
                     os.unlink(f.name)
                 raise
         os.replace(f.name, cache_name)
 
-        return model_builder.root
+        return (model_builder.root, model_builder.metadata)
 
     def _yang_getter(self, yang_name, *, debug=False):
         if self.yang_directory:
             if debug:
                 print(f"open local file {yang_name}")
             with open(self._find_module(yang_name), "r", encoding="utf8") as f:
                 return f.read()
@@ -263,15 +283,15 @@
             print(f" * {len(data)/1024:.1f} kB downloaded in {(datetime.datetime.now()-start).total_seconds():.3f} sec")
 
         return data
 
     def _find_module(self, yang_name):
         if os.path.isfile(f"""{self.yang_directory}/nokia-combined/{yang_name}.yang"""):
             return f"""{self.yang_directory}/nokia-combined/{yang_name}.yang"""
-        if yang_name in self._ns_map: #module
+        if yang_name in self._ns_map:  # module
             for candidate in pathlib.Path(self.yang_directory).rglob(f"{yang_name}*.yang"):
                 if candidate.parts and re.fullmatch(f"{yang_name}[@]{self._mod_revs[yang_name]}.yang", str(candidate.parts[-1])):
                     return candidate
         for candidate in pathlib.Path(self.yang_directory).rglob(f"{yang_name}*.yang"):
             if candidate.parts and re.fullmatch(f"{yang_name}.yang", str(candidate.parts[-1])):
                 return candidate
         raise make_exception(pysros_err_can_not_find_yang, yang_name=yang_name)
@@ -292,35 +312,45 @@
         )
 
         get_text = lambda e, path: e.findtext(path, namespaces=COMMON_NAMESPACES)
         for m in modules:
             submodules = []
             for sm in m.xpath("./library:submodule", namespaces=COMMON_NAMESPACES):
                 submodules.append(YangSubmodule(
-                    name      = get_text(sm, "./library:name"),
-                    revision  = get_text(sm, "./library:revision"),
+                    name=get_text(sm, "./library:name"),
+                    revision=get_text(sm, "./library:revision"),
                 ))
-            submodules.sort(key = lambda sm: sm.name)
+            submodules.sort(key=lambda sm: sm.name)
             result.append(YangModule(
-                name       = get_text(m, "./library:name"),
-                namespace  = get_text(m, "./library:namespace"),
-                revision   = get_text(m, "./library:revision"),
-                submodules = tuple(submodules)
+                name=get_text(m, "./library:name"),
+                namespace=get_text(m, "./library:namespace"),
+                revision=get_text(m, "./library:revision"),
+                submodules=tuple(submodules)
             ))
         return tuple(result)
 
     def _request_data(self, **kwargs):
-        return RequestData(self.root, self._ns_map, self._ns_map_rev, **kwargs)
+        return RequestData(
+            self.root, self._metadata_map,
+            self._metadata_map_no_module, self._ns_map,
+            self._ns_map_rev, **kwargs
+        )
 
     def _action(self, path, value):
         rd = self._request_data(walker=ActionInputFilteredDataModelWalker)
         current = rd.process_path(path)
+        if self.intensive_checks:
+            rd.sanity_check()
         if not current.is_action():
             raise make_exception(pysros_err_unsupported_action_path)
-        if current._walker.current.name.name == "md-compare" and "path" in value and "subtree-path" in value["path"]:
+        if (
+            current._walker.current.name.name == "md-compare"
+            and "path" in value
+            and "subtree-path" in value["path"]
+        ):
             raise make_exception(pysros_err_action_subtree_not_supported)
         current.set(value)
 
         xml_action = etree.Element(f"""{{{COMMON_NAMESPACES["yang_1_0"]}}}action""")
         xml_action.extend(rd.to_xml())
 
         if self.debug:
@@ -331,74 +361,91 @@
 
         if self.debug:
             print("ACTION response")
             print(response)
 
         del rd
         rd = self._request_data(walker=ActionOutputFilteredDataModelWalker)
-        #data should be wrapped in dummy root. RPC reply can be dummy root if does not have attributes
+        # data should be wrapped in dummy root. RPC reply can be dummy root if does not have attributes
         response.xpath('.')[0].attrib.clear()
         rd.set_action_as_xml(path, response)
+        if self.intensive_checks:
+            rd.sanity_check()
         current = rd.process_path(path, strict=True)
-        return current.to_model()
+        model = current.to_model()
+        if model and model['status'].data == "terminated-incomplete":
+            errors = model['error-message'].data
+            errors = [e.strip() for e in errors]
+            args = errors or ["MINOR: MGMT_AGENT #2007: Operation failed"]
+            raise ActionTerminatedIncompleteError(*args)
+        return model
 
     def _convert(self, path, payload, src_fmt, dst_fmt, pretty_print, action_io):
         def convert_walker(action_io):
             if action_io == "input":
                 return ActionInputFilteredDataModelWalker
             elif action_io == "output":
                 return ActionOutputFilteredDataModelWalker
             raise make_exception(pysros_err_unsupported_action_io)
 
         if not all(fmt in ("xml", "json", "pysros") for fmt in (src_fmt, dst_fmt)):
             raise make_exception(pysros_err_unsupported_convert_method)
-        rd = self._request_data(action=RequestData._Action.convert, walker=convert_walker(action_io))
+        rd = self._request_data(
+            action=RequestData._Action.convert,
+            walker=convert_walker(action_io)
+        )
         current = rd.process_path(path)
 
         if src_fmt == "pysros":
             current.set(payload)
         elif src_fmt == "xml":
             if not isinstance(payload, str):
                 raise make_exception(pysros_err_convert_wrong_payload_type)
             try:
                 data = to_ele(f"<dummy-root>{payload}</dummy-root>")
             except Exception as e:
+                if isinstance(e, etree.XMLSyntaxError) and len(e.args) and re.match('Attribute .* redefined', e.args[0]):
+                    raise make_exception(pysros_err_multiple_occurences_of_xml_attribute)
                 raise XmlDecodeError(*e.args)
             current.set_as_xml(data)
         elif src_fmt == "json":
             if not isinstance(payload, str):
                 raise make_exception(pysros_err_convert_wrong_payload_type)
             current.set_as_json(payload)
         else:
             raise NotImplementedError()
 
+        if self.intensive_checks:
+            rd.sanity_check()
+
         if dst_fmt == "pysros":
             return current.to_model()
         elif dst_fmt == "xml":
             root = current.to_xml()
-            xml_output=""
+            xml_output = ""
             for subtree in root:
                 if pretty_print:
                     etree.indent(subtree, space="    ")
-                    if xml_output:  xml_output += "\n"
+                    if xml_output:
+                        xml_output += "\n"
                 xml_output += etree.tostring(subtree).decode("utf-8")
             return xml_output
         elif dst_fmt == "json":
             return current.to_json(pretty_print)
         else:
             raise NotImplementedError()
 
     @contextlib.contextmanager
     def _process_connected(self):
         try:
-            if  not self._nc.connected:
+            if not self._nc.connected:
                 # test wether connection is not disconected before start of the body
                 raise make_exception(pysros_err_not_connected)
             yield
-        except nc_TransportError as e:
+        except nc_TransportError:
             raise make_exception(pysros_err_not_connected) from None
         except nc_RPCError as e:
             raise SrosMgmtError(e.message.strip() or str(e).strip()) from None
 
     def disconnect(self):
         """Disconnect the current transport session. After disconnect,
         the model-driven interfaces for the SR OS devices are not available.
@@ -441,17 +488,23 @@
            connection_object = connect(host='192.168.1.1', username='myusername', password='mypassword')
            print(connection_object.cli('show version'))
 
         .. Reviewed by PLM 20220901
         """
         with self._process_connected():
             output = self._nc.md_cli_raw_command(command)
-        status = output.xpath("/ncbase:rpc-reply/nokiaoper:status", COMMON_NAMESPACES)
+        status = output.xpath(
+            "/ncbase:rpc-reply/nokiaoper:status",
+            COMMON_NAMESPACES
+        )
         if status and status[0].text == "terminated-incomplete":
-            errors = output.xpath("/ncbase:rpc-reply/nokiaoper:error-message", COMMON_NAMESPACES)
+            errors = output.xpath(
+                "/ncbase:rpc-reply/nokiaoper:error-message",
+                COMMON_NAMESPACES
+            )
             errors = [e.text.strip() for e in errors]
             args = errors or ["MINOR: MGMT_AGENT #2007: Operation failed"]
             raise ActionTerminatedIncompleteError(*args)
         output = output.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-cli-output-block", COMMON_NAMESPACES)
         return output[0].text if output else ""
 
     def action(self, path, value={}):
@@ -602,39 +655,42 @@
                   in the payload in XML or JSON format, it is stripped from the
                   resulting output. Attention should be given to converting the output
                   of the ``compare summary netconf-rpc`` MD-CLI command.
 
         .. Reviewed by PLM 20221123
         .. Reviewed by TechComms 20221124
         """
-        return self._convert(path, payload, source_format, destination_format, pretty_print, action_io)
+        return self._convert(
+            path, payload, source_format,
+            destination_format, pretty_print, action_io
+        )
 
 
 class Datastore:
     """Datastore object that can be used to perform multiple operations on a specified datastore.
 
     .. Reviewed by PLM 20210614
     .. Reviewed by TechComms 20210705
     """
     class _SetAction(Enum):
-        set    = auto()
+        set = auto()
         delete = auto()
 
     class _ExistReason(Enum):
-        exist  = auto()
+        exist = auto()
         delete = auto()
 
     def __init__(self, connection, target):
         if target != 'running' and target != 'candidate':
-            raise make_exception(pysros_invalid_target)
-        self.connection  = connection
-        self.nc          = connection._nc
-        self.target      = target
+            raise make_exception(pysros_err_invalid_target)
+        self.connection = connection
+        self.nc = connection._nc
+        self.target = target
         self.transaction = None
-        self.debug       = False
+        self.debug = False
 
     def _get_defaults(self, defaults):
         return "report-all" if defaults else None
 
     def _check_empty_string(self, model_walker):
         for k in model_walker.keys:
             if '' in k.values():
@@ -681,140 +737,212 @@
             if config_only:
                 response = self._operation_get_config(config, defaults, path)
                 model_walker.config_only = True
             else:
                 response = self._operation_get(config, defaults, path)
         else:
             if model_walker.current.config == False:
-                raise make_exception(pysros_err_can_get_state_from_running_only)
+                raise make_exception(
+                    pysros_err_can_get_state_from_running_only
+                )
             model_walker.config_only = True
             response = self._operation_get_config(config, defaults, path)
 
         if self.debug:
             print("GET response")
             print(response)
         del rd, current
 
         rd = self.connection._request_data()
         rd.set_as_xml(response)
+
+        if self.connection.intensive_checks:
+            rd.sanity_check()
+
         try:
             current = rd.process_path(model_walker, strict=True)
         except LookupError as e:
-            #two possible scenarions - entry does not exists or is empty
-            #if has presence and LookupError is raised, it does not exists
+            # two possible scenarions - entry does not exists or is empty
+            # if has presence and LookupError is raised, it does not exists
             if model_walker.has_explicit_presence() and not filter:
                 raise e from None
             if model_walker.get_dds() == Model.StatementType.list_:
                 res = OrderedDict() if model_walker.current.user_ordered else {}
             else:
                 res = Container._with_model({}, model_walker.current)
 
             model_walker_copy = model_walker.copy()
-            #doing exists to check whether really exists or not
+            # doing exists to check whether really exists or not
             model_walker_copy.go_to_last_with_presence()
             if model_walker_copy.is_root:
                 return res
             else:
                 try:
                     self._get(path, custom_walker=model_walker_copy)
                 except LookupError:
                     raise e from None
                 return res
         return current.to_model(key_filter=(filter or {}))
 
-    def _set(self, path, value, action, method="merge"):
+    def _replace_leaflist(self, path):
+        rd = self.connection._request_data()
+        current = rd.process_path(path)
+        try:
+            leaflist_to_replace = rd.to_xml()
+            old_values = self._operation_get_config(leaflist_to_replace, False, path)
+            del rd
+            rd = self.connection._request_data()
+            rd.set_as_xml(old_values)
+            current = rd.process_path(path, strict=True)
+            current.delete()
+            values_to_delete = rd.to_xml()
+        except:
+            values_to_delete = []
+        return values_to_delete
+
+    def _handle_annotations_only(self, path, rd, annotations_only):
+        requested_cfg_to_strip = rd.to_xml()
+        responded_cfg_to_strip = self._operation_get_config(requested_cfg_to_strip, False, path);
+        del rd
+        rd = self.connection._request_data()
+        rd.set_as_xml(responded_cfg_to_strip)
+        current = rd.process_path(path, strict=True)
+        current.delete_annotations(annotations_only)
+        current.replace()
+        return rd
+
+    def _set(self, path, value, action, method="default", annotations_only=False):
         if self.target == 'running':
             raise make_exception(pysros_err_cannot_modify_config)
-        if method != 'merge' and method != 'replace':
+        if method not in ("default", "merge", "replace"):
             raise make_exception(pysros_err_unsupported_set_method)
-        model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
+        if not isinstance(annotations_only, (bool, list, Annotation)):
+            raise make_exception(pysros_err_annotation_invalid_type)
+        model_walker = FilteredDataModelWalker.user_path_parse(
+            self.connection.root,
+            path
+        )
         if model_walker.current.config == False:
             raise make_exception(pysros_err_cannot_modify_state)
         rd = self.connection._request_data()
+        current = rd.process_path(path)
+        replacing_leaflist = method=="replace" and current._walker.is_leaflist
+        values_to_delete = []
         if action == Datastore._SetAction.delete:
-            default_operation="none"
-            rd.process_path(path).delete()
+            default_operation = "none"
+            if current._walker.is_leaflist:
+                raise make_exception(pysros_err_invalid_operation_on_leaflist)
+            if annotations_only:
+                rd = self._handle_annotations_only(path, rd, annotations_only)
+            else:
+                current.delete()
         else:
-            default_operation="merge"
-            current = rd.process_path(path)
+            default_operation = None
+            if method=="replace" and current._walker.is_leaflist:
+                values_to_delete = self._replace_leaflist(path)
             current.set(value)
             if method == "replace":
                 current.replace()
+            elif method == "merge":
+                current.merge()
+
+        if self.connection.intensive_checks:
+            rd.sanity_check()
+
         children = rd.to_xml()
         config = new_ele_nsmap("config", rd._extra_ns)
-
+        config.extend(values_to_delete)
         config.extend(children)
         if self.debug:
             print("SET request")
             print(f"path: '{path}', value: '{value}'")
             print(etree.dump(config))
-        self.nc.edit_config(target=self.target, default_operation=default_operation, config=config)
+        self.nc.edit_config(
+            target=self.target,
+            default_operation=default_operation,
+            config=config
+        )
 
-    def _delete(self, path):
-        self._set(path, None, Datastore._SetAction.delete)
+    def _delete(self, path, annotations_only):
+        self._set(path, None, Datastore._SetAction.delete, annotations_only=annotations_only)
 
     def _exists(self, path, exist_reason):
         model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
         # if exists is called as a check before deletion, check for path to avoid
         # incorrect errors such as pysros_err_can_check_state_from_running_only
         # as we want to handle state delete related errors first
         if model_walker.current.config == False:
             if exist_reason == Datastore._ExistReason.delete:
                 raise make_exception(pysros_err_cannot_delete_from_state)
             elif self.target == "candidate":
-                raise make_exception(pysros_err_can_check_state_from_running_only)
+                raise make_exception(
+                    pysros_err_can_check_state_from_running_only
+                )
         if exist_reason == Datastore._ExistReason.delete:
             if model_walker.is_local_key:
                 raise make_exception(pysros_err_invalid_operation_on_key)
             if model_walker.is_leaflist:
                 raise make_exception(pysros_err_invalid_operation_on_leaflist)
         if model_walker.has_missing_keys():
-            raise make_exception(pysros_err_invalid_path_operation_missing_keys)
+            raise make_exception(
+                pysros_err_invalid_path_operation_missing_keys
+            )
         model_walker.go_to_last_with_presence()
         if model_walker.is_root:
             return True
         else:
             try:
                 self._get(path, custom_walker=model_walker)
             except LookupError:
                 return False
             return True
 
     def _get_list_keys(self, path, defaults):
-        model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
+        model_walker = FilteredDataModelWalker.user_path_parse(
+            self.connection.root,
+            path
+        )
         self._check_empty_string(model_walker)
 
         rd = self.connection._request_data()
         current = rd.process_path(model_walker)
 
-        #get possible errors related to the getting candidate from state before
-        #errors related to the incorrect path while calling entry_get_keys
+        # get possible errors related to the getting candidate from state before
+        # errors related to the incorrect path while calling entry_get_keys
         if self.target == "candidate" and model_walker.current.config == False:
             raise make_exception(pysros_err_can_get_state_from_running_only)
 
         current.entry_get_keys()
+
+        if self.connection.intensive_checks:
+            rd.sanity_check()
+
         config = rd.to_xml()
 
         if self.target == "running":
             response = self._operation_get(config, defaults, path)
         else:
             response = self._operation_get_config(config, defaults, path)
 
         if self.debug:
             print("GET response")
             print(response)
         del rd, current
 
         rd = self.connection._request_data()
         rd.set_as_xml(response)
+
+        if self.connection.intensive_checks:
+            rd.sanity_check()
+
         try:
             current = rd.process_path(model_walker, strict=True)
         except LookupError as e:
-            #two possible scenarios - list has no entries or path does not exist
-            #doing exists to check whether really exists or not
+            # two possible scenarios - list has no entries or path does not exist
+            # doing exists to check whether really exists or not
             model_walker_copy = model_walker.copy()
             model_walker_copy.go_to_last_with_presence()
             if model_walker_copy.is_root:
                 return []
             else:
                 try:
                     self._get(path, custom_walker=model_walker_copy)
@@ -829,33 +957,40 @@
             raise make_exception(pysros_err_unsupported_compare_datastore)
         if output_format not in ("md-cli", "xml"):
             raise make_exception(pysros_err_unsupported_compare_method)
 
         path = user_path if user_path != "/" else ""
 
         if path:
-            model_walker = FilteredDataModelWalker.user_path_parse(self.connection.root, path)
+            model_walker = FilteredDataModelWalker.user_path_parse(
+                self.connection.root,
+                path
+            )
             if model_walker.current.config == False:
                 raise make_exception(pysros_err_unsupported_compare_endpoint)
             rd = self.connection._request_data()
             current = rd.process_path(model_walker)
+
+            if self.connection.intensive_checks:
+                rd.sanity_check()
+
             if not current.is_compare_supported_endpoint():
                 raise make_exception(pysros_err_unsupported_compare_endpoint)
             path = rd.to_xml()
 
         op_ns = COMMON_NAMESPACES["nokiaoper"]
         xml_action = etree.Element(f"""{{{COMMON_NAMESPACES["yang_1_0"]}}}action""")
         xml_gl_op = etree.SubElement(xml_action, f"{{{op_ns}}}global-operations")
         xml_md_cmp = etree.SubElement(xml_gl_op, f"{{{op_ns}}}md-compare")
         if path:
             xml_path = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}path")
             xml_sbtr_path = etree.SubElement(xml_path, f"{{{op_ns}}}subtree-path")
             xml_sbtr_path.extend(path)
         xml_fmt = etree.Element(f"{{{op_ns}}}format")
-        xml_fmt.text=output_format if output_format == "xml" else "md-cli"
+        xml_fmt.text = output_format if output_format == "xml" else "md-cli"
         xml_md_cmp.append(xml_fmt)
         xml_src = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}source")
         xml_src.append(etree.Element(f"{{{op_ns}}}{self.target}"))
         xml_dst = etree.SubElement(xml_md_cmp, f"{{{op_ns}}}destination")
         xml_dst.append(etree.Element(f"{{{op_ns}}}baseline"))
 
         if self.debug:
@@ -867,18 +1002,18 @@
         if self.debug:
             print("COMPARE reply")
             print(reply)
 
         if output_format == "md-cli":
             return reply.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-compare-output/text()")[0].strip()
 
-        xml_output=""
+        xml_output = ""
         for subtree in reply.xpath("/ncbase:rpc-reply/nokiaoper:results/nokiaoper:md-compare-output/*"):
             subtree.getparent().remove(subtree)
-            xml_output+=etree.tostring(subtree).decode("utf-8")
+            xml_output += etree.tostring(subtree).decode("utf-8")
 
         if xml_output:
             xml_trees = etree.fromstring(f"<root>{xml_output}</root>", parser=etree.XMLParser(remove_blank_text=True))
             for xml_tree in xml_trees:
                 etree.indent(xml_tree, space="    ")
             return "\n".join(etree.tostring(xml_tree, pretty_print=True).decode("utf-8").strip() for xml_tree in xml_trees)
         return ""
@@ -886,15 +1021,17 @@
     def _commit(self):
         try:
             self.nc.commit()
         except nc_RPCError as e:
             if e.message and e.message.find("MGMT_CORE #2703:") > -1:
                 self.nc.discard_changes()
                 self.nc.commit()
-                raise make_exception(pysros_err_commit_conflicts_detected) from None
+                raise make_exception(
+                    pysros_err_commit_conflicts_detected
+                ) from None
             raise e from None
 
     def get(self, path, *, defaults=False, config_only=False, filter=None):
         """Obtain a pySROS data structure containing the contents of the supplied path.  See the
         :ref:`pysros-data-model`
         section for more information about the pySROS data structure.
 
@@ -1004,15 +1141,15 @@
         .. Reviewed by PLM 20220621
         .. Reviewed by TechComms 20220624
 
         """
         with self.connection._process_connected():
             return self._get(path, defaults=defaults, config_only=config_only, filter=filter)
 
-    def set(self, path, value, commit=True, method="merge"):
+    def set(self, path, value, commit=True, method="default"):
         """Set a pySROS data structure to the supplied path. See the
         :ref:`pysros-data-model` section for more information about the pySROS data structure.
 
         :param path: Path to the target node in the datastore.  See the path parameter definition in
                      :py:meth:`pysros.management.Datastore.get` for details.
         :type path: str
 
@@ -1024,15 +1161,15 @@
                       Container or list item, the value should be a `dict` (optionally
                       wrapped in a :class:`pysros.wrappers.Container`).
                       Valid nested data structures are supported.
 
         :param commit: Specify whether update and commit should be executed after set.  Default True.
         :type commit: bool
 
-        :param method: Specify whether set operation should be ``merge`` or ``replace``.  Default ``merge``.
+        :param method: Specify whether set operation should be ``default`` or ``merge`` or ``replace``.  Default ``default``.
         :type method: str
 
         :raises RuntimeError: Error if the connection is lost.
         :raises InvalidPathError: Error if the path is malformed.
         :raises SrosMgmtError: Error for broader SR OS issues, including (non-exhaustive list):
                 passing invalid objects, and setting to an unsupported branch.
         :raises TypeError: Error if fields or keys are incorrect.
@@ -1066,25 +1203,29 @@
         .. Reviewed by PLM 20220901
         """
         with self.connection._process_connected():
             self._set(path, value, Datastore._SetAction.set, method)
             if commit:
                 self._commit()
 
-    def delete(self, path, commit=True):
+    def delete(self, path, commit=True, *, annotations_only=False):
         """Delete a specific path from an SR OS node.
 
         :param path: Path to the node in the datastore.  See the path parameter definition in
                      :py:meth:`pysros.management.Datastore.get` for details.
         :type path: str
         :param commit: Specify whether commit should be executed after delete.  Default True.
         :type commit: bool
+        :param annotations_only: If specified, object where path is pointing is not deleted but 
+                                 only the annotation attached to the object.
+        :type annotations_only: bool
 
         :raises RuntimeError: Error if the connection is lost.
         :raises InvalidPathError: Error if the path is malformed.
+        :raises LookupError: Error if path does not exist.
         :raises SrosMgmtError: Error for broader SR OS issues, including (non-exhaustive list):
                 passing invalid objects, and setting to an unsupported branch.
         :raises TypeError: Error if fields or keys are incorrect.
         :raises InternalError: Error if the schema is corrupted.
         :raises SrosConfigConflictError: Error if configuration commit failed due to conflicts.
 
         .. code-block:: python
@@ -1098,16 +1239,16 @@
         .. Reviewed by PLM 20211201
         .. Reviewed by TechComms 20211202
         """
         with self.connection._process_connected():
             if self.target == 'running':
                 raise make_exception(pysros_err_cannot_modify_config)
             if not self._exists(path, Datastore._ExistReason.delete):
-                raise make_exception(pysros_err_data_missing)
-            self._delete(path)
+                raise make_exception(pysros_err_no_data_found)
+            self._delete(path, annotations_only)
             if commit:
                 self._commit()
 
     def exists(self, path):
         """Check if a specific node exists.
 
         :param path: Path to the node in the datastore. See the path parameter definition in
@@ -1227,15 +1368,14 @@
         .. Reviewed by TechComms 20220624
         """
         with self.connection._process_connected():
             if self.target == 'running':
                 raise make_exception(pysros_err_cannot_modify_config)
             self.nc.discard_changes()
 
-
     def compare(self, path="", *, output_format):
         """Perform a comparison of the uncommitted candidate configuration with the baseline
         configuration.
         The output can be provided in XML or in MD-CLI format and provided in a format
         where, if applied to the node, the resulting configuration would be the same as if the
         candidate configuration is committed.
 
@@ -1286,16 +1426,18 @@
 
     def __setitem__(self, path, value):
         self.set(path, value)
 
     def __delitem__(self, path):
         self.delete(path)
 
+
 class YangSubmodule(NamedTuple):
     name: str
     revision: str
 
+
 class YangModule(NamedTuple):
     name: str
     namespace: str
     revision: str
     submodules: Tuple[YangSubmodule]
```

### Comparing `pysros-23.7.2/pysros/model.py` & `pysros-24.3.1/pysros/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 # Copyright 2021-2023 Nokia
 
 import copy
 import locale
 import sys
-
-from enum import Enum, IntFlag, IntEnum, auto
-from typing import Any, Dict, List, Optional, Tuple
-
-from lxml import etree
+from enum import Enum, IntEnum, IntFlag
+from typing import List, Optional
 
 from .errors import *
-from .identifier import Identifier, NoModule
-from .yang_type import Enumeration, YangType, YangTypeBase
+from .errors import make_exception
+from .identifier import Identifier
 from .yang_type import YangType
 
+
 class AModel:
     class StatementType(Enum):
-        leaf_         = 0
-        list_         = 1
-        container_    = 2
-        leaf_list_    = 3
-        choice_       = 4
-        case_         = 5
-        augment_      = 6
-        uses_         = 7
-        typedef_      = 8
-        module_       = 9
-        submodule_    = 10
-        grouping_     = 11
-        import_       = 12
-        identity_     = 13
-        action_       = 14
-        anydata_      = 15
-        anyxml_       = 16
+        leaf_ = 0
+        list_ = 1
+        container_ = 2
+        leaf_list_ = 3
+        choice_ = 4
+        case_ = 5
+        augment_ = 6
+        uses_ = 7
+        typedef_ = 8
+        module_ = 9
+        submodule_ = 10
+        grouping_ = 11
+        import_ = 12
+        identity_ = 13
+        action_ = 14
+        anydata_ = 15
+        anyxml_ = 16
         notification_ = 17
-        rpc_          = 18
-        input_        = 19
-        output_       = 20
-        deviation_    = 21
-        deviate_      = 22
+        rpc_ = 18
+        input_ = 19
+        output_ = 20
+        deviation_ = 21
+        deviate_ = 22
+        annotate_ = 23
 
     __slots__ = ()
 
     def recursive_walk(self, cb):
         cont = cb(self)
         if cont == False:
             return
         for i in self.children:
             i.recursive_walk(cb)
 
     def __str__(self):
         return f"""Model("{str(self.name)}")"""
 
     def __repr__(self):
-       return f"""Model("{str(self.name)}")"""
+        return f"""Model("{str(self.name)}")"""
 
     def __deepcopy__(self, memo):
         raise make_exception(pysros_err_use_deepcopy)
 
-    def debug_print(self, prefix="", last = False):
+    def debug_print(self, prefix="", last=False):
         class Colors:
-            RED    = '\033[1;31;48m'
-            GREEN  = '\033[1;32;48m'
+            RED = '\033[1;31;48m'
+            GREEN = '\033[1;32;48m'
             DGREEN = '\033[2;32;48m'
-            BLUE   = '\033[1;34;48m'
-            CYAN   = '\033[1;36;48m'
+            BLUE = '\033[1;34;48m'
+            CYAN = '\033[1;36;48m'
             PURPLE = '\033[1;35;48m'
             YELLOW = '\033[1;33;48m'
-            RESET  = '\033[1;37;0m'
+            RESET = '\033[1;37;0m'
 
         utf_supported = locale.getlocale()[1] == "UTF-8"
+
         class AsciiArt:
-            CHILD =         "+-- " if not utf_supported else "\u251c\u2500\u2500 "
-            LAST_CHILD =    "+-- " if not utf_supported else "\u2514\u2500\u2500 "
+            CHILD = "+-- " if not utf_supported else "\u251c\u2500\u2500 "
+            LAST_CHILD = "+-- " if not utf_supported else "\u2514\u2500\u2500 "
             VERTICAL_LINE = "   |" if not utf_supported else "   \u2502"
 
         data_def_stm = self.data_def_stm.name[:-1]
 
         if sys.stdout.isatty():
-            colorize = lambda data, color : color + str(data) + Colors.RESET
+            colorize = lambda data, color: color + str(data) + Colors.RESET
         else:
-            colorize = lambda data, color : str(data)
+            colorize = lambda data, color: str(data)
 
         if not prefix:
             field_prefix = ""
         elif last:
             field_prefix = AsciiArt.LAST_CHILD
         else:
             field_prefix = AsciiArt.CHILD
@@ -142,15 +142,15 @@
             }[self.config]
         if data_def_stm in ("rpc", "action"):
             return "-x"
         if data_def_stm == "notification":
             return "-n"
         return "mp"
 
-    def test_print(self, prefix="", _last = False):
+    def test_print(self, prefix="", _last=False):
         data_def_stm = self.data_def_stm.name[:-1]
         if not prefix:
             field_prefix = ""
         else:
             field_prefix = "+-- "
         t_sufix = [data_def_stm]
         if data_def_stm in ("leaf", "typedef"):
@@ -174,14 +174,15 @@
             new_prefix = prefix + ("    " if not remain else "   |")
             if not prefix:
                 new_prefix = new_prefix[3:]
             res += i.test_print(new_prefix, not remain)
             remain -= 1
         return res
 
+
 class BuildingModel(AModel):
     __slots__ = (
         "name",
         "children",
         "yang_type",
         "units",
         "namespace",
@@ -200,15 +201,15 @@
     )
 
     def __init__(self, name: Identifier, data_def_stm: AModel.StatementType, parent):
         self.name = Identifier.builtin(name) if type(name) == str else name
         self.children: List[Model] = []
         self.yang_type: Optional[YangType] = None
         self.units: Optional[str] = None
-        self.namespace: str = None
+        self.namespace: Optional[str] = None
         self.default: Optional[str] = None
         self.mandatory: Optional[str] = None
         self.status: Optional[str] = None
         self.presence_container = False
         self.user_ordered = False
         self.local_keys: List[str] = []
         self.data_def_stm = data_def_stm
@@ -251,15 +252,18 @@
 
     def delete_from_parent(self, *, quiet=True):
         idx = self.parent.children.index(self)
         if idx < 0:
             if quiet:
                 return
             else:
-                raise make_exception(pysros_err_cannot_remove_node, node=self.name)
+                raise make_exception(
+                    pysros_err_cannot_remove_node,
+                    node=self.name
+                )
         del self.parent.children[idx]
         self.parent = None
 
     def deepcopy(self, parent):
         cls = self.__class__
         result = cls.__new__(cls)
         for i in self.__slots__:
@@ -268,47 +272,51 @@
             setattr(result, i, copy.deepcopy(getattr(self, i)))
         result.parent = parent
         result.children = []
         for child in self.children:
             child.deepcopy(result)
         return result
 
+
 class StorageModel(AModel):
     __slots__ = (
         "_storage",
         "_index",
     )
 
     class DataBitmask(IntFlag):
-        data_def_stm        = 0xff
-        presence_container  = 1 << 8
-        user_ordered        = 1 << 9
-        config              = 1 << 10
-        mandatory           = 1 << 11
-        status              = 1 << 12
+        data_def_stm = 0xff
+        presence_container = 1 << 8
+        user_ordered = 1 << 9
+        config = 1 << 10
+        mandatory = 1 << 11
+        status = 1 << 12
 
     class DataMembers(IntEnum):
-        name            = 0
-        children        = 1
-        yang_type       = 2
-        local_keys      = 3
-        target_path     = 4
-        identity_bases  = 5
-        parent          = 6
-        bitmask         = 7
-        units           = 8
-        namespace       = 9
-        default         = 10
+        name = 0
+        children = 1
+        yang_type = 2
+        local_keys = 3
+        target_path = 4
+        identity_bases = 5
+        parent = 6
+        bitmask = 7
+        units = 8
+        namespace = 9
+        default = 10
+
 
 class Model(StorageModel):
     """Class to represent a single YANG entry and hold additional information, such as type, configuration state, children, and data definition statement.
 
     .. Reviewed by TechComms 20210713
     """
-    __slots__ = ("_data", "children", "parent", "name", "_bitmask", "data_def_stm",)
+    __slots__ = (
+        "_data", "children", "parent", "name", "_bitmask", "data_def_stm",
+    )
 
     def __init__(self, storage, index, parent):
         assert storage
         assert isinstance(storage, list)
         assert 0 <= index < len(storage)
         self._storage = storage
         self._index = index
@@ -331,21 +339,25 @@
     def _name_getter(self):
         name = self._data[Model.DataMembers.name]
         if name[0] is None:
             return Identifier.builtin(name[1])
         return Identifier(*name)
 
     def _children_getter(self):
-        return [Model(self._storage, index, self) for index in self._data[Model.DataMembers.children]]
+        return [
+            Model(self._storage, index, self) for index in self._data[Model.DataMembers.children]
+        ]
 
     def _bitmask_getter(self):
         return self._data[Model.DataMembers.bitmask]
 
     def _data_def_stm_getter(self):
-        return Model.StatementType(int(self._bitmask & Model.DataBitmask.data_def_stm))
+        return Model.StatementType(
+            int(self._bitmask & Model.DataBitmask.data_def_stm)
+        )
 
     @property
     def prefix(self):
         return self._data[Model.DataMembers.name][0]
 
     @property
     def has_children(self):
@@ -389,15 +401,18 @@
 
     @property
     def user_ordered(self):
         return bool(self._bitmask & Model.DataBitmask.user_ordered)
 
     @property
     def is_region_blocked(self):
-        return self.prefix in ("nokia-bof-state", "nokia-li-state", "nokia-debug-state", "nokia-li-conf", "nokia-bof-conf", "nokia-debug-conf")
+        return self.prefix in (
+            "nokia-bof-state", "nokia-li-state", "nokia-debug-state",
+            "nokia-li-conf", "nokia-bof-conf", "nokia-debug-conf"
+        )
 
     @property
     def local_keys(self):
         return self._data[Model.DataMembers.local_keys]
 
     @property
     def target_path(self):
@@ -424,14 +439,15 @@
 
     def __deepcopy__(self, memo):
         raise make_exception(pysros_err_use_deepcopy)
 
     def __eq__(self, other):
         return self._data is other._data
 
+
 class StorageConstructionModel(StorageModel):
     __slots__ = ()
 
     def __init__(self, *args, **kwargs):
         storage, data = new_Model_data(*args, **kwargs)
         self._storage = storage
         self._index = len(storage)
@@ -649,14 +665,15 @@
 
     def __deepcopy__(self, memo):
         raise make_exception(pysros_err_use_deepcopy)
 
     def __eq__(self, other):
         return self._data is other._data
 
+
 def new_Model_data(name: Identifier, data_def_stm: Model.StatementType, parent):
     return (parent._storage if parent is not None else []), [
         [None, name] if type(name) == str else [name.prefix, name.name],        # 0 = name
         [],                                                                     # 1 = children
         None,                                                                   # 2 = yang_type
         [],                                                                     # 3 = local_keys
         None,                                                                   # 4 = target_path
```

### Comparing `pysros-23.7.2/pysros/model_builder.py` & `pysros-24.3.1/pysros/model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,47 @@
 # Copyright 2021-2023 Nokia
 
 import copy
-import xml.parsers.expat
-
 from collections import defaultdict
-from typing import Dict, DefaultDict, List, Set, Union, Optional
+from itertools import chain
+from typing import DefaultDict, Dict, Optional, Set, Union
 
 from .errors import *
-from .identifier import Identifier, NoModule, LazyBindModule
-from .model import AModel, Model, BuildingModel, StorageConstructionModel
+from .errors import InvalidPathError, make_exception
+from .identifier import Identifier, LazyBindModule
+from .model import AModel, BuildingModel, Model, StorageConstructionModel
 from .model_path import ModelPath
-from .model_walker import ModelWalker, DataModelWalker
+from .model_walker import DataModelWalker, ModelWalker
+from .request_data import COMMON_NAMESPACES
 from .tokenizer import yang_parser
-from .yang_type import IdentityRef, LeafRef, PrimitiveType, UnresolvedIdentifier, YangType, YangTypeBase, YangUnion, Enumeration, Bits, should_be_buildin, type_from_name, DECIMAL_LEAF_TYPE, INTEGRAL_TYPES_MIN, INTEGRAL_TYPES_MAX, IP_TYPES
+from .yang_type import (DECIMAL_LEAF_TYPE, INTEGRAL_TYPES_MAX,
+                        INTEGRAL_TYPES_MIN, Bits, Enumeration,
+                        IdentityRef, LeafRef, PrimitiveType,
+                        UnresolvedIdentifier, YangType, YangTypeBase,
+                        YangUnion, should_be_buildin, type_from_name)
+
 
 class YangHandler:
     """Handler for yang processing."""
-    TAGS_WITH_MODEL = ("container", "list", "leaf", "typedef", "module", "submodule", "uses", "leaf-list", "import", "identity", "notification", "rpc", "input", "output", "choice", "case", "deviate", "action")
-    TAGS_FORCE_MODULE = ("grouping", "identity", "typedef", "uses", "augment", "deviation", "type", "base")
+    TAGS_WITH_MODEL = (
+        "container", "list", "leaf", "typedef", "module", "submodule", "uses",
+        "leaf-list", "import", "identity", "notification", "rpc",
+        "input", "output", "choice", "case", "deviate", "action"
+    )
+    TAGS_FORCE_MODULE = (
+        "grouping", "identity", "typedef", "uses", "augment",
+        "deviation", "type", "base"
+    )
     TAGS_ARG_IS_IDENTIFIER = ("base", "type", )
     TAGS_ARG_IS_YANG_PATH_NOT_ABSOLUTE_SCHEMA_ID = ("path", )
-    assert not ({"config", "default", "fraction-digits", "length", "mandatory", "max-elements", "min-elements", "must", "range", "status", "type", "unique", "units", } & set(TAGS_WITH_MODEL)), "Substmt of deviate can not have model"
+    assert not ({
+        "config", "default", "fraction-digits", "length", "mandatory",
+        "max-elements", "min-elements", "must", "range", "status", "type",
+        "unique", "units",
+    } & set(TAGS_WITH_MODEL)), "Substmt of deviate can not have model"
     TAGS_SHOULD_BE_PROCESSED = (
         "action",
         "anydata",
         "anyxml",
         "argument",
         "augment",
         "base",
@@ -36,17 +53,17 @@
         "contact",
         "container",
         "default",
         "description",
         "deviate",
         "deviation",
         "enum",
-#        "error-app-tag",
-#        "error-message",
-#        "extension",
+        # "error-app-tag",
+        # error-message",
+        # extension",
         "feature",
         "fraction-digits",
         "grouping",
         "identity",
         "if-feature",
         "import",
         "include",
@@ -54,14 +71,15 @@
         "key",
         "leaf",
         "leaf-list",
         "length",
         "list",
         "mandatory",
         "max-elements",
+        "md:annotation",
         "min-elements",
         "modifier",
         "module",
         "must",
         "namespace",
         "notification",
         "ordered-by",
@@ -83,27 +101,27 @@
         "submodule",
         "type",
         "typedef",
         "unique",
         "units",
         "uses",
         "value",
-#        "when",
+        # "when",
         "yang-version",
         "yin-element",
     )
 
     def __init__(self, builder: "ModelBuilder", root: BuildingModel):
         self.builder = builder
         self.root = root
         self.path = [root]
         self.full_path = []
         self.grouping_depth = 0
         self.in_type = 0
-        self.derived_identities: Dict[Identifier, Set(Identifier)] = {}
+        self.derived_identities: Dict[Identifier, Set[Identifier]] = {}
         self.include_stack = [{}]
         self.module = None
         self.prefix = None
         self.ignore_depth = 0
 
     def enter(self, name, arg):
         if self.ignore_depth or name not in self.TAGS_SHOULD_BE_PROCESSED:
@@ -132,22 +150,27 @@
             self.path.append(new)
         elif name == "grouping":
             new_id = self.get_identifier(arg, name in self.TAGS_FORCE_MODULE)
             new = BuildingModel(new_id, BuildingModel.StatementType[name.replace("-", "_") + "_"], None)
             self.path.append(new)
             assert new_id not in self.builder.groupings
             self.builder.groupings[new_id] = new
+        elif name == "md:annotation":
+            new_id = self.get_identifier(arg, name in self.TAGS_FORCE_MODULE)
+            new = BuildingModel(new_id, BuildingModel.StatementType.annotate_, None)
+            self.path.append(new)
+            self.builder.metadata.append(new)
         else:
             if name in self.TAGS_ARG_IS_IDENTIFIER:
                 if name == "type" and should_be_buildin(arg):
                     arg = Identifier.builtin(arg)
                 else:
                     arg = self.get_identifier(arg, name in self.TAGS_FORCE_MODULE)
             elif name in self.TAGS_ARG_IS_YANG_PATH_NOT_ABSOLUTE_SCHEMA_ID:
-                arg = self.yang_path_to_model_path(arg, absolute_schema_id = False)
+                arg = self.yang_path_to_model_path(arg, absolute_schema_id=False)
             self.model.blueprint.append((True, (name, arg)))
 
         handle_name = f'handle_early_{name.replace("-", "_DASH_")}'
         if hasattr(self, handle_name):
             handler = getattr(self, handle_name)
             handler(arg)
 
@@ -172,15 +195,15 @@
                     break
             else:
                 self.enter("output", None)
                 self.leave("output")
 
         popped = self.full_path.pop()
         assert popped == name
-        if name in (*self.TAGS_WITH_MODEL, "grouping", "augment", "deviation"):
+        if name in (*self.TAGS_WITH_MODEL, "grouping", "augment", "deviation", "md:annotation"):
             self.path.pop()
         else:
             self.model.blueprint.append((False, name))
 
     def construct(self, model=None):
         model = model or self.root
         self.path.append(model)
@@ -348,21 +371,28 @@
             self.prefixModuleMapping[arg] = self.model.name.name
 
     def handle_config(self, arg: str):
         if arg not in ('false', 'true'):
             raise make_exception(pysros_err_invalid_config)
         self.model.config = (arg == 'true')
 
+
 def _dummy_getter(filename):
     assert False, "Missing getter"
 
+
 class ModelBuilder:
     """API for walking model tree."""
     def __init__(self, yang_getter=_dummy_getter, ns_map={}):
-        self.root = BuildingModel("root", BuildingModel.StatementType["container_"], None)
+        self.root = BuildingModel(
+            "root",
+            BuildingModel.StatementType["container_"],
+            None
+        )
+        self.metadata = []
         self.types_to_resolve = dict()
         self.groupings = dict()
         self.resolved_types = dict()
         self.all_yangs = set()
         self.parsed_yangs = set()
         self.files_to_parse = []
         self.augments = []
@@ -409,156 +439,166 @@
         self.resolve_typedefs()
         self.resolve_type_ranges()
         self.resolve_identities()
         self.resolve_leafrefs()
         self.resolve_config()
         self.resolve_namespaces()
         self.delete_blueprints()
+        self.resolve_metadata_exceptions()
         self.convert_model()
 
     def walk_models(self, cb):
         self.root.recursive_walk(cb)
+        for a in self.metadata:
+            a.recursive_walk(cb)
 
     def perform_parse(self, yang_name, yang_handler=None):
         if yang_name in self.parsed_yangs:
             return
         self.parsed_yangs.add(yang_name)
 
-        yang_parser(self.get_module_content(yang_name), yang_handler or YangHandler(self, self.root))
-
+        yang_parser(
+            self.get_module_content(yang_name),
+            yang_handler or YangHandler(self, self.root)
+        )
 
     def add_child_to_uses(self, m: BuildingModel):
         if m.data_def_stm == BuildingModel.StatementType.uses_:
             assert not m.has_children
             i = m
             while True:
                 if i.data_def_stm == BuildingModel.StatementType.module_:
                     module = i.name.name
                     break
                 elif i.data_def_stm == BuildingModel.StatementType.augment_:
                     module = i.name.prefix
                     break
                 i = i.parent
 
-            def resolve_unresolved(m:BuildingModel):
+            def resolve_unresolved(m: BuildingModel):
                 if m.name.prefix is LazyBindModule():
                     m.prefix = module
 
             for i in self.groupings[m.name].children:
                 i.deepcopy(m)
             m.recursive_walk(resolve_unresolved)
             return False
 
-    def set_correct_types(self, m:BuildingModel):
+    def set_correct_types(self, m: BuildingModel):
         if isinstance(m.yang_type, (UnresolvedIdentifier, YangUnion)):
             tdm = resolve_typedefs_deep(TypeDefModel(m), self.resolved_types)
-            m.yang_type         = tdm.yang_type
-            m.default           = tdm.default
-            m.units             = tdm.units
+            m.yang_type = tdm.yang_type
+            m.default = tdm.default
+            m.units = tdm.units
+        #RFC6020: If the type referenced by the leaf-list has a default value, it has no effect in the leaf-list.
+        if m.data_def_stm == AModel.StatementType.leaf_list_ and m.default:
+            m.default = None
 
     def resolve_typedefs(self):
         for key, value in self.types_to_resolve.items():
-            assert not key in self.resolved_types
+            assert key not in self.resolved_types
             self.resolved_types[key] = resolve_typedefs_deep(value, self.types_to_resolve)
-            if key in IP_TYPES:
-                assert isinstance(self.resolved_types[key].yang_type, YangUnion)
-                self.resolved_types[key].yang_type.deduplicate()
-                assert len(self.resolved_types[key].yang_type) == 1 and self.resolved_types[key].yang_type._types[0].identifier.name == "string"
-                self.resolved_types[key].yang_type = self.resolved_types[key].yang_type._types[0]
         self.walk_models(self.set_correct_types)
 
-    def set_correct_range(self, yt:YangTypeBase):
+    def set_correct_range(self, yt: YangTypeBase):
         assert yt.json_name() != "decimal64" or yt.fraction_digits
         if isinstance(yt, YangUnion):
             for t in yt:
                 self.set_correct_range(t)
 
-        if not yt or not yt.json_name() in (*DECIMAL_LEAF_TYPE, "string", "binary"):    return
-        if yt.json_name() in ("string", "binary") and not yt.length:                    return
+        if not yt or not yt.json_name() in (*DECIMAL_LEAF_TYPE, "string", "binary"):
+            return
+        if yt.json_name() in ("string", "binary") and not yt.length:
+            return
 
         full_range = False if (yt.yang_range or yt.json_name() in ("string", "binary")) else True
         work_range = yt.length if yt.json_name() in ("string", "binary") else yt.yang_range
 
-        if full_range: work_range = "min..max"
+        if full_range:
+            work_range = "min..max"
         if yt.json_name() == "decimal64":
-            min_val = str(-2**63+1)
-            max_val = str(2**63-1)
+            min_val = str(-2**63 + 1)
+            max_val = str(2**63 - 1)
             min_val = min_val[:-yt.fraction_digits] + '.' + min_val[-yt.fraction_digits:]
             max_val = max_val[:-yt.fraction_digits] + '.' + max_val[-yt.fraction_digits:]
         elif yt.json_name() in ("string", "binary"):
             min_val = str(0)
-            max_val = str(2**64-1)
+            max_val = str(2**64 - 1)
         else:
             min_val = INTEGRAL_TYPES_MIN[yt.json_name()]
             max_val = INTEGRAL_TYPES_MAX[yt.json_name()]
 
         work_range = work_range.replace("min", min_val)
         work_range = work_range.replace("max", max_val)
 
         if full_range:
             yt.yang_range = work_range
             return
 
         # merge adjacent subranges, such as "0|1..100" to "0..100" or "0..10|11..20" to "0..20"
-        def process_subrange(subrange:str):
+        def process_subrange(subrange: str):
             nonlocal yt
-            map_f       = float if yt.json_name() == "decimal64" else int
-            i_subrange  = list(map(map_f, subrange.split("..")))
+            map_f = float if yt.json_name() == "decimal64" else int
+            i_subrange = list(map(map_f, subrange.split("..")))
             assert len(i_subrange) in (1, 2)
             return i_subrange if len(i_subrange) == 2 else 2 * i_subrange
 
-        subranges       = work_range.split("|")
-        res_subranges   = [process_subrange(subranges[0])]
+        subranges = work_range.split("|")
+        res_subranges = [process_subrange(subranges[0])]
         for subrange in subranges[1:]:
             i_subrange = process_subrange(subrange)
             if res_subranges[-1][1] == i_subrange[0] - 1:
                 res_subranges[-1][1] = i_subrange[1]
             else:
                 res_subranges.append(i_subrange)
 
-        res_subranges   = [subr if subr[0] != subr[1] else [subr[0]] for subr in res_subranges]
-        work_range      = "|".join(["..".join(map(str, subr)) for subr in res_subranges])
+        res_subranges = [subr if subr[0] != subr[1] else [subr[0]] for subr in res_subranges]
+        work_range = "|".join(
+            "..".join(map(str, subr)) for subr in res_subranges
+        )
         if yt.json_name() in ("string", "binary"):
-            yt.length       = work_range
+            yt.length = work_range
         else:
-            yt.yang_range   = work_range
+            yt.yang_range = work_range
 
     def resolve_type_ranges(self):
-        def setter(m:BuildingModel):
+        def setter(m: BuildingModel):
             if isinstance(m.yang_type, YangTypeBase):
                 self.set_correct_range(m.yang_type)
         self.walk_models(setter)
 
     def resolve_identities(self):
         # first step creates dict, where we find for each identity
         # its all identities, that are directly derived from it.
         directly_derived: DefaultDict[Identifier, Set[Identifier]] = defaultdict(set)
-        def find_derived(m:BuildingModel):
+
+        def find_derived(m: BuildingModel):
             if m.data_def_stm != BuildingModel.StatementType.identity_:
                 return
             for b in m.identity_bases:
                 if m.status != 'obsolete':
                     directly_derived[b].add(m.name)
 
         self.walk_models(find_derived)
         # second step adds all direct and indirect derived identities together
+
         def add_derived_recursive(result_set, id):
             got = directly_derived.get(id, set())
             toUpdate = got - result_set
             result_set.update(got)
             for c in toUpdate:
                 add_derived_recursive(result_set, c)
 
         derived: Dict[Identifier, Set(Identifier)] = {}
         for id in directly_derived.keys():
             derived[id] = set()
             add_derived_recursive(derived[id], id)
 
         # last step iterates through all identityrefs and set possible values
-        def identityref_set_value(m:BuildingModel):
+        def identityref_set_value(m: BuildingModel):
             if m.yang_type is None:
                 return
             if type(m.yang_type) is IdentityRef:
                 m.yang_type.set_values(derived, self._ns_map)
             elif type(m.yang_type) is YangUnion:
                 for st in m.yang_type:
                     if type(st) is IdentityRef:
@@ -568,56 +608,59 @@
 
     def resolve_leafrefs(self):
         def replace_leafrefs(m: BuildingModel):
             if not isinstance(m.yang_type, LeafRef):
                 return
 
             w = DataModelWalker(m)
-            assert m.data_def_stm in (BuildingModel.StatementType.leaf_, BuildingModel.StatementType.leaf_list_)
+            assert m.data_def_stm in (
+                BuildingModel.StatementType.leaf_,
+                BuildingModel.StatementType.leaf_list_
+            )
 
             while isinstance(w.current.yang_type, LeafRef):
                 path = w.current.yang_type.path
                 module_name = w.current.name.prefix
                 if path._path and path._path[0].name != '..':
                     # absolute path - go to root
                     while not w.is_root:
                         w.go_to_parent()
                 w.go_to(path, module_name)
             m.yang_type = w.current.yang_type
         self.walk_models(replace_leafrefs)
 
     def resolve_groupings(self):
-        def inner(m:BuildingModel):
+        def inner(m: BuildingModel):
             if m.data_def_stm == BuildingModel.StatementType.uses_:
                 if m.has_children:
                     return False
                 for child in self.groupings[m.name].children:
                     child.deepcopy(m)
         for grouping in self.groupings.values():
             grouping.recursive_walk(inner)
         self.root.recursive_walk(self.add_child_to_uses)
         for augment in self.augments:
             augment.recursive_walk(self.add_child_to_uses)
 
-    def process_augment(self, m:BuildingModel):
+    def process_augment(self, m: BuildingModel):
         if m.data_def_stm == BuildingModel.StatementType.augment_:
             w = ModelWalker.path_parse(self.root, m.target_path)
             for i in m.children:
                 i.deepcopy(w.current)
 
     def resolve_augments(self):
         current = self.augments
         while current:
             remaining = []
             for augment in current:
                 w = ModelWalker(self.root)
                 try:
                     w.go_to(augment.target_path)
                     node = w.current
-                except InvalidPathError as e:
+                except InvalidPathError:
                     remaining.append(augment)
                     continue
                 for i in augment.children:
                     i.deepcopy(node)
             if len(remaining) >= len(current):
                 raise make_exception(pysros_err_unresolved_augment)
             current = remaining
@@ -654,40 +697,51 @@
                             w.current.blueprint = list(self.filter_blueprint(lambda b: b[0] != instruction[1][0], w.current.blueprint))
                         depth += 1 if instruction[0] else -1
                     w.current.blueprint = list(w.current.blueprint) + deviate.blueprint
                 if deviate.name.name == "not-supported":
                     w.current.delete_from_parent(quiet=False)
 
     def resolve_namespaces(self):
-        def ns_set(m:BuildingModel):
-            if m.namespace or not m.name.prefix in self._ns_map.keys():
+        def ns_set(m: BuildingModel):
+            if m.namespace or m.name.prefix not in self._ns_map.keys():
                 return
             m.namespace = self._ns_map[m.name.prefix]
-        for root_child in self.root.children:
+        for root_child in chain(self.root.children, self.metadata):
             root_child.recursive_walk(ns_set)
 
     def build_blueprints(self):
         handler = YangHandler(self, self.root)
         handler.construct()
+        for a in self.metadata:
+            handler.construct(a)
 
     def delete_blueprints(self):
         def deleter(m: BuildingModel):
             del m.blueprint
         self.walk_models(deleter)
 
     def resolve_config(self):
         def false_setter(m: BuildingModel):
             m.config = False
+
         def resolver(m: BuildingModel):
             if not m.config:
                 m.recursive_walk(false_setter)
                 return False
 
         self.walk_models(resolver)
 
+    def resolve_metadata_exceptions(self):
+        new = BuildingModel(Identifier("ietf-netconf", "operation"), BuildingModel.StatementType.annotate_, None)
+        new.namespace = COMMON_NAMESPACES["ncbase"]
+        type = Enumeration()
+        type.add_enums("merge", "replace", "create", "delete", "remove")
+        new.yang_type = type
+        self.metadata.append(new)
+
     def convert_model(self):
         new_root = StorageConstructionModel("root", BuildingModel.StatementType["container_"], None)
         w = DataModelWalker(self.root)
 
         stack = [new_root]
 
         def enter_fnc(w: DataModelWalker):
@@ -712,96 +766,101 @@
         def leave_fnc(w: DataModelWalker):
             nonlocal stack
             stack.pop()
 
         w.recursive_walk(enter_fnc=enter_fnc, leave_fnc=leave_fnc)
         self.root = Model(new_root._storage, new_root._index, None)
 
+
 class TypeDefModel:
     __slots__ = ("yang_type", "default", "units")
 
     def __init__(self, arg: Union[YangType, Model, BuildingModel], default: Optional[str] = None, units: Optional[str] = None) -> None:
         assert isinstance(arg, (YangTypeBase, AModel))
         if isinstance(arg, AModel):
-            self.yang_type          = arg.yang_type
-            self.default            = arg.default
-            self.units              = arg.units
+            self.yang_type = arg.yang_type
+            self.default = arg.default
+            self.units = arg.units
         else:
-            self.yang_type          = arg
-            self.default            = default
-            self.units              = units
+            self.yang_type = arg
+            self.default = default
+            self.units = units
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__) or self.__slots__ != other.__slots__:
             return False
         return all(getattr(self, name) == getattr(other, name) for name in self.__slots__)
 
-def merge_typedef_ranges(parent_range:str, child_range:str):
+
+def merge_typedef_ranges(parent_range: str, child_range: str):
     """
     Vertically merge typedef integer ranges across typedef parent and child
     - keep child's integer range values (non-'min' or 'max')
     - replace child's 'min'/'max' strings with integer min or max values if present in parent
     - return child's ranges as-is if parent has no range defined or child has no 'max' or 'min'
     examples:
         - parent typedef range "1..200", child type range "min..100", result "1..100"
         - parent typedef range "1..200", child type range "100..max", result "100..200"
         - parent typedef range is None, child type range "100..max", result "100..max"
         - parent typedef range is '1..200', child type range "50..150", result "50..150"
     """
     if not parent_range:
         return child_range
 
-    min_val     = parent_range.split("|")[0].split("..")[0]
+    min_val = parent_range.split("|")[0].split("..")[0]
     child_range = child_range.replace("min", min_val)
-    max_val     = parent_range.split("|")[-1].split("..")[-1]
+    max_val = parent_range.split("|")[-1].split("..")[-1]
     child_range = child_range.replace("max", max_val)
 
     return child_range
 
+
 def resolve_typedefs_shallow(t: TypeDefModel, typedefs: Dict[Identifier, TypeDefModel]):
     assert isinstance(t.yang_type, YangTypeBase)
     yang_type, default, units = t.yang_type, t.default, t.units
-    while type(yang_type) is UnresolvedIdentifier and yang_type.identifier in typedefs:
+    while (type(yang_type) is UnresolvedIdentifier and
+            yang_type.identifier in typedefs):
         r_model = typedefs[yang_type.identifier]
         u_range = yang_type.yang_range
-        frac_d  = yang_type.fraction_digits
-        length  = yang_type.length
+        frac_d = yang_type.fraction_digits
+        length = yang_type.length
         if any((u_range, frac_d, length)):
             yang_type = copy.copy(r_model.yang_type)
             if u_range:
                 yang_type.yang_range = merge_typedef_ranges(yang_type.yang_range, u_range)
             if frac_d:
                 yang_type.fraction_digits = frac_d
             if length:
                 yang_type.length = length
         else:
             yang_type = r_model.yang_type
-        default = default   or r_model.default
-        units   = units     or r_model.units
+        default = default or r_model.default
+        units = units or r_model.units
 
     assert not isinstance(yang_type, UnresolvedIdentifier), f"Cannot resolve type {yang_type}"
     assert isinstance(yang_type, YangTypeBase)
     return TypeDefModel(
         copy.copy(yang_type),
         default,
         units,
     )
 
+
 def resolve_typedefs_deep(m: TypeDefModel, typedefs: Dict[Identifier, TypeDefModel]):
     m = resolve_typedefs_shallow(m, typedefs)
     if not isinstance(m.yang_type, YangUnion):
         return m
 
     u_yang_type, u_default, u_units = YangUnion(), None, None
     for sub in m.yang_type:
         tdm = resolve_typedefs_deep(TypeDefModel(sub), typedefs)
         if type(tdm.yang_type) == YangUnion:
             for t in tdm.yang_type:
                 u_yang_type.append(t)
         else:
             u_yang_type.append(tdm.yang_type)
-        u_default   = tdm.default
-        u_units     = tdm.units
-    m.yang_type         = u_yang_type
-    m.default           = m.default         or u_default
-    m.units             = m.units           or u_units
+        u_default = tdm.default
+        u_units = tdm.units
+    m.yang_type = u_yang_type
+    m.default = m.default or u_default
+    m.units = m.units or u_units
     return m
```

### Comparing `pysros-23.7.2/pysros/model_path.py` & `pysros-24.3.1/pysros/model_path.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2021-2023 Nokia
 
-from typing import Dict, Iterable
+from typing import Iterable
 
 from .identifier import Identifier
 
+
 class ModelPath:
     """Representation of path as a sequence of identifiers.
 
     .. Reviewed by TechComms 20210712
     """
     def __init__(self, parts: Iterable[Identifier]):
         self._path = tuple(parts)
```

### Comparing `pysros-23.7.2/pysros/model_walker.py` & `pysros-24.3.1/pysros/model_walker.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 # Copyright 2021-2023 Nokia
 
 import contextlib
 import copy
 import json
-
 from enum import Enum, auto
-
-from lxml import etree
+from typing import List, Optional, Union
 
 from .errors import *
+from .errors import InvalidPathError, SrosMgmtError, make_exception
 from .identifier import Identifier
 from .model import Model
-from .wrappers import *
+from .wrappers import Container, Leaf, LeafList
 from .yang_type import *
 
+
 class Token:
     def __init__(self):
         self.kind: Optional["ModelWalker._TokenKind"] = None
         self.value = ''
 
+
 class ModelWalker:
     """API representation for walking model tree.
 
     .. Reviewed by TechComms 20210712
     """
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.augment_, Model.StatementType.notification_, Model.StatementType.rpc_, Model.StatementType.input_, Model.StatementType.output_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.action_)
-    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.grouping_, Model.StatementType.augment_)
+    _expected_dds = (
+        Model.StatementType.container_, Model.StatementType.list_,
+        Model.StatementType.leaf_, Model.StatementType.leaf_list_,
+        Model.StatementType.augment_, Model.StatementType.notification_,
+        Model.StatementType.rpc_, Model.StatementType.input_,
+        Model.StatementType.output_, Model.StatementType.choice_,
+        Model.StatementType.case_, Model.StatementType.action_
+    )
+    _recursive_visited_dds = (
+        Model.StatementType.module_, Model.StatementType.submodule_,
+        Model.StatementType.uses_, Model.StatementType.grouping_,
+        Model.StatementType.augment_
+    )
 
-    def __init__(self, model:Model):
-        self.path = []
+    def __init__(self, model: Model):
+        self.path: List[Model] = []
         self.keys = []
         while model.parent is not None:
             if model.data_def_stm in self._expected_dds:
                 self.path.insert(0, model)
                 self.keys.insert(0, dict())
             model = model.parent
         self.model = model
@@ -56,15 +68,15 @@
     def go_to_parent(self):
         if not self.path:
             raise make_exception(pysros_err_cannot_call_go_to_parent)
 
         self.path.pop()
         self.keys.pop()
 
-    def go_to_child(self, child_name:Union[str, Identifier]):
+    def go_to_child(self, child_name: Union[str, Identifier]):
         child = self._get_child(child_name)
         self.path.append(child)
         self.keys.append(dict())
         return child
 
     def go_to(self, path: ModelPath, module: Optional[str] = None):
         for p in path._path:
@@ -84,36 +96,36 @@
 
             try:
                 self.go_to_child(
                     Identifier(prefix, p.name))
             except SrosMgmtError as e:
                 raise InvalidPathError(*e.args) from None
 
-    def check_child_field_value(self, name:Union[str, Identifier], value, *, json=False):
+    def check_child_field_value(self, name: Union[str, Identifier], value, *, json=False, strict=False):
         with self.visit_child(name):
-            return self.check_field_value(value, json=json)
+            return self.check_field_value(value, json=json, strict=strict)
 
-    def check_field_value(self, value, *, json=False):
+    def check_field_value(self, value, *, json=False, strict=False, is_convert=False, metadata=None):
         if self.get_dds() == Model.StatementType.leaf_list_:
             if not isinstance(value, list):
                 raise make_exception(pysros_err_leaflist_should_be_list, type_name=value.__class__.__name__)
-            return all(self.get_type().check_field_value(i, json) for i in value)
+            return all(self.get_type().check_field_value(i, json=json, strict=strict, is_convert=is_convert, metadata=metadata) for i in value)
         elif self.get_dds() == Model.StatementType.leaf_:
-            return self.get_type().check_field_value(value, json)
+            return self.get_type().check_field_value(value, json=json, strict=strict, is_convert=is_convert, metadata=metadata)
         else:
             assert False, "Checking field value for non-field walker"
 
     def get_parent(self):
         res = self.__class__(self.model)
         if self.path:
             res.path = self.path[:-1]
             res.keys = self.keys[:-1]
         return res
 
-    def get_child(self, child_name:Union[str, Identifier]):
+    def get_child(self, child_name: Union[str, Identifier]):
         res = self.copy()
         res.path.append(self._get_child(child_name))
         res.keys.append(dict())
         return res
 
     def copy(self):
         res = self.__class__(self.model)
@@ -122,35 +134,41 @@
         return res
 
     def go_to_last_with_presence(self):
         while self.path and not self.has_explicit_presence():
             self.go_to_parent()
 
     def has_explicit_presence(self):
-        types_with_presence = (Model.StatementType.leaf_, Model.StatementType.leaf_list_)
-        return self.get_dds() in types_with_presence or \
-               self.get_dds() == Model.StatementType.list_ and not self.has_missing_keys() or \
-               self.get_dds() == Model.StatementType.container_ and self.current.presence_container
+        types_with_presence = (
+            Model.StatementType.leaf_, Model.StatementType.leaf_list_
+        )
+        return (
+            self.get_dds() in types_with_presence
+            or self.get_dds() == Model.StatementType.list_ and not self.has_missing_keys()
+            or self.get_dds() == Model.StatementType.container_ and self.current.presence_container)
 
     def has_missing_keys(self):
-        return self.get_dds() == Model.StatementType.list_ and len(self.keys[-1]) != len(self.current.local_keys)
+        return (
+            self.get_dds() == Model.StatementType.list_ and
+            len(self.keys[-1]) != len(self.current.local_keys)
+        )
 
     def dict_keys(self, value):
         for i in value.keys():
             if not isinstance(i, tuple):
                 i = (i,)
             if (len(self.get_local_key_names()) != len(i)):
                 return False
-            if not all(self.check_child_field_value(key_name, key_val) for key_name, key_val in zip(self.get_local_key_names(), i)):
+            if not all(self.check_child_field_value(key_name, key_val, strict=True) for key_name, key_val in zip(self.get_local_key_names(), i)):
                 return False
         return all(isinstance(v, (dict, Container)) for v in value.values())
 
-    def entry_keys(self, value:"DictionaryKeysProxy"):
-        def correct_key(entry:"DictionaryKeysProxy", key):
-            if key in entry and self.check_child_field_value(key, entry[key]):
+    def entry_keys(self, value):
+        def correct_key(entry, key):
+            if key in entry and self.check_child_field_value(key, entry[key], strict=True):
                 return True
             return False
 
         local_keys = [Identifier(self.get_name().prefix, k) for k in self.get_local_key_names()]
         return all(correct_key(value, k) for k in local_keys)
 
     def as_model_type(self, s):
@@ -163,16 +181,16 @@
         if self.get_dds() == Model.StatementType.leaf_:
             res = res[0]
         return res
 
     def dump_json(self):
         def _dump_json(self, parent_data):
             if self.get_dds() in self._expected_dds:
-                data = {"name" : self.get_name().name,
-                        "dds"  : self.get_dds().name}
+                data = {"name": self.get_name().name,
+                        "dds":  self.get_dds().name}
                 if self.get_dds() != Model.StatementType.leaf_:
                     data["children"] = []
                 if self.get_dds() == Model.StatementType.leaf_:
                     data["type"] = self.get_type().json_name()
                 parent_data["children"].append(data)
                 parent_data = data
 
@@ -181,39 +199,37 @@
                 child = children.pop()
                 if child.data_def_stm in (Model.StatementType.module_, Model.StatementType.submodule_):
                     children.extend(child.children)
                     continue
                 if child.data_def_stm in (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.choice_, Model.StatementType.case_, ):
                     with self.visit_child(child.name.name):
                         _dump_json(self, parent_data)
-        root_data = {"children":[]}
+        root_data = {"children": []}
         _dump_json(self, root_data)
         return json.dumps(root_data, indent=4)
 
-
-
     def as_child_model_type(self, child, s):
         with self.visit_child(child):
             return self.as_model_type(s)
 
     @contextlib.contextmanager
-    def visit_child(self, child:Union[str, Identifier]):
+    def visit_child(self, child: Union[str, Identifier]):
         self.go_to_child(child)
         try:
             yield
         finally:
             self.go_to_parent()
 
-    def get_child_type(self, child_name:Union[str, Identifier]):
+    def get_child_type(self, child_name: Union[str, Identifier]):
         return self._get_child(child_name).yang_type
 
-    def get_child_dds(self, child_name:Union[str, Identifier]):
+    def get_child_dds(self, child_name: Union[str, Identifier]):
         return self._get_child(child_name).data_def_stm
 
-    def get_child_name(self, child_name:Union[str, Identifier]):
+    def get_child_name(self, child_name: Union[str, Identifier]):
         return self._get_child(child_name).name
 
     def get_type(self):
         return self.current.yang_type
 
     def get_dds(self):
         return self.current.data_def_stm
@@ -227,25 +243,30 @@
     def has_local_keys_specified(self):
         return len(self.get_local_key_names()) == len(self.local_keys)
 
     def has_local_key_named(self, name):
         return name in self.get_local_key_names()
 
     def has_field_named(self, name):
-        return self.has_child(name) and self.get_child_dds(name) in (Model.StatementType.leaf_, Model.StatementType.leaf_list_)
+        return (
+            self.has_child(name) and
+            self.get_child_dds(name) in (
+                Model.StatementType.leaf_, Model.StatementType.leaf_list_
+            )
+        )
 
     @property
     def is_leaflist(self):
         return self.get_dds() == Model.StatementType.leaf_list_
 
     @property
     def is_local_key(self):
         return self.get_name().name in self.get_parent().get_local_key_names()
 
-    def has_child(self, child_name:Union[str, Identifier] = None):
+    def has_child(self, child_name: Union[str, Identifier] = None):
         if child_name:
             try:
                 self._get_child(child_name)
             except:
                 return False
             else:
                 return True
@@ -272,20 +293,23 @@
             if isinstance(filter, LeafList) and self.get_dds() == Model.StatementType.leaf_list_:
                 filter = filter.data
             if isinstance(filter, dict):
                 if filter:
                     raise make_exception(pysros_err_filter_wrong_leaf_value, leaf_name=self.get_name().name)
             elif isinstance(filter, str):
                 pass
-            elif not self.check_field_value(filter):
-                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self.get_name().name)
+            elif not self.check_field_value(filter, strict=True):
+                raise make_exception(
+                    pysros_err_incorrect_leaf_value,
+                    leaf_name=self.get_name().name
+                )
 
     class _TokenKind(Enum):
-        string  = auto()
-        symbol  = auto()
+        string = auto()
+        symbol = auto()
 
     @classmethod
     def _tokenize(cls, string):
         for i in cls._tokenize_(string):
             yield i
 
     @classmethod
@@ -339,15 +363,17 @@
     def user_path_parse(cls, *args, accept_root=False, **kwargs):
         res = cls.path_parse(*args, **kwargs)
         assert isinstance(res, ModelWalker)
         if not accept_root and res.is_root:
             raise make_exception(pysros_err_root_path)
         for elem in res.path:
             if elem.is_region_blocked:
-                raise make_exception(pysros_err_unknown_element, element=elem.name.name)
+                raise make_exception(
+                    pysros_err_unknown_element, element=elem.name.name
+                )
         return res
 
     @classmethod
     def path_parse(cls, model_root, path_string):
         if not isinstance(path_string, str):
             raise make_exception(pysros_err_path_should_be_string)
 
@@ -358,14 +384,15 @@
             if not path_string:
                 raise make_exception(pysros_err_empty_path)
             raise make_exception(pysros_err_not_found_slash_before_name)
         if path_string.endswith('/'):
             raise make_exception(pysros_err_invalid_identifier)
 
         iterator = iter(cls._tokenize(path_string))
+
         def next_token(*accepts, err,  **kwarg):
             """Verify a next token from path and return tuple(kind, token) if no errors.
                 Otherwise, raise make_exception(err, **kwarg).
 
 :param accepts: Contains a list of the following:
     - one of '/', '[', ']' or '=' - Function accepts specified symbol.
     - 'string' - Function accepts a string, not a symbol.
@@ -382,46 +409,57 @@
                 if n[1] in accepts:
                     return n
             elif 'string' in accepts:
                 return n
             raise make_exception(err, **kwarg)
 
         res = cls(model_root)
-        is_root_element = True
         missing_keys = set()
         elem = 'root'
 
         while True:
-            _, i = next_token('/', '[', None, err = pysros_err_not_found_slash_before_name)
+            _, i = next_token('/', '[', None, err=pysros_err_not_found_slash_before_name)
             if i == None:
-                if missing_keys and len(missing_keys) != len(res.current.local_keys):
+                if (
+                    missing_keys
+                    and len(missing_keys) != len(res.current.local_keys)
+                ):
                     raise make_exception(pysros_err_missing_keys, element=elem)
                 break
             if i == "/":
                 if missing_keys:
                     raise make_exception(pysros_err_missing_keys, element=elem)
-                _, elem = next_token('string', None, err = pysros_err_invalid_identifier)
+                _, elem = next_token('string', None, err=pysros_err_invalid_identifier)
                 try:
                     res.go_to_child(elem)
                     missing_keys.update(res.current.local_keys)
-                    is_root_element = False
-                except Exception as e:
-                    raise make_exception(pysros_err_unknown_element, element=elem) from None
+                except Exception:
+                    raise make_exception(
+                        pysros_err_unknown_element,
+                        element=elem) from None
                 continue
             if i == "[":
-                _, key_name = next_token('string', err = pysros_err_invalid_identifier)
-                next_token('=', err = pysros_err_expected_equal_operator)
-                _, value = next_token('string', err = pysros_err_invalid_identifier)
-                next_token(']', err = pysros_err_expected_end_bracket)
+                _, key_name = next_token(
+                    'string', err=pysros_err_invalid_identifier
+                )
+                next_token('=', err=pysros_err_expected_equal_operator)
+                _, value = next_token(
+                    'string', err=pysros_err_invalid_identifier
+                )
+                next_token(']', err=pysros_err_expected_end_bracket)
                 if key_name not in missing_keys:
                     try:
                         res._get_child(key_name)
-                    except Exception as _:
-                        raise make_exception(pysros_err_unknown_key, key_name = key_name)
-                    raise make_exception(pysros_err_cannot_specify_non_key_leaf)
+                    except Exception:
+                        raise make_exception(
+                            pysros_err_unknown_key, key_name=key_name
+                        )
+                    raise make_exception(
+                        pysros_err_cannot_specify_non_key_leaf
+                    )
                 missing_keys.remove(key_name)
                 res.local_keys[key_name] = value
         return res
 
     @classmethod
     def tokenize_path(cls, path: str, absolute_schema_id: bool):
         # absolute schema id has form: absolute-schema-nodeid = 1*("/" node-identifier)
@@ -429,22 +467,23 @@
         if not path.startswith(('/', '../')):
             raise make_exception(pysros_err_invalid_yang_path, path=path)
 
         _end = None, ''
         t = Token()
 
         iterator = iter(cls._tokenize_(path))
+
         def next_token(t):
             t.kind, t.value = next(iterator, _end)
         next_token(t)
         if t.value == '/':
             # skip '/' in absolute path
             next_token(t)
 
-        while True :
+        while True:
             if t.kind != cls._TokenKind.string:
                 raise make_exception(pysros_err_invalid_yang_path, path=path)
             yield t.value
             next_token(t)
 
             while t.value == '[' and not absolute_schema_id:
                 while t.value not in ('', ']'):
@@ -461,23 +500,27 @@
                 return
 
             raise make_exception(pysros_err_invalid_yang_path, path=path)
 
     def __str__(self):
         return "/" + "/".join(str(name.name) + "".join(f"[{key}={value}]" for key, value in keys.items()) for name, keys in zip(self.path, self.keys))
 
-    def _get_child(self, child_name:Union[str, Identifier]):
+    def _get_child(self, child_name: Union[str, Identifier]):
         children = list(self.current.children)
         while children:
             child = children.pop()
             if child.name == child_name and child.data_def_stm in self._expected_dds and self._is_allowed(child):
                 return child
             if child.data_def_stm in self._recursive_visited_dds:
                 children.extend(child.children)
-        raise make_exception(pysros_err_unknown_child, child_name=child_name, path=self._get_path())
+        raise make_exception(
+            pysros_err_unknown_child,
+            child_name=child_name,
+            path=self._get_path()
+        )
 
     def recursive_walk(self, *, enter_fnc=None, leave_fnc=None):
         children = list(self.current.children)
         while children:
             child = children.pop()
             if child.data_def_stm in self._expected_dds and self._is_allowed(child):
                 self.path.append(child)
@@ -492,35 +535,70 @@
 
     def _get_path(self):
         return " ".join(str(model.name) for model in self.path)
 
     def _is_allowed(self, model):
         return True
 
-    def is_region_blocked_in_child(self, child_name:Union[str, Identifier]):
+    def is_region_blocked_in_child(self, child_name: Union[str, Identifier]):
         return self._get_child(child_name).is_region_blocked
 
+
 class DataModelWalker(ModelWalker):
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_, Model.StatementType.input_, Model.StatementType.output_)
-    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_)
+    _expected_dds = (
+        Model.StatementType.container_, Model.StatementType.list_,
+        Model.StatementType.leaf_, Model.StatementType.leaf_list_,
+        Model.StatementType.action_, Model.StatementType.input_,
+        Model.StatementType.output_
+    )
+    _recursive_visited_dds = (
+        Model.StatementType.module_, Model.StatementType.submodule_,
+        Model.StatementType.uses_, Model.StatementType.augment_,
+        Model.StatementType.choice_, Model.StatementType.case_
+    )
+
 
 class FilteredDataModelWalker(DataModelWalker):
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_)
+    _expected_dds = (
+        Model.StatementType.container_, Model.StatementType.list_,
+        Model.StatementType.leaf_, Model.StatementType.leaf_list_
+    )
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.config_only = False
         self.return_blocked_regions = False
 
     def _is_allowed(self, model):
         if self.config_only and not model.config:
             return False
         if not self.return_blocked_regions and model.is_region_blocked:
             return False
         return any(i in model.name.prefix for i in ("nokia", "openconfig"))
 
+
 class ActionInputFilteredDataModelWalker(FilteredDataModelWalker):
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_)
-    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.input_)
+    _expected_dds = (
+        Model.StatementType.container_, Model.StatementType.list_,
+        Model.StatementType.leaf_, Model.StatementType.leaf_list_,
+        Model.StatementType.action_
+    )
+    _recursive_visited_dds = (
+        Model.StatementType.module_, Model.StatementType.submodule_,
+        Model.StatementType.uses_, Model.StatementType.augment_,
+        Model.StatementType.choice_, Model.StatementType.case_,
+        Model.StatementType.input_
+    )
+
 
 class ActionOutputFilteredDataModelWalker(FilteredDataModelWalker):
-    _expected_dds = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.leaf_, Model.StatementType.leaf_list_, Model.StatementType.action_)
-    _recursive_visited_dds = (Model.StatementType.module_, Model.StatementType.submodule_, Model.StatementType.uses_, Model.StatementType.augment_, Model.StatementType.choice_, Model.StatementType.case_, Model.StatementType.output_)
+    _expected_dds = (
+        Model.StatementType.container_, Model.StatementType.list_,
+        Model.StatementType.leaf_, Model.StatementType.leaf_list_,
+        Model.StatementType.action_
+    )
+    _recursive_visited_dds = (
+        Model.StatementType.module_, Model.StatementType.submodule_,
+        Model.StatementType.uses_, Model.StatementType.augment_,
+        Model.StatementType.choice_, Model.StatementType.case_,
+        Model.StatementType.output_
+    )
```

### Comparing `pysros-23.7.2/pysros/pprint.py` & `pysros-24.3.1/pysros/pprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 # Copyright 2021-2023 Nokia
 
-from .wrappers import *
 from .errors import *
+from .errors import make_exception
+from .wrappers import *
 
-__all__ = ("TreePrinter", "printTree", "Column", "Padding", "Table", "KeyValueTable", )
+__all__ = (
+    "TreePrinter", "printTree", "Column", "Padding", "Table", "KeyValueTable",
+)
 
 __doc__ = """This module contains functions to assist with stylized
 formatting of data.
 
 .. reviewed by PLM 20211201
 .. reviewed by TechComms 20211202
 """
 
+
 def _signalLast(iterable):
     iterable = iter(iterable)
     try:
         ret_var = next(iterable)
         for val in iterable:
             yield False, ret_var
             ret_var = val
         yield True, ret_var
     except StopIteration:
         pass
 
+
 def _groupByTwo(it):
     while True:
         try:
             yield (next(it), next(it))
         except StopIteration:
             break
 
+
 class TreePrinter:
     """Object used to print the result of a call
     to :py:meth:`pysros.management.Datastore.get` as an ASCII tree.
 
     :param align: Whether to align values of a container in the same column.
     :type align: bool
     :param depth: Maximum tree depth to print.
@@ -84,30 +90,31 @@
             print("{...}")
             return
 
         if len(branches) > 0:
             print("")
 
         padding = max([len(key) for key in container.keys()], default=0) if self.align else 0
-        for last,(key,value) in _signalLast(container.items()):
+        for last, (key, value) in _signalLast(container.items()):
             if isinstance(value, list):
-                for list_last,value in _signalLast(value):
+                for list_last, value in _signalLast(value):
                     self._printKeyValue(key, value, last and list_last, branches, padding)
             else:
                 self._printKeyValue(key, value, last, branches, padding)
 
     def _printKeyValue(self, key, value, last, branches, padding):
         for branch in branches:
             print(branch, end='')
         print("`-- " if last else "+-- ", end='')
         print("{:<{padding}}: ".format(str(key), padding=padding), end='')
         branches.append("    " if last else "|   ")
         self._printItem(value, branches)
         branches.pop()
 
+
 def printTree(obj, **kwargs):
     """Print the result of a call to :py:meth:`pysros.management.Datastore.get`
     as an ASCII tree.
 
     See arguments of :class:`.TreePrinter`
 
     .. code-block:: python
@@ -128,14 +135,15 @@
            main()
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     TreePrinter(**kwargs).print(obj)
 
+
 class Column:
     """Column descriptor to be used in :class:`pysros.pprint.Table`
     and :class:`pysros.pprint.KeyValueTable`.
 
     :param width: Width of the column (number of characters).
     :type width: int
     :param name: Name of the column. This may be None when column
@@ -151,20 +159,20 @@
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     def __init__(self, width, name=None, align='<', padding=0):
         if align != '<' and align != '>' and align != '^':
             raise make_exception(pysros_err_invalid_align, align=align)
-        self.name     = name
-        self.width    = width
-        self.align    = align
-        self.padding  = padding
-        self._padstr  = " " * padding
-        self._format  = self._make_format()
+        self.name = name
+        self.width = width
+        self.align = align
+        self.padding = padding
+        self._padstr = " " * padding
+        self._format = self._make_format()
 
     def _make_format(self):
         return "{{}}{{:{}{}s}}".format(self.align, self.width - self.padding)
 
     def format(self, value):
         """Format a value according to the parameters of this column,
         considering width, alignment, and padding.
@@ -195,42 +203,44 @@
         if isinstance(arg, Column):
             return arg
         elif isinstance(arg, tuple):
             return Column(*arg)
         else:
             raise make_exception(pysros_err_invalid_col_description)
 
+
 class Padding(Column):
     """Special type of column which takes no data.  It is only used to add empty space into a table.
 
     :param width: Width of the (empty) column.
     :type width: int
 
     .. Reviewed by PLM 20210628
     .. Reviewed by TechComms 20210705
 
     """
     def __init__(self, width):
         super().__init__(width, padding=width)
 
+
 class ATable:
     """Abstract parent class for Table and KeyValueTable containing the common functionality.
 
     .. Reviewed by PLM 20210628
     .. Reviewed by TechComms 20210712
     """
     def __init__(self, title, width=79):
-        self._title      = title
-        self._width      = width
-        self._double     = "=" * self._width
-        self._single     = "-" * self._width
+        self._title = title
+        self._width = width
+        self._double = "=" * self._width
+        self._single = "-" * self._width
         self.reset()
 
     def reset(self):
-        self._numRows   = 0
+        self._numRows = 0
         self._truncated = False
 
     def printDoubleLine(self):
         """Print a double line."""
         print(self._double)
 
     def printSingleLine(self):
@@ -263,17 +273,18 @@
         if self._truncated:
             print("* indicates that the corresponding row element may have been truncated.")
 
     def _prepareValue(self, value, col):
         s = str(value)
         if col.padding + len(s) > col.width:
             self._truncated = True
-            s = s[:col.width-col.padding-1]+"*"
+            s = s[:col.width - col.padding - 1] + "*"
         return col.format(s)
 
+
 class Table(ATable):
     """Class that provides the functionality to display tabulated data in the standard SR OS style.
 
     :param title: Title of the table.
     :type title: str
     :param columns: List of column descriptions. Elements of the list can
                     be a :py:class:`pysros.pprint.Column` or a tuple with
@@ -310,18 +321,17 @@
            table, rows = simple_table_builder_example()
 
     .. Reviewed by PLM 20211201
     .. Reviewed by TechComms 20211202
     """
     def __init__(self, title, columns, width=79, showCount=None, summary=None):
         super().__init__(title, width=width)
-        self._columns   = list(map(Column.create, columns))
+        self._columns = list(map(Column.create, columns))
         self._showCount = showCount
-        self._summary   = summary
-
+        self._summary = summary
 
     def print(self, rows):
         """
         Display a complete table when passed in the rows of data.
         Separate components are displayed as configured during initialization.
 
         :param rows: List of tuples containing the data to be displayed. Each tuple in the list is a row
@@ -409,15 +419,15 @@
            row0col0                       row0col1
 
         .. Reviewed by PLM 20210629
         .. Reviewed by TechComms 20210712
         """
         width = self._width
         row_iter = iter(row)
-        for last,col in _signalLast(self._columns):
+        for last, col in _signalLast(self._columns):
             # In case there is no data, or if the column is padding,
             # use the empty string as data
             data = ""
             try:
                 if not isinstance(col, Padding):
                     data = next(row_iter)
             except StopIteration:
@@ -496,14 +506,15 @@
         if showLine:
             self.printSingleLine()
         if self._showCount:
             print("No. of {}: {}".format(self._showCount, self._numRows))
         if customSummary is not None:
             print(customSummary)
 
+
 class KeyValueTable(ATable):
     """Display a list of key and value data in an SR OS table format.
 
     :param title: Title of the table.
     :type title: str
     :param columns: List of column descriptions. Elements of the list can be :py:class:`pysros.pprint.Column` or
                     a tuple with parameters to be passed to :py:meth:`pysros.pprint.Column.create`.
@@ -541,34 +552,40 @@
             raise make_exception(pysros_err_even_num_of_columns_required)
 
     def _printIter(self, item_iter):
         col_iter = iter(_signalLast(self._columns))
         last_col = False
         last_data = True
         while not last_col:
-            last_col,key_col = next(col_iter)
+            last_col, key_col = next(col_iter)
 
             # print padding-columns
             if isinstance(key_col, Padding):
-                print(self._prepareValue("", key_col), end=('' if last_col else ' '))
+                print(
+                    self._prepareValue("", key_col),
+                    end=('' if last_col else ' ')
+                )
                 continue
 
             # In case there is no data, stop printing
             try:
-                last_data,(key,value) = next(item_iter)
+                last_data, (key, value) = next(item_iter)
             except StopIteration:
                 break
 
             # also fetch the value-column
             last_col, value_col = next(col_iter)
 
             # format both key and value
             print(self._prepareValue(key, key_col), end='')
             print(": ", end='')
-            print(self._prepareValue(value, value_col), end=('' if last_col else ' '))
+            print(
+                self._prepareValue(value, value_col),
+                end=('' if last_col else ' ')
+            )
 
         print()
         return not last_data
 
     def printKV(self, *kvs):
         """Print a table of key-value pairs that are passed into this method.
         This method does not require the data to be structured as a list of 2-tuples.
@@ -681,8 +698,7 @@
            ...
            >>> table_printColumnHeaders_example(table)
            Column0                        Column1
         """
         if any(col.name for col in self._columns):
             self.printKV(*[col.name for col in self._columns])
             self.printSingleLine()
-
```

### Comparing `pysros-23.7.2/pysros/request_data.py` & `pysros-24.3.1/pysros/request_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 # Copyright 2021-2023 Nokia
 
 import copy
-import pprint
 import json
-
+import pprint
+import itertools
 from abc import ABC, abstractmethod
 from collections import OrderedDict
-from contextlib import ExitStack
 from enum import Enum, auto
+from typing import Dict, Union
+
 from lxml import etree
 from ncclient.xml_ import to_ele
-from typing import Union, List, Dict
 
 from .errors import *
-from .identifier import NoModule, Identifier
+from .errors import JsonDecodeError, SrosMgmtError, make_exception
+from .identifier import Identifier, NoModule
 from .model import Model
 from .model_walker import FilteredDataModelWalker, ModelWalker
-from .singleton import _Singleton, Empty
-from .wrappers import Wrapper, Action, Container, Leaf, LeafList
-from .yang_type import IdentityRef
+from .singleton import Empty, _Singleton
+from .wrappers import (Action, Annotation, Annotations, Container, Leaf,
+                       LeafList, Wrapper)
+from .yang_type import IdentityRef, YangUnion, INTEGRAL_LEAF_TYPE
 
 COMMON_NAMESPACES = {
-    "ncbase": "urn:ietf:params:xml:ns:netconf:base:1.0",
+    "ncbase":     "urn:ietf:params:xml:ns:netconf:base:1.0",
     "monitoring": "urn:ietf:params:xml:ns:yang:ietf-netconf-monitoring",
-    "library": "urn:ietf:params:xml:ns:yang:ietf-yang-library",
-    "nokiaoper": "urn:nokia.com:sros:ns:yang:sr:oper-global",
-    "yang_1_0" : "urn:ietf:params:xml:ns:yang:1",
-    "attrs"    : "urn:nokia.com:sros:ns:yang:sr:attributes",
+    "library":    "urn:ietf:params:xml:ns:yang:ietf-yang-library",
+    "nokiaoper":  "urn:nokia.com:sros:ns:yang:sr:oper-global",
+    "yang_1_0":   "urn:ietf:params:xml:ns:yang:1",
+    "attrs":      "urn:nokia.com:sros:ns:yang:sr:attributes",
 }
 
-MO_STATEMENT_TYPES = (Model.StatementType.container_, Model.StatementType.list_, Model.StatementType.action_)
-FIELD_STATEMENT_TYPES = (Model.StatementType.leaf_, Model.StatementType.leaf_list_)
+MO_STATEMENT_TYPES = (
+    Model.StatementType.container_,
+    Model.StatementType.list_,
+    Model.StatementType.action_
+)
+FIELD_STATEMENT_TYPES = (
+    Model.StatementType.leaf_,
+    Model.StatementType.leaf_list_
+)
 
 _get_tag_name = lambda x: etree.QName(x).localname
 _get_tag_ns = lambda x: etree.QName(x).namespace
 _text_in_tag_tail = lambda x: x.tail and x.tail.strip()
 _text_in_tag_text = lambda x: x.text and x.text.strip()
-_create_root_ele = lambda : etree.Element("dummy-root", nsmap={"nokia-attr": COMMON_NAMESPACES["attrs"]})
+_create_root_ele = lambda: etree.Element("dummy-root", nsmap={"nokia-attr": COMMON_NAMESPACES["attrs"]})
+_metadata_from_xml = lambda e, rev_ns_map: {f"""{rev_ns_map.get(_get_tag_ns(k), "")}:{_get_tag_name(k)}""": v for k, v in e.attrib.items()} if e.attrib else {}
 
 def subelement(parent, tag, nsmap, text=None, attrib=None, add_ns=None):
     """Wrapper around etree.Subelement, that raises SrosMgmtError instead of ValueError."""
     local_nsmap = {}
     if add_ns:
         local_nsmap[add_ns] = nsmap[add_ns]
     try:
         if tag.is_builtin():
-            result = etree.SubElement(parent, tag.name, attrib, nsmap=local_nsmap)
+            result = etree.SubElement(
+                parent, tag.name, attrib, nsmap=local_nsmap
+            )
         else:
             module = tag.prefix
             uri = nsmap[module]
             local_nsmap[module] = uri
             result = etree.SubElement(
                 parent,
                 etree.QName(uri, tag.name),
@@ -59,49 +71,58 @@
 
         if text is not None:
             result.text = text
         return result
     except ValueError as err:
         raise SrosMgmtError(err.args) from None
 
+
 def _raise_invalid_text_exception(tag, check_parent_tag=True):
     tag_to_check = tag.getparent() if check_parent_tag else tag
     if tag_to_check.tag == "dummy-root":
         raise make_exception(pysros_err_invalid_xml_root)
     else:
-        raise make_exception(pysros_err_invalid_xml_element, element=_get_tag_name(tag_to_check))
+        raise make_exception(
+            pysros_err_invalid_xml_element,
+            element=_get_tag_name(tag_to_check)
+        )
+
+
+def _raise_unknown_attribute(name):
+    if isinstance(name, Annotation):
+        module = getattr(name, 'module', None)
+        name = module + ':' + name.key if module else name.key
+    raise make_exception(
+        pysros_err_unknown_attribute,
+        name=name
+    )
 
-def _leaf_to_xml(value, root, walker, ns_map, replace_field=False):
-    if walker.get_dds() == Model.StatementType.leaf_:
-        value = (value, )
-    for i in value:
-        txt, add_ns = walker.get_type().to_string(i)
-        subelement(root, walker.current.name, ns_map, txt, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""":"replace"} if replace_field else {}, add_ns)
-        replace_field=False
 
 class RequestData:
     """Basic API for holding and handling data.
 
     .. Reviewed by TechComms 20210712
     """
 
     class _Action(Enum):
-        basic   = auto()
+        basic = auto()
         convert = auto()
 
-    def __init__(self, root:Model, ns_map:dict, ns_map_rev:dict, *, action:_Action=_Action.basic, walker=FilteredDataModelWalker):
-        self._root             = root
-        self._data             = _ListStorage(root, self)
-        self._ns_map           = ns_map
-        self._ns_map_rev       = ns_map_rev
-        self._action           = action
-        self._Walker           = walker
-        self._extra_ns         = {}
+    def __init__(self, root: Model, annotations: Dict[str, Model], annotations_no_module: Dict[str, Model], ns_map: dict, ns_map_rev: dict, *, action: _Action = _Action.basic, walker=FilteredDataModelWalker):
+        self._root = root
+        self._Walker = walker
+        self._data = _ListStorage(root, self)
+        self._ns_map = ns_map
+        self._ns_map_rev = ns_map_rev
+        self._action = action
+        self._extra_ns: Dict[str, str] = {}
+        self._modeled_metadata = annotations
+        self._modeled_metadata_no_module = annotations_no_module
 
-    def process_path(self, path:Union[str, FilteredDataModelWalker], *, strict=False):
+    def process_path(self, path: Union[str, FilteredDataModelWalker], *, strict=False):
         """Create all entries in given path and return setter for last section of the path.
 
         .. Reviewed by TechComms 20210712
         """
         walker = path if isinstance(path, ModelWalker) else self._Walker.user_path_parse(self._root, path, accept_root=(self._action == self._Action.convert))
         current = _ASetter.create_setter(self._data, self)
         for elem, keys in zip(walker.path, walker.keys):
@@ -177,30 +198,41 @@
     def debug_dump(self):
         """Dump rquest data in raw form.
 
         .. Reviewed by TechComms 20210712
         """
         self._data.debug_dump()
 
+    def sanity_check(self):
+        self._data.sanity_check()
+
     def _unwrap(self, value):
         return value.data if isinstance(value, Wrapper) else value
 
-
     def _add_xml_namespace(self, identity):
         assert self._ns_map[identity.module] == identity.namespace
         self._extra_ns[identity.module] = identity.namespace
 
 
 class _AStorage(ABC):
     """Abstract representation of data storage.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, rd:RequestData):
+    def __init__(self, rd: RequestData):
         self.rd = rd
+        self._metadata = None
+
+    @property
+    def metadata(self):
+        return self._metadata
+
+    @metadata.setter
+    def metadata(self, val):
+        self._metadata = copy.copy(val)
 
     def to_xml(self, ns_map, root):
         """Return data in xml format.
 
         .. Reviewed by TechComms 20210712
         """
         return self._to_xml(ns_map, root)
@@ -228,147 +260,235 @@
         if model.name.prefix in ns_map:
             return etree.QName(ns_map[model.name.prefix], model.name.name)
         elif model.name.prefix is NoModule():
             return model.name.name
         else:
             raise make_exception(pysros_err_prefix_does_not_have_ns, prefix=model.name.prefix, name=model.name.name)
 
+    def _metadata_to_model(self, metadata):
+        is_leaflist = self._walker.is_leaflist
+        if not metadata or not any(metadata):
+            return None
+        metadata = metadata if is_leaflist else [metadata]
+        res = []
+        for m in metadata:
+            res.append(Annotations())
+            for k, v in m.items():
+                model = self.rd._modeled_metadata[k]
+                res[-1].append(Annotation._with_model(key=model.name.name, data=v, module=model.name.prefix, namespace=model.namespace, model=model))
+        return res if is_leaflist else res[0]
+
+    def _metadata_to_xml(self, metadata):
+        if not metadata or not any(metadata):
+            return None
+        res = {}
+        for k, v in metadata.items():
+            model = self.rd._modeled_metadata[k]
+            res[etree.QName(model.namespace, model.name.name).text], _ = model.yang_type.to_string(v)
+        return res
+
+    def _leaf_to_xml(self, value, root, walker, ns_map, operation, metadata=None):
+        if walker.get_dds() == Model.StatementType.leaf_:
+            value = (value, )
+            metadata = (metadata, )
+        elif not metadata:
+            metadata = [None] * len(value)
+        for i, m in zip(value, metadata):
+            txt, add_ns = walker.get_type().to_string(i)
+            attrib = {}
+            if m and (not isinstance(m, list) or any(m)):
+                attrib.update(self._metadata_to_xml(m))
+            if operation:
+                attrib[f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation"""] = operation
+            subelement(root, walker.current.name, ns_map, txt, attrib, add_ns)
+            replace_field = False
+
+
 class _FieldStorage(_AStorage):
     """Data storage for leaves.
     """
 
-    def __init__(self, model:Model, rd:RequestData):
+    def __init__(self, model: Model, rd: RequestData, *, value = None):
         super().__init__(rd)
         self._model = model
-        self._value = None
+        self._value = value
         self._operation = ""
 
     def _to_xml(self, ns_map, root):
-        if self._operation == "delete":
-            subelement(root, self._walker.current.name, ns_map, None, {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": "remove"})
-        elif self._value is FieldValuePlaceholder():
+        if self._value is FieldValuePlaceholder():
             pass
         elif self._value is GetValuePlaceholder():
-            subelement(root, self._walker.current.name, ns_map)
+            if self._operation:
+                subelement(root, self._walker.current.name, ns_map, attrib={f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation})
+            else:
+                subelement(root, self._walker.current.name, ns_map)
         else:
-            _leaf_to_xml(self._value, root, self._walker, ns_map, self._operation=="replace")
+            self._leaf_to_xml(
+                self._value, root, self._walker, ns_map,
+                self._operation, metadata=self.metadata
+            )
 
     def to_model(self, *, key_filter={}):
         assert self.rd._action == RequestData._Action.convert or self._value is not GetValuePlaceholder()
         assert self._value is not FieldValuePlaceholder()
         if self._walker.get_dds() == Model.StatementType.leaf_:
-            return Leaf._with_model(self._value, self._model)
-        return LeafList._with_model(self._value, self._model)
+            return Leaf._with_model(self._value, self._model, annotations=self._metadata_to_model(self.metadata))
+        return LeafList._with_model(self._value, self._model, annotations=self._metadata_to_model(self.metadata))
+
+    def _debug_dump_single_metadata(self, metadata):
+        return f'<{", ".join(f"{k}:{v}" for k, v in metadata.items())}>'
+
+    def _debug_dump_metadata(self):
+        if not self.metadata:
+            return ""
+        if isinstance(self.metadata, list):
+            return "[" + ", ".join(map(self._debug_dump_single_metadata, self.metadata)) + "]"
+        return self._debug_dump_single_metadata(self.metadata)
 
     def debug_dump(self, indent=0):
-        print(f"{' '*(indent+1)}{self._model.name} = {self._value}")
+        print(f"{' '*(indent+1)*(not self._walker.is_local_key)}{self._model.name} = {self._value}{self._debug_dump_metadata()}", end="\n"*(not self._walker.is_local_key))
+
+    def sanity_check(self):
+        expected_type = {
+            "string": str,
+            "empty":  Empty.__class__,
+            "boolean": bool,
+            "decimal64": str,
+            "binary": (bytes, str),
+            "union": object,
+            "enumeration": str,
+            "bits": str,
+            "identityref": str,
+            "int8": int,
+            "int16": int,
+            "int32": int,
+            "int64": int,
+            "uint8": int,
+            "uint16": int,
+            "uint32": int,
+            "uint64": int,
+        }[self._walker.get_type().json_name()]
+        if not isinstance(expected_type, tuple):
+            expected_type = (expected_type, )
+        val = self._value
+        if not self._walker.is_leaflist or isinstance(val, (FieldValuePlaceholder, GetValuePlaceholder, )):
+            val = [val]
+
+        if self._walker.is_leaflist and not isinstance(self._value, (FieldValuePlaceholder, GetValuePlaceholder, )) and self.metadata != None:
+            assert not len(self.metadata) or len(self.metadata) == len(self._value)
+
+        assert all(isinstance(v, (*expected_type, FieldValuePlaceholder, GetValuePlaceholder, )) for v in val)
+
+    def has_metadata(self):
+        if self._walker.is_leaflist:
+            return self.metadata and any(self.metadata)
+        return bool(self.metadata)
 
 
 class _MoStorage(_AStorage):
     """Data storage for containers and list entries (list+local keys).
 
     .. Reviewed by TechComms 20210712
     """
 
-    def __init__(self, model:Model, local_keys, rd:RequestData):
+    def __init__(self, model: Model, local_keys, rd: RequestData):
         super().__init__(rd)
         self._model = model
-        self._local_keys = copy.deepcopy(local_keys)
+        self._local_keys = self._prepare_keys(local_keys)
         self._child = {}
         self._operation = ""
 
+    def _prepare_keys(self, keys):
+        w = self._walker
+        return {k: _FieldStorage(w.get_child(k).current, self.rd, value=copy.deepcopy(v)) for k, v in keys.items()}
+
     def _to_xml(self, ns_map, root):
-        root_attr = {} if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
+        root_attr = {}
+        if self.metadata:
+            root_attr.update(self._metadata_to_xml(self.metadata))
+        if self._operation:
+            root_attr[f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation"""] = self._operation
         root = subelement(root, self._model.name, ns_map, None, root_attr)
-        for k, v in self._local_keys.items():
-            if v is FieldValuePlaceholder():
-                pass
-            elif v is GetValuePlaceholder():
-                self._leaf_placeholder_to_xml(v, root, self._walker.get_child(k), ns_map)
-            else:
-               txt, add_ns = self._walker.get_child(k).get_type().to_string(v)
-               subelement(root, self._walker.get_child(k).current.name, ns_map, txt, {}, add_ns)
-
-        for k, v in self._child.items():
-            v._to_xml(ns_map,root)
+        for v in itertools.chain(self._local_keys.values(), self._child.values()):
+            v._to_xml(ns_map, root)
 
     def to_xml(self, ns_map, root):
-        root_attr = {} if not self._operation else {f"""{{{COMMON_NAMESPACES["ncbase"]}}}operation""": self._operation}
-
         for k, v in self._child.items():
             v._to_xml(ns_map, root)
 
     def _leaf_placeholder_to_xml(self, value, root, walker, ns_map):
         subelement(root, walker.current.name, ns_map)
 
     def to_model(self, *, key_filter={}):
         data = {}
         is_selection_filter = {} in key_filter.values()
         for k, v in self._local_keys.items():
             if is_selection_filter and k not in key_filter:
                 continue
-            data[k] = self._leaf_to_model(k, v)
+            data[k] = v.to_model(key_filter=(key_filter.get(k, {})))
         for k, v in self._child.items():
             key_proxy = DictionaryKeysProxy(self.rd._unwrap(key_filter))
             if is_selection_filter and self._walker.get_child(k).current.name not in key_proxy:
                 continue
             data[k] = v.to_model(key_filter=(key_filter.get(k, {})))
-            if not data[k] and not self._walker.get_child(k).has_explicit_presence():
+            if not data[k] and (not isinstance(data[k], Wrapper) or not len(data[k].annotations)) and not self._walker.get_child(k).has_explicit_presence():
                 del data[k]
         if self._walker.is_root:
             return data
         if self._model.data_def_stm == Model.StatementType.action_:
-            return Action._with_model(data, self._model)
-        return Container._with_model(data, self._model)
-
-    def _leaf_to_model(self, name, value):
-        assert self.rd._action == RequestData._Action.convert or value is not GetValuePlaceholder()
-        assert value is not FieldValuePlaceholder()
-        model = self._walker.get_child(name).current
-        if self._walker.get_child_dds(name) == Model.StatementType.leaf_:
-            return Leaf._with_model(value, model)
-        return LeafList._with_model(value, model)
+            return Action._with_model(data, self._model, annotations=self._metadata_to_model(self.metadata))
+        return Container._with_model(data, self._model, annotations=self._metadata_to_model(self.metadata))
 
     def keys_equal(self, keys):
         """Compare if keys are equal. Keys are expected as dict(name->value).
 
         .. Reviewed by TechComms 20210712
         """
         return self._local_keys == keys
 
     def get_keys_flat(self):
-        keys = tuple(self._local_keys[key] for key in self._model.local_keys)
-        if len(keys) == 1: keys = keys[0]
+        keys = tuple(self._local_keys[key]._value for key in self._model.local_keys)
+        if len(keys) == 1:
+            keys = keys[0]
         return keys
 
     def debug_dump(self, indent=0):
-        line = " "*indent
+        line = " " * indent
         if self._operation:
             line += self._operation + " "
         line += self._walker.get_name().name
+        print(line, end="")
         if self._local_keys:
-            line += " ["
-            line += ", ".join(f"{k}={v}" for k, v in self._local_keys.items())
-            line += "]"
-        line += " {"
-        print(line)
+            print(" [", end="")
+            first = True
+            for v in self._local_keys.values():
+                if not first:
+                    print(" , ", end="")
+                first = False
+                v.debug_dump()
+            print("]", end="")
+        print(" {")
         for k, v in self._child.items():
             if isinstance(v, _AStorage):
-                v.debug_dump(indent+1)
+                v.debug_dump(indent + 1)
             else:
-                print(f"{' '*(indent+1)}{k} = {v}")
-        print((" "*indent)+"}")
+                print(f"{' '*(indent + 1)}{k} = {v}")
+        print((" " * indent) + "}")
+
+    def sanity_check(self):
+        for v in self._child.values():
+            v.sanity_check()
 
 
 class _ListStorage(_AStorage):
     """Storage for all entries for a specific list.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, model:Model, rd:RequestData):
+    def __init__(self, model: Model, rd: RequestData):
         if model.data_def_stm in (Model.StatementType.container_, Model.StatementType.action_):
             self.__class__ = _MoStorage
             self.__class__.__init__(self, model, {}, rd)
         else:
             super().__init__(rd)
             self._model = model
             self._entries = {}
@@ -432,100 +552,132 @@
         assert not self.has_entry(keys)
         res = _MoStorage(self._model, keys, self.rd)
         self._entries[tuple(sorted(keys.items()))] = res
         return res
 
     def debug_dump(self, indent=0):
         for i in self._entries.values():
-            i.debug_dump(indent+1)
+            i.debug_dump(indent + 1)
+
+    def sanity_check(self):
+        for v in self._entries.values():
+            v.sanity_check()
+
 
 class DictionaryKeysProxy():
     """Proxy for dictionary keys which unwraps keys and compares by performing Identifier.__eq__"""
     def __init__(self, data):
         if not isinstance(data, dict):
             raise make_exception(pysros_err_invalid_value, data=data)
         self.data = data
 
-    def __getitem__(self, key:Identifier):
-        #need to call Identifier.__eq__
+    def __getitem__(self, key: Identifier):
+        # need to call Identifier.__eq__
         for k in self.data.keys():
             if key == k:
                 return self._unwrap(self.data[k])
         raise KeyError(key)
 
-    def __contains__(self, val:Identifier):
-        #need to call Identifier.__eq__
+    def __contains__(self, val: Identifier):
+        # need to call Identifier.__eq__
         for ele in self.data:
             if val == ele:
                 return True
         return False
 
     def __str__(self):
         return str(self.data)
 
     def _unwrap(self, val):
         return val.data if isinstance(val, Wrapper) else val
 
+
 class RdJsonEncoder(json.JSONEncoder):
-    def add_ns(self, o, d, walker:ModelWalker):
-        if o is self.root:
+    def add_ns(self, d, is_root, walker: ModelWalker):
+        if is_root:
             return {walker.get_child(k).get_name().model_string: (v if not isinstance(v, _FieldStorage) else v._value) for k, v in d.items()}
         return {walker.get_child(k).get_name().model_string if walker.get_name().prefix != walker.get_child(k).get_name().prefix else k: (v if not isinstance(v, _FieldStorage) else v._value) for k, v in d.items()}
 
     def stringify(self, x, dds):
         return [str(v) for v in x] if dds == Model.StatementType.leaf_list_ else str(x)
 
-    def convert(self, o:_FieldStorage):
+    def convert(self, o: _FieldStorage):
+        if o._value is None:
+            return ""
         return self.stringify(o._value, o._walker.get_dds()) if o._walker.get_type().json_name() in ("int64", "uint64") else o._value
 
     def convert_child(self, o, k, v):
+        if v is None:
+            return ""
         return self.stringify(v, o._walker.get_child_dds(k)) if o._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES and o._walker.get_child_type(k).json_name() in ("int64", "uint64") else v
 
+    def convert_metadata(self, metadata):
+        if isinstance(metadata, list):
+            for i, v in enumerate(metadata):
+                if v == {}:
+                    metadata[i] = None
+            return list(map(self.convert_metadata, metadata))
+        if metadata is None:
+            return None
+        return {k: (str(v) if self.metadata_models[k].yang_type.json_name() in ("int64", "uint64") else v) for k, v in metadata.items()}
+
     def default(self, o):
         is_root = o is self.root
         if isinstance(o, _FieldStorage) and is_root:
             res = {}
+            if o.has_metadata():
+                res[f"@{o._walker.get_name().model_string}"] = self.convert_metadata(o.metadata)
             res[o._walker.get_name().model_string] = self.convert(o)
             return res
         if isinstance(o, _MoStorage):
             res = {}
+            metadata_sources = o._child.items()
             if not is_root:
-                res.update(self.add_ns(o, o._local_keys, o._walker))
+                res.update(self.add_ns(o._local_keys, is_root, o._walker))
+                metadata_sources = itertools.chain(metadata_sources, o._local_keys.items())
             elif is_root and self.force_key:
-                res[o._walker.get_child(self.force_key).get_name().model_string] = o._local_keys[self.force_key]
-            res.update(self.add_ns(o, o._child, o._walker))
+                res[o._walker.get_child(self.force_key).get_name().model_string] = o._local_keys[self.force_key]._value
+                metadata_sources = itertools.chain(metadata_sources, ((self.force_key, o._local_keys[self.force_key]), ))
+            res.update(self.add_ns(o._child, is_root, o._walker))
+
             res = {k: self.convert_child(o, k, v) for k, v in res.items()}
+            metadata = {k: self.convert_metadata(v.metadata) for k, v in metadata_sources if isinstance(v, _FieldStorage) and v.has_metadata()}
+            metadata = self.add_ns(metadata, is_root, o._walker)
+            res.update((f"@{k}", v) for k, v in metadata.items())
+            if o.metadata and not is_root:
+                res["@"] = self.convert_metadata(o.metadata)
             return res
         elif isinstance(o, _ListStorage):
             res = list(o._entries.values())
             return {o._walker.get_name().model_string: res} if is_root else res
         if isinstance(o, _FieldStorage):
             o = o._value
         if isinstance(o, (str, list, dict, bool, int)):
             return o
         elif o is Empty:
             return [None]
         else:
             return str(o)
 
+
 class _ASetter(ABC):
     """Data setter representation for storage classes.
 
     .. Reviewed by TechComms 20210712
     """
-    def __init__(self, storage:"_AStorage", rd:RequestData):
+    def __init__(self, storage: "_AStorage", rd: RequestData):
         self._storage = storage
         self.rd = rd
 
     @property
     def _walker(self):
         return self.rd._Walker(self._storage._model)
 
     @staticmethod
-    def create_setter(storage:"_AStorage", rd:RequestData):
+    def create_setter(storage: "_AStorage", rd: RequestData):
         if isinstance(storage, _MoStorage):
             return _MoSetter(storage, rd)
         else:
             return _ListSetter(storage, rd)
 
     @abstractmethod
     def set(self, value):
@@ -539,14 +691,144 @@
     def set_as_xml(self, value):
         """Set data in xml format.
 
         .. Reviewed by TechComms 20210712
         """
         pass
 
+    def _metadata_from_model(self, value: Wrapper):
+        if not (isinstance(value, Wrapper) and value.annotations):
+            return None
+
+        res = []
+        is_leaflist = isinstance(value, LeafList)
+        if is_leaflist:
+            annotations_list = value.annotations
+            if len(annotations_list) > len(value):
+                raise make_exception(pysros_err_too_many_leaflist_annotations)
+            elif len(value) > len(annotations_list):
+                annotations_list = annotations_list + (len(value) - len(annotations_list)) * [None]
+        else:
+            annotations_list = [value.annotations]
+
+        for annotations in annotations_list:
+            res.append({})
+            if annotations is not None:
+                for annotation in annotations:
+                    if not isinstance(annotation, Annotation):
+                        raise make_exception(
+                            pysros_err_expected_type_but_got_another,
+                            expected='Annotation',
+                            type_name=str(annotation.__class__.__name__)
+                        )
+                    m = self._find_metadata_model_by_annotation(annotation)
+                    name = m.name.model_string
+                    if name in res[-1]:
+                        raise make_exception(
+                            pysros_err_multiple_occurences_of_annotation
+                        )
+                    if not m.yang_type.check_field_value(annotation.data,
+                                                         is_convert=self.rd._action == RequestData._Action.convert):
+                        raise make_exception(
+                            pysros_err_annotation_incorrect_value, name=name
+                        )
+                    res[-1][name] = m.yang_type.to_value(annotation.data)
+        return res if is_leaflist else res[0]
+
+    def _metadata_to_model_type(self, value, *, is_json=False, is_xml=False, nsmap={}):
+        res = []
+        is_leaflist = self._walker.is_leaflist
+        if not is_leaflist:
+            value = [value]
+        for val in value:
+            res.append({})
+            if is_json and val is None:
+                continue
+            for k, v in val.items():
+                m = self._find_metadata_model_by_name(k)
+                name = m.name.model_string
+                if is_json and not m.yang_type.check_field_value(v, json=True,
+                                                                 is_convert=self.rd._action == RequestData._Action.convert):
+                    raise make_exception(
+                        pysros_err_annotation_incorrect_value,
+                        name=name
+                    )
+                if name in res[-1]:
+                    raise make_exception(
+                        pysros_err_multiple_occurences_of_annotation
+                    )
+                res[-1][k] = m.yang_type.to_value(v)
+                if is_xml:
+                    res[-1][k] = self._fix_xml_identityref_prefix(res[-1][k], m.yang_type, nsmap=nsmap)
+        return res if is_leaflist else res[0]
+
+    def _fix_xml_identityref_prefix(self, value, value_type, *, is_leaflist=False, nsmap={}):
+        if isinstance(value_type, (IdentityRef, YangUnion)) and value is not None:
+            if is_leaflist:
+                assert len(value) == 1
+            identity = value_type._find_identity(value[0] if is_leaflist else value, nsmap)
+            if not identity:
+                if isinstance(value_type, IdentityRef):
+                    raise make_exception(
+                        pysros_err_incorrect_leaf_value,
+                        leaf_name=self._walker.current.name.name
+                    )
+            else:
+                value = identity.module + ':' + identity.name
+                if is_leaflist:
+                    value = [value]
+        return value
+
+    def _find_metadata_model_by_annotation(self, ann: Annotation) -> Model:
+        module_name = getattr(ann, "module", None)
+        namespace = getattr(ann, "namespace", None)
+        candidates = self.rd._modeled_metadata_no_module.get(ann.key, [])
+        for m in candidates:
+            if m.name == ann.key:
+                if module_name and module_name != m.name.prefix:
+                    continue
+                if namespace and namespace != m.namespace:
+                    continue
+                return m
+        _raise_unknown_attribute(ann)
+
+    def _find_metadata_model_by_name(self, name) -> Model:
+        id = Identifier.from_model_string(name)
+        if id.is_lazy_bound():
+            candidates = self.rd._modeled_metadata_no_module.get(name)
+            if not candidates:
+                _raise_unknown_attribute(name)
+            return candidates[0]
+        candidate = self.rd._modeled_metadata.get(name)
+        if not candidate:
+            _raise_unknown_attribute(name)
+        return candidate
+
+    def _set_metadata(self, *, model_value=None, json_metadata=None, xml_metadata=None, nsmap={}, json_num_of_leaflist_vals=None):
+        assert sum(map(lambda v: v is not None, (model_value, xml_metadata, json_metadata))) <= 1, "You can specify only one format of metadata"
+        if model_value is not None:
+            self._storage.metadata = self._metadata_from_model(model_value)
+        if xml_metadata is not None:
+            if self._walker.is_leaflist:
+                xml_metadata = [xml_metadata]
+            new_val = self._metadata_to_model_type(xml_metadata, nsmap=nsmap, is_xml=True)
+            if self._walker.is_leaflist and self._storage.metadata:
+                self._storage.metadata.extend(new_val)
+            else:
+                self._storage.metadata = new_val
+        if json_metadata is not None:
+            self._storage.metadata = self._metadata_to_model_type(json_metadata, is_json=True)
+            if self._walker.is_leaflist:
+                assert json_num_of_leaflist_vals is not None
+                if len(self._storage.metadata) > json_num_of_leaflist_vals:
+                    raise make_exception(pysros_err_too_many_leaflist_annotations)
+                self._storage.metadata = self._storage.metadata[:json_num_of_leaflist_vals]
+                if len(self._storage.metadata) < json_num_of_leaflist_vals:
+                    self._storage.metadata += [{}]*(json_num_of_leaflist_vals-len(self._storage.metadata))
+
     def checkJsonDuplicates(x):
         if len(x) != len({i[0] for i in x}):
             raise make_exception(pysros_err_multiple_occurences_of_node)
         return dict(x)
 
     def set_as_json(self, value):
         """Set data in json format."""
@@ -554,61 +836,84 @@
             val = json.loads(value, object_pairs_hook=_ASetter.checkJsonDuplicates)
         except json.JSONDecodeError as e:
             raise JsonDecodeError(*e.args) from None
 
         if not isinstance(val, dict):
             raise make_exception(pysros_err_wrong_json_root)
 
-        self._set_as_json(val, is_root = True)
+        self._set_as_json(val, is_root=True)
 
     @abstractmethod
-    def _set_as_json(self, value, is_root = False):
+    def _set_as_json(self, value, is_root=False):
         """Implementation of setter for JSON."""
         pass
 
-    def to_json(self, pprint = True):
+    def to_json(self, pprint=True):
         """Return data in json format."""
         members = {
             "root": self._storage,
             "root_setter": self,
             "force_key": getattr(self, "_key_name", None),
+            "metadata_models": self.rd._modeled_metadata,
         }
         encoder = type("RdJsonEncoderSpecialization", (RdJsonEncoder, ), members)
         indent = 4 if pprint else None
         return json.dumps(self._storage, cls=encoder, indent=indent)
 
     @abstractmethod
     def delete(self):
         """Set data operation to delete"""
         pass
 
+    def delete_annotations(self, annotations_to_delete):
+        """Delete specified annotations. If True, delete all annotations."""
+        if annotations_to_delete == True:
+            self._storage._metadata = None
+            return
+        elif isinstance(annotations_to_delete, Annotation):
+            annotations_to_delete = (annotations_to_delete, )
+        for ann in annotations_to_delete:
+            try:
+                m = self._find_metadata_model_by_annotation(ann)
+            except:
+                raise make_exception(pysros_err_annotation_invalid)
+            if m.name.name == "operation":
+                raise make_exception(pysros_err_annotation_cannot_delete)
+            elif (self._storage._metadata
+                  and m.name.model_string in self._storage._metadata
+                  and (ann.data == self._storage._metadata[m.name.model_string] if hasattr(ann, "data") else True)):
+                    self._storage._metadata.pop(m.name.model_string)
+
     @abstractmethod
     def replace(self):
         """Set data operation to replace"""
         pass
 
+    @abstractmethod
+    def merge(self):
+        """Set data operation to merge"""
+        pass
+
     def entry_get_keys(self):
         """Set list keys as a placeholders"""
         raise make_exception(pysros_err_target_should_be_list)
 
-
     def to_model(self, *, key_filter={}):
         """Return data in model format.
 
         .. Reviewed by TechComms 20210712
         """
         return self._storage.to_model(key_filter=key_filter)
 
     def to_xml(self):
         """Return data in xml format."""
         root = _create_root_ele()
         self._storage.to_xml(self.rd._ns_map, root)
         return root
 
-
     def set_filter(self, value):
         """Populate request data with filter syntax"""
         raise make_exception(pysros_err_filter_not_supported_on_leaves)
 
     def is_compare_supported_endpoint(self):
         return False
 
@@ -637,28 +942,35 @@
         local_keys = [Identifier(self._walker.get_name().prefix, k) for k in self._walker.get_local_key_names()]
         for k in local_keys:
             if k.model_string in entry:
                 if k.name in entry:
                     raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=entry[k.model_string])
                 entry[k.name] = entry.pop(k.model_string)
 
+
 class _LeafSetter(_ASetter):
     """Interface for managing leafs. Because leafs do not have dedicated storage, the
        class has its own implementation of to_model method.
 
     .. Reviewed by TechComms 20210713
     """
-    def __init__(self, storage:"_FieldStorage", leaf_name:str, rd:RequestData):
+    def __init__(self, storage: "_FieldStorage", leaf_name: str, rd: RequestData):
         super().__init__(storage, rd)
         self._leaf_name = leaf_name
 
     def set(self, value):
+        if not self._storage.metadata:
+            self._set_metadata(model_value=value)
         value = self.rd._unwrap(value)
-        if not self._walker.check_field_value(value):
-            raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._leaf_name)
+        if not self._walker.check_field_value(value, is_convert=self.rd._action == RequestData._Action.convert,
+                                              metadata=self._storage.metadata):
+            raise make_exception(
+                pysros_err_incorrect_leaf_value,
+                leaf_name=self._leaf_name
+            )
         else:
             val = self._as_storage_type(value)
             self._set_nocheck(val)
 
     def _set_nocheck(self, value):
         self._storage._value = value
 
@@ -667,140 +979,156 @@
 
     def set_as_xml(self, value):
         if not len(value):
             raise make_exception(pysros_err_malformed_xml)
         for v in value:
             self.set_or_append_as_xml(v)
 
-    def _set_as_json(self, value, is_root = False):
+    def _set_as_json(self, value, is_root=False):
         if not isinstance(value, dict) or not all(isinstance(k, str) for k in value):
             raise make_exception(pysros_err_invalid_json_structure)
-        value = {k:v for k, v in value.items() if not k.startswith("@")}
-        if len(value) != 1:
+        metadata = {k: v for k, v in value.items() if k.startswith("@")}
+        value = {k: v for k, v in value.items() if not k.startswith("@")}
+        if len(value) != 1 or len(metadata) > 1:
             raise make_exception(pysros_err_invalid_json_structure)
 
         val = next(iter(value.items()))
+        if metadata:
+            metadata = next(iter(metadata.items()))
+            if "@" + val[0] != metadata[0]:
+                raise make_exception(pysros_err_invalid_json_structure)
         if self._walker.get_name() != val[0]:
             raise make_exception(pysros_err_invalid_json_structure)
         val = val[1]
-        if self._walker.get_type().json_name() in ("int64", "uint64"):
+        if self._walker.get_type().json_name() in ("int64", "uint64") and val != "":
             if self._walker.get_dds() != Model.StatementType.leaf_list_:
                 val = [self.rd._unwrap(val)]
             else:
                 val = self.rd._unwrap(val)
             if not isinstance(val, list) or not all(isinstance(v, str) for v in val):
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name)
             try:
                 value = [int(self.rd._unwrap(v)) for v in val]
             except:
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name) from None
         self.set(self._walker.as_model_type(val))
+        if metadata:
+            if self._walker.is_leaflist:
+                self._set_metadata(json_metadata=metadata[1], json_num_of_leaflist_vals=len(self._storage._value))
+            else:
+                self._set_metadata(json_metadata=metadata[1])
 
     def set_or_append_as_xml(self, value_element):
         is_leaflist = self._walker.get_dds() == Model.StatementType.leaf_list_
+        self._set_metadata(xml_metadata=_metadata_from_xml(value_element, self.rd._ns_map_rev), nsmap=value_element.nsmap)
         if _text_in_tag_tail(value_element) or (is_leaflist and _text_in_tag_text(value_element.getparent())):
             _raise_invalid_text_exception(value_element)
-        value = self._walker.as_model_type(value_element.text or "")
-
-        if isinstance(self._walker.get_type(), IdentityRef):
-            is_leaf_list = isinstance(value, list)
-            assert not is_leaf_list or len(value) == 1
-            identity = self._walker.get_type()._find_identity(value[0] if is_leaf_list else value)
-            if not identity:
-                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
-            value_ns = value_element.nsmap.get(identity.module, None)
-            if value_ns is not None and value_ns!=identity.namespace:
-                raise make_exception(pysros_err_incorrect_leaf_value, leaf_name = self._walker.current.name.name)
+        value = self._walker.as_model_type(value_element.text)
+        value = self._fix_xml_identityref_prefix(value, self._walker.get_type(), is_leaflist=is_leaflist, nsmap=value_element.nsmap)
 
         if is_leaflist and isinstance(self._storage._value, list):
             value = self._storage._value + value
         self.set(value)
 
     def to_model(self, *, key_filter={}):
         return self._storage.to_model(key_filter=key_filter)
 
     def to_xml(self):
         root = _create_root_ele()
         self._storage._to_xml(self.rd._ns_map, root)
         return root
 
     def delete(self):
-        if self._walker.get_dds() == Model.StatementType.leaf_list_:
-            raise make_exception(pysros_err_invalid_operation_on_leaflist)
-        self._storage._operation = "delete"
+        self._storage._operation = "remove"
 
     def replace(self):
         self._storage._operation = "replace"
 
+    def merge(self):
+        self._storage._operation = "merge"
+
 class _KeySetter(_ASetter):
+
     """Interface for keys. Most of this class are stub methods to provide
        setter interface to keys."""
-    def __init__(self, storage:"_ListStorage", key_name:str, rd:RequestData):
-        super().__init__(storage, rd)
+    def __init__(self, storage: "_MoStorage", key_name: str, rd: RequestData):
+        super().__init__(storage._local_keys[key_name], rd)
         self._key_name = key_name
 
     def set(self, value):
+        if not self._storage.metadata:
+            self._set_metadata(model_value=value)
         value = self.rd._unwrap(value)
-        if not self._walker.check_field_value(value):
+        if not self._walker.check_field_value(value, is_convert=self.rd._action == RequestData._Action.convert,
+                                              metadata=self._storage.metadata):
             raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._key_name)
-        elif self._as_storage_type(value) != self._storage._local_keys[self._key_name]:
+        elif self._as_storage_type(value) != self._storage._value:
             raise make_exception(pysros_err_key_val_mismatch, key_name=self._key_name)
 
     def set_getValue(self):
         pass
 
     def set_placeholder(self):
         pass
 
     def to_model(self, *, key_filter={}):
-        return self._storage._leaf_to_model(self._key_name, self._storage._local_keys[self._key_name])
+        return self._storage.to_model()
 
     def to_xml(self):
         root = _create_root_ele()
-        _leaf_to_xml(self._storage._local_keys[self._key_name], root, self._walker, self.rd._ns_map)
+        self._storage._to_xml(self.rd._ns_map, root)
         return root
 
     def delete(self):
         raise make_exception(pysros_err_invalid_operation_on_key)
 
     def replace(self):
         raise make_exception(pysros_err_invalid_operation_on_key)
 
+    def merge(self):
+        pass
+
     def set_as_xml(self, value):
         if _text_in_tag_tail(value):
             _raise_invalid_text_exception(value_element)
         if not len(value):
             raise make_exception(pysros_err_malformed_xml)
         for v in value:
             if _text_in_tag_tail(v):
                 _raise_invalid_text_exception(v)
+            self._set_metadata(xml_metadata=_metadata_from_xml(v, self.rd._ns_map_rev), nsmap=value.nsmap)
             self.set(self._walker.as_model_type(v.text or ""))
 
-    def _set_as_json(self, value, is_root = False):
+    def _set_as_json(self, value, is_root=False):
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_json_structure)
-        value = {k:v for k, v in value.items() if not k.startswith("@")}
-        if  len(value) != 1:
+        metadata = {k: v for k, v in value.items() if k.startswith("@")}
+        value = {k: v for k, v in value.items() if not k.startswith("@")}
+        if len(value) != 1 or len(metadata) > 1:
             raise make_exception(pysros_err_invalid_json_structure)
 
         val = next(iter(value.items()))
+        if metadata:
+            metadata = next(iter(metadata.items()))
+            if "@" + val[0] != metadata[0]:
+                raise make_exception(pysros_err_invalid_json_structure)
+
         if self._walker.get_name() != val[0]:
             raise make_exception(pysros_err_invalid_json_structure)
         if self._walker.get_type().json_name() in ("int64", "uint64"):
             if not isinstance(val[1], str):
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name)
             try:
                 value = int(val[1])
             except:
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=self._walker.get_name().name) from None
         self.set(self._walker.as_model_type(val[1]))
+        if metadata:
+            self._set_metadata(json_metadata=metadata[1])
 
-    @property
-    def _walker(self):
-        return super()._walker.get_child(self._key_name)
 
 class _ListSetter(_ASetter):
     """Interface for managing instances of specific list.
 
     .. Reviewed by TechComms 20210712
     """
 
@@ -809,70 +1137,76 @@
 
         Keys may be in format {(key1, key2) : Container({}), (key1, key2) : Container({})}
         or directly in entry {key1: value1, key2: value2, field1 : value}.
 
         .. Reviewed by PLM 20211018
         """
         is_wrapped = isinstance(value, Container)
+        wrapped = value
         value = self.rd._unwrap(value)
         value = copy.copy(value)
         unwrapper = DictionaryKeysProxy(value)
         if value and not is_wrapped and self._walker.dict_keys(value):
             for k, v in value.items():
                 self._handle_entry_keys_namespaces(v)
                 self.entry(self._tuple_to_dict(k)).set(v)
         elif self._walker.entry_keys(unwrapper):
             self._handle_entry_keys_namespaces(value)
-            self.entry(value).set(value)
+            self.entry(value).set(value, wrapped=wrapped)
         else:
             raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=value)
 
     def set_filter(self, value):
         value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
         for k in self._walker.get_local_key_names():
             if k not in value:
                 value[k] = FieldValuePlaceholder()
         self.entry_nocheck(value).set_filter(value)
 
     def _tuple_to_dict(self, t):
-        return {k:v for k, v in zip(self._walker.get_local_key_names(), (t if isinstance(t, tuple) else (t, )))}
+        return {k: v for k, v in zip(self._walker.get_local_key_names(), (t if isinstance(t, tuple) else (t, )))}
 
     def _extract_keys(self, entry):
-        return {k:self._as_storage_type(v, child_name=k) for k, v in entry.items() if k in self._walker.get_local_key_names()}
+        return {k: self._as_storage_type(v, child_name=k) for k, v in entry.items() if k in self._walker.get_local_key_names()}
 
     def _convert_keys_to_model(self, entry):
         try:
             def unwrap(v):
                 return v.data if isinstance(v, Wrapper) else v
-            val =  {k: (GetValuePlaceholder() if unwrap(v) in (GetValuePlaceholder(), {}) else self._walker.as_child_model_type(k, unwrap(v))) for k, v in entry.items() if v is not FieldValuePlaceholder()}
+            val = {k: (GetValuePlaceholder() if unwrap(v) in (GetValuePlaceholder(), {}) else self._walker.as_child_model_type(k, unwrap(v))) for k, v in entry.items() if v is not FieldValuePlaceholder()}
             return val
         except:
             raise make_exception(pysros_err_invalid_key_in_path) from None
 
     def _check_and_unwrap_keys(self, entry, *, json=False):
         for k in self._walker.get_local_key_names():
             if k not in entry:
-                raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=k)
+                raise make_exception(
+                    pysros_err_malformed_keys,
+                    full_path=self._walker, value=k
+                )
             entry[k] = self.rd._unwrap(entry[k])
-            if not self._walker.check_child_field_value(k, entry[k], json=json):
+            if not self._walker.check_child_field_value(k, entry[k], json=json, strict=True):
                 raise make_exception(pysros_err_incorrect_leaf_value, leaf_name=k)
             entry[k] = self._walker.get_child_type(k).as_storage_type(entry[k], self.rd._action == RequestData._Action.convert, self.rd._add_xml_namespace)
 
     def entry(self, value, *, json=False):
         """Receive entry with specified keys in value. Keys are expected as dict(name->value). Additional
         fields may be present (no verification for extra fields).
 
         .. Reviewed by TechComms 20210712
         """
-        if json:
-            value = copy.copy(value)
+        value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
         self._check_and_unwrap_keys(value, json=json)
-        return _MoSetter(self._storage.get_or_create_entry(self._extract_keys(value)), self.rd)
+        return _MoSetter(
+            self._storage.get_or_create_entry(self._extract_keys(value)),
+            self.rd
+        )
 
     def add_entry(self, value, *, json=False):
         if json:
             value = copy.copy(value)
         self._handle_entry_keys_namespaces(value)
         self._check_and_unwrap_keys(value, json=json)
         keys = self._extract_keys(value)
@@ -882,14 +1216,15 @@
 
     def entry_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields).
 
         .. Reviewed by PLM 20211018
         """
+
         return _MoSetter(self._storage.get_or_create_entry(self._convert_keys_to_model(self._extract_keys(value))), self.rd)
 
     def entry_exists_nocheck(self, value):
         """Receive entry with specified keys in value without checking for the correct type. Keys are expected
         as dict(name->value). Additional fields may be present (no verification for extra fields)
         Returns true if entry exists, otherwise false.
         """
@@ -899,28 +1234,31 @@
         keys = {}
         for e in value:
             if _get_tag_name(e) in self._walker.get_local_key_names():
                 if _text_in_tag_tail(e):
                     _raise_invalid_text_exception(e)
                 keys[_get_tag_name(e)] = e.text or ""
         if set(keys.keys()) != set(self._walker.get_local_key_names()):
-            raise make_exception(pysros_err_malformed_keys, full_path=self._walker, value=keys)
+            raise make_exception(
+                pysros_err_malformed_keys,
+                full_path=self._walker, value=keys
+            )
         if self.entry_exists_nocheck(keys):
             raise make_exception(pysros_err_multiple_occurences_of_entry)
         return self.entry_nocheck(keys)
 
     def set_as_xml(self, value):
         for v in value:
             self.entry_xml(v).set_as_xml(v)
 
-    def _set_as_json(self, value, is_root = False):
+    def _set_as_json(self, value, is_root=False):
         if is_root:
             if not isinstance(value, dict):
                 raise make_exception(pysros_err_invalid_json_structure)
-            value = {k:v for k, v in value.items() if not k.startswith("@")}
+            value = {k: v for k, v in value.items() if not k.startswith("@")}
             if len(value) != 1:
                 raise make_exception(pysros_err_invalid_json_structure)
             value = next(iter(value.items()))
             if self._walker.get_name() != value[0] or not isinstance(value[1], list):
                 raise make_exception(pysros_err_invalid_json_structure)
             value = value[1]
         else:
@@ -932,59 +1270,72 @@
     def delete(self):
         raise make_exception(pysros_err_invalid_path_operation_missing_keys)
 
     def replace(self):
         for k, v in self._storage._entries.items():
             v._operation = "replace"
 
+    def merge(self):
+        for k, v in self._storage._entries.items():
+            v._operation = "merge"
+
     def entry_get_keys(self):
-        keys = {key:GetValuePlaceholder() for key in self._walker.get_local_key_names()}
+        keys = {key: GetValuePlaceholder() for key in self._walker.get_local_key_names()}
         setter = _MoSetter(self._storage.get_or_create_entry(keys), self.rd)
         setter.set({})
         return setter
 
+    def _set_metadata(self, *, model_value=None, json_metadata=None, xml_metadata=None):
+        assert False, "metadata should not be supported in ListSetter"
+
+
 class _MoSetter(_ASetter):
     """Interface managing specific list entry or container.
 
     .. Reviewed by TechComms 20210712
     """
     class _AChild:
-        def __init__(self, setter:"_MoSetter"):
+        def __init__(self, setter: "_MoSetter"):
             self._setter = setter
 
         @property
         def _walker(self):
             return self._setter.rd._Walker(self._setter._storage._model)
 
     class _Keys(_AChild):
         """Interface for retrieving and setting keys.
 
         .. Reviewed by TechComms 20210712
         """
+
         def set(self, name, value):
             name = Identifier.from_model_string(name).name
             self.get(name).set(value)
 
         def set_as_json(self, name, value):
             name = Identifier.from_model_string(name).name
             self.get(name)._set_as_json({name: value})
 
         def set_getValue(self, name):
+            if not self.contains(name):
+                self._setter._storage._local_keys[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd, value=FieldValuePlaceholder())
             self.get(name).set_getValue()
 
         def set_placeholder(self, name):
+            if not self.contains(name):
+                self._setter._storage._local_keys[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd, value=FieldValuePlaceholder())
             self.get(name).set_placeholder()
 
         def get(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
             return _KeySetter(self._setter._storage, name, self._setter.rd)
 
         def contains(self, name):
-            return self.can_contains(name)
+            return name in self._setter._storage._local_keys
 
         def can_contains(self, name):
             return self._walker.has_local_key_named(name)
 
     class _Fields(_AChild):
         """Interface for retrieving and setting fields.
 
@@ -1013,26 +1364,25 @@
                 self._setter._storage._child[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd)
             return _LeafSetter(self._setter._storage._child[name], name, self._setter.rd)
 
         def get_nonexisting(self, name):
             if not self.can_contains(name):
                 raise make_exception(pysros_err_unknown_child, child_name=name, path=self._walker._get_path())
             if self.contains(name) and self._walker.get_child_dds(name) != Model.StatementType.leaf_list_:
-                raise make_exception(pysros_err_multiple_occurences_of_node) #rewrite these two conditions
+                raise make_exception(pysros_err_multiple_occurences_of_node)
             if not self.contains(name):
                 self._setter._storage._child[name] = _FieldStorage(self._setter._walker.get_child(name).current, self._setter.rd)
             return _LeafSetter(self._setter._storage._child[name], name, self._setter.rd)
 
         def contains(self, name):
             return name in self._setter._storage._child
 
         def can_contains(self, name):
             return self._walker.has_field_named(name)
 
-
     class _ChildMos(_AChild):
         """Interface for retrieving and setting children.
 
         .. Reviewed by TechComms 20210712
         """
         def set(self, name, value):
             self.get_or_create(Identifier.from_model_string(name).name).set(value)
@@ -1048,55 +1398,66 @@
             else:
                 raise KeyError(name)
 
         def get(self, name):
             if self._walker.get_child_dds(name) in MO_STATEMENT_TYPES:
                 if self.is_created(name):
                     if not self._walker.get_child_dds(name) == Model.StatementType.list_:
-                        raise make_exception(pysros_err_multiple_occurences_of_node)
+                        raise make_exception(pysros_err_multiple_occurences_of_annotation)
                 else:
                     self._setter._storage._child[name] = _ListStorage(self._setter._walker.get_child(name).current, self._setter.rd)
-                return _ASetter.create_setter(self._setter._storage._child[name], self._setter.rd)
+                return _ASetter.create_setter(
+                    self._setter._storage._child[name], self._setter.rd
+                )
             else:
                 raise KeyError(name)
 
         def is_created(self, name):
-            return self._walker.get_child_dds(name) in MO_STATEMENT_TYPES and name in self._setter._storage._child
-
+            return (
+                self._walker.get_child_dds(name) in MO_STATEMENT_TYPES and
+                name in self._setter._storage._child
+            )
 
     @property
     def keys(self):
         return self._Keys(self)
 
     @property
     def fields(self):
         return self._Fields(self)
 
     @property
     def child_mos(self):
         return self._ChildMos(self)
 
-    def set(self, value):
+    def set(self, value, *, wrapped=None):
+        self._set_metadata(model_value=(wrapped if wrapped is not None else value))
         value = self.rd._unwrap(value)
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_value, data=value)
         children_to_set = set()
         walker = self._walker
         for k, v in value.items():
             if k in walker.get_local_key_names():
                 self.keys.set(k, v)
             elif walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
                 self.fields.set(k, v)
             elif walker.get_child_dds(k) in MO_STATEMENT_TYPES:
                 self.child_mos.set(k, v)
             else:
-                raise make_exception(pysros_err_unknown_dds, dds=walker.get_child_dds(k))
+                raise make_exception(
+                    pysros_err_unknown_dds,
+                    dds=walker.get_child_dds(k)
+                )
             name = Identifier.from_model_string(k).name
             if name in children_to_set:
-                raise make_exception(pysros_err_duplicate_found, duplicate=name)
+                raise make_exception(
+                    pysros_err_duplicate_found,
+                    duplicate=name
+                )
             children_to_set.add(name)
 
     def set_filter(self, value):
         value = self.rd._unwrap(value)
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_value, data=value)
         self._handle_entry_keys_namespaces(value)
@@ -1114,21 +1475,28 @@
                 if v == {}:
                     self.fields.set_getValue(k)
                 else:
                     self.fields.set(k, v)
             elif self._walker.get_child_dds(k) in MO_STATEMENT_TYPES:
                 self.child_mos.get_or_create(k).set_filter(v)
             else:
-                raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
+                raise make_exception(
+                    pysros_err_unknown_dds,
+                    dds=self._walker.get_child_dds(k)
+                )
             name = Identifier.from_model_string(k).name
             if name in children_to_set:
-                raise make_exception(pysros_err_duplicate_found, duplicate=name)
+                raise make_exception(
+                    pysros_err_duplicate_found,
+                    duplicate=name
+                )
             children_to_set.add(name)
 
     def set_as_xml(self, value):
+        self._set_metadata(xml_metadata=_metadata_from_xml(value, self.rd._ns_map_rev), nsmap=value.nsmap)
         walker = self._walker
         if self.rd._action != RequestData._Action.convert:
             walker.return_blocked_regions = True
         if _text_in_tag_text(value):
             _raise_invalid_text_exception(value, check_parent_tag=False)
         if _text_in_tag_tail(value):
             _raise_invalid_text_exception(value)
@@ -1143,61 +1511,87 @@
                         self.fields.get_nonexisting(_get_tag_name(e)).set_or_append_as_xml(e)
                     elif self.rd._action == RequestData._Action.convert:
                         xml = to_ele(f"<{_get_tag_name(value)}>{etree.tostring(e, encoding='unicode')}</{_get_tag_name(value)}>")
                         _KeySetter(self._storage, _get_tag_name(e), self.rd).set_as_xml(xml)
                 elif walker.get_child_dds(_get_tag_name(e)) in MO_STATEMENT_TYPES:
                     self.child_mos.get(_get_tag_name(e)).entry_xml(e).set_as_xml(e)
 
-    def _set_as_json(self, value, is_root = False):
+    def _set_as_json(self, value, is_root=False):
         if not isinstance(value, dict):
             raise make_exception(pysros_err_invalid_json_structure)
 
         children_to_set = set()
         already_set = set()
+
         def check_duplicates(name):
             if name in children_to_set:
-                raise make_exception(pysros_err_duplicate_found, duplicate=name)
+                raise make_exception(
+                    pysros_err_duplicate_found,
+                    duplicate=name
+                )
             children_to_set.add(name)
 
         for k, v in value.items():
-            if k.startswith("@"):
+            if k == "@":
+                self._set_metadata(json_metadata=v)
+                continue
+            elif k.startswith("@"):
                 k = k[1:]
-                self._walker.get_child(k) #module name check?
+                self._walker.get_child(k)
                 name = Identifier.from_model_string(k).name
+
+                if self.keys.can_contains(name):
+                    self.keys.get(name)._set_metadata(json_metadata=v)
+                    continue
+
                 if not self.fields.can_contains(name):
-                    raise make_exception(pysros_err_unknown_field, field_name=name, path=self._walker._get_path())
+                    raise make_exception(
+                        pysros_err_unknown_field,
+                        field_name=name, path=self._walker._get_path()
+                    )
                 if k not in value:
-                    raise make_exception(pysros_err_annotation_without_value, child_name=name, path=self._walker._get_path())
-                if not self.fields.contains(name):
-                    self.fields.set_as_json(name, value[k])
-                    check_duplicates(name)
-                    already_set.add(name)
+                    raise make_exception(
+                        pysros_err_annotation_without_value,
+                        child_name=name, path=self._walker._get_path()
+                    )
+                self.fields.get(name)._set_as_json({k: value[k], f"@{k}": v})
+                check_duplicates(name)
+                already_set.add(name)
                 continue
-            self._walker.get_child(k) #module name check?
-            k = Identifier.from_model_string(k).name
-            if k in already_set:
+            self._walker.get_child(k)
+            name = Identifier.from_model_string(k).name
+            if name in already_set:
                 continue
-            if k in self._walker.get_local_key_names():
-                self.keys.set_as_json(k, v)
-            elif self._walker.get_child_dds(k) in FIELD_STATEMENT_TYPES:
-                self.fields.set_as_json(k, v)
-            elif self._walker.get_child_dds(k) in MO_STATEMENT_TYPES:
-                self.child_mos.set_as_json(k, v)
+            if name in self._walker.get_local_key_names():
+                self.keys.set_as_json(name, v)
+            elif self._walker.get_child_dds(name) in FIELD_STATEMENT_TYPES:
+                if f"@{k}" in value:
+                    continue
+                self.fields.set_as_json(name, v)
+            elif self._walker.get_child_dds(name) in MO_STATEMENT_TYPES:
+                self.child_mos.set_as_json(name, v)
             else:
-                raise make_exception(pysros_err_unknown_dds, dds=self._walker.get_child_dds(k))
-            check_duplicates(k)
+                raise make_exception(
+                    pysros_err_unknown_dds,
+                    dds=self._walker.get_child_dds(name)
+                )
+            check_duplicates(name)
 
     def delete(self):
         self._storage._operation = "delete"
 
     def replace(self):
         self._storage._operation = "replace"
 
+    def merge(self):
+        self._storage._operation = "merge"
+
     def is_compare_supported_endpoint(self):
         return True
 
+
 class GetValuePlaceholder(metaclass=_Singleton):
     pass
 
+
 class FieldValuePlaceholder(metaclass=_Singleton):
     pass
-
```

### Comparing `pysros-23.7.2/pysros/singleton.py` & `pysros-24.3.1/pysros/singleton.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,60 @@
 # Copyright 2021-2023 Nokia
 
 class _Singleton(type):
     _instances = {}
+
     def __new__(cls, *args, **kwargs):
         res = super(_Singleton, cls).__new__(cls, *args, **kwargs)
-        res.__copy__     = lambda self: self
+        res.__copy__ = lambda self: self
         res.__deepcopy__ = lambda self, memo: self
-        res.__reduce__   = lambda self: (self.__class__, ())
+        res.__reduce__ = lambda self: (self.__class__, ())
         return res
 
     def __call__(cls, *args, **kwargs):
         assert args == () and kwargs == {}
         if cls not in cls._instances:
             cls._instances[cls] = super(_Singleton, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
+
 class _Empty(metaclass=_Singleton):
     """Representation of whether empty leaf is present.
 
     .. Reviewed by TechComms 20210712
     """
 
     def __str__(self):
         return "Empty"
 
     def __repr__(self):
         return "Empty"
 
+
 Empty = _Empty()
-Empty.__doc__="""Define the YANG ``empty`` type.
+Empty.__doc__ = """Define the YANG ``empty`` type.
 
     The YANG ``empty`` type is not the same as an empty string ``""`` or as the ``None``
     type in Python.  It requires specific translation depending on whether it is being
     used in XML or in JSON IETF encodings.
 
     The :py:class:`Empty` class is used to represent the value of a node that is of the
     YANG type ``empty``.
 
     .. code-block:: python
        :caption: Example - Obtaining YANG ``empty`` type values
        :name: pysros-singleton-empty-example-get
 
        >>> connection_object.running.get('/nokia-conf:configure/system/grpc/allow-unsecure-connection')
        Leaf(Empty)
-       
+
     .. code-block:: python
        :caption: Example - Configuring a YANG ``empty`` type
        :name: pysros-singleton-empty-example-set
 
        >>> from pysros.management import Empty
        >>> connection_object.candidate.set('/nokia-conf:configure/system/grpc/allow-unsecure-connection', Empty)
-     
+
     .. Reviewed by PLM 20230228
     .. Reviewed by TechComms 20230302
 
 """
```

### Comparing `pysros-23.7.2/pysros/tokenizer.py` & `pysros-24.3.1/pysros/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021-2023 Nokia
 
 import collections
 import re
 
 from .errors import *
-
+from .errors import make_exception
 
 NL_RE = "[\n]+"
 WSP_RE = "[ \t\r]+"
 SINGLELINE_COMMENT_RE = "[/][/][^\n]*"
 MULTILINE_COMMENT_RE = "[/][*].*?[*][/]"
 UNQUOTED_STR_RE = """[^ \t\r\n"';{}](?:[^ \t\r\n;{}/]|[/*](?=[^/])|[/](?=[^/*]))*"""
 QUOTED_STR_RE = """\
@@ -29,15 +29,14 @@
 |(?P<STMT_END>{STMT_END_RE})\
 |(?P<BLOCK_BEGIN>{BLOCK_BEGIN_RE})\
 |(?P<BLOCK_END>{BLOCK_END_RE})\
 |(?P<REST>.)\
 )""", re.DOTALL)
 
 
-
 TOKEN_KIND_STR = 0
 TOKEN_STMT_END = 1
 TOKEN_BLOCK_BEGIN = 2
 TOKEN_BLOCK_END = 3
 TOKEN_COMMENT = 4
 
 TOKEN_NAME_TO_ID = {
@@ -46,26 +45,28 @@
     "STMT_END": TOKEN_STMT_END,
     "BLOCK_BEGIN": TOKEN_BLOCK_BEGIN,
     "BLOCK_END": TOKEN_BLOCK_END,
     "SINGLELINE_COMMENT_RE": TOKEN_COMMENT,
     "MULTILINE_COMMENT_RE": TOKEN_COMMENT,
 }
 
-def tokenize(s:str):
+
+def tokenize(s: str):
     for i in re.finditer(TOKEN_REGEX, s):
         if i.lastgroup in ("WSP", "SINGLELINE_COMMENT"):
             continue
         if i.lastgroup in ("NEW_LINES", "MULTILINE_COMMENT"):
             continue
         assert i.lastgroup != "REST"
         val = i.group()
         if i.lastgroup == "QUOTED_STR":
             val = val[1:-1]
         yield (TOKEN_NAME_TO_ID[i.lastgroup], val)
 
+
 def yang_parser(yang, handler):
     it = iter(tokenize(yang))
     stack = collections.deque()
     ahead_token = None
 
     def get_token(expected):
         nonlocal ahead_token
```

### Comparing `pysros-23.7.2/pysros/yang_type.py` & `pysros-24.3.1/pysros/yang_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,76 +1,57 @@
 # Copyright 2021-2023 Nokia
 
 import base64
-
 from abc import ABC, abstractmethod
-from collections import OrderedDict, namedtuple
-from enum import Enum
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Set, Type, Tuple, Union, NamedTuple, Iterable
-
-from lxml.etree import SubElement
+from collections import OrderedDict
+from typing import (Any, Dict, Iterable, List, Mapping, NamedTuple, Optional,
+                    Set, Tuple, Union)
 
 from .errors import *
-from .identifier import Identifier, NoModule
+from .errors import make_exception
+from .identifier import Identifier
 from .model_path import ModelPath
 from .singleton import Empty
 
-
-INTEGRAL_LEAF_TYPE      = ("int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64")
-DECIMAL_LEAF_TYPE       = INTEGRAL_LEAF_TYPE + ("decimal64",)
-YANG_PRIMITIVE_TYPES    = INTEGRAL_LEAF_TYPE + ("binary", "boolean", "decimal64", "empty", "string", "instance-identifier")
+INTEGRAL_LEAF_TYPE = ("int8", "int16", "int32", "int64", "uint8", "uint16", "uint32", "uint64")
+DECIMAL_LEAF_TYPE = INTEGRAL_LEAF_TYPE + ("decimal64",)
+YANG_PRIMITIVE_TYPES = INTEGRAL_LEAF_TYPE + (
+    "binary", "boolean", "decimal64", "empty", "string", "instance-identifier"
+)
 
 INTEGRAL_TYPES_MIN = {
     'uint8':    "0",
     'uint16':   "0",
     'uint32':   "0",
     'uint64':   "0",
     'int8':     str(-(2**7)),
     'int16':    str(-(2**15)),
     'int32':    str(-(2**31)),
-    'int64':    str(-(2**63)+1),
+    'int64':    str(-(2**63) + 1),
 }
 
 INTEGRAL_TYPES_MAX = {
-    'int8':     str((2**7)-1),
-    'uint8':    str((2**8)-1),
-    'int16':    str((2**15)-1),
-    'uint16':   str((2**16)-1),
-    'int32':    str((2**31)-1),
-    'uint32':   str((2**32)-1),
-    'int64':    str((2**63)-1),
-    'uint64':   str((2**64)-1),
+    'int8':     str((2 ** 7) - 1),
+    'uint8':    str((2 ** 8) - 1),
+    'int16':    str((2 ** 15) - 1),
+    'uint16':   str((2 ** 16) - 1),
+    'int32':    str((2 ** 31) - 1),
+    'uint32':   str((2 ** 32) - 1),
+    'int64':    str((2 ** 63) - 1),
+    'uint64':   str((2 ** 64) - 1),
 }
 
 assert set(INTEGRAL_LEAF_TYPE) == set(INTEGRAL_TYPES_MIN.keys()) == set(INTEGRAL_TYPES_MAX.keys())
 
-IP_TYPES = {
-    Identifier('ietf-inet-types',       'ip-address'),
-    Identifier('ietf-inet-types',       'ip-address-no-zone'),
-    Identifier('ietf-inet-types',       'ip-prefix'),
-    Identifier('nokia-types-sros',      'ip-address'),
-    Identifier('nokia-types-sros',      'ip-address-with-zone'),
-    Identifier('nokia-types-sros',      'ip-prefix'),
-    Identifier('nokia-types-sros',      'ip-prefix-with-host-bits'),
-    Identifier('nokia-types-sros',      'ip-multicast-address'),
-    Identifier('nokia-types-sros',      'ip-multicast-prefix'),
-    Identifier('nokia-types-sros',      'ip-unicast-address'),
-    Identifier('nokia-types-sros',      'ip-unicast-address-with-zone'),
-    Identifier('nokia-types-sros',      'ip-unicast-without-local-address'),
-    Identifier('nokia-types-sros',      'ip-unicast-or-linklocal-without-site-or-unique-local-address'),
-    Identifier('nokia-types-sros',      'ip-unicast-prefix'),
-    Identifier('openconfig-inet-types', 'ip-address'),
-    Identifier('openconfig-inet-types', 'ip-prefix'),
-}
-
 class YangTypeBase(ABC):
     """Abstract interface for all leaf types.
 
     .. Reviewed by TechComms 20210713
     """
+
     @abstractmethod
     def __str__(self):
         pass
 
     @abstractmethod
     def __repr__(self):
         pass
@@ -86,94 +67,111 @@
         assert isinstance(other, YangTypeBase)
         return self.__class__ is other.__class__
 
     @property
     def name(self):
         return self.__str__()
 
-    def to_string(self, val: Any) -> Tuple[str, str]:
+    def to_string(self, val: Any) -> Tuple[str, Optional[str]]:
         """Translate value to xml text without any checking."""
         # User input is also checked by check_field_value, paths are not
+        if val is None:
+            return '', None
         if isinstance(val, bool) and isinstance(self, PrimitiveType):
             if self.identifier.name == 'boolean':
                 return str(val).lower(), None
             assert self.identifier.name in INTEGRAL_LEAF_TYPE
             return str(int(val)), None
         if isinstance(val, (int, str)):
             return str(val), None
         if val is Empty:
             return '', None
         if isinstance(val, bytes):
             return base64.b64encode(val).decode('utf8'), None
-        raise make_exception(pysros_err_unexpected_value_of_type, val_type=type(val), type=str(self))
+        raise make_exception(
+            pysros_err_unexpected_value_of_type,
+            val_type=type(val), type=str(self)
+        )
 
     def to_value(self, val: str) -> Any:
         """Transform string to native Python type.
+
             If the value does not fit the expected type, a TypeError exception is raised. This exception is tested
             in union."""
-        raise make_exception(pysros_err_invalid_value_for_type, type=self, value=val)
+        raise make_exception(
+            pysros_err_invalid_value_for_type, type=self, value=val
+        )
 
     @abstractmethod
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
         """Check whether value is acceptable for a specific yang_type."""
         return False
 
     def json_name(self) -> str:
         return self.__class__.__name__.lower()
 
     def as_storage_type(self, obj, is_convert, idref_cb):
+        if obj is None:
+            return ""
         return obj
 
 
 def _is_valid_decimal64(value: str) -> bool:
     return isinstance(value, str)
 
+
 def _is_valid_base64(value: Any) -> bool:
     return isinstance(value, (bytes, str))
 
+
 class PrimitiveType(YangTypeBase):
     """Primitive built-in types representation, such as int8, str, and binary. All types are in YANG_PRIMITIVE_TYPES.
 
     .. Reviewed by TechComms 20210713
     """
+
     def __init__(self, name: str, yang_range: Optional[str] = None, fraction_digits: Optional[int] = None, length: Optional[str] = None):
         assert name in YANG_PRIMITIVE_TYPES
-        self.identifier         = Identifier.builtin(name)
-        self.yang_range         = yang_range
-        self.fraction_digits    = fraction_digits
-        self.length             = length
+        self.identifier = Identifier.builtin(name)
+        self.yang_range = yang_range
+        self.fraction_digits = fraction_digits
+        self.length = length
 
     def __str__(self):
         return str(self.identifier)
 
     def __repr__(self):
         if self.yang_range:
             repr_str = f"(name={self.identifier.name!r}, yang_range={self.yang_range!r})"
         else:
             repr_str = f"({self.identifier.name!r})"
         return self.__class__.__name__ + repr_str
 
     def __eq__(self, other):
         if not YangTypeBase.__eq__(self, other):
             return False
-        return all((
-            self.identifier         == other.identifier,
-            self.yang_range         == other.yang_range,
-            self.fraction_digits    == other.fraction_digits,
-        ))
+        return (
+            self.identifier == other.identifier and
+            self.yang_range == other.yang_range and
+            self.fraction_digits == other.fraction_digits
+        )
 
     def __hash__(self):
         return hash((
             self.identifier,
             self.yang_range,
             self.fraction_digits,
         ))
 
     def to_value(self, val: str) -> Any:
         t = self.identifier.name
+        if val is None or val == "":
+            if t == "empty":
+                return Empty
+            return ("" if t in ("string", "decimal64", "binary") else None)
         if t in INTEGRAL_LEAF_TYPE:
             return int(val)
         if t == "boolean":
             if isinstance(val, str) and val.lower() in ("true", "false"):
                 return val.lower() == "true"
             elif isinstance(val, bool):
                 return val
@@ -182,50 +180,63 @@
         if t in ("string", "binary"):
             return val
         if t == "decimal64":
             return val
         return super().to_value(val)
 
     _check_field_value = {
-        "string":   lambda val: type(val) == str,
-        "empty":    lambda val:  val is Empty,
-        "boolean":  lambda val:  isinstance(val, bool),
+        "string": lambda val: type(val) == str,
+        "empty": lambda val:  val is Empty,
+        "boolean": lambda val:  isinstance(val, bool),
         "decimal64": _is_valid_decimal64,
         "binary": _is_valid_base64
     }
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
         name = self.identifier.name
+        if not strict and value is None:
+            if not is_convert and name == "empty":
+                return metadata and metadata.get("ietf-netconf:operation") in ("remove", "delete")
+            return True
         cmp = self._check_field_value.get(name, None)
         if cmp is not None:
             return cmp(value)
 
         if json and name in ("int64", "uint64"):
             return isinstance(name, str)
         elif name in INTEGRAL_LEAF_TYPE:
             return isinstance(value, int) and not isinstance(value, bool)
         return False
 
     def json_name(self) -> str:
         return self.identifier.name
 
     def as_storage_type(self, obj, is_convert, idref_cb):
+        if obj is None:
+            if self.identifier.name == "empty":
+                return Empty
+            elif self.identifier.name in ("string", "decimal64", "binary"):
+                return ""
+            else:
+                return obj
         if self.identifier.name == "boolean" and type(obj) == int:
             return bool(obj)
         elif self.identifier.name in INTEGRAL_LEAF_TYPE and (type(obj) == bool or self.identifier.name in ("int64", "uint64")):
             return int(obj)
         return super().as_storage_type(obj, is_convert, idref_cb)
 
+
 class UnresolvedIdentifier(YangTypeBase):
     """Identifier that has not been resolved yet."""
+
     def __init__(self, identifier: Identifier, yang_range: Optional[str] = None, fraction_digits: Optional[int] = None, length: Optional[str] = None):
-        self.identifier         = identifier
-        self.yang_range         = yang_range
-        self.fraction_digits    = fraction_digits
-        self.length             = length
+        self.identifier = identifier
+        self.yang_range = yang_range
+        self.fraction_digits = fraction_digits
+        self.length = length
         assert not self.identifier.is_builtin()
 
     def __str__(self):
         return str(self.identifier)
 
     def __repr__(self):
         if self.yang_range:
@@ -233,36 +244,37 @@
         else:
             repr_str = f"({self.identifier!r})"
         return self.__class__.__name__ + repr_str
 
     def __eq__(self, other):
         if not YangTypeBase.__eq__(self, other):
             return False
-        return all((
-            self.identifier         == other.identifier,
-            self.yang_range         == other.yang_range,
-            self.fraction_digits    == other.fraction_digits,
-        ))
+        return (
+            self.identifier == other.identifier and
+            self.yang_range == other.yang_range and
+            self.fraction_digits == other.fraction_digits
+        )
 
     def __hash__(self):
         return hash((
             self.identifier,
             self.yang_range,
             self.fraction_digits,
         ))
 
-    def to_string(self, _val: Any) -> Tuple[str, str]:
+    def to_string(self, _val: Any) -> Tuple[str, Optional[str]]:
         raise make_exception(pysros_err_unresolved_type, type=self)
 
     def to_value(self, _val: str) -> Any:
         raise make_exception(pysros_err_unresolved_type, type=self)
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
         return False
 
+
 class YangUnion(YangTypeBase):
     def __init__(self, types: List["YangType"] = []):
         super().__init__()
 
         self._types: List["YangType"] = types.copy() if isinstance(types, list) else list(types)
         self.deduplicate()
 
@@ -289,234 +301,289 @@
             YangTypeBase.__eq__(self, other)
             and self._types == other._types
         )
 
     def __len__(self):
         return len(self._types)
 
-    def to_string(self, val: Any) -> Tuple[str, str]:
+    def to_string(self, val: Any) -> Tuple[str, Optional[str]]:
+        if val is None:
+            return '', None
         if isinstance(val, str):
             for t in self._types:
                 if isinstance(t, IdentityRef) and t._find_identity(val):
                     return t.to_string(val)
         if isinstance(val, bool):
             return "true" if val else "false", None
         return super().to_string(val)
 
     def to_value(self, val: Any) -> Any:
+        if val is None:
+            return ""
         return val
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
+        if not strict and value is None:
+            return True
         if isinstance(value, str):
             return True
-        return any(t.check_field_value(value, json) for t in self._types)
+        return any(t.check_field_value(value, json=json, strict=strict, is_convert=is_convert, metadata=metadata) for t in self._types)
 
     def json_name(self) -> str:
         return "union"
 
     def deduplicate(self):
         types = list(OrderedDict.fromkeys(self._types))
         if len(types) != len(self._types):
             self._types = types
 
+    def _find_identity(self, val: str, xml_nsmap=None):
+        for t in self._types:
+            if isinstance(t, IdentityRef):
+                identity = t._find_identity(val, xml_nsmap)
+                if identity is not None:
+                    return identity
+        return None
+
     def as_storage_type(self, obj, is_convert, idref_cb):
+        if obj is None:
+            return ""
         if isinstance(obj, str):
-            for t in self._types:
-                if isinstance(t, IdentityRef):
-                    identinty = t._find_identity(obj)
-                    if identinty is not None:
-                        if idref_cb:
-                            idref_cb(identinty)
-                        return identinty.module + ':' + identinty.name
+            identity = self._find_identity(obj)
+            if identity is not None:
+                if idref_cb:
+                    idref_cb(identity)
+                return identity.module + ':' + identity.name
 
         return super().as_storage_type(obj,  is_convert, idref_cb)
 
+
 class Enumeration(OrderedDict, YangTypeBase):
     def __str__(self):
         return f"enumeration[{'|'.join(map(str, self.keys()))}]"
 
     def __hash__(self):
         return hash(tuple(self))
 
     def add_enum(self, name: str):
-        val = 1+max(self.values()) if self else 0
+        val = 1 + max(self.values()) if self else 0
         self[name] = val
 
     def add_enums(self, *names: Iterable[str]):
         for name in names:
             self.add_enum(name)
 
     def set_last_enum_value(self, val: int):
         assert self
         last_used_key = next(reversed(self))
         self[last_used_key] = val
 
     def to_value(self, val: str) -> Any:
+        if val is None:
+            return ""
         return str(val)
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
+        if not strict and value is None:
+            return True
         return isinstance(value, str)
 
 
 class Bits(set, YangTypeBase):
     def __str__(self):
         return f"bits[{' '.join(sorted(self))}]"
 
     def __repr__(self):
         return f"Bits(({', '.join(map(repr, sorted(self)))}))"
 
     def __hash__(self):
         return hash(frozenset(self))
 
     def __eq__(self, other):
-        return YangTypeBase.__eq__(self, other) and frozenset(self) == frozenset(other)
+        return (
+            YangTypeBase.__eq__(self, other) and
+            frozenset(self) == frozenset(other)
+        )
 
     def is_valid_value(self, val: Any) -> bool:
         return isinstance(val, str)
 
     def to_value(self, val: str) -> Any:
+        if val is None:
+            return ""
         if self.is_valid_value(val):
             return val
         return super().to_value(val)
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
+        if not strict and value is None:
+            return True
         return self.is_valid_value(value)
 
+
 class LeafRef(YangTypeBase):
-    def __init__(self, path = None):
+    def __init__(self, path=None):
         if path is None or isinstance(path, ModelPath):
             self._path: Optional[ModelPath] = path
             return
         assert isinstance(path, tuple) and all(isinstance(p, Identifier) for p in path)
         self._path = ModelPath(path)
 
-
     def set_path(self, path: ModelPath):
         assert isinstance(path, ModelPath)
         self._path = path
 
     def __eq__(self, other):
         return YangTypeBase.__eq__(self, other) and self._path == other._path
 
     def __ne__(self, other):
-        return not(self == other)
+        return not (self == other)
 
     def __str__(self):
         return f"leafref({self._path!s})"
 
     def __repr__(self):
         return f"LeafRef({self._path.repr_path()})"
 
     def __hash__(self):
         return hash((self.__class__.__name__, self._path))
 
-    def to_string(self, _val: Any) -> Tuple[str, str]:
+    def to_string(self, _val: Any) -> Tuple[str, Optional[str]]:
         raise make_exception(pysros_err_unresolved_leafref, type=str(self))
 
     def to_value(self, _val: str) -> Any:
         raise make_exception(pysros_err_unresolved_leafref, type=str(self))
 
-    def check_field_value(self, value: Any, json=False) -> bool:
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
         return False
 
     @property
     def path(self):
         return self._path
 
+
 class Identity(NamedTuple):
     name: str
     module: str
     namespace: str
 
+
 class IdentityRef(YangTypeBase):
-    def __init__(self, bases = (), identities: Optional[Iterable[Identity]] = None):
+    def __init__(self, bases=(), identities: Optional[Iterable[Identity]] = None):
         self.bases:  List[Identifier] = list(bases)
-        self.values: Dict[str, Identity] = {} if identities is None else {i.name : i for i in identities}
+        self.values: Dict[str, Identity] = {} if identities is None else {i.name: i for i in identities}
 
     def add_base(self, base: Identifier):
         assert isinstance(base, Identifier)
         self.bases.append(base)
 
     def set_values(self, derived: Mapping[Identifier, Set[Identifier]], ns_map):
         assert not self.values
         self.values = {}
         for b in self.bases:
             if b not in derived:
                 continue
             for id in derived[b]:
                 if id.prefix not in ns_map:
-                    raise RuntimeError(f"Module {id.prefix} is not in map of known modules")
+                    raise RuntimeError(
+                        f"Module {id.prefix} is not in map of known modules"
+                    )
                 self.values[id.name] = Identity(id.name, id.prefix, ns_map[id.prefix])
 
     def __eq__(self, other):
         return (
             YangTypeBase.__eq__(self, other)
             and self.bases == other.bases
             and self.values == other.values
         )
 
     def __str__(self):
         return f"identityref[{', '.join(b.__str__() for b in self.bases)}]"
 
     def __repr__(self):
         # values has to be stable order
-        ordered_values = sorted(self.values.values(), key = lambda id: id.name)
+        ordered_values = sorted(self.values.values(), key=lambda id: id.name)
         return f"IdentityRef({self.bases!r}, {ordered_values!r})"
 
     def __hash__(self):
         return hash((self.__class__.__name__, *self.bases, frozenset(self.values)))
 
-    def to_string(self, val: str) -> Tuple[str, str]:
+    def to_string(self, val: str) -> Tuple[str, Optional[str]]:
+        if val == "":
+            return "", None
         identity = self._find_identity(val)
         if not identity:
-            raise make_exception(pysros_err_invalid_value_for_type, type=self, value=val)
-        return identity.module + ':' + identity.name, identity.module
+            raise make_exception(
+                pysros_err_invalid_value_for_type, type=self, value=val
+            )
+        return (
+            identity.module + ':' + identity.name,
+            identity.module
+        )
 
-    def _find_identity(self, val: str):
-        prefix = None
+    def _find_identity(self, val: str, xml_nsmap=None):
         if ':' in val:
-            mod,value = val.split(':', 1)
+            mod, value = val.split(':', 1)
+            if not mod:
+                return None
             result = self.values.get(value, None)
-            return result if result is not None and result.module == mod else None
+            if result is None:
+                return None
+            if xml_nsmap is None:
+                return result if result.module == mod else None
+            else:
+                return result if result.namespace == xml_nsmap.get(mod, None) else None
         else:
             return self.values.get(val, None)
 
     def to_value(self, _val: str) -> Any:
+        if _val == "":
+            return None
         return _val
 
     def as_storage_type(self, obj, is_convert, idref_cb):
+        if obj is None:
+            return ""
         identinty = self._find_identity(obj)
         if idref_cb:
             idref_cb(identinty)
         return identinty.module + ':' + identinty.name
 
-    def check_field_value(self, value: Any, json=False) -> bool:
-        return isinstance(value, str) and self._find_identity(value) is not None
+    def check_field_value(self, value: Any, json=False, strict=False, is_convert=False, metadata=None) -> bool:
+        if not strict and value is None:
+            return True
+        return (
+            isinstance(value, str) and
+            self._find_identity(value) is not None
+        )
+
 
 YangType = Union[
     PrimitiveType,
     UnresolvedIdentifier,
     Enumeration,
     Bits,
     YangUnion,
     LeafRef,
     IdentityRef]
 
 
 _KNOWN_TYPES = {
-        "leafref":     LeafRef,
-        "bits":        Bits,
-        "enumeration": Enumeration,
-        "union":       YangUnion,
-        "identityref": IdentityRef,
-    }
+    "leafref":     LeafRef,
+    "bits":        Bits,
+    "enumeration": Enumeration,
+    "union":       YangUnion,
+    "identityref": IdentityRef,
+}
+
 
 def should_be_buildin(name):
     return name in _KNOWN_TYPES or name in YANG_PRIMITIVE_TYPES
 
+
 def type_from_name(identifier: Identifier):
     if identifier.is_builtin():
         t = _KNOWN_TYPES.get(identifier.name)
         if t is not None:
             return t()
         return PrimitiveType(identifier.name)
     return UnresolvedIdentifier(identifier)
```

### Comparing `pysros-23.7.2/pysros.egg-info/PKG-INFO` & `pysros-24.3.1/pysros.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: pysros
-Version: 23.7.2
+Version: 24.3.1
 Summary: Python for the Nokia Service Router Operating Systems (pySROS)
 Home-page: https://www.nokia.com
 Author: Nokia
 Author-email: 
-License: Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.
+License: Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.
 Project-URL: Documentation, https://network.developer.nokia.com/static/sr/learn/pysros/latest/
 Project-URL: Source, https://github.com/nokia/pysros
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: ncclient~=0.6.12
+Requires-Dist: lxml~=4.9.2
 
 # Python 3 for Nokia Service Router Operating System (pySROS) #
 
 ## Overview ##
 
 The pySROS libraries provide a model-driven management interface for
 Python developers to integrate with supported Nokia routers
```

### Comparing `pysros-23.7.2/setup.py` & `pysros-24.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pysros',
-    version='23.7.2',
+    version='24.3.1',
     packages=['pysros'],
     url='https://www.nokia.com',
-    license='Copyright 2021-2023 Nokia.  License available in the LICENSE.md file.',
+    license='Copyright 2021-2024 Nokia.  License available in the LICENSE.md file.',
     author='Nokia',
     author_email='',
     description='Python for the Nokia Service Router Operating Systems (pySROS)',
     project_urls={
         "Documentation": "https://network.developer.nokia.com/static/sr/learn/pysros/latest/",
         "Source": "https://github.com/nokia/pysros",
     },
```

