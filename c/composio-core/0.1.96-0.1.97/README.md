# Comparing `tmp/composio_core-0.1.96.tar.gz` & `tmp/composio_core-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.96.tar", last modified: Fri Apr 12 15:12:16 2024, max compression
+gzip compressed data, was "composio_core-0.1.97.tar", last modified: Fri Apr 12 15:19:11 2024, max compression
```

## Comparing `composio_core-0.1.96.tar` & `composio_core-0.1.97.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:12:16.423446 composio_core-0.1.96/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.96/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:12:16.423222 composio_core-0.1.96/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.96/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:12:16.419890 composio_core-0.1.96/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.96/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21879 2024-04-12 13:27:15.000000 composio_core-0.1.96/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:12:16.421934 composio_core-0.1.96/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.96/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7042 2024-04-12 13:36:37.000000 composio_core-0.1.96/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.96/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    19094 2024-04-12 13:26:45.000000 composio_core-0.1.96/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.1.96/composio/sdk/shared.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.96/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.96/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:12:16.422977 composio_core-0.1.96/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 15:12:16.000000 composio_core-0.1.96/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.1.96/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.1.96/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:12:16.423489 composio_core-0.1.96/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 15:12:06.000000 composio_core-0.1.96/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:19:11.203873 composio_core-0.1.97/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.97/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:19:11.203638 composio_core-0.1.97/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.97/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:19:11.200335 composio_core-0.1.97/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.97/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21879 2024-04-12 13:27:15.000000 composio_core-0.1.97/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:19:11.202435 composio_core-0.1.97/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.97/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7042 2024-04-12 13:36:37.000000 composio_core-0.1.97/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.97/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    19094 2024-04-12 13:26:45.000000 composio_core-0.1.97/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:36:37.000000 composio_core-0.1.97/composio/sdk/shared.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.97/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.97/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:19:11.203417 composio_core-0.1.97/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      797 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      489 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      103 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 15:19:11.000000 composio_core-0.1.97/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      528 2024-04-12 15:10:44.000000 composio_core-0.1.97/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      130 2024-04-12 15:11:16.000000 composio_core-0.1.97/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 15:19:11.203914 composio_core-0.1.97/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 15:17:53.000000 composio_core-0.1.97/setup.py
```

### Comparing `composio_core-0.1.96/PKG-INFO` & `composio_core-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.96
+Version: 0.1.97
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.96/composio/composio_cli.py` & `composio_core-0.1.97/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio/sdk/core.py` & `composio_core-0.1.97/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio/sdk/enums.py` & `composio_core-0.1.97/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio/sdk/sdk.py` & `composio_core-0.1.97/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio/sdk/storage.py` & `composio_core-0.1.97/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio/sdk/utils.py` & `composio_core-0.1.97/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.97/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.96
+Version: 0.1.97
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.96/pyproject.toml` & `composio_core-0.1.97/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.96/setup.py` & `composio_core-0.1.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.96",
+    version="0.1.97",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

