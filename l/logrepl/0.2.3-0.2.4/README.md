# Comparing `tmp/logrepl-0.2.3.tar.gz` & `tmp/logrepl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrepl-0.2.3.tar", max compression
+gzip compressed data, was "logrepl-0.2.4.tar", max compression
```

## Comparing `logrepl-0.2.3.tar` & `logrepl-0.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.3/LICENSE
--rw-r--r--   0        0        0     3080 2024-04-11 03:23:06.462650 logrepl-0.2.3/README.md
--rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.3/logrepl/__init__.py
--rw-r--r--   0        0        0     8226 2024-04-12 04:01:37.054551 logrepl-0.2.3/logrepl/handler.py
--rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.3/logrepl/run.py
--rw-r--r--   0        0        0      507 2024-04-12 04:02:25.054069 logrepl-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 logrepl-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.4/LICENSE
+-rw-r--r--   0        0        0     3408 2024-04-12 05:49:01.625131 logrepl-0.2.4/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.4/logrepl/__init__.py
+-rw-r--r--   0        0        0     8226 2024-04-12 04:01:37.054551 logrepl-0.2.4/logrepl/handler.py
+-rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.4/logrepl/run.py
+-rw-r--r--   0        0        0      507 2024-04-12 05:49:48.634015 logrepl-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 logrepl-0.2.4/PKG-INFO
```

### Comparing `logrepl-0.2.3/LICENSE` & `logrepl-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.3/README.md` & `logrepl-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 ```python
 import logrepl
 with logrepl.log_handler(
     log_dir,
     prefix,
     err_acc_time
 ) as logrepl_handler:
+    # import modules and packages
     # run your program here
     # ...
 ```
 
+Beware that you have to import all the modules and packages in the `with` clause. If a logger of some module or package is initialized before the `with` clause, `logrepl` cannot modify its `logging.StreamHandler`, then all the iniformation directed to that `StreamHandler` will not be logged.
+
 # Config
 
 ## Prefix of the log file
 
 use the optional positional argument, for example:
 ```
 pylogrepl prefix
```

### Comparing `logrepl-0.2.3/logrepl/handler.py` & `logrepl-0.2.4/logrepl/handler.py`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.3/logrepl/run.py` & `logrepl-0.2.4/logrepl/run.py`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.3/PKG-INFO` & `logrepl-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrepl
-Version: 0.2.3
+Version: 0.2.4
 Summary: By this command line tool, you can run a python repl which logs everying into a file.
 Home-page: https://github.com/baliuzeger/logrepl
 Keywords: repl,log,logging
 Author: bali
 Author-email: baluzeger@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -37,18 +37,21 @@
 ```python
 import logrepl
 with logrepl.log_handler(
     log_dir,
     prefix,
     err_acc_time
 ) as logrepl_handler:
+    # import modules and packages
     # run your program here
     # ...
 ```
 
+Beware that you have to import all the modules and packages in the `with` clause. If a logger of some module or package is initialized before the `with` clause, `logrepl` cannot modify its `logging.StreamHandler`, then all the iniformation directed to that `StreamHandler` will not be logged.
+
 # Config
 
 ## Prefix of the log file
 
 use the optional positional argument, for example:
 ```
 pylogrepl prefix
```

