# Comparing `tmp/alibabacloud_pai-dsw20220101-1.2.0.tar.gz` & `tmp/alibabacloud_pai-dsw20220101-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dsw20220101-1.2.0.tar", last modified: Thu Feb 22 09:17:20 2024, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dsw20220101-1.3.0.tar", last modified: Fri Apr 12 17:12:49 2024, max compression
```

## Comparing `alibabacloud_pai-dsw20220101-1.2.0.tar` & `alibabacloud_pai-dsw20220101-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1690 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2429 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85831 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   217576 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2429 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-22 09:17:20.000000 alibabacloud_pai-dsw20220101-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2633 2024-02-22 09:17:19.000000 alibabacloud_pai-dsw20220101-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1751 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85831 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   219637 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-12 17:12:49.000000 alibabacloud_pai-dsw20220101-1.3.0/setup.py
```

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/ChangeLog.md` & `alibabacloud_pai-dsw20220101-1.3.0/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-02-22 Version: 1.2.0
+- Support API GetInstanceEvents.
+
+
 2024-01-09 Version: 1.1.45
 - Generated python 2022-01-01 for pai-dsw.
 
 2023-12-27 Version: 1.1.44
 - Generated python 2022-01-01 for pai-dsw.
 
 2023-08-21 Version: 1.1.43
```

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/LICENSE` & `alibabacloud_pai-dsw20220101-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/PKG-INFO` & `alibabacloud_pai-dsw20220101-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dsw20220101
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud pai-dsw (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/README-CN.md` & `alibabacloud_pai-dsw20220101-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/README.md` & `alibabacloud_pai-dsw20220101-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/client.py` & `alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101/models.py` & `alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2165,14 +2165,53 @@
         if m.get('RepositoryUrl') is not None:
             self.repository_url = m.get('RepositoryUrl')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
+class GetInstanceResponseBodyNodeErrorRecovery(TeaModel):
+    def __init__(
+        self,
+        auto_switch_countdown_seconds: int = None,
+        enable_auto_switch_on_node_error: bool = None,
+        has_node_error: bool = None,
+    ):
+        self.auto_switch_countdown_seconds = auto_switch_countdown_seconds
+        self.enable_auto_switch_on_node_error = enable_auto_switch_on_node_error
+        self.has_node_error = has_node_error
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auto_switch_countdown_seconds is not None:
+            result['autoSwitchCountdownSeconds'] = self.auto_switch_countdown_seconds
+        if self.enable_auto_switch_on_node_error is not None:
+            result['enableAutoSwitchOnNodeError'] = self.enable_auto_switch_on_node_error
+        if self.has_node_error is not None:
+            result['hasNodeError'] = self.has_node_error
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('autoSwitchCountdownSeconds') is not None:
+            self.auto_switch_countdown_seconds = m.get('autoSwitchCountdownSeconds')
+        if m.get('enableAutoSwitchOnNodeError') is not None:
+            self.enable_auto_switch_on_node_error = m.get('enableAutoSwitchOnNodeError')
+        if m.get('hasNodeError') is not None:
+            self.has_node_error = m.get('hasNodeError')
+        return self
+
+
 class GetInstanceResponseBodyRequestedResource(TeaModel):
     def __init__(
         self,
         cpu: str = None,
         gpu: str = None,
         gputype: str = None,
         memory: str = None,
@@ -2310,14 +2349,15 @@
         instance_shutdown_timer: GetInstanceResponseBodyInstanceShutdownTimer = None,
         instance_snapshot_list: List[GetInstanceResponseBodyInstanceSnapshotList] = None,
         instance_url: str = None,
         jupyterlab_url: str = None,
         labels: List[GetInstanceResponseBodyLabels] = None,
         latest_snapshot: GetInstanceResponseBodyLatestSnapshot = None,
         message: str = None,
+        node_error_recovery: GetInstanceResponseBodyNodeErrorRecovery = None,
         payment_type: str = None,
         priority: int = None,
         reason_code: str = None,
         reason_message: str = None,
         request_id: str = None,
         requested_resource: GetInstanceResponseBodyRequestedResource = None,
         resource_id: str = None,
@@ -2355,14 +2395,15 @@
         self.instance_snapshot_list = instance_snapshot_list
         self.instance_url = instance_url
         # Jupyterlab Url。
         self.jupyterlab_url = jupyterlab_url
         self.labels = labels
         self.latest_snapshot = latest_snapshot
         self.message = message
+        self.node_error_recovery = node_error_recovery
         self.payment_type = payment_type
         self.priority = priority
         self.reason_code = reason_code
         self.reason_message = reason_message
         self.request_id = request_id
         self.requested_resource = requested_resource
         self.resource_id = resource_id
@@ -2398,14 +2439,16 @@
                     k.validate()
         if self.labels:
             for k in self.labels:
                 if k:
                     k.validate()
         if self.latest_snapshot:
             self.latest_snapshot.validate()
+        if self.node_error_recovery:
+            self.node_error_recovery.validate()
         if self.requested_resource:
             self.requested_resource.validate()
         if self.user_vpc:
             self.user_vpc.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -2467,14 +2510,16 @@
         if self.labels is not None:
             for k in self.labels:
                 result['Labels'].append(k.to_map() if k else None)
         if self.latest_snapshot is not None:
             result['LatestSnapshot'] = self.latest_snapshot.to_map()
         if self.message is not None:
             result['Message'] = self.message
+        if self.node_error_recovery is not None:
+            result['NodeErrorRecovery'] = self.node_error_recovery.to_map()
         if self.payment_type is not None:
             result['PaymentType'] = self.payment_type
         if self.priority is not None:
             result['Priority'] = self.priority
         if self.reason_code is not None:
             result['ReasonCode'] = self.reason_code
         if self.reason_message is not None:
@@ -2572,14 +2617,17 @@
                 temp_model = GetInstanceResponseBodyLabels()
                 self.labels.append(temp_model.from_map(k))
         if m.get('LatestSnapshot') is not None:
             temp_model = GetInstanceResponseBodyLatestSnapshot()
             self.latest_snapshot = temp_model.from_map(m['LatestSnapshot'])
         if m.get('Message') is not None:
             self.message = m.get('Message')
+        if m.get('NodeErrorRecovery') is not None:
+            temp_model = GetInstanceResponseBodyNodeErrorRecovery()
+            self.node_error_recovery = temp_model.from_map(m['NodeErrorRecovery'])
         if m.get('PaymentType') is not None:
             self.payment_type = m.get('PaymentType')
         if m.get('Priority') is not None:
             self.priority = m.get('Priority')
         if m.get('ReasonCode') is not None:
             self.reason_code = m.get('ReasonCode')
         if m.get('ReasonMessage') is not None:
```

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/alibabacloud_pai_dsw20220101.egg-info/PKG-INFO` & `alibabacloud_pai-dsw20220101-1.3.0/alibabacloud_pai_dsw20220101.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dsw20220101
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud pai-dsw (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dsw20220101-1.2.0/setup.py` & `alibabacloud_pai-dsw20220101-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dsw20220101.
 
-Created on 22/02/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dsw20220101"
 NAME = "alibabacloud_pai-dsw20220101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dsw (20220101) SDK Library for Python"
```

