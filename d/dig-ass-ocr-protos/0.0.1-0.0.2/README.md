# Comparing `tmp/dig_ass_ocr_protos-0.0.1.tar.gz` & `tmp/dig_ass_ocr_protos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ocr_protos-0.0.1.tar", last modified: Thu Apr 11 10:45:13 2024, max compression
+gzip compressed data, was "dig_ass_ocr_protos-0.0.2.tar", last modified: Fri Apr 12 20:32:01 2024, max compression
```

## Comparing `dig_ass_ocr_protos-0.0.1.tar` & `dig_ass_ocr_protos-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 10:45:13.538446 dig_ass_ocr_protos-0.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-11 10:45:13.538446 dig_ass_ocr_protos-0.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 10:45:13.538446 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1689 2024-04-11 10:45:12.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-04-11 10:45:12.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2917 2024-04-11 10:45:12.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      832 2024-04-11 10:42:44.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-11 10:45:13.538446 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-11 10:45:13.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      460 2024-04-11 10:45:13.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-11 10:45:13.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:45:13.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-04-11 10:45:13.000000 dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-11 10:45:13.538446 dig_ass_ocr_protos-0.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-04-11 10:26:57.000000 dig_ass_ocr_protos-0.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:01.271763 dig_ass_ocr_protos-0.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-12 20:32:01.271763 dig_ass_ocr_protos-0.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:44.000000 dig_ass_ocr_protos-0.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:01.271763 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1689 2024-04-12 20:31:59.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      692 2024-04-12 20:31:59.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2917 2024-04-12 20:31:59.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       21 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      647 2024-04-12 20:28:21.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-12 20:32:01.271763 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      333 2024-04-12 20:32:01.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      498 2024-04-12 20:32:01.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-12 20:32:01.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-12 20:32:01.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-04-12 20:32:01.000000 dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_ocr_protos-0.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-12 20:32:01.271763 dig_ass_ocr_protos-0.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      800 2024-04-11 10:26:57.000000 dig_ass_ocr_protos-0.0.2/setup.py
```

### Comparing `dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py` & `dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi` & `dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.1/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py` & `dig_ass_ocr_protos-0.0.2/dig_ass_ocr_protos/DigitalAssistantOCR_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_ocr_protos-0.0.1/setup.py` & `dig_ass_ocr_protos-0.0.2/setup.py`

 * *Files identical despite different names*

