# Comparing `tmp/composio_core-0.1.91.tar.gz` & `tmp/composio_core-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.91.tar", last modified: Fri Apr 12 10:14:41 2024, max compression
+gzip compressed data, was "composio_core-0.1.92.tar", last modified: Fri Apr 12 10:23:35 2024, max compression
```

## Comparing `composio_core-0.1.91.tar` & `composio_core-0.1.92.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.108548 composio_core-0.1.91/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.91/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:14:41.108273 composio_core-0.1.91/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.91/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.105044 composio_core-0.1.91/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.91/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21735 2024-04-12 10:12:57.000000 composio_core-0.1.91/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.107003 composio_core-0.1.91/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.91/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.91/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.91/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.91/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.91/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.91/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.108002 composio_core-0.1.91/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.91/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.91/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:14:41.108588 composio_core-0.1.91/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:14:00.000000 composio_core-0.1.91/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.212017 composio_core-0.1.92/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.92/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:23:35.211787 composio_core-0.1.92/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.92/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.208915 composio_core-0.1.92/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.92/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21737 2024-04-12 10:22:42.000000 composio_core-0.1.92/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.210520 composio_core-0.1.92/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.92/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.92/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.92/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.92/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.92/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.92/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.211579 composio_core-0.1.92/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.92/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.92/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:23:35.212060 composio_core-0.1.92/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:23:04.000000 composio_core-0.1.92/setup.py
```

### Comparing `composio_core-0.1.91/PKG-INFO` & `composio_core-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.91
+Version: 0.1.92
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.91/composio/composio_cli.py` & `composio_core-0.1.92/composio/composio_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     response = requests.get("https://pypi.org/pypi/composio_core/json")
     latest_pypi_version = response.json()['info']['version']
 
     console.print(f"\n Version: {installed_version} \n")
 
     if(latest_pypi_version > installed_version):
         console.print(f"\n[yellow] 🧐🧐 A newer version {latest_pypi_version} of composio-core is available. Please upgrade.[/yellow]")
-        console.print(f"\n 🔧🔧 Run [cyan]pip install --upgrade composio-core=={latest_pypi_version} [/cyan] to update.")
+        console.print(f"\n 🔧🔧 Run [cyan]pip install --upgrade composio-core=={latest_pypi_version} [/cyan] to update.\n")
 
 def print_intro():
         text = termcolor.colored('Composio', 'white', attrs=['bold'])  
         aiPlatformText = termcolor.colored('100+', 'green', attrs=['bold'])
         pinkEmojiText = termcolor.colored('hello@composio.dev', 'magenta', attrs=['bold'])
         boldNoteText = termcolor.colored('Note*', 'white', attrs=['bold'])
         print(f"""
```

### Comparing `composio_core-0.1.91/composio/sdk/core.py` & `composio_core-0.1.92/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/composio/sdk/enums.py` & `composio_core-0.1.92/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/composio/sdk/sdk.py` & `composio_core-0.1.92/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/composio/sdk/storage.py` & `composio_core-0.1.92/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/composio/sdk/utils.py` & `composio_core-0.1.92/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.92/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.91
+Version: 0.1.92
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.91/pyproject.toml` & `composio_core-0.1.92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.91/setup.py` & `composio_core-0.1.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.91",
+    version="0.1.92",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

