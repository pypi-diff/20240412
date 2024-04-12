# Comparing `tmp/composio_core-0.1.88.tar.gz` & `tmp/composio_core-0.1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.88.tar", last modified: Thu Apr 11 15:13:05 2024, max compression
+gzip compressed data, was "composio_core-0.1.89.tar", last modified: Fri Apr 12 06:29:34 2024, max compression
```

## Comparing `composio_core-0.1.88.tar` & `composio_core-0.1.89.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.205449 composio_core-0.1.88/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.88/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 15:13:05.205254 composio_core-0.1.88/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.88/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.201385 composio_core-0.1.88/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.88/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    20845 2024-04-11 15:11:48.000000 composio_core-0.1.88/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.203939 composio_core-0.1.88/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.88/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     6590 2024-04-11 14:47:56.000000 composio_core-0.1.88/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    10555 2024-04-11 15:09:43.000000 composio_core-0.1.88/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    18019 2024-04-11 14:47:56.000000 composio_core-0.1.88/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.88/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3591 2024-04-11 15:11:48.000000 composio_core-0.1.88/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-11 15:13:05.205036 composio_core-0.1.88/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-11 15:13:05.000000 composio_core-0.1.88/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.88/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.88/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-11 15:13:05.205486 composio_core-0.1.88/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-11 15:12:31.000000 composio_core-0.1.88/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.406092 composio_core-0.1.89/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.89/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-12 06:29:34.405888 composio_core-0.1.89/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.89/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.401235 composio_core-0.1.89/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.89/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    20845 2024-04-12 06:28:43.000000 composio_core-0.1.89/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.404607 composio_core-0.1.89/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.89/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     6972 2024-04-12 06:26:15.000000 composio_core-0.1.89/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    13983 2024-04-12 06:27:53.000000 composio_core-0.1.89/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    18019 2024-04-11 14:47:56.000000 composio_core-0.1.89/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2300 2024-04-11 12:39:00.000000 composio_core-0.1.89/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3591 2024-04-11 15:11:48.000000 composio_core-0.1.89/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-12 06:29:34.405642 composio_core-0.1.89/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      798 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      104 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-12 06:29:34.000000 composio_core-0.1.89/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      529 2024-04-11 12:39:00.000000 composio_core-0.1.89/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      105 2024-04-11 12:39:00.000000 composio_core-0.1.89/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-12 06:29:34.406170 composio_core-0.1.89/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1128 2024-04-12 06:28:28.000000 composio_core-0.1.89/setup.py
```

### Comparing `composio_core-0.1.88/PKG-INFO` & `composio_core-0.1.89/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.88
+Version: 0.1.89
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.88/composio/composio_cli.py` & `composio_core-0.1.89/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.88/composio/sdk/core.py` & `composio_core-0.1.89/composio/sdk/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,19 +143,26 @@
         except Exception as e:
             raise Exception(e)
 
     def get_saved_connections(self, app_name: str = None):
         connectionId = get_user_connection(app_name)
         return connectionId
 
-    def execute_action(self, action: Action, params: dict):
+    def execute_action(self, action: Action, params: dict, entity_id: str = None):
         tool_name  = action.value[0]
-        connectionId = get_user_connection(tool_name)
-        if not connectionId:
-            raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
+        if entity_id is not None:
+            entity = self.sdk.get_entity(entity_id)
+            account = entity.get_connection(tool_name)
+            if not account:
+                raise Exception(f"Entity {entity_id} does not have a connection to {tool_name}")
+        else:
+            connectionId = get_user_connection(tool_name)
+            if not connectionId:
+                raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
+            account = self.sdk.get_connected_account(connectionId)
 
         account = self.sdk.get_connected_account(connectionId)
         resp = account.execute_action(action, params)
         return resp
 
     def get_list_of_connections(self, app_name: list[Union[App, str]] = None) -> list[ConnectedAccount]:
         for i, item in enumerate(app_name):
```

### Comparing `composio_core-0.1.88/composio/sdk/enums.py` & `composio_core-0.1.89/composio/sdk/enums.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,242 +1,320 @@
 from enum import Enum
 
 class App(Enum):
-    GMAIL = "gmail"
-    ATTIO = "attio"
-    ZENDESK = "zendesk"
-    TODOIST = "todoist"
-    KLAVIYO = "klaviyo"
-    BITBUCKET = "bitbucket"
-    MONDAY = "monday"
-    SLACK = "slack"
-    CLICKUP = "clickup"
-    DISCORD = "discord"
-    STRAVA = "strava"
-    DROPBOX = "dropbox"
-    INTERCOM = "intercom"
-    SHOPIFY = "shopify"
-    GOOGLE_SHEETS = "google-sheets"
     ASANA = "asana"
-    EVENTBRITE = "eventbrite"
+    TRELLO = "trello"
     LINEAR = "linear"
-    HUBSPOT = "hubspot"
+    GOOGLE = "google"
+    GMAIL = "gmail"
+    TIMELY = "timely"
+    BOX = "box"
     JIRA = "jira"
-    NOTION = "notion"
-    TASKADE = "taskade"
-    GOOGLE_DRIVE = "google-drive"
-    GITLAB = "gitlab"
-    MIXPANEL = "mixpanel"
+    MONDAY = "monday"
+    GOOGLE_SHEETS = "google-sheets"
+    ATTIO = "attio"
+    SHOPIFY = "shopify"
+    SLACK = "slack"
+    BITBUCKET = "bitbucket"
     GOOGLE_DOCS = "google-docs"
-    GUMROAD = "gumroad"
+    EVENTBRITE = "eventbrite"
     MAILCHIMP = "mailchimp"
-    BOX = "box"
-    MIRO = "miro"
-    KEAP = "keap"
-    SPLITWISE = "splitwise"
+    STRAVA = "strava"
+    DROPBOX = "dropbox"
     PAGERDUTY = "pagerduty"
+    FIGMA = "figma"
+    CLICKUP = "clickup"
+    MIRO = "miro"
+    GUMROAD = "gumroad"
+    KLAVIYO = "klaviyo"
+    FRESHDESK = "freshdesk"
+    MIXPANEL = "mixpanel"
+    INTERCOM = "intercom"
+    STACK_EXCHANGE = "stack-exchange"
     ZOOM = "zoom"
-    TIMELY = "timely"
     ZOHO = "zoho"
-    FRESHDESK = "freshdesk"
-    FIGMA = "figma"
+    SPLITWISE = "splitwise"
+    NOTION = "notion"
+    TASKADE = "taskade"
+    TYPEFORM = "typeform"
     PIPEDRIVE = "pipedrive"
-    APIFY = "apify"
-    TWITCH = "twitch"
-    STACK_EXCHANGE = "stack-exchange"
-    GITHUB_OPEN_API_SPEC = "github_open_api_spec"
-    ACCELO = "accelo"
-    REDDIT = "reddit"
-    SURVEY_MONKEY = "survey-monkey"
     TWITTER = "twitter"
-    XERO = "xero"
-    ZOHO_INVENTORY = "zoho_inventory"
-    ZOHO_MAIL = "zoho_mail"
+    BOLDSIGN = "boldsign"
+    KEAP = "keap"
     AMAZON = "amazon"
-    SERVICEM8 = "servicem8"
-    SHORTCUT = "shortcut"
+    SALESFORCE = "salesforce"
     ZOHO_BOOKS = "zoho_books"
-    ZOHO_INVOICE = "zoho_invoice"
     GORGIAS = "gorgias"
-    SALESFORCE = "salesforce"
-    SMUGMUG = "smugmug"
-    WAKATIME = "wakatime"
-    ZOHO_BIGIN = "zoho_bigin"
-    ZOHO_DESK = "zoho_desk"
     HACKERRANK_WORK = "hackerrank-work"
-    BOLDSIGN = "boldsign"
-    GURU = "guru"
-    BAMBOOHR = "bamboohr"
-    HARVEST = "harvest"
-    ATLASSIAN = "atlassian"
-    DEEL = "deel"
+    REDDIT = "reddit"
+    SERVICEM8 = "servicem8"
+    SHORTCUT = "shortcut"
     FRONT = "front"
-    GITHUB = "github"
-    FRESHBOOKS = "freshbooks"
+    SURVEY_MONKEY = "survey-monkey"
+    WAKATIME = "wakatime"
+    ZOHO_INVENTORY = "zoho_inventory"
+    DISCORD = "discord"
+    TWITCH = "twitch"
+    ATLASSIAN = "atlassian"
+    HARVEST = "harvest"
     CALENDLY = "calendly"
-    TRELLO = "trello"
-    TYPEFORM = "typeform"
     GOOGLE_CALENDAR = "google_calendar"
+    BAMBOOHR = "bamboohr"
+    GITHUB = "github"
+    DEEL = "deel"
+    GITLAB = "gitlab"
+    HUBSPOT = "hubspot"
+    SLACKBOT = "slackbot"
+    YANDEX = "yandex"
+    BRAINTREE = "braintree"
+    ZOHO_INVOICE = "zoho_invoice"
+    FRESHBOOKS = "freshbooks"
+    AUTH0 = "auth0"
+    ONE_DRIVE = "one-drive"
+    OKTA = "okta"
+    ZOHO_DESK = "zoho_desk"
+    SMARTRECRUITERS = "smartrecruiters"
+    FACEBOOK = "facebook"
+    MURAL = "mural"
+    WORKABLE = "workable"
+    YOUTUBE = "youtube"
+    ADOBE = "adobe"
+    SQUARE = "square"
+    ASHBY = "ashby"
+    HIGHLEVEL = "highlevel"
+    GOOGLE_DRIVE = "google-drive"
+    EPIC_GAMES = "epic-games"
+    TODOIST = "todoist"
+    ZOHO_BIGIN = "zoho_bigin"
+    AMPLITUDE = "amplitude"
+    HEROKU = "heroku"
+    SAGE = "sage"
+    WAVE_ACCOUNTING = "wave-accounting"
+    CLOSE = "close"
+    PANDADOC = "pandadoc"
+    BLACKBAUD = "blackbaud"
+    GURU = "guru"
+    SERPAPI = "serpapi"
+    SMUGMUG = "smugmug"
+    BATTLENET = "battlenet"
+    LINKHUT = "linkhut"
+    XERO = "xero"
+    APIFY = "apify"
+    LINEARSANDBOX = "linearsandbox"
+    ZENDESK = "zendesk"
+    ZOHO_MAIL = "zoho_mail"
+    RING_CENTRAL = "ring-central"
+    CODEINTERPRETER = "CodeInterpreter"
+    GOOGLECALENDAR = "googlecalendar"
+    ACCELO = "accelo"
 
 class TestIntegration(Enum):
-    GMAIL = "test-gmail-connector"
-    ATTIO = "test-attio-connector"
-    ZENDESK = "test-zendesk-connector"
-    TODOIST = "test-todoist-connector"
-    KLAVIYO = "test-klaviyo-connector"
-    BITBUCKET = "test-bitbucket-connector"
-    MONDAY = "test-monday-connector"
-    SLACK = "test-slack-connector"
-    CLICKUP = "test-clickup-connector"
-    DISCORD = "test-discord-connector"
-    STRAVA = "test-strava-connector"
-    DROPBOX = "test-dropbox-connector"
-    INTERCOM = "test-intercom-connector"
-    SHOPIFY = "test-shopify-connector"
-    GOOGLE_SHEETS = "test-google-sheets-connector"
     ASANA = "test-asana-connector"
-    EVENTBRITE = "test-eventbrite-connector"
+    TRELLO = "test-trello-connector"
     LINEAR = "test-linear-connector"
-    HUBSPOT = "test-hubspot-connector"
+    GOOGLE = "test-google-connector"
+    GMAIL = "test-gmail-connector"
+    TIMELY = "test-timely-connector"
+    BOX = "test-box-connector"
     JIRA = "test-jira-connector"
-    NOTION = "test-notion-connector"
-    TASKADE = "test-taskade-connector"
-    GOOGLE_DRIVE = "test-google-drive-connector"
-    GITLAB = "test-gitlab-connector"
-    MIXPANEL = "test-mixpanel-connector"
+    MONDAY = "test-monday-connector"
+    GOOGLE_SHEETS = "test-google-sheets-connector"
+    ATTIO = "test-attio-connector"
+    SHOPIFY = "test-shopify-connector"
+    SLACK = "test-slack-connector"
+    BITBUCKET = "test-bitbucket-connector"
     GOOGLE_DOCS = "test-google-docs-connector"
-    GUMROAD = "test-gumroad-connector"
+    EVENTBRITE = "test-eventbrite-connector"
     MAILCHIMP = "test-mailchimp-connector"
-    BOX = "test-box-connector"
-    MIRO = "test-miro-connector"
-    KEAP = "test-keap-connector"
-    SPLITWISE = "test-splitwise-connector"
+    STRAVA = "test-strava-connector"
+    DROPBOX = "test-dropbox-connector"
     PAGERDUTY = "test-pagerduty-connector"
+    FIGMA = "test-figma-connector"
+    CLICKUP = "test-clickup-connector"
+    MIRO = "test-miro-connector"
+    GUMROAD = "test-gumroad-connector"
+    KLAVIYO = "test-klaviyo-connector"
+    FRESHDESK = "test-freshdesk-connector"
+    MIXPANEL = "test-mixpanel-connector"
+    INTERCOM = "test-intercom-connector"
+    STACK_EXCHANGE = "test-stack-exchange-connector"
     ZOOM = "test-zoom-connector"
-    TIMELY = "test-timely-connector"
     ZOHO = "test-zoho-connector"
-    FRESHDESK = "test-freshdesk-connector"
-    FIGMA = "test-figma-connector"
+    SPLITWISE = "test-splitwise-connector"
+    NOTION = "test-notion-connector"
+    TASKADE = "test-taskade-connector"
+    TYPEFORM = "test-typeform-connector"
     PIPEDRIVE = "test-pipedrive-connector"
-    APIFY = "test-apify-connector"
-    TWITCH = "test-twitch-connector"
-    STACK_EXCHANGE = "test-stack-exchange-connector"
-    GITHUB_OPEN_API_SPEC = "test-github_open_api_spec-connector"
-    ACCELO = "test-accelo-connector"
-    REDDIT = "test-reddit-connector"
-    SURVEY_MONKEY = "test-survey-monkey-connector"
     TWITTER = "test-twitter-connector"
-    XERO = "test-xero-connector"
-    ZOHO_INVENTORY = "test-zoho_inventory-connector"
-    ZOHO_MAIL = "test-zoho_mail-connector"
+    BOLDSIGN = "test-boldsign-connector"
+    KEAP = "test-keap-connector"
     AMAZON = "test-amazon-connector"
-    SERVICEM8 = "test-servicem8-connector"
-    SHORTCUT = "test-shortcut-connector"
+    SALESFORCE = "test-salesforce-connector"
     ZOHO_BOOKS = "test-zoho_books-connector"
-    ZOHO_INVOICE = "test-zoho_invoice-connector"
     GORGIAS = "test-gorgias-connector"
-    SALESFORCE = "test-salesforce-connector"
-    SMUGMUG = "test-smugmug-connector"
-    WAKATIME = "test-wakatime-connector"
-    ZOHO_BIGIN = "test-zoho_bigin-connector"
-    ZOHO_DESK = "test-zoho_desk-connector"
     HACKERRANK_WORK = "test-hackerrank-work-connector"
-    BOLDSIGN = "test-boldsign-connector"
-    GURU = "test-guru-connector"
-    BAMBOOHR = "test-bamboohr-connector"
-    HARVEST = "test-harvest-connector"
-    ATLASSIAN = "test-atlassian-connector"
-    DEEL = "test-deel-connector"
+    REDDIT = "test-reddit-connector"
+    SERVICEM8 = "test-servicem8-connector"
+    SHORTCUT = "test-shortcut-connector"
     FRONT = "test-front-connector"
-    GITHUB = "test-github-connector"
-    FRESHBOOKS = "test-freshbooks-connector"
+    SURVEY_MONKEY = "test-survey-monkey-connector"
+    WAKATIME = "test-wakatime-connector"
+    ZOHO_INVENTORY = "test-zoho_inventory-connector"
+    DISCORD = "test-discord-connector"
+    TWITCH = "test-twitch-connector"
+    ATLASSIAN = "test-atlassian-connector"
+    HARVEST = "test-harvest-connector"
     CALENDLY = "test-calendly-connector"
-    TRELLO = "test-trello-connector"
-    TYPEFORM = "test-typeform-connector"
     GOOGLE_CALENDAR = "test-google_calendar-connector"
+    BAMBOOHR = "test-bamboohr-connector"
+    GITHUB = "test-github-connector"
+    DEEL = "test-deel-connector"
+    GITLAB = "test-gitlab-connector"
+    HUBSPOT = "test-hubspot-connector"
+    SLACKBOT = "test-slackbot-connector"
+    YANDEX = "test-yandex-connector"
+    BRAINTREE = "test-braintree-connector"
+    ZOHO_INVOICE = "test-zoho_invoice-connector"
+    FRESHBOOKS = "test-freshbooks-connector"
+    AUTH0 = "test-auth0-connector"
+    ONE_DRIVE = "test-one-drive-connector"
+    OKTA = "test-okta-connector"
+    ZOHO_DESK = "test-zoho_desk-connector"
+    SMARTRECRUITERS = "test-smartrecruiters-connector"
+    FACEBOOK = "test-facebook-connector"
+    MURAL = "test-mural-connector"
+    WORKABLE = "test-workable-connector"
+    YOUTUBE = "test-youtube-connector"
+    ADOBE = "test-adobe-connector"
+    SQUARE = "test-square-connector"
+    ASHBY = "test-ashby-connector"
+    HIGHLEVEL = "test-highlevel-connector"
+    GOOGLE_DRIVE = "test-google-drive-connector"
+    EPIC_GAMES = "test-epic-games-connector"
+    TODOIST = "test-todoist-connector"
+    ZOHO_BIGIN = "test-zoho_bigin-connector"
+    AMPLITUDE = "test-amplitude-connector"
+    HEROKU = "test-heroku-connector"
+    SAGE = "test-sage-connector"
+    WAVE_ACCOUNTING = "test-wave-accounting-connector"
+    CLOSE = "test-close-connector"
+    PANDADOC = "test-pandadoc-connector"
+    BLACKBAUD = "test-blackbaud-connector"
+    GURU = "test-guru-connector"
+    SERPAPI = "test-serpapi-connector"
+    SMUGMUG = "test-smugmug-connector"
+    BATTLENET = "test-battlenet-connector"
+    LINKHUT = "test-linkhut-connector"
+    XERO = "test-xero-connector"
+    APIFY = "test-apify-connector"
+    LINEARSANDBOX = "test-linearsandbox-connector"
+    ZENDESK = "test-zendesk-connector"
+    ZOHO_MAIL = "test-zoho_mail-connector"
+    RING_CENTRAL = "test-ring-central-connector"
+    CODEINTERPRETER = "test-CodeInterpreter-connector"
+    GOOGLECALENDAR = "test-googlecalendar-connector"
+    ACCELO = "test-accelo-connector"
 
 class Action(Enum):
     def __init__(self, service, action):
         self.service = service
         self.action = action
 
+    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
+    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
+    TRELLO_CREATE_TRELLO_LIST = ("trello", "trello_create_trello_list")
+    TRELLO_CREATE_TRELLO_CARD = ("trello", "trello_create_trello_card")
+    TRELLO_GET_TRELLO_BOARD_CARDS = ("trello", "trello_get_trello_board_cards")
+    TRELLO_DELETE_TRELLO_CARD = ("trello", "trello_delete_trello_card")
+    TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
+    TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
+    TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
+    TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
+    TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
+    TRELLO_SEARCH_TRELLO_MEMBER = ("trello", "trello_search_trello_member")
+    TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
+    TRELLO_GET_TRELLO_MEMBER_BOARD = ("trello", "trello_get_trello_member_board")
+    LINEAR_CREATE_LINEAR_ISSUE = ("linear", "linear_create_linear_issue")
+    LINEAR_LIST_LINEAR_PROJECTS = ("linear", "linear_list_linear_projects")
+    LINEAR_LIST_LINEAR_TEAMS = ("linear", "linear_list_linear_teams")
     GMAIL_SEND_EMAIL = ("gmail", "gmail_send_email")
     GMAIL_CREATE_EMAIL_DRAFT = ("gmail", "gmail_create_email_draft")
-    GMAIL_FIND_EMAIL_ID_IN_GMAIL = ("gmail", "gmail_find_email_id")
+    GMAIL_FIND_EMAIL_ID = ("gmail", "gmail_find_email_id")
+    GMAIL_FETCH_LAST_THREE_MESSAGES = ("gmail", "gmail_fetch_last_three_messages")
     GMAIL_ADD_LABEL_TO_EMAIL = ("gmail", "gmail_add_label_to_email")
-    ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
-    ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
-    ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
-    ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
-    ZENDESK_GET_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
-    ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
-    ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
-    ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
-    ZENDESK_GET_ZENDESK_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
+    GMAIL_LIST_LABELS = ("gmail", "gmail_list_labels")
+    GMAIL_FETCH_MESSAGE_BY_THREAD_ID = ("gmail", "gmail_fetch_message_by_thread_id")
+    GMAIL_REPLY_TO_THREAD = ("gmail", "gmail_reply_to_thread")
+    GMAIL_FETCH_EMAILS_WITH_LABEL = ("gmail", "gmail_fetch_emails_with_label")
     SLACK_SEND_SLACK_MESSAGE = ("slack", "slack_send_slack_message")
-    SLACK_LIST_CHANNELS = ("slack", "slack_list_slack_channels")
-    SLACK_LIST_MEMBERS = ("slack", "slack_list_slack_members")
-    SLACK_LIST_MESSAGES = ("slack", "slack_list_slack_messages")
+    SLACK_LIST_SLACK_CHANNELS = ("slack", "slack_list_slack_channels")
+    SLACK_LIST_SLACK_MEMBERS = ("slack", "slack_list_slack_members")
+    SLACK_LIST_SLACK_MESSAGES = ("slack", "slack_list_slack_messages")
+    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
     CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
     CLICKUP_GET_TASKS = ("clickup", "clickup_get_tasks")
     CLICKUP_GET_TASK = ("clickup", "clickup_get_task")
     CLICKUP_CREATE_LIST = ("clickup", "clickup_create_list")
     CLICKUP_GET_LISTS = ("clickup", "clickup_get_lists")
     CLICKUP_GET_SPACES = ("clickup", "clickup_get_spaces")
     CLICKUP_CREATE_SPACE = ("clickup", "clickup_create_space")
     CLICKUP_CREATE_FOLDER = ("clickup", "clickup_create_folder")
     CLICKUP_GET_FOLDERS = ("clickup", "clickup_get_folders")
-    DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
-    ASANA_CREATE_SUBTASK = ("asana", "asana_create_subtask")
-    ASANA_GET_SUBTASKS = ("asana", "asana_get_subtasks")
-    LINEAR_CREATE_ISSUE = ("linear", "linear_create_linear_issue")
-    LINEAR_GET_PROJECTS = ("linear", "linear_list_linear_projects")
-    LINEAR_GET_TEAMS_BY_PROJECT = ("linear", "linear_list_linear_teams")
     NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
-    NOTION_ADD_CONTENT_NOTION_PAGE = ("notion", "notion_add_notion_page_children")
+    NOTION_ADD_NOTION_PAGE_CHILDREN = ("notion", "notion_add_notion_page_children")
     NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
     NOTION_CREATE_NOTION_DATABASE = ("notion", "notion_create_notion_database")
     NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
     NOTION_CREATE_NOTION_PAGE = ("notion", "notion_create_notion_page")
-    NOTION_DELETE_BLOCKS = ("notion", "notion_delete_notion_page_children")
-    NOTION_FETCH_ALL_UNRESOLVED_COMMENTS = ("notion", "notion_fetch_notion_comment")
+    NOTION_DELETE_NOTION_PAGE_CHILDREN = ("notion", "notion_delete_notion_page_children")
+    NOTION_FETCH_NOTION_COMMENT = ("notion", "notion_fetch_notion_comment")
     NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
     NOTION_FETCH_NOTION_PAGE = ("notion", "notion_fetch_notion_page")
-    NOTION_SEARCH_LIST_NOTION_PAGE = ("notion", "notion_search_notion_page")
+    NOTION_SEARCH_NOTION_PAGE = ("notion", "notion_search_notion_page")
     NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
-    NOTION_FETCH_NOTION_BLOCKS = ("notion", "notion_fetch_notion_block")
-    NOTION_FETCH_NOTION_BLOCK_CHILDREN = ("notion", "notion_fetch_notion_child_block")
-    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
-    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
-    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
-    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
-    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
-    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
+    NOTION_FETCH_NOTION_BLOCK = ("notion", "notion_fetch_notion_block")
+    NOTION_FETCH_NOTION_CHILD_BLOCK = ("notion", "notion_fetch_notion_child_block")
+    TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
     GITHUB_CREATE_ISSUE = ("github", "github_create_issue")
-    GITHUB_GET_REPOSITORY = ("github", "github_list_github_repos")
+    GITHUB_LIST_GITHUB_REPOS = ("github", "github_list_github_repos")
     GITHUB_STAR_REPO = ("github", "github_star_repo")
     GITHUB_GET_ABOUT_ME = ("github", "github_get_about_me")
     GITHUB_FETCH_README = ("github", "github_fetch_readme")
     GITHUB_GET_COMMITS = ("github", "github_get_commits")
-    GITHUB_GET_COMMITS_WITH_PATCH_FILE_FOR_THAT_COMMIT = ("github", "github_get_commits_with_code")
+    GITHUB_GET_COMMITS_WITH_CODE = ("github", "github_get_commits_with_code")
     GITHUB_GET_PATCH_FOR_COMMIT = ("github", "github_get_patch_for_commit")
-    TRELLO_CREATE_TRELLO_LIST = ("trello", "trello_create_trello_list")
-    TRELLO_CREATE_TRELLO_CARD = ("trello", "trello_create_trello_card")
-    TRELLO_GET_TRELLO_BOARD_CARDS = ("trello", "trello_get_trello_board_cards")
-    TRELLO_DELETE_TRELLO_CARD = ("trello", "trello_delete_trello_card")
-    TRELLO_ADD_TRELLO_CARD_COMMENT = ("trello", "trello_add_trello_card_comment")
-    TRELLO_CREATE_TRELLO_LABEL = ("trello", "trello_create_trello_label")
-    TRELLO_UPDATE_TRELLO_BOARD = ("trello", "trello_update_trello_board")
-    TRELLO_GET_ABOUT_ME = ("trello", "trello_get_about_me")
-    TRELLO_SEARCH_TRELLO = ("trello", "trello_search_trello")
-    TRELLO_SEARCH_TRELLO_MEMBERS = ("trello", "trello_search_trello_member")
-    TRELLO_UPDATE_TRELLO_CARD = ("trello", "trello_update_trello_card")
-    TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
+    SLACKBOT_SEND_SLACK_MESSAGE = ("slackbot", "slackbot_send_slack_message")
+    SLACKBOT_LIST_SLACK_CHANNELS = ("slackbot", "slackbot_list_slack_channels")
+    SLACKBOT_LIST_SLACK_MEMBERS = ("slackbot", "slackbot_list_slack_members")
+    SLACKBOT_LIST_SLACK_MESSAGES = ("slackbot", "slackbot_list_slack_messages")
+    SERPAPI_SEARCH = ("serpapi", "serpapi_search")
+    APIFY_LIST_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
+    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
+    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
+    APIFY_SEARCH_STORE = ("apify", "apify_search_store")
+    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
+    APIFY_LIST_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
+    ZENDESK_CREATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_create_zendesk_organization")
+    ZENDESK_DELETE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_delete_zendesk_organization")
+    ZENDESK_COUNT_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_count_zendesk_organizations")
+    ZENDESK_GET_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_get_zendesk_organization")
+    ZENDESK_GET_ALL_ZENDESK_ORGANIZATIONS = ("zendesk", "zendesk_get_all_zendesk_organizations")
+    ZENDESK_UPDATE_ZENDESK_ORGANIZATION = ("zendesk", "zendesk_update_zendesk_organization")
+    ZENDESK_CREATE_ZENDESK_TICKET = ("zendesk", "zendesk_create_zendesk_ticket")
+    ZENDESK_DELETE_ZENDESK_TICKET = ("zendesk", "zendesk_delete_zendesk_ticket")
+    ZENDESK_GET_ABOUT_ME = ("zendesk", "zendesk_get_about_me")
+    GOOGLECALENDAR_CREATE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_create_google_event")
+    GOOGLECALENDAR_REMOVE_ATTENDEE = ("googlecalendar", "googlecalendar_remove_attendee")
+    GOOGLECALENDAR_FIND_EVENT = ("googlecalendar", "googlecalendar_find_event")
+    GOOGLECALENDAR_CHECK_ATTENDEES = ("googlecalendar", "googlecalendar_check_attendees")
+    GOOGLECALENDAR_DELETE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_delete_google_event")
+    GOOGLECALENDAR_UPDATE_GOOGLE_EVENT = ("googlecalendar", "googlecalendar_update_google_event")
 
 class Trigger(Enum):
     def __init__(self, service, trigger):
         self.service = service
         self.trigger = trigger
 
     SLACK_NEW_MESSAGE = ("slack", "slack_receive_message")
     GITHUB_PULL_REQUEST_EVENT = ("github", "github_pull_request_event")
     GITHUB_COMMIT_EVENT = ("github", "github_commit_event")
+    SLACKBOT_NEW_MESSAGE = ("slackbot", "slackbot_receive_message")
```

### Comparing `composio_core-0.1.88/composio/sdk/sdk.py` & `composio_core-0.1.89/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.88/composio/sdk/storage.py` & `composio_core-0.1.89/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.88/composio/sdk/utils.py` & `composio_core-0.1.89/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.88/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.89/composio_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.88
+Version: 0.1.89
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.88/pyproject.toml` & `composio_core-0.1.89/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.88/setup.py` & `composio_core-0.1.89/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """Customized setuptools install command."""
 
     def run(self):
         install.run(self)
 
 setup(
     name="composio_core",
-    version="0.1.88",
+    version="0.1.89",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

