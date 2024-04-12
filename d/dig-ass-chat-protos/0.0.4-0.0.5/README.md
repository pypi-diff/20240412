# Comparing `tmp/dig_ass_chat_protos-0.0.4.tar.gz` & `tmp/dig_ass_chat_protos-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.4.tar", last modified: Fri Apr 12 13:29:54 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-0.0.5.tar", last modified: Fri Apr 12 13:50:24 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.4.tar` & `dig_ass_chat_protos-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.4/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.4/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 12:31:05.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1445 2024-04-12 13:11:04.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      494 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.4/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.4/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.5/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.5/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:49:44.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1501 2024-04-12 13:49:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      494 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.5/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.5/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py` & `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi` & `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py` & `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/client.py` & `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from grpc import insecure_channel
 from google.protobuf.json_format import MessageToDict, ParseDict
-from dig_ass_chat_protos.DigitalAssistantChatManager_pb2_grpc import DigitalAssistantChatStub
-from dig_ass_chat_protos.DigitalAssistantChatManager_pb2 import DigitalAssistantChatRequest, DigitalAssistantChatResponse
+from dig_ass_chat_protos.DigitalAssistantChatManager_pb2_grpc import DigitalAssistantChatManagerStub
+from dig_ass_chat_protos.DigitalAssistantChatManager_pb2 import DigitalAssistantChatManagerRequest, DigitalAssistantChatManagerResponse
 
 
 class ChatManagerClient:
 
     def __init__(self, address: str) -> None:
         self._channel = insecure_channel(address)
-        self._stub = DigitalAssistantChatStub(self._channel)
+        self._stub = DigitalAssistantChatManagerStub(self._channel)
 
     def __call__(self, text: str, outerContextDict: dict):
 
         request = dict2Message(text, outerContextDict)
-        response: DigitalAssistantChatResponse = self._stub.GetTextResponse(request)
+        response: DigitalAssistantChatManagerResponse = self._stub.GetTextResponse(request)
         responseDict = message2Dict(response)
 
         return responseDict["Text"]
 
     # https://stackoverflow.com/a/65131927
     def close(self):
         self._channel.close()
@@ -25,18 +25,18 @@
     def __enter__(self):
         return self
 
     def __exit__(self):
         self.close()
 
 
-def dict2Message(text: str, outerContextDict: dict) -> DigitalAssistantChatRequest:
+def dict2Message(text: str, outerContextDict: dict) -> DigitalAssistantChatManagerRequest:
 
     messageDict = {"Text": text, "OuterContext": outerContextDict}
-    message = ParseDict(messageDict, DigitalAssistantChatRequest())
+    message = ParseDict(messageDict, DigitalAssistantChatManagerRequest())
     return message
 
 
-def message2Dict(message: DigitalAssistantChatResponse) -> dict:
+def message2Dict(message: DigitalAssistantChatManagerResponse) -> dict:
 
     messageDict = MessageToDict(message, preserving_proto_field_name=True, use_integers_for_enums=False, including_default_value_fields=True)
     return messageDict
```

### Comparing `dig_ass_chat_protos-0.0.4/setup.py` & `dig_ass_chat_protos-0.0.5/setup.py`

 * *Files identical despite different names*

