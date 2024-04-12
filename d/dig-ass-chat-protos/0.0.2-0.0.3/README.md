# Comparing `tmp/dig_ass_chat_protos-0.0.2.tar.gz` & `tmp/dig_ass_chat_protos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.2.tar", last modified: Thu Apr 11 14:36:41 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-0.0.3.tar", last modified: Thu Apr 11 15:05:08 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.2.tar` & `dig_ass_chat_protos-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 14:36:41.685233 dig_ass_chat_protos-0.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 14:36:41.685233 dig_ass_chat_protos-0.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 14:36:41.685233 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2033 2024-04-11 14:36:40.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1259 2024-04-11 14:36:40.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-11 14:36:40.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-11 14:35:10.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1517 2024-04-11 14:34:54.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 14:36:41.685233 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 14:36:41.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-11 14:36:41.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 14:36:41.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 14:36:41.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-11 14:36:41.000000 dig_ass_chat_protos-0.0.2/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 14:36:41.685233 dig_ass_chat_protos-0.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.601100 dig_ass_chat_protos-0.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2033 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1259 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-11 15:05:07.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-11 15:04:43.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1620 2024-04-11 15:03:18.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 15:05:08.597100 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-11 15:05:08.000000 dig_ass_chat_protos-0.0.3/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 15:05:08.601100 dig_ass_chat_protos-0.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.3/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2.py` & `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi` & `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py` & `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/DigitalAssistantChat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.2/dig_ass_chat_protos/client.py` & `dig_ass_chat_protos-0.0.3/dig_ass_chat_protos/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,46 +5,47 @@
 
 class ChatClient:
 
     def __init__(self, address: str) -> None:
         self._channel = insecure_channel(address)
         self._stub = DigitalAssistantChatStub(self._channel)
 
-    def __call__(self, requestDict: dict):
+    def __call__(self, text: str, outerContextDict: dict):
 
-        request = packageRequestDict(requestDict)
+        request = packageGRPCRequest(text, outerContextDict)
         response: DigitalAssistantChatResponse = self._stub.GetTextResponse(request)
         return response.Text
 
     # https://stackoverflow.com/a/65131927
     def close(self):
         self._channel.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self):
         self.close()
 
 
-def packageRequestDict(requestDict: dict) -> DigitalAssistantChatRequest:
+def outerContextDict2GRPC(outerContextDict: dict) -> OuterContextItem:
     """
-    requestDict must have the following structure
-    {
-        "text":,
+    outerContextDict must have the following structure
         "outerContext":{
             "sex":,
             "age":,
             "userId":,
             "sessionId"
         }
-    }
     """
 
     # populate outer context
-    outerContextDict = requestDict["outerContext"]
     outerContext = OuterContextItem(Sex=outerContextDict["sex"], Age=outerContextDict["age"], UserId=outerContextDict["userId"], SessionId=outerContextDict["sessionId"])
+    return outerContext
 
-    # populate final request
-    request = DigitalAssistantChatRequest(Text=requestDict["text"], OuterContext=outerContext)
+
+def packageGRPCRequest(text: str, outerContextDict: dict) -> DigitalAssistantChatRequest:
+
+    outerContext = outerContextDict2GRPC(outerContextDict)
+    # populate request
+    request = DigitalAssistantChatRequest(Text=text, OuterContext=outerContext)
 
     return request
```

### Comparing `dig_ass_chat_protos-0.0.2/setup.py` & `dig_ass_chat_protos-0.0.3/setup.py`

 * *Files identical despite different names*

