# Comparing `tmp/SideJITServer-1.2.1.tar.gz` & `tmp/SideJITServer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SideJITServer-1.2.1.tar", last modified: Thu Apr  4 18:32:48 2024, max compression
+gzip compressed data, was "SideJITServer-1.3.0.tar", last modified: Fri Apr 12 08:33:49 2024, max compression
```

## Comparing `SideJITServer-1.2.1.tar` & `SideJITServer-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:48.843510 SideJITServer-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/README.Docker.md
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/SideJITServer/
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/SideJITServer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/SideJITServer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/SideJITServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 18:32:48.000000 SideJITServer-1.2.1/SideJITServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/compose.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 18:32:31.000000 SideJITServer-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:32:48.847510 SideJITServer-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/README.Docker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.837055 SideJITServer-1.3.0/SideJITServer/
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/SideJITServer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/SideJITServer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/SideJITServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 08:33:49.000000 SideJITServer-1.3.0/SideJITServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 08:33:33.000000 SideJITServer-1.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 08:33:49.841055 SideJITServer-1.3.0/setup.cfg
```

### Comparing `SideJITServer-1.2.1/.dockerignore` & `SideJITServer-1.3.0/.dockerignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/.github/workflows/python-publish.yml` & `SideJITServer-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/.gitignore` & `SideJITServer-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/Dockerfile` & `SideJITServer-1.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/PKG-INFO` & `SideJITServer-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.2.1
+Version: 1.3.0
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,15 +17,15 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.1.0,>=3.0.3
+Requires-Dist: pymobiledevice3<3.5.0,>=3.4.0
 Requires-Dist: Flask==3.0.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
 This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
```

### Comparing `SideJITServer-1.2.1/README.md` & `SideJITServer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/SideJITServer/__init__.py` & `SideJITServer-1.3.0/SideJITServer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,18 @@
 @app.route("/")
 def devices():
     global devs
     if len(devs) == 0:
         return {"ERROR": "Could not find any device!"}
     return {d.name: d.udid for d in devs}
 
+@app.route("/ver/")
+def route_version():
+    return {"pymobiledevice3": pymd_ver, "SideJITServer": __version__}
+
 @app.route("/re/")
 def refresh_devices():
     refresh_devs()
     return {"OK": "Refreshed!"}
 
 @app.route("/<device>/")
 def get_apps(device):
```

### Comparing `SideJITServer-1.2.1/SideJITServer.egg-info/PKG-INFO` & `SideJITServer-1.3.0/SideJITServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SideJITServer
-Version: 1.2.1
+Version: 1.3.0
 Summary: SideJITServer is an iOS 17 JIT enabler for Windows/macOS!
 Author: khanhduytran0
 Author-email: nythepegasus <me@nythepegas.us>, JoeMatt <git@joemattiello.com>
 Maintainer-email: nythepegasus <me@nythepegas.us>
 Project-URL: Homepage, https://github.com/nythepegasus/SideJITServer
 Project-URL: Bug Reports, https://github.com/nythepegasus/SideJITServer/issues
 Keywords: ios,automation,cli,jit
@@ -17,15 +17,15 @@
 Classifier: Operating System :: iOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: pymobiledevice3<3.1.0,>=3.0.3
+Requires-Dist: pymobiledevice3<3.5.0,>=3.4.0
 Requires-Dist: Flask==3.0.2
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 
 # SideJITServer
 This project allows you to start a server that wirelessly gives you JIT for iOS 17+ on Windows/macOS. Linux support depends on a [kernel patch](https://github.com/doronz88/pymobiledevice3/issues/566#issuecomment-1850486679).
```

### Comparing `SideJITServer-1.2.1/compose.yaml` & `SideJITServer-1.3.0/compose.yaml`

 * *Files identical despite different names*

### Comparing `SideJITServer-1.2.1/pyproject.toml` & `SideJITServer-1.3.0/pyproject.toml`

 * *Files identical despite different names*

