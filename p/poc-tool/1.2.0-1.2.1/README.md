# Comparing `tmp/poc_tool-1.2.0.tar.gz` & `tmp/poc_tool-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poc_tool-1.2.0.tar", last modified: Tue Apr  2 05:27:08 2024, max compression
+gzip compressed data, was "poc_tool-1.2.1.tar", last modified: Fri Apr 12 03:01:50 2024, max compression
```

## Comparing `poc_tool-1.2.0.tar` & `poc_tool-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.683754 poc_tool-1.2.0/
--rw-r--r--   0 zhizhuo    (501) staff       (20)     1062 2023-08-10 21:52:31.000000 poc_tool-1.2.0/LICENSE.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2800 2024-04-02 05:27:08.683658 poc_tool-1.2.0/PKG-INFO
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2354 2024-04-02 05:21:55.000000 poc_tool-1.2.0/README.md
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.678860 poc_tool-1.2.0/poc_tool/
--rw-r--r--   0 zhizhuo    (501) staff       (20)      226 2024-04-02 05:09:40.000000 poc_tool-1.2.0/poc_tool/__init__.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.682353 poc_tool-1.2.0/poc_tool/log/
--rw-r--r--   0 zhizhuo    (501) staff       (20)      187 2023-11-17 04:58:06.000000 poc_tool-1.2.0/poc_tool/log/__init__.py
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2660 2023-11-17 05:05:43.000000 poc_tool-1.2.0/poc_tool/log/logger.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.683250 poc_tool-1.2.0/poc_tool/tools/
--rw-r--r--   0 zhizhuo    (501) staff       (20)     1356 2024-04-02 05:25:31.000000 poc_tool-1.2.0/poc_tool/tools/HexDump.py
--rw-r--r--   0 zhizhuo    (501) staff       (20)    13015 2024-04-02 05:03:39.000000 poc_tool-1.2.0/poc_tool/tools/Tools.py
--rw-r--r--   0 zhizhuo    (501) staff       (20)      195 2024-04-02 05:09:47.000000 poc_tool-1.2.0/poc_tool/tools/__init__.py
-drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-02 05:27:08.681994 poc_tool-1.2.0/poc_tool.egg-info/
--rw-r--r--   0 zhizhuo    (501) staff       (20)     2800 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/PKG-INFO
--rw-r--r--   0 zhizhuo    (501) staff       (20)      345 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/SOURCES.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)        1 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/dependency_links.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)       18 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/requires.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)        9 2024-04-02 05:27:08.000000 poc_tool-1.2.0/poc_tool.egg-info/top_level.txt
--rw-r--r--   0 zhizhuo    (501) staff       (20)       79 2024-04-02 05:27:08.683958 poc_tool-1.2.0/setup.cfg
--rw-r--r--   0 zhizhuo    (501) staff       (20)      794 2024-04-02 05:27:03.000000 poc_tool-1.2.0/setup.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-12 03:01:50.744792 poc_tool-1.2.1/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     1062 2024-04-12 02:50:36.000000 poc_tool-1.2.1/LICENSE.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2804 2024-04-12 03:01:50.744729 poc_tool-1.2.1/PKG-INFO
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2358 2024-04-12 03:01:07.000000 poc_tool-1.2.1/README.md
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-12 03:01:50.742855 poc_tool-1.2.1/poc_tool/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      175 2024-04-12 03:00:49.000000 poc_tool-1.2.1/poc_tool/__init__.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-12 03:01:50.743803 poc_tool-1.2.1/poc_tool/log/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      187 2024-04-12 02:50:36.000000 poc_tool-1.2.1/poc_tool/log/__init__.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2660 2024-04-12 02:50:36.000000 poc_tool-1.2.1/poc_tool/log/logger.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-12 03:01:50.744478 poc_tool-1.2.1/poc_tool/tools/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     1356 2024-04-12 02:50:36.000000 poc_tool-1.2.1/poc_tool/tools/HexDump.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)    13015 2024-04-12 02:50:36.000000 poc_tool-1.2.1/poc_tool/tools/Tools.py
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      195 2024-04-12 02:50:36.000000 poc_tool-1.2.1/poc_tool/tools/__init__.py
+drwxr-xr-x   0 zhizhuo    (501) staff       (20)        0 2024-04-12 03:01:50.743488 poc_tool-1.2.1/poc_tool.egg-info/
+-rw-r--r--   0 zhizhuo    (501) staff       (20)     2804 2024-04-12 03:01:50.000000 poc_tool-1.2.1/poc_tool.egg-info/PKG-INFO
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      345 2024-04-12 03:01:50.000000 poc_tool-1.2.1/poc_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)        1 2024-04-12 03:01:50.000000 poc_tool-1.2.1/poc_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)       18 2024-04-12 03:01:50.000000 poc_tool-1.2.1/poc_tool.egg-info/requires.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)        9 2024-04-12 03:01:50.000000 poc_tool-1.2.1/poc_tool.egg-info/top_level.txt
+-rw-r--r--   0 zhizhuo    (501) staff       (20)       79 2024-04-12 03:01:50.744979 poc_tool-1.2.1/setup.cfg
+-rw-r--r--   0 zhizhuo    (501) staff       (20)      794 2024-04-12 03:01:37.000000 poc_tool-1.2.1/setup.py
```

### Comparing `poc_tool-1.2.0/LICENSE.txt` & `poc_tool-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `poc_tool-1.2.0/PKG-INFO` & `poc_tool-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poc_tool
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Poc 还原原始http请求数据包以及常用工具集成化封装类，可以更快帮助您完成POC的书写及调试
 Home-page: https://github.com/zhizhuoshuma/poc_tool
 Author: zhizhuo
 Author-email: zhizhuoshuma@163.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -90,15 +90,15 @@
 ```
 
 ### 日志输出类logger使用
 
 默认日志输出是INFO模式，如果需要所有信息都输出请设置成DEBUG模式
 
 ```shell
-from poc_tool import log, LoggingLevel, LOGGER
+from poc_tool.log import log, LoggingLevel, LOGGER
 
 # 设置日志等级，可以设置info，error，debug，warning，success
 LOGGER.setLevel(LoggingLevel.INFO)
 
 # 使用
 log.info("zhizhuo")
 log.success("zhizhuo")
```

### Comparing `poc_tool-1.2.0/README.md` & `poc_tool-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ```
 
 ### 日志输出类logger使用
 
 默认日志输出是INFO模式，如果需要所有信息都输出请设置成DEBUG模式
 
 ```shell
-from poc_tool import log, LoggingLevel, LOGGER
+from poc_tool.log import log, LoggingLevel, LOGGER
 
 # 设置日志等级，可以设置info，error，debug，warning，success
 LOGGER.setLevel(LoggingLevel.INFO)
 
 # 使用
 log.info("zhizhuo")
 log.success("zhizhuo")
```

### Comparing `poc_tool-1.2.0/poc_tool/log/logger.py` & `poc_tool-1.2.1/poc_tool/log/logger.py`

 * *Files identical despite different names*

### Comparing `poc_tool-1.2.0/poc_tool/tools/HexDump.py` & `poc_tool-1.2.1/poc_tool/tools/HexDump.py`

 * *Files identical despite different names*

### Comparing `poc_tool-1.2.0/poc_tool/tools/Tools.py` & `poc_tool-1.2.1/poc_tool/tools/Tools.py`

 * *Files identical despite different names*

### Comparing `poc_tool-1.2.0/poc_tool.egg-info/PKG-INFO` & `poc_tool-1.2.1/poc_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poc-tool
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python Poc 还原原始http请求数据包以及常用工具集成化封装类，可以更快帮助您完成POC的书写及调试
 Home-page: https://github.com/zhizhuoshuma/poc_tool
 Author: zhizhuo
 Author-email: zhizhuoshuma@163.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -90,15 +90,15 @@
 ```
 
 ### 日志输出类logger使用
 
 默认日志输出是INFO模式，如果需要所有信息都输出请设置成DEBUG模式
 
 ```shell
-from poc_tool import log, LoggingLevel, LOGGER
+from poc_tool.log import log, LoggingLevel, LOGGER
 
 # 设置日志等级，可以设置info，error，debug，warning，success
 LOGGER.setLevel(LoggingLevel.INFO)
 
 # 使用
 log.info("zhizhuo")
 log.success("zhizhuo")
```

### Comparing `poc_tool-1.2.0/setup.py` & `poc_tool-1.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(current_dir, "README.md"), encoding="utf-8") as fd:
     desc = fd.read()
 
 setup(
     name="poc_tool",
     license='MIT',
-    version="1.2.0",
+    version="1.2.1",
     long_description=desc,
     long_description_content_type="text/markdown",
     description="Python Poc 还原原始http请求数据包以及常用工具集成化封装类，可以更快帮助您完成POC的书写及调试",
     author="zhizhuo",
     author_email="zhizhuoshuma@163.com",
     url='https://github.com/zhizhuoshuma/poc_tool',
     packages=find_packages(),
```

