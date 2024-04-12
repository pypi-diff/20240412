# Comparing `tmp/mainshortcuts-1.6.73.tar.gz` & `tmp/mainshortcuts-1.6.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainshortcuts-1.6.73.tar", max compression
+gzip compressed data, was "mainshortcuts-1.6.74.tar", max compression
```

## Comparing `mainshortcuts-1.6.73.tar` & `mainshortcuts-1.6.74.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.73/README.md
--rwxr-xr-x   0        0        0      696 2024-04-12 17:34:12.000000 mainshortcuts-1.6.73/pyproject.toml
--rwxr-xr-x   0        0        0     6027 2024-03-18 12:04:56.000000 mainshortcuts-1.6.73/src/MainShortcuts/MainCore.py
--rwxr-xr-x   0        0        0      937 2024-04-12 17:34:05.000000 mainshortcuts-1.6.73/src/MainShortcuts/__init__.py
--rwxr-xr-x   0        0        0      456 2024-01-13 08:00:52.000000 mainshortcuts-1.6.73/src/MainShortcuts/addon.py
--rwxr-xr-x   0        0        0     6649 2024-03-18 10:53:54.000000 mainshortcuts-1.6.73/src/MainShortcuts/cfg.py
--rwxr-xr-x   0        0        0      890 2024-03-18 10:58:02.000000 mainshortcuts-1.6.73/src/MainShortcuts/dict.py
--rwxr-xr-x   0        0        0     1467 2024-03-18 11:02:06.000000 mainshortcuts-1.6.73/src/MainShortcuts/dictplus.py
--rwxr-xr-x   0        0        0     3103 2024-03-18 11:11:00.000000 mainshortcuts-1.6.73/src/MainShortcuts/dir.py
--rwxr-xr-x   0        0        0     2852 2024-03-18 11:17:08.000000 mainshortcuts-1.6.73/src/MainShortcuts/file.py
--rwxr-xr-x   0        0        0     5877 2024-03-18 11:35:14.000000 mainshortcuts-1.6.73/src/MainShortcuts/fileobj.py
--rwxr-xr-x   0        0        0     2549 2024-04-12 17:33:55.000000 mainshortcuts-1.6.73/src/MainShortcuts/imports.py
--rwxr-xr-x   0        0        0     3592 2024-04-12 17:33:51.000000 mainshortcuts-1.6.73/src/MainShortcuts/json.py
--rwxr-xr-x   0        0        0     2120 2024-03-18 11:57:28.000000 mainshortcuts-1.6.73/src/MainShortcuts/list.py
--rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.73/src/MainShortcuts/main.py
--rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.73/src/MainShortcuts/os.py
--rwxr-xr-x   0        0        0     6163 2024-03-18 12:10:52.000000 mainshortcuts-1.6.73/src/MainShortcuts/path.py
--rwxr-xr-x   0        0        0      783 2024-03-18 12:11:44.000000 mainshortcuts-1.6.73/src/MainShortcuts/proc.py
--rwxr-xr-x   0        0        0      616 2024-03-18 12:12:40.000000 mainshortcuts-1.6.73/src/MainShortcuts/reg.py
--rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.73/src/MainShortcuts/script.py
--rwxr-xr-x   0        0        0      937 2024-03-18 12:15:06.000000 mainshortcuts-1.6.73/src/MainShortcuts/str.py
--rwxr-xr-x   0        0        0    14794 2024-03-18 12:16:26.000000 mainshortcuts-1.6.73/src/MainShortcuts/values.py
--rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.73/PKG-INFO
+-rwxr-xr-x   0        0        0     2788 2024-03-02 06:10:12.000000 mainshortcuts-1.6.74/README.md
+-rwxr-xr-x   0        0        0      696 2024-04-12 17:42:12.000000 mainshortcuts-1.6.74/pyproject.toml
+-rwxr-xr-x   0        0        0     6027 2024-03-18 12:04:56.000000 mainshortcuts-1.6.74/src/MainShortcuts/MainCore.py
+-rwxr-xr-x   0        0        0      937 2024-04-12 17:42:05.000000 mainshortcuts-1.6.74/src/MainShortcuts/__init__.py
+-rwxr-xr-x   0        0        0      456 2024-01-13 08:00:52.000000 mainshortcuts-1.6.74/src/MainShortcuts/addon.py
+-rwxr-xr-x   0        0        0     6649 2024-03-18 10:53:54.000000 mainshortcuts-1.6.74/src/MainShortcuts/cfg.py
+-rwxr-xr-x   0        0        0      890 2024-03-18 10:58:02.000000 mainshortcuts-1.6.74/src/MainShortcuts/dict.py
+-rwxr-xr-x   0        0        0     1467 2024-03-18 11:02:06.000000 mainshortcuts-1.6.74/src/MainShortcuts/dictplus.py
+-rwxr-xr-x   0        0        0     3103 2024-03-18 11:11:00.000000 mainshortcuts-1.6.74/src/MainShortcuts/dir.py
+-rwxr-xr-x   0        0        0     2852 2024-03-18 11:17:08.000000 mainshortcuts-1.6.74/src/MainShortcuts/file.py
+-rwxr-xr-x   0        0        0     5877 2024-03-18 11:35:14.000000 mainshortcuts-1.6.74/src/MainShortcuts/fileobj.py
+-rwxr-xr-x   0        0        0     2549 2024-04-12 17:41:55.000000 mainshortcuts-1.6.74/src/MainShortcuts/imports.py
+-rwxr-xr-x   0        0        0     3618 2024-04-12 17:41:50.000000 mainshortcuts-1.6.74/src/MainShortcuts/json.py
+-rwxr-xr-x   0        0        0     2120 2024-03-18 11:57:28.000000 mainshortcuts-1.6.74/src/MainShortcuts/list.py
+-rwxr-xr-x   0        0        0     1040 2024-03-21 02:56:48.000000 mainshortcuts-1.6.74/src/MainShortcuts/main.py
+-rwxr-xr-x   0        0        0       86 2024-01-17 08:34:46.000000 mainshortcuts-1.6.74/src/MainShortcuts/os.py
+-rwxr-xr-x   0        0        0     6163 2024-03-18 12:10:52.000000 mainshortcuts-1.6.74/src/MainShortcuts/path.py
+-rwxr-xr-x   0        0        0      783 2024-03-18 12:11:44.000000 mainshortcuts-1.6.74/src/MainShortcuts/proc.py
+-rwxr-xr-x   0        0        0      616 2024-03-18 12:12:40.000000 mainshortcuts-1.6.74/src/MainShortcuts/reg.py
+-rwxr-xr-x   0        0        0     1428 2024-03-27 04:45:04.000000 mainshortcuts-1.6.74/src/MainShortcuts/script.py
+-rwxr-xr-x   0        0        0      937 2024-03-18 12:15:06.000000 mainshortcuts-1.6.74/src/MainShortcuts/str.py
+-rwxr-xr-x   0        0        0    14794 2024-03-18 12:16:26.000000 mainshortcuts-1.6.74/src/MainShortcuts/values.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 mainshortcuts-1.6.74/PKG-INFO
```

### Comparing `mainshortcuts-1.6.73/README.md` & `mainshortcuts-1.6.74/README.md`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/pyproject.toml` & `mainshortcuts-1.6.74/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.poetry]
-version = "1.6.73"
+version = "1.6.74"
 name = "mainshortcuts"
 description = "Simplifying Python Built-in Commands"
 authors = [ "MainPlay TG <xbox.roman6666666666@gmail.com>",]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainShortcuts.py"
 packages = [
     { include = "MainShortcuts", from = "src" },
```

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/MainCore.py` & `mainshortcuts-1.6.74/src/MainShortcuts/MainCore.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/__init__.py` & `mainshortcuts-1.6.74/src/MainShortcuts/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """MainShortcuts - \u043D\u0435\u0431\u043E\u043B\u044C\u0448\u0430\u044F \u0431\u0438\u0431\u043B\u0438\u043E\u0442\u0435\u043A\u0430 \u0434\u043B\u044F \u0443\u043F\u0440\u043E\u0449\u0435\u043D\u0438\u044F \u043D\u0430\u043F\u0438\u0441\u0430\u043D\u0438\u044F \u043A\u043E\u0434\u0430
 \u0420\u0430\u0437\u0440\u0430\u0431\u043E\u0442\u0447\u0438\u043A: MainPlay TG
 https://t.me/MainPlay_InfoCh"""
 
-__version_tuple__=(1,6,73)
+__version_tuple__=(1,6,74)
 __depends__={
   "required":[
     "json",
     "os",
     "platform",
     "shutil",
     "subprocess",
```

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/cfg.py` & `mainshortcuts-1.6.74/src/MainShortcuts/cfg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/dict.py` & `mainshortcuts-1.6.74/src/MainShortcuts/dict.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/dictplus.py` & `mainshortcuts-1.6.74/src/MainShortcuts/dictplus.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/dir.py` & `mainshortcuts-1.6.74/src/MainShortcuts/dir.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/file.py` & `mainshortcuts-1.6.74/src/MainShortcuts/file.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/fileobj.py` & `mainshortcuts-1.6.74/src/MainShortcuts/fileobj.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/imports.py` & `mainshortcuts-1.6.74/src/MainShortcuts/imports.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/json.py` & `mainshortcuts-1.6.74/src/MainShortcuts/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import MainShortcuts.file as m_file
 import MainShortcuts.path as m_path
 import json as _json
 import sys as _sys
 _print=print
-def _obj_encoder(obj,recurse=True,func=lambda k:not k.startswith("_")):
+def _obj_encoder(obj,recurse=2,func=lambda k:not k.startswith("_")):
   """Преобразование объекта в словарь
   obj - сам объект
-  recurse - обработка рекурсивно
+  recurse - глубина рекурсивной обработки
   func - фильтр атрибутов"""
   if hasattr(obj,"to_dict"):
     to_dict=getattr(obj,"to_dict")
     if callable(to_dict):
       return to_dict()
   types=[
     str,
@@ -25,16 +25,16 @@
     ]
   d={}
   for k in dir(obj):
     if func(k):
       v=getattr(obj,k)
       if type(v) in types:
         d[k]=v
-      elif recurse:
-        d[k]=_obj_encoder(v,recurse)
+      elif recurse>0:
+        d[k]=_obj_encoder(v,recurse=recurse-1)
   return d
 def encode(data,mode="c",indent=2,sort=True,force=True,**kwargs):
   """Данные в текст JSON
   data - данные для кодирования
   mode - c/compress/min/zip: сжатый JSON
          p/pretty/max/print: развёрнутый JSON
   indent - кол-во отступов в развёрнутом JSON
```

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/list.py` & `mainshortcuts-1.6.74/src/MainShortcuts/list.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/main.py` & `mainshortcuts-1.6.74/src/MainShortcuts/main.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/path.py` & `mainshortcuts-1.6.74/src/MainShortcuts/path.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/proc.py` & `mainshortcuts-1.6.74/src/MainShortcuts/proc.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/reg.py` & `mainshortcuts-1.6.74/src/MainShortcuts/reg.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/script.py` & `mainshortcuts-1.6.74/src/MainShortcuts/script.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/str.py` & `mainshortcuts-1.6.74/src/MainShortcuts/str.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/src/MainShortcuts/values.py` & `mainshortcuts-1.6.74/src/MainShortcuts/values.py`

 * *Files identical despite different names*

### Comparing `mainshortcuts-1.6.73/PKG-INFO` & `mainshortcuts-1.6.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mainshortcuts
-Version: 1.6.73
+Version: 1.6.74
 Summary: Simplifying Python Built-in Commands
 Home-page: https://github.com/MainPlay-TG/MainShortcuts.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

