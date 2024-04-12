# Comparing `tmp/fps_jupyterlab-0.4.2.tar.gz` & `tmp/fps_jupyterlab-0.5.0.tar.gz`

## Comparing `fps_jupyterlab-0.4.2.tar` & `fps_jupyterlab-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/COPYING.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fps_jupyterlab-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/COPYING.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fps_jupyterlab-0.5.0/PKG-INFO
```

### Comparing `fps_jupyterlab-0.4.2/fps_jupyterlab/index.py` & `fps_jupyterlab-0.5.0/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.4.2/fps_jupyterlab/main.py` & `fps_jupyterlab-0.5.0/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.4.2/fps_jupyterlab/routes.py` & `fps_jupyterlab-0.5.0/fps_jupyterlab/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         self.jupyterlab_config = jupyterlab_config
         self.frontend_config = frontend_config
         self.lab = lab
         lab.redirect_after_root = "lab"
 
         extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
-        self.federated_extensions, self.disabled_extension = lab.get_federated_extensions(
+        self.federated_extensions, self.disabled_extensions = lab.get_federated_extensions(
             extensions_dir
         )
         jupyterlab_dir = Path(jupyterlab_module.__file__).parents[1]
 
         if jupyterlab_config.dev_mode:
             self.static_lab_dir = jupyterlab_dir / "dev_mode" / "static"
         else:
@@ -122,15 +122,15 @@
             "appUrl": "/lab",
             "appVersion": jupyterlab_module.__version__,
             "baseUrl": base_url,
             "cacheFiles": False,
             "collaborative": collaborative,
             "serverSideExecution": server_side_execution,
             "devMode": dev_mode,
-            "disabledExtensions": self.disabled_extension,
+            "disabledExtensions": self.disabled_extensions,
             "exposeAppInBrowser": False,
             "extraLabextensionsPath": [],
             "federated_extensions": self.federated_extensions,
             "fullAppUrl": f"{base_url}lab",
             "fullLabextensionsUrl": f"{base_url}lab/extensions",
             "fullLicensesUrl": f"{base_url}lab/api/licenses",
             "fullListingsUrl": f"{base_url}lab/api/listings",
```

### Comparing `fps_jupyterlab-0.4.2/.gitignore` & `fps_jupyterlab-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.4.2/COPYING.md` & `fps_jupyterlab-0.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.4.2/pyproject.toml` & `fps_jupyterlab-0.5.0/pyproject.toml`

 * *Files identical despite different names*

