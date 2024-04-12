# Comparing `tmp/fps_yjs-0.4.2.tar.gz` & `tmp/fps_yjs-0.5.0.tar.gz`

## Comparing `fps_yjs-0.4.2.tar` & `fps_yjs-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/py.typed
--rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/routes.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/utils.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/ybasedoc.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/yblob.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/yfile.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/ynotebook.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ydocs/yunicode.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/awareness.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/django_channels_consumer.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket_provider.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket_server.py
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/yroom.py
--rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/ystore.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywebsocket/yutils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywidgets/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/fps_yjs/ywidgets/widgets.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/README.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fps_yjs-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/routes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/utils.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/ybasedoc.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/yblob.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/yfile.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/ynotebook.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ydocs/yunicode.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/awareness.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/django_channels_consumer.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket_provider.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket_server.py
+-rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/yroom.py
+-rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/ystore.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywebsocket/yutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywidgets/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/fps_yjs/ywidgets/widgets.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fps_yjs-0.5.0/PKG-INFO
```

### Comparing `fps_yjs-0.4.2/fps_yjs/main.py` & `fps_yjs-0.5.0/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/routes.py` & `fps_yjs-0.5.0/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ydocs/utils.py` & `fps_yjs-0.5.0/fps_yjs/ydocs/utils.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ydocs/ybasedoc.py` & `fps_yjs-0.5.0/fps_yjs/ydocs/ybasedoc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, Optional
 
-from pycrdt import Doc, Map
+from pycrdt import Doc, Map, Subscription
 
 
 class YBaseDoc(ABC):
     def __init__(self, ydoc: Optional[Doc] = None):
         if ydoc is None:
             self._ydoc = Doc()
         else:
             self._ydoc = ydoc
         self._ystate = Map()
         self._ydoc["state"] = self._ystate
-        self._subscriptions: Dict[Any, str] = {}
+        self._subscriptions: Dict[Any, Subscription] = {}
 
     @property
     @abstractmethod
     def version(self) -> str:
         ...
 
     @property
```

### Comparing `fps_yjs-0.4.2/fps_yjs/ydocs/yblob.py` & `fps_yjs-0.5.0/fps_yjs/ydocs/yblob.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ydocs/ynotebook.py` & `fps_yjs-0.5.0/fps_yjs/ydocs/ynotebook.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ydocs/yunicode.py` & `fps_yjs-0.5.0/fps_yjs/ydocs/yunicode.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/asgi_server.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/awareness.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/awareness.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/django_channels_consumer.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket_provider.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/websocket_server.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/yroom.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/yroom.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/ystore.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/ystore.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywebsocket/yutils.py` & `fps_yjs-0.5.0/fps_yjs/ywebsocket/yutils.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/fps_yjs/ywidgets/widgets.py` & `fps_yjs-0.5.0/fps_yjs/ywidgets/widgets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+import sys
 from typing import Any
 
-import pkg_resources
 from pycrdt import TransactionEvent
 
 try:
     from ypywidgets.utils import (  # type: ignore
         YMessageType,
         YSyncMessageType,
         create_update_message,
         process_sync_message,
         sync,
     )
     ypywidgets_installed = True
 except ImportError:
     ypywidgets_installed = False
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 
 Widgets: Any
 
 if ypywidgets_installed:
     class Widgets:  # type: ignore
         def __init__(self):
             self.ydocs = {
-                ep.name: ep.load() for ep in pkg_resources.iter_entry_points(group="ypywidgets")
+                ep.name: ep.load() for ep in entry_points(group="ypywidgets")
             }
             self.widgets = {}
 
         def comm_open(self, msg, comm) -> None:
             target_name = msg["content"]["target_name"]
             if target_name != "ywidget":
                 return
```

### Comparing `fps_yjs-0.4.2/.gitignore` & `fps_yjs-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/COPYING.md` & `fps_yjs-0.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.4.2/pyproject.toml` & `fps_yjs-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-    "pycrdt >=0.8.2,<0.9.0",
+    "importlib_metadata >=3.6; python_version<'3.10'",
+    "pycrdt >=0.8.16,<0.9.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

