# Comparing `tmp/ado_wrapper-0.0.5.tar.gz` & `tmp/ado_wrapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-0.0.5.tar", max compression
+gzip compressed data, was "ado_wrapper-0.0.6.tar", max compression
```

## Comparing `ado_wrapper-0.0.5.tar` & `ado_wrapper-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.5/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.5/README.md
--rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.5/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6446 2024-04-08 17:57:20.745729 ado_wrapper-0.0.5/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2123 2024-04-09 20:35:21.978850 ado_wrapper-0.0.5/ado_wrapper/client.py
--rw-r--r--   0        0        0    17177 2024-04-08 17:58:36.801350 ado_wrapper-0.0.5/ado_wrapper/dumps.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.5/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.5/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.5/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1805 2024-04-09 15:28:42.531252 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0     1497 2024-04-09 20:33:02.558531 ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.5/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.5/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.5/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.5/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.5/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.5/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.5/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.5/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0     9135 2024-04-09 18:30:44.069270 ado_wrapper-0.0.5/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     6093 2024-04-09 18:53:39.689874 ado_wrapper-0.0.5/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.5/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8370 2024-04-09 18:46:26.714212 ado_wrapper-0.0.5/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.5/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     8415 2024-04-09 18:32:40.182058 ado_wrapper-0.0.5/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8347 2024-04-09 20:34:04.740783 ado_wrapper-0.0.5/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.5/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2098 2024-04-09 09:42:33.352412 ado_wrapper-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-0.0.6/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-0.0.6/README.md
+-rw-r--r--   0        0        0      118 2024-04-05 11:26:35.608768 ado_wrapper-0.0.6/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6446 2024-04-08 17:57:20.745729 ado_wrapper-0.0.6/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2123 2024-04-10 11:16:39.930064 ado_wrapper-0.0.6/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25667 2024-04-11 13:43:04.075027 ado_wrapper-0.0.6/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-0.0.6/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-0.0.6/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      295 2024-04-05 11:26:35.657464 ado_wrapper-0.0.6/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1039 2024-04-09 15:28:42.529947 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1805 2024-04-09 15:28:42.531252 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0     1342 2024-04-10 19:18:54.311903 ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0      659 2024-04-08 18:01:44.152197 ado_wrapper-0.0.6/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     4650 2024-04-09 09:35:29.826115 ado_wrapper-0.0.6/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    13517 2024-04-09 20:21:18.486611 ado_wrapper-0.0.6/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6637 2024-04-09 18:43:12.632598 ado_wrapper-0.0.6/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     3477 2024-04-09 18:30:16.745942 ado_wrapper-0.0.6/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0     2145 2024-04-09 18:43:06.211713 ado_wrapper-0.0.6/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14800 2024-04-09 18:53:28.574098 ado_wrapper-0.0.6/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12781 2024-04-09 20:19:59.831154 ado_wrapper-0.0.6/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    15647 2024-04-12 10:04:22.381132 ado_wrapper-0.0.6/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0     6014 2024-04-10 18:05:31.126571 ado_wrapper-0.0.6/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4622 2024-04-09 18:43:22.061540 ado_wrapper-0.0.6/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8370 2024-04-11 10:38:27.069961 ado_wrapper-0.0.6/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4934 2024-04-09 18:30:55.561929 ado_wrapper-0.0.6/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     8415 2024-04-10 18:17:52.653711 ado_wrapper-0.0.6/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8158 2024-04-10 17:53:40.392730 ado_wrapper-0.0.6/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4257 2024-04-08 17:51:22.897215 ado_wrapper-0.0.6/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2098 2024-04-12 10:04:57.932187 ado_wrapper-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-0.0.6/PKG-INFO
```

### Comparing `ado_wrapper-0.0.5/LICENSE` & `ado_wrapper-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/README.md` & `ado_wrapper-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/__main__.py` & `ado_wrapper-0.0.6/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/client.py` & `ado_wrapper-0.0.6/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/dumps.py` & `ado_wrapper-0.0.6/ado_wrapper/dumps.py`

 * *Files 23% similar despite different names*

```diff
@@ -150,14 +150,29 @@
     "remoteUrl": "https://{ado_client.org}@dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}",
     "sshUrl": "git@ssh.dev.azure.com:v3/{ado_client.org}/{ado_client.project}/{repo_name}",
     "webUrl": "https://dev.azure.com/{ado_client.org}/{ado_client.project}/_git/{repo_name}",
     "isDisabled": False,
     "isInMaintenance": False,
 }
 
+REPO_POLICY_DUMP = {
+    'dataProviderSharedData': {},
+    'dataProviders': {
+        'ms.vss-web.component-data': {}, 'ms.vss-web.shared-data': None, 'ms.vss-code-web.branch-policies-data-provider': {
+            'identities': "<Member>", 'supportServicePrincipals': True, 'isEditable': True, 'buildDefinitions': None, 'recentStatuses': None,
+            'policyGroups': {'{policy_id_uuid}': {
+                             'currentScopePolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1712832031819)/',
+                                                       'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'minimumApproverCount': 1, 'creatorVoteCounts': False, 'allowDownvotes': False, 'resetOnSourcePush': False, 'requireVoteOnLastIteration': False, 'resetRejectionsOnSourcePush': False, 'blockLastPusherVote': True, 'requireVoteOnEachIteration': False, 'scope': [{'refName': 'refs/heads/main', 'matchKind': 'Exact', 'repositoryId': '{repo_id}'}]}, 'isEnterpriseManaged': False, '_links': "<links>", 'revision': 13, 'id': 8178, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8178', 'type': {'id': '{policy_id_uuid}', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}', 'displayName': 'Minimum number of reviewers'}}], 'enterpriseManagedPolicies': None, 
+                                                       'inheritedPolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1710074353140)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'minimumApproverCount': 1, 'creatorVoteCounts': False, 'allowDownvotes': False, 'resetOnSourcePush': False, 'requireVoteOnLastIteration': False, 'resetRejectionsOnSourcePush': False, 'blockLastPusherVote': False, 'requireVoteOnEachIteration': False, 'scope': [{'refName': None, 'matchKind': 'DefaultBranch', 'repositoryId': None}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/{config_id}'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}'}}, 'revision': 2, 'id': "{config_id}", 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/{config_id}', 'type': {'id': '{policy_id_uuid}', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/{policy_id_uuid}', 'displayName': 'Minimum number of reviewers'}}]}, 'c6a1889d-b943-4856-b76f-9e46bb6b0df2': {'currentScopePolicies': None, 'enterpriseManagedPolicies': None,
+                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          'inheritedPolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1670239096642)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'scope': [{'refName': None, 'matchKind': 'DefaultBranch', 'repositoryId': None}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2'}}, 'revision': 1, 'id': 40, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/40', 'type': {'id': 'c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/c6a1889d-b943-4856-b76f-9e46bb6b0df2', 'displayName': 'Comment requirements'}}]},
+                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          'fd2167ab-b0be-447a-8ec8-39368250530e': {'currentScopePolicies': [{'createdBy': "<Member>", 'createdDate': '/Date(1712766957032)/', 'isEnabled': True, 'isBlocking': True, 'isDeleted': False, 'settings': {'requiredReviewerIds': ['ab35e0e5-b36d-46c4-8d91-714d413e4fae'], 'minimumApproverCount': 1, 'creatorVoteCounts': True, 'scope': [{'refName': 'refs/heads/main', 'matchKind': 'Exact', 'repositoryId': '1aa43e9c-ffca-4388-98b5-59b272a497b8'}]}, 'isEnterpriseManaged': False, '_links': {'self': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179'}, 'policyType': {'href': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e'}}, 'revision': 1, 'id': 8179, 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/configurations/8179', 'type': {'id': 'fd2167ab-b0be-447a-8ec8-39368250530e', 'url': 'https://dev.azure.com/{ado_org}/{repo_id}/_apis/policy/types/fd2167ab-b0be-447a-8ec8-39368250530e', 'displayName': 'Required reviewers'}}],
+                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   'enterpriseManagedPolicies': None, 'inheritedPolicies': None}},
+        }},
+}
+
 SERVICE_ENDPOINT_DUMP = {
     "data": {},
     "id": "{service_endpoint_id}",
     "name": "{service_connection_name}",
     "type": "github",
     "url": "https://github.com",
     "createdBy": "<Member>",
```

### Comparing `ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-0.0.6/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from typing import Any, TypedDict, TYPE_CHECKING
+from typing import Any, TypedDict
 import json
 import re
 
 from ado_wrapper.utils import ResourceType
 from ado_wrapper.state_manager import StateManager
-from ado_wrapper.plan_resources.mapping import get_resource_variables_plans
 from ado_wrapper.plan_resources.colours import ACTIONS
 
-if TYPE_CHECKING:
-    from ado_wrapper.client import AdoClient
-
 STATE_FILE_VERSION = "1.4"
 
 
 class StateFileType(TypedDict):
     state_file_version: str
     resources: dict[ResourceType, dict[str, Any]]
```

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/__init__.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/branches.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/builds.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/commits.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/groups.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/projects.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/releases.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/repo.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/users.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,192 @@
 from __future__ import annotations
 
-import io
-import zipfile
+from typing import Literal, Any, TYPE_CHECKING
 from dataclasses import dataclass, field
-from typing import Any, Literal, TYPE_CHECKING
-
-import requests
 
 from ado_wrapper.state_managed_abc import StateManagedResource
-from ado_wrapper.resources.pull_requests import PullRequest, PullRequestStatus
-from ado_wrapper.resources.commits import Commit
-from ado_wrapper.utils import ResourceNotFound, UnknownError
 
 if TYPE_CHECKING:
     from ado_wrapper.client import AdoClient
 
-RepoEditableAttribute = Literal["name", "default_branch", "is_disabled"]
+VOTE_ID_TO_TYPE = {
+    10: "approved",
+    5: "approved with suggestions",
+    0: "no vote",
+    -5: "waiting for author",
+    -10: "rejected",
+}
+VoteOptions = Literal[10, 5, 0, -5, -10]
 
-# ====================================================================
+# ======================================================================================================= #
 
 
 @dataclass
-class Repo(StateManagedResource):
-    """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/repositories?view=azure-devops-rest-7.1"""
+class AdoUser(StateManagedResource):
+    """https://learn.microsoft.com/en-us/rest/api/azure/devops/graph/users?view=azure-devops-rest-7.1"""
 
-    repo_id: str = field(metadata={"is_id_field": True})
-    name: str = field(metadata={"editable": True})
-    default_branch: str = field(default="main", repr=False, metadata={"editable": True, "internal_name": "defaultBranch"})
-    is_disabled: bool = field(default=False, repr=False, metadata={"editable": True, "internal_name": "isDisabled"})
-    # WARNING, disabling a repo means it's not able to be deleted, proceed with caution.
+    descriptor_id: str = field(metadata={"is_id_field": True})
+    display_name: str
+    email: str
+    origin: str
+    origin_id: str  # DON'T USE THIS, USE `descriptor_id` INSTEAD
+    # "subjectKind": "user",
+    # "metaType": "member",
+    # "directoryAlias": "MiryabblliS",
+    # "domain": "68283f3b-8487-4c86-adb3-a5228f18b893",
+    # "url": "https://vssps.dev.azure.com/vfuk-digital/_apis/Graph/Users/aad.M2Q5NDlkZTgtZDI2Yi03MGQ3LWEyYjItMDAwYTQzYTdlNzFi",
 
     def __str__(self) -> str:
-        return f"Repo(name={self.name}, id={self.repo_id})"
+        return f"{self.display_name} ({self.email})"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str]) -> "Repo":
-        return cls(
-            data["id"], data["name"], data.get("defaultBranch", "main").removeprefix("refs/heads/"), bool(data.get("isDisabled", False))
-        )
+    def from_request_payload(cls, data: dict[str, str]) -> "AdoUser":
+        return cls(data["descriptor"], data["displayName"], data["mailAddress"].removeprefix("vstfs:///Classification/TeamProject/"),
+                   data["origin"], data["originId"])  # fmt: skip
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "Repo":
+    def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> "AdoUser":
         return super().get_by_url(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
+            ado_client,  # Preview required
+            f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, include_readme: bool = True) -> "Repo":  # type: ignore[override]
-        repo: Repo = super().create(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
-            {"name": name},
-        )  # type: ignore[assignment]
-        if include_readme:
-            Commit.add_initial_readme(ado_client, repo.repo_id)
-        return repo
-
-    def update(self, ado_client: AdoClient, attribute_name: RepoEditableAttribute, attribute_value: Any) -> None:  # type: ignore[override]
-        return super().update(
-            ado_client, "patch",
-            f"/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}?api-version=7.1",
-            attribute_name, attribute_value, {},  # fmt: skip
-        )
-
-    @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, repo_id: str) -> None:  # type: ignore[override]
-        # TODO: This never checks if it's disabled, so might error
-        for pull_request in Repo.get_all_pull_requests(ado_client, repo_id, "all"):
-            ado_client.state_manager.remove_resource_from_state("PullRequest", pull_request.pull_request_id)
-        return super().delete_by_id(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories/{repo_id}?api-version=7.1",
-            repo_id,
-        )
+    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "AdoUser":  # type: ignore[override]
+        raise NotImplementedError("Creating a new user is not supported")
+
+    @classmethod
+    def delete_by_id(cls, ado_client: AdoClient, member_id: str) -> None:  # type: ignore[override]
+        raise NotImplementedError("Deleting a user is not supported")
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list["Repo"]:  # type: ignore[override]
+    def get_all(cls, ado_client: AdoClient) -> list["AdoUser"]:  # type: ignore[override]
         return super().get_all(
-            ado_client,
-            f"/{ado_client.ado_project}/_apis/git/repositories?api-version=7.1",
+            ado_client,  # Preview required
+            f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
-    def get_by_name(cls, ado_client: AdoClient, repo_name: str) -> "Repo | None":  # type: ignore[return]
-        """Warning, this function must fetch `all` repos to work, be cautious when calling it in a loop."""
-        for repo in cls.get_all(ado_client):
-            if repo.name == repo_name:
-                return repo
-
-    def get_file(self, ado_client: AdoClient, file_path: str, branch_name: str = "main") -> str:
-        request = requests.get(
-            f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?path={file_path}&versionType={'Branch'}&version={branch_name}&api-version=7.1",
-            auth=ado_client.auth,
-        )
-        if request.status_code == 404:
-            raise ResourceNotFound(f"File {file_path} not found in repo {self.repo_id}")
-        if request.status_code != 200:
-            raise UnknownError(f"Error getting file {file_path} from repo {self.repo_id}: {request.text}")
-        return request.text  # This is the file content
-
-    def get_contents(self, ado_client: AdoClient, file_types: list[str] | None = None, branch_name: str = "main") -> dict[str, str]:
-        """https://learn.microsoft.com/en-us/rest/api/azure/devops/git/items/get?view=azure-devops-rest-7.1&tabs=HTTP
-        This function downloads the contents of a repo, and returns a dictionary of the files and their contents
-        The file_types parameter is a list of file types to filter for, e.g. ["json", "yaml"]"""
-        try:
-            request = requests.get(
-                f"https://dev.azure.com/{ado_client.ado_org}/{ado_client.ado_project}/_apis/git/repositories/{self.repo_id}/items?recursionLevel={'Full'}&download={True}&$format={'Zip'}&versionDescriptor.version={branch_name}&api-version=7.1",
-                auth=ado_client.auth,
-            )
-        except requests.exceptions.ConnectionError:
-            print(f"=== Connection error, failed to download {self.repo_id}")
-            return {}
-        if request.status_code != 200:
-            print(f"Error getting repo contents for {self.name} ({self.repo_id}):", request.text)
-            return {}
-        # ============ We do this because ADO ===================
-        bytes_io = io.BytesIO()
-        for chunk in request.iter_content(chunk_size=128):
-            bytes_io.write(chunk)
-
-        files = {}
-        try:
-            with zipfile.ZipFile(bytes_io) as zip_ref:
-                # For each file, read the bytes and convert to string
-                for file_name in [x for x in zip_ref.namelist() if file_types is None or x.split(".")[-1] in file_types]:
-                    try:
-                        files[file_name] = zip_ref.read(file_name).decode()  # fmt: skip
-                    except UnicodeDecodeError:
-                        print(f"Error decoding file: {file_name} in {self.name}")
-        except zipfile.BadZipFile as e:
-            print(f"{self.name} ({self.repo_id}) couldn't be unzipped:", e)
-
-        bytes_io.close()
-        # =========== That's all I have to say ==================
-        return files
-
-    def create_pull_request(self, ado_client: AdoClient, branch_name: str, pull_request_title: str, pull_request_description: str) -> "PullRequest":  # fmt: skip
-        """Helper function which redirects to the PullRequest class to make a PR"""
-        return PullRequest.create(ado_client, self.repo_id, branch_name, pull_request_title, pull_request_description)
-
-    @staticmethod
-    def get_all_pull_requests(ado_client: AdoClient, repo_id: str, status: PullRequestStatus = "all") -> list["PullRequest"]:
-        return PullRequest.get_all_by_repo_id(ado_client, repo_id, status)
-
-    def delete(self, ado_client: AdoClient) -> None:
-        if self.is_disabled:
-            self.update(ado_client, "is_disabled", False)
-        self.delete_by_id(ado_client, self.repo_id)
-
-    @staticmethod
-    def get_content_static(
-        ado_client: AdoClient, repo_id: str, file_types: list[str] | None = None, branch_name: str = "main"
-    ) -> dict[str, str]:
-        repo = Repo.get_by_id(ado_client, repo_id)
-        return repo.get_contents(ado_client, file_types, branch_name)
+    def get_by_email(cls, ado_client: AdoClient, member_email: str) -> "AdoUser":
+        user: AdoUser = cls.get_by_abstract_filter(ado_client, lambda user: user.email == member_email)  # type: ignore[attr-defined, assignment]
+        if not user:
+            raise ValueError(f"Member with email {member_email} not found")
+        return user
+
+    @classmethod
+    def get_by_name(cls, ado_client: AdoClient, member_name: str) -> "AdoUser | None":
+        return cls.get_by_abstract_filter(ado_client, lambda user: user.display_name == member_name)  # type: ignore[return-value, attr-defined]
 
 
-# ====================================================================
+# ======================================================================================================= #
+# ------------------------------------------------------------------------------------------------------- #
+# ======================================================================================================= #
 
 
 @dataclass
-class BuildRepository:
-    build_repository_id: str = field(metadata={"is_id_field": True})
-    name: str | None = None
-    type: str = "TfsGit"
-    clean: bool | None = None
-    checkout_submodules: bool = field(default=False, metadata={"internal_name": "checkoutSubmodules"})
+class Member(StateManagedResource):
+    """A stripped down member class which is often returned by the API, for example in build requests."""
+
+    name: str  # Static
+    email: str  # Static
+    member_id: str  # Static
+
+    def __str__(self) -> str:
+        return f"{self.name} ({self.email})"
 
     @classmethod
-    def from_request_payload(cls, data: dict[str, str | bool]) -> "BuildRepository":
-        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
+    def from_request_payload(cls, data: dict[str, Any]) -> "Member":
+        # displayName, uniqueName/mailAddress, id/originId
+        # This gets returned slightly differently from different APIs
+        return cls(data["displayName"], data.get("uniqueName") or data.get("mailAddress", "UNKNOWN"),  # type: ignore[arg-type]
+                   data.get("id") or data["originId"])  # fmt: skip
 
     @classmethod
-    def from_json(cls, data: dict[str, str | bool]) -> "BuildRepository":
-        return cls(data["id"], data.get("name"), data.get("type", "TfsGit"), data.get("clean"), data.get("checkoutSubmodules", False))  # type: ignore[arg-type]
+    def get_by_id(cls, ado_client: AdoClient, member_id: str) -> "Member":
+        raise NotImplementedError("Getting a member by ID is not supported")
 
-    def to_json(self) -> dict[str, str | bool | None]:
+    @classmethod
+    def create(cls, ado_client: AdoClient, member_name: str, member_email: str) -> "Member":  # type: ignore[override]
+        raise NotImplementedError("Creating a new member is not supported")
+
+    @classmethod
+    def delete_by_id(cls, ado_client: AdoClient, member_id: str) -> None:  # type: ignore[override]
+        raise NotImplementedError("Deleting a member is not supported")
+
+
+# ======================================================================================================= #
+# ------------------------------------------------------------------------------------------------------- #
+# ======================================================================================================= #
+
+
+class TeamMember(Member):
+    """Identical to Member, but with an additional attribute `is_team_admin`."""
+
+    def __init__(self, name: str, email: str, member_id: str, is_team_admin: bool) -> None:
+        super().__init__(name, email, member_id)
+        self.is_team_admin = is_team_admin  # Static
+
+    def __str__(self) -> str:
+        return f"{super().__str__()}" + (" (Team Admin)" if self.is_team_admin else "")
+
+    def __repr__(self) -> str:
+        return f"{super().__str__()[:-1]}, team_admin={self.is_team_admin})"
+
+    @classmethod
+    def from_json(cls, data: dict[str, Any]) -> "TeamMember":
+        return cls(data["name"], data["email"], data["id"], data["is_team_admin"])
+
+    def to_json(self) -> dict[str, Any]:
+        return {
+            "name": self.name,
+            "email": self.email,
+            "id": self.member_id,
+            "is_team_admin": self.is_team_admin,
+        }
+
+    @classmethod
+    def from_request_payload(cls, data: dict[str, Any]) -> "TeamMember":
+        return cls(data["identity"]["displayName"], data["identity"]["uniqueName"], data["identity"]["id"], data.get("isTeamAdmin", False))
+
+
+# ======================================================================================================= #
+# ------------------------------------------------------------------------------------------------------- #
+# ======================================================================================================= #
+
+
+class Reviewer(Member):
+    """Identical to Member, but with additional attributes `vote` and `is_required` for PR reviews."""
+
+    def __init__(self, name: str, email: str, reviewer_id: str, vote: VoteOptions, is_required: bool) -> None:
+        super().__init__(name, email, reviewer_id)
+        self.vote = vote  # Static
+        self.is_required = is_required  # Static
+
+    def __str__(self) -> str:
+        return f'{self.name} ({self.email}) voted {VOTE_ID_TO_TYPE[self.vote]}, and was {"required" if self.is_required else "optional"}'
+
+    def __repr__(self) -> str:
+        return f"Reviewer(name={self.name}, email={self.email}, id={self.member_id}, vote={self.vote}, is_required={self.is_required})"
+
+    def to_json(self) -> dict[str, Any]:
         return {
-            "id": self.build_repository_id, "name": self.name, "type": self.type,
-            "clean": self.clean, "checkoutSubmodules": self.checkout_submodules,  # fmt: skip
+            "name": self.name,
+            "email": self.email,
+            "id": self.member_id,
+            "vote": self.vote,
+            "is_required": self.is_required,
         }
+
+    @classmethod
+    def from_json(cls, data: dict[str, Any]) -> "Reviewer":
+        return cls(data["name"], data["email"], data["id"], data["vote"], data["isRequired"])
+
+    @classmethod
+    def from_request_payload(cls, data: dict[str, Any]) -> "Reviewer":
+        return cls(data["displayName"], data["uniqueName"], data["id"], data["vote"], data.get("isRequired", False))
+
+
+# ======================================================================================================= #
```

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/service_endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,26 +34,19 @@
     owner: str
     service_endpoint_project_references: list[dict[str, Any]]
     # _raw_data: dict[str, Any] = field(default_factory=dict)
 
     @classmethod
     def from_request_payload(cls, data: dict[str, Any]) -> ServiceEndpoint:
         return cls(
-            data["id"],
-            data["name"],
-            data["type"],
-            data["url"],
+            data["id"], data["name"], data["type"], data["url"],
             Member.from_request_payload(data["createdBy"]),
-            data.get("description", ""),
-            data["authorization"],
-            data["isShared"],
-            data["isOutdated"],
-            data["isReady"],
-            data["owner"],
-            data["serviceEndpointProjectReferences"],  # data
+            data.get("description", ""), data["authorization"], data["isShared"],
+            data["isOutdated"], data["isReady"], data["owner"],
+            data["serviceEndpointProjectReferences"],  # fmt: skip
         )
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, repo_id: str) -> "ServiceEndpoint":
         return super().get_by_url(
             ado_client,
             f"/{ado_client.ado_project}/_apis/serviceendpoint/endpoints/{repo_id}",
```

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/teams.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-0.0.6/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/state_managed_abc.py` & `ado_wrapper-0.0.6/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/ado_wrapper/state_manager.py` & `ado_wrapper-0.0.6/ado_wrapper/state_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,19 +110,15 @@
 
     def import_into_state(self, resource_type: ResourceType, resource_id: str) -> None:
         class_reference = get_resource_variables()[resource_type]
         data = class_reference.get_by_id(self.ado_client, resource_id).to_json()
         self.add_resource_to_state(resource_type, resource_id, data)
 
     def wipe_state(self) -> None:
-        if self.state_file_name is None:
-            self.state = EMPTY_STATE
-            return
-        with open(self.state_file_name, "w", encoding="utf-8") as state_file:
-            json.dump(EMPTY_STATE, state_file, indent=4)
+        self.write_state_file(EMPTY_STATE)
 
     def generate_in_memory_state(self) -> StateFileType:
         """This method goes through every resource in state and updates it to the latest version in real world space"""
         ALL_RESOURCES = get_resource_variables()
         all_states = self.load_state()
         for resource_type in all_states["resources"]:
             for resource_id in all_states["resources"][resource_type]:
```

### Comparing `ado_wrapper-0.0.5/ado_wrapper/utils.py` & `ado_wrapper-0.0.6/ado_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-0.0.5/pyproject.toml` & `ado_wrapper-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "0.0.5"
+version = "0.0.6"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-0.0.5/PKG-INFO` & `ado_wrapper-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

