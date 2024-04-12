# Comparing `tmp/dig_ass_critic_protos-0.0.1.tar.gz` & `tmp/dig_ass_critic_protos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_critic_protos-0.0.1.tar", last modified: Thu Apr 11 11:48:20 2024, max compression
+gzip compressed data, was "dig_ass_critic_protos-0.0.2.tar", last modified: Fri Apr 12 13:30:02 2024, max compression
```

## Comparing `dig_ass_critic_protos-0.0.1.tar` & `dig_ass_critic_protos-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 11:48:20.814035 dig_ass_critic_protos-0.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-11 11:48:20.814035 dig_ass_critic_protos-0.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-0.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 11:48:20.814035 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2791 2024-04-11 11:48:19.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2378 2024-04-11 11:48:19.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-04-11 11:48:19.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-04-11 09:58:31.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2239 2024-04-11 11:46:54.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 11:48:20.814035 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-11 11:48:20.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      499 2024-04-11 11:48:20.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 11:48:20.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 11:48:20.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-11 11:48:20.000000 dig_ass_critic_protos-0.0.1/dig_ass_critic_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 11:48:20.814035 dig_ass_critic_protos-0.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-04-11 10:26:57.000000 dig_ass_critic_protos-0.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-0.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2789 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2378 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:26:35.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1411 2024-04-12 13:12:17.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      499 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-04-11 10:26:57.000000 dig_ass_critic_protos-0.0.2/setup.py
```

### Comparing `dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py` & `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_critic_protos/DigitalAssistantCritic.proto\x12\x11\x64ig.ass.critic.v1\"/\n\x1e\x44igitalAssistantCriticResponse\x12\r\n\x05Score\x18\x01 \x01(\x02\"X\n\x1d\x44igitalAssistantCriticRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12)\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x1b.dig.ass.critic.v1.ChatItem\"\x80\x01\n\x08\x43hatItem\x12\x39\n\x0cOuterContext\x18\x01 \x01(\x0b\x32#.dig.ass.critic.v1.OuterContextItem\x12\x39\n\x0cInnerContext\x18\x02 \x01(\x0b\x32#.dig.ass.critic.v1.InnerContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\x05\"D\n\x10InnerContextItem\x12\x30\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1e.dig.ass.critic.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x90\x01\n\x16\x44igitalAssistantCritic\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.critic.v1.DigitalAssistantCriticRequest\x1a\x31.dig.ass.critic.v1.DigitalAssistantCriticResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_critic_protos/DigitalAssistantCritic.proto\x12\x11\x64ig.ass.critic.v1\"/\n\x1e\x44igitalAssistantCriticResponse\x12\r\n\x05Score\x18\x01 \x01(\x02\"X\n\x1d\x44igitalAssistantCriticRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12)\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x1b.dig.ass.critic.v1.ChatItem\"\x80\x01\n\x08\x43hatItem\x12\x39\n\x0cOuterContext\x18\x01 \x01(\x0b\x32#.dig.ass.critic.v1.OuterContextItem\x12\x39\n\x0cInnerContext\x18\x02 \x01(\x0b\x32#.dig.ass.critic.v1.InnerContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r\"D\n\x10InnerContextItem\x12\x30\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1e.dig.ass.critic.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x90\x01\n\x16\x44igitalAssistantCritic\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.critic.v1.DigitalAssistantCriticRequest\x1a\x31.dig.ass.critic.v1.DigitalAssistantCriticResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_critic_protos.DigitalAssistantCritic_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTCRITICRESPONSE']._serialized_start=73
```

### Comparing `dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi` & `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-0.0.1/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py` & `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-0.0.1/setup.py` & `dig_ass_critic_protos-0.0.2/setup.py`

 * *Files identical despite different names*

