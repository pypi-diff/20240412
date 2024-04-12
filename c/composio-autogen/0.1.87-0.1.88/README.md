# Comparing `tmp/composio_autogen-0.1.87.tar.gz` & `tmp/composio_autogen-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.87.tar", last modified: Thu Apr 11 12:40:44 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.88.tar", last modified: Thu Apr 11 15:13:28 2024, max compression
```

## Comparing `composio_autogen-0.1.87.tar` & `composio_autogen-0.1.88.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.401886 composio_autogen-0.1.87/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 12:40:44.401695 composio_autogen-0.1.87/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.87/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.400518 composio_autogen-0.1.87/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.87/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     8397 2024-04-11 12:39:00.000000 composio_autogen-0.1.87/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:44.401485 composio_autogen-0.1.87/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-11 12:40:44.000000 composio_autogen-0.1.87/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 12:39:53.000000 composio_autogen-0.1.87/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:44.401931 composio_autogen-0.1.87/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-11 12:39:53.000000 composio_autogen-0.1.87/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.237318 composio_autogen-0.1.88/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 15:13:28.237112 composio_autogen-0.1.88/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.88/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.235679 composio_autogen-0.1.88/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.88/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     8397 2024-04-11 12:39:00.000000 composio_autogen-0.1.88/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:28.236902 composio_autogen-0.1.88/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-11 15:13:28.000000 composio_autogen-0.1.88/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-11 15:12:31.000000 composio_autogen-0.1.88/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:28.237362 composio_autogen-0.1.88/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-11 15:12:31.000000 composio_autogen-0.1.88/setup.py
```

### Comparing `composio_autogen-0.1.87/PKG-INFO` & `composio_autogen-0.1.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.87
+Version: 0.1.88
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.87
+Requires-Dist: composio_core===0.1.88
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.87/README.md` & `composio_autogen-0.1.88/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.87/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.88/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.87/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.88/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.87
+Version: 0.1.88
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.87
+Requires-Dist: composio_core===0.1.88
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.87/setup.py` & `composio_autogen-0.1.88/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.87",
+    version="0.1.88",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

