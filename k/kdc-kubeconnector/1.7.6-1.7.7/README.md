# Comparing `tmp/kdc-kubeconnector-1.7.6.tar.gz` & `tmp/kdc-kubeconnector-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdc-kubeconnector-1.7.6.tar", last modified: Wed Apr 10 08:16:30 2024, max compression
+gzip compressed data, was "kdc-kubeconnector-1.7.7.tar", last modified: Fri Apr 12 09:32:25 2024, max compression
```

## Comparing `kdc-kubeconnector-1.7.6.tar` & `kdc-kubeconnector-1.7.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:16:30.556426 kdc-kubeconnector-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 08:16:30.556426 kdc-kubeconnector-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:16:30.556426 kdc-kubeconnector-1.7.6/kdc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/kdc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/kdc/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/kdc/kube_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/kdc/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/kdc/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 08:16:30.556426 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 08:16:30.000000 kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-10 08:16:26.000000 kdc-kubeconnector-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 08:16:30.556426 kdc-kubeconnector-1.7.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:32:25.161274 kdc-kubeconnector-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 09:32:25.161274 kdc-kubeconnector-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:32:25.161274 kdc-kubeconnector-1.7.7/kdc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/kdc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/kdc/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/kdc/kube_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/kdc/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/kdc/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:32:25.161274 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 09:32:25.000000 kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-12 09:32:18.000000 kdc-kubeconnector-1.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:32:25.161274 kdc-kubeconnector-1.7.7/setup.cfg
```

### Comparing `kdc-kubeconnector-1.7.6/PKG-INFO` & `kdc-kubeconnector-1.7.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdc-kubeconnector
-Version: 1.7.6
+Version: 1.7.7
 Summary: Tool to work with kubernetes dashboard, if there is no kubectl access
 Author: Oleksii Ostapov
 Project-URL: Homepage, https://infopulse.com
 Project-URL: Documentation, https://github.com/infopulse/kdc
 Project-URL: Code, https://github.com/infopulse/kdc
 Classifier: Topic :: Software Development :: Testing
 Classifier: Development Status :: 3 - Alpha
@@ -108,9 +108,10 @@
 kdc -n uat
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Release Notes
+- 1.7.7 - fixed wrong selection of namespace by cluster
 - 1.7.6 - fixed GitHub actions pipeline. Fixed version issue
 - 1.7.0 - fixed version issue. Added the ability to set the namespace by cluster. Improved env selection argument
```

### Comparing `kdc-kubeconnector-1.7.6/Readme.md` & `kdc-kubeconnector-1.7.7/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -86,9 +86,10 @@
 kdc -n uat
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Release Notes
+- 1.7.7 - fixed wrong selection of namespace by cluster
 - 1.7.6 - fixed GitHub actions pipeline. Fixed version issue
 - 1.7.0 - fixed version issue. Added the ability to set the namespace by cluster. Improved env selection argument
```

### Comparing `kdc-kubeconnector-1.7.6/kdc/config.py` & `kdc-kubeconnector-1.7.7/kdc/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     if len(cfg['cluster']) == 0:
         return None
     if not cluster:
         default = tuple(cfg['cluster'].keys())[0]
         cluster = cfg['cluster'].get(default)
     cluster['name'] = default
     cluster.update(cfg['connection'])
-    cluster.update({'namespace': cfg['default'].get('namespace')})
+    cluster.update({'namespace': get_namespace(cfg)})
     return cluster
 
 
 def get_version():
     dist = distribution('kdc-kubeconnector')
     return dist.version
```

### Comparing `kdc-kubeconnector-1.7.6/kdc/kube_dashboard.py` & `kdc-kubeconnector-1.7.7/kdc/kube_dashboard.py`

 * *Files identical despite different names*

### Comparing `kdc-kubeconnector-1.7.6/kdc/main.py` & `kdc-kubeconnector-1.7.7/kdc/main.py`

 * *Files identical despite different names*

### Comparing `kdc-kubeconnector-1.7.6/kdc/parsers.py` & `kdc-kubeconnector-1.7.7/kdc/parsers.py`

 * *Files identical despite different names*

### Comparing `kdc-kubeconnector-1.7.6/kdc_kubeconnector.egg-info/PKG-INFO` & `kdc-kubeconnector-1.7.7/kdc_kubeconnector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdc-kubeconnector
-Version: 1.7.6
+Version: 1.7.7
 Summary: Tool to work with kubernetes dashboard, if there is no kubectl access
 Author: Oleksii Ostapov
 Project-URL: Homepage, https://infopulse.com
 Project-URL: Documentation, https://github.com/infopulse/kdc
 Project-URL: Code, https://github.com/infopulse/kdc
 Classifier: Topic :: Software Development :: Testing
 Classifier: Development Status :: 3 - Alpha
@@ -108,9 +108,10 @@
 kdc -n uat
 ```
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## Release Notes
+- 1.7.7 - fixed wrong selection of namespace by cluster
 - 1.7.6 - fixed GitHub actions pipeline. Fixed version issue
 - 1.7.0 - fixed version issue. Added the ability to set the namespace by cluster. Improved env selection argument
```

### Comparing `kdc-kubeconnector-1.7.6/pyproject.toml` & `kdc-kubeconnector-1.7.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = [".github", "config.toml", "build.bat", "build.sh"]
 
 [project]
 name = "kdc-kubeconnector"
-version = "1.7.6"
+version = "1.7.7"
 description = "Tool to work with kubernetes dashboard, if there is no kubectl access"
 requires-python = ">=3.11"
 readme = "Readme.md"
 
 dependencies = [
     "argparse>=1.4.0",
     "requests>=2.31.0",
```

