# Comparing `tmp/alibabacloud_pai-dsw20220101_py2-1.2.0.tar.gz` & `tmp/alibabacloud_pai-dsw20220101_py2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dsw20220101_py2-1.2.0.tar", last modified: Thu Feb 22 09:16:15 2024, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dsw20220101_py2-1.3.0.tar", last modified: Fri Apr 12 17:16:49 2024, max compression
```

## Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0.tar` & `alibabacloud_pai-dsw20220101_py2-1.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/
--rw-r--r--   0 root         (0) root         (0)      753 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36322 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   218950 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2024-02-22 09:16:15.000000 alibabacloud_pai-dsw20220101_py2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)      814 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36322 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   221044 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:16:49.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-12 17:16:48.000000 alibabacloud_pai-dsw20220101_py2-1.3.0/setup.py
```

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/ChangeLog.md` & `alibabacloud_pai-dsw20220101_py2-1.3.0/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-02-22 Version: 1.2.0
+- Support API GetInstanceEvents.
+
+
 2024-01-09 Version: 1.1.24
 - Generated python2 2022-01-01 for pai-dsw.
 
 2023-12-27 Version: 1.1.23
 - Generated python2 2022-01-01 for pai-dsw.
 
 2023-08-14 Version: 1.1.22
```

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/LICENSE` & `alibabacloud_pai-dsw20220101_py2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/PKG-INFO` & `alibabacloud_pai-dsw20220101_py2-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dsw20220101_py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud pai-dsw (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/README-CN.md` & `alibabacloud_pai-dsw20220101_py2-1.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/README.md` & `alibabacloud_pai-dsw20220101_py2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/client.py` & `alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101/models.py` & `alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1899,14 +1899,49 @@
         if m.get('RepositoryUrl') is not None:
             self.repository_url = m.get('RepositoryUrl')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         return self
 
 
+class GetInstanceResponseBodyNodeErrorRecovery(TeaModel):
+    def __init__(self, auto_switch_countdown_seconds=None, enable_auto_switch_on_node_error=None,
+                 has_node_error=None):
+        self.auto_switch_countdown_seconds = auto_switch_countdown_seconds  # type: long
+        self.enable_auto_switch_on_node_error = enable_auto_switch_on_node_error  # type: bool
+        self.has_node_error = has_node_error  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetInstanceResponseBodyNodeErrorRecovery, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, cpu=None, gpu=None, gputype=None, memory=None, shared_memory=None):
         self.cpu = cpu  # type: str
         self.gpu = gpu  # type: str
         self.gputype = gputype  # type: str
         self.memory = memory  # type: str
         self.shared_memory = shared_memory  # type: str
@@ -2008,15 +2043,15 @@
 
 class GetInstanceResponseBody(TeaModel):
     def __init__(self, accelerator_type=None, accessibility=None, accumulated_running_time_in_ms=None,
                  cloud_disks=None, code=None, datasets=None, driver=None, ecs_spec=None, environment_variables=None,
                  gmt_create_time=None, gmt_modified_time=None, http_status_code=None, idle_instance_culler=None, image_id=None,
                  image_name=None, image_url=None, instance_id=None, instance_name=None, instance_shutdown_timer=None,
                  instance_snapshot_list=None, instance_url=None, jupyterlab_url=None, labels=None, latest_snapshot=None, message=None,
-                 payment_type=None, priority=None, reason_code=None, reason_message=None, request_id=None,
+                 node_error_recovery=None, payment_type=None, priority=None, reason_code=None, reason_message=None, request_id=None,
                  requested_resource=None, resource_id=None, resource_name=None, status=None, success=None, terminal_url=None,
                  user_id=None, user_name=None, user_vpc=None, web_ideurl=None, workspace_id=None, workspace_name=None,
                  workspace_source=None):
         self.accelerator_type = accelerator_type  # type: str
         self.accessibility = accessibility  # type: str
         self.accumulated_running_time_in_ms = accumulated_running_time_in_ms  # type: long
         self.cloud_disks = cloud_disks  # type: list[GetInstanceResponseBodyCloudDisks]
@@ -2038,14 +2073,15 @@
         self.instance_snapshot_list = instance_snapshot_list  # type: list[GetInstanceResponseBodyInstanceSnapshotList]
         self.instance_url = instance_url  # type: str
         # Jupyterlab Url。
         self.jupyterlab_url = jupyterlab_url  # type: str
         self.labels = labels  # type: list[GetInstanceResponseBodyLabels]
         self.latest_snapshot = latest_snapshot  # type: GetInstanceResponseBodyLatestSnapshot
         self.message = message  # type: str
+        self.node_error_recovery = node_error_recovery  # type: GetInstanceResponseBodyNodeErrorRecovery
         self.payment_type = payment_type  # type: str
         self.priority = priority  # type: long
         self.reason_code = reason_code  # type: str
         self.reason_message = reason_message  # type: str
         self.request_id = request_id  # type: str
         self.requested_resource = requested_resource  # type: GetInstanceResponseBodyRequestedResource
         self.resource_id = resource_id  # type: str
@@ -2081,14 +2117,16 @@
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
         _map = super(GetInstanceResponseBody, self).to_map()
@@ -2150,14 +2188,16 @@
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
@@ -2255,14 +2295,17 @@
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

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/alibabacloud_pai_dsw20220101_py2.egg-info/PKG-INFO` & `alibabacloud_pai-dsw20220101_py2-1.3.0/alibabacloud_pai_dsw20220101_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dsw20220101-py2
-Version: 1.2.0
+Version: 1.3.0
 Summary: Alibaba Cloud pai-dsw (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dsw20220101_py2-1.2.0/setup.py` & `alibabacloud_pai-dsw20220101_py2-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dsw20220101_py2.
 
-Created on 22/02/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dsw20220101"
 NAME = "alibabacloud_pai-dsw20220101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dsw (20220101) SDK Library for Python2"
```

