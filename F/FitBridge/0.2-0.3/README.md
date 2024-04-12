# Comparing `tmp/FitBridge-0.2.tar.gz` & `tmp/FitBridge-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FitBridge-0.2.tar", last modified: Sat Feb 17 15:45:55 2024, max compression
+gzip compressed data, was "FitBridge-0.3.tar", last modified: Fri Apr 12 01:55:36 2024, max compression
```

## Comparing `FitBridge-0.2.tar` & `FitBridge-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:45:55.950517 FitBridge-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:45:55.950517 FitBridge-0.2/FitBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-17 15:45:43.000000 FitBridge-0.2/FitBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-02-17 15:45:43.000000 FitBridge-0.2/FitBridge/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 15:45:55.950517 FitBridge-0.2/FitBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-17 15:45:55.000000 FitBridge-0.2/FitBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-17 15:45:43.000000 FitBridge-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-02-17 15:45:55.950517 FitBridge-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-17 15:45:43.000000 FitBridge-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 15:45:55.950517 FitBridge-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-17 15:45:43.000000 FitBridge-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:55:36.356364 FitBridge-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:55:36.352364 FitBridge-0.3/FitBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 01:55:32.000000 FitBridge-0.3/FitBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-12 01:55:32.000000 FitBridge-0.3/FitBridge/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:55:36.356364 FitBridge-0.3/FitBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 01:55:36.000000 FitBridge-0.3/FitBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 01:55:32.000000 FitBridge-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-12 01:55:36.356364 FitBridge-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-12 01:55:32.000000 FitBridge-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:55:36.356364 FitBridge-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-12 01:55:32.000000 FitBridge-0.3/setup.py
```

### Comparing `FitBridge-0.2/FitBridge/main.py` & `FitBridge-0.3/FitBridge/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,19 @@
 
         credentials = flow.run_console()
 
         with open(credentials_file, "wb") as f:
             pickle.dump(credentials, f)
 
     if not credentials.valid or credentials.expired:
-        credentials.refresh(Request())
+        try:
+            credentials.refresh(Request())
+        except:
+            os.remove(os.path.join(conf_dir, "token.pickle"))
+            return auth(conf_dir)
 
     return credentials
 
 def register_datasources(credentials):
     heart_rate_reg_json = """{
     "dataStreamName": "FitBridgge",
     "type": "derived",
```

### Comparing `FitBridge-0.2/FitBridge.egg-info/PKG-INFO` & `FitBridge-0.3/FitBridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FitBridge
-Version: 0.2
+Version: 0.3
 Summary: A simple script to sync Gadgetbridge exported data to Google Fit
 Home-page: https://github.com/moh53n/FitBridge
 Author: Mohsen Tahmasebi
 Author-email: moh53n@moh53n.ir
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/moh53n/FitBridge/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FitBridge-0.2/LICENSE` & `FitBridge-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FitBridge-0.2/PKG-INFO` & `FitBridge-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FitBridge
-Version: 0.2
+Version: 0.3
 Summary: A simple script to sync Gadgetbridge exported data to Google Fit
 Home-page: https://github.com/moh53n/FitBridge
 Author: Mohsen Tahmasebi
 Author-email: moh53n@moh53n.ir
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/moh53n/FitBridge/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FitBridge-0.2/README.md` & `FitBridge-0.3/README.md`

 * *Files identical despite different names*

### Comparing `FitBridge-0.2/setup.py` & `FitBridge-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FitBridge",
-    version="0.2",
+    version="0.3",
     author="Mohsen Tahmasebi",
     author_email="moh53n@moh53n.ir",
     description="A simple script to sync Gadgetbridge exported data to Google Fit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/moh53n/FitBridge",
     project_urls={
```

