# Comparing `tmp/htagui-0.1.1.tar.gz` & `tmp/htagui-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.1.1.tar", max compression
+gzip compressed data, was "htagui-0.1.2.tar", max compression
```

## Comparing `htagui-0.1.1.tar` & `htagui-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-12 06:29:42.745061 htagui-0.1.1/LICENSE
--rw-r--r--   0        0        0     6586 2024-04-12 06:29:42.745061 htagui-0.1.1/README.md
--rw-r--r--   0        0        0     1113 2024-04-12 06:29:43.277064 htagui-0.1.1/htagui/__init__.py
--rw-r--r--   0        0        0     3549 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/basics/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/common.py
--rw-r--r--   0        0        0     5335 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/form.py
--rw-r--r--   0        0        0     8884 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-12 06:29:43.277064 htagui-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 htagui-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 10:32:57.364749 htagui-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6586 2024-04-12 10:32:57.364749 htagui-0.1.2/README.md
+-rw-r--r--   0        0        0     1113 2024-04-12 10:32:57.612750 htagui-0.1.2/htagui/__init__.py
+-rw-r--r--   0        0        0     3549 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/common.py
+-rw-r--r--   0        0        0     5344 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/form.py
+-rw-r--r--   0        0        0     8884 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-12 10:32:57.368749 htagui-0.1.2/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-12 10:32:57.612750 htagui-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 htagui-0.1.2/PKG-INFO
```

### Comparing `htagui-0.1.1/LICENSE` & `htagui-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/README.md` & `htagui-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/__init__.py` & `htagui-0.1.2/htagui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.1.1" # auto updated
+__version__ = "0.1.2" # auto updated
 
 from htag import Tag
 ########################################################################################
 from .basics import Button,Input,Menu,Spinner,Select
 ########################################################################################
 from .form import Form
 from .tabs import Tabs
```

### Comparing `htagui-0.1.1/htagui/basics/__init__.py` & `htagui-0.1.2/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/common.py` & `htagui-0.1.2/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/dialog.py` & `htagui-0.1.2/htagui/dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         def init(self,main,obj,trbl:tuple=("30%","30%","","30%"),closable=True,radius=6):
             t,r,b,l = trbl
             if closable:
                 bc=Tag.button("X",_onclick=main.stepevent(),_style="float:right;border-radius:50%;border:0px;cursor:pointer;background:white")
                 self <= Voile(_onmousedown=main.stepevent())
                 self <= Tag.div( [bc,obj] ,_style=f"position:fixed;top:{t};bottom:{b};left:{l};right:{r};background:white;border-radius:{radius}px;box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;;z-index:1001;padding:10px")
             else:
-                self <= Voile(_style="cursor:wait")
-                self <= Tag.div( obj ,_style=f"position:fixed;top:{t};right:{r};z-index:1001;transform:translate(50%,50%);")
+                self <= Voile(_style="cursor:not-allowed;")
+                self <= Tag.div( obj ,_style=f"position:fixed;top:{t};right:{r};z-index:1001;transform:translate(50%,-50%);")
 
     class ModalConfirm(Modal):
         def __init__(self,main,obj,cb):
             def call(ev):
                 cb(ev.target.val)
                 main.step()
             box=[
```

### Comparing `htagui-0.1.1/htagui/flex.py` & `htagui-0.1.2/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/form.py` & `htagui-0.1.2/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/splitters.py` & `htagui-0.1.2/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/htagui/tabs.py` & `htagui-0.1.2/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.1/pyproject.toml` & `htagui-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.1.1" # auto-updated
+version = "0.1.2" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.1.1/PKG-INFO` & `htagui-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.1.1
+Version: 0.1.2
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

