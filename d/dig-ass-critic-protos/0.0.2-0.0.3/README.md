# Comparing `tmp/dig_ass_critic_protos-0.0.2.tar.gz` & `tmp/dig_ass_critic_protos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_critic_protos-0.0.2.tar", last modified: Fri Apr 12 13:30:02 2024, max compression
+gzip compressed data, was "dig_ass_critic_protos-0.0.3.tar", last modified: Fri Apr 12 20:31:47 2024, max compression
```

## Comparing `dig_ass_critic_protos-0.0.2.tar` & `dig_ass_critic_protos-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-0.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2789 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2378 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-04-12 13:30:00.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:26:35.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1411 2024-04-12 13:12:17.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      499 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:30:02.000000 dig_ass_critic_protos-0.0.2/dig_ass_critic_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:30:02.329100 dig_ass_critic_protos-0.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-04-11 10:26:57.000000 dig_ass_critic_protos-0.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:47.975578 dig_ass_critic_protos-0.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 20:31:47.975578 dig_ass_critic_protos-0.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:31.000000 dig_ass_critic_protos-0.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:47.975578 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2789 2024-04-12 20:31:46.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2378 2024-04-12 20:31:46.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3010 2024-04-12 20:31:46.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 20:28:20.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:20.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      788 2024-04-12 20:28:20.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:47.975578 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      339 2024-04-12 20:31:47.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      540 2024-04-12 20:31:47.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 20:31:47.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 20:31:47.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 20:31:47.000000 dig_ass_critic_protos-0.0.3/dig_ass_critic_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_critic_protos-0.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 20:31:47.975578 dig_ass_critic_protos-0.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      809 2024-04-11 10:26:57.000000 dig_ass_critic_protos-0.0.3/setup.py
```

### Comparing `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py` & `dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi` & `dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-0.0.2/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py` & `dig_ass_critic_protos-0.0.3/dig_ass_critic_protos/DigitalAssistantCritic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_critic_protos-0.0.2/setup.py` & `dig_ass_critic_protos-0.0.3/setup.py`

 * *Files identical despite different names*

