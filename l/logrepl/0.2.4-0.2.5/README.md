# Comparing `tmp/logrepl-0.2.4.tar.gz` & `tmp/logrepl-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logrepl-0.2.4.tar", max compression
+gzip compressed data, was "logrepl-0.2.5.tar", max compression
```

## Comparing `logrepl-0.2.4.tar` & `logrepl-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.4/LICENSE
--rw-r--r--   0        0        0     3408 2024-04-12 05:49:01.625131 logrepl-0.2.4/README.md
--rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.4/logrepl/__init__.py
--rw-r--r--   0        0        0     8226 2024-04-12 04:01:37.054551 logrepl-0.2.4/logrepl/handler.py
--rw-r--r--   0        0        0      789 2024-04-04 14:20:57.326734 logrepl-0.2.4/logrepl/run.py
--rw-r--r--   0        0        0      507 2024-04-12 05:49:48.634015 logrepl-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 logrepl-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-26 09:15:47.656696 logrepl-0.2.5/LICENSE
+-rw-r--r--   0        0        0     3408 2024-04-12 05:49:01.625131 logrepl-0.2.5/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 02:54:57.958672 logrepl-0.2.5/logrepl/__init__.py
+-rw-r--r--   0        0        0     8514 2024-04-12 06:30:22.052590 logrepl-0.2.5/logrepl/handler.py
+-rw-r--r--   0        0        0      803 2024-04-12 06:20:34.415102 logrepl-0.2.5/logrepl/run.py
+-rw-r--r--   0        0        0      507 2024-04-12 06:31:05.331839 logrepl-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     4240 1970-01-01 00:00:00.000000 logrepl-0.2.5/PKG-INFO
```

### Comparing `logrepl-0.2.4/LICENSE` & `logrepl-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.4/README.md` & `logrepl-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `logrepl-0.2.4/logrepl/handler.py` & `logrepl-0.2.5/logrepl/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,32 +86,35 @@
 
     def __init__(
         self,
         log_dir=default_dir,
         prefix=None,
         err_acc_time=default_err_acc_time,
         will_log=default_will_log,
+        is_repl=False
     ):
 
         self.log_dir = Path(log_dir)
         self.prefix = prefix
         self.update_suffix()
         self.will_log = will_log
 
         self.err_acc_time = err_acc_time
         self.last_err_time = None
         self.errors = Queue()
         self.err_thread = None
+        self.is_repl = is_repl
 
     @classmethod
     def from_env(
         cls,
         log_dir=None,
         prefix=None,
         err_acc_time=None,
+        is_repl=None,
     ):
         config = dotenv_values(fname_config)
 
         log_dir = arg_config_default(log_dir, config, nm_config_dir, default_dir, str)
 
         if prefix is None and nm_config_prefix in config:
             prefix = str(config[nm_config_prefix])
@@ -120,15 +123,18 @@
             err_acc_time,
             config,
             nm_config_err_acc_time,
             default_err_acc_time,
             float
         )
 
-        return cls(log_dir, prefix, err_acc_time, True)
+        if is_repl is None:
+            is_repl = False
+
+        return cls(log_dir, prefix, err_acc_time, True, is_repl)
 
     def set_dir(self, log_dir):
         """
         Update new logging dir.
         log_dir must be string or Path.
         The suffix _yyyymmddhhmm.log will also be updated.
         """
@@ -158,15 +164,15 @@
     def get_path(self):
         if self.log_file is None:
             raise ValueError('logrepl log_file is None.')
         return self.log_dir/self.log_file
     
     def check_dir_write(self, msg):
         if self.will_log:
-            # raise Exception(f'dead {self.errors.qsize() % 2}') # for debug
+            raise Exception(f'dead {self.errors.qsize() % 2}') # for debug
             self.log_dir.mkdir(exist_ok=True, parents=True)
             with open(self.get_path(), 'a') as log:
                 log.write(msg)
 
     def decorate_log_out(self, fn):
         def new_func(*args, **kwargs):
             try:
@@ -214,21 +220,24 @@
                 time.sleep(self.err_acc_time)
                 time_diff = time.time() - self.last_err_time
             
             set_errs = set()
             while not self.errors.empty():
                 set_errs.add(str(self.errors.get(block=False)))
 
-            builtin_stderr_write(
-                reduce(
-                    lambda acc, x: acc + f'{x}\n',
-                    set_errs,
-                    '\nlogrepl got errors (ignore the duplicated ones):\n'
-                ) + '>>> '
-            )
+            msg = reduce(
+                lambda acc, x: acc + f'{x}\n',
+                set_errs,
+                '\nlogrepl got errors (ignore the duplicated ones):\n'
+            ) + '\n'
+
+            if self.is_repl:
+                msg += '>>> '
+
+            builtin_stderr_write(msg)
         
         except Exception as e:
             debug_write(str(e))
             builtin_stderr_write(str(e))
 
     def add_err(self, err):
         try:
@@ -240,15 +249,17 @@
                 self.err_thread = thr
         except Exception as e:
             debug_write(str(e))
             builtin_stderr_write(str(e))
     
     def exit(self):
         if not self.err_thread is None and self.err_thread.is_alive():
+            self.is_repl = False
             self.err_thread.join()
+            # builtin_stderr_write('exit join done.')
         self.reset_io()
 
     def stop_log(self):
         print('logrepl stopped log to file.')
         self.set_will_log(False)
 
     def start_log(self):
@@ -265,16 +276,17 @@
         builtins.input = builtin_input # useless for the running repl!!
     
 @contextmanager
 def log_handler(
     log_dir=None,
     prefix=None,
     err_acc_time=None,
+    is_repl=False
 ):
-    hd = Handler.from_env(log_dir, prefix, err_acc_time)
+    hd = Handler.from_env(log_dir, prefix, err_acc_time, is_repl)
     hd.set_io()
     try:
         yield hd
     except Exception as e:
         e_str = traceback.format_exc()
         try:
             hd.check_dir_write(e_str)
```

### Comparing `logrepl-0.2.4/logrepl/run.py` & `logrepl-0.2.5/logrepl/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,16 @@
     parser.add_argument('-d', '--dir', help="dir for log file")
     parser.add_argument('-t', '--time', help="time for accummulate logrepl error msgs")
     args = parser.parse_args()
 
     with logrepl.log_handler(
         args.dir,
         args.prefix,
-        args.time
+        args.time,
+        True
     ) as logrepl_handler:
         dict_global = globals().copy()
         dict_global['logrepl_handler'] = logrepl_handler
         ls_to_pop = ['argparse', 'code', 'logrepl', 'asyncio', 'run_repl', 'main',]
         for k in ls_to_pop:
             dict_global.pop(k, None)
         code.interact(local=dict_global)
```

### Comparing `logrepl-0.2.4/PKG-INFO` & `logrepl-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logrepl
-Version: 0.2.4
+Version: 0.2.5
 Summary: By this command line tool, you can run a python repl which logs everying into a file.
 Home-page: https://github.com/baliuzeger/logrepl
 Keywords: repl,log,logging
 Author: bali
 Author-email: baluzeger@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
```

