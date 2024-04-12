# Comparing `tmp/auterion-cli-1.6.2.tar.gz` & `tmp/auterion-cli-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.6.2.tar", last modified: Tue Feb  6 13:58:27 2024, max compression
+gzip compressed data, was "auterion-cli-1.7.0.tar", last modified: Fri Apr 12 09:33:54 2024, max compression
```

## Comparing `auterion-cli-1.6.2.tar` & `auterion-cli-1.7.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 13:58:25.000000 auterion-cli-1.6.2/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 13:58:27.000000 auterion-cli-1.6.2/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-06 13:58:10.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-02-06 13:58:10.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-02-06 13:58:10.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-3.json
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-06 13:58:10.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-02-06 13:58:10.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_inspect_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9321 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4403 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 13:58:27.433822 auterion-cli-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-02-06 13:58:09.000000 auterion-cli-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 09:33:53.000000 auterion-cli-1.7.0/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.624145 auterion-cli-1.7.0/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 09:33:54.000000 auterion-cli-1.7.0/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.624145 auterion-cli-1.7.0/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26516 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19739 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_inspect_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9751 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7789 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4407 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:33:54.628145 auterion-cli-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-12 09:33:42.000000 auterion-cli-1.7.0/setup.py
```

### Comparing `auterion-cli-1.6.2/README.md` & `auterion-cli-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.7.0/auterion_cli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 auterioncli/commands/app_sdk/app_inspect_command.py
 auterioncli/commands/app_sdk/app_install_command.py
 auterioncli/commands/app_sdk/environment.py
 auterioncli/commands/app_sdk/slimify.py
 auterioncli/commands/app_sdk/update.py
 auterioncli/commands/app_sdk/app-yml-spec/api-1.json
 auterioncli/commands/app_sdk/app-yml-spec/api-2.json
-auterioncli/commands/app_sdk/app-yml-spec/api-3.json
+auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json
 auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
 auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_command.py` & `auterion-cli-1.7.0/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-1.json` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-1.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-2.json` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-2.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/api-3.json` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/api-3-4.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998312662212401%*

 * *Differences: {"'definitions'": "{'AuterionAppYml': {'properties': {'auterion-api-version': {'enum': [3, 4], "*

 * *                  "delete: ['const']}}}, 'AuterionAppYmlLoggingSubscriptions': "*

 * *                  "{'patternProperties': {'^.*$': {'anyOf': {0: {'pattern': "*

 * *                  '\'^[a-zA-Z0-9_]+/[a-zA-Z0-9_]+$\', \'description\': "Message Type, e.g. '*

 * *                  '\'geometry_msgs/Point\'"}, 1: {\'properties\': {\'type\': {\'pattern\': '*

 * *                  '\'^[a-zA-Z0-9_]+/[a-zA-Z0-9_]+$\', \'description\': […]*

```diff
@@ -13,15 +13,18 @@
                     "pattern": "^[a-z0-9-_]+$",
                     "type": "string"
                 },
                 "app-version": {
                     "type": "string"
                 },
                 "auterion-api-version": {
-                    "const": 3,
+                    "enum": [
+                        3,
+                        4
+                    ],
                     "type": "integer"
                 },
                 "auterion-app-base": {
                     "pattern": "^v\\d+|none$",
                     "type": "string"
                 },
                 "compose-override": {
@@ -133,27 +136,31 @@
             "type": "object"
         },
         "AuterionAppYmlLoggingSubscriptions": {
             "patternProperties": {
                 "^.*$": {
                     "anyOf": [
                         {
+                            "description": "Message Type, e.g. 'geometry_msgs/Point'",
+                            "pattern": "^[a-zA-Z0-9_]+/[a-zA-Z0-9_]+$",
                             "type": "string"
                         },
                         {
                             "additionalProperties": false,
                             "properties": {
                                 "dds_name_prefix": {
                                     "default": "rt",
                                     "type": "string"
                                 },
                                 "max_rate_hz": {
                                     "type": "number"
                                 },
                                 "type": {
+                                    "description": "Message Type, e.g. 'geometry_msgs/Point'",
+                                    "pattern": "^[a-zA-Z0-9_]+/[a-zA-Z0-9_]+$",
                                     "type": "string"
                                 }
                             },
                             "required": [
                                 "type"
                             ],
                             "type": "object"
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9854166666666668%*

 * *Differences: {"'allOf'": "{2: {'if': {'properties': {'auterion-api-version': {replace: OrderedDict([('enum', "*

 * *            "[3, 4])])}}}, 'then': {'$ref': 'api-3-4.json'}}}",*

 * * "'properties'": "{'auterion-api-version': {'maximum': 4}}"}*

```diff
@@ -25,26 +25,29 @@
                 "$ref": "api-2.json"
             }
         },
         {
             "if": {
                 "properties": {
                     "auterion-api-version": {
-                        "const": 3
+                        "enum": [
+                            3,
+                            4
+                        ]
                     }
                 }
             },
             "then": {
-                "$ref": "api-3.json"
+                "$ref": "api-3-4.json"
             }
         }
     ],
     "properties": {
         "auterion-api-version": {
-            "maximum": 3,
+            "maximum": 4,
             "minimum": 1,
             "type": "integer"
         }
     },
     "required": [
         "auterion-api-version"
     ],
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,16 +155,16 @@
         target_platforms = [PLATFORM_ALIAS.get(d, d) for d in target_devices]
         if len(set(target_platforms)) > 1:
             error('Targets have multiple architectures. Aborting.')
         return target_platforms[0]
 
     def _compose_for_building_from_meta(self, meta):
         api_version = meta['auterion-api-version']
-        assert 0 <= api_version <= 3, f'Auterion API version {api_version} is not supported by this ' \
-                                      f'version of auterion-cli. Supported API versions are 0 to 3.'
+        assert 0 <= api_version <= 4, f'Auterion API version {api_version} is not supported by this ' \
+                                      f'version of auterion-cli. Supported API versions are 0 to 4.'
 
         compose = {}
         if api_version == 0:
             compose = {
                 'version': '3.7',
                 **meta['compose']
             }
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/app_inspect_command.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/app_inspect_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
     code, result = try_command(['docker', 'run', '--rm', '--platform=linux/arm64', ARM64_TEST_IMAGE,
                                 'uname', '-m'])
     if code != 0 or ('aarch64' not in result and 'arm64' not in result):
         error('Docker cannot run arm64 containers. \n'
               'Make sure you have docker installed and configured to run arm64 containers.\n'
               'You can check this by running \'docker run --rm --platform=linux/arm64 ubuntu:latest uname -m\'\n'
-              'For docker setup instructions find more information on  https://docs.auterion.com/developers/')
+              'For docker setup instructions find more information on  https://docs.auterion.com/app-development/resources/auterion-cli')
     print('.. Docker can run arm64 containers')
 
     return compose_cmd
 
 
 MENDER_CI_TOOLS_TAG = 'mendersoftware/mender-ci-tools:1.0.0'
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/slimify.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.7.0/auterioncli/commands/app_sdk/update.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         else:
             if response.status_code == 504:  # initial request timed out
                 return True, "Installation taking longer, switching to polling.."
             try:
                 data = response.json()
                 if "logs" in data:
                     print("Error logs:", file=sys.stderr)
-                    for line in data['logs'].split('\n'):
+                    for line in data['logs'].replace("\\n", "\n").split('\n'):
                         print(' |  ' + line, file=sys.stderr)
                 message = "Failed to install"
                 if "message" in data:
                     message = data['message']
             except:
                 message = "Failed to install. Response code: {}".format(response.status_code)
             return False, message
@@ -109,18 +109,23 @@
             return False
     return False
 
 def get_device_status(url, reboot_counter=0, last_status=None):
     status = None
     try:
         response = requests.get("{}/status".format(url), timeout=1)
-        if response and "status" in response.json():
-            status = response.json()["status"]
-        elif response.status_code == 404:
+
+        if response.status_code == 404:
             return False, ExitCode.REQUEST_API_VERSION, None, reboot_counter
+
+        # In local-updater PR #77, the status of the update was moved from the status field to the status_key field.
+        # This change was required to ensure compatibility with task-monitor's status schema.
+        # The following line extract the status in a manner that is compatible with both versions of local-updater.
+        # Order is important, as the newer version uses the status field for a different purpose.
+        status = response.json().get("status_key") or response.json().get("status")
     except:
         if reboot_counter > 5:
             status = "REBOOTING"
         else:
             status = last_status
             reboot_counter += 1
     # if status == "UPLOADING":
```

### Comparing `auterion-cli-1.6.2/auterioncli/commands/container_command.py` & `auterion-cli-1.7.0/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/device_command.py` & `auterion-cli-1.7.0/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/info_command.py` & `auterion-cli-1.7.0/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/report_command.py` & `auterion-cli-1.7.0/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/commands/utils.py` & `auterion-cli-1.7.0/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/auterioncli/main.py` & `auterion-cli-1.7.0/auterioncli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         device_present, serial_at_address = get_device_presence(config['device_address'])
         if not device_present:
             eprint(f"Error: No device reachable at {config['device_address']}.\n"
                    f"       Use 'device discover' command to show available devices.\n"
                    f"Aborting.\n")
             exit(1)
         elif not config['have_selected_device']:
-            if config['this_device_type'].startswith('auterion'):
+            if not config['this_device_type'].startswith('auterion'):
                 eprint(f'Warn: No device serial selected.\n'
                       f'      Use \'device discover\' and \'device select\' commands to specify which device to use.\n'
                       f'      Falling back to device with serial {serial_at_address} on {config["device_address"]}\n')
 
         elif serial_at_address != config['device_serial']:
             if serial_at_address == '':
                 eprint(f"Warn: Could not verify serial number of device at address {config['device_address']}.\n"
```

### Comparing `auterion-cli-1.6.2/auterioncli/meta_util.py` & `auterion-cli-1.7.0/auterioncli/meta_util.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.6.2/setup.py` & `auterion-cli-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     git_version = git_version.replace('-', '.dev', 1).replace('-', '+', 1)
     return git_version
 
 
 setup(name='auterion-cli',
       version=get_version(),
       description='CLI tool to interact with AuterionOS devices and apps',
-      url='https://docs.auterion.com/developers',
+      url='https://docs.auterion.com/app-development/resources/auterion-cli',
       author='Auterion',
       author_email='support@auterion.com',
       license='proprietary',
       packages=find_packages(),
       install_requires=[
           'tabulate',
           'requests',
```

