# Comparing `tmp/joo-0.1.0.139.tar.gz` & `tmp/joo-0.1.0.140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joo-0.1.0.139.tar", last modified: Thu Apr 11 09:21:51 2024, max compression
+gzip compressed data, was "joo-0.1.0.140.tar", last modified: Fri Apr 12 07:24:29 2024, max compression
```

## Comparing `joo-0.1.0.139.tar` & `joo-0.1.0.140.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.800181 joo-0.1.0.139/
--rw-rw-rw-   0        0        0      625 2024-04-11 09:21:51.797304 joo-0.1.0.139/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-11 09:21:46.000000 joo-0.1.0.139/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.651939 joo-0.1.0.139/lib/
-drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.708979 joo-0.1.0.139/lib/joo/
--rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.139/lib/joo/LICENSE
--rw-rw-rw-   0        0        0     4178 2024-04-03 08:59:24.000000 joo-0.1.0.139/lib/joo/__init__.py
--rw-rw-rw-   0        0        0      759 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/__version__.py
--rw-rw-rw-   0        0        0     2780 2024-04-03 08:58:39.000000 joo-0.1.0.139/lib/joo/cli.py
--rw-rw-rw-   0        0        0    12338 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/datetimeutil.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.791174 joo-0.1.0.139/lib/joo/dc/
--rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/dc/__init__.py
--rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.139/lib/joo/dc/http.py
--rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.139/lib/joo/dc/selenium.py
--rw-rw-rw-   0        0        0     5119 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/httpapi.py
--rw-rw-rw-   0        0        0    12685 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/logging.py
--rw-rw-rw-   0        0        0    15596 2024-04-11 09:21:46.000000 joo-0.1.0.139/lib/joo/sysutil.py
-drwxrwxrwx   0        0        0        0 2024-04-11 09:21:51.773643 joo-0.1.0.139/lib/joo.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-11 09:21:49.000000 joo-0.1.0.139/lib/joo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 09:21:51.805202 joo-0.1.0.139/setup.cfg
--rw-rw-rw-   0        0        0     1424 2024-04-11 09:21:46.000000 joo-0.1.0.139/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.048524 joo-0.1.0.140/
+-rw-rw-rw-   0        0        0      625 2024-04-12 07:24:29.045528 joo-0.1.0.140/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-12 07:24:25.000000 joo-0.1.0.140/README.md
+drwxrwxrwx   0        0        0        0 2024-04-12 07:24:28.948236 joo-0.1.0.140/lib/
+drwxrwxrwx   0        0        0        0 2024-04-12 07:24:28.985097 joo-0.1.0.140/lib/joo/
+-rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.140/lib/joo/LICENSE
+-rw-rw-rw-   0        0        0     6197 2024-04-12 05:15:52.000000 joo-0.1.0.140/lib/joo/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-12 07:24:25.000000 joo-0.1.0.140/lib/joo/__version__.py
+-rw-rw-rw-   0        0        0     2780 2024-04-12 03:38:16.000000 joo-0.1.0.140/lib/joo/cli.py
+-rw-rw-rw-   0        0        0    12338 2024-04-11 09:21:46.000000 joo-0.1.0.140/lib/joo/datetimeutil.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.042107 joo-0.1.0.140/lib/joo/dc/
+-rw-rw-rw-   0        0        0     8141 2024-04-11 09:21:46.000000 joo-0.1.0.140/lib/joo/dc/__init__.py
+-rw-rw-rw-   0        0        0     4921 2024-04-09 06:59:29.000000 joo-0.1.0.140/lib/joo/dc/http.py
+-rw-rw-rw-   0        0        0     9678 2024-04-09 05:54:46.000000 joo-0.1.0.140/lib/joo/dc/selenium.py
+-rw-rw-rw-   0        0        0     5119 2024-04-12 05:42:04.000000 joo-0.1.0.140/lib/joo/httpapi.py
+-rw-rw-rw-   0        0        0    11864 2024-04-12 04:32:41.000000 joo-0.1.0.140/lib/joo/logging.py
+-rw-rw-rw-   0        0        0    15809 2024-04-12 05:34:00.000000 joo-0.1.0.140/lib/joo/sysutil.py
+drwxrwxrwx   0        0        0        0 2024-04-12 07:24:29.031591 joo-0.1.0.140/lib/joo.egg-info/
+-rw-rw-rw-   0        0        0      625 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      362 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-12 07:24:27.000000 joo-0.1.0.140/lib/joo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-12 07:24:29.048524 joo-0.1.0.140/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2024-04-12 07:24:25.000000 joo-0.1.0.140/setup.py
```

### Comparing `joo-0.1.0.139/PKG-INFO` & `joo-0.1.0.140/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.139
+Version: 0.1.0.140
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.139/lib/joo/LICENSE` & `joo-0.1.0.140/lib/joo/LICENSE`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/__version__.py` & `joo-0.1.0.140/lib/joo/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 __VERSION__ = {
     "name": "joo",
     "description": "joo library",
     "version": "0.1.0",
-    "build": 139,
+    "build": 140,
     "license": "MIT License",
     "author": "Wooloo Studio",
     "author_email": "max.wu@wooloostudio.com",
     "url": "https://github.com/metatutu/joo",
     "project_urls": {
         "Documentation": "https://github.com/metatutu/joo",
         "Source Code": "https://github.com/metatutu/joo",
```

### Comparing `joo-0.1.0.139/lib/joo/cli.py` & `joo-0.1.0.140/lib/joo/cli.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/datetimeutil.py` & `joo-0.1.0.140/lib/joo/datetimeutil.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/dc/__init__.py` & `joo-0.1.0.140/lib/joo/dc/__init__.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/dc/http.py` & `joo-0.1.0.140/lib/joo/dc/http.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/dc/selenium.py` & `joo-0.1.0.140/lib/joo/dc/selenium.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/httpapi.py` & `joo-0.1.0.140/lib/joo/httpapi.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.139/lib/joo/logging.py` & `joo-0.1.0.140/lib/joo/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,34 @@
     def __init__(self):
         ManagedObject.__init__(self)
 
         # settings
         self.enabled_level = 0  # log messages at any level (level >= 0)
         self.use_log_lock = False  # use thread lock when logging message
 
+    def __del__(self):
+        # NOTE: Not calling close() here to make sure the object will be
+        # closed explicitly to make sure it's closed gracefully before
+        # garbage collection process.
+        ManagedObject.__del__(self)
+
     def open(self):
         if self._state is not None: return True
         self._log_lock = threading.Lock() if self.use_log_lock else None
         self._state = "opened"
         return True
 
     def close(self):
         if self._state is None: return
         self._log_lock = None
         self._state = None
 
+    def gc(self):
+        self.close()
+
     @abstractmethod
     def _log(self, timestamp, message, depth, level): pass
 
     def _log_low(self, timestamp, message, depth, level, std_level):
         # open
         if not self.open(): return
         
@@ -252,45 +261,43 @@
             return None
 
 class Loggers(ManagedObjects):
     def __init__(self):
         ManagedObjects.__init__(self)
 
     def register_logger(self, logger):
-        self.register_object(logger)
+        self.register_object(logger, Logger)
 
     def close(self):
-        for obj in self._objects: obj.close()
-        self._objects.clear()
-
-    gc = close
+        for obj in self: obj.close()
+        self.clear()
 
     def log(self, message, depth=0, level=MessageLevel.GENERAL):
-        for logger in self._objects: logger.log(message, depth, level)
+        for logger in self: logger.log(message, depth, level)
 
     def debug(self, message, depth=0, level=MessageLevel.DEBUG):
-        for logger in self._objects: logger.debug(message, depth, level)
+        for logger in self: logger.debug(message, depth, level)
 
     def info(self, message, depth=0, level=MessageLevel.INFO):
-        for logger in self._objects: logger.info(message, depth, level)
+        for logger in self: logger.info(message, depth, level)
 
     def warning(self, message, depth=0, level=MessageLevel.WARNING):
-        for logger in self._objects: logger.warning(message, depth, level)
+        for logger in self: logger.warning(message, depth, level)
 
     def error(self, message, depth=0, level=MessageLevel.ERROR):
-        for logger in self._objects: logger.error(message, depth, level)
+        for logger in self: logger.error(message, depth, level)
 
     def critical(self, message, depth=0, level=MessageLevel.CRITICAL):
-        for logger in self._objects: logger.critical(message, depth, level)
+        for logger in self: logger.critical(message, depth, level)
 
     def separator(self, ch="=", width=80, level=MessageLevel.SEPARATOR):
-        for logger in self._objects: logger.separator(ch, width, level)
+        for logger in self: logger.separator(ch, width, level)
 
     def exception(self, ex, depth=0, level=MessageLevel.DEBUG):
-        for logger in self._objects: logger.exception(ex, depth, level)
+        for logger in self: logger.exception(ex, depth, level)
 
 class LoggerHelper:
     def __init__(self):
         self._logger = None
 
     @property
     def logger(self):
@@ -323,34 +330,10 @@
     def exception(self, ex, depth=0, level=MessageLevel.DEBUG):
         if self._logger: self._logger.exception(ex, depth, level)
 
     def error_x(self, x, message, depth=0, level=MessageLevel.ERROR):
         self.error(message, depth, level)
         return x
 
-    def error_n(self, message, depth=0, level=MessageLevel.ERROR):
-        return self.error_x(None, message, depth, level)
-
-    def error_f(self, message, depth=0, level=MessageLevel.ERROR):
-        return self.error_x(False, message, depth, level)
-
-    def error_0(self, message, depth=0, level=MessageLevel.ERROR):
-        return self.error_x(0, message, depth, level)
-
-    def error_1(self, message, depth=0, level=MessageLevel.ERROR):
-        return self.error_x(1, message, depth, level)
-    
     def exception_x(self, x, ex, depth=0, level=MessageLevel.DEBUG):
         self.exception(ex, depth, level)
         return x
-    
-    def exception_n(self, ex, depth=0, level=MessageLevel.DEBUG):
-        return self.exception_x(None, ex, depth, level)
-
-    def exception_f(self, ex, depth=0, level=MessageLevel.DEBUG):
-        return self.exception_x(False, ex, depth, level)
-
-    def exception_0(self, ex, depth=0, level=MessageLevel.DEBUG):
-        return self.exception_x(0, ex, depth, level)
-
-    def exception_1(self, ex, depth=0, level=MessageLevel.DEBUG):
-        return self.exception_x(1, ex, depth, level)
```

### Comparing `joo-0.1.0.139/lib/joo/sysutil.py` & `joo-0.1.0.140/lib/joo/sysutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,28 +189,38 @@
             else:
                 contents = base64.b64encode(f.read()).decode(encoding)
         return contents
     except:
         return None
 
 class TempFileSystemObject(ManagedObject):
+    _objects = ManagedObjects()
+
+    @classmethod
+    def GC(cls): cls._objects.gc()
+
     def __init__(self):
+        self._objects.register_object(self)
         ManagedObject.__init__(self)
 
         # control
         self._is_folder = False
         self._fpath = None
 
+    def __del__(self):
+        ManagedObject.__del__(self)
+        self._objects.unregister_object(self)
+
+    def gc(self):
+        self.delete()
+        self._objects.unregister_object(self)
+        del self
+
     @property
     def path(self): return self._fpath
-    
-    _objects = ManagedObjects()
-
-    @classmethod
-    def gc(cls): cls._objects.gc()
 
     def create(self, temp_folderpath=None):
         # create
         if temp_folderpath is None: temp_folderpath = tempfile.gettempdir()
         while True:
             fpath = os.path.join(temp_folderpath, str(uuid.uuid4()))
             if not os.path.exists(fpath): break
@@ -227,30 +237,24 @@
         # delete
         self.delete()
 
         # attach
         self._state = "created"
         self._fpath = fpath
 
-        # register
-        self._objects.register_object(self)
-
-    def detach(self, gc=False):
-        # unregister
-        if not gc: self._objects.unregister_object(self)
-
+    def detach(self):
         # detach
         fpath = self._fpath
         self._fpath = None
         self._state = None
         return fpath
 
-    def delete(self, gc=False):
+    def delete(self):
         # detach
-        fpath = self.detach(gc)
+        fpath = self.detach()
 
         # delete
         if fpath is None: return
         if self._is_folder:
             delete_folder(self._fpath)
         else:
             delete_file(self._fpath)
@@ -311,27 +315,35 @@
     def get_temp_folderpath(self):
         return self.get_path(".temp")
     
     def create_temp_file(self): return create_temp_file(self.get_temp_folderpath())
 
     def create_temp_folder(self): return create_temp_folder(self.get_temp_folderpath())
 
-class ResourceLock(ManagedObject, FileSystemDataStore):
+FSDS = FileSystemDataStore
+Workspace = FileSystemDataStore
+
+class FileSystemLock(ManagedObject, FileSystemDataStore):
     def __init__(self, id, temp_folderpath=None):
         ManagedObject.__init__(self)
         FileSystemDataStore.__init__(self, None)
 
         # control
         self.id = id
         if temp_folderpath is None: temp_folderpath = tempfile.gettempdir()
         self.root_folderpath = os.path.join(temp_folderpath, id)
         self.lockfile = None
 
     def __del__(self):
         self.unlock()
+        FileSystemDataStore.__del__(self)
+        ManagedObject.__del__(self)
+
+    def gc(self):
+        self.unlock()
 
     @property
     def state(self):
         return self._state
 
     def lockfile_filepath(self):
         return self.get_path("lock.ctl", True)
@@ -399,33 +411,31 @@
             self.lockfile = None
             delete_file(self.lockfile_filepath())
 
             # delete parent folder
             delete_folder(self.root_folderpath)
         self._state = None
 
-    def delete(self, gc=False):
-        self.unlock()
-
     def initialize_workspace(self):
         self.cleanup_workspace()
 
     def cleanup_workspace(self):
         fpath_lockfile = self.lockfile_filepath()
         items = list_all(self.root_folderpath)
         for fpath, is_folder in items:
             print(fpath)
             if is_folder:
                 delete_folder(fpath)
             else:
-                if fpath == fpath_lockfile:
-                    print("skip")
-                    continue
+                if fpath == fpath_lockfile: continue
                 delete_file(fpath)
 
+FSL = FileSystemLock
+FSLock = FileSystemLock
+
 def parse_command_line(parts):
     """Parse command line.
 
     Syntax of command list is as:
     program <command 1> <command 2> ... [option 1] [option 2] ...
 
     Commands are required and options are optional, and commands are always
```

### Comparing `joo-0.1.0.139/lib/joo.egg-info/PKG-INFO` & `joo-0.1.0.140/lib/joo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.139
+Version: 0.1.0.140
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.139/setup.py` & `joo-0.1.0.140/setup.py`

 * *Files identical despite different names*

