# Comparing `tmp/mainupdater-0.0.2.tar.gz` & `tmp/mainupdater-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainupdater-0.0.2.tar", max compression
+gzip compressed data, was "mainupdater-0.0.3.tar", max compression
```

## Comparing `mainupdater-0.0.2.tar` & `mainupdater-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0       26 2024-03-04 01:06:56.000000 mainupdater-0.0.2/README.md
--rwxr-xr-x   0        0        0      686 2024-04-12 15:30:18.000000 mainupdater-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      373 2024-04-12 15:30:06.000000 mainupdater-0.0.2/src/MainUpdater/__init__.py
--rwxr-xr-x   0        0        0      463 2024-04-12 02:54:22.000000 mainupdater-0.0.2/src/MainUpdater/example.MainUpdater
--rwxr-xr-x   0        0        0     2833 2024-04-12 15:29:47.000000 mainupdater-0.0.2/src/MainUpdater/main.py
--rwxr-xr-x   0        0        0      184 2024-04-12 04:01:52.000000 mainupdater-0.0.2/src/MainUpdater/script.py
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 mainupdater-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2024-03-04 01:06:56.000000 mainupdater-0.0.3/README.md
+-rwxr-xr-x   0        0        0      686 2024-04-12 15:35:12.000000 mainupdater-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      373 2024-04-12 15:35:07.000000 mainupdater-0.0.3/src/MainUpdater/__init__.py
+-rwxr-xr-x   0        0        0      463 2024-04-12 02:54:22.000000 mainupdater-0.0.3/src/MainUpdater/example.MainUpdater
+-rwxr-xr-x   0        0        0     2802 2024-04-12 15:34:53.000000 mainupdater-0.0.3/src/MainUpdater/main.py
+-rwxr-xr-x   0        0        0      184 2024-04-12 04:01:52.000000 mainupdater-0.0.3/src/MainUpdater/script.py
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 mainupdater-0.0.3/PKG-INFO
```

### Comparing `mainupdater-0.0.2/pyproject.toml` & `mainupdater-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mainupdater"
-version = "0.0.2"
+version = "0.0.3"
 description = "Простое обновление файлов по ссылке"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainUpdater.py"
 packages = [
     { include = "MainUpdater", from = "src" },
 ]
```

### Comparing `mainupdater-0.0.2/src/MainUpdater/main.py` & `mainupdater-0.0.3/src/MainUpdater/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,20 @@
 def _request(method,url,**kw):
   if not "headers" in kw:kw["headers"]={}
   if "data" in kw:
     if type(kw["data"]) in [dict,list,tuple,type(True),type(False),type(None)]:
       kw["data"]=ms.json.encode(kw["data"])
       kw["headers"]["Content-Type"]="application/json"
   r=requests.request(method,url,**kw)
-  if "DEBUG" in os.environ:print(r.content,file=stderr)
   r.raise_for_status()
   return r
-def get_info(url,**kw):
+def get_info(url,file,**kw):
   kw["stream"]=False
   r=_request("GET",url,**kw)
-  info=r.json()
+  info=r.json()["files"][file]
   r.close()
   if info["info"]["url"]!=url:
     kw={}
     if "request" in info["info"]:
       kw=info["info"]["request"]
     info=get_info(info["info"]["url"],**kw)
   return info
@@ -75,15 +74,15 @@
 def update(path,info_old,cli=False):
   if cli:
     print('Updating file "{}"'.format(path))
     print("Getting information about a file")
   kw={}
   if "request" in info_old["info"]:
     kw=info["info"]["request"]
-  info_new=get_info(info_old["info"]["url"],**kw)
+  info_new=get_info(info_old["info"]["url"],path,**kw)
   kw={}
   if "request" in info["file"]:
     kw=info["file"]["request"]
   if ms.path.exists(path):
     if info_new["info"]["version"]>info_old["info"]["version"]:
       download_url(info_new["file"]["url"],path,cli=cli,**kw)
   else:
```

### Comparing `mainupdater-0.0.2/PKG-INFO` & `mainupdater-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainupdater
-Version: 0.0.2
+Version: 0.0.3
 Summary: Простое обновление файлов по ссылке
 Home-page: https://github.com/MainPlay-TG/MainUpdater.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

