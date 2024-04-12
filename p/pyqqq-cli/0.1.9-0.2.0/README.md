# Comparing `tmp/pyqqq_cli-0.1.9.tar.gz` & `tmp/pyqqq_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.1.9.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.2.0.tar", max compression
```

## Comparing `pyqqq_cli-0.1.9.tar` & `pyqqq_cli-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      937 2024-03-26 03:56:47.680900 pyqqq_cli-0.1.9/README.md
--rw-r--r--   0        0        0      655 2024-04-12 07:50:19.019879 pyqqq_cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      358 2024-04-12 07:34:36.984208 pyqqq_cli-0.1.9/qupiato/cli/config.py
--rw-r--r--   0        0        0     6353 2024-04-12 07:50:13.466796 pyqqq_cli-0.1.9/qupiato/cli/main.py
--rw-r--r--   0        0        0     4459 2024-04-12 02:18:24.801494 pyqqq_cli-0.1.9/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      937 2024-03-26 03:56:47.680900 pyqqq_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      655 2024-04-12 07:54:14.026822 pyqqq_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-04-12 07:34:36.984208 pyqqq_cli-0.2.0/qupiato/cli/config.py
+-rw-r--r--   0        0        0     6353 2024-04-12 07:50:13.466796 pyqqq_cli-0.2.0/qupiato/cli/main.py
+-rw-r--r--   0        0        0     4459 2024-04-12 02:18:24.801494 pyqqq_cli-0.2.0/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.0/PKG-INFO
```

### Comparing `pyqqq_cli-0.1.9/README.md` & `pyqqq_cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.1.9/pyproject.toml` & `pyqqq_cli-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.1.9"
+version = "0.2.0"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq_cli-0.1.9/qupiato/cli/main.py` & `pyqqq_cli-0.2.0/qupiato/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.1.9/qupiato/cli/utils.py` & `pyqqq_cli-0.2.0/qupiato/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.1.9/PKG-INFO` & `pyqqq_cli-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.1.9
+Version: 0.2.0
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

