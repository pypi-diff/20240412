# Comparing `tmp/freedownload-1.0.5.tar.gz` & `tmp/freedownload-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freedownload-1.0.5.tar", last modified: Thu Apr 11 00:44:40 2024, max compression
+gzip compressed data, was "freedownload-1.0.6.tar", last modified: Fri Apr 12 00:51:05 2024, max compression
```

## Comparing `freedownload-1.0.5.tar` & `freedownload-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 00:44:40.309384 freedownload-1.0.5/
--rw-rw-rw-   0        0        0      966 2024-04-11 00:44:40.309384 freedownload-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 00:44:40.291433 freedownload-1.0.5/freedownload/
--rw-rw-rw-   0        0        0     6247 2024-04-11 00:42:32.000000 freedownload-1.0.5/freedownload/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-11 00:43:36.000000 freedownload-1.0.5/freedownload/version.py
-drwxrwxrwx   0        0        0        0 2024-04-11 00:44:40.308388 freedownload-1.0.5/freedownload.egg-info/
--rw-rw-rw-   0        0        0      966 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-11 00:44:40.000000 freedownload-1.0.5/freedownload.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-11 00:44:40.309384 freedownload-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:05.400709 freedownload-1.0.6/
+-rw-rw-rw-   0        0        0      966 2024-04-12 00:51:05.399710 freedownload-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 freedownload-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:05.373780 freedownload-1.0.6/freedownload/
+-rw-rw-rw-   0        0        0     6095 2024-04-12 00:45:26.000000 freedownload-1.0.6/freedownload/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-12 00:50:42.000000 freedownload-1.0.6/freedownload/version.py
+drwxrwxrwx   0        0        0        0 2024-04-12 00:51:05.398712 freedownload-1.0.6/freedownload.egg-info/
+-rw-rw-rw-   0        0        0      966 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 00:51:05.000000 freedownload-1.0.6/freedownload.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-04-12 00:51:05.400709 freedownload-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1612 2023-12-21 01:53:29.000000 freedownload-1.0.6/setup.py
```

### Comparing `freedownload-1.0.5/PKG-INFO` & `freedownload-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-1.0.5/README.md` & `freedownload-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `freedownload-1.0.5/freedownload/__init__.py` & `freedownload-1.0.6/freedownload/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,18 @@
 import shutil
 import ast
 import os
 import platform
 sistema_operativo = platform.system()
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-import dns.resolver
 import json
 import sys
 sys.setrecursionlimit(1500)
 
-dns.resolver.default_resolver = dns.resolver.Resolver(configure=False)
-dns.resolver.default_resolver.nameservers = ['1.1.1.1']
-
 headers = {"User-Agent":"Mozilla/5.0 (Windows NT 6.1; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0"}
 
 if sistema_operativo == "Windows":
     cmd = "cls"
 elif sistema_operativo == "Linux":
     cmd = "clear"
```

### Comparing `freedownload-1.0.5/freedownload.egg-info/PKG-INFO` & `freedownload-1.0.6/freedownload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freedownload
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python 3 library for short text
 Home-page: https://github.com/hiyabo69/downfree
 Author: Jose
 Author-email: josepalaciosgiraldo91@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `freedownload-1.0.5/setup.py` & `freedownload-1.0.6/setup.py`

 * *Files identical despite different names*

