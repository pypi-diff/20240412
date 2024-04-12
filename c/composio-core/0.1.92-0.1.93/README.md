# Comparing `tmp/composio_core-0.1.92.tar.gz` & `tmp/composio_core-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.92.tar", last modified: Fri Apr 12 10:23:35 2024, max compression
+gzip compressed data, was "composio_core-0.1.93.tar", last modified: Fri Apr 12 10:27:11 2024, max compression
```

## Comparing `composio_core-0.1.92.tar` & `composio_core-0.1.93.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.212017 composio_core-0.1.92/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.92/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:23:35.211787 composio_core-0.1.92/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.92/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.208915 composio_core-0.1.92/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.92/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21737 2024-04-12 10:22:42.000000 composio_core-0.1.92/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.210520 composio_core-0.1.92/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.92/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.92/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.92/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.92/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.92/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.92/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:23:35.211579 composio_core-0.1.92/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:23:35.000000 composio_core-0.1.92/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.92/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.92/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:23:35.212060 composio_core-0.1.92/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:23:04.000000 composio_core-0.1.92/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.024458 composio_core-0.1.93/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.93/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:27:11.024204 composio_core-0.1.93/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.93/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.022176 composio_core-0.1.93/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.93/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21929 2024-04-12 10:26:25.000000 composio_core-0.1.93/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.022969 composio_core-0.1.93/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.93/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.93/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.93/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.93/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.93/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.93/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:27:11.023995 composio_core-0.1.93/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:27:11.000000 composio_core-0.1.93/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.93/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.93/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:27:11.024515 composio_core-0.1.93/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:27:04.000000 composio_core-0.1.93/setup.py
```

### Comparing `composio_core-0.1.92/PKG-INFO` & `composio_core-0.1.93/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.92
+Version: 0.1.93
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.92/composio/composio_cli.py` & `composio_core-0.1.93/composio/composio_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import sys
 from beaupy.spinners import Spinner, DOTS
 from rich.console import Console
 from uuid import getnode as get_mac
 
 import termcolor
-from .sdk.storage import get_user_connection, save_api_key, save_user_connection
+from .sdk.storage import get_base_url, get_user_connection, save_api_key, save_user_connection
 from .sdk.core import ComposioCore, UnauthorizedAccessException
 from .sdk.utils import generate_enums, generate_enums_beta
 from rich.table import Table
 
 import webbrowser
 
 from importlib.metadata import version
@@ -115,18 +115,20 @@
     if client.is_authenticated():
         console.print("Already authenticated. Use [green]composio-cli logout[/green] to log out.\n")
         return
     
     console.print(f"\n[green]> Authenticating...[/green]\n")
     try:
         cli_key = client.generate_cli_auth_session()
+        base_url = get_base_url()
+        frontend_url = f"https://app.composio.dev/?cliKey={cli_key}" if base_url == 'https://backend.composio.dev/api' else f"https://hermes-frontend-git-master-composio.vercel.app/?cliKey={cli_key}"
         console.print(f"> Redirecting you to the login page. Please login using the following link:\n")
-        console.print(f"[green]https://app.composio.dev/?cliKey={cli_key}[/green]\n")
+        console.print(f"[green]{frontend_url}[/green]\n")
         if not should_disable_webbrowser_open:
-            webbrowser.open(f"https://app.composio.dev/?cliKey={cli_key}")
+            webbrowser.open(f"{frontend_url}")
 
         for attempt in range(3):
             try:
                 session_data = client.verify_cli_auth_session(cli_key, input("> Enter the code: "))
                 api_key = session_data.get('apiKey')
                 if api_key:
                     save_api_key(api_key)
```

### Comparing `composio_core-0.1.92/composio/sdk/core.py` & `composio_core-0.1.93/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/composio/sdk/enums.py` & `composio_core-0.1.93/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/composio/sdk/sdk.py` & `composio_core-0.1.93/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/composio/sdk/storage.py` & `composio_core-0.1.93/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/composio/sdk/utils.py` & `composio_core-0.1.93/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.93/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.92
+Version: 0.1.93
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.92/pyproject.toml` & `composio_core-0.1.93/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.92/setup.py` & `composio_core-0.1.93/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.92",
+    version="0.1.93",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

