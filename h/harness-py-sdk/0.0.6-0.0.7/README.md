# Comparing `tmp/harness_py_sdk-0.0.6.tar.gz` & `tmp/harness_py_sdk-0.0.7.tar.gz`

## Comparing `harness_py_sdk-0.0.6.tar` & `harness_py_sdk-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/publish.sh
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    34745 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk.html
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/index.html
--rw-r--r--   0        0        0    96377 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/search.js
--rw-r--r--   0        0        0    34733 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/ __init__.html
--rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_base_service.html
--rw-r--r--   0        0        0    39751 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_connectors.html
--rw-r--r--   0        0        0    38088 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_old_connectors.html
--rw-r--r--   0        0        0    39703 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_pipelines.html
--rw-r--r--   0        0        0    38057 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_services.html
--rw-r--r--   0        0        0    39334 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_templates.html
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/ __init__.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_connectors.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_old_connectors.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_pipelines.py
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_sdk.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_services.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/src/harness_py_sdk/harness_templates.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/LICENSE
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/publish.sh
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    34745 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/index.html
+-rw-r--r--   0        0        0    96377 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/search.js
+-rw-r--r--   0        0        0    34733 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/ __init__.html
+-rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_base_service.html
+-rw-r--r--   0        0        0    39751 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_connectors.html
+-rw-r--r--   0        0        0    38088 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_old_connectors.html
+-rw-r--r--   0        0        0    39703 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_pipelines.html
+-rw-r--r--   0        0        0    38057 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_services.html
+-rw-r--r--   0        0        0    39334 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_templates.html
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/ __init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_connectors.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_old_connectors.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_pipelines.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_sdk.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_services.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/src/harness_py_sdk/harness_templates.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.7/PKG-INFO
```

### Comparing `harness_py_sdk-0.0.6/.github/workflows/python-publish.yml` & `harness_py_sdk-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/search.js` & `harness_py_sdk-0.0.7/docs/search.js`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/ __init__.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/ __init__.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_base_service.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_base_service.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_connectors.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_connectors.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_old_connectors.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_old_connectors.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_pipelines.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_pipelines.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_services.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_services.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/docs/harness_py_sdk/harness_templates.html` & `harness_py_sdk-0.0.7/docs/harness_py_sdk/harness_templates.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_connectors.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_connectors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from harness_old_connectors import *
+from .harness_old_connectors import *
 
 class HarnessConnectors():
     def __init__(self, harness_service):
         self._harness_service = harness_service
         self._old = None  # Placeholder for the Old Connector class
 
     @property
```

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_old_connectors.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_old_connectors.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_pipelines.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_pipelines.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_sdk.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_sdk.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_services.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_services.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/src/harness_py_sdk/harness_templates.py` & `harness_py_sdk-0.0.7/src/harness_py_sdk/harness_templates.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/LICENSE` & `harness_py_sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/README.md` & `harness_py_sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.6/pyproject.toml` & `harness_py_sdk-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "harness-py-sdk"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Guilherme Zanini", email="guilherme.zanini@harness.io" },
 ]
 description = "This is a non-official package that leverages the Harness API using Python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `harness_py_sdk-0.0.6/PKG-INFO` & `harness_py_sdk-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: harness-py-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is a non-official package that leverages the Harness API using Python.
 Project-URL: Homepage, https://github.com/guilhermezanini-harness/harness-py-sdk
 Project-URL: Issues, https://github.com/guilhermezanini-harness/harness-py-sdk/issues
 Author-email: Guilherme Zanini <guilherme.zanini@harness.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

