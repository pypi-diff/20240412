# Comparing `tmp/avilla_qqapi-1.0.0a28.tar.gz` & `tmp/avilla_qqapi-1.0.0a29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avilla_qqapi-1.0.0a28.tar", last modified: Sat Jan 13 13:01:29 2024, max compression
+gzip compressed data, was "avilla_qqapi-1.0.0a29.tar", last modified: Fri Apr 12 14:08:36 2024, max compression
```

## Comparing `avilla_qqapi-1.0.0a28.tar` & `avilla_qqapi-1.0.0a29.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      447 2024-01-13 13:01:17.410789 avilla_qqapi-1.0.0a28/.mina/qqapi.toml
--rw-r--r--   0        0        0     1070 2024-01-13 13:01:17.410789 avilla_qqapi-1.0.0a28/LICENSE
--rw-r--r--   0        0        0     8444 2024-01-13 13:01:17.410789 avilla_qqapi-1.0.0a28/README.md
--rw-r--r--   0        0        0      102 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/__init__.py
--rw-r--r--   0        0        0      699 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/account.py
--rw-r--r--   0        0        0      253 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/audit/__init__.py
--rw-r--r--   0        0        0      761 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/audit/event.py
--rw-r--r--   0        0        0      417 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/audit/metadata.py
--rw-r--r--   0        0        0      886 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/audit/store.py
--rw-r--r--   0        0        0     2879 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/capability.py
--rw-r--r--   0        0        0        0 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/collector/__init__.py
--rw-r--r--   0        0        0      924 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/collector/connection.py
--rw-r--r--   0        0        0        0 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/connection/__init__.py
--rw-r--r--   0        0        0     3244 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/connection/base.py
--rw-r--r--   0        0        0     1870 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/connection/util.py
--rw-r--r--   0        0        0    17347 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/connection/ws_client.py
--rw-r--r--   0        0        0      941 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/const.py
--rw-r--r--   0        0        0     2297 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/element.py
--rw-r--r--   0        0        0     2330 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/exception.py
--rw-r--r--   0        0        0        0 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/__init__.py
--rw-r--r--   0        0        0        0 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/__init__.py
--rw-r--r--   0        0        0     2911 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/channel.py
--rw-r--r--   0        0        0     1404 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/guild.py
--rw-r--r--   0        0        0     8439 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/guild_member.py
--rw-r--r--   0        0        0    16912 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/message.py
--rw-r--r--   0        0        0    12722 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/role.py
--rw-r--r--   0        0        0     1216 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/user.py
--rw-r--r--   0        0        0     4853 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/context.py
--rw-r--r--   0        0        0        0 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/__init__.py
--rw-r--r--   0        0        0     3056 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/activity.py
--rw-r--r--   0        0        0     2525 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/audit.py
--rw-r--r--   0        0        0    13955 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/message.py
--rw-r--r--   0        0        0     2256 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/metadata.py
--rw-r--r--   0        0        0     7676 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/relationship.py
--rw-r--r--   0        0        0     5474 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/message/deserialize.py
--rw-r--r--   0        0        0     5262 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/message/serialize.py
--rw-r--r--   0        0        0     5463 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/query.py
--rw-r--r--   0        0        0     1139 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/perform/resource_fetch.py
--rw-r--r--   0        0        0     5030 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/protocol.py
--rw-r--r--   0        0        0      986 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/resource.py
--rw-r--r--   0        0        0      247 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/role/__init__.py
--rw-r--r--   0        0        0     1087 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/role/capability.py
--rw-r--r--   0        0        0      304 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/role/metadata.py
--rw-r--r--   0        0        0     1530 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/service.py
--rw-r--r--   0        0        0     1614 2024-01-13 13:01:17.418789 avilla_qqapi-1.0.0a28/avilla/qqapi/utils.py
--rw-r--r--   0        0        0      938 2024-01-13 13:01:29.722890 avilla_qqapi-1.0.0a28/pyproject.toml
--rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 avilla_qqapi-1.0.0a28/PKG-INFO
+-rw-r--r--   0        0        0      447 2024-04-12 14:08:23.843206 avilla_qqapi-1.0.0a29/.mina/qqapi.toml
+-rw-r--r--   0        0        0     1070 2024-04-12 14:08:23.847206 avilla_qqapi-1.0.0a29/LICENSE
+-rw-r--r--   0        0        0     8444 2024-04-12 14:08:23.847206 avilla_qqapi-1.0.0a29/README.md
+-rw-r--r--   0        0        0      102 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/account.py
+-rw-r--r--   0        0        0      253 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/__init__.py
+-rw-r--r--   0        0        0      761 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/event.py
+-rw-r--r--   0        0        0      417 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/metadata.py
+-rw-r--r--   0        0        0      886 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/audit/store.py
+-rw-r--r--   0        0        0     3230 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/capability.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/collector/__init__.py
+-rw-r--r--   0        0        0      924 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/collector/connection.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/__init__.py
+-rw-r--r--   0        0        0     3244 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/base.py
+-rw-r--r--   0        0        0     1870 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/util.py
+-rw-r--r--   0        0        0    17347 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/connection/ws_client.py
+-rw-r--r--   0        0        0      941 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/const.py
+-rw-r--r--   0        0        0     2297 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/element.py
+-rw-r--r--   0        0        0     2330 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/exception.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/__init__.py
+-rw-r--r--   0        0        0     2911 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/channel.py
+-rw-r--r--   0        0        0     1404 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild.py
+-rw-r--r--   0        0        0     8439 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild_member.py
+-rw-r--r--   0        0        0    19240 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/message.py
+-rw-r--r--   0        0        0    12722 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/role.py
+-rw-r--r--   0        0        0     1216 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/user.py
+-rw-r--r--   0        0        0     4853 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/context.py
+-rw-r--r--   0        0        0        0 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/__init__.py
+-rw-r--r--   0        0        0     3056 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/activity.py
+-rw-r--r--   0        0        0     2525 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/audit.py
+-rw-r--r--   0        0        0    13955 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/message.py
+-rw-r--r--   0        0        0     2256 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/metadata.py
+-rw-r--r--   0        0        0     7676 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/relationship.py
+-rw-r--r--   0        0        0     5474 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/deserialize.py
+-rw-r--r--   0        0        0     6431 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/serialize.py
+-rw-r--r--   0        0        0     5463 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/query.py
+-rw-r--r--   0        0        0     1139 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/perform/resource_fetch.py
+-rw-r--r--   0        0        0     5030 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/protocol.py
+-rw-r--r--   0        0        0      986 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/resource.py
+-rw-r--r--   0        0        0      247 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/__init__.py
+-rw-r--r--   0        0        0     1087 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/capability.py
+-rw-r--r--   0        0        0      304 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/role/metadata.py
+-rw-r--r--   0        0        0     1530 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/service.py
+-rw-r--r--   0        0        0     1614 2024-04-12 14:08:23.855206 avilla_qqapi-1.0.0a29/avilla/qqapi/utils.py
+-rw-r--r--   0        0        0      963 2024-04-12 14:08:36.595352 avilla_qqapi-1.0.0a29/pyproject.toml
+-rw-r--r--   0        0        0     8835 1970-01-01 00:00:00.000000 avilla_qqapi-1.0.0a29/PKG-INFO
```

### Comparing `avilla_qqapi-1.0.0a28/LICENSE` & `avilla_qqapi-1.0.0a29/LICENSE`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/README.md` & `avilla_qqapi-1.0.0a29/README.md`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/account.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/account.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/audit/event.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/audit/event.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/audit/store.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/audit/store.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/capability.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/capability.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Literal
 
 from graia.amnesia.message import Element, MessageChain
 
 from avilla.core.event import AvillaEvent
 from avilla.core.ryanvk.collector.application import ApplicationCollector
 from avilla.core.ryanvk.overload.target import TargetOverload
 from avilla.core.selector import Selector
@@ -28,14 +28,26 @@
         ...
 
     @Fn.complex({TargetOverload(): ["target"]})
     async def create_dms(self, target: Selector) -> Selector:
         """主动创建私聊会话，返回临时的 Guild"""
         ...
 
+    @Fn.complex({TargetOverload(): ["target"]})
+    async def post_file(
+        self,
+        target: Selector,
+        file_type: Literal[1, 2, 3, 4],
+        url: str | None = None,
+        srv_send_msg: bool = True,
+        file_data: str | bytes | None = None,
+    ) -> dict:
+        """上传文件，返回文件信息"""
+        ...
+
     async def deserialize(self, event: dict):
         elements = []
 
         if message_reference := event.get("message_reference"):
             elements.append(await self.deserialize_element({"type": "message_reference", **message_reference}))
         if event.get("mention_everyone", False):
             elements.append(await self.deserialize_element({"type": "mention_everyone"}))
```

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/collector/connection.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/collector/connection.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/connection/base.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/base.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/connection/util.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/util.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/connection/ws_client.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/connection/ws_client.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/const.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/const.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/element.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/element.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/exception.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/exception.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/channel.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/channel.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/guild.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/guild_member.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/guild_member.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/message.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from base64 import b64encode
 from datetime import datetime, timedelta, timezone
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from graia.amnesia.builtins.memcache import Memcache, MemcacheService
 from graia.amnesia.message import MessageChain
 from loguru import logger
 
 from avilla.core import Context, CoreCapability, Message
 from avilla.core.exceptions import ActionFailed
@@ -29,14 +30,84 @@
 
 class QQAPIMessageActionPerform((m := AccountCollector["QQAPIProtocol", "QQAPIAccount"]())._):
     m.namespace = "avilla.protocol/qqapi::action"
     m.identify = "message"
 
     context: OptionalAccess[Context] = OptionalAccess()
 
+    @m.entity(QQAPICapability.post_file, target="land.group")
+    async def post_group_file(
+        self,
+        target: Selector,
+        file_type: int,
+        url: str | None = None,
+        srv_send_msg: bool = True,
+        file_data: str | bytes | None = None,
+    ) -> dict:
+        if isinstance(file_data, bytes):
+            file_data = b64encode(file_data).decode()
+        result = await self.account.connection.call_http(
+            "post",
+            f"v2/groups/{target.pattern['group']}/files",
+            {
+                "file_type": file_type,
+                "url": url,
+                "srv_send_msg": srv_send_msg,
+                "file_data": file_data,
+            },
+        )
+        if result is None:
+            raise ActionFailed(f"Failed to post file to {target.pattern['group']}")
+        return result
+
+    @m.entity(QQAPICapability.post_file, target="land.friend")
+    async def post_friend_file(
+        self,
+        target: Selector,
+        file_type: int,
+        url: str | None = None,
+        srv_send_msg: bool = True,
+        file_data: str | bytes | None = None,
+    ) -> dict:
+        if isinstance(file_data, bytes):
+            file_data = b64encode(file_data).decode()
+        result = await self.account.connection.call_http(
+            "post",
+            f"v2/users/{target.pattern['friend']}/files",
+            {
+                "file_type": file_type,
+                "url": url,
+                "srv_send_msg": srv_send_msg,
+                "file_data": file_data,
+            },
+        )
+        if result is None:
+            raise ActionFailed(f"Failed to post file to {target.pattern['friend']}")
+        return result
+
+    @staticmethod
+    def _extract_qq_media(msg: dict) -> dict[str, Any]:
+        kwargs = {}
+        if media := msg.get("media"):
+            kwargs["file_type"] = {"image": 1, "video": 2, "audio": 3, "file": 4}.get(media[0], 4)
+            kwargs["url"] = media[1]
+        elif "file_image" in msg:
+            kwargs["file_type"] = 1
+            kwargs["file_data"] = msg.pop("file_image")
+        elif "file_audio" in msg:
+            kwargs["file_type"] = 2
+            kwargs["file_data"] = msg.pop("file_audio")
+        elif "file_video" in msg:
+            kwargs["file_type"] = 3
+            kwargs["file_data"] = msg.pop("file_video")
+        elif "file_file" in msg:
+            kwargs["file_type"] = 4
+            kwargs["file_data"] = msg.pop("file_file")
+        return kwargs
+
     @MessageSend.send.collect(m, target="land.guild.channel")
     async def send_channel_msg(
         self,
         target: Selector,
         message: MessageChain,
         *,
         reply: Selector | None = None,
@@ -103,40 +174,36 @@
         context = self.context
         if context and (event_id := context.cache.get(target.display_without_land)):
             msg["msg_id"] = event_id
         if reply:
             msg["msg_id"] = reply.pattern["message"]
             # TODO: wait for api upgrade
             # msg["message_reference"] = {"message_id": reply.pattern["message"]}
-        if "file_image" in msg:
-            raise NotImplementedError("file_image is not supported yet")
         if msg.get("embed"):
             msg_type = 4
         elif msg.get("ark"):
             msg_type = 3
         elif msg.get("markdown"):
             msg_type = 2
-        elif msg.get("media"):
+        elif any(
+            i in msg
+            for i in (
+                "media",
+                "file_image",
+                "file_video",
+                "file_audio",
+                "file_file",
+            )
+        ):
             msg_type = 7
         else:
             msg_type = 0
         msg["timestamp"] = int(datetime.now(timezone.utc).timestamp())
         if msg_type == 7:
-            file_types = {"image": 1, "video": 2, "audio": 3}
-            result = await self.account.connection.call_http(
-                "post",
-                f"v2/groups/{target.pattern['group']}/files",
-                {
-                    "file_type": file_types.get(msg["media"][0], 1),
-                    "url": msg["media"][1],
-                    "srv_send_msg": "msg_id" not in msg,
-                },
-            )
-            if result is None:
-                raise ActionFailed(f"Failed to send message to {target.pattern['group']}: {message}")
+            result = await self.post_group_file(target, srv_send_msg="msg_id" not in msg, **self._extract_qq_media(msg))
             if "msg_id" not in msg:
                 context = self.account.get_context(target)
                 msg = Message(
                     result.get("id", "UNKNOWN"),
                     target,
                     target.member(self.account.route["account"]),
                     message,
@@ -164,15 +231,19 @@
                 f"qqapi/account({self.account.route['account']}):{target}+msg_id:{msg.get('msg_id', '_')}",
                 2,
                 expire=timedelta(minutes=5),
             )
         # TODO: wait for api upgrade
         msg["content"] = unescape(msg["content"])
         method, data = form_data(msg)
-        result = await self.account.connection.call_http(method, f"v2/groups/{target.pattern['group']}/messages", data)
+        try:
+            result = await self.account.connection.call_http(method, f"v2/groups/{target.pattern['group']}/messages", data)
+        except ActionFailed:
+            msg["msg_seq"] = msg["msg_seq"] + (hash(target.pattern['group']) % 0x7FFFFFF) + int(datetime.now(timezone.utc).timestamp())
+            result = await self.account.connection.call_http(method, f"v2/groups/{target.pattern['group']}/messages", data)
         if result is None:
             raise ActionFailed(f"Failed to send message to {target.pattern['group']}: {message}")
         context = self.account.get_context(target)
         msg = Message(
             result.get("id", "UNKNOWN"),
             target,
             target.member(self.account.route["account"]),
@@ -195,40 +266,36 @@
         msg = await QQAPICapability(self.account.staff).serialize(message)
         if context and (event_id := context.cache.get(target.display_without_land)):
             msg["msg_id"] = event_id
         if reply:
             msg["msg_id"] = reply.pattern["message"]
             # TODO: wait for api upgrade
             # msg["message_reference"] = {"message_id": reply.pattern["message"]}
-        if "file_image" in msg:
-            raise NotImplementedError("file_image is not supported yet")
         if msg.get("embed"):
             msg_type = 4
         elif msg.get("ark"):
             msg_type = 3
         elif msg.get("markdown"):
             msg_type = 2
-        elif msg.get("media"):
-            msg_type = 1
+        elif any(
+            i in msg
+            for i in (
+                "media",
+                "file_image",
+                "file_video",
+                "file_audio",
+                "file_file",
+            )
+        ):
+            msg_type = 7
         else:
             msg_type = 0
         msg["timestamp"] = int(datetime.now(timezone.utc).timestamp())
-        if msg_type == 1:
-            file_types = {"image": 1, "video": 2, "audio": 3}
-            result = await self.account.connection.call_http(
-                "post",
-                f"v2/users/{target.pattern['friend']}/files",
-                {
-                    "file_type": file_types.get(msg["media"][0], 1),
-                    "url": msg["media"][1],
-                    "srv_send_msg": "msg_id" not in msg,
-                },
-            )
-            if result is None:
-                raise ActionFailed(f"Failed to send message to {target.pattern['friend']}: {message}")
+        if msg_type == 7:
+            result = await self.post_friend_file(target, srv_send_msg="msg_id" not in msg, **self._extract_qq_media(msg))
             if "msg_id" not in msg:
                 context = self.account.get_context(target)
                 msg = Message(
                     result.get("id", "UNKNOWN"),
                     target,
                     target.member(self.account.route["account"]),
                     message,
@@ -236,16 +303,14 @@
                 )
                 self.protocol.post_event(MessageSent(context, msg, self.account))
                 return target.message(result.get("id", "UNKNOWN"))
             msg["media"] = {"file_info": result["file_info"]}
             if "content" not in msg or not msg["content"]:
                 msg["content"] = " "
         msg["msg_type"] = msg_type
-        if "file_image" in msg:
-            raise NotImplementedError("file_image is not supported yet")
         if seq := await cache.get(
             f"qqapi/account({self.account.route['account']}):{target}+msg_id:{msg.get('msg_id', '_')}"
         ):
             msg["msg_seq"] = seq
             await cache.set(
                 f"qqapi/account({self.account.route['account']}):{target}+msg_id:{msg.get('msg_id', '_')}",
                 seq + 1,
@@ -257,15 +322,19 @@
                 f"qqapi/account({self.account.route['account']}):{target}+msg_id:{msg.get('msg_id', '_')}",
                 2,
                 expire=timedelta(minutes=5),
             )
         # TODO: wait for api upgrade
         msg["content"] = unescape(msg["content"])
         method, data = form_data(msg)
-        result = await self.account.connection.call_http(method, f"v2/users/{target.pattern['friend']}/messages", data)
+        try:
+            result = await self.account.connection.call_http(method, f"v2/users/{target.pattern['friend']}/messages", data)
+        except ActionFailed:
+            msg["msg_seq"] = msg["msg_seq"] + (hash(target.pattern['friend']) % 0x7FFFFFF) + int(datetime.now(timezone.utc).timestamp())
+            result = await self.account.connection.call_http(method, f"v2/users/{target.pattern['friend']}/messages", data)
         if result is None:
             raise ActionFailed(f"Failed to send message to {target.pattern['friend']}: {message}")
         context = self.account.get_context(target)
         msg = Message(
             result.get("id", "UNKNOWN"),
             target,
             target.member(self.account.route["account"]),
```

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/role.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/role.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/action/user.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/action/user.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/context.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/context.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/activity.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/activity.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/audit.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/audit.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/message.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/message.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/metadata.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/metadata.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/event/relationship.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/event/relationship.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/message/deserialize.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/deserialize.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/message/serialize.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/message/serialize.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
 from dataclasses import asdict
 from typing import TYPE_CHECKING
 
-from avilla.core.elements import Audio, Face, Notice, NoticeAll, Picture, Text, Video
+from avilla.core.elements import Audio, Face, File, Notice, NoticeAll, Picture, Text, Video
 from avilla.core.resource import LocalFileResource, RawResource, UrlResource
 from avilla.core.ryanvk.collector.account import AccountCollector
 from avilla.qqapi.capability import QQAPICapability
 from avilla.qqapi.element import Ark, Embed, Keyboard, Markdown, Reference
 from avilla.qqapi.resource import (
     QQAPIAudioResource,
     QQAPIImageResource,
     QQAPIVideoResource,
+    QQAPIFileResource,
 )
 from avilla.qqapi.utils import escape
 
 if TYPE_CHECKING:
     from avilla.qqapi.account import QQAPIAccount  # noqa
     from avilla.qqapi.protocol import QQAPIProtocol  # noqa
 
@@ -54,21 +55,39 @@
             return "file_image", element.resource.data
         return "file_image", await self.account.staff.fetch_resource(element.resource)
 
     @m.entity(QQAPICapability.serialize_element, element=Audio)
     async def audio(self, element: Audio):
         if isinstance(element.resource, (QQAPIAudioResource, UrlResource)):
             return "media", ("audio", element.resource.url)
-        raise NotImplementedError
+        if isinstance(element.resource, LocalFileResource):
+            return "file_audio", element.resource.file.read_bytes()
+        if isinstance(element.resource, RawResource):
+            return "file_audio", element.resource.data
+        return "file_audio", await self.account.staff.fetch_resource(element.resource)
 
     @m.entity(QQAPICapability.serialize_element, element=Video)
     async def video(self, element: Video):
         if isinstance(element.resource, (QQAPIVideoResource, UrlResource)):
             return "media", ("video", element.resource.url)
-        raise NotImplementedError
+        if isinstance(element.resource, LocalFileResource):
+            return "file_video", element.resource.file.read_bytes()
+        if isinstance(element.resource, RawResource):
+            return "file_video", element.resource.data
+        return "file_video", await self.account.staff.fetch_resource(element.resource)
+
+    @m.entity(QQAPICapability.serialize_element, element=File)
+    async def file(self, element: File):
+        if isinstance(element.resource, (QQAPIFileResource, UrlResource)):
+            return "media", ("file", element.resource.url)
+        if isinstance(element.resource, LocalFileResource):
+            return "file_file", element.resource.file.read_bytes()
+        if isinstance(element.resource, RawResource):
+            return "file_file", element.resource.data
+        return "file_file", await self.account.staff.fetch_resource(element.resource)
 
     @m.entity(QQAPICapability.serialize_element, element=Reference)
     async def reference(self, element: Reference):
         return "message_reference", {
             "message_id": element.message["message"],
             "ignore_get_message_error": element.ignore_get_message_error,
         }
```

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/query.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/query.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/perform/resource_fetch.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/perform/resource_fetch.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/protocol.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/protocol.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/resource.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/resource.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/role/capability.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/role/capability.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/service.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/service.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/avilla/qqapi/utils.py` & `avilla_qqapi-1.0.0a29/avilla/qqapi/utils.py`

 * *Files identical despite different names*

### Comparing `avilla_qqapi-1.0.0a28/pyproject.toml` & `avilla_qqapi-1.0.0a29/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "avilla-qqapi"
-version = "1.0.0a28"
+version = "1.0.0a29"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "aiohttp>=3.8.1",
 ]
 description = ""
@@ -16,35 +16,36 @@
 
 [project.urls]
 homepage = "https://github.com/GraiaProject/Avilla"
 repository = "https://github.com/GraiaProject/Avilla"
 
 [build-system]
 requires = [
-    "mina-build>=0.5.1",
+    "mina-build<0.6.0",
 ]
 build-backend = "mina.backend"
 
 [tool.pdm.build]
 includes = [
     "avilla/qqapi",
     ".mina/qqapi.toml",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=23.7.0",
-    "mina-build>=0.4.0",
+    "black>=24.2.0",
+    "mina-build>=0.4.0,<0.6.0",
     "richuru>=0.1.1",
-    "ruff>=0.0.272",
-    "uvicorn>=0.22.0",
+    "ruff>=0.3.2",
+    "uvicorn>=0.27.0",
     "devtools>=0.11",
     "ipykernel>=6.23.2",
     "pip>=23.2.1",
     "pdm-mina>=0.3.1",
+    "isort>=5.13.2",
 ]
 
 [tool.mina]
 enabled = true
 
 [tool.black]
 include = "\\.pyi?$"
```

### Comparing `avilla_qqapi-1.0.0a28/PKG-INFO` & `avilla_qqapi-1.0.0a29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avilla-qqapi
-Version: 1.0.0a28
+Version: 1.0.0a29
 Home-page: https://github.com/GraiaProject/Avilla
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/GraiaProject/Avilla
 Project-URL: Repository, https://github.com/GraiaProject/Avilla
 Requires-Python: >=3.9
 Requires-Dist: aiohttp>=3.8.1
```

