# Comparing `tmp/jupyverse_api-0.4.2.tar.gz` & `tmp/jupyverse_api-0.5.0.tar.gz`

## Comparing `jupyverse_api-0.4.2.tar` & `jupyverse_api-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/cli.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/py.typed
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/README.md
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyverse_api-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/notebook/__init__.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 jupyverse_api-0.5.0/PKG-INFO
```

### Comparing `jupyverse_api-0.4.2/jupyverse_api/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.4.2/jupyverse_api/cli.py` & `jupyverse_api-0.5.0/jupyverse_api/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import sys
 from typing import List, Tuple
 
-import pkg_resources
 import rich_click as click
 from asphalt.core.cli import run
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 
 @click.command()  # type: ignore
 @click.option(
     "--open-browser",
     is_flag=True,
     show_default=True,
     default=False,
@@ -68,15 +73,15 @@
         configfile=[config],
     )  # type: ignore
 
 
 def get_config(disable: Tuple[str, ...]) -> str:
     jupyverse_components = [
         ep.name
-        for ep in pkg_resources.iter_entry_points(group="jupyverse.components")
+        for ep in entry_points(group="jupyverse.components")
         if ep.name not in disable
     ]
 
     config = ["component:\n  type: jupyverse\n  components:\n"]
     for component in jupyverse_components:
         config.append(f"    {component}:\n      type: {component}\n")
```

### Comparing `jupyverse_api-0.4.2/jupyverse_api/app/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/contents/models.py` & `jupyverse_api-0.5.0/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/kernels/models.py` & `jupyverse_api-0.5.0/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/main/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/notebook/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 from jupyverse_api import Router
 
 from ..app import App
 from ..auth import Auth, User
 from ..lab import Lab
 
 
-class RetroLab(Router, ABC):
+class Notebook(Router, ABC):
     def __init__(self, app: App, auth: Auth, lab: Lab):
         super().__init__(app=app)
 
         router = APIRouter()
 
-        @router.get("/retro/tree", response_class=HTMLResponse)
+        @router.get("/tree", response_class=HTMLResponse)
         async def get_tree(
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_tree(user)
 
-        @router.get("/retro/notebooks/{path:path}", response_class=HTMLResponse)
+        @router.get("/notebooks/{path:path}", response_class=HTMLResponse)
         async def get_notebook(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_notebook(path, user)
 
-        @router.get("/retro/edit/{path:path}", response_class=HTMLResponse)
+        @router.get("/edit/{path:path}", response_class=HTMLResponse)
         async def edit_file(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.edit_file(path, user)
 
-        @router.get("/retro/consoles/{path:path}", response_class=HTMLResponse)
+        @router.get("/consoles/{path:path}", response_class=HTMLResponse)
         async def get_console(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_console(path, user)
 
-        @router.get("/retro/terminals/{name}", response_class=HTMLResponse)
+        @router.get("/terminals/{name}", response_class=HTMLResponse)
         async def get_terminal(
             name: str,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_terminal(name, user)
 
         self.include_router(router)
```

### Comparing `jupyverse_api-0.4.2/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.5.0/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/.gitignore` & `jupyverse_api-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/COPYING.md` & `jupyverse_api-0.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.4.2/pyproject.toml` & `jupyverse_api-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+  "importlib_metadata >=3.6; python_version<'3.10'",
   "pydantic >=2,<3",
   "fastapi >=0.95.0,<1",
   "rich-click >=1.6.1,<2",
   "asphalt >=4.11.0,<5",
   "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
```

### Comparing `jupyverse_api-0.4.2/PKG-INFO` & `jupyverse_api-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyverse_api
-Version: 0.4.2
+Version: 0.5.0
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: asphalt-web[fastapi]<2,>=1.1.0
 Requires-Dist: asphalt<5,>=4.11.0
 Requires-Dist: fastapi<1,>=0.95.0
+Requires-Dist: importlib-metadata>=3.6; python_version < '3.10'
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: rich-click<2,>=1.6.1
 Description-Content-Type: text/markdown
 
 # Jupyverse API
 
 The public API for Jupyverse.
```

