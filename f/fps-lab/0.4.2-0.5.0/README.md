# Comparing `tmp/fps_lab-0.4.2.tar.gz` & `tmp/fps_lab-0.5.0.tar.gz`

## Comparing `fps_lab-0.4.2.tar` & `fps_lab-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.4.2/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.4.2/fps_lab/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fps_lab-0.4.2/fps_lab/main.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 fps_lab-0.4.2/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_lab-0.4.2/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_lab-0.4.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.4.2/COPYING.md
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.4.2/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fps_lab-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 fps_lab-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_lab-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_lab-0.5.0/fps_lab/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 fps_lab-0.5.0/fps_lab/main.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 fps_lab-0.5.0/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_lab-0.5.0/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_lab-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_lab-0.5.0/COPYING.md
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fps_lab-0.5.0/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fps_lab-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 fps_lab-0.5.0/PKG-INFO
```

### Comparing `fps_lab-0.4.2/fps_lab/main.py` & `fps_lab-0.5.0/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `fps_lab-0.4.2/fps_lab/routes.py` & `fps_lab-0.5.0/fps_lab/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import json
 import logging
 import os
+import sys
 from glob import glob
 from http import HTTPStatus
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import json5  # type: ignore
-import pkg_resources
 from babel import Locale
 from fastapi import Response, status
 from fastapi.responses import FileResponse, RedirectResponse
 from starlette.requests import Request
 
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.jupyterlab import JupyterLabConfig
 from jupyverse_api.lab import Lab
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 logger = logging.getLogger("lab")
 
 
 class _Lab(Lab):
     def __init__(
         self,
         app: App,
@@ -75,15 +80,15 @@
         native_name = (locale.get_display_name() or "").capitalize()
         data = {
             "en": {
                 "displayName": display_name,
                 "nativeName": native_name,
             }
         }
-        for ep in pkg_resources.iter_entry_points(group="jupyterlab.languagepack"):
+        for ep in entry_points(group="jupyterlab.languagepack"):
             locale = Locale.parse(ep.name)
             data[ep.name] = {
                 "displayName": display_name,
                 "nativeName": native_name,
             }
         return {"data": data, "message": ""}
 
@@ -92,15 +97,15 @@
         language,
         user: User,
     ):
         if language == "en":
             self.locale = language
             return {}
 
-        for ep in pkg_resources.iter_entry_points(group="jupyterlab.languagepack"):
+        for ep in entry_points(group="jupyterlab.languagepack"):
             if ep.name == language:
                 break
         else:
             return {"data": {}, "message": f"Language pack '{language}' not installed!"}
         self.locale = language
         package = ep.load()
         data = {}
@@ -116,15 +121,15 @@
         name0,
         name1,
         name2,
         user: User,
     ):
         with open(self.jlab_dir / "static" / "package.json") as f:
             package = json.load(f)
-        if name0 in ["@jupyterlab", "@retrolab"]:
+        if name0 in ["@jupyterlab", "@notebook"]:
             schemas_parent = self.jlab_dir
         else:
             schemas_parent = self.extensions_dir / name0 / name1
         with open(schemas_parent / "schemas" / name0 / name1 / f"{name2}.json") as f:
             schema = json.load(f)
         key = f"{name1}:{name2}"
         setting = {
```

### Comparing `fps_lab-0.4.2/fps_lab/static/favicon.ico` & `fps_lab-0.5.0/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fps_lab-0.4.2/.gitignore` & `fps_lab-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_lab-0.4.2/COPYING.md` & `fps_lab-0.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_lab-0.4.2/pyproject.toml` & `fps_lab-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 name = "fps_lab"
-description = "An FPS plugin for the JupyterLab/RetroLab API"
+description = "An FPS plugin for the JupyterLab/Notebook API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
+  "importlib_metadata >=3.6; python_version<'3.10'",
   "babel",
   "json5",
   "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
```

