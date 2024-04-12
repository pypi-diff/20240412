# Comparing `tmp/gentccode-0.2.5.tar.gz` & `tmp/gentccode-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentccode-0.2.5.tar", max compression
+gzip compressed data, was "gentccode-0.2.6.tar", max compression
```

## Comparing `gentccode-0.2.5.tar` & `gentccode-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.5/LICENSE
--rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.5/README.md
--rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.5/gentccode/__init__.py
--rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.5/gentccode/cartesian_for_case.py
--rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.5/gentccode/check_version.py
--rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.5/gentccode/cli.py
--rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.5/gentccode/convert_to_jmx.py
--rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.5/gentccode/convert_to_locust.py
--rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.5/gentccode/generate_case_code.py
--rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.5/gentccode/merge_api.py
--rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.5/gentccode/produce_search_case.py
--rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.5/gentccode/produce_test_case.py
--rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.5/gentccode/read_swagger_rule.py
--rw-r--r--   0        0        0      612 2024-04-10 07:53:59.621191 gentccode-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-13 07:38:48.461356 gentccode-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1084 2024-04-10 07:58:28.662833 gentccode-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2023-09-08 11:07:44.041027 gentccode-0.2.6/gentccode/__init__.py
+-rw-r--r--   0        0        0     1487 2023-09-08 11:12:45.187569 gentccode-0.2.6/gentccode/cartesian_for_case.py
+-rw-r--r--   0        0        0     1216 2023-10-24 06:33:03.360847 gentccode-0.2.6/gentccode/check_version.py
+-rw-r--r--   0        0        0     3348 2024-04-10 07:48:10.190075 gentccode-0.2.6/gentccode/cli.py
+-rw-r--r--   0        0        0    21552 2024-04-10 07:57:26.821826 gentccode-0.2.6/gentccode/convert_to_jmx.py
+-rw-r--r--   0        0        0     4311 2023-11-13 08:42:54.613204 gentccode-0.2.6/gentccode/convert_to_locust.py
+-rw-r--r--   0        0        0    17994 2023-09-26 08:23:03.100251 gentccode-0.2.6/gentccode/generate_case_code.py
+-rw-r--r--   0        0        0     5311 2023-09-11 02:27:59.106915 gentccode-0.2.6/gentccode/merge_api.py
+-rw-r--r--   0        0        0     2857 2023-09-15 06:07:23.156642 gentccode-0.2.6/gentccode/produce_search_case.py
+-rw-r--r--   0        0        0     7089 2023-09-15 03:39:56.738346 gentccode-0.2.6/gentccode/produce_test_case.py
+-rw-r--r--   0        0        0      790 2023-09-13 03:50:15.782471 gentccode-0.2.6/gentccode/read_swagger_rule.py
+-rw-r--r--   0        0        0      612 2024-04-12 10:16:32.869965 gentccode-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 gentccode-0.2.6/PKG-INFO
```

### Comparing `gentccode-0.2.5/LICENSE` & `gentccode-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/README.md` & `gentccode-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/cartesian_for_case.py` & `gentccode-0.2.6/gentccode/cartesian_for_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/check_version.py` & `gentccode-0.2.6/gentccode/check_version.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/cli.py` & `gentccode-0.2.6/gentccode/cli.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/convert_to_jmx.py` & `gentccode-0.2.6/gentccode/convert_to_jmx.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/convert_to_locust.py` & `gentccode-0.2.6/gentccode/convert_to_locust.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/generate_case_code.py` & `gentccode-0.2.6/gentccode/generate_case_code.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/merge_api.py` & `gentccode-0.2.6/gentccode/merge_api.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/produce_search_case.py` & `gentccode-0.2.6/gentccode/produce_search_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/produce_test_case.py` & `gentccode-0.2.6/gentccode/produce_test_case.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/gentccode/read_swagger_rule.py` & `gentccode-0.2.6/gentccode/read_swagger_rule.py`

 * *Files identical despite different names*

### Comparing `gentccode-0.2.5/pyproject.toml` & `gentccode-0.2.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "gentccode"
-version = "0.2.5"
+version = "0.2.6"
 description = "generate test case code"
 authors = ["Lei Su <lei.susl@shopee.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyyaml = "^6.0"
-http-content-parser = "^0.0.14"
+http-content-parser = "^0.0.15"
 click = "^8.1.7"
 lxml = "^4.9.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [tool.poetry.scripts]
```

### Comparing `gentccode-0.2.5/PKG-INFO` & `gentccode-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gentccode
-Version: 0.2.5
+Version: 0.2.6
 Summary: generate test case code
 Author: Lei Su
 Author-email: lei.susl@shopee.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: http-content-parser (>=0.0.14,<0.0.15)
+Requires-Dist: http-content-parser (>=0.0.15,<0.0.16)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## 简介
 
 gtc(generate test case) 是一个把http请求转换为测试代码的cli工具
```

