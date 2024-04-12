# Comparing `tmp/dig_ass_ep_protos-0.0.3.tar.gz` & `tmp/dig_ass_ep_protos-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-0.0.3.tar", last modified: Wed Apr 10 14:31:02 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-0.0.4.tar", last modified: Fri Apr 12 11:56:34 2024, max compression
```

## Comparing `dig_ass_ep_protos-0.0.3.tar` & `dig_ass_ep_protos-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:31:02.124027 dig_ass_ep_protos-0.0.3/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.3/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 14:31:02.124027 dig_ass_ep_protos-0.0.3/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.3/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:31:02.124027 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2171 2024-04-10 14:31:00.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-10 14:31:00.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-10 14:31:00.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-10 14:30:20.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1161 2024-04-10 14:30:14.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-10 14:31:02.124027 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-10 14:31:02.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      471 2024-04-10 14:31:02.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-10 14:31:02.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-10 14:31:02.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-10 14:31:02.000000 dig_ass_ep_protos-0.0.3/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.3/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-10 14:31:02.124027 dig_ass_ep_protos-0.0.3/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      793 2024-04-10 09:02:25.000000 dig_ass_ep_protos-0.0.3/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.4/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.4/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 11:55:22.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1612 2024-04-12 11:54:30.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      471 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.4/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.4/setup.py
```

### Comparing `dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\x05\x32\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r2\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTENTRYPOINTRESPONSE']._serialized_start=69
```

### Comparing `dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.3/dig_ass_ep_protos/client.py` & `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 from grpc import insecure_channel
+from google.protobuf.json_format import MessageToDict, ParseDict
 from dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2_grpc import DigitalAssistantEntryPointStub
 from dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2 import DigitalAssistantEntryPointRequest, DigitalAssistantEntryPointResponse, OuterContextItem
 
 
 class EntryPointClient:
 
     def __init__(self, address: str) -> None:
         self._channel = insecure_channel(address)
         self._stub = DigitalAssistantEntryPointStub(self._channel)
 
-    def get_stub(self):
-        return self._stub
+    def __call__(self, text: str, outerContextDict: dict, image: bytearray, pdf: bytearray):
 
-    def __call__(self, text: str, image: bytearray, pdf: bytearray, sex: bool, age: int, userId: int, sessionId: int):
+        request = dict2Message(text, outerContextDict, image, pdf)
+        response: DigitalAssistantEntryPointResponse = self._stub.GetTextResponse(request)
+        responseDict = message2Dict(response)
 
-        outerContext = OuterContextItem(Sex=sex, Age=age, UserId=userId, SessionId=sessionId)
-        request = DigitalAssistantEntryPointRequest(Text=text, OuterContext=outerContext, Image=image, PDF=pdf)
-        response: DigitalAssistantEntryPointResponse = self.get_stub().GetTextResponse(request)
-
-        return response.Text
+        return responseDict["Text"]
 
     # https://stackoverflow.com/a/65131927
     def close(self):
         self._channel.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self):
         self.close()
+
+
+def dict2Message(text: str, outerContextDict: dict, image: bytearray, pdf: bytearray) -> DigitalAssistantEntryPointRequest:
+
+    messageDict = {"Text": text, "OuterContext": outerContextDict, "Image": image, "PDF": pdf}
+    message = ParseDict(messageDict, DigitalAssistantEntryPointRequest())
+    return message
+
+
+def message2Dict(message: DigitalAssistantEntryPointResponse) -> dict:
+
+    messageDict = MessageToDict(message, preserving_proto_field_name=True, use_integers_for_enums=False, including_default_value_fields=True)
+    return messageDict
```

