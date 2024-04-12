# Comparing `tmp/loggerjava-0.8.0.tar.gz` & `tmp/loggerjava-0.8.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.8.0.tar", last modified: Fri Apr 12 15:23:39 2024, max compression
+gzip compressed data, was "loggerjava-0.8.0.dev1.tar", last modified: Thu Apr  4 15:13:03 2024, max compression
```

## Comparing `loggerjava-0.8.0.tar` & `loggerjava-0.8.0.dev1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:23:39.948869 loggerjava-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 15:23:32.000000 loggerjava-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-12 15:23:39.948869 loggerjava-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-12 15:23:32.000000 loggerjava-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:23:39.948869 loggerjava-0.8.0/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-12 15:23:32.000000 loggerjava-0.8.0/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-12 15:23:32.000000 loggerjava-0.8.0/loggerjava/exceptionhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-12 15:23:32.000000 loggerjava-0.8.0/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-12 15:23:32.000000 loggerjava-0.8.0/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 15:23:39.948869 loggerjava-0.8.0/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-12 15:23:39.000000 loggerjava-0.8.0/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-12 15:23:39.000000 loggerjava-0.8.0/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 15:23:39.000000 loggerjava-0.8.0/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 15:23:39.000000 loggerjava-0.8.0/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-12 15:23:32.000000 loggerjava-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 15:23:39.948869 loggerjava-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-12 15:23:32.000000 loggerjava-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.699328 loggerjava-0.8.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/exceptionhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 15:13:03.695328 loggerjava-0.8.0.dev1/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 15:13:03.000000 loggerjava-0.8.0.dev1/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 15:13:03.699328 loggerjava-0.8.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-04 15:12:58.000000 loggerjava-0.8.0.dev1/setup.py
```

### Comparing `loggerjava-0.8.0/LICENSE` & `loggerjava-0.8.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.8.0/PKG-INFO` & `loggerjava-0.8.0.dev1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.8.0
+Version: 0.8.0.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Keywords: python,logger,java_like
 Classifier: Programming Language :: Python :: 3
@@ -78,46 +78,30 @@
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 
 ### Exception handler
 using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
 
-remember to register the defs/classes after you created them
-
 ```python
 import loggerjava
 import loggerjava.exceptionhandler
 def test1(a):
     print(b)
-class test2():
-    def printa(self):
-        print(self.b)
-loggerjava.exceptionhandler.register_def(test1)
-loggerjava.exceptionhandler.register_def(test2)
 if __name__ == "__main__":
     try:
         test1(1)
     except Exception as E:
         loggerjava.error(loggerjava.exceptionhandler.handler(E))
-    try:
-        a = test2
-        a.printa()
-    except Exception as E:
-        loggerjava.error(loggerjava.exceptionhandler.handler(E))
 ```
 #### Output：
 ```commandline
 [20:39:00] [main/ERROR]: NameError: name 'b' is not defined
-    at <module> (test.py:30)
-    at test1.test1 (test.py:21)
-
-[20:39:00] [main/ERROR]: AttributeError: 'test2' object has no attribute 'b'
-    at <module> (test.py:35)
-    at test2.printa (test.py:25)
+    at <module> (<input>:7)
+    at test1 (<input>:4)
 ```
 ### Versions
 
 `v0.8.0` added the exceptionhandler and clearcurrentlog function
 
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
```

### Comparing `loggerjava-0.8.0/README.md` & `loggerjava-0.8.0.dev1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -62,46 +62,30 @@
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 
 ### Exception handler
 using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
 
-remember to register the defs/classes after you created them
-
 ```python
 import loggerjava
 import loggerjava.exceptionhandler
 def test1(a):
     print(b)
-class test2():
-    def printa(self):
-        print(self.b)
-loggerjava.exceptionhandler.register_def(test1)
-loggerjava.exceptionhandler.register_def(test2)
 if __name__ == "__main__":
     try:
         test1(1)
     except Exception as E:
         loggerjava.error(loggerjava.exceptionhandler.handler(E))
-    try:
-        a = test2
-        a.printa()
-    except Exception as E:
-        loggerjava.error(loggerjava.exceptionhandler.handler(E))
 ```
 #### Output：
 ```commandline
 [20:39:00] [main/ERROR]: NameError: name 'b' is not defined
-    at <module> (test.py:30)
-    at test1.test1 (test.py:21)
-
-[20:39:00] [main/ERROR]: AttributeError: 'test2' object has no attribute 'b'
-    at <module> (test.py:35)
-    at test2.printa (test.py:25)
+    at <module> (<input>:7)
+    at test1 (<input>:4)
 ```
 ### Versions
 
 `v0.8.0` added the exceptionhandler and clearcurrentlog function
 
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
```

### Comparing `loggerjava-0.8.0/loggerjava/__init__.py` & `loggerjava-0.8.0.dev1/loggerjava/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import time
 import loggerjava
-from loggerjava.exceptionhandler import *
+import loggerjava.exceptionhandler
 
 if __name__ == '__main__':
 
     pass
 
-ver = "v0.8.0"
+ver = "v0.8.0.dev1"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
 fileextension = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
@@ -71,15 +71,15 @@
     if inconsole:
         print(_formats.format(timelog, pos, level, txt))
     if not debugmodein:
         f.write(_formats.format(timelog, pos, level, txt))
         f.close()
     if debugmodein:
         return _formats.format(timelog, pos, level, txt)
-    del detailtime, inconsole, debugmodein, timelog
+    del detailtime, inconsole, debugmodein
 
 
 def debug(txt, pos="main", **overrides):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :param overrides: the overrides of the current config,only actives once
@@ -199,14 +199,15 @@
             try:
                 if absolutepath:
                     tmpf = open(route, mode="w", encoding=configname)
                 else:
                     tmpf = open(name + fileextension, mode="w", encoding=configname)
                 tmpf.close()
                 file_encoding = configname
+                del tmpf
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
                     f = open(name + fileextension, mode="w", encoding=file_encoding)
                 f.close()
             except LookupError:
                 warn("wrong file encoding config.this config is set to default", pos="main_loggerjava",
@@ -280,26 +281,26 @@
 
 
 def exportconfig():
     """
     export current config
     use loadconfig(config) to load this exported config
     returning as a lib
-    :return: a dictonary contains configs
+    :return:
     """
     i = {"name": name, "fileextension": fileextension, "absolutepath": absolutepath,
          "route": route, "showdetailedtime": showdetailedtime, "showinconsole": showinconsole,
          "file_encoding": file_encoding, "fatalexit": fatalclose}
     return i
 
 
 def loadconfig(inputconfig):
     """
     :param inputconfig: the config lib exported from exportconfig()
-    :return: nothing
+    :return:
     """
     global name, showdetailedtime, showinconsole, absolutepath, fileextension, file_encoding, route, fatalclose
 
     if _formats.testformat(inputconfig["absolutepath"], 1):
         absolutepath = inputconfig["absolutepath"]
     else:
         warn("wrong absolute path config.this config is set to default", pos="main_loggerjava", showinconsole=True)
@@ -312,14 +313,15 @@
     try:
         if absolutepath:
             tmpf = open(route, mode="w", encoding=inputconfig["file_encoding"])
         else:
             tmpf = open(name + fileextension, mode="w", encoding=inputconfig["file_encoding"])
         tmpf.close()
         file_encoding = inputconfig["file_encoding"]
+        del tmpf
     except LookupError:
         warn("wrong file encoding config.this config is set to default", pos="main_loggerjava", showinconsole=True)
         file_encoding = "utf-8"
 
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
```

### Comparing `loggerjava-0.8.0/loggerjava/loggerjava.py` & `loggerjava-0.8.0.dev1/loggerjava/loggerjava.py`

 * *Files identical despite different names*

### Comparing `loggerjava-0.8.0/loggerjava/test_loggerjava.py` & `loggerjava-0.8.0.dev1/loggerjava/test_loggerjava.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import unittest
 import loggerjava as lj
 # import pytest
 import time
 
-import loggerjava.exceptionhandler
-
 """
 class MyTestCase(unittest.TestCase):
     def test_something(self):
         self.assertEqual(True, False)  # add assertion here
         """
 
 """
@@ -43,21 +41,11 @@
     assert logger.name == "test"
     logger.config(showdetailedtime=True)
     assert logger.info("test8") == "[" + time.asctime() + "] [main/INFO]: test8\n"
     logger.config(showdetailedtime=False)
     assert logger.log("testoverride", type="d",
                       showdetailedtime=True) == "[" + time.asctime() + "] [main/debug]: testoverride\n"
     assert logger.warn("testoverride", showdetailedtime=True) == "[" + time.asctime() + "] [main/WARN]: testoverride\n"
-    try:
-        def test1(a):
-            print(b)
-        test1(1)
-    except Exception as e:
-        a = loggerjava.exceptionhandler.handler(e)
-        assert a == "NameError: name 'b' is not defined\n    at testin (test_loggerjava.py:53)\n    at test1 (test_loggerjava.py:52)\n"
-        assert logger.warn(loggerjava.exceptionhandler.handler(e)) == "[" + str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
-           str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2,
-                                                                                                 "0") + "] [main/WARN]: %s\n"%a
 
 
 if __name__ == "__main__":
     testin()
```

### Comparing `loggerjava-0.8.0/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.8.0.dev1/loggerjava.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.8.0
+Version: 0.8.0.dev1
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Keywords: python,logger,java_like
 Classifier: Programming Language :: Python :: 3
@@ -78,46 +78,30 @@
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 
 ### Exception handler
 using the `loggerjava.exceptionhandler.exception(exc)` function to process an Exception
 
-remember to register the defs/classes after you created them
-
 ```python
 import loggerjava
 import loggerjava.exceptionhandler
 def test1(a):
     print(b)
-class test2():
-    def printa(self):
-        print(self.b)
-loggerjava.exceptionhandler.register_def(test1)
-loggerjava.exceptionhandler.register_def(test2)
 if __name__ == "__main__":
     try:
         test1(1)
     except Exception as E:
         loggerjava.error(loggerjava.exceptionhandler.handler(E))
-    try:
-        a = test2
-        a.printa()
-    except Exception as E:
-        loggerjava.error(loggerjava.exceptionhandler.handler(E))
 ```
 #### Output：
 ```commandline
 [20:39:00] [main/ERROR]: NameError: name 'b' is not defined
-    at <module> (test.py:30)
-    at test1.test1 (test.py:21)
-
-[20:39:00] [main/ERROR]: AttributeError: 'test2' object has no attribute 'b'
-    at <module> (test.py:35)
-    at test2.printa (test.py:25)
+    at <module> (<input>:7)
+    at test1 (<input>:4)
 ```
 ### Versions
 
 `v0.8.0` added the exceptionhandler and clearcurrentlog function
 
 `v0.7.6` change filetype -> fileextension, simplified the code, completed the override funciton
```

### Comparing `loggerjava-0.8.0/pyproject.toml` & `loggerjava-0.8.0.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "loggerjava"
-version = "v0.8.0"
+version = "v0.8.0.dev1"
 authors = [
   { name="HTony03", email="HTony03@foxmail.com" },
 ]
 description = "an easy logger outputs like java logs"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["python","logger","java_like"]
```

### Comparing `loggerjava-0.8.0/setup.py` & `loggerjava-0.8.0.dev1/setup.py`

 * *Files identical despite different names*

