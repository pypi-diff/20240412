# Comparing `tmp/omu-0.2.3.tar.gz` & `tmp/omu-0.2.4.tar.gz`

## Comparing `omu-0.2.3.tar` & `omu-0.2.4.tar`

### file list

```diff
@@ -1,60 +1,65 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.3/.gitattributes
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.3/.prettierrc
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.3/.python-version
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.3/run_client.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/__init__.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/app.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/event_emitter.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/helper.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/identifier.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/model.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/plugin.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/serializer.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/client/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/client/client.py
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/client/omuclient.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/__init__.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/extension.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/extension_registry.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/asset/__init__.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/asset/asset_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/dashboard/dashboard.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/endpoint/endpoint.py
--rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/message/__init__.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/message/message.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/message/message_extension.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/permission/__init__.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/permission/permission.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/permission/permission_extension.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/registry/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/registry/registry.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/registry/registry_extension.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/server/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/server/server_extension.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/table/__init__.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/table/table.py
--rw-r--r--   0        0        0    15093 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/extension/table/table_extension.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/interface/__init__.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/interface/keyable.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/interface/named.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/address.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/bytebuffer.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/connection.py
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/network.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/packet_mapper.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/websocket_connection.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/packet/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/packet/packet.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.3/src/omu/network/packet/packet_types.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.3/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 omu-0.2.4/.gitattributes
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omu-0.2.4/.prettierrc
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omu-0.2.4/.python-version
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 omu-0.2.4/run_client.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/__init__.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/app.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/event_emitter.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/helper.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/identifier.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/model.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/plugin.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/serializer.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/__init__.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/client.py
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/client/omuclient.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/__init__.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/extension.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/extension_registry.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/asset/__init__.py
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/dashboard.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/endpoint.py
+-rw-r--r--   0        0        0     6277 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/i18n/__init__.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/i18n/i18n_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/__init__.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/message.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/message/message_extension.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/__init__.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/permission.py
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/registry.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/server/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/server/server_extension.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/__init__.py
+-rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/table.py
+-rw-r--r--   0        0        0    15097 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/extension/table/table_extension.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/__init__.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/keyable.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/interface/named.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/__init__.py
+-rw-r--r--   0        0        0    33905 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/locale.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/localization/localization.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/address.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/bytebuffer.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/connection.py
+-rw-r--r--   0        0        0     5470 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/network.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet_mapper.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/websocket_connection.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/packet.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 omu-0.2.4/src/omu/network/packet/packet_types.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 omu-0.2.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omu-0.2.4/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omu-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 omu-0.2.4/PKG-INFO
```

### Comparing `omu-0.2.3/run_client.py` & `omu-0.2.4/run_client.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/event_emitter.py` & `omu-0.2.4/src/omu/event_emitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,44 +10,47 @@
     def __init__(
         self,
         on_subscribe: Callable[[], None] | Coro[[], None] | None = None,
         on_empty: Callable[[], None] | Coro[[], None] | None = None,
     ) -> None:
         self.on_subscribe = on_subscribe
         self.on_empty = on_empty
-        self._listeners: List[Coro[P, None]] = []
+        self._listeners: List[Callable[P, None] | Coro[P, None]] = []
 
     @property
     def empty(self) -> bool:
         return len(self._listeners) == 0
 
-    def subscribe(self, listener: Coro[P, None]) -> None:
+    def subscribe(self, listener: Callable[P, None] | Coro[P, None]) -> None:
         if listener in self._listeners:
             raise ValueError("Listener already subscribed")
         if self.on_subscribe and len(self._listeners) == 0:
             coroutine = self.on_subscribe()
             if asyncio.iscoroutine(coroutine):
                 asyncio.create_task(coroutine)
         self._listeners.append(listener)
 
-    def unsubscribe(self, listener: Coro[P, None]) -> None:
+    def unsubscribe(self, listener: Callable[P, None] | Coro[P, None]) -> None:
         if listener not in self._listeners:
             return
         self._listeners.remove(listener)
         if self.on_empty and len(self._listeners) == 0:
             coroutine = self.on_empty()
             if asyncio.iscoroutine(coroutine):
                 asyncio.create_task(coroutine)
 
-    def __iadd__(self, listener: Coro[P, None]) -> Self:
+    def __iadd__(self, listener: Callable[P, None] | Coro[P, None]) -> Self:
         self.subscribe(listener)
         return self
 
-    def __isub__(self, listener: Coro[P, None]) -> Self:
+    def __isub__(self, listener: Callable[P, None] | Coro[P, None]) -> Self:
         self.unsubscribe(listener)
         return self
 
     async def emit(self, *args: P.args, **kwargs: P.kwargs) -> None:
-        for listener in self._listeners:
-            await listener(*args, **kwargs)
+        for listener in tuple(self._listeners):
+            if asyncio.iscoroutinefunction(listener):
+                await listener(*args, **kwargs)
+            else:
+                listener(*args, **kwargs)
 
     __call__ = emit
```

### Comparing `omu-0.2.3/src/omu/helper.py` & `omu-0.2.4/src/omu/helper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/identifier.py` & `omu-0.2.4/src/omu/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def to_path(self) -> Path:
         namespace = (
             f"{sanitize_filename(self.namespace)}-{generate_md5_hash(self.namespace)}"
         )
         return Path(namespace, *self.path)
 
-    def is_subpath_of(self, base: Identifier) -> bool:
+    def is_subpart_of(self, base: Identifier) -> bool:
         return (
             self.namespace == base.namespace
             and self.path[: len(base.path)] == base.path
         )
 
     def join(self, *path: str) -> Identifier:
         return Identifier(self.namespace, *self.path, *path)
```

### Comparing `omu-0.2.3/src/omu/serializer.py` & `omu-0.2.4/src/omu/serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 import abc
 import json
 from typing import Callable, Mapping, Protocol
 
 
+class SerializeError(Exception):
+    pass
+
+
 class Serializable[T, D](Protocol):
     @abc.abstractmethod
     def serialize(self, item: T) -> D: ...
 
     @abc.abstractmethod
     def deserialize(self, item: D) -> T: ...
 
@@ -43,18 +47,21 @@
     def model[_T, _D](cls, model: type[JsonSerializable[_T, _D]]) -> Serializer[_T, _D]:
         return ModelSerializer(model)
 
     @classmethod
     def json(cls) -> Serializer[T, bytes]:
         return JsonSerializer()
 
-    def array(self) -> Serializer[list[T], list[D]]:
+    def to_json(self) -> Serializer[T, bytes]:
+        return self.pipe(JsonSerializer())
+
+    def to_array(self) -> Serializer[list[T], list[D]]:
         return ArraySerializer(self)
 
-    def map(self) -> Serializer[Mapping[str, T], Mapping[str, D]]:
+    def to_map(self) -> Serializer[Mapping[str, T], Mapping[str, D]]:
         return MapSerializer(self)
 
     def pipe[E](self, other: Serializable[D, E]) -> Serializer[T, E]:
         return PipeSerializer(self, other)
 
 
 class NoopSerializer[T](Serializer[T, T]):
@@ -75,18 +82,28 @@
     def __repr__(self) -> str:
         return f"ModelSerializer({self._model})"
 
 
 class JsonSerializer[T](Serializer[T, bytes]):
     def __init__(self):
         super().__init__(
-            lambda item: json.dumps(item).encode("utf-8"),
-            lambda item: json.loads(item.decode("utf-8")),
+            self._serialize,
+            self._deserialize,
         )
 
+    def _serialize(self, item: T) -> bytes:
+        return json.dumps(item).encode("utf-8")
+
+    def _deserialize(self, item: bytes) -> T:
+        decoded = item.decode("utf-8")
+        try:
+            return json.loads(decoded)
+        except json.JSONDecodeError as e:
+            raise SerializeError(f"Failed to deserialize JSON: {decoded}") from e
+
     def __repr__(self) -> str:
         return "JsonSerializer()"
 
 
 class ArraySerializer[T, D](Serializer[list[T], list[D]]):
     def __init__(self, serializer: Serializable[T, D]):
         self._serializer = serializer
```

### Comparing `omu-0.2.3/src/omu/client/client.py` & `omu-0.2.4/src/omu/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
     from omu.app import App
     from omu.extension import ExtensionRegistry
     from omu.extension.dashboard import DashboardExtension
     from omu.extension.endpoint import EndpointExtension
+    from omu.extension.i18n import I18nExtension
     from omu.extension.message import MessageExtension
     from omu.extension.permission import PermissionExtension
     from omu.extension.registry import RegistryExtension
     from omu.extension.server import ServerExtension
     from omu.extension.table import TableExtension
     from omu.network import Network
     from omu.network.packet import PacketType
@@ -71,14 +72,18 @@
 
     @property
     @abc.abstractmethod
     def dashboard(self) -> DashboardExtension: ...
 
     @property
     @abc.abstractmethod
+    def i18n(self) -> I18nExtension: ...
+
+    @property
+    @abc.abstractmethod
     def running(self) -> bool: ...
 
     @abc.abstractmethod
     def run(self) -> None: ...
 
     @abc.abstractmethod
     async def start(self) -> None: ...
```

### Comparing `omu-0.2.3/src/omu/client/omuclient.py` & `omu-0.2.4/src/omu/client/omuclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     DASHBOARD_EXTENSION_TYPE,
     DashboardExtension,
 )
 from omu.extension.endpoint import (
     ENDPOINT_EXTENSION_TYPE,
     EndpointExtension,
 )
+from omu.extension.i18n import (
+    I18N_EXTENSION_TYPE,
+    I18nExtension,
+)
 from omu.extension.message import (
     MESSAGE_EXTENSION_TYPE,
     MessageExtension,
 )
 from omu.extension.permission import (
     PERMISSION_EXTENSION_TYPE,
     PermissionExtension,
@@ -70,14 +74,15 @@
         self._tables = self.extensions.register(TABLE_EXTENSION_TYPE)
         self._registry = self.extensions.register(REGISTRY_EXTENSION_TYPE)
         self._message = self.extensions.register(MESSAGE_EXTENSION_TYPE)
         self._assets = self.extensions.register(ASSET_EXTENSION_TYPE)
         self._server = self.extensions.register(SERVER_EXTENSION_TYPE)
         self._permissions = self.extensions.register(PERMISSION_EXTENSION_TYPE)
         self._dashboard = self.extensions.register(DASHBOARD_EXTENSION_TYPE)
+        self._i18n = self.extensions.register(I18N_EXTENSION_TYPE)
 
         self._loop.create_task(self._listeners.initialized.emit())
 
     @property
     def app(self) -> App:
         return self._app
 
@@ -122,14 +127,18 @@
         return self._permissions
 
     @property
     def dashboard(self) -> DashboardExtension:
         return self._dashboard
 
     @property
+    def i18n(self) -> I18nExtension:
+        return self._i18n
+
+    @property
     def running(self) -> bool:
         return self._running
 
     async def send[T](self, type: PacketType[T], data: T) -> None:
         await self._network.send(Packet(type, data))
 
     def run(self, *, token: str | None = None, reconnect: bool = True) -> None:
```

### Comparing `omu-0.2.3/src/omu/extension/extension.py` & `omu-0.2.4/src/omu/extension/extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/extension_registry.py` & `omu-0.2.4/src/omu/extension/extension_registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/asset/asset_extension.py` & `omu-0.2.4/src/omu/extension/asset/asset_extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,20 +37,20 @@
         return files
 
 
 ASSET_UPLOAD_ENDPOINT = EndpointType[Files, List[Identifier]].create_serialized(
     ASSET_EXTENSION_TYPE,
     "upload",
     request_serializer=FILES_SERIALIZER,
-    response_serializer=Serializer.model(Identifier).array().pipe(Serializer.json()),
+    response_serializer=Serializer.model(Identifier).to_array().to_json(),
 )
 ASSET_DOWNLOAD_ENDPOINT = EndpointType[List[Identifier], Files].create_serialized(
     ASSET_EXTENSION_TYPE,
     "download",
-    request_serializer=Serializer.model(Identifier).array().pipe(Serializer.json()),
+    request_serializer=Serializer.model(Identifier).to_array().to_json(),
     response_serializer=FILES_SERIALIZER,
 )
 
 
 class AssetExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
```

### Comparing `omu-0.2.3/src/omu/extension/dashboard/dashboard.py` & `omu-0.2.4/src/omu/extension/dashboard/dashboard.py`

 * *Files 24% similar despite different names*

```diff
@@ -30,7 +30,13 @@
 
     def to_json(self) -> PermissionRequestJson:
         return {
             "request_id": self.request_id,
             "app": self.app.to_json(),
             "permissions": [p.to_json() for p in self.permissions],
         }
+
+
+class DashboardOpenAppResponse(TypedDict):
+    success: bool
+    already_open: bool
+    dashboard_not_connected: bool
```

### Comparing `omu-0.2.3/src/omu/extension/endpoint/endpoint.py` & `omu-0.2.4/src/omu/extension/endpoint/endpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         request_serializer: Serializable[Req, Any] | None = None,
         response_serializer: Serializable[Res, Any] | None = None,
     ):
         return cls(
             identifier=identifier / name,
             request_serializer=Serializer.of(
                 request_serializer or Serializer.noop()
-            ).pipe(Serializer.json()),
+            ).to_json(),
             response_serializer=Serializer.of(
                 response_serializer or Serializer.noop()
-            ).pipe(Serializer.json()),
+            ).to_json(),
         )
 
     @classmethod
     def create_serialized(
         cls,
         identifier: Identifier,
         name: str,
```

### Comparing `omu-0.2.3/src/omu/extension/endpoint/endpoint_extension.py` & `omu-0.2.4/src/omu/extension/endpoint/endpoint_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,41 +77,41 @@
     ) -> None:
         if type.identifier in self.endpoints:
             raise Exception(f"Endpoint for key {type.identifier} already registered")
         self.endpoints[type.identifier] = (type, func)
 
     def bind[T, R](
         self,
-        func: Coro[[T], R] | None = None,
+        handler: Coro[[T], R] | None = None,
         endpoint_type: EndpointType[T, R] | None = None,
     ):
         if endpoint_type is None:
             raise Exception("Endpoint type must be provided")
 
         def decorator(func: Coro[[T], R]) -> Coro[[T], R]:
             self.register(endpoint_type, func)
             return func
 
-        if func:
-            decorator(func)
+        if handler:
+            decorator(handler)
         return decorator
 
     def listen(
-        self, func: Coro | None = None, name: str | None = None
+        self, handler: Coro | None = None, name: str | None = None
     ) -> Callable[[Coro], Coro]:
         def decorator(func: Coro) -> Coro:
             type = EndpointType.create_json(
                 self.client.app.identifier,
                 name or func.__name__,
             )
             self.register(type, func)
             return func
 
-        if func:
-            decorator(func)
+        if handler:
+            decorator(handler)
         return decorator
 
     async def call[Req, Res](self, endpoint: EndpointType[Req, Res], data: Req) -> Res:
         try:
             self.call_id += 1
             future = Future[bytes]()
             self.response_promises[self.call_id] = future
@@ -160,15 +160,15 @@
             data = reader.read_byte_array()
         return EndpointDataPacket(type=type, id=id, data=data)
 
 
 ENDPOINT_REGISTER_PACKET = PacketType[List[Identifier]].create_json(
     ENDPOINT_EXTENSION_TYPE,
     "register",
-    Serializer.model(Identifier).array(),
+    Serializer.model(Identifier).to_array(),
 )
 ENDPOINT_CALL_PACKET = PacketType[EndpointDataPacket].create_serialized(
     ENDPOINT_EXTENSION_TYPE,
     "call",
     ENDPOINT_DATA_SERIALIZER,
 )
 ENDPOINT_RECEIVE_PACKET = PacketType[EndpointDataPacket].create_serialized(
```

### Comparing `omu-0.2.3/src/omu/extension/message/message.py` & `omu-0.2.4/src/omu/extension/message/message.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/message/message_extension.py` & `omu-0.2.4/src/omu/extension/message/message_extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,51 +5,56 @@
 
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.helper import Coro
 from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import PacketType
+from omu.serializer import Serializer
 
 from .message import Message, MessageType
 
 MESSAGE_EXTENSION_TYPE = ExtensionType(
     "message",
     lambda client: MessageExtension(client),
     lambda: [],
 )
 
 
 @dataclass
 class MessagePacket:
-    key: str
+    id: Identifier
     body: bytes
 
 
-class MESSAGE_SERIALIZER:
+class MessageSerializer:
     @classmethod
     def serialize(cls, item: MessagePacket) -> bytes:
         writer = ByteWriter()
-        writer.write_string(item.key)
+        writer.write_string(item.id.key())
         writer.write_byte_array(item.body)
         return writer.finish()
 
     @classmethod
     def deserialize(cls, item: bytes) -> MessagePacket:
         with ByteReader(item) as reader:
-            key = reader.read_string()
+            key = Identifier.from_key(reader.read_string())
             body = reader.read_byte_array()
-        return MessagePacket(key=key, body=body)
+        return MessagePacket(id=key, body=body)
 
 
-MESSAGE_LISTEN_PACKET = PacketType[str].create_json(MESSAGE_EXTENSION_TYPE, "listen")
+MESSAGE_LISTEN_PACKET = PacketType[Identifier].create_json(
+    MESSAGE_EXTENSION_TYPE,
+    "listen",
+    serializer=Serializer.model(Identifier),
+)
 MESSAGE_BROADCAST_PACKET = PacketType[MessagePacket].create_serialized(
     MESSAGE_EXTENSION_TYPE,
     "broadcast",
-    MESSAGE_SERIALIZER(),
+    MessageSerializer,
 )
 
 
 class MessageExtension(Extension):
     def __init__(self, client: Client):
         self.client = client
         self._message_identifiers: List[Identifier] = []
@@ -69,35 +74,38 @@
     def get[T](self, message_type: MessageType[T]) -> Message[T]:
         return MessageImpl(self.client, message_type)
 
 
 class MessageImpl[T](Message):
     def __init__(self, client: Client, message_type: MessageType[T]):
         self.client = client
-        self.key = message_type.identifier.key()
+        self.identifier = message_type.identifier
         self.serializer = message_type.serializer
         self.listeners = []
         self.listening = False
         client.network.add_packet_handler(MESSAGE_BROADCAST_PACKET, self._on_broadcast)
 
     async def broadcast(self, body: T) -> None:
         data = self.serializer.serialize(body)
         await self.client.send(
             MESSAGE_BROADCAST_PACKET,
-            MessagePacket(key=self.key, body=data),
+            MessagePacket(id=self.identifier, body=data),
         )
 
     def listen(self, listener: Coro[[T], None]) -> Callable[[], None]:
-        self.listeners.append(listener)
         if not self.listening:
-            self.client.network.add_task(self._listen)
+            self.client.network.add_task(self._send_listen)
             self.listening = True
+
+        self.listeners.append(listener)
         return lambda: self.listeners.remove(listener)
 
-    async def _listen(self) -> None:
-        await self.client.send(MESSAGE_LISTEN_PACKET, self.key)
+    async def _send_listen(self) -> None:
+        await self.client.send(MESSAGE_LISTEN_PACKET, self.identifier)
 
     async def _on_broadcast(self, data: MessagePacket) -> None:
-        if data.key != self.key:
+        if data.id != self.identifier:
             return
+
+        body = self.serializer.deserialize(data.body)
         for listener in self.listeners:
-            await listener(data.body)
+            await listener(body)
```

### Comparing `omu-0.2.3/src/omu/extension/permission/permission.py` & `omu-0.2.4/src/omu/extension/permission/permission.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/permission/permission_extension.py` & `omu-0.2.4/src/omu/extension/permission/permission_extension.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,48 +30,49 @@
             PERMISSION_GRANT_PACKET,
             self.handle_grant,
         )
         client.network.listeners.connected += self.on_connected
 
     def register(self, permission: PermissionType):
         base_identifier = self.client.app.identifier
-        if not permission.identifier.is_subpath_of(base_identifier):
+        if not permission.identifier.is_subpart_of(base_identifier):
             raise ValueError(
-                f"Permission identifier {permission.identifier} is not a subpath of app identifier {base_identifier}"
+                f"Permission identifier {permission.identifier} is not a subpart of app identifier {base_identifier}"
             )
         self.registered_permissions[permission.identifier] = permission
 
     def require(self, permission: PermissionType):
         self.required_permissions[permission.identifier] = permission
 
     def has(self, permission_identifier: Identifier):
         return permission_identifier in self.permissions
 
     async def on_connected(self):
         await self.client.send(
             PERMISSION_REGISTER_PACKET,
             [*self.registered_permissions.values()],
         )
-        await self.client.endpoints.call(
-            PERMISSION_REQUEST_ENDPOINT,
-            [*self.required_permissions.keys()],
-        )
+        if len(self.required_permissions) > 0:
+            await self.client.endpoints.call(
+                PERMISSION_REQUEST_ENDPOINT,
+                [*self.required_permissions.keys()],
+            )
 
     async def handle_grant(self, permissions: List[PermissionType]):
         self.permissions = permissions
 
 
 PERMISSION_REGISTER_PACKET = PacketType.create_json(
     PERMISSION_EXTENSION_TYPE,
     "register",
-    Serializer.model(PermissionType).array(),
+    Serializer.model(PermissionType).to_array(),
 )
 PERMISSION_REQUEST_ENDPOINT = EndpointType[List[Identifier], None].create_json(
     PERMISSION_EXTENSION_TYPE,
     "request",
-    request_serializer=Serializer.model(Identifier).array(),
+    request_serializer=Serializer.model(Identifier).to_array(),
 )
 PERMISSION_GRANT_PACKET = PacketType.create_json(
     PERMISSION_EXTENSION_TYPE,
     "grant",
-    Serializer.model(PermissionType).array(),
+    Serializer.model(PermissionType).to_array(),
 )
```

### Comparing `omu-0.2.3/src/omu/extension/plugin/plugin_extension.py` & `omu-0.2.4/src/omu/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/registry/registry.py` & `omu-0.2.4/src/omu/extension/registry/registry.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/extension/registry/registry_extension.py` & `omu-0.2.4/src/omu/extension/registry/registry_extension.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,60 +6,64 @@
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
 from omu.helper import Coro
 from omu.identifier import Identifier
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import PacketType
-from omu.serializer import Serializable, Serializer
+from omu.serializer import Serializable, SerializeError, Serializer
 
 from .registry import Registry, RegistryType
 
 REGISTRY_EXTENSION_TYPE = ExtensionType(
     "registry",
     lambda client: RegistryExtension(client),
     lambda: [],
 )
 
 
 @dataclass(frozen=True)
 class RegistryPacket:
-    key: str
-    existing: bool
-    value: bytes
+    identifier: Identifier
+    value: bytes | None
 
 
 class REGISTRY_DATA_SERIALIZER:
     @classmethod
     def serialize(cls, item: RegistryPacket) -> bytes:
         writer = ByteWriter()
-        writer.write_string(item.key)
-        writer.write_boolean(item.existing)
-        writer.write_byte_array(item.value)
+        writer.write_string(item.identifier.key())
+        writer.write_boolean(item.value is not None)
+        if item.value is not None:
+            writer.write_byte_array(item.value)
         return writer.finish()
 
     @classmethod
     def deserialize(cls, item: bytes) -> RegistryPacket:
         with ByteReader(item) as reader:
-            key = reader.read_string()
+            key = Identifier.from_key(reader.read_string())
             existing = reader.read_boolean()
-            value = reader.read_byte_array()
-            return RegistryPacket(key, existing, value)
+            value = reader.read_byte_array() if existing else None
+        return RegistryPacket(key, value)
 
 
 REGISTRY_UPDATE_PACKET = PacketType[RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "update",
     serializer=REGISTRY_DATA_SERIALIZER,
 )
-REGISTRY_LISTEN_PACKET = PacketType[str].create_json(REGISTRY_EXTENSION_TYPE, "listen")
-REGISTRY_GET_ENDPOINT = EndpointType[str, RegistryPacket].create_serialized(
+REGISTRY_LISTEN_PACKET = PacketType[Identifier].create_json(
+    REGISTRY_EXTENSION_TYPE,
+    "listen",
+    Serializer.model(Identifier),
+)
+REGISTRY_GET_ENDPOINT = EndpointType[Identifier, RegistryPacket].create_serialized(
     REGISTRY_EXTENSION_TYPE,
     "get",
-    request_serializer=Serializer.json(),
+    request_serializer=Serializer.model(Identifier).to_json(),
     response_serializer=REGISTRY_DATA_SERIALIZER,
 )
 
 
 class RegistryExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
@@ -86,49 +90,59 @@
         default_value: T,
         serializer: Serializable[T, bytes],
     ) -> None:
         self.client = client
         self.identifier = identifier
         self.default_value = default_value
         self.serializer = serializer
-        self.key = identifier.key()
         self.listeners: List[Coro[[T], None]] = []
         self.listening = False
         client.network.add_packet_handler(REGISTRY_UPDATE_PACKET, self._on_update)
 
     async def get(self) -> T:
-        result = await self.client.endpoints.call(REGISTRY_GET_ENDPOINT, self.key)
-        if not result.existing:
+        result = await self.client.endpoints.call(
+            REGISTRY_GET_ENDPOINT, self.identifier
+        )
+        if result.value is None:
             return self.default_value
-        return self.serializer.deserialize(result.value)
+        try:
+            return self.serializer.deserialize(result.value)
+        except SerializeError as e:
+            raise SerializeError(
+                f"Failed to deserialize registry value for identifier {self.identifier}"
+            ) from e
 
     async def update(self, handler: Coro[[T], T]) -> None:
         value = await self.get()
         new_value = await handler(value)
         await self.client.send(
             REGISTRY_UPDATE_PACKET,
             RegistryPacket(
-                self.key,
-                True,
-                self.serializer.serialize(new_value),
+                identifier=self.identifier,
+                value=self.serializer.serialize(new_value),
             ),
         )
 
     def listen(self, handler: Coro[[T], None]) -> Callable[[], None]:
         if not self.listening:
             self.client.network.add_task(
-                lambda: self.client.send(REGISTRY_LISTEN_PACKET, self.key)
+                lambda: self.client.send(REGISTRY_LISTEN_PACKET, self.identifier)
             )
             self.listening = True
 
         self.listeners.append(handler)
         return lambda: self.listeners.remove(handler)
 
     async def _on_update(self, event: RegistryPacket) -> None:
-        if event.key != self.key:
+        if event.identifier != self.identifier:
             return
-        if event.existing:
-            value = self.serializer.deserialize(event.value)
+        if event.value is not None:
+            try:
+                value = self.serializer.deserialize(event.value)
+            except SerializeError as e:
+                raise SerializeError(
+                    f"Failed to deserialize registry value for identifier {self.identifier}"
+                ) from e
         else:
             value = self.default_value
         for listener in self.listeners:
             await listener(value)
```

### Comparing `omu-0.2.3/src/omu/extension/server/server_extension.py` & `omu-0.2.4/src/omu/extension/server/server_extension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from omu.app import App
 from omu.client import Client
 from omu.extension import Extension, ExtensionType
 from omu.extension.endpoint import EndpointType
+from omu.extension.registry import RegistryType
 from omu.extension.table import TABLE_EXTENSION_TYPE, TableType
 
 SERVER_EXTENSION_TYPE = ExtensionType(
     "server", lambda client: ServerExtension(client), lambda: []
 )
 
 APPS_TABLE_TYPE = TableType.create_model(
@@ -13,14 +14,19 @@
     "apps",
     App,
 )
 SHUTDOWN_ENDPOINT_TYPE = EndpointType[bool, bool].create_json(
     SERVER_EXTENSION_TYPE,
     "shutdown",
 )
+VERSION_REGISTRY_TYPE = RegistryType[str | None].create_json(
+    SERVER_EXTENSION_TYPE,
+    "version",
+    default_value=None,
+)
 
 
 class ServerExtension(Extension):
     def __init__(self, client: Client) -> None:
         self.client = client
         tables = client.extensions.get(TABLE_EXTENSION_TYPE)
         self.apps = tables.get(APPS_TABLE_TYPE)
```

### Comparing `omu-0.2.3/src/omu/extension/table/table.py` & `omu-0.2.4/src/omu/extension/table/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,19 +130,19 @@
     key_func: Callable[[T], str]
 
     @classmethod
     def create_model[_T: Keyable, _D](
         cls,
         identifier: Identifier,
         name: str,
-        model: type[ModelEntry[_T, _D]],
+        model_type: type[ModelEntry[_T, _D]],
     ) -> TableType[_T]:
         return TableType(
             identifier=identifier / name,
-            serializer=Serializer.model(model).pipe(Serializer.json()),
+            serializer=Serializer.model(model_type).to_json(),
             key_func=lambda item: item.key(),
         )
 
     @classmethod
     def create_serialized[_T: Keyable](
         cls,
         identifier: Identifier,
```

### Comparing `omu-0.2.3/src/omu/extension/table/table_extension.py` & `omu-0.2.4/src/omu/extension/table/table_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,22 +63,22 @@
 
     def get[T](self, type: TableType[T]) -> Table[T]:
         if self.has(type.identifier):
             return self._tables[type.identifier]
         return self.create(type.identifier, type.serializer, type.key_func)
 
     def model[T: Keyable, D](
-        self, identifier: Identifier, name: str, type: type[ModelType[T, D]]
+        self, identifier: Identifier, name: str, model_type: type[ModelType[T, D]]
     ) -> Table[T]:
         identifier = identifier / name
         if self.has(identifier):
             return self._tables[identifier]
         return self.create(
             identifier,
-            Serializer.model(type).pipe(Serializer.json()),
+            Serializer.model(model_type).to_json(),
             lambda item: item.key(),
         )
 
     def has(self, identifier: Identifier) -> bool:
         return identifier in self._tables
 
 
@@ -88,15 +88,15 @@
 
 
 class TableEventData(TypedDict):
     type: str
 
 
 class TableItemsData(TableEventData):
-    items: Dict[str, bytes]
+    items: Mapping[str, bytes]
 
 
 class TableKeysData(TableEventData):
     keys: Sequence[str]
 
 
 class TableProxyData(TableItemsData):
@@ -444,15 +444,15 @@
         for key, item_bytes in items.items():
             item = self._serializer.deserialize(item_bytes)
             if item is None:
                 raise ValueError(f"Failed to deserialize item with key: {key}")
             parsed_items[key] = item
         return parsed_items
 
-    def _serialize_items(self, items: Iterable[T]) -> Dict[str, bytes]:
+    def _serialize_items(self, items: Iterable[T]) -> Mapping[str, bytes]:
         serialized_items: Mapping[str, bytes] = {}
         for item in items:
             key = self._key_function(item)
             serialized_items[key] = self._serializer.serialize(item)
         return serialized_items
 
     def set_cache_size(self, size: int | None) -> None:
```

### Comparing `omu-0.2.3/src/omu/network/bytebuffer.py` & `omu-0.2.4/src/omu/network/bytebuffer.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/network/connection.py` & `omu-0.2.4/src/omu/network/connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/network/network.py` & `omu-0.2.4/src/omu/network/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,16 @@
         self,
         packet_type: PacketType[T],
         packet_handler: Coro[[T], None] | None = None,
     ):
         if not self._packet_handlers.get(packet_type.identifier):
             raise ValueError(f"Event type {packet_type.identifier} not registered")
 
-        def decorator(packet_handler: Coro[[T], None]) -> None:
-            self._packet_handlers[packet_type.identifier].listeners.subscribe(
-                packet_handler
-            )
+        def decorator(func: Coro[[T], None]) -> None:
+            self._packet_handlers[packet_type.identifier].listeners.subscribe(func)
 
         if packet_handler:
             decorator(packet_handler)
         return decorator
 
     @property
     def connected(self) -> bool:
@@ -102,19 +100,20 @@
             )
         )
         self._closed_event.clear()
         self._client.loop.create_task(self._listen())
 
         await self._listeners.status.emit("connected")
         await self._listeners.connected.emit()
-        self._client.loop.create_task(self._dispatch_tasks())
+        await self._dispatch_tasks()
 
         await self._closed_event.wait()
 
         if reconnect:
+            await asyncio.sleep(1)
             await self.connect(token=self._token, reconnect=True)
 
     async def disconnect(self) -> None:
         if self._connection.closed:
             return
         self._connected = False
         await self._connection.close()
@@ -158,11 +157,11 @@
 
 
 type NetworkStatus = Literal["connecting", "connected", "disconnected"]
 
 
 class NetworkListeners:
     def __init__(self) -> None:
-        self.connected = EventEmitter()
-        self.disconnected = EventEmitter()
+        self.connected = EventEmitter[[]]()
+        self.disconnected = EventEmitter[[]]()
         self.packet = EventEmitter[Packet]()
         self.status = EventEmitter[NetworkStatus]()
```

### Comparing `omu-0.2.3/src/omu/network/packet_mapper.py` & `omu-0.2.4/src/omu/network/packet_mapper.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/network/websocket_connection.py` & `omu-0.2.4/src/omu/network/websocket_connection.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/network/packet/packet.py` & `omu-0.2.4/src/omu/network/packet/packet.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/src/omu/network/packet/packet_types.py` & `omu-0.2.4/src/omu/network/packet/packet_types.py`

 * *Files identical despite different names*

### Comparing `omu-0.2.3/pyproject.toml` & `omu-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omu"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = ["loguru>=0.7.2"]
 readme = "README.md"
 requires-python = ">= 3.12"
```

