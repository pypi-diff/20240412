# Comparing `tmp/dig_ass_text_protos-0.0.1.tar.gz` & `tmp/dig_ass_text_protos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-0.0.1.tar", last modified: Thu Apr 11 12:01:55 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-0.0.2.tar", last modified: Fri Apr 12 13:30:10 2024, max compression
```

## Comparing `dig_ass_text_protos-0.0.1.tar` & `dig_ass_text_protos-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 12:01:55.803651 dig_ass_text_protos-0.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 12:01:55.803651 dig_ass_text_protos-0.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 12:01:55.803651 dig_ass_text_protos-0.0.1/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2727 2024-04-11 12:01:54.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-11 12:01:54.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-11 12:01:54.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2217 2024-04-11 12:00:27.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 12:01:55.803651 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-11 12:01:55.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-11 12:01:55.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 12:01:55.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 12:01:55.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-11 12:01:55.000000 dig_ass_text_protos-0.0.1/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 12:01:55.803651 dig_ass_text_protos-0.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.317246 dig_ass_text_protos-0.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:13:41.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1384 2024-04-12 13:15:36.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:30:10.317246 dig_ass_text_protos-0.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.2/setup.py
```

### Comparing `dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.dig_ass_text_protos/DigitalAssistantText.proto\x12\x0f\x64ig.ass.text.v1\",\n\x1c\x44igitalAssistantTextResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"T\n\x1b\x44igitalAssistantTextRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\'\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x19.dig.ass.text.v1.ChatItem\"|\n\x08\x43hatItem\x12\x37\n\x0cOuterContext\x18\x01 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\x12\x37\n\x0cInnerContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.InnerContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\x05\"B\n\x10InnerContextItem\x12.\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1c.dig.ass.text.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x86\x01\n\x14\x44igitalAssistantText\x12n\n\x0fGetTextResponse\x12,.dig.ass.text.v1.DigitalAssistantTextRequest\x1a-.dig.ass.text.v1.DigitalAssistantTextResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.dig_ass_text_protos/DigitalAssistantText.proto\x12\x0f\x64ig.ass.text.v1\",\n\x1c\x44igitalAssistantTextResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"T\n\x1b\x44igitalAssistantTextRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\'\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x19.dig.ass.text.v1.ChatItem\"|\n\x08\x43hatItem\x12\x37\n\x0cOuterContext\x18\x01 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\x12\x37\n\x0cInnerContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.InnerContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r\"B\n\x10InnerContextItem\x12.\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1c.dig.ass.text.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x86\x01\n\x14\x44igitalAssistantText\x12n\n\x0fGetTextResponse\x12,.dig.ass.text.v1.DigitalAssistantTextRequest\x1a-.dig.ass.text.v1.DigitalAssistantTextResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_text_protos.DigitalAssistantText_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTTEXTRESPONSE']._serialized_start=67
```

### Comparing `dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.1/setup.py` & `dig_ass_text_protos-0.0.2/setup.py`

 * *Files identical despite different names*

