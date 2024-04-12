# Comparing `tmp/alibabacloud_aiworkspace20210204_py2-1.0.6.tar.gz` & `tmp/alibabacloud_aiworkspace20210204_py2-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aiworkspace20210204_py2-1.0.6.tar", last modified: Tue Apr  2 17:14:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aiworkspace20210204_py2-1.0.7.tar", last modified: Fri Apr 12 17:17:28 2024, max compression
```

## Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6.tar` & `alibabacloud_aiworkspace20210204_py2-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      545 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86389 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/client.py
--rw-r--r--   0 root         (0) root         (0)   326780 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2943 2024-04-02 17:14:18.000000 alibabacloud_aiworkspace20210204_py2-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      545 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86389 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/client.py
+-rw-r--r--   0 root         (0) root         (0)   326780 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-12 17:17:28.000000 alibabacloud_aiworkspace20210204_py2-1.0.7/setup.py
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/ChangeLog.md` & `alibabacloud_aiworkspace20210204_py2-1.0.7/ChangeLog.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/LICENSE` & `alibabacloud_aiworkspace20210204_py2-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/PKG-INFO` & `alibabacloud_aiworkspace20210204_py2-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aiworkspace20210204_py2
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/README-CN.md` & `alibabacloud_aiworkspace20210204_py2-1.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/README.md` & `alibabacloud_aiworkspace20210204_py2-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/client.py` & `alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204/models.py` & `alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO` & `alibabacloud_aiworkspace20210204_py2-1.0.7/alibabacloud_aiworkspace20210204_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aiworkspace20210204-py2
-Version: 1.0.6
+Version: 1.0.7
 Summary: Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aiworkspace20210204_py2-1.0.6/setup.py` & `alibabacloud_aiworkspace20210204_py2-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aiworkspace20210204_py2.
 
-Created on 02/04/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aiworkspace20210204"
 NAME = "alibabacloud_aiworkspace20210204_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AIWorkSpace (20210204) SDK Library for Python2"
```

