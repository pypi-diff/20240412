# Comparing `tmp/alibabacloud_linkedmall20230930-2.1.3.tar.gz` & `tmp/alibabacloud_linkedmall20230930-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.1.3.tar", last modified: Mon Apr  8 04:23:55 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmall20230930-2.1.4.tar", last modified: Fri Apr 12 05:36:11 2024, max compression
```

## Comparing `alibabacloud_linkedmall20230930-2.1.3.tar` & `alibabacloud_linkedmall20230930-2.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/
--rw-r--r--   0 root         (0) root         (0)      454 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1123 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1208 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63190 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/client.py
--rw-r--r--   0 root         (0) root         (0)   157477 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2450 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2646 2024-04-08 04:23:55.000000 alibabacloud_linkedmall20230930-2.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/
+-rw-r--r--   0 root         (0) root         (0)      527 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1208 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63190 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/client.py
+-rw-r--r--   0 root         (0) root         (0)   157477 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2646 2024-04-12 05:36:11.000000 alibabacloud_linkedmall20230930-2.1.4/setup.py
```

### Comparing `alibabacloud_linkedmall20230930-2.1.3/LICENSE` & `alibabacloud_linkedmall20230930-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.3/PKG-INFO` & `alibabacloud_linkedmall20230930-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkedmall20230930
-Version: 2.1.3
+Version: 2.1.4
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.3/README-CN.md` & `alibabacloud_linkedmall20230930-2.1.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.3/README.md` & `alibabacloud_linkedmall20230930-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/client.py` & `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930/models.py` & `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmall20230930-2.1.3/alibabacloud_linkedmall20230930.egg-info/PKG-INFO` & `alibabacloud_linkedmall20230930-2.1.4/alibabacloud_linkedmall20230930.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkedmall20230930
-Version: 2.1.3
+Version: 2.1.4
 Summary: Alibaba Cloud linkedmall (20230930) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmall20230930-2.1.3/setup.py` & `alibabacloud_linkedmall20230930-2.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmall20230930.
 
-Created on 08/04/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmall20230930"
 NAME = "alibabacloud_linkedmall20230930" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud linkedmall (20230930) SDK Library for Python"
```

