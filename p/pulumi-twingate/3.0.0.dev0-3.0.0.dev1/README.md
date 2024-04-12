# Comparing `tmp/pulumi_twingate-3.0.0.dev0.tar.gz` & `tmp/pulumi_twingate-3.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_twingate-3.0.0.dev0.tar", last modified: Thu Apr 11 21:56:09 2024, max compression
+gzip compressed data, was "pulumi_twingate-3.0.0.dev1.tar", last modified: Thu Apr 11 22:11:20 2024, max compression
```

## Comparing `pulumi_twingate-3.0.0.dev0.tar` & `pulumi_twingate-3.0.0.dev1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/pulumi_twingate/
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/pulumi_twingate/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_remote_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_security_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_security_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_service_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    25767 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_connector_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_remote_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    30932 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_service_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_service_account_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 21:56:09.725505 pulumi_twingate-3.0.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-11 21:56:09.000000 pulumi_twingate-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:11:20.201274 pulumi_twingate-3.0.0.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 22:11:20.201274 pulumi_twingate-3.0.0.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:11:20.197273 pulumi_twingate-3.0.0.dev1/pulumi_twingate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:11:20.201274 pulumi_twingate-3.0.0.dev1/pulumi_twingate/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8724 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10154 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_remote_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8864 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_security_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_security_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_service_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21211 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27091 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_connector_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14916 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_remote_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34383 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15542 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_service_account_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:11:20.201274 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-11 22:11:20.000000 pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:11:20.201274 pulumi_twingate-3.0.0.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-11 22:11:19.000000 pulumi_twingate-3.0.0.dev1/setup.py
```

### Comparing `pulumi_twingate-3.0.0.dev0/PKG-INFO` & `pulumi_twingate-3.0.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_twingate
-Version: 3.0.0.dev0
+Version: 3.0.0.dev1
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.0.dev0/README.md` & `pulumi_twingate-3.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/__init__.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/_inputs.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_connector_tokens.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,301 +5,273 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = [
-    'TwingateResourceAccessArgs',
-    'TwingateResourceProtocolsArgs',
-    'TwingateResourceProtocolsTcpArgs',
-    'TwingateResourceProtocolsUdpArgs',
-    'GetTwingateResourceProtocolsArgs',
-    'GetTwingateResourceProtocolsTcpArgs',
-    'GetTwingateResourceProtocolsUdpArgs',
-]
+__all__ = ['TwingateConnectorTokensArgs', 'TwingateConnectorTokens']
 
 @pulumi.input_type
-class TwingateResourceAccessArgs:
+class TwingateConnectorTokensArgs:
     def __init__(__self__, *,
-                 group_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 service_account_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+                 connector_id: pulumi.Input[str],
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] group_ids: List of Group IDs that will have permission to access the Resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] service_account_ids: List of Service Account IDs that will have permission to access the Resource.
+        The set of arguments for constructing a TwingateConnectorTokens resource.
+        :param pulumi.Input[str] connector_id: The ID of the parent Connector
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
-        if group_ids is not None:
-            pulumi.set(__self__, "group_ids", group_ids)
-        if service_account_ids is not None:
-            pulumi.set(__self__, "service_account_ids", service_account_ids)
+        pulumi.set(__self__, "connector_id", connector_id)
+        if keepers is not None:
+            pulumi.set(__self__, "keepers", keepers)
 
     @property
-    @pulumi.getter(name="groupIds")
-    def group_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter(name="connectorId")
+    def connector_id(self) -> pulumi.Input[str]:
         """
-        List of Group IDs that will have permission to access the Resource.
+        The ID of the parent Connector
         """
-        return pulumi.get(self, "group_ids")
+        return pulumi.get(self, "connector_id")
 
-    @group_ids.setter
-    def group_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "group_ids", value)
+    @connector_id.setter
+    def connector_id(self, value: pulumi.Input[str]):
+        pulumi.set(self, "connector_id", value)
 
     @property
-    @pulumi.getter(name="serviceAccountIds")
-    def service_account_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    @pulumi.getter
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        List of Service Account IDs that will have permission to access the Resource.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
-        return pulumi.get(self, "service_account_ids")
+        return pulumi.get(self, "keepers")
 
-    @service_account_ids.setter
-    def service_account_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "service_account_ids", value)
+    @keepers.setter
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "keepers", value)
 
 
 @pulumi.input_type
-class TwingateResourceProtocolsArgs:
+class _TwingateConnectorTokensState:
     def __init__(__self__, *,
-                 allow_icmp: Optional[pulumi.Input[bool]] = None,
-                 tcp: Optional[pulumi.Input['TwingateResourceProtocolsTcpArgs']] = None,
-                 udp: Optional[pulumi.Input['TwingateResourceProtocolsUdpArgs']] = None):
-        """
-        :param pulumi.Input[bool] allow_icmp: Whether to allow ICMP (ping) traffic
-        """
-        if allow_icmp is not None:
-            pulumi.set(__self__, "allow_icmp", allow_icmp)
-        if tcp is not None:
-            pulumi.set(__self__, "tcp", tcp)
-        if udp is not None:
-            pulumi.set(__self__, "udp", udp)
-
-    @property
-    @pulumi.getter(name="allowIcmp")
-    def allow_icmp(self) -> Optional[pulumi.Input[bool]]:
+                 access_token: Optional[pulumi.Input[str]] = None,
+                 connector_id: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 refresh_token: Optional[pulumi.Input[str]] = None):
         """
-        Whether to allow ICMP (ping) traffic
+        Input properties used for looking up and filtering TwingateConnectorTokens resources.
+        :param pulumi.Input[str] access_token: The Access Token of the parent Connector
+        :param pulumi.Input[str] connector_id: The ID of the parent Connector
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
+        :param pulumi.Input[str] refresh_token: The Refresh Token of the parent Connector
         """
-        return pulumi.get(self, "allow_icmp")
-
-    @allow_icmp.setter
-    def allow_icmp(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "allow_icmp", value)
+        if access_token is not None:
+            pulumi.set(__self__, "access_token", access_token)
+        if connector_id is not None:
+            pulumi.set(__self__, "connector_id", connector_id)
+        if keepers is not None:
+            pulumi.set(__self__, "keepers", keepers)
+        if refresh_token is not None:
+            pulumi.set(__self__, "refresh_token", refresh_token)
 
     @property
-    @pulumi.getter
-    def tcp(self) -> Optional[pulumi.Input['TwingateResourceProtocolsTcpArgs']]:
-        return pulumi.get(self, "tcp")
-
-    @tcp.setter
-    def tcp(self, value: Optional[pulumi.Input['TwingateResourceProtocolsTcpArgs']]):
-        pulumi.set(self, "tcp", value)
-
-    @property
-    @pulumi.getter
-    def udp(self) -> Optional[pulumi.Input['TwingateResourceProtocolsUdpArgs']]:
-        return pulumi.get(self, "udp")
-
-    @udp.setter
-    def udp(self, value: Optional[pulumi.Input['TwingateResourceProtocolsUdpArgs']]):
-        pulumi.set(self, "udp", value)
-
-
-@pulumi.input_type
-class TwingateResourceProtocolsTcpArgs:
-    def __init__(__self__, *,
-                 policy: Optional[pulumi.Input[str]] = None,
-                 ports: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> Optional[pulumi.Input[str]]:
         """
-        :param pulumi.Input[str] policy: Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ports: List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+        The Access Token of the parent Connector
         """
-        if policy is not None:
-            pulumi.set(__self__, "policy", policy)
-        if ports is not None:
-            pulumi.set(__self__, "ports", ports)
+        return pulumi.get(self, "access_token")
+
+    @access_token.setter
+    def access_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access_token", value)
 
     @property
-    @pulumi.getter
-    def policy(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="connectorId")
+    def connector_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
+        The ID of the parent Connector
         """
-        return pulumi.get(self, "policy")
+        return pulumi.get(self, "connector_id")
 
-    @policy.setter
-    def policy(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "policy", value)
+    @connector_id.setter
+    def connector_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "connector_id", value)
 
     @property
     @pulumi.getter
-    def ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+        Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
-        return pulumi.get(self, "ports")
-
-    @ports.setter
-    def ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ports", value)
+        return pulumi.get(self, "keepers")
 
-
-@pulumi.input_type
-class TwingateResourceProtocolsUdpArgs:
-    def __init__(__self__, *,
-                 policy: Optional[pulumi.Input[str]] = None,
-                 ports: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
-        """
-        :param pulumi.Input[str] policy: Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] ports: List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
-        """
-        if policy is not None:
-            pulumi.set(__self__, "policy", policy)
-        if ports is not None:
-            pulumi.set(__self__, "ports", ports)
+    @keepers.setter
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "keepers", value)
 
     @property
-    @pulumi.getter
-    def policy(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> Optional[pulumi.Input[str]]:
         """
-        Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
+        The Refresh Token of the parent Connector
         """
-        return pulumi.get(self, "policy")
+        return pulumi.get(self, "refresh_token")
 
-    @policy.setter
-    def policy(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "policy", value)
+    @refresh_token.setter
+    def refresh_token(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "refresh_token", value)
 
-    @property
-    @pulumi.getter
-    def ports(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+
+class TwingateConnectorTokens(pulumi.CustomResource):
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 connector_id: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 __props__=None):
         """
-        return pulumi.get(self, "ports")
+        This resource type will generate tokens for a Connector, which are needed to successfully provision one on your network. The Connector itself has its own resource type and must be created before you can provision tokens.
 
-    @ports.setter
-    def ports(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "ports", value)
+        ## Example Usage
 
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_twingate as twingate
 
-@pulumi.input_type
-class GetTwingateResourceProtocolsArgs:
-    def __init__(__self__, *,
-                 allow_icmp: bool,
-                 tcp: Optional['GetTwingateResourceProtocolsTcpArgs'] = None,
-                 udp: Optional['GetTwingateResourceProtocolsUdpArgs'] = None):
-        """
-        :param bool allow_icmp: Whether to allow ICMP (ping) traffic
-        """
-        pulumi.set(__self__, "allow_icmp", allow_icmp)
-        if tcp is not None:
-            pulumi.set(__self__, "tcp", tcp)
-        if udp is not None:
-            pulumi.set(__self__, "udp", udp)
+        aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
+        aws_connector = twingate.TwingateConnector("awsConnector", remote_network_id=aws_network.id)
+        aws_connector_tokens = twingate.TwingateConnectorTokens("awsConnectorTokens", connector_id=aws_connector.id)
+        ```
+        <!--End PulumiCodeChooser -->
 
-    @property
-    @pulumi.getter(name="allowIcmp")
-    def allow_icmp(self) -> bool:
+        :param str resource_name: The name of the resource.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] connector_id: The ID of the parent Connector
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
-        Whether to allow ICMP (ping) traffic
+        ...
+    @overload
+    def __init__(__self__,
+                 resource_name: str,
+                 args: TwingateConnectorTokensArgs,
+                 opts: Optional[pulumi.ResourceOptions] = None):
         """
-        return pulumi.get(self, "allow_icmp")
+        This resource type will generate tokens for a Connector, which are needed to successfully provision one on your network. The Connector itself has its own resource type and must be created before you can provision tokens.
 
-    @allow_icmp.setter
-    def allow_icmp(self, value: bool):
-        pulumi.set(self, "allow_icmp", value)
+        ## Example Usage
 
-    @property
-    @pulumi.getter
-    def tcp(self) -> Optional['GetTwingateResourceProtocolsTcpArgs']:
-        return pulumi.get(self, "tcp")
+        <!--Start PulumiCodeChooser -->
+        ```python
+        import pulumi
+        import pulumi_twingate as twingate
 
-    @tcp.setter
-    def tcp(self, value: Optional['GetTwingateResourceProtocolsTcpArgs']):
-        pulumi.set(self, "tcp", value)
+        aws_network = twingate.TwingateRemoteNetwork("awsNetwork")
+        aws_connector = twingate.TwingateConnector("awsConnector", remote_network_id=aws_network.id)
+        aws_connector_tokens = twingate.TwingateConnectorTokens("awsConnectorTokens", connector_id=aws_connector.id)
+        ```
+        <!--End PulumiCodeChooser -->
 
-    @property
-    @pulumi.getter
-    def udp(self) -> Optional['GetTwingateResourceProtocolsUdpArgs']:
-        return pulumi.get(self, "udp")
+        :param str resource_name: The name of the resource.
+        :param TwingateConnectorTokensArgs args: The arguments to use to populate this resource's properties.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        """
+        ...
+    def __init__(__self__, resource_name: str, *args, **kwargs):
+        resource_args, opts = _utilities.get_resource_args_opts(TwingateConnectorTokensArgs, pulumi.ResourceOptions, *args, **kwargs)
+        if resource_args is not None:
+            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
+        else:
+            __self__._internal_init(resource_name, *args, **kwargs)
 
-    @udp.setter
-    def udp(self, value: Optional['GetTwingateResourceProtocolsUdpArgs']):
-        pulumi.set(self, "udp", value)
+    def _internal_init(__self__,
+                 resource_name: str,
+                 opts: Optional[pulumi.ResourceOptions] = None,
+                 connector_id: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 __props__=None):
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
+        if not isinstance(opts, pulumi.ResourceOptions):
+            raise TypeError('Expected resource options to be a ResourceOptions instance')
+        if opts.id is None:
+            if __props__ is not None:
+                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
+            __props__ = TwingateConnectorTokensArgs.__new__(TwingateConnectorTokensArgs)
 
+            if connector_id is None and not opts.urn:
+                raise TypeError("Missing required property 'connector_id'")
+            __props__.__dict__["connector_id"] = connector_id
+            __props__.__dict__["keepers"] = keepers
+            __props__.__dict__["access_token"] = None
+            __props__.__dict__["refresh_token"] = None
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["accessToken", "refreshToken"])
+        opts = pulumi.ResourceOptions.merge(opts, secret_opts)
+        super(TwingateConnectorTokens, __self__).__init__(
+            'twingate:index/twingateConnectorTokens:TwingateConnectorTokens',
+            resource_name,
+            __props__,
+            opts)
 
-@pulumi.input_type
-class GetTwingateResourceProtocolsTcpArgs:
-    def __init__(__self__, *,
-                 policy: str,
-                 ports: Sequence[str]):
-        """
-        :param str policy: Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
-        :param Sequence[str] ports: List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+    @staticmethod
+    def get(resource_name: str,
+            id: pulumi.Input[str],
+            opts: Optional[pulumi.ResourceOptions] = None,
+            access_token: Optional[pulumi.Input[str]] = None,
+            connector_id: Optional[pulumi.Input[str]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+            refresh_token: Optional[pulumi.Input[str]] = None) -> 'TwingateConnectorTokens':
         """
-        pulumi.set(__self__, "policy", policy)
-        pulumi.set(__self__, "ports", ports)
+        Get an existing TwingateConnectorTokens resource's state with the given name, id, and optional extra
+        properties used to qualify the lookup.
 
-    @property
-    @pulumi.getter
-    def policy(self) -> str:
-        """
-        Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
+        :param str resource_name: The unique name of the resulting resource.
+        :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
+        :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[str] access_token: The Access Token of the parent Connector
+        :param pulumi.Input[str] connector_id: The ID of the parent Connector
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
+        :param pulumi.Input[str] refresh_token: The Refresh Token of the parent Connector
         """
-        return pulumi.get(self, "policy")
+        opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-    @policy.setter
-    def policy(self, value: str):
-        pulumi.set(self, "policy", value)
+        __props__ = _TwingateConnectorTokensState.__new__(_TwingateConnectorTokensState)
+
+        __props__.__dict__["access_token"] = access_token
+        __props__.__dict__["connector_id"] = connector_id
+        __props__.__dict__["keepers"] = keepers
+        __props__.__dict__["refresh_token"] = refresh_token
+        return TwingateConnectorTokens(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def ports(self) -> Sequence[str]:
+    @pulumi.getter(name="accessToken")
+    def access_token(self) -> pulumi.Output[str]:
         """
-        List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+        The Access Token of the parent Connector
         """
-        return pulumi.get(self, "ports")
+        return pulumi.get(self, "access_token")
 
-    @ports.setter
-    def ports(self, value: Sequence[str]):
-        pulumi.set(self, "ports", value)
-
-
-@pulumi.input_type
-class GetTwingateResourceProtocolsUdpArgs:
-    def __init__(__self__, *,
-                 policy: str,
-                 ports: Sequence[str]):
+    @property
+    @pulumi.getter(name="connectorId")
+    def connector_id(self) -> pulumi.Output[str]:
         """
-        :param str policy: Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
-        :param Sequence[str] ports: List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+        The ID of the parent Connector
         """
-        pulumi.set(__self__, "policy", policy)
-        pulumi.set(__self__, "ports", ports)
+        return pulumi.get(self, "connector_id")
 
     @property
     @pulumi.getter
-    def policy(self) -> str:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Whether to allow or deny all ports, or restrict protocol access within certain port ranges: Can be `RESTRICTED` (only listed ports are allowed), `ALLOW_ALL`, or `DENY_ALL`
+        Arbitrary map of values that, when changed, will trigger recreation of resource. Use this to automatically rotate Connector tokens on a schedule.
         """
-        return pulumi.get(self, "policy")
-
-    @policy.setter
-    def policy(self, value: str):
-        pulumi.set(self, "policy", value)
+        return pulumi.get(self, "keepers")
 
     @property
-    @pulumi.getter
-    def ports(self) -> Sequence[str]:
+    @pulumi.getter(name="refreshToken")
+    def refresh_token(self) -> pulumi.Output[str]:
         """
-        List of port ranges between 1 and 65535 inclusive, in the format `100-200` for a range, or `8080` for a single port
+        The Refresh Token of the parent Connector
         """
-        return pulumi.get(self, "ports")
-
-    @ports.setter
-    def ports(self, value: Sequence[str]):
-        pulumi.set(self, "ports", value)
-
+        return pulumi.get(self, "refresh_token")
```

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/_utilities.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/config/vars.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_connector.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_connectors.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_connectors.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_group.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_groups.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_remote_network.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_remote_networks.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_remote_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_resource.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_resources.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_security_policies.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_security_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_security_policy.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_security_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_service_accounts.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_service_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_user.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/get_twingate_users.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/get_twingate_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/outputs.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
-    'TwingateResourceAccess',
+    'TwingateResourceAccessGroup',
+    'TwingateResourceAccessService',
     'TwingateResourceProtocols',
     'TwingateResourceProtocolsTcp',
     'TwingateResourceProtocolsUdp',
     'GetTwingateConnectorsConnectorResult',
     'GetTwingateGroupsGroupResult',
     'GetTwingateRemoteNetworksRemoteNetworkResult',
     'GetTwingateResourceProtocolsResult',
@@ -27,61 +28,97 @@
     'GetTwingateResourcesResourceProtocolsUdpResult',
     'GetTwingateSecurityPoliciesSecurityPolicyResult',
     'GetTwingateServiceAccountsServiceAccountResult',
     'GetTwingateUsersUserResult',
 ]
 
 @pulumi.output_type
-class TwingateResourceAccess(dict):
+class TwingateResourceAccessGroup(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
-        if key == "groupIds":
-            suggest = "group_ids"
-        elif key == "serviceAccountIds":
-            suggest = "service_account_ids"
+        if key == "groupId":
+            suggest = "group_id"
+        elif key == "securityPolicyId":
+            suggest = "security_policy_id"
 
         if suggest:
-            pulumi.log.warn(f"Key '{key}' not found in TwingateResourceAccess. Access the value via the '{suggest}' property getter instead.")
+            pulumi.log.warn(f"Key '{key}' not found in TwingateResourceAccessGroup. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
-        TwingateResourceAccess.__key_warning(key)
+        TwingateResourceAccessGroup.__key_warning(key)
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
-        TwingateResourceAccess.__key_warning(key)
+        TwingateResourceAccessGroup.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
-                 group_ids: Optional[Sequence[str]] = None,
-                 service_account_ids: Optional[Sequence[str]] = None):
+                 group_id: Optional[str] = None,
+                 security_policy_id: Optional[str] = None):
         """
-        :param Sequence[str] group_ids: List of Group IDs that will have permission to access the Resource.
-        :param Sequence[str] service_account_ids: List of Service Account IDs that will have permission to access the Resource.
+        :param str group_id: Group ID that will have permission to access the Resource.
+        :param str security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
-        if group_ids is not None:
-            pulumi.set(__self__, "group_ids", group_ids)
-        if service_account_ids is not None:
-            pulumi.set(__self__, "service_account_ids", service_account_ids)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if security_policy_id is not None:
+            pulumi.set(__self__, "security_policy_id", security_policy_id)
 
     @property
-    @pulumi.getter(name="groupIds")
-    def group_ids(self) -> Optional[Sequence[str]]:
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[str]:
         """
-        List of Group IDs that will have permission to access the Resource.
+        Group ID that will have permission to access the Resource.
         """
-        return pulumi.get(self, "group_ids")
+        return pulumi.get(self, "group_id")
 
     @property
-    @pulumi.getter(name="serviceAccountIds")
-    def service_account_ids(self) -> Optional[Sequence[str]]:
+    @pulumi.getter(name="securityPolicyId")
+    def security_policy_id(self) -> Optional[str]:
         """
-        List of Service Account IDs that will have permission to access the Resource.
+        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
-        return pulumi.get(self, "service_account_ids")
+        return pulumi.get(self, "security_policy_id")
+
+
+@pulumi.output_type
+class TwingateResourceAccessService(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "serviceAccountId":
+            suggest = "service_account_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in TwingateResourceAccessService. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        TwingateResourceAccessService.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        TwingateResourceAccessService.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 service_account_id: Optional[str] = None):
+        """
+        :param str service_account_id: The ID of the service account that should have access to this Resource.
+        """
+        if service_account_id is not None:
+            pulumi.set(__self__, "service_account_id", service_account_id)
+
+    @property
+    @pulumi.getter(name="serviceAccountId")
+    def service_account_id(self) -> Optional[str]:
+        """
+        The ID of the service account that should have access to this Resource.
+        """
+        return pulumi.get(self, "service_account_id")
 
 
 @pulumi.output_type
 class TwingateResourceProtocols(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
```

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/provider.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_connector.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_group.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_remote_network.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_remote_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_resource.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,42 +14,46 @@
 __all__ = ['TwingateResourceArgs', 'TwingateResource']
 
 @pulumi.input_type
 class TwingateResourceArgs:
     def __init__(__self__, *,
                  address: pulumi.Input[str],
                  remote_network_id: pulumi.Input[str],
-                 access: Optional[pulumi.Input['TwingateResourceAccessArgs']] = None,
+                 access_groups: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]] = None,
+                 access_services: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]] = None,
                  alias: Optional[pulumi.Input[str]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  is_browser_shortcut_enabled: Optional[pulumi.Input[bool]] = None,
                  is_visible: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protocols: Optional[pulumi.Input['TwingateResourceProtocolsArgs']] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a TwingateResource resource.
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input['TwingateResourceAccessArgs'] access: Restrict access to certain groups or service accounts
+        :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]] access_groups: Restrict access to certain group
+        :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "remote_network_id", remote_network_id)
-        if access is not None:
-            pulumi.set(__self__, "access", access)
+        if access_groups is not None:
+            pulumi.set(__self__, "access_groups", access_groups)
+        if access_services is not None:
+            pulumi.set(__self__, "access_services", access_services)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if is_active is not None:
             pulumi.set(__self__, "is_active", is_active)
         if is_authoritative is not None:
             pulumi.set(__self__, "is_authoritative", is_authoritative)
         if is_browser_shortcut_enabled is not None:
@@ -84,24 +88,36 @@
         return pulumi.get(self, "remote_network_id")
 
     @remote_network_id.setter
     def remote_network_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "remote_network_id", value)
 
     @property
-    @pulumi.getter
-    def access(self) -> Optional[pulumi.Input['TwingateResourceAccessArgs']]:
+    @pulumi.getter(name="accessGroups")
+    def access_groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]]:
         """
-        Restrict access to certain groups or service accounts
+        Restrict access to certain group
         """
-        return pulumi.get(self, "access")
+        return pulumi.get(self, "access_groups")
 
-    @access.setter
-    def access(self, value: Optional[pulumi.Input['TwingateResourceAccessArgs']]):
-        pulumi.set(self, "access", value)
+    @access_groups.setter
+    def access_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]]):
+        pulumi.set(self, "access_groups", value)
+
+    @property
+    @pulumi.getter(name="accessServices")
+    def access_services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]]:
+        """
+        Restrict access to certain service account
+        """
+        return pulumi.get(self, "access_services")
+
+    @access_services.setter
+    def access_services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]]):
+        pulumi.set(self, "access_services", value)
 
     @property
     @pulumi.getter
     def alias(self) -> Optional[pulumi.Input[str]]:
         """
         Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         """
@@ -184,54 +200,58 @@
     def protocols(self, value: Optional[pulumi.Input['TwingateResourceProtocolsArgs']]):
         pulumi.set(self, "protocols", value)
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
 
 @pulumi.input_type
 class _TwingateResourceState:
     def __init__(__self__, *,
-                 access: Optional[pulumi.Input['TwingateResourceAccessArgs']] = None,
+                 access_groups: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]] = None,
+                 access_services: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  alias: Optional[pulumi.Input[str]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  is_browser_shortcut_enabled: Optional[pulumi.Input[bool]] = None,
                  is_visible: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  protocols: Optional[pulumi.Input['TwingateResourceProtocolsArgs']] = None,
                  remote_network_id: Optional[pulumi.Input[str]] = None,
                  security_policy_id: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TwingateResource resources.
-        :param pulumi.Input['TwingateResourceAccessArgs'] access: Restrict access to certain groups or service accounts
+        :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]] access_groups: Restrict access to certain group
+        :param pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input['TwingateResourceProtocolsArgs'] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
-        if access is not None:
-            pulumi.set(__self__, "access", access)
+        if access_groups is not None:
+            pulumi.set(__self__, "access_groups", access_groups)
+        if access_services is not None:
+            pulumi.set(__self__, "access_services", access_services)
         if address is not None:
             pulumi.set(__self__, "address", address)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if is_active is not None:
             pulumi.set(__self__, "is_active", is_active)
         if is_authoritative is not None:
@@ -246,24 +266,36 @@
             pulumi.set(__self__, "protocols", protocols)
         if remote_network_id is not None:
             pulumi.set(__self__, "remote_network_id", remote_network_id)
         if security_policy_id is not None:
             pulumi.set(__self__, "security_policy_id", security_policy_id)
 
     @property
-    @pulumi.getter
-    def access(self) -> Optional[pulumi.Input['TwingateResourceAccessArgs']]:
+    @pulumi.getter(name="accessGroups")
+    def access_groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]]:
         """
-        Restrict access to certain groups or service accounts
+        Restrict access to certain group
         """
-        return pulumi.get(self, "access")
+        return pulumi.get(self, "access_groups")
 
-    @access.setter
-    def access(self, value: Optional[pulumi.Input['TwingateResourceAccessArgs']]):
-        pulumi.set(self, "access", value)
+    @access_groups.setter
+    def access_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessGroupArgs']]]]):
+        pulumi.set(self, "access_groups", value)
+
+    @property
+    @pulumi.getter(name="accessServices")
+    def access_services(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]]:
+        """
+        Restrict access to certain service account
+        """
+        return pulumi.get(self, "access_services")
+
+    @access_services.setter
+    def access_services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TwingateResourceAccessServiceArgs']]]]):
+        pulumi.set(self, "access_services", value)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
         """
         The Resource's IP/CIDR or FQDN/DNS zone
         """
@@ -370,29 +402,30 @@
     def remote_network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "remote_network_id", value)
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         return pulumi.get(self, "security_policy_id")
 
     @security_policy_id.setter
     def security_policy_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_policy_id", value)
 
 
 class TwingateResource(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 access: Optional[pulumi.Input[pulumi.InputType['TwingateResourceAccessArgs']]] = None,
+                 access_groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]]] = None,
+                 access_services: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]]] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  alias: Optional[pulumi.Input[str]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  is_browser_shortcut_enabled: Optional[pulumi.Input[bool]] = None,
                  is_visible: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -407,26 +440,27 @@
 
         ```sh
         $ pulumi import twingate:index/twingateResource:TwingateResource resource UmVzb3VyY2U6MzQwNDQ3
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['TwingateResourceAccessArgs']] access: Restrict access to certain groups or service accounts
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]] access_groups: Restrict access to certain group
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TwingateResourceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -450,15 +484,16 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 access: Optional[pulumi.Input[pulumi.InputType['TwingateResourceAccessArgs']]] = None,
+                 access_groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]]] = None,
+                 access_services: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]]] = None,
                  address: Optional[pulumi.Input[str]] = None,
                  alias: Optional[pulumi.Input[str]] = None,
                  is_active: Optional[pulumi.Input[bool]] = None,
                  is_authoritative: Optional[pulumi.Input[bool]] = None,
                  is_browser_shortcut_enabled: Optional[pulumi.Input[bool]] = None,
                  is_visible: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
@@ -470,15 +505,16 @@
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TwingateResourceArgs.__new__(TwingateResourceArgs)
 
-            __props__.__dict__["access"] = access
+            __props__.__dict__["access_groups"] = access_groups
+            __props__.__dict__["access_services"] = access_services
             if address is None and not opts.urn:
                 raise TypeError("Missing required property 'address'")
             __props__.__dict__["address"] = address
             __props__.__dict__["alias"] = alias
             __props__.__dict__["is_active"] = is_active
             __props__.__dict__["is_authoritative"] = is_authoritative
             __props__.__dict__["is_browser_shortcut_enabled"] = is_browser_shortcut_enabled
@@ -495,15 +531,16 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            access: Optional[pulumi.Input[pulumi.InputType['TwingateResourceAccessArgs']]] = None,
+            access_groups: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]]] = None,
+            access_services: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]]] = None,
             address: Optional[pulumi.Input[str]] = None,
             alias: Optional[pulumi.Input[str]] = None,
             is_active: Optional[pulumi.Input[bool]] = None,
             is_authoritative: Optional[pulumi.Input[bool]] = None,
             is_browser_shortcut_enabled: Optional[pulumi.Input[bool]] = None,
             is_visible: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
@@ -513,51 +550,61 @@
         """
         Get an existing TwingateResource resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['TwingateResourceAccessArgs']] access: Restrict access to certain groups or service accounts
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessGroupArgs']]]] access_groups: Restrict access to certain group
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TwingateResourceAccessServiceArgs']]]] access_services: Restrict access to certain service account
         :param pulumi.Input[str] address: The Resource's IP/CIDR or FQDN/DNS zone
         :param pulumi.Input[str] alias: Set a DNS alias address for the Resource. Must be a DNS-valid name string.
         :param pulumi.Input[bool] is_active: Set the resource as active or inactive. Default is `true`.
         :param pulumi.Input[bool] is_authoritative: Determines whether assignments in the access block will override any existing assignments. Default is `true`. If set to
                `false`, assignments made outside of Terraform will be ignored.
         :param pulumi.Input[bool] is_browser_shortcut_enabled: Controls whether an "Open in Browser" shortcut will be shown for this Resource in the Twingate Client. Default is `false`.
         :param pulumi.Input[bool] is_visible: Controls whether this Resource will be visible in the main Resource list in the Twingate Client. Default is `true`.
         :param pulumi.Input[str] name: The name of the Resource
         :param pulumi.Input[pulumi.InputType['TwingateResourceProtocolsArgs']] protocols: Restrict access to certain protocols and ports. By default or when this argument is not defined, there is no restriction, and all protocols and ports are allowed.
         :param pulumi.Input[str] remote_network_id: Remote Network ID where the Resource lives
-        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        :param pulumi.Input[str] security_policy_id: The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TwingateResourceState.__new__(_TwingateResourceState)
 
-        __props__.__dict__["access"] = access
+        __props__.__dict__["access_groups"] = access_groups
+        __props__.__dict__["access_services"] = access_services
         __props__.__dict__["address"] = address
         __props__.__dict__["alias"] = alias
         __props__.__dict__["is_active"] = is_active
         __props__.__dict__["is_authoritative"] = is_authoritative
         __props__.__dict__["is_browser_shortcut_enabled"] = is_browser_shortcut_enabled
         __props__.__dict__["is_visible"] = is_visible
         __props__.__dict__["name"] = name
         __props__.__dict__["protocols"] = protocols
         __props__.__dict__["remote_network_id"] = remote_network_id
         __props__.__dict__["security_policy_id"] = security_policy_id
         return TwingateResource(resource_name, opts=opts, __props__=__props__)
 
     @property
-    @pulumi.getter
-    def access(self) -> pulumi.Output[Optional['outputs.TwingateResourceAccess']]:
+    @pulumi.getter(name="accessGroups")
+    def access_groups(self) -> pulumi.Output[Optional[Sequence['outputs.TwingateResourceAccessGroup']]]:
+        """
+        Restrict access to certain group
+        """
+        return pulumi.get(self, "access_groups")
+
+    @property
+    @pulumi.getter(name="accessServices")
+    def access_services(self) -> pulumi.Output[Optional[Sequence['outputs.TwingateResourceAccessService']]]:
         """
-        Restrict access to certain groups or service accounts
+        Restrict access to certain service account
         """
-        return pulumi.get(self, "access")
+        return pulumi.get(self, "access_services")
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Output[str]:
         """
         The Resource's IP/CIDR or FQDN/DNS zone
         """
@@ -628,11 +675,11 @@
         """
         return pulumi.get(self, "remote_network_id")
 
     @property
     @pulumi.getter(name="securityPolicyId")
     def security_policy_id(self) -> pulumi.Output[str]:
         """
-        The ID of a `get_twingate_security_policy` to set as this Resource's Security Policy. Default is `Default Policy`.
+        The ID of a `get_twingate_security_policy` to use as the access policy for the group IDs in the access block.
         """
         return pulumi.get(self, "security_policy_id")
```

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_service_account.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_service_account_key.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_service_account_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate/twingate_user.py` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate/twingate_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/PKG-INFO` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-twingate
-Version: 3.0.0.dev0
+Version: 3.0.0.dev1
 Summary: A Pulumi package for creating and managing Twingate cloud resources.
 Home-page: https://www.twingate.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Twingate/pulumi-twingate
 Keywords: pulumi twingate category/infrastructure
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_twingate-3.0.0.dev0/pulumi_twingate.egg-info/SOURCES.txt` & `pulumi_twingate-3.0.0.dev1/pulumi_twingate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_twingate-3.0.0.dev0/setup.py` & `pulumi_twingate-3.0.0.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.0.0dev0"
+VERSION = "3.0.0dev1"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "twingate Pulumi Package - Development Version"
```

