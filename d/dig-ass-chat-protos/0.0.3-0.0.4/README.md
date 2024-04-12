# Comparing `tmp/dig_ass_chat_protos-0.0.3.tar.gz` & `tmp/dig_ass_chat_protos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.3.tar", last modified: Thu Apr 11 15:05:08 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-0.0.4.tar", last modified: Fri Apr 12 13:29:54 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.3.tar` & `dig_ass_chat_protos-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.601100 dig_ass_chat_protos-0.0.3/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.3/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.3/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2033 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1259 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-11 15:04:43.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1620 2024-04-11 15:03:18.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.3/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 15:05:08.601100 dig_ass_chat_protos-0.0.3/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.3/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.4/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.4/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 13:29:53.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 12:31:05.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1445 2024-04-12 13:11:04.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      494 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:29:54.000000 dig_ass_chat_protos-0.0.4/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.4/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:29:54.696961 dig_ass_chat_protos-0.0.4/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.4/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.py` & `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: dig_ass_chat_protos/DigitalAssistantChat.proto
+# source: dig_ass_chat_protos/DigitalAssistantChatManager.proto
 # Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.dig_ass_chat_protos/DigitalAssistantChat.proto\x12\x0f\x64ig.ass.text.v1\",\n\x1c\x44igitalAssistantChatResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"d\n\x1b\x44igitalAssistantChatRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x37\n\x0cOuterContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\x05\x12\x0e\n\x06UserId\x18\x03 \x01(\x05\x12\x11\n\tSessionId\x18\x04 \x01(\x05\x32\x86\x01\n\x14\x44igitalAssistantChat\x12n\n\x0fGetTextResponse\x12,.dig.ass.text.v1.DigitalAssistantChatRequest\x1a-.dig.ass.text.v1.DigitalAssistantChatResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5dig_ass_chat_protos/DigitalAssistantChatManager.proto\x12\x0f\x64ig.ass.text.v1\"3\n#DigitalAssistantChatManagerResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"k\n\"DigitalAssistantChatManagerRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x37\n\x0cOuterContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r2\x9b\x01\n\x1b\x44igitalAssistantChatManager\x12|\n\x0fGetTextResponse\x12\x33.dig.ass.text.v1.DigitalAssistantChatManagerRequest\x1a\x34.dig.ass.text.v1.DigitalAssistantChatManagerResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_chat_protos.DigitalAssistantChat_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_chat_protos.DigitalAssistantChatManager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_DIGITALASSISTANTCHATRESPONSE']._serialized_start=67
-  _globals['_DIGITALASSISTANTCHATRESPONSE']._serialized_end=111
-  _globals['_DIGITALASSISTANTCHATREQUEST']._serialized_start=113
-  _globals['_DIGITALASSISTANTCHATREQUEST']._serialized_end=213
-  _globals['_OUTERCONTEXTITEM']._serialized_start=215
-  _globals['_OUTERCONTEXTITEM']._serialized_end=294
-  _globals['_DIGITALASSISTANTCHAT']._serialized_start=297
-  _globals['_DIGITALASSISTANTCHAT']._serialized_end=431
+  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_start=74
+  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_end=125
+  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_start=127
+  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_end=234
+  _globals['_OUTERCONTEXTITEM']._serialized_start=236
+  _globals['_OUTERCONTEXTITEM']._serialized_end=315
+  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_start=318
+  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_end=473
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi` & `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class DigitalAssistantChatResponse(_message.Message):
+class DigitalAssistantChatManagerResponse(_message.Message):
     __slots__ = ("Text",)
     TEXT_FIELD_NUMBER: _ClassVar[int]
     Text: str
     def __init__(self, Text: _Optional[str] = ...) -> None: ...
 
-class DigitalAssistantChatRequest(_message.Message):
+class DigitalAssistantChatManagerRequest(_message.Message):
     __slots__ = ("Text", "OuterContext")
     TEXT_FIELD_NUMBER: _ClassVar[int]
     OUTERCONTEXT_FIELD_NUMBER: _ClassVar[int]
     Text: str
     OuterContext: OuterContextItem
     def __init__(self, Text: _Optional[str] = ..., OuterContext: _Optional[_Union[OuterContextItem, _Mapping]] = ...) -> None: ...
```

### Comparing `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py` & `dig_ass_chat_protos-0.0.4/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from dig_ass_chat_protos import DigitalAssistantChat_pb2 as dig__ass__chat__protos_dot_DigitalAssistantChat__pb2
+from dig_ass_chat_protos import DigitalAssistantChatManager_pb2 as dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2
 
 
-class DigitalAssistantChatStub(object):
+class DigitalAssistantChatManagerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetTextResponse = channel.unary_unary(
-                '/dig.ass.text.v1.DigitalAssistantChat/GetTextResponse',
-                request_serializer=dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatRequest.SerializeToString,
-                response_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatResponse.FromString,
+                '/dig.ass.text.v1.DigitalAssistantChatManager/GetTextResponse',
+                request_serializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.SerializeToString,
+                response_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.FromString,
                 )
 
 
-class DigitalAssistantChatServicer(object):
+class DigitalAssistantChatManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetTextResponse(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_DigitalAssistantChatServicer_to_server(servicer, server):
+def add_DigitalAssistantChatManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetTextResponse': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTextResponse,
-                    request_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatRequest.FromString,
-                    response_serializer=dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatResponse.SerializeToString,
+                    request_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.FromString,
+                    response_serializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'dig.ass.text.v1.DigitalAssistantChat', rpc_method_handlers)
+            'dig.ass.text.v1.DigitalAssistantChatManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class DigitalAssistantChat(object):
+class DigitalAssistantChatManager(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def GetTextResponse(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/dig.ass.text.v1.DigitalAssistantChat/GetTextResponse',
-            dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatRequest.SerializeToString,
-            dig__ass__chat__protos_dot_DigitalAssistantChat__pb2.DigitalAssistantChatResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/dig.ass.text.v1.DigitalAssistantChatManager/GetTextResponse',
+            dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.SerializeToString,
+            dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dig_ass_chat_protos-0.0.3/setup.py` & `dig_ass_chat_protos-0.0.4/setup.py`

 * *Files identical despite different names*

