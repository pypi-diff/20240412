# Comparing `tmp/alibabacloud_tingwu20230930_py2-2.0.7.tar.gz` & `tmp/alibabacloud_tingwu20230930_py2-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_tingwu20230930_py2-2.0.7.tar", last modified: Wed Apr 10 17:10:54 2024, max compression
+gzip compressed data, was "dist/alibabacloud_tingwu20230930_py2-2.0.8.tar", last modified: Fri Apr 12 03:56:31 2024, max compression
```

## Comparing `alibabacloud_tingwu20230930_py2-2.0.7.tar` & `alibabacloud_tingwu20230930_py2-2.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/
--rw-r--r--   0 root         (0) root         (0)      954 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9485 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/client.py
--rw-r--r--   0 root         (0) root         (0)    53082 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2490 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2918 2024-04-10 17:10:54.000000 alibabacloud_tingwu20230930_py2-2.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9485 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)    54345 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2918 2024-04-12 03:56:31.000000 alibabacloud_tingwu20230930_py2-2.0.8/setup.py
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/ChangeLog.md` & `alibabacloud_tingwu20230930_py2-2.0.8/ChangeLog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-10 Version: 2.0.7
+- Update API GetTaskInfo: update response param.
+
+
 2024-03-18 Version: 2.0.6
 - Update API CreateTask: update param body.
 - Update API CreateTask: update response param.
 
 
 2024-03-15 Version: 2.0.5
 - Update API CreateTask: update param body.
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/LICENSE` & `alibabacloud_tingwu20230930_py2-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/PKG-INFO` & `alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_tingwu20230930_py2
-Version: 2.0.7
+Name: alibabacloud-tingwu20230930-py2
+Version: 2.0.8
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/README-CN.md` & `alibabacloud_tingwu20230930_py2-2.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/README.md` & `alibabacloud_tingwu20230930_py2-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/client.py` & `alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930/models.py` & `alibabacloud_tingwu20230930_py2-2.0.8/alibabacloud_tingwu20230930/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -821,18 +821,22 @@
             self.transcription = m.get('Transcription')
         if m.get('Translation') is not None:
             self.translation = m.get('Translation')
         return self
 
 
 class GetTaskInfoResponseBodyData(TeaModel):
-    def __init__(self, error_code=None, error_message=None, result=None, task_id=None, task_key=None,
-                 task_status=None):
+    def __init__(self, error_code=None, error_message=None, output_mp_3path=None, output_mp_4path=None,
+                 output_spectrum_path=None, output_thumbnail_path=None, result=None, task_id=None, task_key=None, task_status=None):
         self.error_code = error_code  # type: str
         self.error_message = error_message  # type: str
+        self.output_mp_3path = output_mp_3path  # type: str
+        self.output_mp_4path = output_mp_4path  # type: str
+        self.output_spectrum_path = output_spectrum_path  # type: str
+        self.output_thumbnail_path = output_thumbnail_path  # type: str
         self.result = result  # type: GetTaskInfoResponseBodyDataResult
         self.task_id = task_id  # type: str
         self.task_key = task_key  # type: str
         self.task_status = task_status  # type: str
 
     def validate(self):
         if self.result:
@@ -844,14 +848,22 @@
             return _map
 
         result = dict()
         if self.error_code is not None:
             result['ErrorCode'] = self.error_code
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
+        if self.output_mp_3path is not None:
+            result['OutputMp3Path'] = self.output_mp_3path
+        if self.output_mp_4path is not None:
+            result['OutputMp4Path'] = self.output_mp_4path
+        if self.output_spectrum_path is not None:
+            result['OutputSpectrumPath'] = self.output_spectrum_path
+        if self.output_thumbnail_path is not None:
+            result['OutputThumbnailPath'] = self.output_thumbnail_path
         if self.result is not None:
             result['Result'] = self.result.to_map()
         if self.task_id is not None:
             result['TaskId'] = self.task_id
         if self.task_key is not None:
             result['TaskKey'] = self.task_key
         if self.task_status is not None:
@@ -860,14 +872,22 @@
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('ErrorCode') is not None:
             self.error_code = m.get('ErrorCode')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
+        if m.get('OutputMp3Path') is not None:
+            self.output_mp_3path = m.get('OutputMp3Path')
+        if m.get('OutputMp4Path') is not None:
+            self.output_mp_4path = m.get('OutputMp4Path')
+        if m.get('OutputSpectrumPath') is not None:
+            self.output_spectrum_path = m.get('OutputSpectrumPath')
+        if m.get('OutputThumbnailPath') is not None:
+            self.output_thumbnail_path = m.get('OutputThumbnailPath')
         if m.get('Result') is not None:
             temp_model = GetTaskInfoResponseBodyDataResult()
             self.result = temp_model.from_map(m['Result'])
         if m.get('TaskId') is not None:
             self.task_id = m.get('TaskId')
         if m.get('TaskKey') is not None:
             self.task_key = m.get('TaskKey')
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/alibabacloud_tingwu20230930_py2.egg-info/PKG-INFO` & `alibabacloud_tingwu20230930_py2-2.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-tingwu20230930-py2
-Version: 2.0.7
+Name: alibabacloud_tingwu20230930_py2
+Version: 2.0.8
 Summary: Alibaba Cloud tingwu (20230930) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_tingwu20230930_py2-2.0.7/setup.py` & `alibabacloud_tingwu20230930_py2-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_tingwu20230930_py2.
 
-Created on 10/04/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_tingwu20230930"
 NAME = "alibabacloud_tingwu20230930_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud tingwu (20230930) SDK Library for Python2"
```

