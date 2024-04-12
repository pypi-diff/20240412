# Comparing `tmp/omuserver-0.2.3.tar.gz` & `tmp/omuserver-0.2.4.tar.gz`

## Comparing `omuserver-0.2.3.tar` & `omuserver-0.2.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.3/.python-version
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.3/.vscode/settings.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/__main__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/config.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/directories.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/helper.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/dashboard/__init__.py
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/dashboard/dashboard_extension.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     6980 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/message/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/message/message_extension.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/permission/__init__.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/permission/permission_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/plugin/plugin_loader.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/security/security.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 omuserver-0.2.3/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.3/test/helper_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.3/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.3/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.4/.python-version
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.4/.vscode/settings.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/config.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/directories.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/helper.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/message/__init__.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/message/message_extension.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     8546 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8307 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0     6704 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 omuserver-0.2.4/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.4/test/helper_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.4/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.4/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.4/PKG-INFO
```

### Comparing `omuserver-0.2.3/src/omuserver/__main__.py` & `omuserver-0.2.4/src/omuserver/__main__.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/helper.py` & `omuserver-0.2.4/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/asset/asset_extension.py` & `omuserver-0.2.4/src/omuserver/extension/asset/asset_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/dashboard/dashboard_extension.py` & `omuserver-0.2.4/src/omuserver/extension/dashboard/dashboard_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from asyncio import Future
 from typing import Dict
 
+from omu.app import App
 from omu.extension.dashboard.dashboard import PermissionRequest
 from omu.extension.dashboard.dashboard_extension import (
+    DASHBOARD_OPEN_APP_ENDPOINT,
+    DASHBOARD_OPEN_APP_PACKET,
     DASHBOARD_PERMISSION_ACCEPT_PACKET,
     DASHBOARD_PERMISSION_DENY_PACKET,
     DASHBOARD_PERMISSION_REQUEST_PACKET,
     DASHBOARD_SET_ENDPOINT,
+    DashboardOpenAppResponse,
     DashboardSetResponse,
 )
 from omu.identifier import Identifier
 
 from omuserver.server import Server
 from omuserver.session import Session
 
@@ -21,27 +25,51 @@
         self.dashboard_session: Session | None = None
         self.pending_permission_requests: Dict[int, PermissionRequest] = {}
         self.permission_requests: Dict[int, Future[bool]] = {}
         server.packet_dispatcher.register(
             DASHBOARD_PERMISSION_REQUEST_PACKET,
             DASHBOARD_PERMISSION_ACCEPT_PACKET,
             DASHBOARD_PERMISSION_DENY_PACKET,
-        )
-        server.endpoints.bind_endpoint(
-            DASHBOARD_SET_ENDPOINT,
-            self.handle_dashboard_set,
+            DASHBOARD_OPEN_APP_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
             DASHBOARD_PERMISSION_ACCEPT_PACKET,
             self.handle_permission_accept,
         )
         server.packet_dispatcher.add_packet_handler(
             DASHBOARD_PERMISSION_DENY_PACKET,
             self.handle_permission_deny,
         )
+        server.endpoints.bind_endpoint(
+            DASHBOARD_SET_ENDPOINT,
+            self.handle_dashboard_set,
+        )
+        server.endpoints.bind_endpoint(
+            DASHBOARD_OPEN_APP_ENDPOINT,
+            self.handle_dashboard_open_app,
+        )
+
+    async def handle_dashboard_open_app(
+        self, session: Session, app: App
+    ) -> DashboardOpenAppResponse:
+        if self.dashboard_session is None:
+            return {
+                "success": False,
+                "already_open": False,
+                "dashboard_not_connected": True,
+            }
+        await self.dashboard_session.send(
+            DASHBOARD_OPEN_APP_PACKET,
+            app,
+        )
+        return {
+            "success": True,
+            "already_open": False,
+            "dashboard_not_connected": False,
+        }
 
     async def handle_dashboard_set(
         self, session: Session, identifier: Identifier
     ) -> DashboardSetResponse:
         if session.token != self.server.config.dashboard_token:
             raise ValueError("Dashboard token does not match")
         self.dashboard_session = session
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/endpoint/endpoint_extension.py` & `omuserver-0.2.4/src/omuserver/extension/endpoint/endpoint_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
     async def _on_endpoint_call(
         self, session: Session, req: EndpointDataPacket
     ) -> None:
         endpoint = await self._get_endpoint(req, session)
         if endpoint is None:
             logger.warning(
-                f"{session.app.name} tried to call unknown endpoint {req['type']}"
+                f"{session.app.key()} tried to call unknown endpoint {req['type']}"
             )
             await session.send(
                 ENDPOINT_ERROR_PACKET,
                 EndpointErrorPacket(
                     type=req["type"],
                     id=req["id"],
                     error=f"Endpoint {req['type']} not found",
@@ -199,11 +199,11 @@
                 EndpointErrorPacket(
                     type=req["type"],
                     id=req["id"],
                     error=f"Endpoint {req['type']} not found",
                 ),
             )
             logger.warning(
-                f"{session.app.name} tried to call unconnected endpoint {req['type']}"
+                f"{session.app.key()} tried to call unconnected endpoint {req['type']}"
             )
             return
         return endpoint
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/permission/permission_extension.py` & `omuserver-0.2.4/src/omuserver/extension/permission/permission_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,19 @@
             raise ValueError(f"Permission {permission.identifier} already registered")
         self.permission_registry[permission.identifier] = permission
 
     async def handle_register(
         self, session: Session, permissions: List[PermissionType]
     ) -> None:
         for permission in permissions:
+            if not permission.identifier.is_subpart_of(session.app.identifier):
+                raise ValueError(
+                    f"Permission identifier {permission.identifier} "
+                    f"is not a subpart of app identifier {session.app.identifier}"
+                )
             self.permission_registry[permission.identifier] = permission
 
     async def handle_request(
         self, session: Session, permission_identifiers: List[Identifier]
     ):
         self.request_id += 1
         permissions: List[PermissionType] = []
@@ -58,10 +63,11 @@
                 permissions.append(permission)
 
         accepted = await self.server.dashboard.request_permissions(
             PermissionRequest(self.request_id, session.app, permissions)
         )
         if accepted:
             self.session_permissions[session] = permissions
-            await session.send(PERMISSION_GRANT_PACKET, permissions)
+            if not session.closed:
+                await session.send(PERMISSION_GRANT_PACKET, permissions)
         else:
             await session.disconnect()
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/plugin/plugin_loader.py` & `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,25 @@
         )
 
 
 class PluginLoader:
     def __init__(self, server: Server) -> None:
         self._server = server
         self.plugins: Dict[str, Plugin] = {}
+        server.listeners.start += self.handle_server_start
+
+    async def handle_server_start(self) -> None:
+        for plugin in self.plugins.values():
+            if plugin.on_start_server is not None:
+                await plugin.on_start_server(self._server)
+
+    async def handle_server_stop(self) -> None:
+        for plugin in self.plugins.values():
+            if plugin.on_stop_server is not None:
+                await plugin.on_stop_server(self._server)
 
     async def load_plugins(self) -> None:
         await self.run_plugins()
 
     async def run_plugins(self):
         entry_points = importlib.metadata.entry_points(group=PLUGIN_GROUP)
         for entry_point in entry_points:
@@ -170,34 +181,37 @@
             plugin = self.load_plugin_from_entry_point(entry_point)
             self.plugins[plugin_key] = plugin
             await self.run_plugin(plugin)
 
     async def run_plugin(self, plugin: Plugin):
         if plugin.isolated:
             process = Process(
-                target=run_plugin_process,
+                target=run_plugin_isolated,
                 args=(
                     plugin,
                     self._server.address,
                 ),
                 daemon=True,
             )
             process.start()
         else:
-            plugin_client = plugin.get_client()
-            connection = PluginConnection()
-            plugin_client.network.set_connection(connection)
-            await plugin_client.start()
-            session_connection = PluginSessionConnection(connection)
-            session = await Session.from_connection(
-                self._server,
-                self._server.packet_dispatcher.packet_mapper,
-                session_connection,
-            )
-            self._server.loop.create_task(self._server.network.process_session(session))
+            if plugin.get_client is not None:
+                plugin_client = plugin.get_client()
+                connection = PluginConnection()
+                plugin_client.network.set_connection(connection)
+                await plugin_client.start()
+                session_connection = PluginSessionConnection(connection)
+                session = await Session.from_connection(
+                    self._server,
+                    self._server.packet_dispatcher.packet_mapper,
+                    session_connection,
+                )
+                self._server.loop.create_task(
+                    self._server.network.process_session(session)
+                )
 
     def load_plugin_from_entry_point(
         self, entry_point: importlib.metadata.EntryPoint
     ) -> Plugin:
         plugin = entry_point.load()
         if not isinstance(plugin, Plugin):
             raise ValueError(f"Invalid plugin: {plugin} is not a Plugin")
@@ -207,18 +221,20 @@
 def handle_exception(loop: asyncio.AbstractEventLoop, context: dict) -> None:
     logger.error(context["message"])
     exception = context.get("exception")
     if exception:
         raise exception
 
 
-def run_plugin_process(
+def run_plugin_isolated(
     plugin: Plugin,
     address: Address,
 ) -> None:
+    if plugin.get_client is None:
+        raise ValueError(f"Invalid plugin: {plugin} has no client")
     client = plugin.get_client()
     connection = WebsocketsConnection(client, address)
     client.network.set_connection(connection)
     loop = asyncio.get_event_loop()
     loop.set_exception_handler(handle_exception)
     loop.run_until_complete(client.start())
     loop.run_forever()
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.2.4/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/registry/registry.py` & `omuserver-0.2.4/src/omuserver/extension/registry/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-from typing import Any, Dict
+from typing import Dict
 
 from omu import Identifier
 from omu.extension.registry.registry_extension import (
     REGISTRY_UPDATE_PACKET,
     RegistryPacket,
 )
 from omu.serializer import Serializable
 
 from omuserver.server import Server
 from omuserver.session import Session
 
 
 class ServerRegistry:
     def __init__(self, server: Server, identifier: Identifier) -> None:
-        self._key = identifier.key()
-        self._listeners: Dict[str, Session] = {}
+        self.identifier = identifier
+        self._listeners: Dict[Identifier, Session] = {}
         self._path = server.directories.get(
             "registry"
         ) / identifier.to_path().with_suffix(".json")
         self._changed = False
-        self.existing = self._path.exists()
-        self.data: bytes = b""
+        self.data: bytes | None = None
 
-    async def load(self) -> Any:
-        if self.data is None:
-            if self._path.exists():
-                self.data = self._path.read_bytes()
-            else:
-                self.data = b""
-        return self.data
+    async def load(self):
+        if self._path.exists():
+            self.data = self._path.read_bytes()
 
-    async def store(self, value: bytes) -> None:
+    async def store(self, value: bytes | None) -> None:
         self.data = value
         self._path.parent.mkdir(parents=True, exist_ok=True)
-        self._path.write_bytes(value)
+        if value is None:
+            self._path.unlink(missing_ok=True)
+        else:
+            self._path.write_bytes(value)
         await self._notify()
 
     async def _notify(self) -> None:
         for listener in self._listeners.values():
             if listener.closed:
                 raise Exception(f"Session {listener.app=} closed")
             await listener.send(
                 REGISTRY_UPDATE_PACKET,
-                RegistryPacket(key=self._key, existing=self.existing, value=self.data),
+                RegistryPacket(identifier=self.identifier, value=self.data),
             )
 
     async def attach_session(self, session: Session) -> None:
-        if session.app.key() in self._listeners:
-            del self._listeners[session.app.key()]
-        self._listeners[session.app.key()] = session
+        if session.app.identifier in self._listeners:
+            raise Exception("Session already attached")
+        self._listeners[session.app.identifier] = session
         session.listeners.disconnected += self.detach_session
         await session.send(
             REGISTRY_UPDATE_PACKET,
-            RegistryPacket(key=self._key, existing=self.existing, value=self.data),
+            RegistryPacket(identifier=self.identifier, value=self.data),
         )
 
     async def detach_session(self, session: Session) -> None:
-        if session.app.key() not in self._listeners:
+        if session.app.identifier not in self._listeners:
             raise Exception("Session not attached")
-        del self._listeners[session.app.key()]
+        del self._listeners[session.app.identifier]
         session.listeners.disconnected -= self.detach_session
 
 
 class Registry[T]:
     def __init__(
         self,
         registry: ServerRegistry,
@@ -70,13 +68,13 @@
         serializer: Serializable[T, bytes],
     ) -> None:
         self._registry = registry
         self._default_value = default_value
         self._serializer = serializer
 
     async def get(self) -> T:
-        if not self._registry.existing:
+        if self._registry.data is None:
             return self._default_value
         return self._serializer.deserialize(self._registry.data)
 
     async def set(self, value: T) -> None:
         await self._registry.store(self._serializer.serialize(value))
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/server/server_extension.py` & `omuserver-0.2.4/src/omuserver/extension/server/server_extension.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 from typing import TYPE_CHECKING
 
 from loguru import logger
 from omu.extension.server.server_extension import (
     APPS_TABLE_TYPE,
     SHUTDOWN_ENDPOINT_TYPE,
+    VERSION_REGISTRY_TYPE,
 )
-from omu.serializer import Serializer
 
 from omuserver import __version__
 from omuserver.helper import get_launch_command
 
 if TYPE_CHECKING:
     from omuserver.server import Server
-    from omuserver.session.session import Session
+    from omuserver.session import Session
 
 
 class ServerExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
+        self.version_registry = self._server.registry.create(VERSION_REGISTRY_TYPE)
         server.network.listeners.connected += self.on_connected
         server.network.listeners.disconnected += self.on_disconnected
         server.listeners.start += self.on_start
         server.endpoints.bind_endpoint(SHUTDOWN_ENDPOINT_TYPE, self.shutdown)
 
     async def shutdown(self, session: Session, restart: bool = False) -> bool:
         await self._server.shutdown()
@@ -36,23 +37,16 @@
             import sys
 
             os.execv(sys.executable, get_launch_command()["args"])
         else:
             self._server.loop.stop()
 
     async def on_start(self) -> None:
+        await self.version_registry.set(__version__)
         self.apps = await self._server.tables.register_table(APPS_TABLE_TYPE)
-        version = await self._server.registry.create(
-            "server:version", __version__, Serializer.json()
-        )
-        await version.set(__version__)
-        directories = await self._server.registry.create(
-            "server:directories", self._server.directories.to_json(), Serializer.json()
-        )
-        await directories.set(self._server.directories.to_json())
         await self.apps.clear()
 
     async def on_connected(self, session: Session) -> None:
         logger.info(f"Connected: {session.app.key()}")
         await self.apps.add(session.app)
 
     async def on_disconnected(self, session: Session) -> None:
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/cached_table.py` & `omuserver-0.2.4/src/omuserver/extension/table/cached_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, AsyncGenerator, Dict, List
+from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Mapping
 
 from omu.extension.table import TableConfig
 from omu.extension.table.table_extension import TABLE_PROXY_PACKET, TableProxyData
 from omu.identifier import Identifier
 
 from .adapters.tableadapter import TableAdapter
 from .server_table import ServerTable, ServerTableListeners
@@ -103,38 +103,40 @@
             return items
         data = await self._adapter.get_many(key_list)
         for key, value in data.items():
             items[key] = value
         await self.update_cache(items)
         return items
 
-    async def add(self, items: Dict[str, bytes]) -> None:
+    async def add(self, items: Mapping[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         if len(self._proxy_sessions) > 0:
             await self.send_proxy_event(items)
             return
         await self._adapter.set_all(items)
         await self._listeners.add(items)
         await self.update_cache(items)
         self.mark_changed()
 
-    async def send_proxy_event(self, items: Dict[str, bytes]) -> None:
+    async def send_proxy_event(self, items: Mapping[str, bytes]) -> None:
         session = tuple(self._proxy_sessions.values())[0]
         self._proxy_id += 1
         await session.send(
             TABLE_PROXY_PACKET,
             TableProxyData(
                 items=items,
                 type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
 
-    async def proxy(self, session: Session, key: int, items: Dict[str, bytes]) -> int:
+    async def proxy(
+        self, session: Session, key: int, items: Mapping[str, bytes]
+    ) -> int:
         adapter = self._adapter
         if adapter is None:
             raise Exception("Table not set")
         if session.app.key() not in self._proxy_sessions:
             raise ValueError("Session not in proxy sessions")
         session_key = session.app.key()
         index = tuple(self._proxy_sessions.keys()).index(session_key)
@@ -154,15 +156,15 @@
                 items=items,
                 type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
         return self._proxy_id
 
-    async def update(self, items: Dict[str, bytes]) -> None:
+    async def update(self, items: Mapping[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         await self._adapter.set_all(items)
         await self._listeners.update(items)
         await self.update_cache(items)
         self.mark_changed()
 
@@ -229,15 +231,15 @@
         self._changed = True
         if self._save_task is None:
             self._save_task = asyncio.create_task(self.save_task())
 
     def set_cache_size(self, size: int) -> None:
         self._cache_size = size
 
-    async def update_cache(self, items: Dict[str, bytes]) -> None:
+    async def update_cache(self, items: Mapping[str, bytes]) -> None:
         if self._cache_size is None or self._cache_size <= 0:
             return
         for key, item in items.items():
             self._cache[key] = item
             if len(self._cache) > self._cache_size:
                 del self._cache[next(iter(self._cache))]
         await self._listeners.cache_update(self._cache)
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.2.4/src/omuserver/extension/table/serialized_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     def __init__(self, table: ServerTable, type: TableType[T]):
         self._table = table
         self._type = type
         self._listeners = TableListeners[T](self)
         self._proxies: List[Coro[[T], T | None]] = []
         self._chunk_size = 100
         self.key = type.identifier.key()
+        self._listening = False
         table.listeners.cache_update += self.on_cache_update
         table.listeners.add += self.on_add
         table.listeners.update += self.on_update
         table.listeners.remove += self.on_remove
         table.listeners.clear += self.on_clear
 
     @property
@@ -117,36 +118,36 @@
     ) -> Callable[[], None]:
         self._listening = True
         if listener:
             self._listeners.cache_update += listener
             return lambda: self._listeners.cache_update.unsubscribe(listener)
         return lambda: None
 
-    async def on_add(self, items: Dict[str, bytes]) -> None:
+    async def on_cache_update(self, cache: Mapping[str, bytes]) -> None:
+        await self._listeners.cache_update(self._parse_items(cache))
+
+    async def on_add(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
         await self._listeners.add(_items)
 
-    async def on_update(self, items: Dict[str, bytes]) -> None:
+    async def on_update(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
         await self._listeners.update(_items)
 
-    async def on_remove(self, items: Dict[str, bytes]) -> None:
+    async def on_remove(self, items: Mapping[str, bytes]) -> None:
         _items = self._parse_items(items)
         await self._listeners.remove(_items)
 
     async def on_clear(self) -> None:
         await self._listeners.clear()
 
-    async def on_cache_update(self, cache: Dict[str, bytes]) -> None:
-        await self._listeners.cache_update(self._parse_items(cache))
-
     def proxy(self, callback: Coro[[T], T | None]) -> Callable[[], None]:
         raise NotImplementedError
 
-    def _parse_items(self, items: Dict[str, bytes]) -> Dict[str, T]:
+    def _parse_items(self, items: Mapping[str, bytes]) -> Dict[str, T]:
         parsed: Dict[str, T] = {}
         for key, item in items.items():
             item = self._type.serializer.deserialize(item)
             if not item:
                 raise Exception(f"Failed to deserialize item {key}")
             parsed[key] = item
         return parsed
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/server_table.py` & `omuserver-0.2.4/src/omuserver/extension/table/server_table.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Union
+from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Mapping, Union
 
 from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
     from omu.extension.table import TableConfig
 
     from omuserver.session import Session
@@ -40,31 +40,31 @@
     def detach_session(self, session: Session) -> None: ...
 
     @abc.abstractmethod
     def attach_proxy_session(self, session: Session) -> None: ...
 
     @abc.abstractmethod
     async def proxy(
-        self, session: Session, key: int, items: Dict[str, bytes]
+        self, session: Session, key: int, items: Mapping[str, bytes]
     ) -> int: ...
 
     @abc.abstractmethod
     async def store(self) -> None: ...
 
     @abc.abstractmethod
     async def get(self, key: str) -> bytes | None: ...
 
     @abc.abstractmethod
     async def get_many(self, *keys: str) -> Dict[str, bytes]: ...
 
     @abc.abstractmethod
-    async def add(self, items: Dict[str, bytes]) -> None: ...
+    async def add(self, items: Mapping[str, bytes]) -> None: ...
 
     @abc.abstractmethod
-    async def update(self, items: Dict[str, bytes]) -> None: ...
+    async def update(self, items: Mapping[str, bytes]) -> None: ...
 
     @abc.abstractmethod
     async def remove(self, keys: List[str]) -> None: ...
 
     @abc.abstractmethod
     async def clear(self) -> None: ...
 
@@ -88,12 +88,12 @@
     @property
     @abc.abstractmethod
     def listeners(self) -> ServerTableListeners: ...
 
 
 class ServerTableListeners:
     def __init__(self) -> None:
-        self.add: EventEmitter[Dict[str, bytes]] = EventEmitter()
-        self.update: EventEmitter[Dict[str, bytes]] = EventEmitter()
-        self.remove: EventEmitter[Dict[str, bytes]] = EventEmitter()
-        self.clear: EventEmitter[[]] = EventEmitter()
-        self.cache_update: EventEmitter[Dict[str, bytes]] = EventEmitter()
+        self.add = EventEmitter[Mapping[str, bytes]]()
+        self.update = EventEmitter[Mapping[str, bytes]]()
+        self.remove = EventEmitter[Mapping[str, bytes]]()
+        self.clear = EventEmitter[[]]()
+        self.cache_update = EventEmitter[Mapping[str, bytes]]()
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/session_table_handler.py` & `omuserver-0.2.4/src/omuserver/extension/table/session_table_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Mapping
 
 from omu.extension.table.table_extension import (
     TABLE_ITEM_ADD_PACKET,
     TABLE_ITEM_CLEAR_PACKET,
     TABLE_ITEM_REMOVE_EVENT,
     TABLE_ITEM_UPDATE_PACKET,
     TableEventData,
@@ -29,37 +29,37 @@
 
     def close(self) -> None:
         self.table.listeners.add -= self.on_add
         self.table.listeners.update -= self.on_update
         self.table.listeners.remove -= self.on_remove
         self.table.listeners.clear -= self.on_clear
 
-    async def on_add(self, items: Dict[str, Any]) -> None:
+    async def on_add(self, items: Mapping[str, Any]) -> None:
         if self._session.closed:
             return
         await self._session.send(
             TABLE_ITEM_ADD_PACKET,
             TableItemsData(
                 items=items,
                 type=self._id,
             ),
         )
 
-    async def on_update(self, items: Dict[str, Any]) -> None:
+    async def on_update(self, items: Mapping[str, Any]) -> None:
         if self._session.closed:
             return
         await self._session.send(
             TABLE_ITEM_UPDATE_PACKET,
             TableItemsData(
                 items=items,
                 type=self._id,
             ),
         )
 
-    async def on_remove(self, items: Dict[str, Any]) -> None:
+    async def on_remove(self, items: Mapping[str, Any]) -> None:
         if self._session.closed:
             return
         await self._session.send(
             TABLE_ITEM_REMOVE_EVENT,
             TableItemsData(
                 items=items,
                 type=self._id,
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/table_extension.py` & `omuserver-0.2.4/src/omuserver/extension/table/table_extension.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.2.4/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         )
         rows = cursor.fetchall()
         return {row[0]: row[1] for row in rows}
 
     async def set(self, key: str, value: bytes) -> None:
         self._conn.execute(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
-            (key, (value)),
+            (key, value),
         )
 
     async def set_all(self, items: Mapping[str, bytes]) -> None:
         query = [(key, value) for key, value in items.items()]
         self._conn.executemany(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
             query,
```

### Comparing `omuserver-0.2.3/src/omuserver/extension/table/adapters/tableadapter.py` & `omuserver-0.2.4/src/omuserver/extension/table/adapters/tableadapter.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/network/network.py` & `omuserver-0.2.4/src/omuserver/network/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,10 +141,10 @@
     @property
     def listeners(self) -> NetworkListeners:
         return self._listeners
 
 
 class NetworkListeners:
     def __init__(self) -> None:
-        self.start = EventEmitter()
+        self.start = EventEmitter[[]]()
         self.connected = EventEmitter[Session]()
         self.disconnected = EventEmitter[Session]()
```

### Comparing `omuserver-0.2.3/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.2.4/src/omuserver/network/packet_dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         self,
         event_type: PacketType[T],
         listener: Coro[[Session, T], None] | None = None,
     ) -> Callable[[Coro[[Session, T], None]], None]:
         if not self._packet_listeners.get(event_type.identifier):
             raise ValueError(f"Event type {event_type.identifier} not registered")
 
-        def decorator(listener: Coro[[Session, T], None]) -> None:
-            self._packet_listeners[event_type.identifier].listeners.subscribe(listener)
+        def decorator(func: Coro[[Session, T], None]) -> None:
+            self._packet_listeners[event_type.identifier].listeners.subscribe(func)
 
         if listener:
             decorator(listener)
         return decorator
 
 
 @dataclass(frozen=True)
```

### Comparing `omuserver-0.2.3/src/omuserver/security/security.py` & `omuserver-0.2.4/src/omuserver/security/security.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import abc
 import datetime
 import random
 import sqlite3
+import string
 
 from omu import App
 
 from omuserver.server import Server
 
 type Token = str
 
@@ -16,15 +17,15 @@
 
     @abc.abstractmethod
     async def validate_app_token(self, app: App, token: Token) -> bool: ...
 
 
 class TokenGenerator:
     def __init__(self):
-        self._chars = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
+        self._chars = string.ascii_letters + string.digits
 
     def generate(self, length: int) -> str:
         return "".join(random.choices(self._chars, k=length))
 
 
 class ServerAuthenticator(Security):
     def __init__(self, server: Server):
```

### Comparing `omuserver-0.2.3/src/omuserver/server/omuserver.py` & `omuserver-0.2.4/src/omuserver/server/omuserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         self._network.add_http_route("/asset", self._handle_assets)
         self._security = ServerAuthenticator(self)
         self._running = False
         self._endpoints = EndpointExtension(self)
         self._dashboard = DashboardExtension(self)
         self._permissions = PermissionExtension(self)
         self._tables = TableExtension(self)
-        self._server = ServerExtension(self)
         self._registry = RegistryExtension(self)
+        self._server = ServerExtension(self)
         self._messages = MessageExtension(self)
         self._plugins = PluginExtension(self)
         self._assets = AssetExtension(self)
 
     async def _handle_proxy(self, request: web.Request) -> web.StreamResponse:
         url = request.query.get("url")
         no_cache = bool(request.query.get("no_cache"))
@@ -79,19 +79,22 @@
         try:
             async with client.get(url) as resp:
                 headers = {
                     "Cache-Control": "no-cache" if no_cache else "max-age=3600",
                     "Content-Type": resp.content_type,
                 }
                 resp.raise_for_status()
-                return web.Response(
+                response = web.StreamResponse(
                     status=resp.status,
                     headers=headers,
-                    body=await resp.read(),
                 )
+                await response.prepare(request)
+                async for chunk in resp.content.iter_any():
+                    await response.write(chunk)
+                return response
         except aiohttp.ClientResponseError as e:
             return web.Response(status=e.status, text=e.message)
         except Exception as e:
             logger.error(e)
             return web.Response(status=500)
 
     async def _handle_assets(self, request: web.Request) -> web.StreamResponse:
```

### Comparing `omuserver-0.2.3/src/omuserver/server/server.py` & `omuserver-0.2.4/src/omuserver/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     from omuserver.network import Network
     from omuserver.network.packet_dispatcher import ServerPacketDispatcher
     from omuserver.security import Security
 
 
 class ServerListeners:
     def __init__(self) -> None:
-        self.start = EventEmitter()
-        self.stop = EventEmitter()
+        self.start = EventEmitter[[]]()
+        self.stop = EventEmitter[[]]()
 
 
 class Server(abc.ABC):
     @property
     @abc.abstractmethod
     def config(self) -> Config: ...
```

### Comparing `omuserver-0.2.3/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.2.4/src/omuserver/session/aiohttp_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/src/omuserver/session/session.py` & `omuserver-0.2.4/src/omuserver/session/session.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.2.3/pyproject.toml` & `omuserver-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "omuserver"
-version = "0.2.3"
+version = "0.2.4"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "sqlitedict>=2.1.0",
     "click>=8.1.7",
```

### Comparing `omuserver-0.2.3/PKG-INFO` & `omuserver-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: omuserver
-Version: 0.2.3
+Version: 0.2.4
 Summary: Add your description here
 Author-email: am230 <111672334+am230@users.noreply.github.com>
 Requires-Python: >=3.12
 Requires-Dist: aiohttp>=3.9.3
 Requires-Dist: aiosqlite>=0.19.0
 Requires-Dist: click>=8.1.7
 Requires-Dist: loguru>=0.7.2
```

