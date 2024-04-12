# Comparing `tmp/aliyun-python-sdk-tingwu-1.0.4.tar.gz` & `tmp/aliyun-python-sdk-tingwu-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-tingwu-1.0.4.tar", last modified: Mon Mar 18 09:01:18 2024, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-tingwu-1.0.5.tar", last modified: Fri Apr 12 03:54:52 2024, max compression
```

## Comparing `aliyun-python-sdk-tingwu-1.0.4.tar` & `aliyun-python-sdk-tingwu-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1552 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      533 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1552 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      859 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/
--rw-r--r--   0 root         (0) root         (0)     1573 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-18 09:01:18.000000 aliyun-python-sdk-tingwu-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2467 2024-03-18 09:01:17.000000 aliyun-python-sdk-tingwu-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1552 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      859 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-12 03:54:52.000000 aliyun-python-sdk-tingwu-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-04-12 03:54:51.000000 aliyun-python-sdk-tingwu-1.0.5/setup.py
```

### Comparing `aliyun-python-sdk-tingwu-1.0.4/LICENSE` & `aliyun-python-sdk-tingwu-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/PKG-INFO` & `aliyun-python-sdk-tingwu-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tingwu
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tingwu module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tingwu
```

### Comparing `aliyun-python-sdk-tingwu-1.0.4/README.rst` & `aliyun-python-sdk-tingwu-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/PKG-INFO` & `aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-tingwu
-Version: 1.0.4
+Version: 1.0.5
 Summary: The tingwu module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-tingwu
```

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt` & `aliyun-python-sdk-tingwu-1.0.5/aliyun_python_sdk_tingwu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/CreateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/CreateTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/DeleteTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/GetTaskInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/GetTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/ListTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py` & `aliyun-python-sdk-tingwu-1.0.5/aliyunsdktingwu/request/v20230930/UpdateTranscriptionPhrasesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-tingwu-1.0.4/setup.py` & `aliyun-python-sdk-tingwu-1.0.5/setup.py`

 * *Files identical despite different names*

