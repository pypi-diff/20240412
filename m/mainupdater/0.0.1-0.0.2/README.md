# Comparing `tmp/mainupdater-0.0.1.tar.gz` & `tmp/mainupdater-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainupdater-0.0.1.tar", max compression
+gzip compressed data, was "mainupdater-0.0.2.tar", max compression
```

## Comparing `mainupdater-0.0.1.tar` & `mainupdater-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rwxr-xr-x   0        0        0     1074 2024-03-04 01:06:04.000000 mainupdater-0.0.1/LICENSE
--rwxr-xr-x   0        0        0       26 2024-03-04 01:06:56.000000 mainupdater-0.0.1/README.md
--rwxr-xr-x   0        0        0      686 2024-04-12 02:48:28.000000 mainupdater-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      373 2024-04-11 16:37:30.000000 mainupdater-0.0.1/src/MainUpdater/__init__.py
--rwxr-xr-x   0        0        0      463 2024-04-12 02:54:23.000000 mainupdater-0.0.1/src/MainUpdater/example.MainUpdater
--rwxr-xr-x   0        0        0     2753 2024-04-12 04:01:16.000000 mainupdater-0.0.1/src/MainUpdater/main.py
--rwxr-xr-x   0        0        0      184 2024-04-12 04:01:53.000000 mainupdater-0.0.1/src/MainUpdater/script.py
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 mainupdater-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2024-03-04 01:06:56.000000 mainupdater-0.0.2/README.md
+-rwxr-xr-x   0        0        0      686 2024-04-12 15:30:18.000000 mainupdater-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      373 2024-04-12 15:30:06.000000 mainupdater-0.0.2/src/MainUpdater/__init__.py
+-rwxr-xr-x   0        0        0      463 2024-04-12 02:54:22.000000 mainupdater-0.0.2/src/MainUpdater/example.MainUpdater
+-rwxr-xr-x   0        0        0     2833 2024-04-12 15:29:47.000000 mainupdater-0.0.2/src/MainUpdater/main.py
+-rwxr-xr-x   0        0        0      184 2024-04-12 04:01:52.000000 mainupdater-0.0.2/src/MainUpdater/script.py
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 mainupdater-0.0.2/PKG-INFO
```

### Comparing `mainupdater-0.0.1/pyproject.toml` & `mainupdater-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mainupdater"
-version = "0.0.1"
+version = "0.0.2"
 description = "Простое обновление файлов по ссылке"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainUpdater.py"
 packages = [
     { include = "MainUpdater", from = "src" },
 ]
```

### Comparing `mainupdater-0.0.1/src/MainUpdater/main.py` & `mainupdater-0.0.2/src/MainUpdater/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os,requests
 import MainShortcuts as ms
 from traceback import print_exc
+from sys import stderr
 try:
   import progressbar
   bar=True
 except:
   bar=False
 pbar_w=[
   progressbar.Percentage(),
@@ -31,14 +32,15 @@
 def _request(method,url,**kw):
   if not "headers" in kw:kw["headers"]={}
   if "data" in kw:
     if type(kw["data"]) in [dict,list,tuple,type(True),type(False),type(None)]:
       kw["data"]=ms.json.encode(kw["data"])
       kw["headers"]["Content-Type"]="application/json"
   r=requests.request(method,url,**kw)
+  if "DEBUG" in os.environ:print(r.content,file=stderr)
   r.raise_for_status()
   return r
 def get_info(url,**kw):
   kw["stream"]=False
   r=_request("GET",url,**kw)
   info=r.json()
   r.close()
@@ -97,8 +99,8 @@
     info=ms.json.read(path)
     for k,v in info["files"].items():
       try:
         info["files"][k]=update(k,v,cli=cli)
       except:
         print_exc()
     ms.json.write(path,info)
-    
+
```

### Comparing `mainupdater-0.0.1/PKG-INFO` & `mainupdater-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainupdater
-Version: 0.0.1
+Version: 0.0.2
 Summary: Простое обновление файлов по ссылке
 Home-page: https://github.com/MainPlay-TG/MainUpdater.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

