# Comparing `tmp/composio_core-0.1.89.tar.gz` & `tmp/composio_core-0.1.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.89.tar", last modified: Fri Apr 12 06:29:34 2024, max compression
+gzip compressed data, was "composio_core-0.1.90.tar", last modified: Fri Apr 12 10:06:08 2024, max compression
```

## Comparing `composio_core-0.1.89.tar` & `composio_core-0.1.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.406092 composio_core-0.1.89/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.89/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-12 06:29:34.405888 composio_core-0.1.89/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.89/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.401235 composio_core-0.1.89/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.89/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    20845 2024-04-12 06:28:43.000000 composio_core-0.1.89/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.404607 composio_core-0.1.89/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.89/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     6972 2024-04-12 06:26:15.000000 composio_core-0.1.89/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    13983 2024-04-12 06:27:53.000000 composio_core-0.1.89/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    18019 2024-04-11 14:47:56.000000 composio_core-0.1.89/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.89/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3591 2024-04-11 15:11:48.000000 composio_core-0.1.89/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.405642 composio_core-0.1.89/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.89/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.89/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-12 06:29:34.406170 composio_core-0.1.89/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-12 06:28:28.000000 composio_core-0.1.89/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.855112 composio_core-0.1.90/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.90/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:06:08.854892 composio_core-0.1.90/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.90/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.852859 composio_core-0.1.90/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      159 2024-04-12 09:34:06.000000 composio_core-0.1.90/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    20235 2024-04-12 09:44:09.000000 composio_core-0.1.90/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.853729 composio_core-0.1.90/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.90/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6982 2024-04-12 09:33:55.000000 composio_core-0.1.90/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    10555 2024-04-09 08:17:39.000000 composio_core-0.1.90/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    18979 2024-04-12 09:53:33.000000 composio_core-0.1.90/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2300 2024-04-11 09:58:04.000000 composio_core-0.1.90/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3328 2024-04-12 09:33:50.000000 composio_core-0.1.90/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-12 10:06:08.854648 composio_core-0.1.90/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      798 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      104 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-12 10:06:08.000000 composio_core-0.1.90/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      529 2024-04-09 10:58:09.000000 composio_core-0.1.90/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)      131 2024-04-12 09:01:50.000000 composio_core-0.1.90/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-12 10:06:08.855242 composio_core-0.1.90/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1128 2024-04-12 10:06:05.000000 composio_core-0.1.90/setup.py
```

### Comparing `composio_core-0.1.89/PKG-INFO` & `composio_core-0.1.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.89
+Version: 0.1.90
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.89/composio/composio_cli.py` & `composio_core-0.1.90/composio/composio_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 
 import argparse
 import json
 import os
 import sys
 from beaupy.spinners import Spinner, DOTS
 from rich.console import Console
-import termcolor
 from uuid import getnode as get_mac
 from .sdk.storage import get_user_connection, save_api_key, save_user_connection
 from .sdk.core import ComposioCore, UnauthorizedAccessException
 from .sdk.utils import generate_enums, generate_enums_beta
 from rich.table import Table
 
 import webbrowser
 
+from importlib.metadata import version
+import requests
+
 console = Console()
 
 should_disable_webbrowser_open = os.getenv("DISABLE_COMPOSIO_WEBBROWSER_OPEN", "false") == "true"
 
 def parse_arguments():
     parser = argparse.ArgumentParser(description='Composio CLI for adding integrations, managing skills, and showing apps.')
     subparsers = parser.add_subparsers(help='commands', dest='command')
@@ -384,41 +386,42 @@
             for connection in connections:
                 console.print(f"[yellow]- {connection['integrationId']} ({connection['status']})[/yellow]")
         else:
             console.print("[red] No connections found for the specified app.[/red]")
     except Exception as e:
         console.print(f"[red] Error occurred during listing connections: {e}[/red]")
         sys.exit(1)
-    
-def print_intro(): 
-        text = termcolor.colored('Composio', 'white', attrs=['bold'])  
-        aiPlatformText = termcolor.colored('100+', 'green', attrs=['bold'])
-        pinkEmojiText = termcolor.colored('hello@composio.dev', 'magenta', attrs=['bold'])
-        boldNoteText = termcolor.colored('Note*', 'white', attrs=['bold'])
-        print(f"""
-┌───────────────────────────────────────────────────────────────────────────┐
-│                                                                           │
-│                                       {text}                            │
-│                                                                           │
-│                     Plug {aiPlatformText} platforms in your agent                     │
-│                                                                           │
-│ {boldNoteText}: This package is in closed beta, please contact {pinkEmojiText}  │
-│        to get early access.                                               │
-│                                                                           │
-└───────────────────────────────────────────────────────────────────────────┘
-        """)
+
+def check_for_updates():
+    try:
+        installed_version = version('composio_core')
+    except Exception as e:
+        installed_version = "dev"
+        console.print(f"[red]Error fetching Composio Core version: {e}[/red]")
+
+    response = requests.get("https://pypi.org/pypi/composio_core/json")
+    latest_pypi_version = response.json()['info']['version']
+
+    console.print(f"\n Version: {installed_version} \n")
+
+    if(latest_pypi_version > installed_version):
+        console.print(f"\n[yellow] 🧐🧐 A newer version {latest_pypi_version} of composio-core is available. Please upgrade.[/yellow]")
+        console.print(f"\n 🔧🔧 Run [cyan]pip install --upgrade composio-core=={latest_pypi_version} [/cyan] to update.")
+
+def print_intro():
+        check_for_updates()
 
 def main():
     print_intro()
 
     args = parse_arguments()
 
     client = ComposioCore()
 
-    if client.is_authenticated() == False:
+    if not client.is_authenticated() and args.func.__name__ not in ['logout', 'whoami', 'login', 'update_base_url']:
         login(args)
         print("\n")
 
     if hasattr(args, 'func'):
         try:
             args.func(args)
         except Exception as e:
```

### Comparing `composio_core-0.1.89/composio/sdk/core.py` & `composio_core-0.1.90/composio/sdk/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 import requests
 
 from .utils import get_git_user_info
 from .sdk import ConnectionRequest, ConnectedAccount
 from .storage import delete_user_connections, get_base_url, get_user_connection, get_api_key, load_user_data, save_api_key, save_user_data, set_base_url
 from .sdk import Composio
-from .enums import TestIntegration, Action, App
+from .enums import Action, App
 from enum import Enum
 
 class FrameworkEnum(Enum):
     AUTOGEN = "autogen"
     LANGCHAIN = "langchain"
 
 __IS_FIRST_TIME__ = True
@@ -93,17 +93,18 @@
         if resp.status_code == 200:
             return resp.json()
         elif resp.status_code == 401:
             raise UnauthorizedAccessException("UnauthorizedError: Unauthorized access to cli/verify-cli-session")
         
         raise Exception("Bad request to cli/verify-cli-session")
     
-    def initiate_connection(self, integrationId: Union[str, TestIntegration]) -> ConnectionRequest:
-        if isinstance(integrationId, TestIntegration):
-            integrationId = integrationId.value
+    def initiate_connection(self, appName: Union[str, App], integrationId: str = None) -> ConnectionRequest:
+        if isinstance(appName, App) and integrationId is None:
+            integration = self.sdk.get_integration(appName, use_default=True)
+            integrationId = integration.id
 
         resp = self.http_client.post(f"{self.base_url}/v1/connectedAccounts", json={
             "integrationId": integrationId,
         })
         if resp.status_code == 200:
             return ConnectionRequest(self.sdk, **resp.json())
         
@@ -156,15 +157,14 @@
                 raise Exception(f"Entity {entity_id} does not have a connection to {tool_name}")
         else:
             connectionId = get_user_connection(tool_name)
             if not connectionId:
                 raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
             account = self.sdk.get_connected_account(connectionId)
 
-        account = self.sdk.get_connected_account(connectionId)
         resp = account.execute_action(action, params)
         return resp
 
     def get_list_of_connections(self, app_name: list[Union[App, str]] = None) -> list[ConnectedAccount]:
         for i, item in enumerate(app_name):
             if isinstance(item, App):
                 app_name[i] = item.value
```

### Comparing `composio_core-0.1.89/composio/sdk/enums.py` & `composio_core-0.1.90/composio/sdk/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,320 +1,242 @@
 from enum import Enum
 
 class App(Enum):
-    ASANA = "asana"
-    TRELLO = "trello"
-    LINEAR = "linear"
-    GOOGLE = "google"
     GMAIL = "gmail"
-    TIMELY = "timely"
-    BOX = "box"
-    JIRA = "jira"
-    MONDAY = "monday"
-    GOOGLE_SHEETS = "google-sheets"
     ATTIO = "attio"
-    SHOPIFY = "shopify"
-    SLACK = "slack"
+    ZENDESK = "zendesk"
+    TODOIST = "todoist"
+    KLAVIYO = "klaviyo"
     BITBUCKET = "bitbucket"
-    GOOGLE_DOCS = "google-docs"
-    EVENTBRITE = "eventbrite"
-    MAILCHIMP = "mailchimp"
+    MONDAY = "monday"
+    SLACK = "slack"
+    CLICKUP = "clickup"
+    DISCORD = "discord"
     STRAVA = "strava"
     DROPBOX = "dropbox"
-    PAGERDUTY = "pagerduty"
-    FIGMA = "figma"
-    CLICKUP = "clickup"
-    MIRO = "miro"
-    GUMROAD = "gumroad"
-    KLAVIYO = "klaviyo"
-    FRESHDESK = "freshdesk"
-    MIXPANEL = "mixpanel"
     INTERCOM = "intercom"
-    STACK_EXCHANGE = "stack-exchange"
-    ZOOM = "zoom"
-    ZOHO = "zoho"
-    SPLITWISE = "splitwise"
+    SHOPIFY = "shopify"
+    GOOGLE_SHEETS = "google-sheets"
+    ASANA = "asana"
+    EVENTBRITE = "eventbrite"
+    LINEAR = "linear"
+    HUBSPOT = "hubspot"
+    JIRA = "jira"
     NOTION = "notion"
     TASKADE = "taskade"
-    TYPEFORM = "typeform"
+    GOOGLE_DRIVE = "google-drive"
+    GITLAB = "gitlab"
+    MIXPANEL = "mixpanel"
+    GOOGLE_DOCS = "google-docs"
+    GUMROAD = "gumroad"
+    MAILCHIMP = "mailchimp"
+    BOX = "box"
+    MIRO = "miro"
+    KEAP = "keap"
+    SPLITWISE = "splitwise"
+    PAGERDUTY = "pagerduty"
+    ZOOM = "zoom"
+    TIMELY = "timely"
+    ZOHO = "zoho"
+    FRESHDESK = "freshdesk"
+    FIGMA = "figma"
     PIPEDRIVE = "pipedrive"
+    APIFY = "apify"
+    TWITCH = "twitch"
+    STACK_EXCHANGE = "stack-exchange"
+    GITHUB_OPEN_API_SPEC = "github_open_api_spec"
+    ACCELO = "accelo"
+    REDDIT = "reddit"
+    SURVEY_MONKEY = "survey-monkey"
     TWITTER = "twitter"
-    BOLDSIGN = "boldsign"
-    KEAP = "keap"
+    XERO = "xero"
+    ZOHO_INVENTORY = "zoho_inventory"
+    ZOHO_MAIL = "zoho_mail"
     AMAZON = "amazon"
-    SALESFORCE = "salesforce"
-    ZOHO_BOOKS = "zoho_books"
-    GORGIAS = "gorgias"
-    HACKERRANK_WORK = "hackerrank-work"
-    REDDIT = "reddit"
     SERVICEM8 = "servicem8"
     SHORTCUT = "shortcut"
-    FRONT = "front"
-    SURVEY_MONKEY = "survey-monkey"
+    ZOHO_BOOKS = "zoho_books"
+    ZOHO_INVOICE = "zoho_invoice"
+    GORGIAS = "gorgias"
+    SALESFORCE = "salesforce"
+    SMUGMUG = "smugmug"
     WAKATIME = "wakatime"
-    ZOHO_INVENTORY = "zoho_inventory"
-    DISCORD = "discord"
-    TWITCH = "twitch"
-    ATLASSIAN = "atlassian"
-    HARVEST = "harvest"
-    CALENDLY = "calendly"
-    GOOGLE_CALENDAR = "google_calendar"
+    ZOHO_BIGIN = "zoho_bigin"
+    ZOHO_DESK = "zoho_desk"
+    HACKERRANK_WORK = "hackerrank-work"
+    BOLDSIGN = "boldsign"
+    GURU = "guru"
     BAMBOOHR = "bamboohr"
-    GITHUB = "github"
+    HARVEST = "harvest"
+    ATLASSIAN = "atlassian"
     DEEL = "deel"
-    GITLAB = "gitlab"
-    HUBSPOT = "hubspot"
-    SLACKBOT = "slackbot"
-    YANDEX = "yandex"
-    BRAINTREE = "braintree"
-    ZOHO_INVOICE = "zoho_invoice"
+    FRONT = "front"
+    GITHUB = "github"
     FRESHBOOKS = "freshbooks"
-    AUTH0 = "auth0"
-    ONE_DRIVE = "one-drive"
-    OKTA = "okta"
-    ZOHO_DESK = "zoho_desk"
-    SMARTRECRUITERS = "smartrecruiters"
-    FACEBOOK = "facebook"
-    MURAL = "mural"
-    WORKABLE = "workable"
-    YOUTUBE = "youtube"
-    ADOBE = "adobe"
-    SQUARE = "square"
-    ASHBY = "ashby"
-    HIGHLEVEL = "highlevel"
-    GOOGLE_DRIVE = "google-drive"
-    EPIC_GAMES = "epic-games"
-    TODOIST = "todoist"
-    ZOHO_BIGIN = "zoho_bigin"
-    AMPLITUDE = "amplitude"
-    HEROKU = "heroku"
-    SAGE = "sage"
-    WAVE_ACCOUNTING = "wave-accounting"
-    CLOSE = "close"
-    PANDADOC = "pandadoc"
-    BLACKBAUD = "blackbaud"
-    GURU = "guru"
-    SERPAPI = "serpapi"
-    SMUGMUG = "smugmug"
-    BATTLENET = "battlenet"
-    LINKHUT = "linkhut"
-    XERO = "xero"
-    APIFY = "apify"
-    LINEARSANDBOX = "linearsandbox"
-    ZENDESK = "zendesk"
-    ZOHO_MAIL = "zoho_mail"
-    RING_CENTRAL = "ring-central"
-    CODEINTERPRETER = "CodeInterpreter"
-    GOOGLECALENDAR = "googlecalendar"
-    ACCELO = "accelo"
+    CALENDLY = "calendly"
+    TRELLO = "trello"
+    TYPEFORM = "typeform"
+    GOOGLE_CALENDAR = "google_calendar"
 
 class TestIntegration(Enum):
-    ASANA = "test-asana-connector"
-    TRELLO = "test-trello-connector"
-    LINEAR = "test-linear-connector"
-    GOOGLE = "test-google-connector"
     GMAIL = "test-gmail-connector"
-    TIMELY = "test-timely-connector"
-    BOX = "test-box-connector"
-    JIRA = "test-jira-connector"
-    MONDAY = "test-monday-connector"
-    GOOGLE_SHEETS = "test-google-sheets-connector"
     ATTIO = "test-attio-connector"
-    SHOPIFY = "test-shopify-connector"
-    SLACK = "test-slack-connector"
+    ZENDESK = "test-zendesk-connector"
+    TODOIST = "test-todoist-connector"
+    KLAVIYO = "test-klaviyo-connector"
     BITBUCKET = "test-bitbucket-connector"
-    GOOGLE_DOCS = "test-google-docs-connector"
-    EVENTBRITE = "test-eventbrite-connector"
-    MAILCHIMP = "test-mailchimp-connector"
+    MONDAY = "test-monday-connector"
+    SLACK = "test-slack-connector"
+    CLICKUP = "test-clickup-connector"
+    DISCORD = "test-discord-connector"
     STRAVA = "test-strava-connector"
     DROPBOX = "test-dropbox-connector"
-    PAGERDUTY = "test-pagerduty-connector"
-    FIGMA = "test-figma-connector"
-    CLICKUP = "test-clickup-connector"
-    MIRO = "test-miro-connector"
-    GUMROAD = "test-gumroad-connector"
-    KLAVIYO = "test-klaviyo-connector"
-    FRESHDESK = "test-freshdesk-connector"
-    MIXPANEL = "test-mixpanel-connector"
     INTERCOM = "test-intercom-connector"
-    STACK_EXCHANGE = "test-stack-exchange-connector"
-    ZOOM = "test-zoom-connector"
-    ZOHO = "test-zoho-connector"
-    SPLITWISE = "test-splitwise-connector"
+    SHOPIFY = "test-shopify-connector"
+    GOOGLE_SHEETS = "test-google-sheets-connector"
+    ASANA = "test-asana-connector"
+    EVENTBRITE = "test-eventbrite-connector"
+    LINEAR = "test-linear-connector"
+    HUBSPOT = "test-hubspot-connector"
+    JIRA = "test-jira-connector"
     NOTION = "test-notion-connector"
     TASKADE = "test-taskade-connector"
-    TYPEFORM = "test-typeform-connector"
+    GOOGLE_DRIVE = "test-google-drive-connector"
+    GITLAB = "test-gitlab-connector"
+    MIXPANEL = "test-mixpanel-connector"
+    GOOGLE_DOCS = "test-google-docs-connector"
+    GUMROAD = "test-gumroad-connector"
+    MAILCHIMP = "test-mailchimp-connector"
+    BOX = "test-box-connector"
+    MIRO = "test-miro-connector"
+    KEAP = "test-keap-connector"
+    SPLITWISE = "test-splitwise-connector"
+    PAGERDUTY = "test-pagerduty-connector"
+    ZOOM = "test-zoom-connector"
+    TIMELY = "test-timely-connector"
+    ZOHO = "test-zoho-connector"
+    FRESHDESK = "test-freshdesk-connector"
+    FIGMA = "test-figma-connector"
     PIPEDRIVE = "test-pipedrive-connector"
+    APIFY = "test-apify-connector"
+    TWITCH = "test-twitch-connector"
+    STACK_EXCHANGE = "test-stack-exchange-connector"
+    GITHUB_OPEN_API_SPEC = "test-github_open_api_spec-connector"
+    ACCELO = "test-accelo-connector"
+    REDDIT = "test-reddit-connector"
+    SURVEY_MONKEY = "test-survey-monkey-connector"
     TWITTER = "test-twitter-connector"
-    BOLDSIGN = "test-boldsign-connector"
-    KEAP = "test-keap-connector"
+    XERO = "test-xero-connector"
+    ZOHO_INVENTORY = "test-zoho_inventory-connector"
+    ZOHO_MAIL = "test-zoho_mail-connector"
     AMAZON = "test-amazon-connector"
-    SALESFORCE = "test-salesforce-connector"
-    ZOHO_BOOKS = "test-zoho_books-connector"
-    GORGIAS = "test-gorgias-connector"
-    HACKERRANK_WORK = "test-hackerrank-work-connector"
-    REDDIT = "test-reddit-connector"
     SERVICEM8 = "test-servicem8-connector"
     SHORTCUT = "test-shortcut-connector"
-    FRONT = "test-front-connector"
-    SURVEY_MONKEY = "test-survey-monkey-connector"
+    ZOHO_BOOKS = "test-zoho_books-connector"
+    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    GORGIAS = "test-gorgias-connector"
+    SALESFORCE = "test-salesforce-connector"
+    SMUGMUG = "test-smugmug-connector"
     WAKATIME = "test-wakatime-connector"
-    ZOHO_INVENTORY = "test-zoho_inventory-connector"
-    DISCORD = "test-discord-connector"
-    TWITCH = "test-twitch-connector"
-    ATLASSIAN = "test-atlassian-connector"
-    HARVEST = "test-harvest-connector"
-    CALENDLY = "test-calendly-connector"
-    GOOGLE_CALENDAR = "test-google_calendar-connector"
+    ZOHO_BIGIN = "test-zoho_bigin-connector"
+    ZOHO_DESK = "test-zoho_desk-connector"
+    HACKERRANK_WORK = "test-hackerrank-work-connector"
+    BOLDSIGN = "test-boldsign-connector"
+    GURU = "test-guru-connector"
     BAMBOOHR = "test-bamboohr-connector"
-    GITHUB = "test-github-connector"
+    HARVEST = "test-harvest-connector"
+    ATLASSIAN = "test-atlassian-connector"
     DEEL = "test-deel-connector"
-    GITLAB = "test-gitlab-connector"
-    HUBSPOT = "test-hubspot-connector"
-    SLACKBOT = "test-slackbot-connector"
-    YANDEX = "test-yandex-connector"
-    BRAINTREE = "test-braintree-connector"
-    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    FRONT = "test-front-connector"
+    GITHUB = "test-github-connector"
     FRESHBOOKS = "test-freshbooks-connector"
-    AUTH0 = "test-auth0-connector"
-    ONE_DRIVE = "test-one-drive-connector"
-    OKTA = "test-okta-connector"
-    ZOHO_DESK = "test-zoho_desk-connector"
-    SMARTRECRUITERS = "test-smartrecruiters-connector"
-    FACEBOOK = "test-facebook-connector"
-    MURAL = "test-mural-connector"
-    WORKABLE = "test-workable-connector"
-    YOUTUBE = "test-youtube-connector"
-    ADOBE = "test-adobe-connector"
-    SQUARE = "test-square-connector"
-    ASHBY = "test-ashby-connector"
-    HIGHLEVEL = "test-highlevel-connector"
-    GOOGLE_DRIVE = "test-google-drive-connector"
-    EPIC_GAMES = "test-epic-games-connector"
-    TODOIST = "test-todoist-connector"
-    ZOHO_BIGIN = "test-zoho_bigin-connector"
-    AMPLITUDE = "test-amplitude-connector"
-    HEROKU = "test-heroku-connector"
-    SAGE = "test-sage-connector"
-    WAVE_ACCOUNTING = "test-wave-accounting-connector"
-    CLOSE = "test-close-connector"
-    PANDADOC = "test-pandadoc-connector"
-    BLACKBAUD = "test-blackbaud-connector"
-    GURU = "test-guru-connector"
-    SERPAPI = "test-serpapi-connector"
-    SMUGMUG = "test-smugmug-connector"
-    BATTLENET = "test-battlenet-connector"
-    LINKHUT = "test-linkhut-connector"
-    XERO = "test-xero-connector"
-    APIFY = "test-apify-connector"
-    LINEARSANDBOX = "test-linearsandbox-connector"
-    ZENDESK = "test-zendesk-connector"
-    ZOHO_MAIL = "test-zoho_mail-connector"
-    RING_CENTRAL = "test-ring-central-connector"
-    CODEINTERPRETER = "test-CodeInterpreter-connector"
-    GOOGLECALENDAR = "test-googlecalendar-connector"
-    ACCELO = "test-accelo-connector"
+    CALENDLY = "test-calendly-connector"
+    TRELLO = "test-trello-connector"
+    TYPEFORM = "test-typeform-connector"
+    GOOGLE_CALENDAR = "test-google_calendar-connector"
 
 class Action(Enum):
     def __init__(self, service, action):
         self.service = service
         self.action = action
 
-    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
-    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
-    TRELLO_CREATE_TRELLO_LIST = ("trello", "trello_create_trello_list")
-    TRELLO_CREATE_TRELLO_CARD = ("trello", "trello_create_trello_card")
-    TRELLO_GET_TRELLO_BOARD_CARDS = ("trello", "trello_get_trello_board_cards")
-    TRELLO_DELETE_TRELLO_CARD = ("trello", "trello_delete_trello_card")
-    TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
-    TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
-    TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
-    TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
-    TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
-    TRELLO_SEARCH_TRELLO_MEMBER = ("trello", "trello_search_trello_member")
-    TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
-    TRELLO_GET_TRELLO_MEMBER_BOARD = ("trello", "trello_get_trello_member_board")
-    LINEAR_CREATE_LINEAR_ISSUE = ("linear", "linear_create_linear_issue")
-    LINEAR_LIST_LINEAR_PROJECTS = ("linear", "linear_list_linear_projects")
-    LINEAR_LIST_LINEAR_TEAMS = ("linear", "linear_list_linear_teams")
     GMAIL_SEND_EMAIL = ("gmail", "gmail_send_email")
     GMAIL_CREATE_EMAIL_DRAFT = ("gmail", "gmail_create_email_draft")
-    GMAIL_FIND_EMAIL_ID = ("gmail", "gmail_find_email_id")
-    GMAIL_FETCH_LAST_THREE_MESSAGES = ("gmail", "gmail_fetch_last_three_messages")
+    GMAIL_FIND_EMAIL_ID_IN_GMAIL = ("gmail", "gmail_find_email_id")
     GMAIL_ADD_LABEL_TO_EMAIL = ("gmail", "gmail_add_label_to_email")
-    GMAIL_LIST_LABELS = ("gmail", "gmail_list_labels")
-    GMAIL_FETCH_MESSAGE_BY_THREAD_ID = ("gmail", "gmail_fetch_message_by_thread_id")
-    GMAIL_REPLY_TO_THREAD = ("gmail", "gmail_reply_to_thread")
-    GMAIL_FETCH_EMAILS_WITH_LABEL = ("gmail", "gmail_fetch_emails_with_label")
+    ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
+    ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
+    ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
+    ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
+    ZENDESK_GET_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
+    ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
+    ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
+    ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
+    ZENDESK_GET_ZENDESK_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
     SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message")
-    SLACK_LIST_SLACK_CHANNELS = ("slack", "slack_list_slack_channels")
-    SLACK_LIST_SLACK_MEMBERS = ("slack", "slack_list_slack_members")
-    SLACK_LIST_SLACK_MESSAGES = ("slack", "slack_list_slack_messages")
-    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
+    SLACK_LIST_CHANNELS = ("slack", "slack_list_slack_channels")
+    SLACK_LIST_MEMBERS = ("slack", "slack_list_slack_members")
+    SLACK_LIST_MESSAGES = ("slack", "slack_list_slack_messages")
     CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
     CLICKUP_GET_TASKS = ("clickup", "clickup_get_tasks")
     CLICKUP_GET_TASK = ("clickup", "clickup_get_task")
     CLICKUP_CREATE_LIST = ("clickup", "clickup_create_list")
     CLICKUP_GET_LISTS = ("clickup", "clickup_get_lists")
     CLICKUP_GET_SPACES = ("clickup", "clickup_get_spaces")
     CLICKUP_CREATE_SPACE = ("clickup", "clickup_create_space")
     CLICKUP_CREATE_FOLDER = ("clickup", "clickup_create_folder")
     CLICKUP_GET_FOLDERS = ("clickup", "clickup_get_folders")
+    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
+    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
+    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
+    LINEAR_CREATE_ISSUE = ("linear", "linear_create_linear_issue")
+    LINEAR_GET_PROJECTS = ("linear", "linear_list_linear_projects")
+    LINEAR_GET_TEAMS_BY_PROJECT = ("linear", "linear_list_linear_teams")
     NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
-    NOTION_ADD_NOTION_PAGE_CHILDREN = ("notion", "notion_add_notion_page_children")
+    NOTION_ADD_CONTENT_NOTION_PAGE = ("notion", "notion_add_notion_page_children")
     NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
     NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
     NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
     NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
-    NOTION_DELETE_NOTION_PAGE_CHILDREN = ("notion", "notion_delete_notion_page_children")
-    NOTION_FETCH_NOTION_COMMENT = ("notion", "notion_fetch_notion_comment")
+    NOTION_DELETE_BLOCKS = ("notion", "notion_delete_notion_page_children")
+    NOTION_FETCH_ALL_UNRESOLVED_COMMENTS = ("notion", "notion_fetch_notion_comment")
     NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
     NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
-    NOTION_SEARCH_NOTION_PAGE = ("notion", "notion_search_notion_page")
+    NOTION_SEARCH_LIST_NOTION_PAGE = ("notion", "notion_search_notion_page")
     NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
-    NOTION_FETCH_NOTION_BLOCK = ("notion", "notion_fetch_notion_block")
-    NOTION_FETCH_NOTION_CHILD_BLOCK = ("notion", "notion_fetch_notion_child_block")
-    TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
+    NOTION_FETCH_NOTION_BLOCKS = ("notion", "notion_fetch_notion_block")
+    NOTION_FETCH_NOTION_BLOCK_CHILDREN = ("notion", "notion_fetch_notion_child_block")
+    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
+    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
+    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
+    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
+    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
+    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
     GITHUB_CREATE_ISSUE = ("github", "github_create_issue")
-    GITHUB_LIST_GITHUB_REPOS = ("github", "github_list_github_repos")
+    GITHUB_GET_REPOSITORY = ("github", "github_list_github_repos")
     GITHUB_STAR_REPO = ("github", "github_star_repo")
     GITHUB_GET_ABOUT_ME = ("github", "github_get_about_me")
     GITHUB_FETCH_README = ("github", "github_fetch_readme")
     GITHUB_GET_COMMITS = ("github", "github_get_commits")
-    GITHUB_GET_COMMITS_WITH_CODE = ("github", "github_get_commits_with_code")
+    GITHUB_GET_COMMITS_WITH_PATCH_FILE_FOR_THAT_COMMIT = ("github", "github_get_commits_with_code")
     GITHUB_GET_PATCH_FOR_COMMIT = ("github", "github_get_patch_for_commit")
-    SLACKBOT_SEND_SLACK_MESSAGE = ("slackbot", "slackbot_send_slack_message")
-    SLACKBOT_LIST_SLACK_CHANNELS = ("slackbot", "slackbot_list_slack_channels")
-    SLACKBOT_LIST_SLACK_MEMBERS = ("slackbot", "slackbot_list_slack_members")
-    SLACKBOT_LIST_SLACK_MESSAGES = ("slackbot", "slackbot_list_slack_messages")
-    SERPAPI_SEARCH = ("serpapi", "serpapi_search")
-    APIFY_LIST_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
-    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
-    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
-    APIFY_SEARCH_STORE = ("apify", "apify_search_store")
-    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
-    APIFY_LIST_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
-    ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
-    ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
-    ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
-    ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
-    ZENDESK_GET_ALL_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
-    ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
-    ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
-    ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
-    ZENDESK_GET_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
-    GOOGLECALENDAR_CREATE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_create_google_event")
-    GOOGLECALENDAR_REMOVE_ATTENDEE = ("googlecalendar", "googlecalendar_remove_attendee")
-    GOOGLECALENDAR_FIND_EVENT = ("googlecalendar", "googlecalendar_find_event")
-    GOOGLECALENDAR_CHECK_ATTENDEES = ("googlecalendar", "googlecalendar_check_attendees")
-    GOOGLECALENDAR_DELETE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_delete_google_event")
-    GOOGLECALENDAR_UPDATE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_update_google_event")
+    TRELLO_CREATE_TRELLO_LIST = ("trello", "trello_create_trello_list")
+    TRELLO_CREATE_TRELLO_CARD = ("trello", "trello_create_trello_card")
+    TRELLO_GET_TRELLO_BOARD_CARDS = ("trello", "trello_get_trello_board_cards")
+    TRELLO_DELETE_TRELLO_CARD = ("trello", "trello_delete_trello_card")
+    TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
+    TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
+    TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
+    TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
+    TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
+    TRELLO_SEARCH_TRELLO_MEMBERS = ("trello", "trello_search_trello_member")
+    TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
+    TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
 
 class Trigger(Enum):
     def __init__(self, service, trigger):
         self.service = service
         self.trigger = trigger
 
     SLACK_NEW_MESSAGE = ("slack", "slack_receive_message")
     GITHUB_PULL_REQUEST_EVENT = ("github", "github_pull_request_event")
     GITHUB_COMMIT_EVENT = ("github", "github_commit_event")
-    SLACKBOT_NEW_MESSAGE = ("slackbot", "slackbot_receive_message")
```

### Comparing `composio_core-0.1.89/composio/sdk/sdk.py` & `composio_core-0.1.90/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import time
 from typing import Optional, Union, Tuple
 import requests
 from pydantic import BaseModel, ConfigDict
 
-from .enums import Action, App, TestIntegration
+from .enums import Action, App
 from .storage import get_base_url
 from openai.types.chat.chat_completion import ChatCompletion
 from openai.types.beta.threads import run
 from openai import Client
 from openai.types.beta import thread
 import json
 
@@ -44,14 +44,15 @@
         start_time = time.time()
         while time.time() - start_time < timeout:
             connection_info = self.sdk_instance.get_connected_account(
                 self.connectedAccountId
             )
             if connection_info.status == "ACTIVE":
                 return connection_info
+                
             time.sleep(1)
         raise TimeoutError(
             "Connection did not become active within the timeout period."
         )
 
 
 class AuthConnectionParams(BaseModel):
@@ -304,38 +305,53 @@
         resp = self.http_client.get(f"{self.base_url}/v1/integrations")
         if resp.status_code != 200:
             raise Exception("Failed to get integrations")
 
         resp = resp.json()
         return [Integration(self, **app) for app in resp["items"]]
 
-    def get_integration(self, connector_id: Union[str, TestIntegration]) -> Integration:
-        if isinstance(connector_id, TestIntegration):
-            connector_id = connector_id.value
+    def get_integration(self, connector_id: Union[str, App]) -> Integration:
+        if isinstance(connector_id, App):
+            return self.create_integration(connector_id, use_default=True)
+
         resp = self.http_client.get(f"{self.base_url}/v1/integrations/{connector_id}")
         if resp.status_code == 200:
             return Integration(self, **resp.json())
+        
+    def create_integration(self, app: Union[App, str], use_default = False) -> Integration:
+        if isinstance(app, App):
+            app = app.value
+        app_details = self.get_app(app)
+        app_id = app_details.get("appId")
+        if app_id is None:
+            raise Exception(f"App {app} does not exist for the account")
+        resp = self.http_client.post(f"{self.base_url}/v1/integrations", json={
+            "appId": app_id,
+            "useComposioAuth": use_default
+        })
+        if resp.status_code == 200:
+            return Integration(self, **resp.json())
 
         raise Exception("Failed to get connector")
 
     def get_connected_account(self, connection_id: str) -> ConnectedAccount:
         resp = self.http_client.get(
             f"{self.base_url}/v1/connectedAccounts/{connection_id}"
         )
         if resp.status_code == 200:
             return ConnectedAccount(self, **resp.json())
 
         raise Exception("Failed to get connection")
 
     def get_connected_accounts(
-        self, entity_id: Union[list[str], str]
+        self, entity_id: Union[list[str], str], status: str = None
     ) -> list[ConnectedAccount]:
         user_uuid_str = entity_id if isinstance(entity_id, str) else ",".join(entity_id)
         resp = self.http_client.get(
-            f"{self.base_url}/v1/connectedAccounts?user_uuid={user_uuid_str}"
+            f"{self.base_url}/v1/connectedAccounts?user_uuid={user_uuid_str}{'&status=' + status if status else ''}"
         )
         if resp.status_code == 200:
             return [ConnectedAccount(self, **item) for item in resp.json()["items"]]
 
         raise Exception("Failed to get connected accounts")
 
     def get_list_of_connected_accounts(self) -> list[ConnectedAccount]:
@@ -380,21 +396,28 @@
         )
 
         for account in connected_accounts:
             account_actions = account.get_all_actions()
             actions.extend(account_actions)
         return actions
 
-    def get_connection(self, tool_name: str) -> ConnectedAccount:
+    def get_connection(self, app_name: Union[str, App]) -> ConnectedAccount:
+        if isinstance(app_name, App):
+            app_name = app_name.value
         connected_accounts = self.client.get_connected_accounts(
-            entity_id=self.entity_id
+            entity_id=self.entity_id,
+            status="ACTIVE"
         )
         for account in connected_accounts:
-            if tool_name == account.appUniqueId:
+            if app_name == account.appUniqueId:
                 return account
+            
+    def is_app_authenticated(self, app_name: Union[str, App]) -> bool:
+        connected_account = self.get_connection(app_name)
+        return connected_account is not None
 
     def handle_tools_calls(
         self, tool_calls: ChatCompletion, verbose: bool = False
     ) -> list[any]:
         output = []
         try:
             if tool_calls.choices:
@@ -402,15 +425,15 @@
                     if choice.message.tool_calls:
                         for tool_call in choice.message.tool_calls:
                             action_name_to_execute = tool_call.function.name
                             action = self.client.get_action_enum_without_tool(
                                 action_name=action_name_to_execute
                             )
                             arguments = json.loads(tool_call.function.arguments)
-                            account = self.get_connection(tool_name=action.service)
+                            account = self.get_connection(app_name=action.service)
                             output.append(account.execute_action(action, arguments))
 
         except Exception as e:
             print(e)
             return output
 
         return output
@@ -422,15 +445,15 @@
             for tool_call in require_action.tool_calls:
                 if tool_call.type == "function":
                     action_name_to_execute = tool_call.function.name
                     action = self.client.get_action_enum_without_tool(
                         action_name=action_name_to_execute
                     )
                     arguments = json.loads(tool_call.function.arguments)
-                    account = self.get_connection(tool_name=action.service)
+                    account = self.get_connection(app_name=action.service)
                     if verbose:
                         print("Executing Function: ", action)
                         print("Arguments: ", arguments)
                     response = account.execute_action(action, arguments)
                     if verbose:
                         print("Output", response)
                     output = {
@@ -470,10 +493,10 @@
                 run_object = client.beta.threads.runs.retrieve(
                     thread_id=thread_object.id,
                     run_id=run_object.id,
                 )
                 time.sleep(0.5)
         return run_object
 
-    def initiate_connection(self, integration_id: str):
-        integration = self.client.get_integration(integration_id)
+    def initiate_connection(self, app_name: Union[str, App]):
+        integration = self.client.get_integration(app_name)
         return integration.initiate_connection(entity_id=self.entity_id)
```

### Comparing `composio_core-0.1.89/composio/sdk/storage.py` & `composio_core-0.1.90/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.89/composio/sdk/utils.py` & `composio_core-0.1.90/composio/sdk/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,20 +14,14 @@
 
 def generate_enums_given_apps(apps, actions, triggers):
     enum_content = 'from enum import Enum\n\n'
     enum_content += 'class App(Enum):\n'
     for app in apps["items"]:
         app_name = app['key'].upper().replace(' ', '_').replace('-', '_')
         enum_content += f'    {app_name} = "{app["key"]}"\n'
-    
-    enum_content += "\n"
-    enum_content += 'class TestIntegration(Enum):\n'
-    for app in apps["items"]:
-        app_name = app['key'].upper().replace(' ', '_').replace('-', '_')
-        enum_content += f'    {app_name} = "test-{app["key"]}-connector"\n'
 
     enum_content += '\n'
     enum_content += 'class Action(Enum):\n'
     enum_content += '    def __init__(self, service, action):\n'
     enum_content += '        self.service = service\n'
     enum_content += '        self.action = action\n\n'
     for app in apps["items"]:
```

### Comparing `composio_core-0.1.89/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.90/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.89
+Version: 0.1.90
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.89/pyproject.toml` & `composio_core-0.1.90/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.89/setup.py` & `composio_core-0.1.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.89",
+    version="0.1.90",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

