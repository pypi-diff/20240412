# Comparing `tmp/snakemake_interface_executor_plugins-9.1.0.tar.gz` & `tmp/snakemake_interface_executor_plugins-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_interface_executor_plugins-9.1.0.tar", max compression
+gzip compressed data, was "snakemake_interface_executor_plugins-9.1.1.tar", max compression
```

## Comparing `snakemake_interface_executor_plugins-9.1.0.tar` & `snakemake_interface_executor_plugins-9.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/LICENSE
--rw-r--r--   0        0        0     7021 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/README.md
--rw-r--r--   0        0        0     1029 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/pyproject.toml
--rw-r--r--   0        0        0      161 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/__init__.py
--rw-r--r--   0        0        0      290 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/_common.py
--rw-r--r--   0        0        0      507 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/cli.py
--rw-r--r--   0        0        0      641 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/dag.py
--rw-r--r--   0        0        0      145 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/__init__.py
--rw-r--r--   0        0        0     3863 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/base.py
--rw-r--r--   0        0        0       49 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/jobscript.sh
--rw-r--r--   0        0        0     6304 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/real.py
--rw-r--r--   0        0        0    10210 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/remote.py
--rw-r--r--   0        0        0     2779 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/jobs.py
--rw-r--r--   0        0        0      434 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/logging.py
--rw-r--r--   0        0        0      403 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/persistence.py
--rw-r--r--   0        0        0     2009 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/registry/__init__.py
--rw-r--r--   0        0        0      913 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/registry/plugin.py
--rw-r--r--   0        0        0      327 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/scheduler.py
--rw-r--r--   0        0        0     5826 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/settings.py
--rw-r--r--   0        0        0     4749 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/utils.py
--rw-r--r--   0        0        0     2141 2024-03-26 16:59:52.574608 snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/workflow.py
--rw-r--r--   0        0        0     7717 1970-01-01 00:00:00.000000 snakemake_interface_executor_plugins-9.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/LICENSE
+-rw-r--r--   0        0        0     7021 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/README.md
+-rw-r--r--   0        0        0     1029 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/pyproject.toml
+-rw-r--r--   0        0        0      161 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/__init__.py
+-rw-r--r--   0        0        0      290 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/_common.py
+-rw-r--r--   0        0        0      507 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/cli.py
+-rw-r--r--   0        0        0      641 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/dag.py
+-rw-r--r--   0        0        0      145 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/__init__.py
+-rw-r--r--   0        0        0     3863 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/base.py
+-rw-r--r--   0        0        0       49 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/jobscript.sh
+-rw-r--r--   0        0        0     6304 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/real.py
+-rw-r--r--   0        0        0    10448 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/remote.py
+-rw-r--r--   0        0        0     2779 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/jobs.py
+-rw-r--r--   0        0        0      434 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/logging.py
+-rw-r--r--   0        0        0      403 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/persistence.py
+-rw-r--r--   0        0        0     2009 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/registry/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/registry/plugin.py
+-rw-r--r--   0        0        0      327 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/scheduler.py
+-rw-r--r--   0        0        0     5826 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/settings.py
+-rw-r--r--   0        0        0     4749 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/utils.py
+-rw-r--r--   0        0        0     2141 2024-04-12 11:00:03.818553 snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/workflow.py
+-rw-r--r--   0        0        0     7717 1970-01-01 00:00:00.000000 snakemake_interface_executor_plugins-9.1.1/PKG-INFO
```

### Comparing `snakemake_interface_executor_plugins-9.1.0/LICENSE` & `snakemake_interface_executor_plugins-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/README.md` & `snakemake_interface_executor_plugins-9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/pyproject.toml` & `snakemake_interface_executor_plugins-9.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Johannes Köster <johannes.koester@uni-due.de>"]
 description = "This package provides a stable interface for interactions between Snakemake and its executor plugins."
 license = "MIT"
 name = "snakemake-interface-executor-plugins"
 packages = [{include = "snakemake_interface_executor_plugins"}]
 readme = "README.md"
-version = "9.1.0"
+version = "9.1.1"
 
 [tool.poetry.dependencies]
 argparse-dataclass = "^2.0.0"
 python = "^3.11"
 throttler = "^1.2.2"
 snakemake-interface-common = "^1.12.0"
```

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/dag.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/dag.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/base.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/base.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/real.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/real.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/executors/remote.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/executors/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,19 @@
             period=max_status_checks_frac.denominator,
         )
 
         self.__post_init__()
 
     @property
     def cores(self):
+        cores = self.workflow.resource_settings.cores
+        # if constrained, pass this info to the job
+        if cores is not None and cores != sys.maxsize:
+            return cores
+        # otherwise, use whatever the node provides
         return "all"
 
     def cancel(self):
         with self.lock:
             active_jobs = list(self.active_jobs)
         self.cancel_jobs(active_jobs)
         self.shutdown()
```

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/jobs.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/jobs.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/registry/__init__.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/registry/plugin.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/registry/plugin.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/settings.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/utils.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/snakemake_interface_executor_plugins/workflow.py` & `snakemake_interface_executor_plugins-9.1.1/snakemake_interface_executor_plugins/workflow.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_executor_plugins-9.1.0/PKG-INFO` & `snakemake_interface_executor_plugins-9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-interface-executor-plugins
-Version: 9.1.0
+Version: 9.1.1
 Summary: This package provides a stable interface for interactions between Snakemake and its executor plugins.
 License: MIT
 Author: Johannes Köster
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

