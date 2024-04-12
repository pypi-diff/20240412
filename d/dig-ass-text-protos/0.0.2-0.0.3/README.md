# Comparing `tmp/dig_ass_text_protos-0.0.2.tar.gz` & `tmp/dig_ass_text_protos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-0.0.2.tar", last modified: Fri Apr 12 13:30:10 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-0.0.3.tar", last modified: Fri Apr 12 20:32:12 2024, max compression
```

## Comparing `dig_ass_text_protos-0.0.2.tar` & `dig_ass_text_protos-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.317246 dig_ass_text_protos-0.0.2/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.2/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.2/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-12 13:30:09.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 13:13:41.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1384 2024-04-12 13:15:36.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 13:30:10.313246 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      473 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 13:30:10.000000 dig_ass_text_protos-0.0.2/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.2/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 13:30:10.317246 dig_ass_text_protos-0.0.2/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.2/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:12.267915 dig_ass_text_protos-0.0.3/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.3/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 20:32:12.267915 dig_ass_text_protos-0.0.3/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.3/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:12.267915 dig_ass_text_protos-0.0.3/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-12 20:32:10.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-12 20:32:10.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-12 20:32:10.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-12 20:31:23.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      769 2024-04-12 20:28:21.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:12.267915 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-12 20:32:12.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-04-12 20:32:12.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 20:32:12.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 20:32:12.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-12 20:32:12.000000 dig_ass_text_protos-0.0.3/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.3/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 20:32:12.267915 dig_ass_text_protos-0.0.3/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.3/setup.py
```

### Comparing `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-0.0.3/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.2/setup.py` & `dig_ass_text_protos-0.0.3/setup.py`

 * *Files identical despite different names*

