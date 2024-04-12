# Comparing `tmp/alibabacloud_aiworkspace20210204-3.0.3.tar.gz` & `tmp/alibabacloud_aiworkspace20210204-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-3.0.3.tar", last modified: Tue Apr  2 17:14:52 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aiworkspace20210204-3.0.4.tar", last modified: Fri Apr 12 17:15:19 2024, max compression
```

## Comparing `alibabacloud_aiworkspace20210204-3.0.3.tar` & `alibabacloud_aiworkspace20210204-3.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/
--rw-r--r--   0 root         (0) root         (0)      895 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/__init__.py
--rw-r--r--   0 root         (0) root         (0)   208726 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/client.py
--rw-r--r--   0 root         (0) root         (0)   325691 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-04-02 17:14:52.000000 alibabacloud_aiworkspace20210204-3.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   208726 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/client.py
+-rw-r--r--   0 root         (0) root         (0)   325691 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-12 17:15:19.000000 alibabacloud_aiworkspace20210204-3.0.4/setup.py
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/ChangeLog.md` & `alibabacloud_aiworkspace20210204-3.0.4/ChangeLog.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/LICENSE` & `alibabacloud_aiworkspace20210204-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/PKG-INFO` & `alibabacloud_aiworkspace20210204-3.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiworkspace20210204
-Version: 3.0.3
+Version: 3.0.4
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/README-CN.md` & `alibabacloud_aiworkspace20210204-3.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/README.md` & `alibabacloud_aiworkspace20210204-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/client.py` & `alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204/models.py` & `alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO` & `alibabacloud_aiworkspace20210204-3.0.4/alibabacloud_aiworkspace20210204.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiworkspace20210204
-Version: 3.0.3
+Version: 3.0.4
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204-3.0.3/setup.py` & `alibabacloud_aiworkspace20210204-3.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiworkspace20210204.
 
-Created on 02/04/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiworkspace20210204"
 NAME = "alibabacloud_aiworkspace20210204" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python"
```

