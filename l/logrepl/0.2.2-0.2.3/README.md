# Comparing `tmp/logrepl-0.2.2.tar.gz` & `tmp/logrepl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrepl-0.2.2.tar", max compression
+gzip compressed data, was "logrepl-0.2.3.tar", max compression
```

## Comparing `logrepl-0.2.2.tar` & `logrepl-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.2/LICENSE
--rw-r--r--   0        0        0     3052 2024-04-04 15:33:44.825619 logrepl-0.2.2/README.md
--rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.2/logrepl/__init__.py
--rw-r--r--   0        0        0     7895 2024-04-04 15:01:45.293613 logrepl-0.2.2/logrepl/handler.py
--rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.2/logrepl/run.py
--rw-r--r--   0        0        0      507 2024-04-04 15:33:51.835647 logrepl-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3884 1970-01-01 00:00:00.000000 logrepl-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3080 2024-04-11 03:23:06.462650 logrepl-0.2.3/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.3/logrepl/__init__.py
+-rw-r--r--   0        0        0     8226 2024-04-12 04:01:37.054551 logrepl-0.2.3/logrepl/handler.py
+-rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.3/logrepl/run.py
+-rw-r--r--   0        0        0      507 2024-04-12 04:02:25.054069 logrepl-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 logrepl-0.2.3/PKG-INFO
```

### Comparing `logrepl-0.2.2/LICENSE` & `logrepl-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.2/README.md` & `logrepl-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 pylogrepl
 ```
 
 then the whole repl will be logged to the file `yyyymmddhhmm.log`.
 
 You can also use `logrepl` to log the whole stream io of a program by:
 
-```
+```python
+import logrepl
 with logrepl.log_handler(
     log_dir,
     prefix,
     err_acc_time
 ) as logrepl_handler:
     # run your program here
     # ...
@@ -90,27 +91,27 @@
 
 Update the timestamp suffix with `log_dir` & `prefix` unchanged.
 
 ## start / stop logging to file
 
 **logrepl.Handler.start_log()**
 
-start logging to the file.
+Start logging to the file.
 
 **logrepl.Handler.stop_log()**
 
-stop logging to the file.
+Stop logging to the file.
 
 ## handle sys.stdin/stdout/stderr & builtins.input
 
 **logrepl.Handler.set_io()**
 
-To log **everything** of the repl, `logrepl` modifies sys.stdin/stdout/stderr & builtins.input by this method.
+To log **everything** of the repl, `logrepl` modifies `sys.stdin/stdout/stderr` & `builtins.input` by this method.
 
 **logrepl.Handler.reset_io()**
 
-Reset sys.stdin/stdout/stderr & builtins.input as-is. The repl will still log input of the repl into the file after executing `reset_io`.
+Reset `sys.stdin/stdout/stderr` & `builtins.input` as-is. The input to the repl wil stil be logged into the file after executing `reset_io`.
 
 # Notes
 
 Exceptions ocurred when writing to the log file will not be logged since it'll lead to infinite loop.
```

### Comparing `logrepl-0.2.2/logrepl/handler.py` & `logrepl-0.2.3/logrepl/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import time
 from contextlib import contextmanager
 from io import TextIOWrapper
 from threading import Thread
 from dotenv import dotenv_values
 from functools import reduce
 from queue import Queue
+import traceback
 
 nm_config_dir = 'dir'
 nm_config_prefix = 'prefix'
 nm_config_err_acc_time = 'err_acc_time'
 fname_config = '.pylogrepl'
 default_dir = '.'
 default_err_acc_time = 1.
@@ -48,14 +49,16 @@
             errors=ref.errors,
             line_buffering=ref.line_buffering,
             write_through=ref.write_through
             # newline use default
         )
         self.write_fn = ref.write
         self.write = decorate(self.write_fn)
+    def __del__(self):
+        pass
 
 class LogInWrapper(TextIOWrapper):
     def __init__(self, ref: TextIOWrapper, decorate):
         super(LogInWrapper, self).__init__(
             ref.buffer,
             encoding=ref.encoding,
             errors=ref.errors,
@@ -63,14 +66,16 @@
             write_through=ref.write_through
             # newline use default
         )
         self.read_fn = ref.read
         self.readline_fn = ref.readline
         self.read = decorate(self.read_fn)
         self.readline = decorate(self.readline_fn)
+    def __del__(self):
+        pass
 
 def arg_config_default(arg, dict_config, nm_config, default, type_fn):
     if arg is None:
         if nm_config in dict_config:
             return type_fn(dict_config[nm_config])
         else:
             return default
@@ -234,38 +239,47 @@
                 thr.start()
                 self.err_thread = thr
         except Exception as e:
             debug_write(str(e))
             builtin_stderr_write(str(e))
     
     def exit(self):
-        if not self.err_thread is None and not self.err_thread.is_alive():
+        if not self.err_thread is None and self.err_thread.is_alive():
             self.err_thread.join()
         self.reset_io()
 
     def stop_log(self):
         print('logrepl stopped log to file.')
         self.set_will_log(False)
 
     def start_log(self):
         self.set_will_log(True)
         print('logrepl start log to file.')
 
     @staticmethod
     def reset_io():
+        sys.stdout.flush()
         sys.stdout = sys.__stdout__
+        sys.stderr.flush()
         sys.stderr = sys.__stderr__
         sys.stdin = sys.__stdin__
         builtins.input = builtin_input # useless for the running repl!!
     
 @contextmanager
 def log_handler(
     log_dir=None,
     prefix=None,
     err_acc_time=None,
 ):
     hd = Handler.from_env(log_dir, prefix, err_acc_time)
     hd.set_io()
     try:
         yield hd
+    except Exception as e:
+        e_str = traceback.format_exc()
+        try:
+            hd.check_dir_write(e_str)
+        except Exception as e1:
+            hd.add_err(e1)
+        raise e
     finally:
         hd.exit()
```

### Comparing `logrepl-0.2.2/logrepl/run.py` & `logrepl-0.2.3/logrepl/run.py`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.2/PKG-INFO` & `logrepl-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrepl
-Version: 0.2.2
+Version: 0.2.3
 Summary: By this command line tool, you can run a python repl which logs everying into a file.
 Home-page: https://github.com/baliuzeger/logrepl
 Keywords: repl,log,logging
 Author: bali
 Author-email: baluzeger@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,16 @@
 pylogrepl
 ```
 
 then the whole repl will be logged to the file `yyyymmddhhmm.log`.
 
 You can also use `logrepl` to log the whole stream io of a program by:
 
-```
+```python
+import logrepl
 with logrepl.log_handler(
     log_dir,
     prefix,
     err_acc_time
 ) as logrepl_handler:
     # run your program here
     # ...
@@ -111,28 +112,28 @@
 
 Update the timestamp suffix with `log_dir` & `prefix` unchanged.
 
 ## start / stop logging to file
 
 **logrepl.Handler.start_log()**
 
-start logging to the file.
+Start logging to the file.
 
 **logrepl.Handler.stop_log()**
 
-stop logging to the file.
+Stop logging to the file.
 
 ## handle sys.stdin/stdout/stderr & builtins.input
 
 **logrepl.Handler.set_io()**
 
-To log **everything** of the repl, `logrepl` modifies sys.stdin/stdout/stderr & builtins.input by this method.
+To log **everything** of the repl, `logrepl` modifies `sys.stdin/stdout/stderr` & `builtins.input` by this method.
 
 **logrepl.Handler.reset_io()**
 
-Reset sys.stdin/stdout/stderr & builtins.input as-is. The repl will still log input of the repl into the file after executing `reset_io`.
+Reset `sys.stdin/stdout/stderr` & `builtins.input` as-is. The input to the repl wil stil be logged into the file after executing `reset_io`.
 
 # Notes
 
 Exceptions ocurred when writing to the log file will not be logged since it'll lead to infinite loop.
```

