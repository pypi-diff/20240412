# Comparing `tmp/ops-py-azure-key-vault-alert-4.3.0.tar.gz` & `tmp/ops-py-azure-key-vault-alert-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-py-azure-key-vault-alert-4.3.0.tar", last modified: Thu Apr 11 12:58:32 2024, max compression
+gzip compressed data, was "ops-py-azure-key-vault-alert-4.4.0.tar", last modified: Fri Apr 12 09:05:46 2024, max compression
```

## Comparing `ops-py-azure-key-vault-alert-4.3.0.tar` & `ops-py-azure-key-vault-alert-4.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.057566 ops-py-azure-key-vault-alert-4.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6387 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/azure_key_vault_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7486 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/slack_alert.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/teams_alert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:58:32.053566 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 12:58:32.000000 ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-11 12:58:21.000000 ops-py-azure-key-vault-alert-4.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:58:32.057566 ops-py-azure-key-vault-alert-4.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 12:58:29.000000 ops-py-azure-key-vault-alert-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:46.145963 ops-py-azure-key-vault-alert-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 09:05:44.000000 ops-py-azure-key-vault-alert-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-12 09:05:46.141963 ops-py-azure-key-vault-alert-4.4.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:46.137963 ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2024-04-12 09:05:41.000000 ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7121 2024-04-12 09:05:41.000000 ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/azure_key_vault_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7486 2024-04-12 09:05:41.000000 ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/slack_alert.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2196 2024-04-12 09:05:41.000000 ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/teams_alert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:05:46.141963 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-12 09:05:46.000000 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-12 09:05:46.000000 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:05:46.000000 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 09:05:46.000000 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-12 09:05:46.000000 ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-12 09:05:44.000000 ops-py-azure-key-vault-alert-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-12 09:05:44.000000 ops-py-azure-key-vault-alert-4.4.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 09:05:41.000000 ops-py-azure-key-vault-alert-4.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:05:46.145963 ops-py-azure-key-vault-alert-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 09:05:44.000000 ops-py-azure-key-vault-alert-4.4.0/setup.py
```

### Comparing `ops-py-azure-key-vault-alert-4.3.0/LICENSE` & `ops-py-azure-key-vault-alert-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.3.0/PKG-INFO` & `ops-py-azure-key-vault-alert-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.3.0
+Version: 4.4.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/azure_key_vault_alert.py` & `ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/azure_key_vault_alert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 
 import os
 import logging
 import argparse
+import json
 from azure_key_vault_report import azure_key_vault_report
 from azure_key_vault_report import az_cmd
 from message_handler import message_handler
 from .slack_alert import slack_alert
 from .teams_alert import teams_alert
 
 ########################################################################################################################
@@ -44,24 +45,28 @@
 
     parser.add_argument("-C", "--teams_max_chars", type=int, default=17367,
                         help="The max characters the report can have due to the MS Teams payload size limits")
 
     parser.add_argument("-S", "--stdout_only", action='store_true',
                         help="Only print report to stdout. No post to messagehandler (Slack or MS Teams")
 
+    parser.add_argument("-w", "--workflow_output_file", type=str, default="output.json",
+                        help="The file where the full json report will be written.")
+
     args = parser.parse_args()
     vaults = args.vaults
     expire_threshold = args.expire_threshold
     include_all = args.include_all
     ignore_no_expiration = args.include_no_expiration
     title = args.title
     record_types = args.record_types
     slack_split_chars = args.slack_split_chars
     teams_max_chars = args.teams_max_chars
     stdout_only = args.stdout_only
+    workflow_output_file = args.workflow_output_file
 
     for k, v in sorted(vars(args).items()):
         logging.info(f"Argument '{k}': '{v}'")
 
     if not vaults:
         logging.error("No vaults specified.")
         exit(2)
@@ -118,31 +123,41 @@
         alert = message_handler.MessageHandler(WEBHOOK_NOTIFY)
         alert.post_payload()
 
     # Get the full report which will be logged for future references.
     # Azure resource information are added.
     report_full = kv_report.get_report_full()
     if isinstance(report_full, dict):
+        workflow_output_name = str(WORKFLOW_OUTPUT_NAME).strip().lower().replace(" ", "_")[:40]
+        report_full["name"] = workflow_output_name
         report_full["client_id"] = AZURE_CLIENT_ID
         report_full["subscription_id"] = AZURE_SUBSCRIPTION_ID
         report_full["tenant_id"] = AZURE_TENANT_ID
 
-        # Temporarily print to stdout, but will be pushed to db
-        print(report_full)
+        # Write full report as json to file
+        if not isinstance(workflow_output_file, str):
+            workflow_output_file = "output.json"
+
+        with open(workflow_output_file, 'w') as f:
+            json.dump(report_full, f)
 
 ########################################################################################################################
 
 
 if __name__ == '__main__':
     # The actual report will be posted to the webhook exported in
     # the following environment variable
     WEBHOOK_REPORT = os.getenv("WEBHOOK_REPORT")
 
     # When all the reports have been posted, an additional POST is performed
     # to the webhook exported in following environment variable:
     WEBHOOK_NOTIFY = os.getenv("WEBHOOK_NOTIFY")
 
+    # These Azure environment variables will be used in the full json logfile
     AZURE_CLIENT_ID = os.getenv("AZURE_CLIENT_ID")
     AZURE_SUBSCRIPTION_ID = os.getenv("AZURE_SUBSCRIPTION_ID")
     AZURE_TENANT_ID = os.getenv("AZURE_TENANT_ID")
 
+    # The value of the name key in the full json logfile
+    WORKFLOW_OUTPUT_NAME = os.getenv("WORKFLOW_OUTPUT_NAME", "")
+
     main()
```

### Comparing `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/slack_alert.py` & `ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/slack_alert.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.3.0/azure_key_vault_alert/teams_alert.py` & `ops-py-azure-key-vault-alert-4.4.0/azure_key_vault_alert/teams_alert.py`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO` & `ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-alert
-Version: 4.3.0
+Version: 4.4.0
 Summary: Post Key Vault Secrets report to webhook
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `ops-py-azure-key-vault-alert-4.3.0/ops_py_azure_key_vault_alert.egg-info/requires.txt` & `ops-py-azure-key-vault-alert-4.4.0/ops_py_azure_key_vault_alert.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.3.0/readme.md` & `ops-py-azure-key-vault-alert-4.4.0/readme.md`

 * *Files identical despite different names*

### Comparing `ops-py-azure-key-vault-alert-4.3.0/requirements.txt` & `ops-py-azure-key-vault-alert-4.4.0/requirements.txt`

 * *Files identical despite different names*

