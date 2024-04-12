# Comparing `tmp/forumaisdktest-0.0.1.tar.gz` & `tmp/forumaisdktest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forumaisdktest-0.0.1.tar", last modified: Thu Apr 11 07:01:25 2024, max compression
+gzip compressed data, was "forumaisdktest-0.0.2.tar", last modified: Fri Apr 12 11:55:43 2024, max compression
```

## Comparing `forumaisdktest-0.0.1.tar` & `forumaisdktest-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 pham-bathong   (502) staff       (20)        0 2024-04-11 07:01:25.610890 forumaisdktest-0.0.1/
--rw-r--r--   0 pham-bathong   (502) staff       (20)     1069 2024-04-10 18:15:27.000000 forumaisdktest-0.0.1/LICENSE
-drwxr-xr-x   0 pham-bathong   (502) staff       (20)        0 2024-04-11 07:01:25.607970 forumaisdktest-0.0.1/ModelMarketSDK/
--rw-r--r--   0 pham-bathong   (502) staff       (20)     9152 2024-04-10 09:53:43.000000 forumaisdktest-0.0.1/ModelMarketSDK/ModelMarket.py
--rw-r--r--   0 pham-bathong   (502) staff       (20)        0 2024-04-10 09:53:43.000000 forumaisdktest-0.0.1/ModelMarketSDK/__init__.py
--rw-r--r--   0 pham-bathong   (502) staff       (20)      886 2024-04-11 07:01:25.610391 forumaisdktest-0.0.1/PKG-INFO
--rw-r--r--   0 pham-bathong   (502) staff       (20)      219 2024-04-10 09:53:43.000000 forumaisdktest-0.0.1/README.md
-drwxr-xr-x   0 pham-bathong   (502) staff       (20)        0 2024-04-11 07:01:25.609938 forumaisdktest-0.0.1/forumaisdktest.egg-info/
--rw-r--r--   0 pham-bathong   (502) staff       (20)      886 2024-04-11 07:01:25.000000 forumaisdktest-0.0.1/forumaisdktest.egg-info/PKG-INFO
--rw-r--r--   0 pham-bathong   (502) staff       (20)      278 2024-04-11 07:01:25.000000 forumaisdktest-0.0.1/forumaisdktest.egg-info/SOURCES.txt
--rw-r--r--   0 pham-bathong   (502) staff       (20)        1 2024-04-11 07:01:25.000000 forumaisdktest-0.0.1/forumaisdktest.egg-info/dependency_links.txt
--rw-r--r--   0 pham-bathong   (502) staff       (20)       65 2024-04-11 07:01:25.000000 forumaisdktest-0.0.1/forumaisdktest.egg-info/requires.txt
--rw-r--r--   0 pham-bathong   (502) staff       (20)       15 2024-04-11 07:01:25.000000 forumaisdktest-0.0.1/forumaisdktest.egg-info/top_level.txt
--rw-r--r--   0 pham-bathong   (502) staff       (20)      714 2024-04-11 07:01:20.000000 forumaisdktest-0.0.1/pyproject.toml
--rw-r--r--   0 pham-bathong   (502) staff       (20)       38 2024-04-11 07:01:25.611059 forumaisdktest-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:43.319067 forumaisdktest-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:43.319067 forumaisdktest-0.0.2/ModelMarketSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)   579187 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/ModelMarketSDK/LLMMarket.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/ModelMarketSDK/ModelMarket.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196960 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/ModelMarketSDK/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/ModelMarketSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-12 11:55:43.319067 forumaisdktest-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:43.319067 forumaisdktest-0.0.2/forumaisdktest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-12 11:55:43.000000 forumaisdktest-0.0.2/forumaisdktest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-12 11:55:43.000000 forumaisdktest-0.0.2/forumaisdktest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:55:43.000000 forumaisdktest-0.0.2/forumaisdktest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 11:55:43.000000 forumaisdktest-0.0.2/forumaisdktest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 11:55:43.000000 forumaisdktest-0.0.2/forumaisdktest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 11:55:35.000000 forumaisdktest-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:55:43.319067 forumaisdktest-0.0.2/setup.cfg
```

### Comparing `forumaisdktest-0.0.1/LICENSE` & `forumaisdktest-0.0.2/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2024 ForumAI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `forumaisdktest-0.0.1/ModelMarketSDK/ModelMarket.py` & `forumaisdktest-0.0.2/ModelMarketSDK/ModelMarket.py`

 * *Files identical despite different names*

### Comparing `forumaisdktest-0.0.1/PKG-INFO` & `forumaisdktest-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forumaisdktest
-Version: 0.0.1
+Version: 0.0.2
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tiktoken; python_version >= "3.8"
-Requires-Dist: web3; python_version >= "3.8"
-Requires-Dist: requests; python_version >= "3.8"
+Requires-Dist: tiktoken==0.6.0
+Requires-Dist: web3==6.15.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv
 
 Alpha implementation of the ForumAI model market python SDK. V.1.0.1
 
 Take a look at the docs to find out how to use it: https://forumai.gitbook.io/forumai/developer-guide/integrate-mixtral8x7b-with-python-sdk-testnet
```

### Comparing `forumaisdktest-0.0.1/forumaisdktest.egg-info/PKG-INFO` & `forumaisdktest-0.0.2/forumaisdktest.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forumaisdktest
-Version: 0.0.1
+Version: 0.0.2
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: tiktoken; python_version >= "3.8"
-Requires-Dist: web3; python_version >= "3.8"
-Requires-Dist: requests; python_version >= "3.8"
+Requires-Dist: tiktoken==0.6.0
+Requires-Dist: web3==6.15.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv
 
 Alpha implementation of the ForumAI model market python SDK. V.1.0.1
 
 Take a look at the docs to find out how to use it: https://forumai.gitbook.io/forumai/developer-guide/integrate-mixtral8x7b-with-python-sdk-testnet
```

### Comparing `forumaisdktest-0.0.1/pyproject.toml` & `forumaisdktest-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+# Include the ABI files
+[tool.setuptools.package-data]
+ModelMarketSDK = ["*.json"]
+
 [project]
 name = "forumaisdktest"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="ForumAISDK", email="forumai@github.com" },
 ]
 description = "ForumAI Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "tiktoken;python_version>='3.8'",
-    "web3;python_version>='3.8'",
-    "requests;python_version>='3.8'",
+    "tiktoken==0.6.0",
+    "web3==6.15.1",
+    "requests==2.31.0",
     "python-dotenv"
 ]
 
 [project.urls]
 Homepage = "https://github.com/0xAresDev/ForumAISDK"
 Issues = "https://github.com/0xAresDev/ForumAISDK/issues"
```

