# Comparing `tmp/dig_ass_chat_protos-0.0.5.tar.gz` & `tmp/dig_ass_chat_protos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.5.tar", last modified: Fri Apr 12 13:50:24 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-0.0.6.tar", last modified: Fri Apr 12 20:31:40 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.5.tar` & `dig_ass_chat_protos-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.5/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.5/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 13:50:22.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:49:44.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1501 2024-04-12 13:49:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      494 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:50:24.000000 dig_ass_chat_protos-0.0.5/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.5/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:50:24.143209 dig_ass_chat_protos-0.0.5/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.5/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:40.387473 dig_ass_chat_protos-0.0.6/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.6/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 20:31:40.387473 dig_ass_chat_protos-0.0.6/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.6/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:40.387473 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-12 20:31:38.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-12 20:31:38.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-12 20:31:38.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      870 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:40.387473 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 20:31:40.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-04-12 20:31:40.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 20:31:40.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 20:31:40.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 20:31:40.000000 dig_ass_chat_protos-0.0.6/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.6/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 20:31:40.387473 dig_ass_chat_protos-0.0.6/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.6/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py` & `dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi` & `dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.5/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py` & `dig_ass_chat_protos-0.0.6/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.5/setup.py` & `dig_ass_chat_protos-0.0.6/setup.py`

 * *Files identical despite different names*

