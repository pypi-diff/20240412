# Comparing `tmp/htagui-0.1.0.tar.gz` & `tmp/htagui-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.1.0.tar", max compression
+gzip compressed data, was "htagui-0.1.1.tar", max compression
```

## Comparing `htagui-0.1.0.tar` & `htagui-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-11 18:19:53.616115 htagui-0.1.0/LICENSE
--rw-r--r--   0        0        0     6445 2024-04-11 18:19:53.616115 htagui-0.1.0/README.md
--rw-r--r--   0        0        0     1113 2024-04-11 18:19:54.152113 htagui-0.1.0/htagui/__init__.py
--rw-r--r--   0        0        0     3549 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/basics/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/common.py
--rw-r--r--   0        0        0     5335 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/form.py
--rw-r--r--   0        0        0     2075 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-11 18:19:54.152113 htagui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7678 1970-01-01 00:00:00.000000 htagui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-12 06:29:42.745061 htagui-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6586 2024-04-12 06:29:42.745061 htagui-0.1.1/README.md
+-rw-r--r--   0        0        0     1113 2024-04-12 06:29:43.277064 htagui-0.1.1/htagui/__init__.py
+-rw-r--r--   0        0        0     3549 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/common.py
+-rw-r--r--   0        0        0     5335 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/form.py
+-rw-r--r--   0        0        0     8884 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-12 06:29:42.745061 htagui-0.1.1/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-12 06:29:43.277064 htagui-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 htagui-0.1.1/PKG-INFO
```

### Comparing `htagui-0.1.0/LICENSE` & `htagui-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/README.md` & `htagui-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 <a href="https://pypi.org/project/htagui/">
     <img src="https://badge.fury.io/py/htagui.svg?x" alt="Package version">
 </a>
 
 **roadmap**
 
+ - provide a darker theme css
  - test test & test, to be rock solid
  - be available in htag4brython too, with the same apis.
- - perhaps provide version using shoelace web component, or simple bulma styles ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
+ - perhaps provide version using "shoelace web components", or "simple bulma styles" (like htbulma) ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
 
 
 **INSTALL**
 ```bash
-python3 -m pip install -U htag htagui
+python3 -m pip install -U htagui
 ```
-
+**note**: it will install htag and htagui, and provide the `ui` in the htag namespace (`htag.ui`)
 
 A hello world could be :
 
 ```python
 from htag import Tag, Runner, ui
 
 class MyApp(ui.App):
@@ -72,15 +73,15 @@
 ## Object Input
 
 A simple surcharge of Tag.input(...), to define a css class 
 
 
 ```python
 import htagui as ui
-self <= ui.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
+self <= ui.Input(_value="my value", _name="myfield", _class="myclass", _required=True )
 ```
 
 ## Object Spinner
 
 A spinner object.
 
 ```python
```

### Comparing `htagui-0.1.0/htagui/__init__.py` & `htagui-0.1.1/htagui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.1.0" # auto updated
+__version__ = "0.1.1" # auto updated
 
 from htag import Tag
 ########################################################################################
 from .basics import Button,Input,Menu,Spinner,Select
 ########################################################################################
 from .form import Form
 from .tabs import Tabs
```

### Comparing `htagui-0.1.0/htagui/basics/__init__.py` & `htagui-0.1.1/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/htagui/common.py` & `htagui-0.1.1/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/htagui/dialog.py` & `htagui-0.1.1/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/htagui/flex.py` & `htagui-0.1.1/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/htagui/form.py` & `htagui-0.1.1/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/htagui/tabs.py` & `htagui-0.1.1/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.1.0/pyproject.toml` & `htagui-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.1.0" # auto-updated
+version = "0.1.1" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.1.0/PKG-INFO` & `htagui-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.1.0
+Version: 0.1.1
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -35,24 +35,25 @@
 
 <a href="https://pypi.org/project/htagui/">
     <img src="https://badge.fury.io/py/htagui.svg?x" alt="Package version">
 </a>
 
 **roadmap**
 
+ - provide a darker theme css
  - test test & test, to be rock solid
  - be available in htag4brython too, with the same apis.
- - perhaps provide version using shoelace web component, or simple bulma styles ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
+ - perhaps provide version using "shoelace web components", or "simple bulma styles" (like htbulma) ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
 
 
 **INSTALL**
 ```bash
-python3 -m pip install -U htag htagui
+python3 -m pip install -U htagui
 ```
-
+**note**: it will install htag and htagui, and provide the `ui` in the htag namespace (`htag.ui`)
 
 A hello world could be :
 
 ```python
 from htag import Tag, Runner, ui
 
 class MyApp(ui.App):
@@ -99,15 +100,15 @@
 ## Object Input
 
 A simple surcharge of Tag.input(...), to define a css class 
 
 
 ```python
 import htagui as ui
-self <= ui.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
+self <= ui.Input(_value="my value", _name="myfield", _class="myclass", _required=True )
 ```
 
 ## Object Spinner
 
 A spinner object.
 
 ```python
```

