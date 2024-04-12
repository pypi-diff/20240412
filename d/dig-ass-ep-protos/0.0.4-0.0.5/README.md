# Comparing `tmp/dig_ass_ep_protos-0.0.4.tar.gz` & `tmp/dig_ass_ep_protos-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-0.0.4.tar", last modified: Fri Apr 12 11:56:34 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-0.0.5.tar", last modified: Fri Apr 12 20:31:54 2024, max compression
```

## Comparing `dig_ass_ep_protos-0.0.4.tar` & `dig_ass_ep_protos-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.4/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.4/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-12 11:56:33.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 11:55:22.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1612 2024-04-12 11:54:30.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      471 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-12 11:56:34.000000 dig_ass_ep_protos-0.0.4/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.4/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 11:56:34.571168 dig_ass_ep_protos-0.0.4/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.4/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:54.603670 dig_ass_ep_protos-0.0.5/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.5/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 20:31:54.603670 dig_ass_ep_protos-0.0.5/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.5/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:54.599670 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-12 20:31:53.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-12 20:31:53.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-12 20:31:53.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      936 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:31:54.603670 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-12 20:31:54.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-04-12 20:31:54.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 20:31:54.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 20:31:54.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-12 20:31:54.000000 dig_ass_ep_protos-0.0.5/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.5/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 20:31:54.603670 dig_ass_ep_protos-0.0.5/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.5/setup.py
```

### Comparing `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.4/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-0.0.5/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ep_protos-0.0.4/setup.py` & `dig_ass_ep_protos-0.0.5/setup.py`

 * *Files identical despite different names*

