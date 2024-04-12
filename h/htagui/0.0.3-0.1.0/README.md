# Comparing `tmp/htagui-0.0.3.tar.gz` & `tmp/htagui-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.0.3.tar", max compression
+gzip compressed data, was "htagui-0.1.0.tar", max compression
```

## Comparing `htagui-0.0.3.tar` & `htagui-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1065 2024-04-11 17:50:46.027510 htagui-0.0.3/LICENSE
--rw-r--r--   0        0        0     6371 2024-04-11 17:50:46.027510 htagui-0.0.3/README.md
--rw-r--r--   0        0        0     1113 2024-04-11 17:50:46.267511 htagui-0.0.3/htagui/__init__.py
--rw-r--r--   0        0        0     3549 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/basics/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/common.py
--rw-r--r--   0        0        0     5335 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/form.py
--rw-r--r--   0        0        0     2075 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-11 17:50:46.027510 htagui-0.0.3/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-11 17:50:46.267511 htagui-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 htagui-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-11 18:19:53.616115 htagui-0.1.0/LICENSE
+-rw-r--r--   0        0        0     6445 2024-04-11 18:19:53.616115 htagui-0.1.0/README.md
+-rw-r--r--   0        0        0     1113 2024-04-11 18:19:54.152113 htagui-0.1.0/htagui/__init__.py
+-rw-r--r--   0        0        0     3549 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/common.py
+-rw-r--r--   0        0        0     5335 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/form.py
+-rw-r--r--   0        0        0     2075 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-11 18:19:53.616115 htagui-0.1.0/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-11 18:19:54.152113 htagui-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7678 1970-01-01 00:00:00.000000 htagui-0.1.0/PKG-INFO
```

### Comparing `htagui-0.0.3/LICENSE` & `htagui-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/README.md` & `htagui-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 **roadmap**
 
  - test test & test, to be rock solid
  - be available in htag4brython too, with the same apis.
  - perhaps provide version using shoelace web component, or simple bulma styles ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
 
 
+**INSTALL**
+```bash
+python3 -m pip install -U htag htagui
+```
+
+
 A hello world could be :
 
 ```python
-from htag import Tag, Runner
-import htagui as ui # `ui` could be available in htag namespace soon
+from htag import Tag, Runner, ui
 
 class MyApp(ui.App):
     def init(self):
         self <= ui.Button("test", _onclick=lambda ev: self.ui.alert( "hello world" ) )
 
 if __name__ == "__main__":
     Runner(MyApp).run()
 ```
 
 
 
-
 It provides some (ready-to-use) Htag Objects, and some utilities methods.
 
 
 ## Object App
 
 This is a surcharge of Tag.body( ... ) which auto provide an `ui` property on the instance, to interact with `Dialog` features
 
@@ -57,84 +61,84 @@
 ```
 
 ## Object Button
 
 A simple surcharge of Tag.button(...), to define a css class 
 
 ```python
-import htagui as u
-self <= u.Button("my button",_class="myclass", _onclick = myevent )
+import htagui as ui
+self <= ui.Button("my button",_class="myclass", _onclick = myevent )
 ```
 
 ## Object Input
 
 A simple surcharge of Tag.input(...), to define a css class 
 
 
 ```python
-import htagui as u
-self <= u.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
+import htagui as ui
+self <= ui.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
 ```
 
 ## Object Spinner
 
 A spinner object.
 
 ```python
-import htagui as u
-self <= u.Spinner()
+import htagui as ui
+self <= ui.Spinner()
 ```
 
 ## Object Select
 
 An htag class to help to create `select/option` html tags, using a dict of {value:title, ...}.
 
 ```python
-import htagui as u
-self <= u.Select( dict(a="A",b="B"), _value="a", _name="myfield" )
+import htagui as ui
+self <= ui.Select( dict(a="A",b="B"), _value="a", _name="myfield" )
 ```
 
 ## Object Menu
 
 An htag class to help to create a (first-level) menu and menu items, using a dict of {title:callback,...}
 
 ```python
-import htagui as u
-ui = u.Dialog(self)
+import htagui as ui
+ux = ui.Dialog(self)
 entries={
-    "menu1": lambda: ui.notify("menu1"),
-    "menu2": lambda: ui.notify("menu2"),
-    "menu3": lambda: ui.notify("menu3"),
+    "menu1": lambda: ux.notify("menu1"),
+    "menu2": lambda: ux.notify("menu2"),
+    "menu3": lambda: ux.notify("menu3"),
 }  
-self <= u.Menu( entries )
+self <= ui.Menu( entries )
 ```
 
 
 ## Object Form
 
 A simple surcharge of Tag.form(...) where you can define a callback to call a method wich will receive a python "dict" of all named inputs defined in the form.
 
 ```python
-import htagui as u
-ui = u.Dialog( self )
-form = u.Form( onsubmit=lambda dico: ui.notify(str(dico)) )
-form <= u.Input(_name="mystring",_placeholder="input something")
-form <= u.Button("ok")
+import htagui as ui
+ux = ui.Dialog( self )
+form = ui.Form( onsubmit=lambda dico: ux.notify(str(dico)) )
+form <= ui.Input(_name="mystring",_placeholder="input something")
+form <= ui.Button("ok")
 self <= form
 ```
 
 ## Object Tabs
 
 An htag class to easily create tabs structure. And provides somes attributs/methods to interact with it.
 
 ```python
-import htagui as u
+import htagui as ui
 tab1 = Tag.div("content1",name="tab1") # tab object needs a `name` property !
 tab2 = Tag.div("content2",name="tab2")
-t = u.Tabs( tab1, tab2 )
+t = ui.Tabs( tab1, tab2 )
 self += t
 ```
 
 ### method t.add_tab( obj )
 
 A method to add dynamically a tab instance, which is automatically selected.
 (note that the tab object needs a `name` property !)
@@ -143,82 +147,82 @@
 
 Dynamic property to retrieve or select the current selected tab.
 
 ### event "onchange"
 
 Event which is called when selected index changes.
 
-## Object UI (Dialog)
+## Object Dialog
 
-Expose "Dialog boxes" with methods on the ui instance.
+Expose "Dialog boxes" with methods on the instance.
 Note that, there can be only one dialog at a time (except toast notification)
 
 ```python
-import htagui as u
-ui = u.Dialog( self )
+import htagui as ui
+dialog = ui.Dialog( self )
 ```
 
-### method ui.alert(obj)
+### method dialog.alert(obj)
 
 (like js window.alert(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able)
 
-### method ui.confirm(obj, cbresponse=lambda bool:bool)
+### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
-### method ui.prompt(value:str, title, cbresponse=lambda val:val)
+### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
-### method ui.notify(obj, time=2000)
+### method dialog.notify(obj, time=2000)
 
 Display a toast message (notification), in the right-bottom ... during 2000 ms.
 (currently toast messages are not stacked)
 
-### method ui.pop(obj, xy:tuple)
+### method dialog.pop(obj, xy:tuple)
 
 Display an object, at coords (x,y).
 
 ex "create a popmenu", using "Menu object"
 ```python
-import htagui as u
-ui = u.Dialog(self)
+import htagui as ui
+dialog = ui.Dialog(self)
 entries={
-    "menu1": lambda: ui.notify("menu1"),
-    "menu2": lambda: ui.notify("menu2"),
-    "menu3": lambda: ui.notify("menu3"),
+    "menu1": lambda: dialog.notify("menu1"),
+    "menu2": lambda: dialog.notify("menu2"),
+    "menu3": lambda: dialog.notify("menu3"),
 }  
-self <= u.Button("pop menu", _onclick=lambda ev: ui.pop( u.Menu(entries) ,(ev.clientX,ev.clientY)) )
+self <= ui.Button("pop menu", _onclick=lambda ev: dialog.pop( ui.Menu(entries) ,(ev.clientX,ev.clientY)) )
 ```
 
-### method ui.drawer(obj, mode="left", size:int=50)
+### method dialog.drawer(obj, mode="left", size:int=50)
 
 Display a drawer, in the left-side, which takes 50% of the page.
 
-### method ui.block(obj=None)
+### method dialog.block(obj=None)
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
-### method ui.close()
+### method dialog.close()
 
 Close programatically, the current ui dialog.
 
 ## Object HSplit (& VSplit)
 
 A Tag object to use "SplitJS" (currently only in horizontal form)
 
 ```python
-import htagui as u
-self <= u.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
+import htagui as ui
+self <= ui.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
 ```
 
 ## utilities methods
 
 ### hflex & vflex
 
 Methods to create an HBox or VBox htag class (flexbox horizontal or vertical, with nowrap mode)
 
 ```python
-import htagui as u
-HBox = u.hflex(50, 50)  # create a hbox of 2 elements of 50% each
+import htagui as ui
+HBox = ui.hflex(50, 50)  # create a hbox of 2 elements of 50% each
 self <= HBox( Tag.div(1), Tag.div(2) )
 ```
```

### Comparing `htagui-0.0.3/htagui/__init__.py` & `htagui-0.1.0/htagui/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.0.3" # auto updated
+__version__ = "0.1.0" # auto updated
 
 from htag import Tag
 ########################################################################################
 from .basics import Button,Input,Menu,Spinner,Select
 ########################################################################################
 from .form import Form
 from .tabs import Tabs
```

### Comparing `htagui-0.0.3/htagui/basics/__init__.py` & `htagui-0.1.0/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/common.py` & `htagui-0.1.0/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/dialog.py` & `htagui-0.1.0/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/flex.py` & `htagui-0.1.0/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/form.py` & `htagui-0.1.0/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/splitters.py` & `htagui-0.1.0/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/htagui/tabs.py` & `htagui-0.1.0/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.0.3/pyproject.toml` & `htagui-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.0.3" # auto-updated
+version = "0.1.0" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.0.3/PKG-INFO` & `htagui-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.0.3
+Version: 0.1.0
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -40,31 +40,35 @@
 **roadmap**
 
  - test test & test, to be rock solid
  - be available in htag4brython too, with the same apis.
  - perhaps provide version using shoelace web component, or simple bulma styles ... but the basics version (current one) will always be available, with its minimal footprint (js/css dependancies in mind)
 
 
+**INSTALL**
+```bash
+python3 -m pip install -U htag htagui
+```
+
+
 A hello world could be :
 
 ```python
-from htag import Tag, Runner
-import htagui as ui # `ui` could be available in htag namespace soon
+from htag import Tag, Runner, ui
 
 class MyApp(ui.App):
     def init(self):
         self <= ui.Button("test", _onclick=lambda ev: self.ui.alert( "hello world" ) )
 
 if __name__ == "__main__":
     Runner(MyApp).run()
 ```
 
 
 
-
 It provides some (ready-to-use) Htag Objects, and some utilities methods.
 
 
 ## Object App
 
 This is a surcharge of Tag.body( ... ) which auto provide an `ui` property on the instance, to interact with `Dialog` features
 
@@ -84,84 +88,84 @@
 ```
 
 ## Object Button
 
 A simple surcharge of Tag.button(...), to define a css class 
 
 ```python
-import htagui as u
-self <= u.Button("my button",_class="myclass", _onclick = myevent )
+import htagui as ui
+self <= ui.Button("my button",_class="myclass", _onclick = myevent )
 ```
 
 ## Object Input
 
 A simple surcharge of Tag.input(...), to define a css class 
 
 
 ```python
-import htagui as u
-self <= u.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
+import htagui as ui
+self <= ui.Input(_value="my value"_, _name="myfield", _class="myclass", _required=True )
 ```
 
 ## Object Spinner
 
 A spinner object.
 
 ```python
-import htagui as u
-self <= u.Spinner()
+import htagui as ui
+self <= ui.Spinner()
 ```
 
 ## Object Select
 
 An htag class to help to create `select/option` html tags, using a dict of {value:title, ...}.
 
 ```python
-import htagui as u
-self <= u.Select( dict(a="A",b="B"), _value="a", _name="myfield" )
+import htagui as ui
+self <= ui.Select( dict(a="A",b="B"), _value="a", _name="myfield" )
 ```
 
 ## Object Menu
 
 An htag class to help to create a (first-level) menu and menu items, using a dict of {title:callback,...}
 
 ```python
-import htagui as u
-ui = u.Dialog(self)
+import htagui as ui
+ux = ui.Dialog(self)
 entries={
-    "menu1": lambda: ui.notify("menu1"),
-    "menu2": lambda: ui.notify("menu2"),
-    "menu3": lambda: ui.notify("menu3"),
+    "menu1": lambda: ux.notify("menu1"),
+    "menu2": lambda: ux.notify("menu2"),
+    "menu3": lambda: ux.notify("menu3"),
 }  
-self <= u.Menu( entries )
+self <= ui.Menu( entries )
 ```
 
 
 ## Object Form
 
 A simple surcharge of Tag.form(...) where you can define a callback to call a method wich will receive a python "dict" of all named inputs defined in the form.
 
 ```python
-import htagui as u
-ui = u.Dialog( self )
-form = u.Form( onsubmit=lambda dico: ui.notify(str(dico)) )
-form <= u.Input(_name="mystring",_placeholder="input something")
-form <= u.Button("ok")
+import htagui as ui
+ux = ui.Dialog( self )
+form = ui.Form( onsubmit=lambda dico: ux.notify(str(dico)) )
+form <= ui.Input(_name="mystring",_placeholder="input something")
+form <= ui.Button("ok")
 self <= form
 ```
 
 ## Object Tabs
 
 An htag class to easily create tabs structure. And provides somes attributs/methods to interact with it.
 
 ```python
-import htagui as u
+import htagui as ui
 tab1 = Tag.div("content1",name="tab1") # tab object needs a `name` property !
 tab2 = Tag.div("content2",name="tab2")
-t = u.Tabs( tab1, tab2 )
+t = ui.Tabs( tab1, tab2 )
 self += t
 ```
 
 ### method t.add_tab( obj )
 
 A method to add dynamically a tab instance, which is automatically selected.
 (note that the tab object needs a `name` property !)
@@ -170,83 +174,83 @@
 
 Dynamic property to retrieve or select the current selected tab.
 
 ### event "onchange"
 
 Event which is called when selected index changes.
 
-## Object UI (Dialog)
+## Object Dialog
 
-Expose "Dialog boxes" with methods on the ui instance.
+Expose "Dialog boxes" with methods on the instance.
 Note that, there can be only one dialog at a time (except toast notification)
 
 ```python
-import htagui as u
-ui = u.Dialog( self )
+import htagui as ui
+dialog = ui.Dialog( self )
 ```
 
-### method ui.alert(obj)
+### method dialog.alert(obj)
 
 (like js window.alert(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able)
 
-### method ui.confirm(obj, cbresponse=lambda bool:bool)
+### method dialog.confirm(obj, cbresponse=lambda bool:bool)
 
 (like js window.confirm(...)) Display a modal dialog box containing the object 'obj' (obj must be str'able), and let the user click on Yes|No buttons, which will call the cbresponse callback with True or False ...
 
-### method ui.prompt(value:str, title, cbresponse=lambda val:val)
+### method dialog.prompt(value:str, title, cbresponse=lambda val:val)
 
 (like js window.prompt(...)) Display a modal dialog letting the user edit the `value` in an Input box, with a `title` (title must be str'able). When the user click the OK button the value is sent in the callback cbresponse. (clicking the cancel button does nothing, except close the dialog)
 
-### method ui.notify(obj, time=2000)
+### method dialog.notify(obj, time=2000)
 
 Display a toast message (notification), in the right-bottom ... during 2000 ms.
 (currently toast messages are not stacked)
 
-### method ui.pop(obj, xy:tuple)
+### method dialog.pop(obj, xy:tuple)
 
 Display an object, at coords (x,y).
 
 ex "create a popmenu", using "Menu object"
 ```python
-import htagui as u
-ui = u.Dialog(self)
+import htagui as ui
+dialog = ui.Dialog(self)
 entries={
-    "menu1": lambda: ui.notify("menu1"),
-    "menu2": lambda: ui.notify("menu2"),
-    "menu3": lambda: ui.notify("menu3"),
+    "menu1": lambda: dialog.notify("menu1"),
+    "menu2": lambda: dialog.notify("menu2"),
+    "menu3": lambda: dialog.notify("menu3"),
 }  
-self <= u.Button("pop menu", _onclick=lambda ev: ui.pop( u.Menu(entries) ,(ev.clientX,ev.clientY)) )
+self <= ui.Button("pop menu", _onclick=lambda ev: dialog.pop( ui.Menu(entries) ,(ev.clientX,ev.clientY)) )
 ```
 
-### method ui.drawer(obj, mode="left", size:int=50)
+### method dialog.drawer(obj, mode="left", size:int=50)
 
 Display a drawer, in the left-side, which takes 50% of the page.
 
-### method ui.block(obj=None)
+### method dialog.block(obj=None)
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
-### method ui.close()
+### method dialog.close()
 
 Close programatically, the current ui dialog.
 
 ## Object HSplit (& VSplit)
 
 A Tag object to use "SplitJS" (currently only in horizontal form)
 
 ```python
-import htagui as u
-self <= u.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
+import htagui as ui
+self <= ui.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
 ```
 
 ## utilities methods
 
 ### hflex & vflex
 
 Methods to create an HBox or VBox htag class (flexbox horizontal or vertical, with nowrap mode)
 
 ```python
-import htagui as u
-HBox = u.hflex(50, 50)  # create a hbox of 2 elements of 50% each
+import htagui as ui
+HBox = ui.hflex(50, 50)  # create a hbox of 2 elements of 50% each
 self <= HBox( Tag.div(1), Tag.div(2) )
 ```
```

