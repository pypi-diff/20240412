# Comparing `tmp/iam_actions-1.2.20240410.tar.gz` & `tmp/iam_actions-1.2.20240411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240410.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240411.tar", max compression
```

## Comparing `iam_actions-1.2.20240410.tar` & `iam_actions-1.2.20240411.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/README.md
--rw-r--r--   0        0        0      228 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/__init__.py
--rw-r--r--   0        0        0  4785181 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-10 02:15:55.173645 iam_actions-1.2.20240410/iam_actions/generate/services.py
--rw-r--r--   0        0        0   622141 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/policies.json
--rw-r--r--   0        0        0   207247 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   603579 2024-04-10 02:17:05.526347 iam_actions-1.2.20240410/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-10 02:17:06.182354 iam_actions-1.2.20240410/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240410/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240410/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/README.md
+-rw-r--r--   0        0        0      228 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4785599 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-11 02:17:43.686671 iam_actions-1.2.20240411/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   622194 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/policies.json
+-rw-r--r--   0        0        0   207247 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   603630 2024-04-11 02:19:34.302694 iam_actions-1.2.20240411/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-11 02:19:34.982694 iam_actions-1.2.20240411/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240411/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240411/PKG-INFO
```

### Comparing `iam_actions-1.2.20240410/LICENSE` & `iam_actions-1.2.20240411/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/README.md` & `iam_actions-1.2.20240411/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/actions.json` & `iam_actions-1.2.20240411/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998900566487776%*

 * *Differences: {"'scn'": "{'SendDataIntegrationEvent': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *          "'SendDataIntegrationEvent'), ('condition_keys', []), ('description', 'Not Documented by "*

 * *          "AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'wisdom'": "{'UpdateSession': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *             "'UpdateSession'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *             "('orphan', False), ('resources', [])])}"}*

```diff
@@ -144576,14 +144576,22 @@
             "access_level": "Undocumented",
             "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "SendDataIntegrationEvent": {
+            "access_level": "Undocumented",
+            "action": "SendDataIntegrationEvent",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "TagResource": {
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -167865,14 +167873,22 @@
         "UpdateQuickResponse": {
             "access_level": "Undocumented",
             "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "UpdateSession": {
+            "access_level": "Undocumented",
+            "action": "UpdateSession",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "workdocs": {
         "AbortDocumentVersionUpload": {
             "access_level": "Write",
             "action": "AbortDocumentVersionUpload",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240411/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240411/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/generate.py` & `iam_actions-1.2.20240411/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240411/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240411/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/generate/services.py` & `iam_actions-1.2.20240411/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/policies.json` & `iam_actions-1.2.20240411/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999991242257561%*

 * *Differences: {"'serviceMap'": "{'AWS Supply Chain': {'Actions': {insert: [(12, 'SendDataIntegrationEvent')]}}, "*

 * *                 "'Amazon Q in Connect': {'Actions': {insert: [(42, 'UpdateSession')]}}}"}*

```diff
@@ -9747,14 +9747,15 @@
                 "DeleteSSOApplication",
                 "DescribeInstance",
                 "GetBillOfMaterialsImportJob",
                 "ListAdminUsers",
                 "ListInstances",
                 "ListTagsForResource",
                 "RemoveAdminPermissionsForUser",
+                "SendDataIntegrationEvent",
                 "TagResource",
                 "UntagResource",
                 "UpdateInstance"
             ],
             "HasResource": true,
             "StringPrefix": "scn",
             "conditionKeys": [
@@ -18850,15 +18851,16 @@
                 "SearchSessions",
                 "StartContentUpload",
                 "StartImportJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateContent",
                 "UpdateKnowledgeBaseTemplateUri",
-                "UpdateQuickResponse"
+                "UpdateQuickResponse",
+                "UpdateSession"
             ],
             "HasResource": true,
             "StringPrefix": "wisdom",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
```

### Comparing `iam_actions-1.2.20240410/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240411/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240410/iam_actions/services.json` & `iam_actions-1.2.20240411/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999908380540649%*

 * *Differences: {"'scn'": "{'Actions': {insert: [(12, 'SendDataIntegrationEvent')]}}",*

 * * "'wisdom'": "{'Actions': {insert: [(42, 'UpdateSession')]}}"}*

```diff
@@ -20119,14 +20119,15 @@
             "DeleteSSOApplication",
             "DescribeInstance",
             "GetBillOfMaterialsImportJob",
             "ListAdminUsers",
             "ListInstances",
             "ListTagsForResource",
             "RemoveAdminPermissionsForUser",
+            "SendDataIntegrationEvent",
             "TagResource",
             "UntagResource",
             "UpdateInstance"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
@@ -23683,15 +23684,16 @@
             "SearchSessions",
             "StartContentUpload",
             "StartImportJob",
             "TagResource",
             "UntagResource",
             "UpdateContent",
             "UpdateKnowledgeBaseTemplateUri",
-            "UpdateQuickResponse"
+            "UpdateQuickResponse",
+            "UpdateSession"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "wisdom:SearchFilter/RoutingProfileArn"
         ],
```

### Comparing `iam_actions-1.2.20240410/pyproject.toml` & `iam_actions-1.2.20240411/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240410"
+version = "1.2.20240411"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240410/setup.py` & `iam_actions-1.2.20240411/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240410',
+    'version': '1.2.20240411',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240410/PKG-INFO` & `iam_actions-1.2.20240411/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240410
+Version: 1.2.20240411
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

