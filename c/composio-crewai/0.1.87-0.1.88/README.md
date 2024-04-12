# Comparing `tmp/composio_crewai-0.1.87.tar.gz` & `tmp/composio_crewai-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.1.87.tar", last modified: Thu Apr 11 12:40:36 2024, max compression
+gzip compressed data, was "composio_crewai-0.1.88.tar", last modified: Thu Apr 11 15:13:21 2024, max compression
```

## Comparing `composio_crewai-0.1.87.tar` & `composio_crewai-0.1.88.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:36.473336 composio_crewai-0.1.87/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-11 12:40:36.473122 composio_crewai-0.1.87/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-02 18:29:17.000000 composio_crewai-0.1.87/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:36.471895 composio_crewai-0.1.87/composio_crewai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       89 2024-04-02 18:29:17.000000 composio_crewai-0.1.87/composio_crewai/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:36.472911 composio_crewai-0.1.87/composio_crewai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-11 12:40:36.000000 composio_crewai-0.1.87/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-11 12:40:36.000000 composio_crewai-0.1.87/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:36.000000 composio_crewai-0.1.87/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       28 2024-04-11 12:40:36.000000 composio_crewai-0.1.87/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-11 12:40:36.000000 composio_crewai-0.1.87/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      276 2024-04-11 12:39:53.000000 composio_crewai-0.1.87/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:36.473377 composio_crewai-0.1.87/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-11 12:39:53.000000 composio_crewai-0.1.87/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:21.014189 composio_crewai-0.1.88/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-11 15:13:21.013994 composio_crewai-0.1.88/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-02 18:29:17.000000 composio_crewai-0.1.88/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:21.012828 composio_crewai-0.1.88/composio_crewai/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       89 2024-04-02 18:29:17.000000 composio_crewai-0.1.88/composio_crewai/__init__.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:21.013808 composio_crewai-0.1.88/composio_crewai.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-11 15:13:21.000000 composio_crewai-0.1.88/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-11 15:13:21.000000 composio_crewai-0.1.88/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:21.000000 composio_crewai-0.1.88/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       28 2024-04-11 15:13:21.000000 composio_crewai-0.1.88/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-11 15:13:21.000000 composio_crewai-0.1.88/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      276 2024-04-11 15:12:31.000000 composio_crewai-0.1.88/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:21.014229 composio_crewai-0.1.88/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-11 15:12:31.000000 composio_crewai-0.1.88/setup.py
```

### Comparing `composio_crewai-0.1.87/PKG-INFO` & `composio_crewai-0.1.88/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.87
+Version: 0.1.88
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.87
+Requires-Dist: composio_langchain===0.1.88
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.87/README.md` & `composio_crewai-0.1.88/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.1.87/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.1.88/composio_crewai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.87
+Version: 0.1.88
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.87
+Requires-Dist: composio_langchain===0.1.88
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.87/setup.py` & `composio_crewai-0.1.88/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.1.87",
+    version="0.1.88",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

