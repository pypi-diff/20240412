# Comparing `tmp/composio_core-0.1.93.tar.gz` & `tmp/composio_core-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.93.tar", last modified: Fri Apr 12 10:27:11 2024, max compression
+gzip compressed data, was "composio_core-0.1.94.tar", last modified: Fri Apr 12 13:10:24 2024, max compression
```

## Comparing `composio_core-0.1.93.tar` & `composio_core-0.1.94.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.024458 composio_core-0.1.93/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.93/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:27:11.024204 composio_core-0.1.93/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.93/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.022176 composio_core-0.1.93/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.93/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21929 2024-04-12 10:26:25.000000 composio_core-0.1.93/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.022969 composio_core-0.1.93/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.93/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.93/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.93/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.93/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.93/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.93/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.023995 composio_core-0.1.93/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.93/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.93/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:27:11.024515 composio_core-0.1.93/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:27:04.000000 composio_core-0.1.93/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.538917 composio_core-0.1.94/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.94/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:10:24.538689 composio_core-0.1.94/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.94/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.536001 composio_core-0.1.94/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.94/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21929 2024-04-12 10:26:25.000000 composio_core-0.1.94/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.537402 composio_core-0.1.94/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.94/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.94/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.94/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.94/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.94/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.94/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.538438 composio_core-0.1.94/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.94/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.94/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 13:10:24.538969 composio_core-0.1.94/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 13:10:03.000000 composio_core-0.1.94/setup.py
```

### Comparing `composio_core-0.1.93/PKG-INFO` & `composio_core-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.93
+Version: 0.1.94
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.93/composio/composio_cli.py` & `composio_core-0.1.94/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/composio/sdk/core.py` & `composio_core-0.1.94/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/composio/sdk/sdk.py` & `composio_core-0.1.94/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/composio/sdk/storage.py` & `composio_core-0.1.94/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/composio/sdk/utils.py` & `composio_core-0.1.94/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.94/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.93
+Version: 0.1.94
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.93/pyproject.toml` & `composio_core-0.1.94/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.93/setup.py` & `composio_core-0.1.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.93",
+    version="0.1.94",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

