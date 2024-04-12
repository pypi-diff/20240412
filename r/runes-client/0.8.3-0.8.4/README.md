# Comparing `tmp/runes-client-0.8.3.tar.gz` & `tmp/runes-client-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runes-client-0.8.3.tar", last modified: Tue Apr  9 03:35:31 2024, max compression
+gzip compressed data, was "runes-client-0.8.4.tar", last modified: Fri Apr 12 04:41:39 2024, max compression
```

## Comparing `runes-client-0.8.3.tar` & `runes-client-0.8.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.658501 runes-client-0.8.3/
--rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.8.3/LICENSE.md
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-09 03:35:31.658264 runes-client-0.8.3/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5723 2024-04-09 00:18:41.000000 runes-client-0.8.3/README.md
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.654097 runes-client-0.8.3/runes_client/
--rw-r--r--   0 stevehiehn   (501) staff       (20)      616 2024-04-09 00:18:41.000000 runes-client-0.8.3/runes_client/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    11397 2024-04-09 03:13:14.000000 runes-client-0.8.3/runes_client/api_client.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1117 2024-04-09 03:13:14.000000 runes-client-0.8.3/runes_client/config.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    39717 2024-04-09 03:32:39.000000 runes-client-0.8.3/runes_client/core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/decorators.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/dn_tracer.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/file_uploader.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.655796 runes-client-0.8.3/runes_client/output/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/output/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.8.3/runes_client/output/results_handler.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.656508 runes-client-0.8.3/runes_client/utils/
--rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/utils/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/utils/audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.8.3/runes_client/utils/file_type_classifier.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.657968 runes-client-0.8.3/runes_client.egg-info/
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/PKG-INFO
--rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/SOURCES.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/dependency_links.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/entry_points.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/requires.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-09 03:35:31.000000 runes-client-0.8.3/runes_client.egg-info/top_level.txt
--rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-09 03:35:31.658569 runes-client-0.8.3/setup.cfg
--rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-09 03:33:36.000000 runes-client-0.8.3/setup.py
-drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-09 03:35:31.657690 runes-client-0.8.3/tests/
--rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.8.3/tests/__init__.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.8.3/tests/test_audio_utils.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.8.3/tests/test_core.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.8.3/tests/test_registration.py
--rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.8.3/tests/test_results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.994933 runes-client-0.8.4/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    35140 2024-03-13 21:22:47.000000 runes-client-0.8.4/LICENSE.md
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-12 04:41:39.994702 runes-client-0.8.4/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5723 2024-04-09 00:18:41.000000 runes-client-0.8.4/README.md
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.990711 runes-client-0.8.4/runes_client/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      638 2024-04-11 00:04:50.000000 runes-client-0.8.4/runes_client/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    10334 2024-04-12 04:09:34.000000 runes-client-0.8.4/runes_client/api_client.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1193 2024-04-12 01:39:49.000000 runes-client-0.8.4/runes_client/config.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    38166 2024-04-12 04:05:10.000000 runes-client-0.8.4/runes_client/core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      277 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/decorators.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     4446 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/dn_tracer.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1404 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/file_uploader.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.992247 runes-client-0.8.4/runes_client/output/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       63 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/output/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6818 2024-04-08 05:37:47.000000 runes-client-0.8.4/runes_client/output/results_handler.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.993056 runes-client-0.8.4/runes_client/utils/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       61 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/utils/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     3060 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/utils/audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      572 2024-03-13 21:22:47.000000 runes-client-0.8.4/runes_client/utils/file_type_classifier.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.994469 runes-client-0.8.4/runes_client.egg-info/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6262 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/PKG-INFO
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      725 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/SOURCES.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        1 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/dependency_links.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       56 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/entry_points.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       72 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/requires.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       19 2024-04-12 04:41:39.000000 runes-client-0.8.4/runes_client.egg-info/top_level.txt
+-rw-r--r--   0 stevehiehn   (501) staff       (20)       38 2024-04-12 04:41:39.994973 runes-client-0.8.4/setup.cfg
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     1556 2024-04-12 04:40:20.000000 runes-client-0.8.4/setup.py
+drwxr-xr-x   0 stevehiehn   (501) staff       (20)        0 2024-04-12 04:41:39.994246 runes-client-0.8.4/tests/
+-rw-r--r--   0 stevehiehn   (501) staff       (20)        0 2024-03-13 21:22:47.000000 runes-client-0.8.4/tests/__init__.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     5372 2024-03-13 21:50:56.000000 runes-client-0.8.4/tests/test_audio_utils.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)     6956 2024-03-13 21:50:43.000000 runes-client-0.8.4/tests/test_core.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)    13164 2024-04-09 00:18:41.000000 runes-client-0.8.4/tests/test_registration.py
+-rw-r--r--   0 stevehiehn   (501) staff       (20)      683 2024-03-13 21:50:56.000000 runes-client-0.8.4/tests/test_results_handler.py
```

### Comparing `runes-client-0.8.3/LICENSE.md` & `runes-client-0.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/PKG-INFO` & `runes-client-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://dawnet.tools
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `runes-client-0.8.3/README.md` & `runes-client-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client/__init__.py` & `runes-client-0.8.4/runes_client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .core import (
     connect_to_server,
     register_method,
+    register_imports,
     set_token,
     set_author,
     set_name,
     set_description,
     set_version,
     set_input_target_format,
     set_input_target_channels,
```

### Comparing `runes-client-0.8.3/runes_client/api_client.py` & `runes-client-0.8.4/runes_client/api_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from urllib.parse import urljoin
 
 import aiohttp
 
 from .config import (
     API_BASE_URL,
     URL_UPDATE_CONNECTION_STATUS,
+    URL_UPDATE_CONNECTION_LOADED_STATUS,
     URL_CREATE_COMPUTE_CONTRACT,
     URL_ADD_CONNECTION_MAPPING,
     URL_GET_PENDING_MESSAGES,
     URL_UPDATE_MESSAGE_STATUS,
     URL_SEND_MESSAGE_RESPONSE,
 )
 
@@ -138,55 +139,40 @@
                         return None
 
                     # Try parsing the response to JSON
                     data = await response.json()
 
                     return data
 
-                    # print('LATEST_PENDING_MESSAGES: ', str(data))
-
-                    # Loop through the connections and send the message to each one
-                    # for record in data:
-                    #     print("ID: ", record["id"])
-                    #     print("TOKEN: ", record["token"])
-                    #     print("REQUEST: ", record["request"])
-                    #     try:
-                    #         result = await connection_manager.send_message_to_token(
-                    #             token=record["token"],
-                    #             message_id=record["id"],
-                    #             message=record["request"],
-                    #         )
-                    #
-                    #         print("RESULT: " + str(result))
-                    #
-                    #         if result is True:
-                    #             await update_message_status(
-                    #                 token=record["token"],
-                    #                 message_id=record["id"],
-                    #                 new_status="processing",
-                    #             )
-                    #         else:
-                    #             await update_message_status(
-                    #                 token=record["token"],
-                    #                 message_id=record["id"],
-                    #                 new_status="error",
-                    #             )
-                    #     except Exception as e:
-                    #         await update_message_status(
-                    #             token=record["token"],
-                    #             message_id=record["id"],
-                    #             new_status="error",
-                    #         )
-                    #         print(
-                    #             f"Unexpected error during the forwarding of a pending request: {e}"
-                    #         )
-
             except Exception as e:
                 print(f"Unexpected error during check_connection_statuses: {e}")
 
+    async def update_connection_loaded_status(
+        self, connection_token: str, loaded: bool
+    ) -> bool:
+        update_url = urljoin(
+            API_BASE_URL,
+            URL_UPDATE_CONNECTION_LOADED_STATUS.format(token=connection_token),
+        )
+
+        data = {"loaded": loaded}
+
+        async with aiohttp.ClientSession() as session:
+            async with session.put(update_url, json=data) as response:
+                if response.status != 200:
+                    logging.info(
+                        f"Error updating status for client_id: {connection_token}."
+                    )
+                    return False
+                else:
+                    logging.info(
+                        f"Successfully updated status for client_id: {connection_token}"
+                    )
+                    return True
+
     async def update_message_status(self, token: str, message_id: str, new_status: str):
         print(f"UPDATING MESSAGE STATUS for id {message_id}")
         update_url = urljoin(
             API_BASE_URL,
             URL_UPDATE_MESSAGE_STATUS.format(token=token, message_id=message_id),
         )
         payload = {"status": new_status}
```

### Comparing `runes-client-0.8.3/runes_client/config.py` & `runes-client-0.8.4/runes_client/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 SOCKET_PORT = os.getenv("DN_CLIENT_SOCKET_PORT", "8765")
 STORAGE_BUCKET_PATH = os.getenv(
     "DN_CLIENT_STORAGE_BUCKET", "https://storage.googleapis.com/byoc-file-transfer/"
 )
 
 # API URLs
 URL_UPDATE_CONNECTION_STATUS = "api/hub/connection/compute/{token}/{connection_status}/"
+URL_UPDATE_CONNECTION_LOADED_STATUS = "api/hub/connections/{token}/loaded/"
 URL_GET_CONNECTIONS = "api/hub/connections/{token}/"
 URL_ADD_CONNECTION_MAPPING = "api/hub/connection_mappings/"
 URL_CREATE_COMPUTE_CONTRACT = "api/hub/compute/contract/"
 URL_GET_COMPUTE_CONTRACT = "api/hub/compute/contract/{token}/"
 URL_GET_PENDING_MESSAGES = "api/hub/get_latest_pending_messages/{connection_token}/"
 URL_UPDATE_MESSAGE_STATUS = "api/hub/update_message_status/{token}/{message_id}/"
 URL_SEND_MESSAGE_RESPONSE = "api/hub/reply_to_message/"
```

### Comparing `runes-client-0.8.3/runes_client/core.py` & `runes-client-0.8.4/runes_client/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import io
 import sys
+import threading
 import uuid
 
 import websockets
 import nest_asyncio
 import json
 import logging
 import os
@@ -33,14 +34,17 @@
 
 run_status = RunStatus()
 
 # Method registry for the client
 method_registry_local = {}
 method_details_local = {}
 
+# This is hold the registered imports function provided by the user
+registered_imports_func = None
+
 
 class WebSocketClient:
     def __init__(self, server_ip, server_port):
         self.api_client = APIClient(API_BASE_URL)
         self.server_ip = server_ip
         self.server_port = server_port
         self.websocket = None
@@ -75,91 +79,57 @@
         self.daw_sample_rate = 0
 
         # Check if DN_CLIENT_TOKEN environment variable is set and non-empty
         dn_client_token = os.getenv("DN_CLIENT_TOKEN")
         if dn_client_token:
             self.master_token = dn_client_token
 
+    async def initialize_dependencies(self):
+        await self.api_client.update_connection_loaded_status(
+            self.connection_token, False
+        )
+        print("INSTALLING DEPENDENCIES - START")
+
+        if registered_imports_func is not None:
+            await registered_imports_func()
+
+        await self.api_client.update_connection_loaded_status(
+            self.connection_token, True
+        )
+        print("INSTALLING DEPENDENCIES - COMPLETE")
+
     async def send_registered_methods_to_server(self):
         if self.connection_token is None:
             raise Exception(
                 "Token not set. Please call set_token(token) before calling send_registered_methods_to_server()."
             )
 
         if self.master_token is None:
             raise Exception(
                 "Master Token not set. Please call set_token(token) before calling send_registered_methods_to_server()."
             )
 
-        # await self.connect()  # Ensure we're connected
-
-        # Check if there's at least one method registered
+        # FIRST REGISTER THE METHOD
         if self.method_registry:
-            # Get the last registered method's name and details
             last_method_name, last_method = next(reversed(self.method_registry.items()))
             last_method_details = self.method_details[last_method_name]
 
-            # Construct the message to register the method
-            # register_compute_contract_msg = {
-            #     "token": self.connection_token,
-            #     "type": "contract",
-            #     "data": last_method_details,
-            # }
-
             await self.api_client.create_compute_contract(
                 token=self.connection_token, data=last_method_details
             )
 
             await self.api_client.add_connection_mapping(
                 master_token=self.master_token,
                 connection_token=self.connection_token,
                 name=self.name,
                 description=self.description,
             )
 
-            # Send the registration message to the server
-            # await self.websocket.send(json.dumps(register_compute_contract_msg))
-            # self.dn_tracer.log_event(
-            #     self.connection_token,
-            #     {
-            #         DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_CONTRACT.value,
-            #         DNTag.DNMsg.value: f"Sent contract for registration. Token: {self.connection_token}",
-            #     },
-            # )
-
-    # async def connect(self):
-    #     if self.websocket is None or self.websocket.closed:
-    #         uri = f"ws://{self.server_ip}:{self.server_port}"
-    #         self.websocket = await websockets.connect(uri)
-    #         self.dn_tracer.log_event(
-    #             self.connection_token,
-    #             {
-    #                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-    #                 DNTag.DNMsg.value: f"Connected to {uri}",
-    #             },
-    #         )
-    #         self.results = ResultsHandler(
-    #             websocket=self.websocket,
-    #             token=self.connection_token,
-    #             target_sample_rate=self.output_sample_rate,
-    #             target_bit_depth=self.output_bit_depth,
-    #             target_channels=self.output_channels,
-    #             target_format=self.output_format,
-    #         )
-    #
-    #     try:
-    #         await self.register_compute_instance()
-    #     except Exception as e:
-    #         self.dn_tracer.log_error(
-    #             self.connection_token,
-    #             {
-    #                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_CONNECTION.value,
-    #                 DNTag.DNMsg.value: f"Error connecting. {e}",
-    #             },
-    #         )
+        # NOW INSTALL THE IMPORTS/DEPENDENCIES
+        await self.initialize_dependencies()
 
     async def register_compute_instance(self):
         if self.connection_token is None:
             raise Exception(
                 "Token not set. Please call set_token(token) before registering a method."
             )
 
@@ -855,14 +825,19 @@
             {
                 DNTag.DNMsgStage.value: DNMsgStage.CLIENT_REG_METHOD.value,
                 DNTag.DNMsg.value: f"Error registering method: {e}",
             },
         )
 
 
+def register_imports(func):
+    global registered_imports_func
+    registered_imports_func = func
+
+
 def set_author(author: str):
     _client.set_author(author)
 
 
 def set_name(name: str):
     _client.set_name(name)
 
@@ -983,33 +958,34 @@
     return _client.daw_bpm
 
 
 def get_daw_sample_rate():
     return _client.daw_sample_rate
 
 
+def run_heartbeat():
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    try:
+        loop.run_until_complete(_client.heartbeat())
+    finally:
+        loop.close()
+
+
 async def async_main():
-    # Initialize your async tasks here
-    task1 = asyncio.create_task(_client.heartbeat())
-    task2 = asyncio.create_task(_client.poll_updates())
+    thread = threading.Thread(target=run_heartbeat)
+    thread.start()
 
-    await _client.send_registered_methods_to_server()
-    # await _client.add_connection_mapping()
-    # await _client.listen()
+    task1 = asyncio.create_task(_client.send_registered_methods_to_server())
+    task2 = asyncio.create_task(_client.poll_updates())
 
-    # If you want to run indefinitely, you can remove the 'await asyncio.gather(...)' line
-    # and just do 'await asyncio.sleep(1e9)' or something similar.
     await asyncio.gather(task1, task2)
 
 
 def connect_to_server():
-    # asyncio.run(_client.send_registered_methods_to_server())
-    # asyncio.run(_client.listen())
-
-    # Setup the asyncio event loop
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
     try:
         # Run the async main function within the event loop
         loop.run_until_complete(async_main())
     finally:
         # Close the loop when done
```

### Comparing `runes-client-0.8.3/runes_client/dn_tracer.py` & `runes-client-0.8.4/runes_client/dn_tracer.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client/file_uploader.py` & `runes-client-0.8.4/runes_client/file_uploader.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client/output/results_handler.py` & `runes-client-0.8.4/runes_client/output/results_handler.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client/utils/audio_utils.py` & `runes-client-0.8.4/runes_client/utils/audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client/utils/file_type_classifier.py` & `runes-client-0.8.4/runes_client/utils/file_type_classifier.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/runes_client.egg-info/PKG-INFO` & `runes-client-0.8.4/runes_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runes-client
-Version: 0.8.3
+Version: 0.8.4
 Summary: Runes client enables remote execution of python code triggered from a Crucible Plugin on the Signals & Sorcery platform.
 Home-page: https://dawnet.tools
 Author: Steve Hiehn
 Author-email: stevehiehn@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `runes-client-0.8.3/runes_client.egg-info/SOURCES.txt` & `runes-client-0.8.4/runes_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/setup.py` & `runes-client-0.8.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 if not is_ffmpeg_installed():
     print(ffmpeg_warning_msg)
 
 setup(
     name="runes-client",
-    version="0.8.3",
+    version="0.8.4",
     packages=find_packages(),
     install_requires=[
         "aiohttp",
         "websockets",
         "nest-asyncio",
         "sentry-sdk",
         "pydub",
```

### Comparing `runes-client-0.8.3/tests/test_audio_utils.py` & `runes-client-0.8.4/tests/test_audio_utils.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/tests/test_core.py` & `runes-client-0.8.4/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/tests/test_registration.py` & `runes-client-0.8.4/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `runes-client-0.8.3/tests/test_results_handler.py` & `runes-client-0.8.4/tests/test_results_handler.py`

 * *Files identical despite different names*

