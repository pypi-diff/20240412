# Comparing `tmp/py_app_dev-2.1.0.tar.gz` & `tmp/py_app_dev-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_app_dev-2.1.0.tar", max compression
+gzip compressed data, was "py_app_dev-2.1.1.tar", max compression
```

## Comparing `py_app_dev-2.1.0.tar` & `py_app_dev-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-02-18 14:53:52.329584 py_app_dev-2.1.0/LICENSE
--rw-r--r--   0        0        0     4773 2024-02-18 14:53:52.329584 py_app_dev-2.1.0/README.md
--rw-r--r--   0        0        0     2606 2024-02-18 14:53:52.993585 py_app_dev-2.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-02-18 14:53:52.965585 py_app_dev-2.1.0/src/py_app_dev/__init__.py
--rw-r--r--   0        0        0        0 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/__init__.py
--rw-r--r--   0        0        0     6223 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/cmd_line.py
--rw-r--r--   0        0        0     1007 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/docs_utils.py
--rw-r--r--   0        0        0      278 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/exceptions.py
--rw-r--r--   0        0        0     2237 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/logging.py
--rw-r--r--   0        0        0     4608 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/pipeline.py
--rw-r--r--   0        0        0     4917 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/runnable.py
--rw-r--r--   0        0        0    10513 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/scoop_wrapper.py
--rw-r--r--   0        0        0     2328 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/core/subprocess.py
--rw-r--r--   0        0        0        0 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/mvp/__init__.py
--rw-r--r--   0        0        0     1862 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/mvp/event_manager.py
--rw-r--r--   0        0        0      258 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/mvp/presenter.py
--rw-r--r--   0        0        0      174 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/mvp/view.py
--rw-r--r--   0        0        0        0 2024-02-18 14:53:52.333584 py_app_dev-2.1.0/src/py_app_dev/py.typed
--rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 py_app_dev-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-12 08:18:41.738261 py_app_dev-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4773 2024-04-12 08:18:41.738261 py_app_dev-2.1.1/README.md
+-rw-r--r--   0        0        0     2606 2024-04-12 08:18:42.418264 py_app_dev-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-12 08:18:42.390264 py_app_dev-2.1.1/src/py_app_dev/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/__init__.py
+-rw-r--r--   0        0        0     6223 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/cmd_line.py
+-rw-r--r--   0        0        0     1007 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/docs_utils.py
+-rw-r--r--   0        0        0      278 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/exceptions.py
+-rw-r--r--   0        0        0     2237 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/logging.py
+-rw-r--r--   0        0        0     4608 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/pipeline.py
+-rw-r--r--   0        0        0     4917 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/runnable.py
+-rw-r--r--   0        0        0    10609 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/scoop_wrapper.py
+-rw-r--r--   0        0        0     2328 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/core/subprocess.py
+-rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/__init__.py
+-rw-r--r--   0        0        0     1862 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/event_manager.py
+-rw-r--r--   0        0        0      258 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/presenter.py
+-rw-r--r--   0        0        0      174 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/mvp/view.py
+-rw-r--r--   0        0        0        0 2024-04-12 08:18:41.742261 py_app_dev-2.1.1/src/py_app_dev/py.typed
+-rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 py_app_dev-2.1.1/PKG-INFO
```

### Comparing `py_app_dev-2.1.0/LICENSE` & `py_app_dev-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/README.md` & `py_app_dev-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/pyproject.toml` & `py_app_dev-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-app-dev"
-version = "2.1.0"
+version = "2.1.1"
 description = "My application development modules."
 authors = ["cuinixam <me@cuinixam.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cuinixam/python-app-dev"
 documentation = "https://python-app-dev.readthedocs.io"
 classifiers = [
```

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/cmd_line.py` & `py_app_dev-2.1.1/src/py_app_dev/core/cmd_line.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/docs_utils.py` & `py_app_dev-2.1.1/src/py_app_dev/core/docs_utils.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/logging.py` & `py_app_dev-2.1.1/src/py_app_dev/core/logging.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/pipeline.py` & `py_app_dev-2.1.1/src/py_app_dev/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/runnable.py` & `py_app_dev-2.1.1/src/py_app_dev/core/runnable.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/scoop_wrapper.py` & `py_app_dev-2.1.1/src/py_app_dev/core/scoop_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,19 @@
                 bin_dirs=bin_dirs,
                 env_add_path=env_add_path,
             )
 
     def get_installed_apps(self) -> List[InstalledScoopApp]:
         installed_tools: List[InstalledScoopApp] = []
         self.logger.info(f"Looking for installed apps in {self.apps_directory}")
-        manifest_files = list(self.apps_directory.glob("*/*/manifest.json"))
+        manifest_files = [
+            file
+            for file in self.apps_directory.glob("*/*/manifest.json")
+            if "current" != file.parent.name
+        ]
 
         with ThreadPoolExecutor() as executor:
             future_to_file = {
                 executor.submit(self.parse_manifest_file, manifest_file): manifest_file
                 for manifest_file in manifest_files
             }
             for future in as_completed(future_to_file):
```

### Comparing `py_app_dev-2.1.0/src/py_app_dev/core/subprocess.py` & `py_app_dev-2.1.1/src/py_app_dev/core/subprocess.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/src/py_app_dev/mvp/event_manager.py` & `py_app_dev-2.1.1/src/py_app_dev/mvp/event_manager.py`

 * *Files identical despite different names*

### Comparing `py_app_dev-2.1.0/PKG-INFO` & `py_app_dev-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-app-dev
-Version: 2.1.0
+Version: 2.1.1
 Summary: My application development modules.
 Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT
 Author: cuinixam
 Author-email: me@cuinixam.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-app-dev Version: 2.1.0 Summary: My application
+Metadata-Version: 2.1 Name: py-app-dev Version: 2.1.1 Summary: My application
 development modules. Home-page: https://github.com/cuinixam/python-app-dev
 License: MIT Author: cuinixam Author-email: me@cuinixam.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

