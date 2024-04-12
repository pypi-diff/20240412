# Comparing `tmp/harness_py_sdk-0.0.4.tar.gz` & `tmp/harness_py_sdk-0.0.5.tar.gz`

## Comparing `harness_py_sdk-0.0.4.tar` & `harness_py_sdk-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/publish.sh
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    34745 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk.html
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/index.html
--rw-r--r--   0        0        0    96377 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/search.js
--rw-r--r--   0        0        0    34733 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/ __init__.html
--rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_base_service.html
--rw-r--r--   0        0        0    39751 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_connectors.html
--rw-r--r--   0        0        0    38088 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_old_connectors.html
--rw-r--r--   0        0        0    39703 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_pipelines.html
--rw-r--r--   0        0        0    38057 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_services.html
--rw-r--r--   0        0        0    39334 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_templates.html
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/ __init__.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_base_service.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_connectors.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_old_connectors.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_pipelines.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_services.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/src/harness_py_sdk/harness_templates.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/LICENSE
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/publish.sh
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/requirements.txt
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    34745 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/index.html
+-rw-r--r--   0        0        0    96377 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/search.js
+-rw-r--r--   0        0        0    34733 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/ __init__.html
+-rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_base_service.html
+-rw-r--r--   0        0        0    39751 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_connectors.html
+-rw-r--r--   0        0        0    38088 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_old_connectors.html
+-rw-r--r--   0        0        0    39703 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_pipelines.html
+-rw-r--r--   0        0        0    38057 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_services.html
+-rw-r--r--   0        0        0    39334 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_templates.html
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/ __init__.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_connectors.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_old_connectors.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_pipelines.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_sdk.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_services.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/src/harness_py_sdk/harness_templates.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 harness_py_sdk-0.0.5/PKG-INFO
```

### Comparing `harness_py_sdk-0.0.4/.github/workflows/python-publish.yml` & `harness_py_sdk-0.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/search.js` & `harness_py_sdk-0.0.5/docs/search.js`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/ __init__.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/ __init__.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_base_service.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_base_service.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_connectors.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_connectors.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_old_connectors.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_old_connectors.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_pipelines.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_pipelines.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_services.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_services.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/docs/harness_py_sdk/harness_templates.html` & `harness_py_sdk-0.0.5/docs/harness_py_sdk/harness_templates.html`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/src/harness_py_sdk/harness_base_service.py` & `harness_py_sdk-0.0.5/src/harness_py_sdk/harness_sdk.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
-from harness_pipelines import HarnessPipelines
-from harness_connectors import HarnessConnectors
-from harness_services import HarnessServices
 
-class HarnessBaseService:
+from harness_pipelines import *
+from harness_connectors import *
+from harness_services import *
+
+class HarnessSDK:
     def __init__(self, api_key, account_identifier):
         self._session = requests.Session()
         self._session.   headers.update({
             'x-api-key': api_key,
             'Harness-Account': account_identifier,
             'Content-Type': 'application/json'
         })
```

### Comparing `harness_py_sdk-0.0.4/src/harness_py_sdk/harness_old_connectors.py` & `harness_py_sdk-0.0.5/src/harness_py_sdk/harness_old_connectors.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/src/harness_py_sdk/harness_pipelines.py` & `harness_py_sdk-0.0.5/src/harness_py_sdk/harness_pipelines.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/src/harness_py_sdk/harness_services.py` & `harness_py_sdk-0.0.5/src/harness_py_sdk/harness_services.py`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/src/harness_py_sdk/harness_templates.py` & `harness_py_sdk-0.0.5/src/harness_py_sdk/harness_templates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from harness_base_service import HarnessBaseService
+class HarnessTemplates():
+    def __init__(self, harness_service):
+        self._harness_service = harness_service
 
-class HarnessTemplates(HarnessBaseService):
     def fetch_template_yaml(self, template_identifier, version, org_identifier=None, project_identifier=None):
-        endpoint = self._construct_url(template_identifier, "templates", org_identifier, project_identifier) + f"/versions/{version}"
-        return self._make_request("GET", endpoint)
+        endpoint = self._harness_service._construct_url(template_identifier, "templates", org_identifier, project_identifier) + f"/versions/{version}"
+        return self._harness_service._make_request("GET", endpoint)
     
     def fetch_stable_template_yaml(self, template_identifier, org_identifier=None, project_identifier=None):
-        return self._make_request("GET", self._construct_url(template_identifier, "templates", org_identifier, project_identifier))
+        return self._harness_service._make_request("GET", self._harness_service._construct_url(template_identifier, "templates", org_identifier, project_identifier))
     
     def create_template_pipeline(self, template_data, org_identifier=None, project_identifier=None):
-        return self._make_request(
+        return self._harness_service._make_request(
             "POST", 
-            self._construct_url(entity = "templates", org_identifier = org_identifier, project_identifier = project_identifier), 
+            self._harness_service._construct_url(entity = "templates", org_identifier = org_identifier, project_identifier = project_identifier), 
             json=template_data
         )
```

### Comparing `harness_py_sdk-0.0.4/LICENSE` & `harness_py_sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/README.md` & `harness_py_sdk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `harness_py_sdk-0.0.4/pyproject.toml` & `harness_py_sdk-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "harness-py-sdk"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Guilherme Zanini", email="guilherme.zanini@harness.io" },
 ]
 description = "This is a non-official package that leverages the Harness API using Python."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `harness_py_sdk-0.0.4/PKG-INFO` & `harness_py_sdk-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: harness-py-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is a non-official package that leverages the Harness API using Python.
 Project-URL: Homepage, https://github.com/guilhermezanini-harness/harness-py-sdk
 Project-URL: Issues, https://github.com/guilhermezanini-harness/harness-py-sdk/issues
 Author-email: Guilherme Zanini <guilherme.zanini@harness.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

