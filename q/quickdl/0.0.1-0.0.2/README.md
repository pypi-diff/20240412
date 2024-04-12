# Comparing `tmp/quickdl-0.0.1.tar.gz` & `tmp/quickdl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickdl-0.0.1.tar", last modified: Fri Apr 12 17:20:23 2024, max compression
+gzip compressed data, was "quickdl-0.0.2.tar", last modified: Fri Apr 12 20:33:26 2024, max compression
```

## Comparing `quickdl-0.0.1.tar` & `quickdl-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:20:23.258078 quickdl-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 17:20:20.000000 quickdl-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-12 17:20:23.258078 quickdl-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-12 17:20:20.000000 quickdl-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:20:23.258078 quickdl-0.0.1/quickdl/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-12 17:20:20.000000 quickdl-0.0.1/quickdl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:20:23.258078 quickdl-0.0.1/quickdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-12 17:20:23.000000 quickdl-0.0.1/quickdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 17:20:23.000000 quickdl-0.0.1/quickdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:20:23.000000 quickdl-0.0.1/quickdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 17:20:23.000000 quickdl-0.0.1/quickdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:20:23.258078 quickdl-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 17:20:20.000000 quickdl-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:26.641777 quickdl-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-12 20:33:23.000000 quickdl-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-12 20:33:26.641777 quickdl-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-12 20:33:23.000000 quickdl-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:26.637777 quickdl-0.0.2/quickdl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-12 20:33:23.000000 quickdl-0.0.2/quickdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 20:33:26.641777 quickdl-0.0.2/quickdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-12 20:33:26.000000 quickdl-0.0.2/quickdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 20:33:26.000000 quickdl-0.0.2/quickdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 20:33:26.000000 quickdl-0.0.2/quickdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 20:33:26.000000 quickdl-0.0.2/quickdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 20:33:26.641777 quickdl-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 20:33:23.000000 quickdl-0.0.2/setup.py
```

### Comparing `quickdl-0.0.1/LICENSE` & `quickdl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickdl-0.0.1/PKG-INFO` & `quickdl-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickdl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple file downloader
 Home-page: https://github.com/manbehindthemadness/quickdl
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickdl-0.0.1/README.md` & `quickdl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quickdl-0.0.1/quickdl/__init__.py` & `quickdl-0.0.2/quickdl/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     Args:
         path (Path): The path to the file.
         url (str): The URL from which to download the file.
     """
     path.mkdir(parents=True, exist_ok=True)
     file_name = url.split('/')[-1]
     file_path = path / file_name
+    if '~' in file_path.as_posix():
+        file_path = file_path.expanduser()
     if not file_path.exists():
         print(f"Downloading {path.name} from {url}...")
         with urllib.request.urlopen(url) as response, open(file_path, 'wb') as out_file:
             file_size = int(response.info().get('Content-Length', -1))
             chunk_size = 1024 * 1024  # 1 MB
             with tqdm(total=file_size, unit='B', unit_scale=True, desc=file_name) as pbar:
                 while True:
```

### Comparing `quickdl-0.0.1/quickdl.egg-info/PKG-INFO` & `quickdl-0.0.2/quickdl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickdl
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple file downloader
 Home-page: https://github.com/manbehindthemadness/quickdl
 Author: Manbehindthemadness
 Author-email: manbehindthemadness@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickdl-0.0.1/setup.py` & `quickdl-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='quickdl',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=install_requires,
     entry_points={
         'console_scripts': [
         ],
     },
     author='Manbehindthemadness',
```

