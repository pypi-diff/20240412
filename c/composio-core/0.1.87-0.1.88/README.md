# Comparing `tmp/composio_core-0.1.87.tar.gz` & `tmp/composio_core-0.1.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.87.tar", last modified: Thu Apr 11 12:40:19 2024, max compression
+gzip compressed data, was "composio_core-0.1.88.tar", last modified: Thu Apr 11 15:13:05 2024, max compression
```

## Comparing `composio_core-0.1.87.tar` & `composio_core-0.1.88.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.874112 composio_core-0.1.87/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.87/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 12:40:19.873878 composio_core-0.1.87/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.87/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.870844 composio_core-0.1.87/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.87/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    18767 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.872444 composio_core-0.1.87/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.87/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     6564 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    17472 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2997 2024-04-11 12:39:00.000000 composio_core-0.1.87/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 12:40:19.873585 composio_core-0.1.87/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-11 12:40:19.000000 composio_core-0.1.87/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.87/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.87/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 12:40:19.874159 composio_core-0.1.87/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-11 12:39:53.000000 composio_core-0.1.87/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.205449 composio_core-0.1.88/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.88/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 15:13:05.205254 composio_core-0.1.88/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.88/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.201385 composio_core-0.1.88/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.88/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    20845 2024-04-11 15:11:48.000000 composio_core-0.1.88/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.203939 composio_core-0.1.88/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.88/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     6590 2024-04-11 14:47:56.000000 composio_core-0.1.88/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-11 15:09:43.000000 composio_core-0.1.88/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    18019 2024-04-11 14:47:56.000000 composio_core-0.1.88/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.88/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3591 2024-04-11 15:11:48.000000 composio_core-0.1.88/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.205036 composio_core-0.1.88/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.88/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.88/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:05.205486 composio_core-0.1.88/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-11 15:12:31.000000 composio_core-0.1.88/setup.py
```

### Comparing `composio_core-0.1.87/PKG-INFO` & `composio_core-0.1.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.87
+Version: 0.1.88
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.87/composio/composio_cli.py` & `composio_core-0.1.88/composio/composio_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #!/usr/bin/env python3
 
 import argparse
 import json
+import os
 import sys
 from beaupy.spinners import Spinner, DOTS
 from rich.console import Console
 import termcolor
 from uuid import getnode as get_mac
 from .sdk.storage import get_user_connection, save_api_key, save_user_connection
 from .sdk.core import ComposioCore, UnauthorizedAccessException
-from .sdk.utils import generate_enums
+from .sdk.utils import generate_enums, generate_enums_beta
 from rich.table import Table
 
 import webbrowser
 
 console = Console()
 
+should_disable_webbrowser_open = os.getenv("DISABLE_COMPOSIO_WEBBROWSER_OPEN", "false") == "true"
+
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Composio CLI for adding integrations, managing skills, and showing apps.')
     subparsers = parser.add_subparsers(help='commands', dest='command')
     subparsers.required = True
 
     # Add integration command
     add_parser = subparsers.add_parser('add', help='Add an integration')
@@ -92,28 +95,34 @@
     logout_parser = subparsers.add_parser('logout', help='Logout from the current session')
     logout_parser.set_defaults(func=logout)
 
     # Generate enums command
     generate_enums_parser = subparsers.add_parser('update', help='Update enums for apps and actions')
     generate_enums_parser.set_defaults(func=handle_update)
 
+    # Generate beta enums command
+    generate_enums_beta_parser = subparsers.add_parser('update-beta', help='Update enums including beta for apps and actions')
+    generate_enums_beta_parser.set_defaults(func=handle_update_beta)
+
     return parser.parse_args()
 
 def login(args):
+    global should_disable_webbrowser_open
     client = ComposioCore()
     if client.is_authenticated():
         console.print("Already authenticated. Use [green]composio-cli logout[/green] to log out.\n")
         return
     
     console.print(f"\n[green]> Authenticating...[/green]\n")
     try:
         cli_key = client.generate_cli_auth_session()
         console.print(f"> Redirecting you to the login page. Please login using the following link:\n")
         console.print(f"[green]https://app.composio.dev/?cliKey={cli_key}[/green]\n")
-        webbrowser.open(f"https://app.composio.dev/?cliKey={cli_key}")
+        if not should_disable_webbrowser_open:
+            webbrowser.open(f"https://app.composio.dev/?cliKey={cli_key}")
 
         for attempt in range(3):
             try:
                 session_data = client.verify_cli_auth_session(cli_key, input("> Enter the code: "))
                 api_key = session_data.get('apiKey')
                 if api_key:
                     save_api_key(api_key)
@@ -288,40 +297,68 @@
         client.set_global_trigger(args.callback_url)
         console.print(f"\n[green]✔ Global trigger callback set successfully![/green]\n")
     except Exception as e:
         console.print(f"[red] Error occurred during setting global trigger callback: {e}[/red]")
         sys.exit(1)
 
 def handle_update(args):
-    client = ComposioCore()
     generate_enums()
     console.print(f"\n[green]✔ Enums updated successfully![/green]\n")
+    
+def handle_update_beta(args):
+    generate_enums_beta()
+    console.print(f"\n[green]✔ Enums(including Beta) updated successfully![/green]\n")
 
 def add_integration(args):
+    global should_disable_webbrowser_open
+
     client = ComposioCore()
     integration_name = args.integration_name
 
     existing_connection = get_user_connection(integration_name)
     if existing_connection is not None:
         console.print(f"[yellow]Warning: An existing connection for {integration_name} was found.[/yellow]\n")
         replace_connection = input("> Do you want to replace the existing connection? (yes/no): ").lower()
         if replace_connection not in ['yes', 'y']:
             console.print("\n[green]Existing connection retained. No new connection added.[/green]\n")
             return
 
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
-        # @TODO: add logic to wait and ask for API_KEY
-        connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
-        webbrowser.open(connection.redirectUrl)
-        print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
-        spinner = Spinner(DOTS, f"[yellow]⚠[/yellow] Waiting for {integration_name} authentication...")
-        spinner.start()
-        connected_account = connection.wait_until_active()
-        spinner.stop()
+        app = client.sdk.get_app(args.integration_name)
+        auth_schemes = app.get('auth_schemes')
+        auth_schemes_arr = [auth_scheme.get('auth_mode') for auth_scheme in auth_schemes]
+        if len(auth_schemes_arr) > 1 and auth_schemes_arr[0] == 'API_KEY':
+            connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
+            fields = auth_schemes[0].get('fields')
+            fields_input = {}
+            for field in fields:
+                if field.get('expected_from_customer', True):
+                    if field.get('required', False):
+                        console.print(f"[green]> Enter {field.get('displayName', field.get('name'))}: [/green]", end="")
+                        value = input() or field.get('default')
+                        if not value:  # If a required field is not provided and no default is available
+                            console.print(f"[red]Error: {field.get('displayName', field.get('name'))} is required[/red]")
+                            sys.exit(1)
+                    else:
+                        console.print(f"[green]> Enter {field.get('displayName', field.get('name'))} (Optional): [/green]", end="")
+                        value = input() or field.get('default')
+                    fields_input[field.get('name')] = value
+
+            connection.save_user_access_data(fields_input)
+        else: 
+            # @TODO: add logic to wait and ask for API_KEY
+            connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
+            if not should_disable_webbrowser_open:
+                webbrowser.open(connection.redirectUrl)
+            print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
+            spinner = Spinner(DOTS, f"[yellow]⚠[/yellow] Waiting for {integration_name} authentication...")
+            spinner.start()
+            connected_account = connection.wait_until_active()
+            spinner.stop()
         save_user_connection(connected_account.id, integration_name)
         print("")
         console.print(f"[green]✔[/green] {integration_name} added successfully!")
     except Exception as e:
         console.print(f"[red] Error occurred during adding integration: {e}[/red]")
         sys.exit(1)
 
@@ -338,15 +375,15 @@
     print("\n")
 
 def list_connections(args):
     client = ComposioCore()
     appName = args.appName
     console.print(f"\n[green]> Listing connections for: {appName}...[/green]\n")
     try:
-        connections = client.get_list_of_connections(appName)
+        connections = client.get_list_of_connections([appName])
         if connections:
             for connection in connections:
                 console.print(f"[yellow]- {connection['integrationId']} ({connection['status']})[/yellow]")
         else:
             console.print("[red] No connections found for the specified app.[/red]")
     except Exception as e:
         console.print(f"[red] Error occurred during listing connections: {e}[/red]")
@@ -385,10 +422,7 @@
         try:
             args.func(args)
         except Exception as e:
             console.print(f"[red]> Error occurred during command execution: \n{e}[/red]")
             sys.exit(1)
     else:
         console.print("[red]Error: No valid command provided. Use --help for more information.[/red]")
-
-if __name__ == "__main__":
-    main()
```

### Comparing `composio_core-0.1.87/composio/sdk/core.py` & `composio_core-0.1.88/composio/sdk/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,16 @@
         resp = account.execute_action(action, params)
         return resp
 
     def get_list_of_connections(self, app_name: list[Union[App, str]] = None) -> list[ConnectedAccount]:
         for i, item in enumerate(app_name):
             if isinstance(item, App):
                 app_name[i] = item.value
-
+        
+        resp = []
         if app_name is not None:
             resp = [item for item in resp if item.appUniqueId in app_name]
 
         return [{
             "id": item.id,
             "integrationId": item.integrationId,
             "status": item.status,
```

### Comparing `composio_core-0.1.87/composio/sdk/enums.py` & `composio_core-0.1.88/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.87/composio/sdk/sdk.py` & `composio_core-0.1.88/composio/sdk/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 
     sdk_instance: "Composio" = None
 
     def __init__(self, sdk_instance: "Composio", **data):
         super().__init__(**data)
         self.sdk_instance = sdk_instance
 
+    def save_user_access_data(self, field_inputs: dict):
+        connected_account_id = self.sdk_instance.get_connected_account(self.connectedAccountId)
+        resp = self.sdk_instance.http_client.post(f"{self.sdk_instance.base_url}/v1/connectedAccounts", json={
+            "integrationId": connected_account_id.integrationId,
+            "data": field_inputs,
+        })
+        return resp.json()
+
     def wait_until_active(
         self, timeout=60
     ) -> "ConnectedAccount":  # Timeout adjusted to seconds
         if not self.sdk_instance:
             raise ValueError("SDK instance not set.")
         start_time = time.time()
         while time.time() - start_time < timeout:
@@ -244,14 +252,18 @@
             return resp.json()
         
         raise Exception("Failed to set global trigger callback")
 
     def get_list_of_apps(self):
         resp = self.http_client.get(f"{self.base_url}/v1/apps")
         return resp.json()
+    
+    def get_app(self, app_name: str):
+        resp = self.http_client.get(f"{self.base_url}/v1/apps/{app_name}")
+        return resp.json()
 
     def get_list_of_actions(
         self, apps: list[App] = None, actions: list[Action] = None
     ) -> list:
         if apps is None or len(apps) == 0:
             resp = self.http_client.get(f"{self.base_url}/v1/actions")
         else:
```

### Comparing `composio_core-0.1.87/composio/sdk/storage.py` & `composio_core-0.1.88/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.87/composio/sdk/utils.py` & `composio_core-0.1.88/composio/sdk/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 
 def _get_enum_key(name):
     characters_to_replace = [' ', '-', '/', '(', ')', '\\', ':', '"', '\'', '.']
     for char in characters_to_replace:
         name = name.replace(char, '_')
     return name.upper()
 
-def generate_enums():
-    sdk_client = Composio(get_base_account_api_key())
-    apps = sdk_client.get_list_of_apps()
-    actions = sdk_client.get_list_of_actions()
-    triggers = sdk_client.get_list_of_triggers()
-
+def generate_enums_given_apps(apps, actions, triggers):
     enum_content = 'from enum import Enum\n\n'
     enum_content += 'class App(Enum):\n'
     for app in apps["items"]:
         app_name = app['key'].upper().replace(' ', '_').replace('-', '_')
         enum_content += f'    {app_name} = "{app["key"]}"\n'
     
     enum_content += "\n"
@@ -55,14 +50,33 @@
             enum_name = f'{app_key.upper()}_{_get_enum_key(trigger["display_name"])}'
             enum_value = f'("{app_key}", "{trigger["name"]}")'
             enum_content += f'    {enum_name} = {enum_value}\n'
         # enum_content += f'Actions.{app_name} = {app_name}\n\n'
     with open(os.path.join(os.path.dirname(__file__), 'enums.py'), 'w') as f:
         f.write(enum_content)
 
+def generate_enums():
+    sdk_client = Composio(get_base_account_api_key())
+    apps = sdk_client.get_list_of_apps()
+    actions = sdk_client.get_list_of_actions()
+    triggers = sdk_client.get_list_of_triggers()
+    apps["items"] = [appitem for appitem in apps["items"] if not appitem["name"].lower().endswith("beta")]
+    actions = [action for action in actions if not action["appName"].lower().endswith("beta")]
+    generate_enums_given_apps(apps, actions, triggers)
+
+
+def generate_enums_beta():
+    sdk_client = Composio(get_base_account_api_key())
+    apps = sdk_client.get_list_of_apps()
+    actions = sdk_client.get_list_of_actions()
+    triggers = sdk_client.get_list_of_triggers()
+    generate_enums_given_apps(apps, actions, triggers)
+    
+
+
 class GitUserInfo(BaseModel):
     name: Union[None, str] 
     email: Union[None, str] 
 
 def get_git_user_info() -> GitUserInfo:
     try:
         name = subprocess.check_output(['git', 'config', 'user.name']).strip().decode('utf-8')
```

### Comparing `composio_core-0.1.87/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.88/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.87
+Version: 0.1.88
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.87/pyproject.toml` & `composio_core-0.1.88/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.87/setup.py` & `composio_core-0.1.88/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.87",
+    version="0.1.88",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

