# Comparing `tmp/composio_core-0.1.90.tar.gz` & `tmp/composio_core-0.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.90.tar", last modified: Fri Apr 12 10:06:08 2024, max compression
+gzip compressed data, was "composio_core-0.1.91.tar", last modified: Fri Apr 12 10:14:41 2024, max compression
```

## Comparing `composio_core-0.1.90.tar` & `composio_core-0.1.91.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.855112 composio_core-0.1.90/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.90/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:06:08.854892 composio_core-0.1.90/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.90/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.852859 composio_core-0.1.90/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.90/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    20235 2024-04-12 09:44:09.000000 composio_core-0.1.90/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.853729 composio_core-0.1.90/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.90/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.90/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.90/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.90/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.90/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.90/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.854648 composio_core-0.1.90/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.90/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.90/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:06:08.855242 composio_core-0.1.90/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:06:05.000000 composio_core-0.1.90/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.108548 composio_core-0.1.91/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.91/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:14:41.108273 composio_core-0.1.91/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.91/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.105044 composio_core-0.1.91/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.91/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21735 2024-04-12 10:12:57.000000 composio_core-0.1.91/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.107003 composio_core-0.1.91/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.91/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.91/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.91/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.91/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.91/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.91/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:14:41.108002 composio_core-0.1.91/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:14:41.000000 composio_core-0.1.91/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.91/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.91/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:14:41.108588 composio_core-0.1.91/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:14:00.000000 composio_core-0.1.91/setup.py
```

### Comparing `composio_core-0.1.90/PKG-INFO` & `composio_core-0.1.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.90
+Version: 0.1.91
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.90/composio/composio_cli.py` & `composio_core-0.1.91/composio/composio_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import argparse
 import json
 import os
 import sys
 from beaupy.spinners import Spinner, DOTS
 from rich.console import Console
 from uuid import getnode as get_mac
+
+import termcolor
 from .sdk.storage import get_user_connection, save_api_key, save_user_connection
 from .sdk.core import ComposioCore, UnauthorizedAccessException
 from .sdk.utils import generate_enums, generate_enums_beta
 from rich.table import Table
 
 import webbrowser
 
@@ -404,14 +406,30 @@
     console.print(f"\n Version: {installed_version} \n")
 
     if(latest_pypi_version > installed_version):
         console.print(f"\n[yellow] 🧐🧐 A newer version {latest_pypi_version} of composio-core is available. Please upgrade.[/yellow]")
         console.print(f"\n 🔧🔧 Run [cyan]pip install --upgrade composio-core=={latest_pypi_version} [/cyan] to update.")
 
 def print_intro():
+        text = termcolor.colored('Composio', 'white', attrs=['bold'])  
+        aiPlatformText = termcolor.colored('100+', 'green', attrs=['bold'])
+        pinkEmojiText = termcolor.colored('hello@composio.dev', 'magenta', attrs=['bold'])
+        boldNoteText = termcolor.colored('Note*', 'white', attrs=['bold'])
+        print(f"""
+┌───────────────────────────────────────────────────────────────────────────┐
+│                                                                           │
+│                                       {text}                            │
+│                                                                           │
+│                     Plug {aiPlatformText} platforms in your agent                     │
+│                                                                           │
+│ {boldNoteText}: This package is in closed beta, please contact {pinkEmojiText}  │
+│        to get early access.                                               │
+│                                                                           │
+└───────────────────────────────────────────────────────────────────────────┘
+        """)
         check_for_updates()
 
 def main():
     print_intro()
 
     args = parse_arguments()
```

### Comparing `composio_core-0.1.90/composio/sdk/core.py` & `composio_core-0.1.91/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/composio/sdk/enums.py` & `composio_core-0.1.91/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/composio/sdk/sdk.py` & `composio_core-0.1.91/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/composio/sdk/storage.py` & `composio_core-0.1.91/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/composio/sdk/utils.py` & `composio_core-0.1.91/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.91/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.90
+Version: 0.1.91
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.90/pyproject.toml` & `composio_core-0.1.91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.90/setup.py` & `composio_core-0.1.91/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.90",
+    version="0.1.91",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

