# Comparing `tmp/composio_core-0.1.94.tar.gz` & `tmp/composio_core-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.94.tar", last modified: Fri Apr 12 13:10:24 2024, max compression
+gzip compressed data, was "composio_core-0.1.95.tar", last modified: Fri Apr 12 13:33:16 2024, max compression
```

## Comparing `composio_core-0.1.94.tar` & `composio_core-0.1.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.538917 composio_core-0.1.94/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.94/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:10:24.538689 composio_core-0.1.94/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.94/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.536001 composio_core-0.1.94/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.94/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    21929 2024-04-12 10:26:25.000000 composio_core-0.1.94/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.537402 composio_core-0.1.94/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.94/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.94/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.94/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.94/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.94/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.94/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:10:24.538438 composio_core-0.1.94/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 13:10:24.000000 composio_core-0.1.94/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.94/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.94/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 13:10:24.538969 composio_core-0.1.94/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 13:10:03.000000 composio_core-0.1.94/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:33:16.028974 composio_core-0.1.95/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.95/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:33:16.028753 composio_core-0.1.95/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.95/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:33:16.025651 composio_core-0.1.95/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.95/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    21879 2024-04-12 13:27:15.000000 composio_core-0.1.95/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:33:16.027459 composio_core-0.1.95/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.95/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7024 2024-04-12 13:31:18.000000 composio_core-0.1.95/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10226 2024-04-12 13:08:03.000000 composio_core-0.1.95/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    19094 2024-04-12 13:26:45.000000 composio_core-0.1.95/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.95/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.95/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 13:33:16.028491 composio_core-0.1.95/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 13:33:16.000000 composio_core-0.1.95/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.95/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.95/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 13:33:16.029060 composio_core-0.1.95/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 13:32:55.000000 composio_core-0.1.95/setup.py
```

### Comparing `composio_core-0.1.94/PKG-INFO` & `composio_core-0.1.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.94
+Version: 0.1.95
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.94/composio/composio_cli.py` & `composio_core-0.1.95/composio/composio_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,15 @@
 
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
         app = client.sdk.get_app(args.integration_name)
         auth_schemes = app.get('auth_schemes')
         auth_schemes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
         if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] == 'API_KEY':
-            connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
+            connection = client.initiate_connection(integration_name.lower())
             fields = auth_schemes[0].get('fields')
             fields_input = {}
             for field in fields:
                 if field.get('expected_from_customer', True):
                     if field.get('required', False):
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))}: [/green]", end="")
                         value = input() or field.get('default')
@@ -349,15 +349,15 @@
                         console.print(f"[green]> Enter {field.get('displayName', field.get('name'))} (Optional): [/green]", end="")
                         value = input() or field.get('default')
                     fields_input[field.get('name')] = value
 
             connection.save_user_access_data(fields_input)
         else: 
             # @TODO: add logic to wait and ask for API_KEY
-            connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
+            connection = client.initiate_connection(integration_name.lower())
             if not should_disable_webbrowser_open:
                 webbrowser.open(connection.redirectUrl)
             print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
             spinner = Spinner(DOTS, f"[yellow]⚠[/yellow] Waiting for {integration_name} authentication...")
             spinner.start()
             connected_account = connection.wait_until_active()
             spinner.stop()
```

### Comparing `composio_core-0.1.94/composio/sdk/core.py` & `composio_core-0.1.95/composio/sdk/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,18 @@
             return resp.json()
         elif resp.status_code == 401:
             raise UnauthorizedAccessException("UnauthorizedError: Unauthorized access to cli/verify-cli-session")
         
         raise Exception("Bad request to cli/verify-cli-session")
     
     def initiate_connection(self, appName: Union[str, App], integrationId: str = None) -> ConnectionRequest:
-        if isinstance(appName, App) and integrationId is None:
-            integration = self.sdk.get_integration(appName, use_default=True)
+        if integrationId is None:
+            if isinstance(appName, App):
+                appName = appName.value
+            integration = self.sdk.get_default_integration(appName)
             integrationId = integration.id
 
         resp = self.http_client.post(f"{self.base_url}/v1/connectedAccounts", json={
             "integrationId": integrationId,
         })
         if resp.status_code == 200:
             return ConnectionRequest(self.sdk, **resp.json())
```

### Comparing `composio_core-0.1.94/composio/sdk/enums.py` & `composio_core-0.1.95/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.94/composio/sdk/sdk.py` & `composio_core-0.1.95/composio/sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,18 +305,21 @@
         resp = self.http_client.get(f"{self.base_url}/v1/integrations")
         if resp.status_code != 200:
             raise Exception("Failed to get integrations")
 
         resp = resp.json()
         return [Integration(self, **app) for app in resp["items"]]
 
-    def get_integration(self, connector_id: Union[str, App]) -> Integration:
-        if isinstance(connector_id, App):
-            return self.create_integration(connector_id, use_default=True)
-
+    def get_default_integration(self, appName: Union[str, App]) -> Integration:
+        if isinstance(appName, App):
+            appName = appName.value
+        
+        return self.create_integration(appName, use_default=True)
+        
+    def get_integration(self, connector_id: str) -> Integration:
         resp = self.http_client.get(f"{self.base_url}/v1/integrations/{connector_id}")
         if resp.status_code == 200:
             return Integration(self, **resp.json())
         
     def create_integration(self, app: Union[App, str], use_default = False) -> Integration:
         if isinstance(app, App):
             app = app.value
@@ -494,9 +497,9 @@
                     thread_id=thread_object.id,
                     run_id=run_object.id,
                 )
                 time.sleep(0.5)
         return run_object
 
     def initiate_connection(self, app_name: Union[str, App]):
-        integration = self.client.get_integration(app_name)
+        integration = self.client.get_default_integration(app_name)
         return integration.initiate_connection(entity_id=self.entity_id)
```

### Comparing `composio_core-0.1.94/composio/sdk/storage.py` & `composio_core-0.1.95/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.94/composio/sdk/utils.py` & `composio_core-0.1.95/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.94/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.95/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.94
+Version: 0.1.95
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.94/pyproject.toml` & `composio_core-0.1.95/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.94/setup.py` & `composio_core-0.1.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.94",
+    version="0.1.95",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

