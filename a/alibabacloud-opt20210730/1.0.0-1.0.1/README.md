# Comparing `tmp/alibabacloud_opt20210730-1.0.0.tar.gz` & `tmp/alibabacloud_opt20210730-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_opt20210730-1.0.0.tar", last modified: Tue Aug 17 07:06:16 2021, max compression
+gzip compressed data, was "dist/alibabacloud_opt20210730-1.0.1.tar", last modified: Fri Apr 12 17:11:50 2024, max compression
```

## Comparing `alibabacloud_opt20210730-1.0.0.tar` & `alibabacloud_opt20210730-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730/
--rw-r--r--   0 root         (0) root         (0)       21 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6066 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730/client.py
--rw-r--r--   0 root         (0) root         (0)     9560 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2562 2021-08-17 07:06:16.000000 alibabacloud_opt20210730-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9175 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/client.py
+-rw-r--r--   0 root         (0) root         (0)    12810 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-12 17:11:50.000000 alibabacloud_opt20210730-1.0.1/setup.py
```

### Comparing `alibabacloud_opt20210730-1.0.0/LICENSE` & `alibabacloud_opt20210730-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_opt20210730-1.0.0/PKG-INFO` & `alibabacloud_opt20210730-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_opt20210730
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud opt (20210730) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/opt-20210730/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_opt20210730-1.0.0/README-CN.md` & `alibabacloud_opt20210730-1.0.1/README-CN.md`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/opt-20210730/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_opt20210730-1.0.0/README.md` & `alibabacloud_opt20210730-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/opt-20210730/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730/models.py` & `alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,130 +1,101 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import List, Dict, Any
+from typing import Dict, Any, List
 
 
-class GetOrderUsageRequest(TeaModel):
-    def __init__(
-        self,
-        rel_service: str = None,
-        resource_type: int = None,
-        time_range: int = None,
-    ):
-        self.rel_service = rel_service
-        self.resource_type = resource_type
-        self.time_range = time_range
-
-    def validate(self):
-        pass
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.rel_service is not None:
-            result['RelService'] = self.rel_service
-        if self.resource_type is not None:
-            result['ResourceType'] = self.resource_type
-        if self.time_range is not None:
-            result['TimeRange'] = self.time_range
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('RelService') is not None:
-            self.rel_service = m.get('RelService')
-        if m.get('ResourceType') is not None:
-            self.resource_type = m.get('ResourceType')
-        if m.get('TimeRange') is not None:
-            self.time_range = m.get('TimeRange')
-        return self
-
-
-class GetOrderUsageResponseBody(TeaModel):
+class GetOpenStatusResponseBody(TeaModel):
     def __init__(
         self,
+        code: int = None,
+        data: Dict[str, Any] = None,
         message: str = None,
-        data: List[Dict[str, Any]] = None,
         request_id: str = None,
         success: bool = None,
     ):
-        self.message = message
+        self.code = code
         self.data = data
+        self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.message is not None:
-            result['Message'] = self.message
+        if self.code is not None:
+            result['Code'] = self.code
         if self.data is not None:
             result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.success is not None:
             result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
         if m.get('Data') is not None:
             self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
-class GetOrderUsageResponse(TeaModel):
+class GetOpenStatusResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetOrderUsageResponseBody = None,
+        status_code: int = None,
+        body: GetOpenStatusResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetOrderUsageResponseBody()
+            temp_model = GetOpenStatusResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetOrderInfoRequest(TeaModel):
     def __init__(
         self,
@@ -154,183 +125,301 @@
         if m.get('RelService') is not None:
             self.rel_service = m.get('RelService')
         if m.get('ResourceType') is not None:
             self.resource_type = m.get('ResourceType')
         return self
 
 
+class GetOrderInfoResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        biz_type: str = None,
+        current_concurrency: int = None,
+        current_days: int = None,
+        instance_id: str = None,
+        license_key: str = None,
+        remark: str = None,
+        total_days: int = None,
+    ):
+        self.biz_type = biz_type
+        self.current_concurrency = current_concurrency
+        self.current_days = current_days
+        self.instance_id = instance_id
+        self.license_key = license_key
+        self.remark = remark
+        self.total_days = total_days
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
+        if self.biz_type is not None:
+            result['bizType'] = self.biz_type
+        if self.current_concurrency is not None:
+            result['currentConcurrency'] = self.current_concurrency
+        if self.current_days is not None:
+            result['currentDays'] = self.current_days
+        if self.instance_id is not None:
+            result['instanceId'] = self.instance_id
+        if self.license_key is not None:
+            result['licenseKey'] = self.license_key
+        if self.remark is not None:
+            result['remark'] = self.remark
+        if self.total_days is not None:
+            result['totalDays'] = self.total_days
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('bizType') is not None:
+            self.biz_type = m.get('bizType')
+        if m.get('currentConcurrency') is not None:
+            self.current_concurrency = m.get('currentConcurrency')
+        if m.get('currentDays') is not None:
+            self.current_days = m.get('currentDays')
+        if m.get('instanceId') is not None:
+            self.instance_id = m.get('instanceId')
+        if m.get('licenseKey') is not None:
+            self.license_key = m.get('licenseKey')
+        if m.get('remark') is not None:
+            self.remark = m.get('remark')
+        if m.get('totalDays') is not None:
+            self.total_days = m.get('totalDays')
+        return self
+
+
 class GetOrderInfoResponseBody(TeaModel):
     def __init__(
         self,
         code: str = None,
+        data: List[GetOrderInfoResponseBodyData] = None,
         message: str = None,
-        data: Dict[str, Any] = None,
         request_id: str = None,
         success: bool = None,
     ):
         self.code = code
-        self.message = message
         self.data = data
+        self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
-        pass
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
         if self.message is not None:
             result['Message'] = self.message
-        if self.data is not None:
-            result['Data'] = self.data
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.success is not None:
             result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = GetOrderInfoResponseBodyData()
+                self.data.append(temp_model.from_map(k))
         if m.get('Message') is not None:
             self.message = m.get('Message')
-        if m.get('Data') is not None:
-            self.data = m.get('Data')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
 class GetOrderInfoResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
+        status_code: int = None,
         body: GetOrderInfoResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetOrderInfoResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetOpenStatusResponseBody(TeaModel):
+class GetOrderUsageRequest(TeaModel):
     def __init__(
         self,
-        code: int = None,
+        license_key: str = None,
+        rel_service: str = None,
+        resource_type: int = None,
+        time_range: int = None,
+    ):
+        self.license_key = license_key
+        self.rel_service = rel_service
+        self.resource_type = resource_type
+        self.time_range = time_range
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
+        if self.license_key is not None:
+            result['LicenseKey'] = self.license_key
+        if self.rel_service is not None:
+            result['RelService'] = self.rel_service
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.time_range is not None:
+            result['TimeRange'] = self.time_range
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('LicenseKey') is not None:
+            self.license_key = m.get('LicenseKey')
+        if m.get('RelService') is not None:
+            self.rel_service = m.get('RelService')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TimeRange') is not None:
+            self.time_range = m.get('TimeRange')
+        return self
+
+
+class GetOrderUsageResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[Dict[str, Any]] = None,
         message: str = None,
-        data: Dict[str, Any] = None,
         request_id: str = None,
         success: bool = None,
     ):
-        self.code = code
-        self.message = message
         self.data = data
+        self.message = message
         self.request_id = request_id
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.code is not None:
-            result['Code'] = self.code
-        if self.message is not None:
-            result['Message'] = self.message
         if self.data is not None:
             result['Data'] = self.data
+        if self.message is not None:
+            result['Message'] = self.message
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.success is not None:
             result['Success'] = self.success
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Code') is not None:
-            self.code = m.get('Code')
-        if m.get('Message') is not None:
-            self.message = m.get('Message')
         if m.get('Data') is not None:
             self.data = m.get('Data')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Success') is not None:
             self.success = m.get('Success')
         return self
 
 
-class GetOpenStatusResponse(TeaModel):
+class GetOrderUsageResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
-        body: GetOpenStatusResponseBody = None,
+        status_code: int = None,
+        body: GetOrderUsageResponseBody = None,
     ):
         self.headers = headers
+        self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.headers is not None:
             result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
         if self.body is not None:
             result['body'] = self.body.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetOpenStatusResponseBody()
+            temp_model = GetOrderUsageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
```

### Comparing `alibabacloud_opt20210730-1.0.0/alibabacloud_opt20210730.egg-info/PKG-INFO` & `alibabacloud_opt20210730-1.0.1/alibabacloud_opt20210730.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-opt20210730
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud opt (20210730) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/opt-20210730/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_opt20210730-1.0.0/setup.py` & `alibabacloud_opt20210730-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_opt20210730.
 
-Created on 17/08/2021
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_opt20210730"
 NAME = "alibabacloud_opt20210730" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud opt (20210730) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.2.4, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

