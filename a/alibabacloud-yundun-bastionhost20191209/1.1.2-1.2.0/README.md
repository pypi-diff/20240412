# Comparing `tmp/alibabacloud_yundun-bastionhost20191209-1.1.2.tar.gz` & `tmp/alibabacloud_yundun-bastionhost20191209-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_yundun-bastionhost20191209-1.1.2.tar", last modified: Wed Feb 28 17:21:40 2024, max compression
+gzip compressed data, was "dist/alibabacloud_yundun-bastionhost20191209-1.2.0.tar", last modified: Fri Apr 12 17:11:49 2024, max compression
```

## Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2.tar` & `alibabacloud_yundun-bastionhost20191209-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      483 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2506 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1240 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/__init__.py
--rw-r--r--   0 root         (0) root         (0)   366342 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/client.py
--rw-r--r--   0 root         (0) root         (0)   585340 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2506 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-28 17:21:40.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2688 2024-02-28 17:21:39.000000 alibabacloud_yundun-bastionhost20191209-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1707 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   594860 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/client.py
+-rw-r--r--   0 root         (0) root         (0)   967616 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2688 2024-04-12 17:11:49.000000 alibabacloud_yundun-bastionhost20191209-1.2.0/setup.py
```

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/LICENSE` & `alibabacloud_yundun-bastionhost20191209-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/PKG-INFO` & `alibabacloud_yundun-bastionhost20191209-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_yundun-bastionhost20191209
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/README-CN.md` & `alibabacloud_yundun-bastionhost20191209-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/README.md` & `alibabacloud_yundun-bastionhost20191209-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/client.py` & `alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -235,14 +235,96 @@
         
         @param request: AcceptOperationTicketRequest
         @return: AcceptOperationTicketResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.accept_operation_ticket_with_options_async(request, runtime)
 
+    def add_databases_to_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.AddDatabasesToGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AddDatabasesToGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def add_databases_to_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AddDatabasesToGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AddDatabasesToGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def add_databases_to_group(
+        self,
+        request: yundun_bastionhost_20191209_models.AddDatabasesToGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.add_databases_to_group_with_options(request, runtime)
+
+    async def add_databases_to_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AddDatabasesToGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.AddDatabasesToGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.add_databases_to_group_with_options_async(request, runtime)
+
     def add_hosts_to_group_with_options(
         self,
         request: yundun_bastionhost_20191209_models.AddHostsToGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.AddHostsToGroupResponse:
         """
         You can call this operation to add one or more hosts to a host group. You can add multiple hosts to a host group to manage and grant permissions on the hosts in a centralized manner.
@@ -471,14 +553,178 @@
         
         @param request: AddUsersToGroupRequest
         @return: AddUsersToGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.add_users_to_group_with_options_async(request, runtime)
 
+    def attach_database_accounts_to_user_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AttachDatabaseAccountsToUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def attach_database_accounts_to_user_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AttachDatabaseAccountsToUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def attach_database_accounts_to_user(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserRequest,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.attach_database_accounts_to_user_with_options(request, runtime)
+
+    async def attach_database_accounts_to_user_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserRequest,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.attach_database_accounts_to_user_with_options_async(request, runtime)
+
+    def attach_database_accounts_to_user_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AttachDatabaseAccountsToUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def attach_database_accounts_to_user_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='AttachDatabaseAccountsToUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def attach_database_accounts_to_user_group(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.attach_database_accounts_to_user_group_with_options(request, runtime)
+
+    async def attach_database_accounts_to_user_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.AttachDatabaseAccountsToUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.attach_database_accounts_to_user_group_with_options_async(request, runtime)
+
     def attach_host_accounts_to_host_share_key_with_options(
         self,
         request: yundun_bastionhost_20191209_models.AttachHostAccountsToHostShareKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.AttachHostAccountsToHostShareKeyResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -995,15 +1241,18 @@
 
     def config_instance_white_list_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ConfigInstanceWhiteListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ConfigInstanceWhiteListResponse:
         """
-        The ID of the request, which is used to locate and troubleshoot issues.
+        ## Usage notes
+        You can call this operation to configure a whitelist of public IP addresses for a bastion host. By default, a bastion host is accessible from all public IP addresses. If you want to allow the requests from specific public IP addresses, you can call this operation to add trusted IP addresses to the whitelist of the bastion host.
+        ## Limits
+        You can call this operation up to 30 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: ConfigInstanceWhiteListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigInstanceWhiteListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1034,15 +1283,18 @@
 
     async def config_instance_white_list_with_options_async(
         self,
         request: yundun_bastionhost_20191209_models.ConfigInstanceWhiteListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ConfigInstanceWhiteListResponse:
         """
-        The ID of the request, which is used to locate and troubleshoot issues.
+        ## Usage notes
+        You can call this operation to configure a whitelist of public IP addresses for a bastion host. By default, a bastion host is accessible from all public IP addresses. If you want to allow the requests from specific public IP addresses, you can call this operation to add trusted IP addresses to the whitelist of the bastion host.
+        ## Limits
+        You can call this operation up to 30 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: ConfigInstanceWhiteListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigInstanceWhiteListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1072,35 +1324,257 @@
         )
 
     def config_instance_white_list(
         self,
         request: yundun_bastionhost_20191209_models.ConfigInstanceWhiteListRequest,
     ) -> yundun_bastionhost_20191209_models.ConfigInstanceWhiteListResponse:
         """
-        The ID of the request, which is used to locate and troubleshoot issues.
+        ## Usage notes
+        You can call this operation to configure a whitelist of public IP addresses for a bastion host. By default, a bastion host is accessible from all public IP addresses. If you want to allow the requests from specific public IP addresses, you can call this operation to add trusted IP addresses to the whitelist of the bastion host.
+        ## Limits
+        You can call this operation up to 30 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: ConfigInstanceWhiteListRequest
         @return: ConfigInstanceWhiteListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.config_instance_white_list_with_options(request, runtime)
 
     async def config_instance_white_list_async(
         self,
         request: yundun_bastionhost_20191209_models.ConfigInstanceWhiteListRequest,
     ) -> yundun_bastionhost_20191209_models.ConfigInstanceWhiteListResponse:
         """
-        The ID of the request, which is used to locate and troubleshoot issues.
+        ## Usage notes
+        You can call this operation to configure a whitelist of public IP addresses for a bastion host. By default, a bastion host is accessible from all public IP addresses. If you want to allow the requests from specific public IP addresses, you can call this operation to add trusted IP addresses to the whitelist of the bastion host.
+        ## Limits
+        You can call this operation up to 30 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: ConfigInstanceWhiteListRequest
         @return: ConfigInstanceWhiteListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.config_instance_white_list_with_options_async(request, runtime)
 
+    def create_database_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.active_address_type):
+            query['ActiveAddressType'] = request.active_address_type
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_port):
+            query['DatabasePort'] = request.database_port
+        if not UtilClient.is_unset(request.database_private_address):
+            query['DatabasePrivateAddress'] = request.database_private_address
+        if not UtilClient.is_unset(request.database_public_address):
+            query['DatabasePublicAddress'] = request.database_public_address
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.polar_dbendpoint_type):
+            query['PolarDBEndpointType'] = request.polar_dbendpoint_type
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_region_id):
+            query['SourceInstanceRegionId'] = request.source_instance_region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_database_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.active_address_type):
+            query['ActiveAddressType'] = request.active_address_type
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_port):
+            query['DatabasePort'] = request.database_port
+        if not UtilClient.is_unset(request.database_private_address):
+            query['DatabasePrivateAddress'] = request.database_private_address
+        if not UtilClient.is_unset(request.database_public_address):
+            query['DatabasePublicAddress'] = request.database_public_address
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.polar_dbendpoint_type):
+            query['PolarDBEndpointType'] = request.polar_dbendpoint_type
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_region_id):
+            query['SourceInstanceRegionId'] = request.source_instance_region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateDatabaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_database(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_database_with_options(request, runtime)
+
+    async def create_database_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_database_with_options_async(request, runtime)
+
+    def create_database_account_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.database_schema):
+            query['DatabaseSchema'] = request.database_schema
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.login_attribute):
+            query['LoginAttribute'] = request.login_attribute
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_database_account_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.database_schema):
+            query['DatabaseSchema'] = request.database_schema
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.login_attribute):
+            query['LoginAttribute'] = request.login_attribute
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_database_account(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_database_account_with_options(request, runtime)
+
+    async def create_database_account_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_database_account_with_options_async(request, runtime)
+
     def create_host_with_options(
         self,
         request: yundun_bastionhost_20191209_models.CreateHostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.CreateHostResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1477,14 +1951,300 @@
     async def create_host_share_key_async(
         self,
         request: yundun_bastionhost_20191209_models.CreateHostShareKeyRequest,
     ) -> yundun_bastionhost_20191209_models.CreateHostShareKeyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_host_share_key_with_options_async(request, runtime)
 
+    def create_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.proxies):
+            query['Proxies'] = request.proxies
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.proxies):
+            query['Proxies'] = request.proxies
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_network_domain_with_options(request, runtime)
+
+    async def create_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_network_domain_with_options_async(request, runtime)
+
+    def create_policy_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.CreatePolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreatePolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.priority):
+            query['Priority'] = request.priority
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreatePolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreatePolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_policy_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreatePolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreatePolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.priority):
+            query['Priority'] = request.priority
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreatePolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreatePolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_policy(
+        self,
+        request: yundun_bastionhost_20191209_models.CreatePolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.CreatePolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_policy_with_options(request, runtime)
+
+    async def create_policy_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreatePolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.CreatePolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_policy_with_options_async(request, runtime)
+
+    def create_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.effective_end_time):
+            query['EffectiveEndTime'] = request.effective_end_time
+        if not UtilClient.is_unset(request.effective_start_time):
+            query['EffectiveStartTime'] = request.effective_start_time
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.CreateRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.effective_end_time):
+            query['EffectiveEndTime'] = request.effective_end_time
+        if not UtilClient.is_unset(request.effective_start_time):
+            query['EffectiveStartTime'] = request.effective_start_time
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.CreateRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_rule_with_options(request, runtime)
+
+    async def create_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.CreateRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.CreateRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_rule_with_options_async(request, runtime)
+
     def create_user_with_options(
         self,
         request: yundun_bastionhost_20191209_models.CreateUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.CreateUserResponse:
         """
         ## Usage notes
@@ -1881,14 +2641,170 @@
         
         @param request: CreateUserPublicKeyRequest
         @return: CreateUserPublicKeyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_public_key_with_options_async(request, runtime)
 
+    def delete_database_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_database_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteDatabaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_database(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_database_with_options(request, runtime)
+
+    async def delete_database_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_database_with_options_async(request, runtime)
+
+    def delete_database_account_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_database_account_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_database_account(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_database_account_with_options(request, runtime)
+
+    async def delete_database_account_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_database_account_with_options_async(request, runtime)
+
     def delete_host_with_options(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.DeleteHostResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1966,18 +2882,18 @@
     def delete_host_account_with_options(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.DeleteHostAccountResponse:
         """
         ## Usage notes
-        You can call this operation to remove a single host account. If you no longer use a host account that is added to a host in Bastionhost, you can call this operation to remove the host account from the host.
+        This interface is used to delete individual host accounts. If a host account is no longer in use, you can invoke this interface to delete the host account for that host that has been configured on the bastion.
         >  After you remove the host account, you must enter the username and password of the host when you log on to the host in Bastionhost.
-        ## Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        ## QPS Limit
+        The single-user QPS limit of this interface is 10 times/second. If the limit is exceeded, the API call will be stream-limited, which may affect your business, please call reasonably.
         
         @param request: DeleteHostAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteHostAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2009,18 +2925,18 @@
     async def delete_host_account_with_options_async(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.DeleteHostAccountResponse:
         """
         ## Usage notes
-        You can call this operation to remove a single host account. If you no longer use a host account that is added to a host in Bastionhost, you can call this operation to remove the host account from the host.
+        This interface is used to delete individual host accounts. If a host account is no longer in use, you can invoke this interface to delete the host account for that host that has been configured on the bastion.
         >  After you remove the host account, you must enter the username and password of the host when you log on to the host in Bastionhost.
-        ## Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        ## QPS Limit
+        The single-user QPS limit of this interface is 10 times/second. If the limit is exceeded, the API call will be stream-limited, which may affect your business, please call reasonably.
         
         @param request: DeleteHostAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteHostAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2051,35 +2967,35 @@
 
     def delete_host_account(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostAccountRequest,
     ) -> yundun_bastionhost_20191209_models.DeleteHostAccountResponse:
         """
         ## Usage notes
-        You can call this operation to remove a single host account. If you no longer use a host account that is added to a host in Bastionhost, you can call this operation to remove the host account from the host.
+        This interface is used to delete individual host accounts. If a host account is no longer in use, you can invoke this interface to delete the host account for that host that has been configured on the bastion.
         >  After you remove the host account, you must enter the username and password of the host when you log on to the host in Bastionhost.
-        ## Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        ## QPS Limit
+        The single-user QPS limit of this interface is 10 times/second. If the limit is exceeded, the API call will be stream-limited, which may affect your business, please call reasonably.
         
         @param request: DeleteHostAccountRequest
         @return: DeleteHostAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_host_account_with_options(request, runtime)
 
     async def delete_host_account_async(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostAccountRequest,
     ) -> yundun_bastionhost_20191209_models.DeleteHostAccountResponse:
         """
         ## Usage notes
-        You can call this operation to remove a single host account. If you no longer use a host account that is added to a host in Bastionhost, you can call this operation to remove the host account from the host.
+        This interface is used to delete individual host accounts. If a host account is no longer in use, you can invoke this interface to delete the host account for that host that has been configured on the bastion.
         >  After you remove the host account, you must enter the username and password of the host when you log on to the host in Bastionhost.
-        ## Limits
-        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        ## QPS Limit
+        The single-user QPS limit of this interface is 10 times/second. If the limit is exceeded, the API call will be stream-limited, which may affect your business, please call reasonably.
         
         @param request: DeleteHostAccountRequest
         @return: DeleteHostAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_host_account_with_options_async(request, runtime)
 
@@ -2269,14 +3185,248 @@
     async def delete_host_share_key_async(
         self,
         request: yundun_bastionhost_20191209_models.DeleteHostShareKeyRequest,
     ) -> yundun_bastionhost_20191209_models.DeleteHostShareKeyResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_host_share_key_with_options_async(request, runtime)
 
+    def delete_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_network_domain_with_options(request, runtime)
+
+    async def delete_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_network_domain_with_options_async(request, runtime)
+
+    def delete_policy_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DeletePolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeletePolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeletePolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeletePolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_policy_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeletePolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeletePolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeletePolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeletePolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_policy(
+        self,
+        request: yundun_bastionhost_20191209_models.DeletePolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.DeletePolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_policy_with_options(request, runtime)
+
+    async def delete_policy_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeletePolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.DeletePolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_policy_with_options_async(request, runtime)
+
+    def delete_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DeleteRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DeleteRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DeleteRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_rule_with_options(request, runtime)
+
+    async def delete_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DeleteRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.DeleteRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_rule_with_options_async(request, runtime)
+
     def delete_user_with_options(
         self,
         request: yundun_bastionhost_20191209_models.DeleteUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.DeleteUserResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -2775,14 +3925,178 @@
     async def describe_regions_async(
         self,
         request: yundun_bastionhost_20191209_models.DescribeRegionsRequest,
     ) -> yundun_bastionhost_20191209_models.DescribeRegionsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_regions_with_options_async(request, runtime)
 
+    def detach_database_accounts_from_user_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DetachDatabaseAccountsFromUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def detach_database_accounts_from_user_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DetachDatabaseAccountsFromUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def detach_database_accounts_from_user(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserRequest,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.detach_database_accounts_from_user_with_options(request, runtime)
+
+    async def detach_database_accounts_from_user_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserRequest,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.detach_database_accounts_from_user_with_options_async(request, runtime)
+
+    def detach_database_accounts_from_user_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DetachDatabaseAccountsFromUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def detach_database_accounts_from_user_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DetachDatabaseAccountsFromUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def detach_database_accounts_from_user_group(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.detach_database_accounts_from_user_group_with_options(request, runtime)
+
+    async def detach_database_accounts_from_user_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.DetachDatabaseAccountsFromUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.detach_database_accounts_from_user_group_with_options_async(request, runtime)
+
     def detach_host_accounts_from_host_share_key_with_options(
         self,
         request: yundun_bastionhost_20191209_models.DetachHostAccountsFromHostShareKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.DetachHostAccountsFromHostShareKeyResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3285,14 +4599,92 @@
     async def disable_instance_public_access_async(
         self,
         request: yundun_bastionhost_20191209_models.DisableInstancePublicAccessRequest,
     ) -> yundun_bastionhost_20191209_models.DisableInstancePublicAccessResponse:
         runtime = util_models.RuntimeOptions()
         return await self.disable_instance_public_access_with_options_async(request, runtime)
 
+    def disable_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.DisableRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DisableRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DisableRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DisableRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def disable_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DisableRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.DisableRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DisableRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.DisableRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def disable_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.DisableRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.DisableRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.disable_rule_with_options(request, runtime)
+
+    async def disable_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.DisableRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.DisableRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.disable_rule_with_options_async(request, runtime)
+
     def enable_instance_public_access_with_options(
         self,
         request: yundun_bastionhost_20191209_models.EnableInstancePublicAccessRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.EnableInstancePublicAccessResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3359,14 +4751,346 @@
     async def enable_instance_public_access_async(
         self,
         request: yundun_bastionhost_20191209_models.EnableInstancePublicAccessRequest,
     ) -> yundun_bastionhost_20191209_models.EnableInstancePublicAccessResponse:
         runtime = util_models.RuntimeOptions()
         return await self.enable_instance_public_access_with_options_async(request, runtime)
 
+    def enable_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.EnableRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.EnableRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EnableRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.EnableRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def enable_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.EnableRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.EnableRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='EnableRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.EnableRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def enable_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.EnableRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.EnableRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.enable_rule_with_options(request, runtime)
+
+    async def enable_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.EnableRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.EnableRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.enable_rule_with_options_async(request, runtime)
+
+    def generate_asset_operation_token_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GenerateAssetOperationTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.asset_account_id):
+            query['AssetAccountId'] = request.asset_account_id
+        if not UtilClient.is_unset(request.asset_account_name):
+            query['AssetAccountName'] = request.asset_account_name
+        if not UtilClient.is_unset(request.asset_account_password):
+            query['AssetAccountPassword'] = request.asset_account_password
+        if not UtilClient.is_unset(request.asset_account_protocol_name):
+            query['AssetAccountProtocolName'] = request.asset_account_protocol_name
+        if not UtilClient.is_unset(request.asset_id):
+            query['AssetId'] = request.asset_id
+        if not UtilClient.is_unset(request.asset_type):
+            query['AssetType'] = request.asset_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GenerateAssetOperationToken',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def generate_asset_operation_token_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GenerateAssetOperationTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.asset_account_id):
+            query['AssetAccountId'] = request.asset_account_id
+        if not UtilClient.is_unset(request.asset_account_name):
+            query['AssetAccountName'] = request.asset_account_name
+        if not UtilClient.is_unset(request.asset_account_password):
+            query['AssetAccountPassword'] = request.asset_account_password
+        if not UtilClient.is_unset(request.asset_account_protocol_name):
+            query['AssetAccountProtocolName'] = request.asset_account_protocol_name
+        if not UtilClient.is_unset(request.asset_id):
+            query['AssetId'] = request.asset_id
+        if not UtilClient.is_unset(request.asset_type):
+            query['AssetType'] = request.asset_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GenerateAssetOperationToken',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def generate_asset_operation_token(
+        self,
+        request: yundun_bastionhost_20191209_models.GenerateAssetOperationTokenRequest,
+    ) -> yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.generate_asset_operation_token_with_options(request, runtime)
+
+    async def generate_asset_operation_token_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GenerateAssetOperationTokenRequest,
+    ) -> yundun_bastionhost_20191209_models.GenerateAssetOperationTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.generate_asset_operation_token_with_options_async(request, runtime)
+
+    def get_database_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_database_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetDatabaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_database(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_database_with_options(request, runtime)
+
+    async def get_database_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_database_with_options_async(request, runtime)
+
+    def get_database_account_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetDatabaseAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_database_account_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetDatabaseAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_database_account(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_database_account_with_options(request, runtime)
+
+    async def get_database_account_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.GetDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_database_account_with_options_async(request, runtime)
+
     def get_host_with_options(
         self,
         request: yundun_bastionhost_20191209_models.GetHostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetHostResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3677,15 +5401,18 @@
 
     def get_instance_adauth_server_with_options(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceADAuthServerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetInstanceADAuthServerResponse:
         """
-        The condition that is used to filter users.
+        ###
+        You can call this operation to query the settings of AD authentication on a bastion host. After you configure AD authentication on a bastion host, you can import AD-authenticated users into the bastion host. After the AD-authenticated users are imported into the bastion host, the AD-authenticated users can log on to the bastion host to perform O\\&M operations on servers.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceADAuthServerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceADAuthServerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3714,15 +5441,18 @@
 
     async def get_instance_adauth_server_with_options_async(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceADAuthServerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetInstanceADAuthServerResponse:
         """
-        The condition that is used to filter users.
+        ###
+        You can call this operation to query the settings of AD authentication on a bastion host. After you configure AD authentication on a bastion host, you can import AD-authenticated users into the bastion host. After the AD-authenticated users are imported into the bastion host, the AD-authenticated users can log on to the bastion host to perform O\\&M operations on servers.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceADAuthServerRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceADAuthServerResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3750,28 +5480,34 @@
         )
 
     def get_instance_adauth_server(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceADAuthServerRequest,
     ) -> yundun_bastionhost_20191209_models.GetInstanceADAuthServerResponse:
         """
-        The condition that is used to filter users.
+        ###
+        You can call this operation to query the settings of AD authentication on a bastion host. After you configure AD authentication on a bastion host, you can import AD-authenticated users into the bastion host. After the AD-authenticated users are imported into the bastion host, the AD-authenticated users can log on to the bastion host to perform O\\&M operations on servers.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceADAuthServerRequest
         @return: GetInstanceADAuthServerResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_instance_adauth_server_with_options(request, runtime)
 
     async def get_instance_adauth_server_async(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceADAuthServerRequest,
     ) -> yundun_bastionhost_20191209_models.GetInstanceADAuthServerResponse:
         """
-        The condition that is used to filter users.
+        ###
+        You can call this operation to query the settings of AD authentication on a bastion host. After you configure AD authentication on a bastion host, you can import AD-authenticated users into the bastion host. After the AD-authenticated users are imported into the bastion host, the AD-authenticated users can log on to the bastion host to perform O\\&M operations on servers.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceADAuthServerRequest
         @return: GetInstanceADAuthServerResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_adauth_server_with_options_async(request, runtime)
 
@@ -3851,17 +5587,17 @@
 
     def get_instance_two_factor_with_options(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceTwoFactorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetInstanceTwoFactorResponse:
         """
-        Indicates whether two-factor authentication is enabled. Valid values:
-        *   **true**: enabled
-        *   **false**: disabled
+        You can call this operation to query the settings of two-factor authentication on a bastion host. After you enable two-factor authentication, Bastionhost sends a verification code to a local user when the local user logs on to a bastion host. A local user can log on to the bastion host only when the local user enters the valid username and password and the verification code. This reduces the security risks caused by account information leaks.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceTwoFactorRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceTwoFactorResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3890,17 +5626,17 @@
 
     async def get_instance_two_factor_with_options_async(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceTwoFactorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetInstanceTwoFactorResponse:
         """
-        Indicates whether two-factor authentication is enabled. Valid values:
-        *   **true**: enabled
-        *   **false**: disabled
+        You can call this operation to query the settings of two-factor authentication on a bastion host. After you enable two-factor authentication, Bastionhost sends a verification code to a local user when the local user logs on to a bastion host. A local user can log on to the bastion host only when the local user enters the valid username and password and the verification code. This reduces the security risks caused by account information leaks.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceTwoFactorRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetInstanceTwoFactorResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3928,39 +5664,429 @@
         )
 
     def get_instance_two_factor(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceTwoFactorRequest,
     ) -> yundun_bastionhost_20191209_models.GetInstanceTwoFactorResponse:
         """
-        Indicates whether two-factor authentication is enabled. Valid values:
-        *   **true**: enabled
-        *   **false**: disabled
+        You can call this operation to query the settings of two-factor authentication on a bastion host. After you enable two-factor authentication, Bastionhost sends a verification code to a local user when the local user logs on to a bastion host. A local user can log on to the bastion host only when the local user enters the valid username and password and the verification code. This reduces the security risks caused by account information leaks.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceTwoFactorRequest
         @return: GetInstanceTwoFactorResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_instance_two_factor_with_options(request, runtime)
 
     async def get_instance_two_factor_async(
         self,
         request: yundun_bastionhost_20191209_models.GetInstanceTwoFactorRequest,
     ) -> yundun_bastionhost_20191209_models.GetInstanceTwoFactorResponse:
         """
-        Indicates whether two-factor authentication is enabled. Valid values:
-        *   **true**: enabled
-        *   **false**: disabled
+        You can call this operation to query the settings of two-factor authentication on a bastion host. After you enable two-factor authentication, Bastionhost sends a verification code to a local user when the local user logs on to a bastion host. A local user can log on to the bastion host only when the local user enters the valid username and password and the verification code. This reduces the security risks caused by account information leaks.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
         @param request: GetInstanceTwoFactorRequest
         @return: GetInstanceTwoFactorResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_instance_two_factor_with_options_async(request, runtime)
 
+    def get_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.GetNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.GetNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_network_domain_with_options(request, runtime)
+
+    async def get_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.GetNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_network_domain_with_options_async(request, runtime)
+
+    def get_policy_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_policy_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_policy(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_with_options(request, runtime)
+
+    async def get_policy_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_policy_with_options_async(request, runtime)
+
+    def get_policy_asset_scope_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyAssetScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicyAssetScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_policy_asset_scope_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyAssetScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicyAssetScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_policy_asset_scope(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyAssetScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_asset_scope_with_options(request, runtime)
+
+    async def get_policy_asset_scope_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyAssetScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyAssetScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_policy_asset_scope_with_options_async(request, runtime)
+
+    def get_policy_user_scope_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyUserScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicyUserScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_policy_user_scope_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyUserScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetPolicyUserScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_policy_user_scope(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyUserScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_user_scope_with_options(request, runtime)
+
+    async def get_policy_user_scope_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetPolicyUserScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.GetPolicyUserScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_policy_user_scope_with_options_async(request, runtime)
+
+    def get_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.GetRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.GetRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.GetRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.GetRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.GetRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_rule_with_options(request, runtime)
+
+    async def get_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.GetRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.GetRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_rule_with_options_async(request, runtime)
+
     def get_user_with_options(
         self,
         request: yundun_bastionhost_20191209_models.GetUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.GetUserResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -4191,14 +6317,594 @@
     async def list_approve_commands_async(
         self,
         request: yundun_bastionhost_20191209_models.ListApproveCommandsRequest,
     ) -> yundun_bastionhost_20191209_models.ListApproveCommandsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_approve_commands_with_options_async(request, runtime)
 
+    def list_database_accounts_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_database_accounts_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_database_accounts(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_with_options(request, runtime)
+
+    async def list_database_accounts_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_database_accounts_with_options_async(request, runtime)
+
+    def list_database_accounts_for_user_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccountsForUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_database_accounts_for_user_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccountsForUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_database_accounts_for_user(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_for_user_with_options(request, runtime)
+
+    async def list_database_accounts_for_user_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_database_accounts_for_user_with_options_async(request, runtime)
+
+    def list_database_accounts_for_user_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccountsForUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_database_accounts_for_user_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabaseAccountsForUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_database_accounts_for_user_group(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_for_user_group_with_options(request, runtime)
+
+    async def list_database_accounts_for_user_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabaseAccountsForUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_database_accounts_for_user_group_with_options_async(request, runtime)
+
+    def list_databases_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabases',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_databases_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabases',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_databases(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_with_options(request, runtime)
+
+    async def list_databases_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_databases_with_options_async(request, runtime)
+
+    def list_databases_for_user_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabasesForUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesForUserResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_databases_for_user_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_id):
+            query['UserId'] = request.user_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabasesForUser',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesForUserResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_databases_for_user(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_for_user_with_options(request, runtime)
+
+    async def list_databases_for_user_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_databases_for_user_with_options_async(request, runtime)
+
+    def list_databases_for_user_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabasesForUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_databases_for_user_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.user_group_id):
+            query['UserGroupId'] = request.user_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDatabasesForUserGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_databases_for_user_group(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_for_user_group_with_options(request, runtime)
+
+    async def list_databases_for_user_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListDatabasesForUserGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.ListDatabasesForUserGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_databases_for_user_group_with_options_async(request, runtime)
+
     def list_host_accounts_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ListHostAccountsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ListHostAccountsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5393,14 +8099,496 @@
     async def list_hosts_for_user_group_async(
         self,
         request: yundun_bastionhost_20191209_models.ListHostsForUserGroupRequest,
     ) -> yundun_bastionhost_20191209_models.ListHostsForUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_hosts_for_user_group_with_options_async(request, runtime)
 
+    def list_network_domains_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListNetworkDomainsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListNetworkDomainsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListNetworkDomains',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListNetworkDomainsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_network_domains_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListNetworkDomainsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListNetworkDomainsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListNetworkDomains',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListNetworkDomainsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_network_domains(
+        self,
+        request: yundun_bastionhost_20191209_models.ListNetworkDomainsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListNetworkDomainsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_network_domains_with_options(request, runtime)
+
+    async def list_network_domains_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListNetworkDomainsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListNetworkDomainsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_network_domains_with_options_async(request, runtime)
+
+    def list_operation_database_accounts_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationDatabaseAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_operation_database_accounts_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationDatabaseAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_operation_database_accounts(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_database_accounts_with_options(request, runtime)
+
+    async def list_operation_database_accounts_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabaseAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_operation_database_accounts_with_options_async(request, runtime)
+
+    def list_operation_databases_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabasesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabasesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_state):
+            query['SourceInstanceState'] = request.source_instance_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationDatabases',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationDatabasesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_operation_databases_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabasesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabasesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_address):
+            query['DatabaseAddress'] = request.database_address
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_type):
+            query['DatabaseType'] = request.database_type
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_state):
+            query['SourceInstanceState'] = request.source_instance_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationDatabases',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationDatabasesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_operation_databases(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabasesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabasesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_databases_with_options(request, runtime)
+
+    async def list_operation_databases_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationDatabasesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationDatabasesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_operation_databases_with_options_async(request, runtime)
+
+    def list_operation_host_accounts_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_account_name):
+            query['HostAccountName'] = request.host_account_name
+        if not UtilClient.is_unset(request.host_id):
+            query['HostId'] = request.host_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationHostAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_operation_host_accounts_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostAccountsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_account_name):
+            query['HostAccountName'] = request.host_account_name
+        if not UtilClient.is_unset(request.host_id):
+            query['HostId'] = request.host_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationHostAccounts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_operation_host_accounts(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_host_accounts_with_options(request, runtime)
+
+    async def list_operation_host_accounts_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostAccountsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostAccountsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_operation_host_accounts_with_options_async(request, runtime)
+
+    def list_operation_hosts_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_address):
+            query['HostAddress'] = request.host_address
+        if not UtilClient.is_unset(request.host_name):
+            query['HostName'] = request.host_name
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.ostype):
+            query['OSType'] = request.ostype
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_state):
+            query['SourceInstanceState'] = request.source_instance_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationHosts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationHostsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_operation_hosts_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostsResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_address):
+            query['HostAddress'] = request.host_address
+        if not UtilClient.is_unset(request.host_name):
+            query['HostName'] = request.host_name
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.ostype):
+            query['OSType'] = request.ostype
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source):
+            query['Source'] = request.source
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        if not UtilClient.is_unset(request.source_instance_state):
+            query['SourceInstanceState'] = request.source_instance_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListOperationHosts',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListOperationHostsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_operation_hosts(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_hosts_with_options(request, runtime)
+
+    async def list_operation_hosts_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListOperationHostsRequest,
+    ) -> yundun_bastionhost_20191209_models.ListOperationHostsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_operation_hosts_with_options_async(request, runtime)
+
     def list_operation_tickets_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ListOperationTicketsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ListOperationTicketsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5479,14 +8667,190 @@
     async def list_operation_tickets_async(
         self,
         request: yundun_bastionhost_20191209_models.ListOperationTicketsRequest,
     ) -> yundun_bastionhost_20191209_models.ListOperationTicketsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_operation_tickets_with_options_async(request, runtime)
 
+    def list_policies_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListPoliciesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListPoliciesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListPolicies',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListPoliciesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_policies_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListPoliciesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListPoliciesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListPolicies',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListPoliciesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_policies(
+        self,
+        request: yundun_bastionhost_20191209_models.ListPoliciesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListPoliciesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_policies_with_options(request, runtime)
+
+    async def list_policies_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListPoliciesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListPoliciesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_policies_with_options_async(request, runtime)
+
+    def list_rules_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ListRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.rule_state):
+            query['RuleState'] = request.rule_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListRules',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListRulesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_rules_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListRulesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ListRulesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.rule_state):
+            query['RuleState'] = request.rule_state
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListRules',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ListRulesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_rules(
+        self,
+        request: yundun_bastionhost_20191209_models.ListRulesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_rules_with_options(request, runtime)
+
+    async def list_rules_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ListRulesRequest,
+    ) -> yundun_bastionhost_20191209_models.ListRulesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_rules_with_options_async(request, runtime)
+
     def list_tag_keys_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ListTagKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ListTagKeysResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6045,14 +9409,214 @@
         
         @param request: LockUsersRequest
         @return: LockUsersResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.lock_users_with_options_async(request, runtime)
 
+    def modify_database_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.active_address_type):
+            query['ActiveAddressType'] = request.active_address_type
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_port):
+            query['DatabasePort'] = request.database_port
+        if not UtilClient.is_unset(request.database_private_address):
+            query['DatabasePrivateAddress'] = request.database_private_address
+        if not UtilClient.is_unset(request.database_public_address):
+            query['DatabasePublicAddress'] = request.database_public_address
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyDatabaseResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_database_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.active_address_type):
+            query['ActiveAddressType'] = request.active_address_type
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.database_id):
+            query['DatabaseId'] = request.database_id
+        if not UtilClient.is_unset(request.database_name):
+            query['DatabaseName'] = request.database_name
+        if not UtilClient.is_unset(request.database_port):
+            query['DatabasePort'] = request.database_port
+        if not UtilClient.is_unset(request.database_private_address):
+            query['DatabasePrivateAddress'] = request.database_private_address
+        if not UtilClient.is_unset(request.database_public_address):
+            query['DatabasePublicAddress'] = request.database_public_address
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.source_instance_id):
+            query['SourceInstanceId'] = request.source_instance_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDatabase',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyDatabaseResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_database(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_database_with_options(request, runtime)
+
+    async def modify_database_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_database_with_options_async(request, runtime)
+
+    def modify_database_account_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_schema):
+            query['DatabaseSchema'] = request.database_schema
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_database_account_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseAccountRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_account_id):
+            query['DatabaseAccountId'] = request.database_account_id
+        if not UtilClient.is_unset(request.database_account_name):
+            query['DatabaseAccountName'] = request.database_account_name
+        if not UtilClient.is_unset(request.database_schema):
+            query['DatabaseSchema'] = request.database_schema
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyDatabaseAccount',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_database_account(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_database_account_with_options(request, runtime)
+
+    async def modify_database_account_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyDatabaseAccountRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyDatabaseAccountResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_database_account_with_options_async(request, runtime)
+
     def modify_host_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ModifyHostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ModifyHostResponse:
         """
         You can call the ModifyHost operation to modify the basic information about a host in a data center, an Elastic Compute Service (ECS) instance, or a host in an ApsaraDB MyBase dedicated cluster.
@@ -7069,14 +10633,312 @@
     async def modify_instance_two_factor_async(
         self,
         request: yundun_bastionhost_20191209_models.ModifyInstanceTwoFactorRequest,
     ) -> yundun_bastionhost_20191209_models.ModifyInstanceTwoFactorResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_instance_two_factor_with_options_async(request, runtime)
 
+    def modify_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.proxies):
+            query['Proxies'] = request.proxies
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.network_domain_name):
+            query['NetworkDomainName'] = request.network_domain_name
+        if not UtilClient.is_unset(request.network_domain_type):
+            query['NetworkDomainType'] = request.network_domain_type
+        if not UtilClient.is_unset(request.proxies):
+            query['Proxies'] = request.proxies
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_network_domain_with_options(request, runtime)
+
+    async def modify_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_network_domain_with_options_async(request, runtime)
+
+    def modify_policy_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.priority):
+            query['Priority'] = request.priority
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyPolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyPolicyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_policy_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyPolicyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyPolicyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.policy_name):
+            query['PolicyName'] = request.policy_name
+        if not UtilClient.is_unset(request.priority):
+            query['Priority'] = request.priority
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyPolicy',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyPolicyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_policy(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyPolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_policy_with_options(request, runtime)
+
+    async def modify_policy_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyPolicyRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyPolicyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_policy_with_options_async(request, runtime)
+
+    def modify_rule_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.effective_end_time):
+            query['EffectiveEndTime'] = request.effective_end_time
+        if not UtilClient.is_unset(request.effective_start_time):
+            query['EffectiveStartTime'] = request.effective_start_time
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyRuleResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_rule_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyRuleRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyRuleResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.effective_end_time):
+            query['EffectiveEndTime'] = request.effective_end_time
+        if not UtilClient.is_unset(request.effective_start_time):
+            query['EffectiveStartTime'] = request.effective_start_time
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.rule_id):
+            query['RuleId'] = request.rule_id
+        if not UtilClient.is_unset(request.rule_name):
+            query['RuleName'] = request.rule_name
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyRule',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyRuleResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_rule(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_rule_with_options(request, runtime)
+
+    async def modify_rule_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyRuleRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyRuleResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_rule_with_options_async(request, runtime)
+
     def modify_user_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ModifyUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ModifyUserResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7285,14 +11147,268 @@
     async def modify_user_group_async(
         self,
         request: yundun_bastionhost_20191209_models.ModifyUserGroupRequest,
     ) -> yundun_bastionhost_20191209_models.ModifyUserGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_user_group_with_options_async(request, runtime)
 
+    def modify_user_public_key_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyUserPublicKeyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.public_key):
+            query['PublicKey'] = request.public_key
+        if not UtilClient.is_unset(request.public_key_id):
+            query['PublicKeyId'] = request.public_key_id
+        if not UtilClient.is_unset(request.public_key_name):
+            query['PublicKeyName'] = request.public_key_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyUserPublicKey',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_user_public_key_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyUserPublicKeyRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.public_key):
+            query['PublicKey'] = request.public_key
+        if not UtilClient.is_unset(request.public_key_id):
+            query['PublicKeyId'] = request.public_key_id
+        if not UtilClient.is_unset(request.public_key_name):
+            query['PublicKeyName'] = request.public_key_name
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyUserPublicKey',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_user_public_key(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyUserPublicKeyRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_user_public_key_with_options(request, runtime)
+
+    async def modify_user_public_key_async(
+        self,
+        request: yundun_bastionhost_20191209_models.ModifyUserPublicKeyRequest,
+    ) -> yundun_bastionhost_20191209_models.ModifyUserPublicKeyResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_user_public_key_with_options_async(request, runtime)
+
+    def move_databases_to_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MoveDatabasesToNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def move_databases_to_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MoveDatabasesToNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def move_databases_to_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.move_databases_to_network_domain_with_options(request, runtime)
+
+    async def move_databases_to_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.MoveDatabasesToNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.move_databases_to_network_domain_with_options_async(request, runtime)
+
+    def move_hosts_to_network_domain_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_ids):
+            query['HostIds'] = request.host_ids
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MoveHostsToNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def move_hosts_to_network_domain_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.host_ids):
+            query['HostIds'] = request.host_ids
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.network_domain_id):
+            query['NetworkDomainId'] = request.network_domain_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='MoveHostsToNetworkDomain',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def move_hosts_to_network_domain(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.move_hosts_to_network_domain_with_options(request, runtime)
+
+    async def move_hosts_to_network_domain_async(
+        self,
+        request: yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainRequest,
+    ) -> yundun_bastionhost_20191209_models.MoveHostsToNetworkDomainResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.move_hosts_to_network_domain_with_options_async(request, runtime)
+
     def move_resource_group_with_options(
         self,
         request: yundun_bastionhost_20191209_models.MoveResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.MoveResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7553,14 +11669,96 @@
         
         @param request: RejectOperationTicketRequest
         @return: RejectOperationTicketResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reject_operation_ticket_with_options_async(request, runtime)
 
+    def remove_databases_from_group_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RemoveDatabasesFromGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def remove_databases_from_group_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.database_ids):
+            query['DatabaseIds'] = request.database_ids
+        if not UtilClient.is_unset(request.host_group_id):
+            query['HostGroupId'] = request.host_group_id
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RemoveDatabasesFromGroup',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def remove_databases_from_group(
+        self,
+        request: yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.remove_databases_from_group_with_options(request, runtime)
+
+    async def remove_databases_from_group_async(
+        self,
+        request: yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupRequest,
+    ) -> yundun_bastionhost_20191209_models.RemoveDatabasesFromGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.remove_databases_from_group_with_options_async(request, runtime)
+
     def remove_hosts_from_group_with_options(
         self,
         request: yundun_bastionhost_20191209_models.RemoveHostsFromGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.RemoveHostsFromGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7751,14 +11949,92 @@
         
         @param request: RemoveUsersFromGroupRequest
         @return: RemoveUsersFromGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.remove_users_from_group_with_options_async(request, runtime)
 
+    def renew_asset_operation_token_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.RenewAssetOperationTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.token_id):
+            query['TokenId'] = request.token_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RenewAssetOperationToken',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def renew_asset_operation_token_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.RenewAssetOperationTokenRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.token_id):
+            query['TokenId'] = request.token_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RenewAssetOperationToken',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def renew_asset_operation_token(
+        self,
+        request: yundun_bastionhost_20191209_models.RenewAssetOperationTokenRequest,
+    ) -> yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.renew_asset_operation_token_with_options(request, runtime)
+
+    async def renew_asset_operation_token_async(
+        self,
+        request: yundun_bastionhost_20191209_models.RenewAssetOperationTokenRequest,
+    ) -> yundun_bastionhost_20191209_models.RenewAssetOperationTokenResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.renew_asset_operation_token_with_options_async(request, runtime)
+
     def reset_host_account_credential_with_options(
         self,
         request: yundun_bastionhost_20191209_models.ResetHostAccountCredentialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.ResetHostAccountCredentialResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7833,14 +12109,648 @@
     async def reset_host_account_credential_async(
         self,
         request: yundun_bastionhost_20191209_models.ResetHostAccountCredentialRequest,
     ) -> yundun_bastionhost_20191209_models.ResetHostAccountCredentialResponse:
         runtime = util_models.RuntimeOptions()
         return await self.reset_host_account_credential_with_options_async(request, runtime)
 
+    def set_policy_access_time_range_config_with_options(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.access_time_range_config):
+            request.access_time_range_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.access_time_range_config, 'AccessTimeRangeConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.access_time_range_config_shrink):
+            query['AccessTimeRangeConfig'] = request.access_time_range_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyAccessTimeRangeConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_access_time_range_config_with_options_async(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.access_time_range_config):
+            request.access_time_range_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.access_time_range_config, 'AccessTimeRangeConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.access_time_range_config_shrink):
+            query['AccessTimeRangeConfig'] = request.access_time_range_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyAccessTimeRangeConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_access_time_range_config(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_access_time_range_config_with_options(request, runtime)
+
+    async def set_policy_access_time_range_config_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAccessTimeRangeConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_access_time_range_config_with_options_async(request, runtime)
+
+    def set_policy_approval_config_with_options(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyApprovalConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyApprovalConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.approval_config):
+            request.approval_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.approval_config, 'ApprovalConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.approval_config_shrink):
+            query['ApprovalConfig'] = request.approval_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyApprovalConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_approval_config_with_options_async(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyApprovalConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyApprovalConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.approval_config):
+            request.approval_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.approval_config, 'ApprovalConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.approval_config_shrink):
+            query['ApprovalConfig'] = request.approval_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyApprovalConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_approval_config(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyApprovalConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_approval_config_with_options(request, runtime)
+
+    async def set_policy_approval_config_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyApprovalConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyApprovalConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_approval_config_with_options_async(request, runtime)
+
+    def set_policy_asset_scope_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAssetScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyAssetScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_asset_scope_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAssetScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.databases):
+            query['Databases'] = request.databases
+        if not UtilClient.is_unset(request.host_groups):
+            query['HostGroups'] = request.host_groups
+        if not UtilClient.is_unset(request.hosts):
+            query['Hosts'] = request.hosts
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyAssetScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_asset_scope(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAssetScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_asset_scope_with_options(request, runtime)
+
+    async def set_policy_asset_scope_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyAssetScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyAssetScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_asset_scope_with_options_async(request, runtime)
+
+    def set_policy_command_config_with_options(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyCommandConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyCommandConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.command_config):
+            request.command_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.command_config, 'CommandConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.command_config_shrink):
+            query['CommandConfig'] = request.command_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyCommandConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_command_config_with_options_async(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyCommandConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyCommandConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.command_config):
+            request.command_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.command_config, 'CommandConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.command_config_shrink):
+            query['CommandConfig'] = request.command_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyCommandConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_command_config(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyCommandConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_command_config_with_options(request, runtime)
+
+    async def set_policy_command_config_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyCommandConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyCommandConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_command_config_with_options_async(request, runtime)
+
+    def set_policy_ipacl_config_with_options(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyIPAclConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyIPAclConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.ipacl_config):
+            request.ipacl_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ipacl_config, 'IPAclConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.ipacl_config_shrink):
+            query['IPAclConfig'] = request.ipacl_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyIPAclConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_ipacl_config_with_options_async(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyIPAclConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyIPAclConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.ipacl_config):
+            request.ipacl_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.ipacl_config, 'IPAclConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.ipacl_config_shrink):
+            query['IPAclConfig'] = request.ipacl_config_shrink
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyIPAclConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_ipacl_config(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyIPAclConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_ipacl_config_with_options(request, runtime)
+
+    async def set_policy_ipacl_config_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyIPAclConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyIPAclConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_ipacl_config_with_options_async(request, runtime)
+
+    def set_policy_protocol_config_with_options(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyProtocolConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyProtocolConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.protocol_config):
+            request.protocol_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.protocol_config, 'ProtocolConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.protocol_config_shrink):
+            query['ProtocolConfig'] = request.protocol_config_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyProtocolConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_protocol_config_with_options_async(
+        self,
+        tmp_req: yundun_bastionhost_20191209_models.SetPolicyProtocolConfigRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse:
+        UtilClient.validate_model(tmp_req)
+        request = yundun_bastionhost_20191209_models.SetPolicyProtocolConfigShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.protocol_config):
+            request.protocol_config_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.protocol_config, 'ProtocolConfig', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.protocol_config_shrink):
+            query['ProtocolConfig'] = request.protocol_config_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyProtocolConfig',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_protocol_config(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyProtocolConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_protocol_config_with_options(request, runtime)
+
+    async def set_policy_protocol_config_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyProtocolConfigRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyProtocolConfigResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_protocol_config_with_options_async(request, runtime)
+
+    def set_policy_user_scope_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyUserScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyUserScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def set_policy_user_scope_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyUserScopeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.policy_id):
+            query['PolicyId'] = request.policy_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.scope_type):
+            query['ScopeType'] = request.scope_type
+        if not UtilClient.is_unset(request.user_group_ids):
+            query['UserGroupIds'] = request.user_group_ids
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SetPolicyUserScope',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def set_policy_user_scope(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyUserScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_user_scope_with_options(request, runtime)
+
+    async def set_policy_user_scope_async(
+        self,
+        request: yundun_bastionhost_20191209_models.SetPolicyUserScopeRequest,
+    ) -> yundun_bastionhost_20191209_models.SetPolicyUserScopeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.set_policy_user_scope_with_options_async(request, runtime)
+
     def start_instance_with_options(
         self,
         request: yundun_bastionhost_20191209_models.StartInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> yundun_bastionhost_20191209_models.StartInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -8194,7 +13104,223 @@
 
     async def untag_resources_async(
         self,
         request: yundun_bastionhost_20191209_models.UntagResourcesRequest,
     ) -> yundun_bastionhost_20191209_models.UntagResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
+
+    def verify_instance_adauth_server_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account):
+            query['Account'] = request.account
+        if not UtilClient.is_unset(request.base_dn):
+            query['BaseDN'] = request.base_dn
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.is_ssl):
+            query['IsSSL'] = request.is_ssl
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.port):
+            query['Port'] = request.port
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.server):
+            query['Server'] = request.server
+        if not UtilClient.is_unset(request.standby_server):
+            query['StandbyServer'] = request.standby_server
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyInstanceADAuthServer',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def verify_instance_adauth_server_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account):
+            query['Account'] = request.account
+        if not UtilClient.is_unset(request.base_dn):
+            query['BaseDN'] = request.base_dn
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.is_ssl):
+            query['IsSSL'] = request.is_ssl
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.port):
+            query['Port'] = request.port
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.server):
+            query['Server'] = request.server
+        if not UtilClient.is_unset(request.standby_server):
+            query['StandbyServer'] = request.standby_server
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyInstanceADAuthServer',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def verify_instance_adauth_server(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerRequest,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.verify_instance_adauth_server_with_options(request, runtime)
+
+    async def verify_instance_adauth_server_async(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerRequest,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceADAuthServerResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.verify_instance_adauth_server_with_options_async(request, runtime)
+
+    def verify_instance_ldapauth_server_with_options(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account):
+            query['Account'] = request.account
+        if not UtilClient.is_unset(request.base_dn):
+            query['BaseDN'] = request.base_dn
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.is_ssl):
+            query['IsSSL'] = request.is_ssl
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.port):
+            query['Port'] = request.port
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.server):
+            query['Server'] = request.server
+        if not UtilClient.is_unset(request.standby_server):
+            query['StandbyServer'] = request.standby_server
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyInstanceLDAPAuthServer',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def verify_instance_ldapauth_server_with_options_async(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.account):
+            query['Account'] = request.account
+        if not UtilClient.is_unset(request.base_dn):
+            query['BaseDN'] = request.base_dn
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.is_ssl):
+            query['IsSSL'] = request.is_ssl
+        if not UtilClient.is_unset(request.password):
+            query['Password'] = request.password
+        if not UtilClient.is_unset(request.port):
+            query['Port'] = request.port
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.server):
+            query['Server'] = request.server
+        if not UtilClient.is_unset(request.standby_server):
+            query['StandbyServer'] = request.standby_server
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='VerifyInstanceLDAPAuthServer',
+            version='2019-12-09',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def verify_instance_ldapauth_server(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerRequest,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.verify_instance_ldapauth_server_with_options(request, runtime)
+
+    async def verify_instance_ldapauth_server_async(
+        self,
+        request: yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerRequest,
+    ) -> yundun_bastionhost_20191209_models.VerifyInstanceLDAPAuthServerResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.verify_instance_ldapauth_server_with_options_async(request, runtime)
```

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209/models.py` & `alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -248,14 +248,186 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AcceptOperationTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AddDatabasesToGroupRequest(TeaModel):
+    def __init__(
+        self,
+        database_ids: List[str] = None,
+        host_group_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_ids = database_ids
+        self.host_group_id = host_group_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_ids is not None:
+            result['DatabaseIds'] = self.database_ids
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseIds') is not None:
+            self.database_ids = m.get('DatabaseIds')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class AddDatabasesToGroupResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_id: str = None,
+        host_group_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_id = database_id
+        self.host_group_id = host_group_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class AddDatabasesToGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[AddDatabasesToGroupResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = AddDatabasesToGroupResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class AddDatabasesToGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AddDatabasesToGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AddDatabasesToGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AddHostsToGroupRequest(TeaModel):
     def __init__(
         self,
         host_group_id: str = None,
         host_ids: str = None,
         instance_id: str = None,
         region_id: str = None,
@@ -660,14 +832,546 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddUsersToGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AttachDatabaseAccountsToUserRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class AttachDatabaseAccountsToUserRequest(TeaModel):
+    def __init__(
+        self,
+        databases: List[AttachDatabaseAccountsToUserRequestDatabases] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        self.databases = databases
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.user_id = user_id
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = AttachDatabaseAccountsToUserRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class AttachDatabaseAccountsToUserResponseBodyResultsDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_account_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_account_id = database_account_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class AttachDatabaseAccountsToUserResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_accounts: List[AttachDatabaseAccountsToUserResponseBodyResultsDatabaseAccounts] = None,
+        database_id: str = None,
+        message: str = None,
+        user_id: str = None,
+    ):
+        self.code = code
+        self.database_accounts = database_accounts
+        self.database_id = database_id
+        self.message = message
+        self.user_id = user_id
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = AttachDatabaseAccountsToUserResponseBodyResultsDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class AttachDatabaseAccountsToUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[AttachDatabaseAccountsToUserResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = AttachDatabaseAccountsToUserResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class AttachDatabaseAccountsToUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AttachDatabaseAccountsToUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AttachDatabaseAccountsToUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        databases: List[AttachDatabaseAccountsToUserGroupRequestDatabases] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        self.databases = databases
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = AttachDatabaseAccountsToUserGroupRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupResponseBodyResultsDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_account_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_account_id = database_account_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_accounts: List[AttachDatabaseAccountsToUserGroupResponseBodyResultsDatabaseAccounts] = None,
+        database_id: str = None,
+        message: str = None,
+        user_group_id: str = None,
+    ):
+        self.code = code
+        self.database_accounts = database_accounts
+        self.database_id = database_id
+        self.message = message
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = AttachDatabaseAccountsToUserGroupResponseBodyResultsDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[AttachDatabaseAccountsToUserGroupResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = AttachDatabaseAccountsToUserGroupResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: AttachDatabaseAccountsToUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = AttachDatabaseAccountsToUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class AttachHostAccountsToHostShareKeyRequest(TeaModel):
     def __init__(
         self,
         host_account_ids: str = None,
         host_share_key_id: str = None,
         instance_id: str = None,
         region_id: str = None,
@@ -2027,19 +2731,19 @@
 class ConfigInstanceWhiteListRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         white_list: List[str] = None,
     ):
-        # The ID of the bastion host for which a whitelist of public IP addresses is configured.
+        # The ID of the bastion host for which you want to configure a whitelist of public IP addresses.
         self.instance_id = instance_id
-        # Configures a whitelist of public IP addresses for a bastion host.
+        # The region ID of the bastion host.
         self.region_id = region_id
-        # ConfigInstanceWhiteList
+        # The public IP addresses that you want to add to the whitelist.
         self.white_list = white_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2068,15 +2772,17 @@
 
 class ConfigInstanceWhiteListResponseBody(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         request_id: str = None,
     ):
+        # The ID of the bastion host for which a whitelist of public IP addresses is configured.
         self.instance_id = instance_id
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2136,14 +2842,330 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ConfigInstanceWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDatabaseRequest(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        polar_dbendpoint_type: str = None,
+        region_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_region_id: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.polar_dbendpoint_type = polar_dbendpoint_type
+        self.region_id = region_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_region_id = source_instance_region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.polar_dbendpoint_type is not None:
+            result['PolarDBEndpointType'] = self.polar_dbendpoint_type
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_region_id is not None:
+            result['SourceInstanceRegionId'] = self.source_instance_region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('PolarDBEndpointType') is not None:
+            self.polar_dbendpoint_type = m.get('PolarDBEndpointType')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceRegionId') is not None:
+            self.source_instance_region_id = m.get('SourceInstanceRegionId')
+        return self
+
+
+class CreateDatabaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_id: str = None,
+        request_id: str = None,
+    ):
+        self.database_id = database_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatabaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDatabaseResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateDatabaseAccountRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_name: str = None,
+        database_id: str = None,
+        database_schema: str = None,
+        instance_id: str = None,
+        login_attribute: str = None,
+        password: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.database_schema = database_schema
+        self.instance_id = instance_id
+        self.login_attribute = login_attribute
+        self.password = password
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_schema is not None:
+            result['DatabaseSchema'] = self.database_schema
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.login_attribute is not None:
+            result['LoginAttribute'] = self.login_attribute
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseSchema') is not None:
+            self.database_schema = m.get('DatabaseSchema')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('LoginAttribute') is not None:
+            self.login_attribute = m.get('LoginAttribute')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class CreateDatabaseAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        request_id: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatabaseAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateDatabaseAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateDatabaseAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateHostRequest(TeaModel):
     def __init__(
         self,
         active_address_type: str = None,
         comment: str = None,
         host_name: str = None,
         host_private_address: str = None,
@@ -2352,46 +3374,46 @@
         instance_id: str = None,
         pass_phrase: str = None,
         password: str = None,
         private_key: str = None,
         protocol_name: str = None,
         region_id: str = None,
     ):
+        # The name of the host account.
+        self.host_account_name = host_account_name
+        # The ID of the host to which you want to add a host account.
+        # 
+        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        self.host_id = host_id
+        # The ID of the shared key.
+        self.host_share_key_id = host_share_key_id
+        # The ID of the bastion host in which you want to add a host account to the host.
+        # 
+        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
         # The passphrase of the private key for the host account.
         # 
         # >  You can specify this parameter when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter.
-        self.host_account_name = host_account_name
-        # The ID of the shared key.
-        self.host_id = host_id
+        self.pass_phrase = pass_phrase
+        # The password of the host account.
+        self.password = password
+        # The private key of the host account. The value is a Base64-encoded string.
+        # 
+        # >  This parameter takes effect only when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter. You can configure a password and a private key for the host account at the same time. If both a password and a private key are configured for the host account, Bastionhost preferentially uses the private key to log on to the host.
+        self.private_key = private_key
         # The protocol of the host to which you want to add a host account.
         # 
         # Valid values:
         # 
         # *   SSH
         # *   RDP
-        self.host_share_key_id = host_share_key_id
-        # master
-        self.instance_id = instance_id
-        # The private key of the host account. The value is a Base64-encoded string.
-        # 
-        # >  This parameter takes effect only when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter. You can configure a password and a private key for the host account at the same time. If both a password and a private key are configured for the host account, Bastionhost preferentially uses the private key to log on to the host.
-        self.pass_phrase = pass_phrase
+        self.protocol_name = protocol_name
         # The region ID of the bastion host in which you want to add a host account to the host.
         # 
         # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.password = password
-        # The ID of the host to which you want to add a host account.
-        # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
-        self.private_key = private_key
-        # The ID of the bastion host in which you want to add a host account to the host.
-        # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
-        self.protocol_name = protocol_name
-        # The password of the host account.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2444,17 +3466,17 @@
 
 class CreateHostAccountResponseBody(TeaModel):
     def __init__(
         self,
         host_account_id: str = None,
         request_id: str = None,
     ):
-        # The ID of the request.
-        self.host_account_id = host_account_id
         # The operation that you want to perform. Set the value to **CreateHostAccount**.
+        self.host_account_id = host_account_id
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2532,17 +3554,15 @@
         self.host_group_name = host_group_name
         # The ID of the bastion host on which you want to create a host group.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
         # The region ID of the bastion host on which you want to create a host group.
         # 
-        # **\
-        # 
-        # **For more information about the mapping between region IDs and region names, see **Regions and zones[.](~~40654~~)
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2777,14 +3797,621 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateHostShareKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateNetworkDomainRequestProxies(TeaModel):
+    def __init__(
+        self,
+        address: str = None,
+        node_type: str = None,
+        password: str = None,
+        port: int = None,
+        proxy_type: str = None,
+        user: str = None,
+    ):
+        self.address = address
+        self.node_type = node_type
+        self.password = password
+        self.port = port
+        self.proxy_type = proxy_type
+        self.user = user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.address is not None:
+            result['Address'] = self.address
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.proxy_type is not None:
+            result['ProxyType'] = self.proxy_type
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Address') is not None:
+            self.address = m.get('Address')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('ProxyType') is not None:
+            self.proxy_type = m.get('ProxyType')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class CreateNetworkDomainRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        instance_id: str = None,
+        network_domain_name: str = None,
+        network_domain_type: str = None,
+        proxies: List[CreateNetworkDomainRequestProxies] = None,
+        region_id: str = None,
+    ):
+        self.comment = comment
+        self.instance_id = instance_id
+        self.network_domain_name = network_domain_name
+        self.network_domain_type = network_domain_type
+        self.proxies = proxies
+        self.region_id = region_id
+
+    def validate(self):
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_name is not None:
+            result['NetworkDomainName'] = self.network_domain_name
+        if self.network_domain_type is not None:
+            result['NetworkDomainType'] = self.network_domain_type
+        result['Proxies'] = []
+        if self.proxies is not None:
+            for k in self.proxies:
+                result['Proxies'].append(k.to_map() if k else None)
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainName') is not None:
+            self.network_domain_name = m.get('NetworkDomainName')
+        if m.get('NetworkDomainType') is not None:
+            self.network_domain_type = m.get('NetworkDomainType')
+        self.proxies = []
+        if m.get('Proxies') is not None:
+            for k in m.get('Proxies'):
+                temp_model = CreateNetworkDomainRequestProxies()
+                self.proxies.append(temp_model.from_map(k))
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class CreateNetworkDomainResponseBody(TeaModel):
+    def __init__(
+        self,
+        network_domain_id: str = None,
+        request_id: str = None,
+    ):
+        self.network_domain_id = network_domain_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateNetworkDomainResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateNetworkDomainResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreatePolicyRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        instance_id: str = None,
+        policy_name: str = None,
+        priority: str = None,
+        region_id: str = None,
+    ):
+        self.comment = comment
+        self.instance_id = instance_id
+        self.policy_name = policy_name
+        self.priority = priority
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.priority is not None:
+            result['Priority'] = self.priority
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Priority') is not None:
+            self.priority = m.get('Priority')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class CreatePolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        policy_id: str = None,
+        request_id: str = None,
+    ):
+        self.policy_id = policy_id
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreatePolicyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreatePolicyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreatePolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class CreateRuleRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class CreateRuleRequestHostGroups(TeaModel):
+    def __init__(
+        self,
+        host_account_names: List[str] = None,
+        host_group_id: str = None,
+    ):
+        self.host_account_names = host_account_names
+        self.host_group_id = host_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_names is not None:
+            result['HostAccountNames'] = self.host_account_names
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class CreateRuleRequestHosts(TeaModel):
+    def __init__(
+        self,
+        host_account_ids: List[str] = None,
+        host_id: str = None,
+    ):
+        self.host_account_ids = host_account_ids
+        self.host_id = host_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_ids is not None:
+            result['HostAccountIds'] = self.host_account_ids
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class CreateRuleRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        databases: List[CreateRuleRequestDatabases] = None,
+        effective_end_time: int = None,
+        effective_start_time: int = None,
+        host_groups: List[CreateRuleRequestHostGroups] = None,
+        hosts: List[CreateRuleRequestHosts] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_name: str = None,
+        user_group_ids: List[str] = None,
+        user_ids: List[str] = None,
+    ):
+        self.comment = comment
+        self.databases = databases
+        self.effective_end_time = effective_end_time
+        self.effective_start_time = effective_start_time
+        self.host_groups = host_groups
+        self.hosts = hosts
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.rule_name = rule_name
+        self.user_group_ids = user_group_ids
+        self.user_ids = user_ids
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+        if self.host_groups:
+            for k in self.host_groups:
+                if k:
+                    k.validate()
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.effective_end_time is not None:
+            result['EffectiveEndTime'] = self.effective_end_time
+        if self.effective_start_time is not None:
+            result['EffectiveStartTime'] = self.effective_start_time
+        result['HostGroups'] = []
+        if self.host_groups is not None:
+            for k in self.host_groups:
+                result['HostGroups'].append(k.to_map() if k else None)
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.user_group_ids is not None:
+            result['UserGroupIds'] = self.user_group_ids
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = CreateRuleRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('EffectiveEndTime') is not None:
+            self.effective_end_time = m.get('EffectiveEndTime')
+        if m.get('EffectiveStartTime') is not None:
+            self.effective_start_time = m.get('EffectiveStartTime')
+        self.host_groups = []
+        if m.get('HostGroups') is not None:
+            for k in m.get('HostGroups'):
+                temp_model = CreateRuleRequestHostGroups()
+                self.host_groups.append(temp_model.from_map(k))
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = CreateRuleRequestHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('UserGroupIds') is not None:
+            self.user_group_ids = m.get('UserGroupIds')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class CreateRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        rule_id: str = None,
+    ):
+        self.request_id = request_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class CreateRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateUserRequest(TeaModel):
     def __init__(
         self,
         comment: str = None,
         display_name: str = None,
         effective_end_time: int = None,
         effective_start_time: int = None,
@@ -3318,14 +4945,228 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateUserPublicKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteDatabaseRequest(TeaModel):
+    def __init__(
+        self,
+        database_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteDatabaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatabaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteDatabaseResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteDatabaseAccountRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteDatabaseAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatabaseAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteDatabaseAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteDatabaseAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteHostRequest(TeaModel):
     def __init__(
         self,
         host_id: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
@@ -3782,14 +5623,335 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHostShareKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteNetworkDomainRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeleteNetworkDomainResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteNetworkDomainResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteNetworkDomainResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeletePolicyRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class DeletePolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeletePolicyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeletePolicyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeletePolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DeleteRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class DeleteRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         user_id: str = None,
     ):
@@ -4021,17 +6183,17 @@
 class DeleteUserPublicKeyRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         public_key_id: str = None,
         region_id: str = None,
     ):
-        # The region ID of the bastion host on which you want to delete the public key from the user.
+        # The ID of the Bastionhost instance to which the users to be queried belong.
         # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
         self.instance_id = instance_id
         # The ID of the public key.
         self.public_key_id = public_key_id
         # The region ID of the bastion host. For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
@@ -4851,17 +7013,21 @@
 
 class DescribeRegionsRequest(TeaModel):
     def __init__(
         self,
         accept_language: str = None,
         region_id: str = None,
     ):
-        # The ID of the region.
+        # The natural language in which responses are returned. Valid values:
+        # 
+        # *   **zh-CN**: Chinese. This is the default value.
+        # *   **en-US**: English.
+        # *   **ja**: Japanese.
         self.accept_language = accept_language
-        # The ID of request.
+        # The ID of the region.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4887,16 +7053,19 @@
 class DescribeRegionsResponseBodyRegions(TeaModel):
     def __init__(
         self,
         local_name: str = None,
         region_endpoint: str = None,
         region_id: str = None,
     ):
+        # The name of the region.
         self.local_name = local_name
+        # The endpoint of the region.
         self.region_endpoint = region_endpoint
+        # The ID of the region.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4925,17 +7094,17 @@
 
 class DescribeRegionsResponseBody(TeaModel):
     def __init__(
         self,
         regions: List[DescribeRegionsResponseBodyRegions] = None,
         request_id: str = None,
     ):
-        # DescribeRegions
+        # The information about regions where you can create bastion hosts.
         self.regions = regions
-        # Queries available regions where you can create bastion hosts.
+        # The ID of request.
         self.request_id = request_id
 
     def validate(self):
         if self.regions:
             for k in self.regions:
                 if k:
                     k.validate()
@@ -5003,14 +7172,546 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DetachDatabaseAccountsFromUserRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserRequest(TeaModel):
+    def __init__(
+        self,
+        databases: List[DetachDatabaseAccountsFromUserRequestDatabases] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        self.databases = databases
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.user_id = user_id
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = DetachDatabaseAccountsFromUserRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserResponseBodyResultsDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_account_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_account_id = database_account_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class DetachDatabaseAccountsFromUserResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_accounts: List[DetachDatabaseAccountsFromUserResponseBodyResultsDatabaseAccounts] = None,
+        database_id: str = None,
+        message: str = None,
+        user_id: str = None,
+    ):
+        self.code = code
+        self.database_accounts = database_accounts
+        self.database_id = database_id
+        self.message = message
+        self.user_id = user_id
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = DetachDatabaseAccountsFromUserResponseBodyResultsDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[DetachDatabaseAccountsFromUserResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = DetachDatabaseAccountsFromUserResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class DetachDatabaseAccountsFromUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DetachDatabaseAccountsFromUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DetachDatabaseAccountsFromUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        databases: List[DetachDatabaseAccountsFromUserGroupRequestDatabases] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        self.databases = databases
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = DetachDatabaseAccountsFromUserGroupRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupResponseBodyResultsDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_account_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_account_id = database_account_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_accounts: List[DetachDatabaseAccountsFromUserGroupResponseBodyResultsDatabaseAccounts] = None,
+        database_id: str = None,
+        message: str = None,
+        user_group_id: str = None,
+    ):
+        self.code = code
+        self.database_accounts = database_accounts
+        self.database_id = database_id
+        self.message = message
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = DetachDatabaseAccountsFromUserGroupResponseBodyResultsDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[DetachDatabaseAccountsFromUserGroupResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = DetachDatabaseAccountsFromUserGroupResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DetachDatabaseAccountsFromUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DetachDatabaseAccountsFromUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DetachHostAccountsFromHostShareKeyRequest(TeaModel):
     def __init__(
         self,
         host_account_ids: str = None,
         host_share_key_id: str = None,
         instance_id: str = None,
         region_id: str = None,
@@ -6336,14 +9037,121 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DisableInstancePublicAccessResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DisableRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class DisableRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DisableRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DisableRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DisableRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class EnableInstancePublicAccessRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
         # The ID of the bastion host.
@@ -6449,14 +9257,709 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableInstancePublicAccessResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class EnableRuleRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.rule_id = rule_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class EnableRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class EnableRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: EnableRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = EnableRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GenerateAssetOperationTokenRequest(TeaModel):
+    def __init__(
+        self,
+        asset_account_id: str = None,
+        asset_account_name: str = None,
+        asset_account_password: str = None,
+        asset_account_protocol_name: str = None,
+        asset_id: str = None,
+        asset_type: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.asset_account_id = asset_account_id
+        self.asset_account_name = asset_account_name
+        self.asset_account_password = asset_account_password
+        self.asset_account_protocol_name = asset_account_protocol_name
+        self.asset_id = asset_id
+        self.asset_type = asset_type
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.asset_account_id is not None:
+            result['AssetAccountId'] = self.asset_account_id
+        if self.asset_account_name is not None:
+            result['AssetAccountName'] = self.asset_account_name
+        if self.asset_account_password is not None:
+            result['AssetAccountPassword'] = self.asset_account_password
+        if self.asset_account_protocol_name is not None:
+            result['AssetAccountProtocolName'] = self.asset_account_protocol_name
+        if self.asset_id is not None:
+            result['AssetId'] = self.asset_id
+        if self.asset_type is not None:
+            result['AssetType'] = self.asset_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AssetAccountId') is not None:
+            self.asset_account_id = m.get('AssetAccountId')
+        if m.get('AssetAccountName') is not None:
+            self.asset_account_name = m.get('AssetAccountName')
+        if m.get('AssetAccountPassword') is not None:
+            self.asset_account_password = m.get('AssetAccountPassword')
+        if m.get('AssetAccountProtocolName') is not None:
+            self.asset_account_protocol_name = m.get('AssetAccountProtocolName')
+        if m.get('AssetId') is not None:
+            self.asset_id = m.get('AssetId')
+        if m.get('AssetType') is not None:
+            self.asset_type = m.get('AssetType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GenerateAssetOperationTokenResponseBodyAssetOperationToken(TeaModel):
+    def __init__(
+        self,
+        count_left: int = None,
+        expire_time: int = None,
+        has_count_limit: bool = None,
+        max_renew_count: int = None,
+        renew_count: int = None,
+        token: str = None,
+        token_id: str = None,
+    ):
+        self.count_left = count_left
+        self.expire_time = expire_time
+        self.has_count_limit = has_count_limit
+        self.max_renew_count = max_renew_count
+        self.renew_count = renew_count
+        self.token = token
+        self.token_id = token_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.count_left is not None:
+            result['CountLeft'] = self.count_left
+        if self.expire_time is not None:
+            result['ExpireTime'] = self.expire_time
+        if self.has_count_limit is not None:
+            result['HasCountLimit'] = self.has_count_limit
+        if self.max_renew_count is not None:
+            result['MaxRenewCount'] = self.max_renew_count
+        if self.renew_count is not None:
+            result['RenewCount'] = self.renew_count
+        if self.token is not None:
+            result['Token'] = self.token
+        if self.token_id is not None:
+            result['TokenId'] = self.token_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CountLeft') is not None:
+            self.count_left = m.get('CountLeft')
+        if m.get('ExpireTime') is not None:
+            self.expire_time = m.get('ExpireTime')
+        if m.get('HasCountLimit') is not None:
+            self.has_count_limit = m.get('HasCountLimit')
+        if m.get('MaxRenewCount') is not None:
+            self.max_renew_count = m.get('MaxRenewCount')
+        if m.get('RenewCount') is not None:
+            self.renew_count = m.get('RenewCount')
+        if m.get('Token') is not None:
+            self.token = m.get('Token')
+        if m.get('TokenId') is not None:
+            self.token_id = m.get('TokenId')
+        return self
+
+
+class GenerateAssetOperationTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        asset_operation_token: GenerateAssetOperationTokenResponseBodyAssetOperationToken = None,
+        request_id: str = None,
+    ):
+        self.asset_operation_token = asset_operation_token
+        self.request_id = request_id
+
+    def validate(self):
+        if self.asset_operation_token:
+            self.asset_operation_token.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.asset_operation_token is not None:
+            result['AssetOperationToken'] = self.asset_operation_token.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AssetOperationToken') is not None:
+            temp_model = GenerateAssetOperationTokenResponseBodyAssetOperationToken()
+            self.asset_operation_token = temp_model.from_map(m['AssetOperationToken'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GenerateAssetOperationTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GenerateAssetOperationTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GenerateAssetOperationTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetDatabaseRequest(TeaModel):
+    def __init__(
+        self,
+        database_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetDatabaseResponseBodyDatabase(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        network_domain_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_region_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.network_domain_id = network_domain_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_region_id = source_instance_region_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_region_id is not None:
+            result['SourceInstanceRegionId'] = self.source_instance_region_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceRegionId') is not None:
+            self.source_instance_region_id = m.get('SourceInstanceRegionId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class GetDatabaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        database: GetDatabaseResponseBodyDatabase = None,
+        request_id: str = None,
+    ):
+        self.database = database
+        self.request_id = request_id
+
+    def validate(self):
+        if self.database:
+            self.database.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database is not None:
+            result['Database'] = self.database.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Database') is not None:
+            temp_model = GetDatabaseResponseBodyDatabase()
+            self.database = temp_model.from_map(m['Database'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetDatabaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDatabaseResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetDatabaseAccountRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class GetDatabaseAccountResponseBodyDatabaseAccount(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_schema: str = None,
+        has_password: bool = None,
+        login_attribute: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_schema = database_schema
+        self.has_password = has_password
+        self.login_attribute = login_attribute
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_schema is not None:
+            result['DatabaseSchema'] = self.database_schema
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        if self.login_attribute is not None:
+            result['LoginAttribute'] = self.login_attribute
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseSchema') is not None:
+            self.database_schema = m.get('DatabaseSchema')
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        if m.get('LoginAttribute') is not None:
+            self.login_attribute = m.get('LoginAttribute')
+        return self
+
+
+class GetDatabaseAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_account: GetDatabaseAccountResponseBodyDatabaseAccount = None,
+        request_id: str = None,
+    ):
+        self.database_account = database_account
+        self.request_id = request_id
+
+    def validate(self):
+        if self.database_account:
+            self.database_account.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account is not None:
+            result['DatabaseAccount'] = self.database_account.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccount') is not None:
+            temp_model = GetDatabaseAccountResponseBodyDatabaseAccount()
+            self.database_account = temp_model.from_map(m['DatabaseAccount'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetDatabaseAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDatabaseAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetDatabaseAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetHostRequest(TeaModel):
     def __init__(
         self,
         host_id: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
@@ -6964,23 +10467,25 @@
 class GetHostGroupRequest(TeaModel):
     def __init__(
         self,
         host_group_id: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
-        # The region ID of the Bastionhost instance where you want to query the host group.
+        # The ID of the host group.
         # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
         self.host_group_id = host_group_id
-        # MyHostGroup
+        # The ID of the bastion host in which you want to query the details of the host group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The ID of the Bastionhost instance where you want to query the host group.
+        # The region ID of the bastion host in which you want to query the details of the host group.
         # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7010,19 +10515,19 @@
 class GetHostGroupResponseBodyHostGroup(TeaModel):
     def __init__(
         self,
         comment: str = None,
         host_group_id: str = None,
         host_group_name: str = None,
     ):
-        # The details of the host group returned.
-        self.comment = comment
         # The description of the host group.
-        self.host_group_id = host_group_id
+        self.comment = comment
         # The ID of the host group.
+        self.host_group_id = host_group_id
+        # The name of the host group.
         self.host_group_name = host_group_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7051,19 +10556,17 @@
 
 class GetHostGroupResponseBody(TeaModel):
     def __init__(
         self,
         host_group: GetHostGroupResponseBodyHostGroup = None,
         request_id: str = None,
     ):
-        # The ID of the host group that you want to query.
-        # 
-        # >  You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        # The details of the host group returned.
         self.host_group = host_group
-        # my host group.
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.host_group:
             self.host_group.validate()
 
     def to_map(self):
@@ -7297,20 +10800,19 @@
 
 class GetInstanceADAuthServerRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
-        # The field that is used to indicate the email address of a user on the AD server.
+        # The ID of the bastion host. You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # Indicates whether passwords are required. Valid values:
+        # The region ID of the bastion host.
         # 
-        # *   **true**: required
-        # *   **false**: not required
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7345,37 +10847,43 @@
         is_ssl: bool = None,
         mobile_mapping: str = None,
         name_mapping: str = None,
         port: int = None,
         server: str = None,
         standby_server: str = None,
     ):
-        # The port that is used to access the AD server.
+        # The distinguished name (DN) of the AD server account.
         self.account = account
-        # The ID of the bastion host to query.
-        # 
-        # You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        # The Base DN of the AD server.
         self.base_dn = base_dn
-        # The settings of AD authentication.
+        # The domain on the AD server.
         self.domain = domain
-        # The address of the secondary AD server.
+        # The field that is used to indicate the email address of a user on the AD server.
         self.email_mapping = email_mapping
-        # The field that is used to indicate the mobile phone number of a user on the AD server.
+        # The condition that is used to filter users.
         self.filter = filter
-        # The address of the AD server.
+        # Indicates whether passwords are required. Valid values:
+        # 
+        # *   **true**:
+        # *   **false**\
         self.has_password = has_password
-        # The Base DN of the AD server.
+        # Indicates whether SSL is supported. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.is_ssl = is_ssl
-        # The field that is used to indicate the name of a user on the AD server.
+        # The field that is used to indicate the mobile phone number of a user on the AD server.
         self.mobile_mapping = mobile_mapping
-        # The ID of the request, which is used to locate and troubleshoot issues.
+        # The field that is used to indicate the name of a user on the AD server.
         self.name_mapping = name_mapping
-        # Queries the settings of Active Directory (AD) authentication on a bastion host.
+        # The port that is used to access the AD server.
         self.port = port
+        # The address of the LDAP server.
         self.server = server
+        # The address of the secondary LDAP server.
         self.standby_server = standby_server
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7440,20 +10948,17 @@
 
 class GetInstanceADAuthServerResponseBody(TeaModel):
     def __init__(
         self,
         ad: GetInstanceADAuthServerResponseBodyAD = None,
         request_id: str = None,
     ):
-        # The operation that you want to perform. Set the value to **GetInstanceADAuthServer**.
+        # The settings of AD authentication.
         self.ad = ad
-        # Indicates whether SSL is supported. Valid values:
-        # 
-        # *   **true**: supported
-        # *   **false**: not supported
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id
 
     def validate(self):
         if self.ad:
             self.ad.validate()
 
     def to_map(self):
@@ -7744,17 +11249,21 @@
 
 class GetInstanceTwoFactorRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
     ):
-        # The ID of the request, which is used to locate and troubleshoot issues.
+        # The ID of the bastion host.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The operation that you want to perform. Set the value to **GetInstanceTwoFactor**.
+        # The region ID of the bastion host.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7780,17 +11289,24 @@
 class GetInstanceTwoFactorResponseBodyConfig(TeaModel):
     def __init__(
         self,
         enable_two_factor: bool = None,
         skip_two_factor_time: int = None,
         two_factor_methods: List[str] = None,
     ):
-        # Queries the settings of two-factor authentication on a bastion host.
+        # Indicates whether two-factor authentication is enabled. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.enable_two_factor = enable_two_factor
+        # The duration within which two-factor authentication is not required after a local user passes two-factor authentication. Valid values: `0 to 168`. Unit: hours.
+        # 
+        # > If 0 is returned, a local user must pass two-factor authentication every time the local user logs on to the bastion host.
         self.skip_two_factor_time = skip_two_factor_time
+        # The two-factor authentication methods.
         self.two_factor_methods = two_factor_methods
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7821,17 +11337,15 @@
     def __init__(
         self,
         config: GetInstanceTwoFactorResponseBodyConfig = None,
         request_id: str = None,
     ):
         # The settings of two-factor authentication.
         self.config = config
-        # The duration within which two-factor authentication is not required after a local user passes two-factor authentication. Valid values: `0 to 168`. Unit: hours.
-        # 
-        # >  If 0 is returned, a local user must pass two-factor authentication every time the local user logs on to the bastion host.
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id
 
     def validate(self):
         if self.config:
             self.config.validate()
 
     def to_map(self):
@@ -7893,275 +11407,228 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetInstanceTwoFactorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetUserRequest(TeaModel):
+class GetNetworkDomainRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
+        network_domain_id: str = None,
         region_id: str = None,
-        user_id: str = None,
     ):
-        # The ID of the bastion host on which you want to query the user.
-        # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The region ID of the bastion host on which you want to query the user.
-        # 
-        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.network_domain_id = network_domain_id
         self.region_id = region_id
-        # The ID of the user.
-        # 
-        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
-        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
         return self
 
 
-class GetUserResponseBodyUser(TeaModel):
+class GetNetworkDomainResponseBodyNetworkDomainProxies(TeaModel):
+    def __init__(
+        self,
+        address: str = None,
+        has_password: bool = None,
+        node_type: str = None,
+        port: int = None,
+        proxy_state: str = None,
+        proxy_state_error_code: str = None,
+        proxy_type: str = None,
+        user: str = None,
+    ):
+        self.address = address
+        self.has_password = has_password
+        self.node_type = node_type
+        self.port = port
+        self.proxy_state = proxy_state
+        self.proxy_state_error_code = proxy_state_error_code
+        self.proxy_type = proxy_type
+        self.user = user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.address is not None:
+            result['Address'] = self.address
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.proxy_state is not None:
+            result['ProxyState'] = self.proxy_state
+        if self.proxy_state_error_code is not None:
+            result['ProxyStateErrorCode'] = self.proxy_state_error_code
+        if self.proxy_type is not None:
+            result['ProxyType'] = self.proxy_type
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Address') is not None:
+            self.address = m.get('Address')
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('ProxyState') is not None:
+            self.proxy_state = m.get('ProxyState')
+        if m.get('ProxyStateErrorCode') is not None:
+            self.proxy_state_error_code = m.get('ProxyStateErrorCode')
+        if m.get('ProxyType') is not None:
+            self.proxy_type = m.get('ProxyType')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class GetNetworkDomainResponseBodyNetworkDomain(TeaModel):
     def __init__(
         self,
         comment: str = None,
-        display_name: str = None,
-        effective_end_time: int = None,
-        effective_start_time: int = None,
-        email: str = None,
-        language: str = None,
-        language_status: str = None,
-        mobile: str = None,
-        mobile_country_code: str = None,
-        need_reset_password: bool = None,
-        source: str = None,
-        source_user_id: str = None,
-        two_factor_methods: List[str] = None,
-        two_factor_status: str = None,
-        user_id: str = None,
-        user_name: str = None,
-        user_state: List[str] = None,
+        default: bool = None,
+        network_domain_id: str = None,
+        network_domain_name: str = None,
+        network_domain_type: str = None,
+        proxies: List[GetNetworkDomainResponseBodyNetworkDomainProxies] = None,
     ):
-        # The description of the user.
         self.comment = comment
-        # The display name of the user.
-        self.display_name = display_name
-        # The end of the validity period of the user. The value is a UNIX timestamp. Unit: seconds.
-        self.effective_end_time = effective_end_time
-        # The beginning of the validity period of the user. The value is a UNIX timestamp. Unit: seconds.
-        self.effective_start_time = effective_start_time
-        # The email address of the user.
-        self.email = email
-        self.language = language
-        self.language_status = language_status
-        # The mobile phone number of the user.
-        self.mobile = mobile
-        # The location in which the mobile number of the user is registered. Valid values:
-        # 
-        # *   **CN**: the Chinese mainland, whose country calling code is +86
-        # *   **HK**: Hong Kong (China), whose country calling code is +852
-        # *   **MO**: Macao (China), whose country calling code is +853
-        # *   **TW**: Taiwan (China), whose country calling code is +886
-        # *   **RU**: Russia, whose country calling code is +7
-        # *   **SG**: Singapore, whose country calling code is +65
-        # *   **MY**: Malaysia, whose country calling code is +60
-        # *   **ID**: Indonesia, whose country calling code is +62
-        # *   **DE**: Germany, whose country calling code is +49
-        # *   **AU**: Australia, whose country calling code is +61
-        # *   **US**: US, whose country calling code is +1
-        # *   **AE**: United Arab Emirates, whose country calling code is +971
-        # *   **JP:** Japan, whose country calling code is +81
-        # *   **GB**: UK, whose country calling code is +44
-        # *   **IN**: India, whose country calling code is +91
-        # *   **KR**: Republic of Korea, whose country calling code is +82
-        # *   **PH**: Philippines, whose country calling code is +63
-        # *   **CH**: Switzerland, whose country calling code is +41
-        # *   **SE**: Sweden, whose country calling code is +46
-        self.mobile_country_code = mobile_country_code
-        # Specifies whether password reset is required upon the next logon. Valid values:
-        # 
-        # *   **true**: yes
-        # *   **false**: no
-        self.need_reset_password = need_reset_password
-        # The source of the user. Valid values:
-        # 
-        # *   **Local**: a local user
-        # *   **Ram**: a RAM user
-        self.source = source
-        # The unique ID of the user.
-        # 
-        # > This parameter uniquely identifies a RAM user of the bastion host. A value is returned for this parameter if the **Source** parameter is set to **Ram**. No value is returned for this parameter if the **Source** parameter is set to **Local**.
-        self.source_user_id = source_user_id
-        # An array that consists of the details of the two-factor authentication method.
-        self.two_factor_methods = two_factor_methods
-        # The two-factor authentication status of the user. Valid values:
-        # 
-        # *   **Global**: The global settings are used.
-        # *   **Disable**: The two-factor authentication is disabled.
-        # *   **Enable**: The two-factor authentication is enabled and the user-specific setting is used.
-        self.two_factor_status = two_factor_status
-        # The ID of the user.
-        self.user_id = user_id
-        # The logon name of the user.
-        self.user_name = user_name
-        # An array that consists of the details of the user status.
-        self.user_state = user_state
+        self.default = default
+        self.network_domain_id = network_domain_id
+        self.network_domain_name = network_domain_name
+        self.network_domain_type = network_domain_type
+        self.proxies = proxies
 
     def validate(self):
-        pass
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.comment is not None:
             result['Comment'] = self.comment
-        if self.display_name is not None:
-            result['DisplayName'] = self.display_name
-        if self.effective_end_time is not None:
-            result['EffectiveEndTime'] = self.effective_end_time
-        if self.effective_start_time is not None:
-            result['EffectiveStartTime'] = self.effective_start_time
-        if self.email is not None:
-            result['Email'] = self.email
-        if self.language is not None:
-            result['Language'] = self.language
-        if self.language_status is not None:
-            result['LanguageStatus'] = self.language_status
-        if self.mobile is not None:
-            result['Mobile'] = self.mobile
-        if self.mobile_country_code is not None:
-            result['MobileCountryCode'] = self.mobile_country_code
-        if self.need_reset_password is not None:
-            result['NeedResetPassword'] = self.need_reset_password
-        if self.source is not None:
-            result['Source'] = self.source
-        if self.source_user_id is not None:
-            result['SourceUserId'] = self.source_user_id
-        if self.two_factor_methods is not None:
-            result['TwoFactorMethods'] = self.two_factor_methods
-        if self.two_factor_status is not None:
-            result['TwoFactorStatus'] = self.two_factor_status
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
-        if self.user_name is not None:
-            result['UserName'] = self.user_name
-        if self.user_state is not None:
-            result['UserState'] = self.user_state
+        if self.default is not None:
+            result['Default'] = self.default
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.network_domain_name is not None:
+            result['NetworkDomainName'] = self.network_domain_name
+        if self.network_domain_type is not None:
+            result['NetworkDomainType'] = self.network_domain_type
+        result['Proxies'] = []
+        if self.proxies is not None:
+            for k in self.proxies:
+                result['Proxies'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Comment') is not None:
             self.comment = m.get('Comment')
-        if m.get('DisplayName') is not None:
-            self.display_name = m.get('DisplayName')
-        if m.get('EffectiveEndTime') is not None:
-            self.effective_end_time = m.get('EffectiveEndTime')
-        if m.get('EffectiveStartTime') is not None:
-            self.effective_start_time = m.get('EffectiveStartTime')
-        if m.get('Email') is not None:
-            self.email = m.get('Email')
-        if m.get('Language') is not None:
-            self.language = m.get('Language')
-        if m.get('LanguageStatus') is not None:
-            self.language_status = m.get('LanguageStatus')
-        if m.get('Mobile') is not None:
-            self.mobile = m.get('Mobile')
-        if m.get('MobileCountryCode') is not None:
-            self.mobile_country_code = m.get('MobileCountryCode')
-        if m.get('NeedResetPassword') is not None:
-            self.need_reset_password = m.get('NeedResetPassword')
-        if m.get('Source') is not None:
-            self.source = m.get('Source')
-        if m.get('SourceUserId') is not None:
-            self.source_user_id = m.get('SourceUserId')
-        if m.get('TwoFactorMethods') is not None:
-            self.two_factor_methods = m.get('TwoFactorMethods')
-        if m.get('TwoFactorStatus') is not None:
-            self.two_factor_status = m.get('TwoFactorStatus')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
-        if m.get('UserName') is not None:
-            self.user_name = m.get('UserName')
-        if m.get('UserState') is not None:
-            self.user_state = m.get('UserState')
+        if m.get('Default') is not None:
+            self.default = m.get('Default')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('NetworkDomainName') is not None:
+            self.network_domain_name = m.get('NetworkDomainName')
+        if m.get('NetworkDomainType') is not None:
+            self.network_domain_type = m.get('NetworkDomainType')
+        self.proxies = []
+        if m.get('Proxies') is not None:
+            for k in m.get('Proxies'):
+                temp_model = GetNetworkDomainResponseBodyNetworkDomainProxies()
+                self.proxies.append(temp_model.from_map(k))
         return self
 
 
-class GetUserResponseBody(TeaModel):
+class GetNetworkDomainResponseBody(TeaModel):
     def __init__(
         self,
+        network_domain: GetNetworkDomainResponseBodyNetworkDomain = None,
         request_id: str = None,
-        user: GetUserResponseBodyUser = None,
     ):
-        # The ID of the request.
+        self.network_domain = network_domain
         self.request_id = request_id
-        # The details of the user that was queried.
-        self.user = user
 
     def validate(self):
-        if self.user:
-            self.user.validate()
+        if self.network_domain:
+            self.network_domain.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.network_domain is not None:
+            result['NetworkDomain'] = self.network_domain.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.user is not None:
-            result['User'] = self.user.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('NetworkDomain') is not None:
+            temp_model = GetNetworkDomainResponseBodyNetworkDomain()
+            self.network_domain = temp_model.from_map(m['NetworkDomain'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('User') is not None:
-            temp_model = GetUserResponseBodyUser()
-            self.user = temp_model.from_map(m['User'])
         return self
 
 
-class GetUserResponse(TeaModel):
+class GetNetworkDomainResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: GetUserResponseBody = None,
+        body: GetNetworkDomainResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         if self.body:
@@ -8184,627 +11651,578 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = GetUserResponseBody()
+            temp_model = GetNetworkDomainResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class GetUserGroupRequest(TeaModel):
+class GetPolicyRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
+        policy_id: str = None,
         region_id: str = None,
-        user_group_id: str = None,
     ):
-        # The ID of the request.
         self.instance_id = instance_id
-        # The name of the user group.
+        self.policy_id = policy_id
         self.region_id = region_id
-        # All Bastionhost API requests must include common request parameters. For more information about common request parameters, see [Common parameters](~~315526~~).
-        # 
-        # For more information about sample requests, see the "Examples" section of this topic.
-        self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
         return self
 
 
-class GetUserGroupResponseBodyUserGroup(TeaModel):
+class GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime(TeaModel):
     def __init__(
         self,
-        comment: str = None,
-        user_group_id: str = None,
-        user_group_name: str = None,
+        days: List[str] = None,
+        hours: List[str] = None,
     ):
-        # GetUserGroup
-        self.comment = comment
-        self.user_group_id = user_group_id
-        # WB662865
-        self.user_group_name = user_group_name
+        self.days = days
+        self.hours = hours
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.comment is not None:
-            result['Comment'] = self.comment
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
-        if self.user_group_name is not None:
-            result['UserGroupName'] = self.user_group_name
+        if self.days is not None:
+            result['Days'] = self.days
+        if self.hours is not None:
+            result['Hours'] = self.hours
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('Comment') is not None:
-            self.comment = m.get('Comment')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
-        if m.get('UserGroupName') is not None:
-            self.user_group_name = m.get('UserGroupName')
+        if m.get('Days') is not None:
+            self.days = m.get('Days')
+        if m.get('Hours') is not None:
+            self.hours = m.get('Hours')
         return self
 
 
-class GetUserGroupResponseBody(TeaModel):
+class GetPolicyResponseBodyPolicyAccessTimeRangeConfig(TeaModel):
     def __init__(
         self,
-        request_id: str = None,
-        user_group: GetUserGroupResponseBodyUserGroup = None,
+        effective_time: List[GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime] = None,
     ):
-        # Queries the details of a specified user group in a specified Bastionhost instance.
-        self.request_id = request_id
-        # GetUserGroup
-        self.user_group = user_group
+        self.effective_time = effective_time
 
     def validate(self):
-        if self.user_group:
-            self.user_group.validate()
+        if self.effective_time:
+            for k in self.effective_time:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.user_group is not None:
-            result['UserGroup'] = self.user_group.to_map()
+        result['EffectiveTime'] = []
+        if self.effective_time is not None:
+            for k in self.effective_time:
+                result['EffectiveTime'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('UserGroup') is not None:
-            temp_model = GetUserGroupResponseBodyUserGroup()
-            self.user_group = temp_model.from_map(m['UserGroup'])
+        self.effective_time = []
+        if m.get('EffectiveTime') is not None:
+            for k in m.get('EffectiveTime'):
+                temp_model = GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime()
+                self.effective_time.append(temp_model.from_map(k))
         return self
 
 
-class GetUserGroupResponse(TeaModel):
+class GetPolicyResponseBodyPolicyApprovalConfig(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: GetUserGroupResponseBody = None,
+        switch_status: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.switch_status = switch_status
 
     def validate(self):
-        if self.body:
-            self.body.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.switch_status is not None:
+            result['SwitchStatus'] = self.switch_status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = GetUserGroupResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('SwitchStatus') is not None:
+            self.switch_status = m.get('SwitchStatus')
         return self
 
 
-class ListApproveCommandsRequest(TeaModel):
+class GetPolicyResponseBodyPolicyCommandConfigApproval(TeaModel):
     def __init__(
         self,
-        instance_id: str = None,
-        page_number: str = None,
-        page_size: str = None,
-        region_id: str = None,
+        commands: List[str] = None,
     ):
-        self.instance_id = instance_id
-        self.page_number = page_number
-        self.page_size = page_size
-        self.region_id = region_id
+        self.commands = commands
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
+        if self.commands is not None:
+            result['Commands'] = self.commands
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
         return self
 
 
-class ListApproveCommandsResponseBodyApproveCommands(TeaModel):
+class GetPolicyResponseBodyPolicyCommandConfigDeny(TeaModel):
     def __init__(
         self,
-        approve_command_id: str = None,
-        asset_account_name: str = None,
-        asset_ip: str = None,
-        asset_name: str = None,
-        client_ip: str = None,
-        client_user: str = None,
-        command: str = None,
-        create_time: str = None,
-        protocol_name: str = None,
-        session_id: str = None,
-        state: str = None,
+        acl_type: str = None,
+        commands: List[str] = None,
     ):
-        self.approve_command_id = approve_command_id
-        self.asset_account_name = asset_account_name
-        self.asset_ip = asset_ip
-        self.asset_name = asset_name
-        self.client_ip = client_ip
-        self.client_user = client_user
-        self.command = command
-        self.create_time = create_time
-        self.protocol_name = protocol_name
-        self.session_id = session_id
-        self.state = state
+        self.acl_type = acl_type
+        self.commands = commands
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.approve_command_id is not None:
-            result['ApproveCommandId'] = self.approve_command_id
-        if self.asset_account_name is not None:
-            result['AssetAccountName'] = self.asset_account_name
-        if self.asset_ip is not None:
-            result['AssetIp'] = self.asset_ip
-        if self.asset_name is not None:
-            result['AssetName'] = self.asset_name
-        if self.client_ip is not None:
-            result['ClientIp'] = self.client_ip
-        if self.client_user is not None:
-            result['ClientUser'] = self.client_user
-        if self.command is not None:
-            result['Command'] = self.command
-        if self.create_time is not None:
-            result['CreateTime'] = self.create_time
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
-        if self.session_id is not None:
-            result['SessionId'] = self.session_id
-        if self.state is not None:
-            result['State'] = self.state
+        if self.acl_type is not None:
+            result['AclType'] = self.acl_type
+        if self.commands is not None:
+            result['Commands'] = self.commands
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('ApproveCommandId') is not None:
-            self.approve_command_id = m.get('ApproveCommandId')
-        if m.get('AssetAccountName') is not None:
-            self.asset_account_name = m.get('AssetAccountName')
-        if m.get('AssetIp') is not None:
-            self.asset_ip = m.get('AssetIp')
-        if m.get('AssetName') is not None:
-            self.asset_name = m.get('AssetName')
-        if m.get('ClientIp') is not None:
-            self.client_ip = m.get('ClientIp')
-        if m.get('ClientUser') is not None:
-            self.client_user = m.get('ClientUser')
-        if m.get('Command') is not None:
-            self.command = m.get('Command')
-        if m.get('CreateTime') is not None:
-            self.create_time = m.get('CreateTime')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
-        if m.get('SessionId') is not None:
-            self.session_id = m.get('SessionId')
-        if m.get('State') is not None:
-            self.state = m.get('State')
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
         return self
 
 
-class ListApproveCommandsResponseBody(TeaModel):
+class GetPolicyResponseBodyPolicyCommandConfig(TeaModel):
     def __init__(
         self,
-        approve_commands: List[ListApproveCommandsResponseBodyApproveCommands] = None,
-        request_id: str = None,
-        total_count: int = None,
+        approval: GetPolicyResponseBodyPolicyCommandConfigApproval = None,
+        deny: GetPolicyResponseBodyPolicyCommandConfigDeny = None,
     ):
-        self.approve_commands = approve_commands
-        self.request_id = request_id
-        self.total_count = total_count
+        self.approval = approval
+        self.deny = deny
 
     def validate(self):
-        if self.approve_commands:
-            for k in self.approve_commands:
-                if k:
-                    k.validate()
+        if self.approval:
+            self.approval.validate()
+        if self.deny:
+            self.deny.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['ApproveCommands'] = []
-        if self.approve_commands is not None:
-            for k in self.approve_commands:
-                result['ApproveCommands'].append(k.to_map() if k else None)
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
+        if self.approval is not None:
+            result['Approval'] = self.approval.to_map()
+        if self.deny is not None:
+            result['Deny'] = self.deny.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.approve_commands = []
-        if m.get('ApproveCommands') is not None:
-            for k in m.get('ApproveCommands'):
-                temp_model = ListApproveCommandsResponseBodyApproveCommands()
-                self.approve_commands.append(temp_model.from_map(k))
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
+        if m.get('Approval') is not None:
+            temp_model = GetPolicyResponseBodyPolicyCommandConfigApproval()
+            self.approval = temp_model.from_map(m['Approval'])
+        if m.get('Deny') is not None:
+            temp_model = GetPolicyResponseBodyPolicyCommandConfigDeny()
+            self.deny = temp_model.from_map(m['Deny'])
         return self
 
 
-class ListApproveCommandsResponse(TeaModel):
+class GetPolicyResponseBodyPolicyIPAclConfig(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListApproveCommandsResponseBody = None,
+        acl_type: str = None,
+        ips: List[str] = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.acl_type = acl_type
+        self.ips = ips
 
     def validate(self):
-        if self.body:
-            self.body.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.acl_type is not None:
+            result['AclType'] = self.acl_type
+        if self.ips is not None:
+            result['IPs'] = self.ips
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = ListApproveCommandsResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('IPs') is not None:
+            self.ips = m.get('IPs')
         return self
 
 
-class ListHostAccountsRequest(TeaModel):
+class GetPolicyResponseBodyPolicyProtocolConfigRDP(TeaModel):
     def __init__(
         self,
-        host_account_name: str = None,
-        host_id: str = None,
-        instance_id: str = None,
-        page_number: str = None,
-        page_size: str = None,
-        protocol_name: str = None,
-        region_id: str = None,
+        clipboard_download: str = None,
+        clipboard_upload: str = None,
+        disk_redirection: str = None,
+        record_keyboard: str = None,
     ):
-        # Indicates whether a password is configured for the host account.
-        # 
-        # Valid values:
-        # 
-        # *   true: A password is configured for the host account.
-        # *   false: No passwords are configured for the host account.
-        self.host_account_name = host_account_name
-        # The protocol used by the host whose accounts you want to query.
-        # 
-        # Valid values:
-        # 
-        # *   SSH
-        # *   RDP
-        self.host_id = host_id
-        # The ID of the shared key.
-        self.instance_id = instance_id
-        # The operation that you want to perform.
-        # 
-        # Set the value to **ListHostAccounts**.
-        self.page_number = page_number
-        # The number of entries to return on each page.
-        # 
-        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
-        # 
-        # >  We recommend that you do not leave this parameter empty.
-        self.page_size = page_size
-        # The name of the host account that you want to query. The name can be up to 128 characters in length. Only exact match is supported.
-        self.protocol_name = protocol_name
-        # The ID of the specified host whose accounts you want to query.
-        # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
-        self.region_id = region_id
+        self.clipboard_download = clipboard_download
+        self.clipboard_upload = clipboard_upload
+        self.disk_redirection = disk_redirection
+        self.record_keyboard = record_keyboard
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
+        if self.clipboard_download is not None:
+            result['ClipboardDownload'] = self.clipboard_download
+        if self.clipboard_upload is not None:
+            result['ClipboardUpload'] = self.clipboard_upload
+        if self.disk_redirection is not None:
+            result['DiskRedirection'] = self.disk_redirection
+        if self.record_keyboard is not None:
+            result['RecordKeyboard'] = self.record_keyboard
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
+        if m.get('ClipboardDownload') is not None:
+            self.clipboard_download = m.get('ClipboardDownload')
+        if m.get('ClipboardUpload') is not None:
+            self.clipboard_upload = m.get('ClipboardUpload')
+        if m.get('DiskRedirection') is not None:
+            self.disk_redirection = m.get('DiskRedirection')
+        if m.get('RecordKeyboard') is not None:
+            self.record_keyboard = m.get('RecordKeyboard')
         return self
 
 
-class ListHostAccountsResponseBodyHostAccounts(TeaModel):
+class GetPolicyResponseBodyPolicyProtocolConfigSSH(TeaModel):
     def __init__(
         self,
-        has_password: bool = None,
-        host_account_id: str = None,
-        host_account_name: str = None,
-        host_id: str = None,
-        host_share_key_id: str = None,
-        host_share_key_name: str = None,
-        private_key_fingerprint: str = None,
-        protocol_name: str = None,
+        exec_command: str = None,
+        sftpchannel: str = None,
+        sftpdownload_file: str = None,
+        sftpmkdir: str = None,
+        sftpremove_file: str = None,
+        sftprename_file: str = None,
+        sftprmdir: str = None,
+        sftpupload_file: str = None,
+        sshchannel: str = None,
+        x_11forwarding: str = None,
     ):
-        # The fingerprint of the private key for the host account.
-        self.has_password = has_password
-        # The ID of the request.
-        self.host_account_id = host_account_id
-        # The name of the shared key.
-        self.host_account_name = host_account_name
-        self.host_id = host_id
-        self.host_share_key_id = host_share_key_id
-        self.host_share_key_name = host_share_key_name
-        # The protocol that is used by the host.
-        # 
-        # Valid values:
-        # 
-        # *   SSH
-        # *   RDP
-        self.private_key_fingerprint = private_key_fingerprint
-        # The number of the page to return. Default value: **1**.
-        self.protocol_name = protocol_name
+        self.exec_command = exec_command
+        self.sftpchannel = sftpchannel
+        self.sftpdownload_file = sftpdownload_file
+        self.sftpmkdir = sftpmkdir
+        self.sftpremove_file = sftpremove_file
+        self.sftprename_file = sftprename_file
+        self.sftprmdir = sftprmdir
+        self.sftpupload_file = sftpupload_file
+        self.sshchannel = sshchannel
+        self.x_11forwarding = x_11forwarding
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.has_password is not None:
-            result['HasPassword'] = self.has_password
-        if self.host_account_id is not None:
-            result['HostAccountId'] = self.host_account_id
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
-        if self.host_share_key_id is not None:
-            result['HostShareKeyId'] = self.host_share_key_id
-        if self.host_share_key_name is not None:
-            result['HostShareKeyName'] = self.host_share_key_name
-        if self.private_key_fingerprint is not None:
-            result['PrivateKeyFingerprint'] = self.private_key_fingerprint
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
+        if self.exec_command is not None:
+            result['ExecCommand'] = self.exec_command
+        if self.sftpchannel is not None:
+            result['SFTPChannel'] = self.sftpchannel
+        if self.sftpdownload_file is not None:
+            result['SFTPDownloadFile'] = self.sftpdownload_file
+        if self.sftpmkdir is not None:
+            result['SFTPMkdir'] = self.sftpmkdir
+        if self.sftpremove_file is not None:
+            result['SFTPRemoveFile'] = self.sftpremove_file
+        if self.sftprename_file is not None:
+            result['SFTPRenameFile'] = self.sftprename_file
+        if self.sftprmdir is not None:
+            result['SFTPRmdir'] = self.sftprmdir
+        if self.sftpupload_file is not None:
+            result['SFTPUploadFile'] = self.sftpupload_file
+        if self.sshchannel is not None:
+            result['SSHChannel'] = self.sshchannel
+        if self.x_11forwarding is not None:
+            result['X11Forwarding'] = self.x_11forwarding
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HasPassword') is not None:
-            self.has_password = m.get('HasPassword')
-        if m.get('HostAccountId') is not None:
-            self.host_account_id = m.get('HostAccountId')
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
-        if m.get('HostShareKeyId') is not None:
-            self.host_share_key_id = m.get('HostShareKeyId')
-        if m.get('HostShareKeyName') is not None:
-            self.host_share_key_name = m.get('HostShareKeyName')
-        if m.get('PrivateKeyFingerprint') is not None:
-            self.private_key_fingerprint = m.get('PrivateKeyFingerprint')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
+        if m.get('ExecCommand') is not None:
+            self.exec_command = m.get('ExecCommand')
+        if m.get('SFTPChannel') is not None:
+            self.sftpchannel = m.get('SFTPChannel')
+        if m.get('SFTPDownloadFile') is not None:
+            self.sftpdownload_file = m.get('SFTPDownloadFile')
+        if m.get('SFTPMkdir') is not None:
+            self.sftpmkdir = m.get('SFTPMkdir')
+        if m.get('SFTPRemoveFile') is not None:
+            self.sftpremove_file = m.get('SFTPRemoveFile')
+        if m.get('SFTPRenameFile') is not None:
+            self.sftprename_file = m.get('SFTPRenameFile')
+        if m.get('SFTPRmdir') is not None:
+            self.sftprmdir = m.get('SFTPRmdir')
+        if m.get('SFTPUploadFile') is not None:
+            self.sftpupload_file = m.get('SFTPUploadFile')
+        if m.get('SSHChannel') is not None:
+            self.sshchannel = m.get('SSHChannel')
+        if m.get('X11Forwarding') is not None:
+            self.x_11forwarding = m.get('X11Forwarding')
         return self
 
 
-class ListHostAccountsResponseBody(TeaModel):
+class GetPolicyResponseBodyPolicyProtocolConfig(TeaModel):
     def __init__(
         self,
-        host_accounts: List[ListHostAccountsResponseBodyHostAccounts] = None,
+        rdp: GetPolicyResponseBodyPolicyProtocolConfigRDP = None,
+        ssh: GetPolicyResponseBodyPolicyProtocolConfigSSH = None,
+    ):
+        self.rdp = rdp
+        self.ssh = ssh
+
+    def validate(self):
+        if self.rdp:
+            self.rdp.validate()
+        if self.ssh:
+            self.ssh.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.rdp is not None:
+            result['RDP'] = self.rdp.to_map()
+        if self.ssh is not None:
+            result['SSH'] = self.ssh.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RDP') is not None:
+            temp_model = GetPolicyResponseBodyPolicyProtocolConfigRDP()
+            self.rdp = temp_model.from_map(m['RDP'])
+        if m.get('SSH') is not None:
+            temp_model = GetPolicyResponseBodyPolicyProtocolConfigSSH()
+            self.ssh = temp_model.from_map(m['SSH'])
+        return self
+
+
+class GetPolicyResponseBodyPolicy(TeaModel):
+    def __init__(
+        self,
+        access_time_range_config: GetPolicyResponseBodyPolicyAccessTimeRangeConfig = None,
+        approval_config: GetPolicyResponseBodyPolicyApprovalConfig = None,
+        command_config: GetPolicyResponseBodyPolicyCommandConfig = None,
+        comment: str = None,
+        ipacl_config: GetPolicyResponseBodyPolicyIPAclConfig = None,
+        policy_id: str = None,
+        policy_name: str = None,
+        priority: int = None,
+        protocol_config: GetPolicyResponseBodyPolicyProtocolConfig = None,
+    ):
+        self.access_time_range_config = access_time_range_config
+        self.approval_config = approval_config
+        self.command_config = command_config
+        self.comment = comment
+        self.ipacl_config = ipacl_config
+        self.policy_id = policy_id
+        self.policy_name = policy_name
+        self.priority = priority
+        self.protocol_config = protocol_config
+
+    def validate(self):
+        if self.access_time_range_config:
+            self.access_time_range_config.validate()
+        if self.approval_config:
+            self.approval_config.validate()
+        if self.command_config:
+            self.command_config.validate()
+        if self.ipacl_config:
+            self.ipacl_config.validate()
+        if self.protocol_config:
+            self.protocol_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_time_range_config is not None:
+            result['AccessTimeRangeConfig'] = self.access_time_range_config.to_map()
+        if self.approval_config is not None:
+            result['ApprovalConfig'] = self.approval_config.to_map()
+        if self.command_config is not None:
+            result['CommandConfig'] = self.command_config.to_map()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.ipacl_config is not None:
+            result['IPAclConfig'] = self.ipacl_config.to_map()
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.priority is not None:
+            result['Priority'] = self.priority
+        if self.protocol_config is not None:
+            result['ProtocolConfig'] = self.protocol_config.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessTimeRangeConfig') is not None:
+            temp_model = GetPolicyResponseBodyPolicyAccessTimeRangeConfig()
+            self.access_time_range_config = temp_model.from_map(m['AccessTimeRangeConfig'])
+        if m.get('ApprovalConfig') is not None:
+            temp_model = GetPolicyResponseBodyPolicyApprovalConfig()
+            self.approval_config = temp_model.from_map(m['ApprovalConfig'])
+        if m.get('CommandConfig') is not None:
+            temp_model = GetPolicyResponseBodyPolicyCommandConfig()
+            self.command_config = temp_model.from_map(m['CommandConfig'])
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('IPAclConfig') is not None:
+            temp_model = GetPolicyResponseBodyPolicyIPAclConfig()
+            self.ipacl_config = temp_model.from_map(m['IPAclConfig'])
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Priority') is not None:
+            self.priority = m.get('Priority')
+        if m.get('ProtocolConfig') is not None:
+            temp_model = GetPolicyResponseBodyPolicyProtocolConfig()
+            self.protocol_config = temp_model.from_map(m['ProtocolConfig'])
+        return self
+
+
+class GetPolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        policy: GetPolicyResponseBodyPolicy = None,
         request_id: str = None,
-        total_count: int = None,
     ):
-        # The ID of the host account.
-        self.host_accounts = host_accounts
-        # An array that consists of the queried host accounts.
+        self.policy = policy
         self.request_id = request_id
-        # The ID of the bastion host in which you want to query accounts of the specified host.
-        # 
-        # >  You can call the DescribeInstances operation to query the ID of the bastion host.
-        self.total_count = total_count
 
     def validate(self):
-        if self.host_accounts:
-            for k in self.host_accounts:
-                if k:
-                    k.validate()
+        if self.policy:
+            self.policy.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['HostAccounts'] = []
-        if self.host_accounts is not None:
-            for k in self.host_accounts:
-                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.host_accounts = []
-        if m.get('HostAccounts') is not None:
-            for k in m.get('HostAccounts'):
-                temp_model = ListHostAccountsResponseBodyHostAccounts()
-                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('Policy') is not None:
+            temp_model = GetPolicyResponseBodyPolicy()
+            self.policy = temp_model.from_map(m['Policy'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
         return self
 
 
-class ListHostAccountsResponse(TeaModel):
+class GetPolicyResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListHostAccountsResponseBody = None,
+        body: GetPolicyResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         if self.body:
@@ -8827,415 +12245,287 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListHostAccountsResponseBody()
+            temp_model = GetPolicyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListHostAccountsForHostShareKeyRequest(TeaModel):
+class GetPolicyAssetScopeRequest(TeaModel):
     def __init__(
         self,
-        host_share_key_id: str = None,
         instance_id: str = None,
-        page_number: str = None,
-        page_size: str = None,
+        policy_id: str = None,
         region_id: str = None,
     ):
-        # The ID of the shared key.
-        self.host_share_key_id = host_share_key_id
-        # The ID of the bastion host. You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The number of the page to return. Default value: **1**.
-        self.page_number = page_number
-        # The number of entries to return on each page. Default value: **10**.
-        self.page_size = page_size
-        # The region ID of the bastion host. For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.policy_id = policy_id
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_share_key_id is not None:
-            result['HostShareKeyId'] = self.host_share_key_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostShareKeyId') is not None:
-            self.host_share_key_id = m.get('HostShareKeyId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
-class ListHostAccountsForHostShareKeyResponseBodyHostAccounts(TeaModel):
+class GetPolicyAssetScopeResponseBodyAssetScopeDatabases(TeaModel):
     def __init__(
         self,
-        host_account_name: str = None,
-        host_id: str = None,
-        hosts_account_id: str = None,
-        protocol_name: str = None,
+        account_scope_type: str = None,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
     ):
-        # The name of the host account.
-        self.host_account_name = host_account_name
-        # The ID of the host.
-        self.host_id = host_id
-        # The ID of the host account.
-        self.hosts_account_id = hosts_account_id
-        # The O\&M protocol.
-        self.protocol_name = protocol_name
+        self.account_scope_type = account_scope_type
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
-        if self.hosts_account_id is not None:
-            result['HostsAccountId'] = self.hosts_account_id
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
-        if m.get('HostsAccountId') is not None:
-            self.hosts_account_id = m.get('HostsAccountId')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
-        return self
-
-
-class ListHostAccountsForHostShareKeyResponseBody(TeaModel):
-    def __init__(
-        self,
-        host_accounts: List[ListHostAccountsForHostShareKeyResponseBodyHostAccounts] = None,
-        request_id: str = None,
-        total_count: int = None,
-    ):
-        # An array that consists of the host accounts that are associated with the shared key.
-        self.host_accounts = host_accounts
-        # The ID of the request, which is used to locate and troubleshoot issues.
-        self.request_id = request_id
-        # The total number of the host accounts that are associated with the shared key.
-        self.total_count = total_count
-
-    def validate(self):
-        if self.host_accounts:
-            for k in self.host_accounts:
-                if k:
-                    k.validate()
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        result['HostAccounts'] = []
-        if self.host_accounts is not None:
-            for k in self.host_accounts:
-                result['HostAccounts'].append(k.to_map() if k else None)
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.host_accounts = []
-        if m.get('HostAccounts') is not None:
-            for k in m.get('HostAccounts'):
-                temp_model = ListHostAccountsForHostShareKeyResponseBodyHostAccounts()
-                self.host_accounts.append(temp_model.from_map(k))
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
         return self
 
 
-class ListHostAccountsForHostShareKeyResponse(TeaModel):
+class GetPolicyAssetScopeResponseBodyAssetScopeHostGroups(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListHostAccountsForHostShareKeyResponseBody = None,
+        account_names: List[str] = None,
+        account_scope_type: str = None,
+        host_group_id: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.account_names = account_names
+        self.account_scope_type = account_scope_type
+        self.host_group_id = host_group_id
 
     def validate(self):
-        if self.body:
-            self.body.validate()
+        pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        if self.account_names is not None:
+            result['AccountNames'] = self.account_names
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = ListHostAccountsForHostShareKeyResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        if m.get('AccountNames') is not None:
+            self.account_names = m.get('AccountNames')
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
         return self
 
 
-class ListHostAccountsForUserRequest(TeaModel):
+class GetPolicyAssetScopeResponseBodyAssetScopeHosts(TeaModel):
     def __init__(
         self,
-        host_account_name: str = None,
+        account_scope_type: str = None,
+        host_account_ids: List[str] = None,
         host_id: str = None,
-        instance_id: str = None,
-        page_number: str = None,
-        page_size: str = None,
-        region_id: str = None,
-        user_id: str = None,
     ):
-        # The number of the page to return. Default value: **1**.
-        self.host_account_name = host_account_name
-        # The ID of the host for which the host accounts were queried.
+        self.account_scope_type = account_scope_type
+        self.host_account_ids = host_account_ids
         self.host_id = host_id
-        # The total number of host accounts returned.
-        self.instance_id = instance_id
-        # The ID of the user for which you want to query authorized host accounts.
-        # 
-        # >  You can call the [ListUsers](~~204522~~) operation to query the ID of the user ID.
-        self.page_number = page_number
-        # The name of the host account that you want to query. Exact match is supported.
-        self.page_size = page_size
-        # The name of the host account.
-        self.region_id = region_id
-        # The region ID of the Bastionhost instance where you want to query the host accounts that the user is authorized to manage on the host.
-        # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.host_account_ids is not None:
+            result['HostAccountIds'] = self.host_account_ids
         if self.host_id is not None:
             result['HostId'] = self.host_id
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
         if m.get('HostId') is not None:
             self.host_id = m.get('HostId')
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
         return self
 
 
-class ListHostAccountsForUserResponseBodyHostAccounts(TeaModel):
+class GetPolicyAssetScopeResponseBodyAssetScope(TeaModel):
     def __init__(
         self,
-        host_account_id: str = None,
-        host_account_name: str = None,
-        host_id: str = None,
-        is_authorized: bool = None,
-        protocol_name: str = None,
+        databases: List[GetPolicyAssetScopeResponseBodyAssetScopeDatabases] = None,
+        host_groups: List[GetPolicyAssetScopeResponseBodyAssetScopeHostGroups] = None,
+        hosts: List[GetPolicyAssetScopeResponseBodyAssetScopeHosts] = None,
+        scope_type: str = None,
     ):
-        # The protocol that is used by the host account. Valid values:
-        # 
-        # *   **SSH**\
-        # *   **RDP**\
-        self.host_account_id = host_account_id
-        # The ID of the host account.
-        self.host_account_name = host_account_name
-        # The ID of the request.
-        self.host_id = host_id
-        # The ID of the host for which you want to query the host accounts that the user is authorized to manage.
-        # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
-        self.is_authorized = is_authorized
-        # Indicates whether the user is authorized to manage the host account. Valid values:
-        # 
-        # *   **true**: The user is authorized to manage the host account.
-        # *   **false**: The user is not authorized to manage the host account.
-        self.protocol_name = protocol_name
+        self.databases = databases
+        self.host_groups = host_groups
+        self.hosts = hosts
+        self.scope_type = scope_type
 
     def validate(self):
-        pass
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+        if self.host_groups:
+            for k in self.host_groups:
+                if k:
+                    k.validate()
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_id is not None:
-            result['HostAccountId'] = self.host_account_id
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
-        if self.is_authorized is not None:
-            result['IsAuthorized'] = self.is_authorized
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        result['HostGroups'] = []
+        if self.host_groups is not None:
+            for k in self.host_groups:
+                result['HostGroups'].append(k.to_map() if k else None)
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountId') is not None:
-            self.host_account_id = m.get('HostAccountId')
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
-        if m.get('IsAuthorized') is not None:
-            self.is_authorized = m.get('IsAuthorized')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = GetPolicyAssetScopeResponseBodyAssetScopeDatabases()
+                self.databases.append(temp_model.from_map(k))
+        self.host_groups = []
+        if m.get('HostGroups') is not None:
+            for k in m.get('HostGroups'):
+                temp_model = GetPolicyAssetScopeResponseBodyAssetScopeHostGroups()
+                self.host_groups.append(temp_model.from_map(k))
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = GetPolicyAssetScopeResponseBodyAssetScopeHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
         return self
 
 
-class ListHostAccountsForUserResponseBody(TeaModel):
+class GetPolicyAssetScopeResponseBody(TeaModel):
     def __init__(
         self,
-        host_accounts: List[ListHostAccountsForUserResponseBodyHostAccounts] = None,
+        asset_scope: GetPolicyAssetScopeResponseBodyAssetScope = None,
         request_id: str = None,
-        total_count: int = None,
     ):
-        # The host accounts returned.
-        self.host_accounts = host_accounts
-        # The ID of the Bastionhost instance where you want to query the host accounts that the user is authorized to manage on the host.
-        # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        self.asset_scope = asset_scope
         self.request_id = request_id
-        # The number of entries to return on each page.
-        # 
-        # The value of the PageSize parameter must not exceed 100. Default value: 20. If you leave the PageSize parameter empty, 20 entries are returned on each page.
-        # 
-        # >  We recommend that you do not leave the PageSize parameter empty.
-        self.total_count = total_count
 
     def validate(self):
-        if self.host_accounts:
-            for k in self.host_accounts:
-                if k:
-                    k.validate()
+        if self.asset_scope:
+            self.asset_scope.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['HostAccounts'] = []
-        if self.host_accounts is not None:
-            for k in self.host_accounts:
-                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.asset_scope is not None:
+            result['AssetScope'] = self.asset_scope.to_map()
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.host_accounts = []
-        if m.get('HostAccounts') is not None:
-            for k in m.get('HostAccounts'):
-                temp_model = ListHostAccountsForUserResponseBodyHostAccounts()
-                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('AssetScope') is not None:
+            temp_model = GetPolicyAssetScopeResponseBodyAssetScope()
+            self.asset_scope = temp_model.from_map(m['AssetScope'])
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
         return self
 
 
-class ListHostAccountsForUserResponse(TeaModel):
+class GetPolicyAssetScopeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListHostAccountsForUserResponseBody = None,
+        body: GetPolicyAssetScopeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         if self.body:
@@ -9258,218 +12548,138 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListHostAccountsForUserResponseBody()
+            temp_model = GetPolicyAssetScopeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListHostAccountsForUserGroupRequest(TeaModel):
+class GetPolicyUserScopeRequest(TeaModel):
     def __init__(
         self,
-        host_account_name: str = None,
-        host_id: str = None,
         instance_id: str = None,
-        page_number: str = None,
-        page_size: str = None,
+        policy_id: str = None,
         region_id: str = None,
-        user_group_id: str = None,
     ):
-        # The name of the host account that you want to query. Exact match is supported.
-        self.host_account_name = host_account_name
-        # The ID of the host to query.
-        # 
-        # > You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
-        self.host_id = host_id
-        # The ID of the bastion host on which you want to query the host accounts to be managed by the specified user group on the specified host.
-        # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The number of the page to return. Default value: **1**.
-        self.page_number = page_number
-        # The number of entries to return on each page.\
-        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
-        # 
-        # > We recommend that you do not leave this parameter empty.
-        self.page_size = page_size
-        # The region ID of the bastion host on which you want to query the host accounts to be managed by the specified user group on the specified host.
-        # 
-        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.policy_id = policy_id
         self.region_id = region_id
-        # The ID of the user group for which you want to query authorized host accounts.
-        # 
-        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
-        self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
-        if self.page_number is not None:
-            result['PageNumber'] = self.page_number
-        if self.page_size is not None:
-            result['PageSize'] = self.page_size
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
-        if m.get('PageNumber') is not None:
-            self.page_number = m.get('PageNumber')
-        if m.get('PageSize') is not None:
-            self.page_size = m.get('PageSize')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
         return self
 
 
-class ListHostAccountsForUserGroupResponseBodyHostAccounts(TeaModel):
+class GetPolicyUserScopeResponseBodyUserScope(TeaModel):
     def __init__(
         self,
-        host_account_id: str = None,
-        host_account_name: str = None,
-        host_id: str = None,
-        is_authorized: bool = None,
-        protocol_name: str = None,
+        scope_type: str = None,
+        user_group_ids: List[str] = None,
+        user_ids: List[str] = None,
     ):
-        # The ID of the host account.
-        self.host_account_id = host_account_id
-        # The name of the host account.
-        self.host_account_name = host_account_name
-        # The ID of the host for which the host accounts were queried.
-        self.host_id = host_id
-        # Indicates whether the user group is authorized to manage the host account. Valid values:
-        # 
-        # *   **true**: yes
-        # *   **false**: no
-        self.is_authorized = is_authorized
-        # The protocol that is used by the host. Valid values:
-        # 
-        # *   **SSH**\
-        # *   **RDP**\
-        self.protocol_name = protocol_name
+        self.scope_type = scope_type
+        self.user_group_ids = user_group_ids
+        self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_id is not None:
-            result['HostAccountId'] = self.host_account_id
-        if self.host_account_name is not None:
-            result['HostAccountName'] = self.host_account_name
-        if self.host_id is not None:
-            result['HostId'] = self.host_id
-        if self.is_authorized is not None:
-            result['IsAuthorized'] = self.is_authorized
-        if self.protocol_name is not None:
-            result['ProtocolName'] = self.protocol_name
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        if self.user_group_ids is not None:
+            result['UserGroupIds'] = self.user_group_ids
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountId') is not None:
-            self.host_account_id = m.get('HostAccountId')
-        if m.get('HostAccountName') is not None:
-            self.host_account_name = m.get('HostAccountName')
-        if m.get('HostId') is not None:
-            self.host_id = m.get('HostId')
-        if m.get('IsAuthorized') is not None:
-            self.is_authorized = m.get('IsAuthorized')
-        if m.get('ProtocolName') is not None:
-            self.protocol_name = m.get('ProtocolName')
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
+        if m.get('UserGroupIds') is not None:
+            self.user_group_ids = m.get('UserGroupIds')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
         return self
 
 
-class ListHostAccountsForUserGroupResponseBody(TeaModel):
+class GetPolicyUserScopeResponseBody(TeaModel):
     def __init__(
         self,
-        host_accounts: List[ListHostAccountsForUserGroupResponseBodyHostAccounts] = None,
         request_id: str = None,
-        total_count: int = None,
+        user_scope: GetPolicyUserScopeResponseBodyUserScope = None,
     ):
-        # An array that consists of the queried host accounts.
-        self.host_accounts = host_accounts
-        # The ID of the request.
         self.request_id = request_id
-        # The total number of host accounts that were queried.
-        self.total_count = total_count
+        self.user_scope = user_scope
 
     def validate(self):
-        if self.host_accounts:
-            for k in self.host_accounts:
-                if k:
-                    k.validate()
+        if self.user_scope:
+            self.user_scope.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['HostAccounts'] = []
-        if self.host_accounts is not None:
-            for k in self.host_accounts:
-                result['HostAccounts'].append(k.to_map() if k else None)
         if self.request_id is not None:
             result['RequestId'] = self.request_id
-        if self.total_count is not None:
-            result['TotalCount'] = self.total_count
+        if self.user_scope is not None:
+            result['UserScope'] = self.user_scope.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.host_accounts = []
-        if m.get('HostAccounts') is not None:
-            for k in m.get('HostAccounts'):
-                temp_model = ListHostAccountsForUserGroupResponseBodyHostAccounts()
-                self.host_accounts.append(temp_model.from_map(k))
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
-        if m.get('TotalCount') is not None:
-            self.total_count = m.get('TotalCount')
+        if m.get('UserScope') is not None:
+            temp_model = GetPolicyUserScopeResponseBodyUserScope()
+            self.user_scope = temp_model.from_map(m['UserScope'])
         return self
 
 
-class ListHostAccountsForUserGroupResponse(TeaModel):
+class GetPolicyUserScopeResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
-        body: ListHostAccountsForUserGroupResponseBody = None,
+        body: GetPolicyUserScopeResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
         if self.body:
@@ -9492,280 +12702,3716 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('headers') is not None:
             self.headers = m.get('headers')
         if m.get('statusCode') is not None:
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
-            temp_model = ListHostAccountsForUserGroupResponseBody()
+            temp_model = GetPolicyUserScopeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
-class ListHostGroupAccountNamesForUserRequest(TeaModel):
+class GetRuleRequest(TeaModel):
     def __init__(
         self,
-        host_group_id: str = None,
         instance_id: str = None,
         region_id: str = None,
-        user_id: str = None,
+        rule_id: str = None,
     ):
-        # The ID of the host group.
-        # 
-        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
-        self.host_group_id = host_group_id
-        # The ID of the bastion host to which the user belongs.
-        # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The region ID of the bastion host to which the user belongs.
-        # 
-        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
-        # The ID of the user.
-        # 
-        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
-        self.user_id = user_id
+        self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_group_id is not None:
-            result['HostGroupId'] = self.host_group_id
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.region_id is not None:
             result['RegionId'] = self.region_id
-        if self.user_id is not None:
-            result['UserId'] = self.user_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostGroupId') is not None:
-            self.host_group_id = m.get('HostGroupId')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
-        if m.get('UserId') is not None:
-            self.user_id = m.get('UserId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
         return self
 
 
-class ListHostGroupAccountNamesForUserResponseBody(TeaModel):
+class GetRuleResponseBodyRuleDatabasesDatabaseAccounts(TeaModel):
     def __init__(
         self,
-        host_account_names: List[str] = None,
-        request_id: str = None,
+        database_account_id: str = None,
     ):
-        # An array that consists of the names of host accounts.
-        self.host_account_names = host_account_names
-        # The ID of the request.
-        self.request_id = request_id
+        self.database_account_id = database_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_names is not None:
-            result['HostAccountNames'] = self.host_account_names
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountNames') is not None:
-            self.host_account_names = m.get('HostAccountNames')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
         return self
 
 
-class ListHostGroupAccountNamesForUserResponse(TeaModel):
+class GetRuleResponseBodyRuleDatabases(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListHostGroupAccountNamesForUserResponseBody = None,
+        database_accounts: List[GetRuleResponseBodyRuleDatabasesDatabaseAccounts] = None,
+        database_id: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.database_accounts = database_accounts
+        self.database_id = database_id
 
     def validate(self):
-        if self.body:
-            self.body.validate()
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
-            temp_model = ListHostGroupAccountNamesForUserResponseBody()
-            self.body = temp_model.from_map(m['body'])
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = GetRuleResponseBodyRuleDatabasesDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
         return self
 
 
-class ListHostGroupAccountNamesForUserGroupRequest(TeaModel):
+class GetRuleResponseBodyRuleHostGroups(TeaModel):
     def __init__(
         self,
+        host_account_names: List[str] = None,
         host_group_id: str = None,
-        instance_id: str = None,
-        region_id: str = None,
-        user_group_id: str = None,
     ):
-        # The ID of the host group.
-        # 
-        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        self.host_account_names = host_account_names
         self.host_group_id = host_group_id
-        # The ID of the bastion host on which you want to query the host account names the user group is authorized to manage in a host group.
-        # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
-        self.instance_id = instance_id
-        # The region ID of the bastion host on which you want to query the host account names the user group is authorized to manage in a host group.
-        # 
-        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.region_id = region_id
-        # The ID of the user group.
-        # 
-        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
-        self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.host_account_names is not None:
+            result['HostAccountNames'] = self.host_account_names
         if self.host_group_id is not None:
             result['HostGroupId'] = self.host_group_id
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
-        if self.region_id is not None:
-            result['RegionId'] = self.region_id
-        if self.user_group_id is not None:
-            result['UserGroupId'] = self.user_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
         if m.get('HostGroupId') is not None:
             self.host_group_id = m.get('HostGroupId')
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
-        if m.get('RegionId') is not None:
-            self.region_id = m.get('RegionId')
-        if m.get('UserGroupId') is not None:
-            self.user_group_id = m.get('UserGroupId')
         return self
 
 
-class ListHostGroupAccountNamesForUserGroupResponseBody(TeaModel):
+class GetRuleResponseBodyRuleHostsHostAccounts(TeaModel):
     def __init__(
         self,
-        host_account_names: List[str] = None,
-        request_id: str = None,
+        host_account_id: str = None,
     ):
-        # The names of host accounts returned.
-        self.host_account_names = host_account_names
-        # The request ID.
-        self.request_id = request_id
+        self.host_account_id = host_account_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.host_account_names is not None:
-            result['HostAccountNames'] = self.host_account_names
-        if self.request_id is not None:
-            result['RequestId'] = self.request_id
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('HostAccountNames') is not None:
-            self.host_account_names = m.get('HostAccountNames')
-        if m.get('RequestId') is not None:
-            self.request_id = m.get('RequestId')
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
         return self
 
 
-class ListHostGroupAccountNamesForUserGroupResponse(TeaModel):
+class GetRuleResponseBodyRuleHosts(TeaModel):
     def __init__(
         self,
-        headers: Dict[str, str] = None,
-        status_code: int = None,
-        body: ListHostGroupAccountNamesForUserGroupResponseBody = None,
+        host_accounts: List[GetRuleResponseBodyRuleHostsHostAccounts] = None,
+        host_id: str = None,
     ):
-        self.headers = headers
-        self.status_code = status_code
-        self.body = body
+        self.host_accounts = host_accounts
+        self.host_id = host_id
 
     def validate(self):
-        if self.body:
-            self.body.validate()
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.headers is not None:
-            result['headers'] = self.headers
-        if self.status_code is not None:
-            result['statusCode'] = self.status_code
-        if self.body is not None:
-            result['body'] = self.body.to_map()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('headers') is not None:
-            self.headers = m.get('headers')
-        if m.get('statusCode') is not None:
-            self.status_code = m.get('statusCode')
-        if m.get('body') is not None:
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = GetRuleResponseBodyRuleHostsHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class GetRuleResponseBodyRuleUserGroups(TeaModel):
+    def __init__(
+        self,
+        user_group_id: str = None,
+    ):
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class GetRuleResponseBodyRuleUsers(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+    ):
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GetRuleResponseBodyRule(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        databases: List[GetRuleResponseBodyRuleDatabases] = None,
+        effective_end_time: str = None,
+        effective_start_time: str = None,
+        host_groups: List[GetRuleResponseBodyRuleHostGroups] = None,
+        hosts: List[GetRuleResponseBodyRuleHosts] = None,
+        rule_id: str = None,
+        rule_name: str = None,
+        user_groups: List[GetRuleResponseBodyRuleUserGroups] = None,
+        users: List[GetRuleResponseBodyRuleUsers] = None,
+    ):
+        self.comment = comment
+        self.databases = databases
+        self.effective_end_time = effective_end_time
+        self.effective_start_time = effective_start_time
+        self.host_groups = host_groups
+        self.hosts = hosts
+        self.rule_id = rule_id
+        self.rule_name = rule_name
+        self.user_groups = user_groups
+        self.users = users
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+        if self.host_groups:
+            for k in self.host_groups:
+                if k:
+                    k.validate()
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+        if self.user_groups:
+            for k in self.user_groups:
+                if k:
+                    k.validate()
+        if self.users:
+            for k in self.users:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.effective_end_time is not None:
+            result['EffectiveEndTime'] = self.effective_end_time
+        if self.effective_start_time is not None:
+            result['EffectiveStartTime'] = self.effective_start_time
+        result['HostGroups'] = []
+        if self.host_groups is not None:
+            for k in self.host_groups:
+                result['HostGroups'].append(k.to_map() if k else None)
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        result['UserGroups'] = []
+        if self.user_groups is not None:
+            for k in self.user_groups:
+                result['UserGroups'].append(k.to_map() if k else None)
+        result['Users'] = []
+        if self.users is not None:
+            for k in self.users:
+                result['Users'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = GetRuleResponseBodyRuleDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('EffectiveEndTime') is not None:
+            self.effective_end_time = m.get('EffectiveEndTime')
+        if m.get('EffectiveStartTime') is not None:
+            self.effective_start_time = m.get('EffectiveStartTime')
+        self.host_groups = []
+        if m.get('HostGroups') is not None:
+            for k in m.get('HostGroups'):
+                temp_model = GetRuleResponseBodyRuleHostGroups()
+                self.host_groups.append(temp_model.from_map(k))
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = GetRuleResponseBodyRuleHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        self.user_groups = []
+        if m.get('UserGroups') is not None:
+            for k in m.get('UserGroups'):
+                temp_model = GetRuleResponseBodyRuleUserGroups()
+                self.user_groups.append(temp_model.from_map(k))
+        self.users = []
+        if m.get('Users') is not None:
+            for k in m.get('Users'):
+                temp_model = GetRuleResponseBodyRuleUsers()
+                self.users.append(temp_model.from_map(k))
+        return self
+
+
+class GetRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        rule: GetRuleResponseBodyRule = None,
+    ):
+        self.request_id = request_id
+        self.rule = rule
+
+    def validate(self):
+        if self.rule:
+            self.rule.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.rule is not None:
+            result['Rule'] = self.rule.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Rule') is not None:
+            temp_model = GetRuleResponseBodyRule()
+            self.rule = temp_model.from_map(m['Rule'])
+        return self
+
+
+class GetRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetUserRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        # The ID of the bastion host on which you want to query the user.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The region ID of the bastion host on which you want to query the user.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user.
+        # 
+        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GetUserResponseBodyUser(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        display_name: str = None,
+        effective_end_time: int = None,
+        effective_start_time: int = None,
+        email: str = None,
+        language: str = None,
+        language_status: str = None,
+        mobile: str = None,
+        mobile_country_code: str = None,
+        need_reset_password: bool = None,
+        source: str = None,
+        source_user_id: str = None,
+        two_factor_methods: List[str] = None,
+        two_factor_status: str = None,
+        user_id: str = None,
+        user_name: str = None,
+        user_state: List[str] = None,
+    ):
+        # The description of the user.
+        self.comment = comment
+        # The display name of the user.
+        self.display_name = display_name
+        # The end of the validity period of the user. The value is a UNIX timestamp. Unit: seconds.
+        self.effective_end_time = effective_end_time
+        # The beginning of the validity period of the user. The value is a UNIX timestamp. Unit: seconds.
+        self.effective_start_time = effective_start_time
+        # The email address of the user.
+        self.email = email
+        self.language = language
+        self.language_status = language_status
+        # The mobile phone number of the user.
+        self.mobile = mobile
+        # The location in which the mobile number of the user is registered. Valid values:
+        # 
+        # *   **CN**: the Chinese mainland, whose country calling code is +86
+        # *   **HK**: Hong Kong (China), whose country calling code is +852
+        # *   **MO**: Macao (China), whose country calling code is +853
+        # *   **TW**: Taiwan (China), whose country calling code is +886
+        # *   **RU**: Russia, whose country calling code is +7
+        # *   **SG**: Singapore, whose country calling code is +65
+        # *   **MY**: Malaysia, whose country calling code is +60
+        # *   **ID**: Indonesia, whose country calling code is +62
+        # *   **DE**: Germany, whose country calling code is +49
+        # *   **AU**: Australia, whose country calling code is +61
+        # *   **US**: US, whose country calling code is +1
+        # *   **AE**: United Arab Emirates, whose country calling code is +971
+        # *   **JP:** Japan, whose country calling code is +81
+        # *   **GB**: UK, whose country calling code is +44
+        # *   **IN**: India, whose country calling code is +91
+        # *   **KR**: Republic of Korea, whose country calling code is +82
+        # *   **PH**: Philippines, whose country calling code is +63
+        # *   **CH**: Switzerland, whose country calling code is +41
+        # *   **SE**: Sweden, whose country calling code is +46
+        self.mobile_country_code = mobile_country_code
+        # Specifies whether password reset is required upon the next logon. Valid values:
+        # 
+        # *   **true**: yes
+        # *   **false**: no
+        self.need_reset_password = need_reset_password
+        # The source of the user. Valid values:
+        # 
+        # *   **Local**: a local user
+        # *   **Ram**: a RAM user
+        self.source = source
+        # The unique ID of the user.
+        # 
+        # > This parameter uniquely identifies a RAM user of the bastion host. A value is returned for this parameter if the **Source** parameter is set to **Ram**. No value is returned for this parameter if the **Source** parameter is set to **Local**.
+        self.source_user_id = source_user_id
+        # An array that consists of the details of the two-factor authentication method.
+        self.two_factor_methods = two_factor_methods
+        # The two-factor authentication status of the user. Valid values:
+        # 
+        # *   **Global**: The global settings are used.
+        # *   **Disable**: The two-factor authentication is disabled.
+        # *   **Enable**: The two-factor authentication is enabled and the user-specific setting is used.
+        self.two_factor_status = two_factor_status
+        # The ID of the user.
+        self.user_id = user_id
+        # The logon name of the user.
+        self.user_name = user_name
+        # An array that consists of the details of the user status.
+        self.user_state = user_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.display_name is not None:
+            result['DisplayName'] = self.display_name
+        if self.effective_end_time is not None:
+            result['EffectiveEndTime'] = self.effective_end_time
+        if self.effective_start_time is not None:
+            result['EffectiveStartTime'] = self.effective_start_time
+        if self.email is not None:
+            result['Email'] = self.email
+        if self.language is not None:
+            result['Language'] = self.language
+        if self.language_status is not None:
+            result['LanguageStatus'] = self.language_status
+        if self.mobile is not None:
+            result['Mobile'] = self.mobile
+        if self.mobile_country_code is not None:
+            result['MobileCountryCode'] = self.mobile_country_code
+        if self.need_reset_password is not None:
+            result['NeedResetPassword'] = self.need_reset_password
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_user_id is not None:
+            result['SourceUserId'] = self.source_user_id
+        if self.two_factor_methods is not None:
+            result['TwoFactorMethods'] = self.two_factor_methods
+        if self.two_factor_status is not None:
+            result['TwoFactorStatus'] = self.two_factor_status
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.user_state is not None:
+            result['UserState'] = self.user_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DisplayName') is not None:
+            self.display_name = m.get('DisplayName')
+        if m.get('EffectiveEndTime') is not None:
+            self.effective_end_time = m.get('EffectiveEndTime')
+        if m.get('EffectiveStartTime') is not None:
+            self.effective_start_time = m.get('EffectiveStartTime')
+        if m.get('Email') is not None:
+            self.email = m.get('Email')
+        if m.get('Language') is not None:
+            self.language = m.get('Language')
+        if m.get('LanguageStatus') is not None:
+            self.language_status = m.get('LanguageStatus')
+        if m.get('Mobile') is not None:
+            self.mobile = m.get('Mobile')
+        if m.get('MobileCountryCode') is not None:
+            self.mobile_country_code = m.get('MobileCountryCode')
+        if m.get('NeedResetPassword') is not None:
+            self.need_reset_password = m.get('NeedResetPassword')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceUserId') is not None:
+            self.source_user_id = m.get('SourceUserId')
+        if m.get('TwoFactorMethods') is not None:
+            self.two_factor_methods = m.get('TwoFactorMethods')
+        if m.get('TwoFactorStatus') is not None:
+            self.two_factor_status = m.get('TwoFactorStatus')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('UserState') is not None:
+            self.user_state = m.get('UserState')
+        return self
+
+
+class GetUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        user: GetUserResponseBodyUser = None,
+    ):
+        # The ID of the request.
+        self.request_id = request_id
+        # The details of the user that was queried.
+        self.user = user
+
+    def validate(self):
+        if self.user:
+            self.user.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.user is not None:
+            result['User'] = self.user.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('User') is not None:
+            temp_model = GetUserResponseBodyUser()
+            self.user = temp_model.from_map(m['User'])
+        return self
+
+
+class GetUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        # The ID of the bastion host in which you want to query the details of the user group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The region ID of the bastion host in which you want to query the details of the user group.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user group.
+        # 
+        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class GetUserGroupResponseBodyUserGroup(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        user_group_id: str = None,
+        user_group_name: str = None,
+    ):
+        # The description of the user group.
+        self.comment = comment
+        # The ID of the group.
+        self.user_group_id = user_group_id
+        # The name of the user group.
+        self.user_group_name = user_group_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        if self.user_group_name is not None:
+            result['UserGroupName'] = self.user_group_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        if m.get('UserGroupName') is not None:
+            self.user_group_name = m.get('UserGroupName')
+        return self
+
+
+class GetUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        user_group: GetUserGroupResponseBodyUserGroup = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
+        # The details of the user group returned.
+        self.user_group = user_group
+
+    def validate(self):
+        if self.user_group:
+            self.user_group.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.user_group is not None:
+            result['UserGroup'] = self.user_group.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('UserGroup') is not None:
+            temp_model = GetUserGroupResponseBodyUserGroup()
+            self.user_group = temp_model.from_map(m['UserGroup'])
+        return self
+
+
+class GetUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListApproveCommandsRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListApproveCommandsResponseBodyApproveCommands(TeaModel):
+    def __init__(
+        self,
+        approve_command_id: str = None,
+        asset_account_name: str = None,
+        asset_ip: str = None,
+        asset_name: str = None,
+        client_ip: str = None,
+        client_user: str = None,
+        command: str = None,
+        create_time: str = None,
+        protocol_name: str = None,
+        session_id: str = None,
+        state: str = None,
+    ):
+        self.approve_command_id = approve_command_id
+        self.asset_account_name = asset_account_name
+        self.asset_ip = asset_ip
+        self.asset_name = asset_name
+        self.client_ip = client_ip
+        self.client_user = client_user
+        self.command = command
+        self.create_time = create_time
+        self.protocol_name = protocol_name
+        self.session_id = session_id
+        self.state = state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approve_command_id is not None:
+            result['ApproveCommandId'] = self.approve_command_id
+        if self.asset_account_name is not None:
+            result['AssetAccountName'] = self.asset_account_name
+        if self.asset_ip is not None:
+            result['AssetIp'] = self.asset_ip
+        if self.asset_name is not None:
+            result['AssetName'] = self.asset_name
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.client_user is not None:
+            result['ClientUser'] = self.client_user
+        if self.command is not None:
+            result['Command'] = self.command
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        if self.session_id is not None:
+            result['SessionId'] = self.session_id
+        if self.state is not None:
+            result['State'] = self.state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApproveCommandId') is not None:
+            self.approve_command_id = m.get('ApproveCommandId')
+        if m.get('AssetAccountName') is not None:
+            self.asset_account_name = m.get('AssetAccountName')
+        if m.get('AssetIp') is not None:
+            self.asset_ip = m.get('AssetIp')
+        if m.get('AssetName') is not None:
+            self.asset_name = m.get('AssetName')
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('ClientUser') is not None:
+            self.client_user = m.get('ClientUser')
+        if m.get('Command') is not None:
+            self.command = m.get('Command')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        if m.get('SessionId') is not None:
+            self.session_id = m.get('SessionId')
+        if m.get('State') is not None:
+            self.state = m.get('State')
+        return self
+
+
+class ListApproveCommandsResponseBody(TeaModel):
+    def __init__(
+        self,
+        approve_commands: List[ListApproveCommandsResponseBodyApproveCommands] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.approve_commands = approve_commands
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.approve_commands:
+            for k in self.approve_commands:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ApproveCommands'] = []
+        if self.approve_commands is not None:
+            for k in self.approve_commands:
+                result['ApproveCommands'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.approve_commands = []
+        if m.get('ApproveCommands') is not None:
+            for k in m.get('ApproveCommands'):
+                temp_model = ListApproveCommandsResponseBodyApproveCommands()
+                self.approve_commands.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListApproveCommandsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListApproveCommandsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListApproveCommandsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabaseAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_name: str = None,
+        database_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListDatabaseAccountsResponseBodyDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_id: str = None,
+        database_schema: str = None,
+        has_password: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.database_schema = database_schema
+        self.has_password = has_password
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_schema is not None:
+            result['DatabaseSchema'] = self.database_schema
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseSchema') is not None:
+            self.database_schema = m.get('DatabaseSchema')
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        return self
+
+
+class ListDatabaseAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_accounts: List[ListDatabaseAccountsResponseBodyDatabaseAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.database_accounts = database_accounts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = ListDatabaseAccountsResponseBodyDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabaseAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabaseAccountsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabaseAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabaseAccountsForUserRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_name: str = None,
+        database_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ListDatabaseAccountsForUserResponseBodyDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_id: str = None,
+        is_authorized: bool = None,
+        protocol_name: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.is_authorized = is_authorized
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.is_authorized is not None:
+            result['IsAuthorized'] = self.is_authorized
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('IsAuthorized') is not None:
+            self.is_authorized = m.get('IsAuthorized')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListDatabaseAccountsForUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_accounts: List[ListDatabaseAccountsForUserResponseBodyDatabaseAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.database_accounts = database_accounts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = ListDatabaseAccountsForUserResponseBodyDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabaseAccountsForUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabaseAccountsForUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabaseAccountsForUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabaseAccountsForUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_name: str = None,
+        database_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class ListDatabaseAccountsForUserGroupResponseBodyDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_id: str = None,
+        is_authorized: bool = None,
+        protocol_name: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.is_authorized = is_authorized
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.is_authorized is not None:
+            result['IsAuthorized'] = self.is_authorized
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('IsAuthorized') is not None:
+            self.is_authorized = m.get('IsAuthorized')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListDatabaseAccountsForUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_accounts: List[ListDatabaseAccountsForUserGroupResponseBodyDatabaseAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.database_accounts = database_accounts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = ListDatabaseAccountsForUserGroupResponseBodyDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabaseAccountsForUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabaseAccountsForUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabaseAccountsForUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabasesRequest(TeaModel):
+    def __init__(
+        self,
+        database_type: str = None,
+        host_group_id: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        source: str = None,
+    ):
+        self.database_type = database_type
+        self.host_group_id = host_group_id
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.source = source
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.source is not None:
+            result['Source'] = self.source
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        return self
+
+
+class ListDatabasesResponseBodyDatabases(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        network_domain_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_region_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.network_domain_id = network_domain_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_region_id = source_instance_region_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_region_id is not None:
+            result['SourceInstanceRegionId'] = self.source_instance_region_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceRegionId') is not None:
+            self.source_instance_region_id = m.get('SourceInstanceRegionId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class ListDatabasesResponseBody(TeaModel):
+    def __init__(
+        self,
+        databases: List[ListDatabasesResponseBodyDatabases] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.databases = databases
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = ListDatabasesResponseBodyDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabasesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabasesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabasesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabasesForUserRequest(TeaModel):
+    def __init__(
+        self,
+        database_address: str = None,
+        database_name: str = None,
+        database_type: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        self.database_address = database_address
+        self.database_name = database_name
+        self.database_type = database_type
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_address is not None:
+            result['DatabaseAddress'] = self.database_address
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAddress') is not None:
+            self.database_address = m.get('DatabaseAddress')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ListDatabasesForUserResponseBodyDatabases(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        network_domain_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.network_domain_id = network_domain_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        return self
+
+
+class ListDatabasesForUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        databases: List[ListDatabasesForUserResponseBodyDatabases] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.databases = databases
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = ListDatabasesForUserResponseBodyDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabasesForUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabasesForUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabasesForUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDatabasesForUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        database_address: str = None,
+        database_name: str = None,
+        database_type: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        self.database_address = database_address
+        self.database_name = database_name
+        self.database_type = database_type
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_address is not None:
+            result['DatabaseAddress'] = self.database_address
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAddress') is not None:
+            self.database_address = m.get('DatabaseAddress')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class ListDatabasesForUserGroupResponseBodyDatabases(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_account_count: int = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        network_domain_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_account_count = database_account_count
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.network_domain_id = network_domain_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_account_count is not None:
+            result['DatabaseAccountCount'] = self.database_account_count
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseAccountCount') is not None:
+            self.database_account_count = m.get('DatabaseAccountCount')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        return self
+
+
+class ListDatabasesForUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        databases: List[ListDatabasesForUserGroupResponseBodyDatabases] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.databases = databases
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = ListDatabasesForUserGroupResponseBodyDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDatabasesForUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDatabasesForUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListDatabasesForUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        host_account_name: str = None,
+        host_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        protocol_name: str = None,
+        region_id: str = None,
+    ):
+        # The name of the host account that you want to query. The name can be up to 128 characters in length. Only exact match is supported.
+        self.host_account_name = host_account_name
+        # The ID of the specified host whose accounts you want to query.
+        # 
+        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        self.host_id = host_id
+        # The ID of the bastion host in which you want to query accounts of the specified host.
+        # 
+        # >  You can call the DescribeInstances operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The number of the page to return. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries to return on each page.
+        # 
+        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
+        # 
+        # >  We recommend that you do not leave this parameter empty.
+        self.page_size = page_size
+        # The protocol used by the host whose accounts you want to query.
+        # 
+        # Valid values:
+        # 
+        # *   SSH
+        # *   RDP
+        self.protocol_name = protocol_name
+        # The region ID of the bastion host in which you want to query accounts of the specified host.
+        # 
+        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListHostAccountsResponseBodyHostAccounts(TeaModel):
+    def __init__(
+        self,
+        has_password: bool = None,
+        host_account_id: str = None,
+        host_account_name: str = None,
+        host_id: str = None,
+        host_share_key_id: str = None,
+        host_share_key_name: str = None,
+        private_key_fingerprint: str = None,
+        protocol_name: str = None,
+    ):
+        # Indicates whether a password is configured for the host account.
+        # 
+        # Valid values:
+        # 
+        # *   true: A password is configured for the host account.
+        # *   false: No passwords are configured for the host account.
+        self.has_password = has_password
+        # The ID of the host account.
+        self.host_account_id = host_account_id
+        # The name of the host account.
+        self.host_account_name = host_account_name
+        # The ID of the host.
+        self.host_id = host_id
+        # The ID of the shared key.
+        self.host_share_key_id = host_share_key_id
+        # The name of the shared key.
+        self.host_share_key_name = host_share_key_name
+        # The fingerprint of the private key for the host account.
+        self.private_key_fingerprint = private_key_fingerprint
+        # The protocol that is used by the host.
+        # 
+        # Valid values:
+        # 
+        # *   SSH
+        # *   RDP
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.host_share_key_id is not None:
+            result['HostShareKeyId'] = self.host_share_key_id
+        if self.host_share_key_name is not None:
+            result['HostShareKeyName'] = self.host_share_key_name
+        if self.private_key_fingerprint is not None:
+            result['PrivateKeyFingerprint'] = self.private_key_fingerprint
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('HostShareKeyId') is not None:
+            self.host_share_key_id = m.get('HostShareKeyId')
+        if m.get('HostShareKeyName') is not None:
+            self.host_share_key_name = m.get('HostShareKeyName')
+        if m.get('PrivateKeyFingerprint') is not None:
+            self.private_key_fingerprint = m.get('PrivateKeyFingerprint')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListHostAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_accounts: List[ListHostAccountsResponseBodyHostAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # An array that consists of the queried host accounts.
+        self.host_accounts = host_accounts
+        # The ID of the request.
+        self.request_id = request_id
+        # The total number of host accounts that are queried.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = ListHostAccountsResponseBodyHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListHostAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostAccountsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListHostAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostAccountsForHostShareKeyRequest(TeaModel):
+    def __init__(
+        self,
+        host_share_key_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        # The ID of the shared key.
+        self.host_share_key_id = host_share_key_id
+        # The ID of the bastion host. You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The number of the page to return. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries to return on each page. Default value: **10**.
+        self.page_size = page_size
+        # The region ID of the bastion host. For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_share_key_id is not None:
+            result['HostShareKeyId'] = self.host_share_key_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostShareKeyId') is not None:
+            self.host_share_key_id = m.get('HostShareKeyId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListHostAccountsForHostShareKeyResponseBodyHostAccounts(TeaModel):
+    def __init__(
+        self,
+        host_account_name: str = None,
+        host_id: str = None,
+        hosts_account_id: str = None,
+        protocol_name: str = None,
+    ):
+        # The name of the host account.
+        self.host_account_name = host_account_name
+        # The ID of the host.
+        self.host_id = host_id
+        # The ID of the host account.
+        self.hosts_account_id = hosts_account_id
+        # The O\&M protocol.
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.hosts_account_id is not None:
+            result['HostsAccountId'] = self.hosts_account_id
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('HostsAccountId') is not None:
+            self.hosts_account_id = m.get('HostsAccountId')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListHostAccountsForHostShareKeyResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_accounts: List[ListHostAccountsForHostShareKeyResponseBodyHostAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # An array that consists of the host accounts that are associated with the shared key.
+        self.host_accounts = host_accounts
+        # The ID of the request, which is used to locate and troubleshoot issues.
+        self.request_id = request_id
+        # The total number of the host accounts that are associated with the shared key.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = ListHostAccountsForHostShareKeyResponseBodyHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListHostAccountsForHostShareKeyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostAccountsForHostShareKeyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListHostAccountsForHostShareKeyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostAccountsForUserRequest(TeaModel):
+    def __init__(
+        self,
+        host_account_name: str = None,
+        host_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        # The name of the host account that you want to query. Exact match is supported.
+        self.host_account_name = host_account_name
+        # The ID of the host to query.
+        # 
+        # > You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        self.host_id = host_id
+        # The ID of the bastion host on which you want to perform the query. The host accounts that the specified user is authorized to manage on the specified host are queried.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The number of the page to return. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries to return on each page.\
+        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
+        # 
+        # > We recommend that you do not leave this parameter empty.
+        self.page_size = page_size
+        # The region ID of the bastion host on which you want to perform the query. The host accounts that the specified user is authorized to manage on the specified host are queried.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user for which you want to query authorized host accounts.
+        # 
+        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ListHostAccountsForUserResponseBodyHostAccounts(TeaModel):
+    def __init__(
+        self,
+        host_account_id: str = None,
+        host_account_name: str = None,
+        host_id: str = None,
+        is_authorized: bool = None,
+        protocol_name: str = None,
+    ):
+        # The ID of the host account.
+        self.host_account_id = host_account_id
+        # The name of the host account.
+        self.host_account_name = host_account_name
+        # The ID of the host for which the host accounts were queried.
+        self.host_id = host_id
+        # Indicates whether the user is authorized to manage the host account. Valid values:
+        # 
+        # *   **true**: yes
+        # *   **false**: no
+        self.is_authorized = is_authorized
+        # The protocol that is used by the host. Valid values:
+        # 
+        # *   **SSH**\
+        # *   **RDP**\
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.is_authorized is not None:
+            result['IsAuthorized'] = self.is_authorized
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('IsAuthorized') is not None:
+            self.is_authorized = m.get('IsAuthorized')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListHostAccountsForUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_accounts: List[ListHostAccountsForUserResponseBodyHostAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # An array that consists of the queried host accounts.
+        self.host_accounts = host_accounts
+        # The ID of the request.
+        self.request_id = request_id
+        # The total number of host accounts that were queried.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = ListHostAccountsForUserResponseBodyHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListHostAccountsForUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostAccountsForUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListHostAccountsForUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostAccountsForUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        host_account_name: str = None,
+        host_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        # The name of the host account that you want to query. Exact match is supported.
+        self.host_account_name = host_account_name
+        # The ID of the host to query.
+        # 
+        # > You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        self.host_id = host_id
+        # The ID of the bastion host on which you want to query the host accounts to be managed by the specified user group on the specified host.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The number of the page to return. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries to return on each page.\
+        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
+        # 
+        # > We recommend that you do not leave this parameter empty.
+        self.page_size = page_size
+        # The region ID of the bastion host on which you want to query the host accounts to be managed by the specified user group on the specified host.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user group for which you want to query authorized host accounts.
+        # 
+        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class ListHostAccountsForUserGroupResponseBodyHostAccounts(TeaModel):
+    def __init__(
+        self,
+        host_account_id: str = None,
+        host_account_name: str = None,
+        host_id: str = None,
+        is_authorized: bool = None,
+        protocol_name: str = None,
+    ):
+        # The ID of the host account.
+        self.host_account_id = host_account_id
+        # The name of the host account.
+        self.host_account_name = host_account_name
+        # The ID of the host for which the host accounts were queried.
+        self.host_id = host_id
+        # Indicates whether the user group is authorized to manage the host account. Valid values:
+        # 
+        # *   **true**: yes
+        # *   **false**: no
+        self.is_authorized = is_authorized
+        # The protocol that is used by the host. Valid values:
+        # 
+        # *   **SSH**\
+        # *   **RDP**\
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.is_authorized is not None:
+            result['IsAuthorized'] = self.is_authorized
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('IsAuthorized') is not None:
+            self.is_authorized = m.get('IsAuthorized')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListHostAccountsForUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_accounts: List[ListHostAccountsForUserGroupResponseBodyHostAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # An array that consists of the queried host accounts.
+        self.host_accounts = host_accounts
+        # The ID of the request.
+        self.request_id = request_id
+        # The total number of host accounts that were queried.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = ListHostAccountsForUserGroupResponseBodyHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListHostAccountsForUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostAccountsForUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListHostAccountsForUserGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostGroupAccountNamesForUserRequest(TeaModel):
+    def __init__(
+        self,
+        host_group_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_id: str = None,
+    ):
+        # The ID of the host group.
+        # 
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        self.host_group_id = host_group_id
+        # The ID of the bastion host to which the user belongs.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The region ID of the bastion host to which the user belongs.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user.
+        # 
+        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class ListHostGroupAccountNamesForUserResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_account_names: List[str] = None,
+        request_id: str = None,
+    ):
+        # An array that consists of the names of host accounts.
+        self.host_account_names = host_account_names
+        # The ID of the request.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_names is not None:
+            result['HostAccountNames'] = self.host_account_names
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListHostGroupAccountNamesForUserResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostGroupAccountNamesForUserResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListHostGroupAccountNamesForUserResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListHostGroupAccountNamesForUserGroupRequest(TeaModel):
+    def __init__(
+        self,
+        host_group_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+        user_group_id: str = None,
+    ):
+        # The ID of the host group.
+        # 
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        self.host_group_id = host_group_id
+        # The ID of the bastion host on which you want to query the host account names the user group is authorized to manage in a host group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The region ID of the bastion host on which you want to query the host account names the user group is authorized to manage in a host group.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+        # The ID of the user group.
+        # 
+        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
+        self.user_group_id = user_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class ListHostGroupAccountNamesForUserGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_account_names: List[str] = None,
+        request_id: str = None,
+    ):
+        # The names of host accounts returned.
+        self.host_account_names = host_account_names
+        # The request ID.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_names is not None:
+            result['HostAccountNames'] = self.host_account_names
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ListHostGroupAccountNamesForUserGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListHostGroupAccountNamesForUserGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
             temp_model = ListHostGroupAccountNamesForUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListHostGroupsRequest(TeaModel):
     def __init__(
@@ -11441,14 +18087,1226 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListHostsForUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListNetworkDomainsRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        network_domain_name: str = None,
+        network_domain_type: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.network_domain_name = network_domain_name
+        self.network_domain_type = network_domain_type
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_name is not None:
+            result['NetworkDomainName'] = self.network_domain_name
+        if self.network_domain_type is not None:
+            result['NetworkDomainType'] = self.network_domain_type
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainName') is not None:
+            self.network_domain_name = m.get('NetworkDomainName')
+        if m.get('NetworkDomainType') is not None:
+            self.network_domain_type = m.get('NetworkDomainType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListNetworkDomainsResponseBodyNetworkDomainsProxiesState(TeaModel):
+    def __init__(
+        self,
+        node_type: str = None,
+        proxy_state: str = None,
+    ):
+        self.node_type = node_type
+        self.proxy_state = proxy_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.proxy_state is not None:
+            result['ProxyState'] = self.proxy_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('ProxyState') is not None:
+            self.proxy_state = m.get('ProxyState')
+        return self
+
+
+class ListNetworkDomainsResponseBodyNetworkDomains(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        default: bool = None,
+        network_domain_id: str = None,
+        network_domain_name: str = None,
+        network_domain_type: str = None,
+        proxies_state: List[ListNetworkDomainsResponseBodyNetworkDomainsProxiesState] = None,
+    ):
+        self.comment = comment
+        self.default = default
+        self.network_domain_id = network_domain_id
+        self.network_domain_name = network_domain_name
+        self.network_domain_type = network_domain_type
+        self.proxies_state = proxies_state
+
+    def validate(self):
+        if self.proxies_state:
+            for k in self.proxies_state:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.default is not None:
+            result['Default'] = self.default
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.network_domain_name is not None:
+            result['NetworkDomainName'] = self.network_domain_name
+        if self.network_domain_type is not None:
+            result['NetworkDomainType'] = self.network_domain_type
+        result['ProxiesState'] = []
+        if self.proxies_state is not None:
+            for k in self.proxies_state:
+                result['ProxiesState'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('Default') is not None:
+            self.default = m.get('Default')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('NetworkDomainName') is not None:
+            self.network_domain_name = m.get('NetworkDomainName')
+        if m.get('NetworkDomainType') is not None:
+            self.network_domain_type = m.get('NetworkDomainType')
+        self.proxies_state = []
+        if m.get('ProxiesState') is not None:
+            for k in m.get('ProxiesState'):
+                temp_model = ListNetworkDomainsResponseBodyNetworkDomainsProxiesState()
+                self.proxies_state.append(temp_model.from_map(k))
+        return self
+
+
+class ListNetworkDomainsResponseBody(TeaModel):
+    def __init__(
+        self,
+        network_domains: List[ListNetworkDomainsResponseBodyNetworkDomains] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.network_domains = network_domains
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.network_domains:
+            for k in self.network_domains:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['NetworkDomains'] = []
+        if self.network_domains is not None:
+            for k in self.network_domains:
+                result['NetworkDomains'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.network_domains = []
+        if m.get('NetworkDomains') is not None:
+            for k in m.get('NetworkDomains'):
+                temp_model = ListNetworkDomainsResponseBodyNetworkDomains()
+                self.network_domains.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListNetworkDomainsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListNetworkDomainsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListNetworkDomainsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListOperationDatabaseAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_name: str = None,
+        database_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListOperationDatabaseAccountsResponseBodyDatabaseAccounts(TeaModel):
+    def __init__(
+        self,
+        dbname: str = None,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_id: str = None,
+        has_password: str = None,
+        login_attribute: str = None,
+        protocol_name: str = None,
+    ):
+        self.dbname = dbname
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_id = database_id
+        self.has_password = has_password
+        self.login_attribute = login_attribute
+        self.protocol_name = protocol_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.dbname is not None:
+            result['DBName'] = self.dbname
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        if self.login_attribute is not None:
+            result['LoginAttribute'] = self.login_attribute
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DBName') is not None:
+            self.dbname = m.get('DBName')
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        if m.get('LoginAttribute') is not None:
+            self.login_attribute = m.get('LoginAttribute')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        return self
+
+
+class ListOperationDatabaseAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        database_accounts: List[ListOperationDatabaseAccountsResponseBodyDatabaseAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.database_accounts = database_accounts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = ListOperationDatabaseAccountsResponseBodyDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListOperationDatabaseAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListOperationDatabaseAccountsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListOperationDatabaseAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListOperationDatabasesRequest(TeaModel):
+    def __init__(
+        self,
+        database_address: str = None,
+        database_name: str = None,
+        database_type: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.database_address = database_address
+        self.database_name = database_name
+        self.database_type = database_type
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_address is not None:
+            result['DatabaseAddress'] = self.database_address
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAddress') is not None:
+            self.database_address = m.get('DatabaseAddress')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class ListOperationDatabasesResponseBodyDatabases(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: int = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        database_type: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_region_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.database_type = database_type
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_region_id = source_instance_region_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.database_type is not None:
+            result['DatabaseType'] = self.database_type
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_region_id is not None:
+            result['SourceInstanceRegionId'] = self.source_instance_region_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('DatabaseType') is not None:
+            self.database_type = m.get('DatabaseType')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceRegionId') is not None:
+            self.source_instance_region_id = m.get('SourceInstanceRegionId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class ListOperationDatabasesResponseBody(TeaModel):
+    def __init__(
+        self,
+        databases: List[ListOperationDatabasesResponseBodyDatabases] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.databases = databases
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = ListOperationDatabasesResponseBodyDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListOperationDatabasesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListOperationDatabasesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListOperationDatabasesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListOperationHostAccountsRequest(TeaModel):
+    def __init__(
+        self,
+        host_account_name: str = None,
+        host_id: str = None,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+    ):
+        self.host_account_name = host_account_name
+        self.host_id = host_id
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListOperationHostAccountsResponseBodyHostAccountsSSHConfig(TeaModel):
+    def __init__(
+        self,
+        enable_sftpchannel: bool = None,
+        enable_sshchannel: bool = None,
+    ):
+        self.enable_sftpchannel = enable_sftpchannel
+        self.enable_sshchannel = enable_sshchannel
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.enable_sftpchannel is not None:
+            result['EnableSFTPChannel'] = self.enable_sftpchannel
+        if self.enable_sshchannel is not None:
+            result['EnableSSHChannel'] = self.enable_sshchannel
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('EnableSFTPChannel') is not None:
+            self.enable_sftpchannel = m.get('EnableSFTPChannel')
+        if m.get('EnableSSHChannel') is not None:
+            self.enable_sshchannel = m.get('EnableSSHChannel')
+        return self
+
+
+class ListOperationHostAccountsResponseBodyHostAccounts(TeaModel):
+    def __init__(
+        self,
+        has_password: bool = None,
+        host_account_id: str = None,
+        host_account_name: str = None,
+        host_id: str = None,
+        host_share_key_id: str = None,
+        private_key_fingerprint: str = None,
+        protocol_name: str = None,
+        sshconfig: ListOperationHostAccountsResponseBodyHostAccountsSSHConfig = None,
+    ):
+        self.has_password = has_password
+        self.host_account_id = host_account_id
+        self.host_account_name = host_account_name
+        self.host_id = host_id
+        self.host_share_key_id = host_share_key_id
+        self.private_key_fingerprint = private_key_fingerprint
+        self.protocol_name = protocol_name
+        self.sshconfig = sshconfig
+
+    def validate(self):
+        if self.sshconfig:
+            self.sshconfig.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_password is not None:
+            result['HasPassword'] = self.has_password
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
+        if self.host_account_name is not None:
+            result['HostAccountName'] = self.host_account_name
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.host_share_key_id is not None:
+            result['HostShareKeyId'] = self.host_share_key_id
+        if self.private_key_fingerprint is not None:
+            result['PrivateKeyFingerprint'] = self.private_key_fingerprint
+        if self.protocol_name is not None:
+            result['ProtocolName'] = self.protocol_name
+        if self.sshconfig is not None:
+            result['SSHConfig'] = self.sshconfig.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HasPassword') is not None:
+            self.has_password = m.get('HasPassword')
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
+        if m.get('HostAccountName') is not None:
+            self.host_account_name = m.get('HostAccountName')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('HostShareKeyId') is not None:
+            self.host_share_key_id = m.get('HostShareKeyId')
+        if m.get('PrivateKeyFingerprint') is not None:
+            self.private_key_fingerprint = m.get('PrivateKeyFingerprint')
+        if m.get('ProtocolName') is not None:
+            self.protocol_name = m.get('ProtocolName')
+        if m.get('SSHConfig') is not None:
+            temp_model = ListOperationHostAccountsResponseBodyHostAccountsSSHConfig()
+            self.sshconfig = temp_model.from_map(m['SSHConfig'])
+        return self
+
+
+class ListOperationHostAccountsResponseBody(TeaModel):
+    def __init__(
+        self,
+        host_accounts: List[ListOperationHostAccountsResponseBodyHostAccounts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.host_accounts = host_accounts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.host_accounts = []
+        if m.get('HostAccounts') is not None:
+            for k in m.get('HostAccounts'):
+                temp_model = ListOperationHostAccountsResponseBodyHostAccounts()
+                self.host_accounts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListOperationHostAccountsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListOperationHostAccountsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListOperationHostAccountsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListOperationHostsRequest(TeaModel):
+    def __init__(
+        self,
+        host_address: str = None,
+        host_name: str = None,
+        instance_id: str = None,
+        ostype: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.host_address = host_address
+        self.host_name = host_name
+        self.instance_id = instance_id
+        self.ostype = ostype
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_address is not None:
+            result['HostAddress'] = self.host_address
+        if self.host_name is not None:
+            result['HostName'] = self.host_name
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.ostype is not None:
+            result['OSType'] = self.ostype
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAddress') is not None:
+            self.host_address = m.get('HostAddress')
+        if m.get('HostName') is not None:
+            self.host_name = m.get('HostName')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('OSType') is not None:
+            self.ostype = m.get('OSType')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class ListOperationHostsResponseBodyHosts(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        host_id: str = None,
+        host_name: str = None,
+        host_private_address: str = None,
+        host_public_address: str = None,
+        ostype: str = None,
+        source: str = None,
+        source_instance_id: str = None,
+        source_instance_state: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.host_id = host_id
+        self.host_name = host_name
+        self.host_private_address = host_private_address
+        self.host_public_address = host_public_address
+        self.ostype = ostype
+        self.source = source
+        self.source_instance_id = source_instance_id
+        self.source_instance_state = source_instance_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.host_name is not None:
+            result['HostName'] = self.host_name
+        if self.host_private_address is not None:
+            result['HostPrivateAddress'] = self.host_private_address
+        if self.host_public_address is not None:
+            result['HostPublicAddress'] = self.host_public_address
+        if self.ostype is not None:
+            result['OSType'] = self.ostype
+        if self.source is not None:
+            result['Source'] = self.source
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        if self.source_instance_state is not None:
+            result['SourceInstanceState'] = self.source_instance_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('HostName') is not None:
+            self.host_name = m.get('HostName')
+        if m.get('HostPrivateAddress') is not None:
+            self.host_private_address = m.get('HostPrivateAddress')
+        if m.get('HostPublicAddress') is not None:
+            self.host_public_address = m.get('HostPublicAddress')
+        if m.get('OSType') is not None:
+            self.ostype = m.get('OSType')
+        if m.get('Source') is not None:
+            self.source = m.get('Source')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        if m.get('SourceInstanceState') is not None:
+            self.source_instance_state = m.get('SourceInstanceState')
+        return self
+
+
+class ListOperationHostsResponseBody(TeaModel):
+    def __init__(
+        self,
+        hosts: List[ListOperationHostsResponseBodyHosts] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.hosts = hosts
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = ListOperationHostsResponseBodyHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListOperationHostsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListOperationHostsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListOperationHostsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListOperationTicketsRequest(TeaModel):
     def __init__(
         self,
         asset_address: str = None,
         instance_id: str = None,
         page_number: str = None,
         page_size: str = None,
@@ -11691,14 +19549,400 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListOperationTicketsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListPoliciesRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        policy_name: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.policy_name = policy_name
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ListPoliciesResponseBodyPolicies(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        policy_id: str = None,
+        policy_name: str = None,
+        priority: int = None,
+    ):
+        self.comment = comment
+        self.policy_id = policy_id
+        self.policy_name = policy_name
+        self.priority = priority
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.priority is not None:
+            result['Priority'] = self.priority
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Priority') is not None:
+            self.priority = m.get('Priority')
+        return self
+
+
+class ListPoliciesResponseBody(TeaModel):
+    def __init__(
+        self,
+        policies: List[ListPoliciesResponseBodyPolicies] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.policies = policies
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Policies'] = []
+        if self.policies is not None:
+            for k in self.policies:
+                result['Policies'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.policies = []
+        if m.get('Policies') is not None:
+            for k in m.get('Policies'):
+                temp_model = ListPoliciesResponseBodyPolicies()
+                self.policies.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListPoliciesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListPoliciesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListPoliciesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListRulesRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        page_number: str = None,
+        page_size: str = None,
+        region_id: str = None,
+        rule_name: str = None,
+        rule_state: str = None,
+    ):
+        self.instance_id = instance_id
+        self.page_number = page_number
+        self.page_size = page_size
+        self.region_id = region_id
+        self.rule_name = rule_name
+        self.rule_state = rule_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.rule_state is not None:
+            result['RuleState'] = self.rule_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('RuleState') is not None:
+            self.rule_state = m.get('RuleState')
+        return self
+
+
+class ListRulesResponseBodyRules(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        effective_end_time: int = None,
+        effective_start_time: int = None,
+        rule_id: str = None,
+        rule_name: str = None,
+        rule_state: str = None,
+    ):
+        self.comment = comment
+        self.effective_end_time = effective_end_time
+        self.effective_start_time = effective_start_time
+        self.rule_id = rule_id
+        self.rule_name = rule_name
+        self.rule_state = rule_state
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.effective_end_time is not None:
+            result['EffectiveEndTime'] = self.effective_end_time
+        if self.effective_start_time is not None:
+            result['EffectiveStartTime'] = self.effective_start_time
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.rule_state is not None:
+            result['RuleState'] = self.rule_state
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('EffectiveEndTime') is not None:
+            self.effective_end_time = m.get('EffectiveEndTime')
+        if m.get('EffectiveStartTime') is not None:
+            self.effective_start_time = m.get('EffectiveStartTime')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('RuleState') is not None:
+            self.rule_state = m.get('RuleState')
+        return self
+
+
+class ListRulesResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        rules: List[ListRulesResponseBodyRules] = None,
+        total_count: int = None,
+    ):
+        self.request_id = request_id
+        self.rules = rules
+        self.total_count = total_count
+
+    def validate(self):
+        if self.rules:
+            for k in self.rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Rules'] = []
+        if self.rules is not None:
+            for k in self.rules:
+                result['Rules'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.rules = []
+        if m.get('Rules') is not None:
+            for k in m.get('Rules'):
+                temp_model = ListRulesResponseBodyRules()
+                self.rules.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListRulesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListRulesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListRulesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListTagKeysRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
         resource_type: str = None,
@@ -11888,19 +20132,21 @@
 
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The ID of the request.
+        # The key of tag N.
+        # 
+        # Valid values of N: 1 to 20.
         self.key = key
-        # The type of the resource.
+        # The value of tag N.
         # 
-        # The returned value is INSTANCE, which indicates that the resource is a Bastionhost instance.
+        # Valid values of N: 1 to 20.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11928,27 +20174,25 @@
         self,
         next_token: str = None,
         region_id: str = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[ListTagResourcesRequestTag] = None,
     ):
-        # The region ID of the Bastionhost instance.
+        # The token for starting the next query.
         self.next_token = next_token
-        # The ID of the instance.
+        # The region ID of the Bastionhost instance.
         self.region_id = region_id
-        # The value of the tag.
+        # The IDs of instances. The ID is up to 20.
         self.resource_id = resource_id
-        # The operation that you want to perform.
+        # The type of the resource.
         # 
-        # Set the value to **ListTagResources**.
+        # Set the value to INSTANCE, which indicates that the resource is a Bastionhost instance.
         self.resource_type = resource_type
-        # The key of tag N.
-        # 
-        # Valid values of N: 1 to 20.
+        # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -11995,17 +20239,23 @@
     def __init__(
         self,
         resource_id: str = None,
         resource_type: str = None,
         tag_key: str = None,
         tag_value: str = None,
     ):
+        # The ID of the instance.
         self.resource_id = resource_id
+        # The type of the resource.
+        # 
+        # The returned value is INSTANCE, which indicates that the resource is a Bastionhost instance.
         self.resource_type = resource_type
+        # The key of the tag.
         self.tag_key = tag_key
+        # The value of the tag.
         self.tag_value = tag_value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12039,19 +20289,21 @@
 class ListTagResourcesResponseBody(TeaModel):
     def __init__(
         self,
         next_token: str = None,
         request_id: str = None,
         tag_resources: List[ListTagResourcesResponseBodyTagResources] = None,
     ):
-        # Queries the tags bound to one or more Bastionhost instances.
+        # The token for starting the next query.
         self.next_token = next_token
-        # ListTagResources
+        # The ID of the request.
         self.request_id = request_id
-        # 58928
+        # The information about Bastionhost instances and the tags bound to Bastionhost instances.
+        # 
+        # The following information is included: instance ID, resource type, tag key, and tag value.
         self.tag_resources = tag_resources
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -13083,14 +21335,294 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = LockUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDatabaseRequest(TeaModel):
+    def __init__(
+        self,
+        active_address_type: str = None,
+        comment: str = None,
+        database_id: str = None,
+        database_name: str = None,
+        database_port: str = None,
+        database_private_address: str = None,
+        database_public_address: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        region_id: str = None,
+        source_instance_id: str = None,
+    ):
+        self.active_address_type = active_address_type
+        self.comment = comment
+        self.database_id = database_id
+        self.database_name = database_name
+        self.database_port = database_port
+        self.database_private_address = database_private_address
+        self.database_public_address = database_public_address
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.region_id = region_id
+        self.source_instance_id = source_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.active_address_type is not None:
+            result['ActiveAddressType'] = self.active_address_type
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.database_name is not None:
+            result['DatabaseName'] = self.database_name
+        if self.database_port is not None:
+            result['DatabasePort'] = self.database_port
+        if self.database_private_address is not None:
+            result['DatabasePrivateAddress'] = self.database_private_address
+        if self.database_public_address is not None:
+            result['DatabasePublicAddress'] = self.database_public_address
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.source_instance_id is not None:
+            result['SourceInstanceId'] = self.source_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ActiveAddressType') is not None:
+            self.active_address_type = m.get('ActiveAddressType')
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('DatabaseName') is not None:
+            self.database_name = m.get('DatabaseName')
+        if m.get('DatabasePort') is not None:
+            self.database_port = m.get('DatabasePort')
+        if m.get('DatabasePrivateAddress') is not None:
+            self.database_private_address = m.get('DatabasePrivateAddress')
+        if m.get('DatabasePublicAddress') is not None:
+            self.database_public_address = m.get('DatabasePublicAddress')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('SourceInstanceId') is not None:
+            self.source_instance_id = m.get('SourceInstanceId')
+        return self
+
+
+class ModifyDatabaseResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatabaseResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyDatabaseResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyDatabaseResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ModifyDatabaseAccountRequest(TeaModel):
+    def __init__(
+        self,
+        database_account_id: str = None,
+        database_account_name: str = None,
+        database_schema: str = None,
+        instance_id: str = None,
+        password: str = None,
+        region_id: str = None,
+    ):
+        self.database_account_id = database_account_id
+        self.database_account_name = database_account_name
+        self.database_schema = database_schema
+        self.instance_id = instance_id
+        self.password = password
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        if self.database_account_name is not None:
+            result['DatabaseAccountName'] = self.database_account_name
+        if self.database_schema is not None:
+            result['DatabaseSchema'] = self.database_schema
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('DatabaseAccountName') is not None:
+            self.database_account_name = m.get('DatabaseAccountName')
+        if m.get('DatabaseSchema') is not None:
+            self.database_schema = m.get('DatabaseSchema')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ModifyDatabaseAccountResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatabaseAccountResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyDatabaseAccountResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyDatabaseAccountResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyHostRequest(TeaModel):
     def __init__(
         self,
         comment: str = None,
         host_id: str = None,
         host_name: str = None,
         host_private_address: str = None,
@@ -13410,29 +21942,29 @@
         self,
         comment: str = None,
         host_group_id: str = None,
         host_group_name: str = None,
         instance_id: str = None,
         region_id: str = None,
     ):
-        # The new name of the host group. The name can be up to 128 characters in length.
+        # The new description of the host group. The value can be up to 500 characters in length.
         self.comment = comment
-        # The region ID of the Bastionhost instance where you want to modify the information of the host group.
-        # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.host_group_id = host_group_id
         # The ID of the host group that you want to modify.
         # 
-        # >  You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        self.host_group_id = host_group_id
+        # The new name of the host group. The name can be up to 128 characters in length.
         self.host_group_name = host_group_name
-        # The ID of the request.
+        # The ID of the bastion host on which you want to modify the information about the host group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id
-        # The ID of the Bastionhost instance where you want to modify the information of the host group.
+        # The region ID of the bastion host on which you want to modify the information about the host group.
         # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14691,14 +23223,621 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceTwoFactorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyNetworkDomainRequestProxies(TeaModel):
+    def __init__(
+        self,
+        address: str = None,
+        node_type: str = None,
+        password: str = None,
+        port: int = None,
+        proxy_type: str = None,
+        user: str = None,
+    ):
+        self.address = address
+        self.node_type = node_type
+        self.password = password
+        self.port = port
+        self.proxy_type = proxy_type
+        self.user = user
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.address is not None:
+            result['Address'] = self.address
+        if self.node_type is not None:
+            result['NodeType'] = self.node_type
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.proxy_type is not None:
+            result['ProxyType'] = self.proxy_type
+        if self.user is not None:
+            result['User'] = self.user
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Address') is not None:
+            self.address = m.get('Address')
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('ProxyType') is not None:
+            self.proxy_type = m.get('ProxyType')
+        if m.get('User') is not None:
+            self.user = m.get('User')
+        return self
+
+
+class ModifyNetworkDomainRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        network_domain_name: str = None,
+        network_domain_type: str = None,
+        proxies: List[ModifyNetworkDomainRequestProxies] = None,
+        region_id: str = None,
+    ):
+        self.comment = comment
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.network_domain_name = network_domain_name
+        self.network_domain_type = network_domain_type
+        self.proxies = proxies
+        self.region_id = region_id
+
+    def validate(self):
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.network_domain_name is not None:
+            result['NetworkDomainName'] = self.network_domain_name
+        if self.network_domain_type is not None:
+            result['NetworkDomainType'] = self.network_domain_type
+        result['Proxies'] = []
+        if self.proxies is not None:
+            for k in self.proxies:
+                result['Proxies'].append(k.to_map() if k else None)
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('NetworkDomainName') is not None:
+            self.network_domain_name = m.get('NetworkDomainName')
+        if m.get('NetworkDomainType') is not None:
+            self.network_domain_type = m.get('NetworkDomainType')
+        self.proxies = []
+        if m.get('Proxies') is not None:
+            for k in m.get('Proxies'):
+                temp_model = ModifyNetworkDomainRequestProxies()
+                self.proxies.append(temp_model.from_map(k))
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ModifyNetworkDomainResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyNetworkDomainResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyNetworkDomainResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ModifyPolicyRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        policy_name: str = None,
+        priority: str = None,
+        region_id: str = None,
+    ):
+        self.comment = comment
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.policy_name = policy_name
+        self.priority = priority
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.policy_name is not None:
+            result['PolicyName'] = self.policy_name
+        if self.priority is not None:
+            result['Priority'] = self.priority
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('PolicyName') is not None:
+            self.policy_name = m.get('PolicyName')
+        if m.get('Priority') is not None:
+            self.priority = m.get('Priority')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ModifyPolicyResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyPolicyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyPolicyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyPolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ModifyRuleRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class ModifyRuleRequestHostGroups(TeaModel):
+    def __init__(
+        self,
+        host_account_names: List[str] = None,
+        host_group_id: str = None,
+    ):
+        self.host_account_names = host_account_names
+        self.host_group_id = host_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_names is not None:
+            result['HostAccountNames'] = self.host_account_names
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class ModifyRuleRequestHosts(TeaModel):
+    def __init__(
+        self,
+        host_account_ids: List[str] = None,
+        host_id: str = None,
+    ):
+        self.host_account_ids = host_account_ids
+        self.host_id = host_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_ids is not None:
+            result['HostAccountIds'] = self.host_account_ids
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class ModifyRuleRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        databases: List[ModifyRuleRequestDatabases] = None,
+        effective_end_time: int = None,
+        effective_start_time: int = None,
+        host_groups: List[ModifyRuleRequestHostGroups] = None,
+        hosts: List[ModifyRuleRequestHosts] = None,
+        instance_id: str = None,
+        region_id: str = None,
+        rule_id: str = None,
+        rule_name: str = None,
+        user_group_ids: List[str] = None,
+        user_ids: List[str] = None,
+    ):
+        self.comment = comment
+        self.databases = databases
+        self.effective_end_time = effective_end_time
+        self.effective_start_time = effective_start_time
+        self.host_groups = host_groups
+        self.hosts = hosts
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.rule_id = rule_id
+        self.rule_name = rule_name
+        self.user_group_ids = user_group_ids
+        self.user_ids = user_ids
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+        if self.host_groups:
+            for k in self.host_groups:
+                if k:
+                    k.validate()
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        if self.effective_end_time is not None:
+            result['EffectiveEndTime'] = self.effective_end_time
+        if self.effective_start_time is not None:
+            result['EffectiveStartTime'] = self.effective_start_time
+        result['HostGroups'] = []
+        if self.host_groups is not None:
+            for k in self.host_groups:
+                result['HostGroups'].append(k.to_map() if k else None)
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.rule_id is not None:
+            result['RuleId'] = self.rule_id
+        if self.rule_name is not None:
+            result['RuleName'] = self.rule_name
+        if self.user_group_ids is not None:
+            result['UserGroupIds'] = self.user_group_ids
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = ModifyRuleRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        if m.get('EffectiveEndTime') is not None:
+            self.effective_end_time = m.get('EffectiveEndTime')
+        if m.get('EffectiveStartTime') is not None:
+            self.effective_start_time = m.get('EffectiveStartTime')
+        self.host_groups = []
+        if m.get('HostGroups') is not None:
+            for k in m.get('HostGroups'):
+                temp_model = ModifyRuleRequestHostGroups()
+                self.host_groups.append(temp_model.from_map(k))
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = ModifyRuleRequestHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        if m.get('RuleName') is not None:
+            self.rule_name = m.get('RuleName')
+        if m.get('UserGroupIds') is not None:
+            self.user_group_ids = m.get('UserGroupIds')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class ModifyRuleResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyRuleResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyRuleResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyRuleResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyUserRequest(TeaModel):
     def __init__(
         self,
         comment: str = None,
         display_name: str = None,
         effective_end_time: int = None,
         effective_start_time: int = None,
@@ -15065,14 +24204,484 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyUserPublicKeyRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        instance_id: str = None,
+        public_key: str = None,
+        public_key_id: str = None,
+        public_key_name: str = None,
+        region_id: str = None,
+    ):
+        # The new description of the user group. The description can be up to 500 characters in length.
+        self.comment = comment
+        # The ID of the bastion host that is used to modify the public key of the user.
+        # 
+        # > You can call the [describeinstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id
+        # The new public key.
+        # 
+        # > The public key must be encoded in Base64.
+        self.public_key = public_key
+        # The ID of the public key that you want to modify.
+        self.public_key_id = public_key_id
+        # The name of the public key that you want to modify. This name can be up to 128 characters in length.
+        self.public_key_name = public_key_name
+        # The region ID of the bastion host that is used to modify the public key of the user.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.public_key is not None:
+            result['PublicKey'] = self.public_key
+        if self.public_key_id is not None:
+            result['PublicKeyId'] = self.public_key_id
+        if self.public_key_name is not None:
+            result['PublicKeyName'] = self.public_key_name
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PublicKey') is not None:
+            self.public_key = m.get('PublicKey')
+        if m.get('PublicKeyId') is not None:
+            self.public_key_id = m.get('PublicKeyId')
+        if m.get('PublicKeyName') is not None:
+            self.public_key_name = m.get('PublicKeyName')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class ModifyUserPublicKeyResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The ID of the request, which is used to locate and troubleshoot issues.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyUserPublicKeyResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyUserPublicKeyResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyUserPublicKeyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class MoveDatabasesToNetworkDomainRequest(TeaModel):
+    def __init__(
+        self,
+        database_ids: List[str] = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_ids = database_ids
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_ids is not None:
+            result['DatabaseIds'] = self.database_ids
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseIds') is not None:
+            self.database_ids = m.get('DatabaseIds')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class MoveDatabasesToNetworkDomainResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_id = database_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class MoveDatabasesToNetworkDomainResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[MoveDatabasesToNetworkDomainResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = MoveDatabasesToNetworkDomainResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class MoveDatabasesToNetworkDomainResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MoveDatabasesToNetworkDomainResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MoveDatabasesToNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class MoveHostsToNetworkDomainRequest(TeaModel):
+    def __init__(
+        self,
+        host_ids: List[str] = None,
+        instance_id: str = None,
+        network_domain_id: str = None,
+        region_id: str = None,
+    ):
+        self.host_ids = host_ids
+        self.instance_id = instance_id
+        self.network_domain_id = network_domain_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_ids is not None:
+            result['HostIds'] = self.host_ids
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.network_domain_id is not None:
+            result['NetworkDomainId'] = self.network_domain_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('HostIds') is not None:
+            self.host_ids = m.get('HostIds')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class MoveHostsToNetworkDomainResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        host_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.host_id = host_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class MoveHostsToNetworkDomainResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[MoveHostsToNetworkDomainResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = MoveHostsToNetworkDomainResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class MoveHostsToNetworkDomainResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: MoveHostsToNetworkDomainResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = MoveHostsToNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class MoveResourceGroupRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         resource_group_id: str = None,
         resource_id: str = None,
         resource_type: str = None,
@@ -15409,14 +25018,186 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RejectOperationTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RemoveDatabasesFromGroupRequest(TeaModel):
+    def __init__(
+        self,
+        database_ids: List[str] = None,
+        host_group_id: str = None,
+        instance_id: str = None,
+        region_id: str = None,
+    ):
+        self.database_ids = database_ids
+        self.host_group_id = host_group_id
+        self.instance_id = instance_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_ids is not None:
+            result['DatabaseIds'] = self.database_ids
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DatabaseIds') is not None:
+            self.database_ids = m.get('DatabaseIds')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class RemoveDatabasesFromGroupResponseBodyResults(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        database_id: str = None,
+        host_group_id: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.database_id = database_id
+        self.host_group_id = host_group_id
+        self.message = message
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        if self.message is not None:
+            result['Message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        return self
+
+
+class RemoveDatabasesFromGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        results: List[RemoveDatabasesFromGroupResponseBodyResults] = None,
+    ):
+        self.request_id = request_id
+        self.results = results
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Results'] = []
+        if self.results is not None:
+            for k in self.results:
+                result['Results'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.results = []
+        if m.get('Results') is not None:
+            for k in m.get('Results'):
+                temp_model = RemoveDatabasesFromGroupResponseBodyResults()
+                self.results.append(temp_model.from_map(k))
+        return self
+
+
+class RemoveDatabasesFromGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RemoveDatabasesFromGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RemoveDatabasesFromGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RemoveHostsFromGroupRequest(TeaModel):
     def __init__(
         self,
         host_group_id: str = None,
         host_ids: str = None,
         instance_id: str = None,
         region_id: str = None,
@@ -15809,14 +25590,121 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveUsersFromGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RenewAssetOperationTokenRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        token_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.region_id = region_id
+        self.token_id = token_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.token_id is not None:
+            result['TokenId'] = self.token_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('TokenId') is not None:
+            self.token_id = m.get('TokenId')
+        return self
+
+
+class RenewAssetOperationTokenResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RenewAssetOperationTokenResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RenewAssetOperationTokenResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = RenewAssetOperationTokenResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ResetHostAccountCredentialRequest(TeaModel):
     def __init__(
         self,
         credential_type: str = None,
         host_account_id: str = None,
         instance_id: str = None,
         region_id: str = None,
@@ -15936,14 +25824,1603 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResetHostAccountCredentialResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime(TeaModel):
+    def __init__(
+        self,
+        days: List[int] = None,
+        hours: List[int] = None,
+    ):
+        self.days = days
+        self.hours = hours
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.days is not None:
+            result['Days'] = self.days
+        if self.hours is not None:
+            result['Hours'] = self.hours
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Days') is not None:
+            self.days = m.get('Days')
+        if m.get('Hours') is not None:
+            self.hours = m.get('Hours')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig(TeaModel):
+    def __init__(
+        self,
+        effective_time: List[SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime] = None,
+    ):
+        self.effective_time = effective_time
+
+    def validate(self):
+        if self.effective_time:
+            for k in self.effective_time:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['EffectiveTime'] = []
+        if self.effective_time is not None:
+            for k in self.effective_time:
+                result['EffectiveTime'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.effective_time = []
+        if m.get('EffectiveTime') is not None:
+            for k in m.get('EffectiveTime'):
+                temp_model = SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime()
+                self.effective_time.append(temp_model.from_map(k))
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigRequest(TeaModel):
+    def __init__(
+        self,
+        access_time_range_config: SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.access_time_range_config = access_time_range_config
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        if self.access_time_range_config:
+            self.access_time_range_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_time_range_config is not None:
+            result['AccessTimeRangeConfig'] = self.access_time_range_config.to_map()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessTimeRangeConfig') is not None:
+            temp_model = SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig()
+            self.access_time_range_config = temp_model.from_map(m['AccessTimeRangeConfig'])
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        access_time_range_config_shrink: str = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.access_time_range_config_shrink = access_time_range_config_shrink
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_time_range_config_shrink is not None:
+            result['AccessTimeRangeConfig'] = self.access_time_range_config_shrink
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessTimeRangeConfig') is not None:
+            self.access_time_range_config_shrink = m.get('AccessTimeRangeConfig')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyAccessTimeRangeConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyAccessTimeRangeConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyApprovalConfigRequestApprovalConfig(TeaModel):
+    def __init__(
+        self,
+        switch_status: str = None,
+    ):
+        self.switch_status = switch_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.switch_status is not None:
+            result['SwitchStatus'] = self.switch_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SwitchStatus') is not None:
+            self.switch_status = m.get('SwitchStatus')
+        return self
+
+
+class SetPolicyApprovalConfigRequest(TeaModel):
+    def __init__(
+        self,
+        approval_config: SetPolicyApprovalConfigRequestApprovalConfig = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.approval_config = approval_config
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        if self.approval_config:
+            self.approval_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approval_config is not None:
+            result['ApprovalConfig'] = self.approval_config.to_map()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApprovalConfig') is not None:
+            temp_model = SetPolicyApprovalConfigRequestApprovalConfig()
+            self.approval_config = temp_model.from_map(m['ApprovalConfig'])
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyApprovalConfigShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        approval_config_shrink: str = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.approval_config_shrink = approval_config_shrink
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approval_config_shrink is not None:
+            result['ApprovalConfig'] = self.approval_config_shrink
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApprovalConfig') is not None:
+            self.approval_config_shrink = m.get('ApprovalConfig')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyApprovalConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyApprovalConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyApprovalConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyApprovalConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyAssetScopeRequestDatabases(TeaModel):
+    def __init__(
+        self,
+        account_scope_type: str = None,
+        database_account_ids: List[str] = None,
+        database_id: str = None,
+    ):
+        self.account_scope_type = account_scope_type
+        self.database_account_ids = database_account_ids
+        self.database_id = database_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.database_account_ids is not None:
+            result['DatabaseAccountIds'] = self.database_account_ids
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class SetPolicyAssetScopeRequestHostGroups(TeaModel):
+    def __init__(
+        self,
+        account_names: List[str] = None,
+        account_scope_type: str = None,
+        host_group_id: str = None,
+    ):
+        self.account_names = account_names
+        self.account_scope_type = account_scope_type
+        self.host_group_id = host_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_names is not None:
+            result['AccountNames'] = self.account_names
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.host_group_id is not None:
+            result['HostGroupId'] = self.host_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountNames') is not None:
+            self.account_names = m.get('AccountNames')
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class SetPolicyAssetScopeRequestHosts(TeaModel):
+    def __init__(
+        self,
+        account_scope_type: str = None,
+        host_account_ids: List[str] = None,
+        host_id: str = None,
+    ):
+        self.account_scope_type = account_scope_type
+        self.host_account_ids = host_account_ids
+        self.host_id = host_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_scope_type is not None:
+            result['AccountScopeType'] = self.account_scope_type
+        if self.host_account_ids is not None:
+            result['HostAccountIds'] = self.host_account_ids
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccountScopeType') is not None:
+            self.account_scope_type = m.get('AccountScopeType')
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class SetPolicyAssetScopeRequest(TeaModel):
+    def __init__(
+        self,
+        databases: List[SetPolicyAssetScopeRequestDatabases] = None,
+        host_groups: List[SetPolicyAssetScopeRequestHostGroups] = None,
+        hosts: List[SetPolicyAssetScopeRequestHosts] = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+        scope_type: str = None,
+    ):
+        self.databases = databases
+        self.host_groups = host_groups
+        self.hosts = hosts
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+        self.scope_type = scope_type
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+        if self.host_groups:
+            for k in self.host_groups:
+                if k:
+                    k.validate()
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Databases'] = []
+        if self.databases is not None:
+            for k in self.databases:
+                result['Databases'].append(k.to_map() if k else None)
+        result['HostGroups'] = []
+        if self.host_groups is not None:
+            for k in self.host_groups:
+                result['HostGroups'].append(k.to_map() if k else None)
+        result['Hosts'] = []
+        if self.hosts is not None:
+            for k in self.hosts:
+                result['Hosts'].append(k.to_map() if k else None)
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.databases = []
+        if m.get('Databases') is not None:
+            for k in m.get('Databases'):
+                temp_model = SetPolicyAssetScopeRequestDatabases()
+                self.databases.append(temp_model.from_map(k))
+        self.host_groups = []
+        if m.get('HostGroups') is not None:
+            for k in m.get('HostGroups'):
+                temp_model = SetPolicyAssetScopeRequestHostGroups()
+                self.host_groups.append(temp_model.from_map(k))
+        self.hosts = []
+        if m.get('Hosts') is not None:
+            for k in m.get('Hosts'):
+                temp_model = SetPolicyAssetScopeRequestHosts()
+                self.hosts.append(temp_model.from_map(k))
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
+        return self
+
+
+class SetPolicyAssetScopeResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyAssetScopeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyAssetScopeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyAssetScopeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyCommandConfigRequestCommandConfigApproval(TeaModel):
+    def __init__(
+        self,
+        commands: List[str] = None,
+    ):
+        self.commands = commands
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.commands is not None:
+            result['Commands'] = self.commands
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class SetPolicyCommandConfigRequestCommandConfigDeny(TeaModel):
+    def __init__(
+        self,
+        acl_type: str = None,
+        commands: List[str] = None,
+    ):
+        self.acl_type = acl_type
+        self.commands = commands
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.acl_type is not None:
+            result['AclType'] = self.acl_type
+        if self.commands is not None:
+            result['Commands'] = self.commands
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class SetPolicyCommandConfigRequestCommandConfig(TeaModel):
+    def __init__(
+        self,
+        approval: SetPolicyCommandConfigRequestCommandConfigApproval = None,
+        deny: SetPolicyCommandConfigRequestCommandConfigDeny = None,
+    ):
+        self.approval = approval
+        self.deny = deny
+
+    def validate(self):
+        if self.approval:
+            self.approval.validate()
+        if self.deny:
+            self.deny.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approval is not None:
+            result['Approval'] = self.approval.to_map()
+        if self.deny is not None:
+            result['Deny'] = self.deny.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Approval') is not None:
+            temp_model = SetPolicyCommandConfigRequestCommandConfigApproval()
+            self.approval = temp_model.from_map(m['Approval'])
+        if m.get('Deny') is not None:
+            temp_model = SetPolicyCommandConfigRequestCommandConfigDeny()
+            self.deny = temp_model.from_map(m['Deny'])
+        return self
+
+
+class SetPolicyCommandConfigRequest(TeaModel):
+    def __init__(
+        self,
+        command_config: SetPolicyCommandConfigRequestCommandConfig = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.command_config = command_config
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        if self.command_config:
+            self.command_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.command_config is not None:
+            result['CommandConfig'] = self.command_config.to_map()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CommandConfig') is not None:
+            temp_model = SetPolicyCommandConfigRequestCommandConfig()
+            self.command_config = temp_model.from_map(m['CommandConfig'])
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyCommandConfigShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        command_config_shrink: str = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.command_config_shrink = command_config_shrink
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.command_config_shrink is not None:
+            result['CommandConfig'] = self.command_config_shrink
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CommandConfig') is not None:
+            self.command_config_shrink = m.get('CommandConfig')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyCommandConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyCommandConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyCommandConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyCommandConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyIPAclConfigRequestIPAclConfig(TeaModel):
+    def __init__(
+        self,
+        acl_type: str = None,
+        ips: List[str] = None,
+    ):
+        self.acl_type = acl_type
+        self.ips = ips
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.acl_type is not None:
+            result['AclType'] = self.acl_type
+        if self.ips is not None:
+            result['IPs'] = self.ips
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('IPs') is not None:
+            self.ips = m.get('IPs')
+        return self
+
+
+class SetPolicyIPAclConfigRequest(TeaModel):
+    def __init__(
+        self,
+        ipacl_config: SetPolicyIPAclConfigRequestIPAclConfig = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.ipacl_config = ipacl_config
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        if self.ipacl_config:
+            self.ipacl_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ipacl_config is not None:
+            result['IPAclConfig'] = self.ipacl_config.to_map()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IPAclConfig') is not None:
+            temp_model = SetPolicyIPAclConfigRequestIPAclConfig()
+            self.ipacl_config = temp_model.from_map(m['IPAclConfig'])
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyIPAclConfigShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        ipacl_config_shrink: str = None,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+    ):
+        self.ipacl_config_shrink = ipacl_config_shrink
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ipacl_config_shrink is not None:
+            result['IPAclConfig'] = self.ipacl_config_shrink
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('IPAclConfig') is not None:
+            self.ipacl_config_shrink = m.get('IPAclConfig')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyIPAclConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyIPAclConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyIPAclConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyIPAclConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyProtocolConfigRequestProtocolConfigRDP(TeaModel):
+    def __init__(
+        self,
+        clipboard_download: str = None,
+        clipboard_upload: str = None,
+        disk_redirection: str = None,
+        record_keyboard: str = None,
+    ):
+        self.clipboard_download = clipboard_download
+        self.clipboard_upload = clipboard_upload
+        self.disk_redirection = disk_redirection
+        self.record_keyboard = record_keyboard
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.clipboard_download is not None:
+            result['ClipboardDownload'] = self.clipboard_download
+        if self.clipboard_upload is not None:
+            result['ClipboardUpload'] = self.clipboard_upload
+        if self.disk_redirection is not None:
+            result['DiskRedirection'] = self.disk_redirection
+        if self.record_keyboard is not None:
+            result['RecordKeyboard'] = self.record_keyboard
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClipboardDownload') is not None:
+            self.clipboard_download = m.get('ClipboardDownload')
+        if m.get('ClipboardUpload') is not None:
+            self.clipboard_upload = m.get('ClipboardUpload')
+        if m.get('DiskRedirection') is not None:
+            self.disk_redirection = m.get('DiskRedirection')
+        if m.get('RecordKeyboard') is not None:
+            self.record_keyboard = m.get('RecordKeyboard')
+        return self
+
+
+class SetPolicyProtocolConfigRequestProtocolConfigSSH(TeaModel):
+    def __init__(
+        self,
+        exec_command: str = None,
+        sftpchannel: str = None,
+        sftpdownload_file: str = None,
+        sftpmkdir: str = None,
+        sftpremove_file: str = None,
+        sftprename_file: str = None,
+        sftprmdir: str = None,
+        sftpupload_file: str = None,
+        sshchannel: str = None,
+        x_11forwarding: str = None,
+    ):
+        self.exec_command = exec_command
+        self.sftpchannel = sftpchannel
+        self.sftpdownload_file = sftpdownload_file
+        self.sftpmkdir = sftpmkdir
+        self.sftpremove_file = sftpremove_file
+        self.sftprename_file = sftprename_file
+        self.sftprmdir = sftprmdir
+        self.sftpupload_file = sftpupload_file
+        self.sshchannel = sshchannel
+        self.x_11forwarding = x_11forwarding
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.exec_command is not None:
+            result['ExecCommand'] = self.exec_command
+        if self.sftpchannel is not None:
+            result['SFTPChannel'] = self.sftpchannel
+        if self.sftpdownload_file is not None:
+            result['SFTPDownloadFile'] = self.sftpdownload_file
+        if self.sftpmkdir is not None:
+            result['SFTPMkdir'] = self.sftpmkdir
+        if self.sftpremove_file is not None:
+            result['SFTPRemoveFile'] = self.sftpremove_file
+        if self.sftprename_file is not None:
+            result['SFTPRenameFile'] = self.sftprename_file
+        if self.sftprmdir is not None:
+            result['SFTPRmdir'] = self.sftprmdir
+        if self.sftpupload_file is not None:
+            result['SFTPUploadFile'] = self.sftpupload_file
+        if self.sshchannel is not None:
+            result['SSHChannel'] = self.sshchannel
+        if self.x_11forwarding is not None:
+            result['X11Forwarding'] = self.x_11forwarding
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExecCommand') is not None:
+            self.exec_command = m.get('ExecCommand')
+        if m.get('SFTPChannel') is not None:
+            self.sftpchannel = m.get('SFTPChannel')
+        if m.get('SFTPDownloadFile') is not None:
+            self.sftpdownload_file = m.get('SFTPDownloadFile')
+        if m.get('SFTPMkdir') is not None:
+            self.sftpmkdir = m.get('SFTPMkdir')
+        if m.get('SFTPRemoveFile') is not None:
+            self.sftpremove_file = m.get('SFTPRemoveFile')
+        if m.get('SFTPRenameFile') is not None:
+            self.sftprename_file = m.get('SFTPRenameFile')
+        if m.get('SFTPRmdir') is not None:
+            self.sftprmdir = m.get('SFTPRmdir')
+        if m.get('SFTPUploadFile') is not None:
+            self.sftpupload_file = m.get('SFTPUploadFile')
+        if m.get('SSHChannel') is not None:
+            self.sshchannel = m.get('SSHChannel')
+        if m.get('X11Forwarding') is not None:
+            self.x_11forwarding = m.get('X11Forwarding')
+        return self
+
+
+class SetPolicyProtocolConfigRequestProtocolConfig(TeaModel):
+    def __init__(
+        self,
+        rdp: SetPolicyProtocolConfigRequestProtocolConfigRDP = None,
+        ssh: SetPolicyProtocolConfigRequestProtocolConfigSSH = None,
+    ):
+        self.rdp = rdp
+        self.ssh = ssh
+
+    def validate(self):
+        if self.rdp:
+            self.rdp.validate()
+        if self.ssh:
+            self.ssh.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.rdp is not None:
+            result['RDP'] = self.rdp.to_map()
+        if self.ssh is not None:
+            result['SSH'] = self.ssh.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RDP') is not None:
+            temp_model = SetPolicyProtocolConfigRequestProtocolConfigRDP()
+            self.rdp = temp_model.from_map(m['RDP'])
+        if m.get('SSH') is not None:
+            temp_model = SetPolicyProtocolConfigRequestProtocolConfigSSH()
+            self.ssh = temp_model.from_map(m['SSH'])
+        return self
+
+
+class SetPolicyProtocolConfigRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        policy_id: str = None,
+        protocol_config: SetPolicyProtocolConfigRequestProtocolConfig = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.protocol_config = protocol_config
+        self.region_id = region_id
+
+    def validate(self):
+        if self.protocol_config:
+            self.protocol_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.protocol_config is not None:
+            result['ProtocolConfig'] = self.protocol_config.to_map()
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('ProtocolConfig') is not None:
+            temp_model = SetPolicyProtocolConfigRequestProtocolConfig()
+            self.protocol_config = temp_model.from_map(m['ProtocolConfig'])
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyProtocolConfigShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        policy_id: str = None,
+        protocol_config_shrink: str = None,
+        region_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.protocol_config_shrink = protocol_config_shrink
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.protocol_config_shrink is not None:
+            result['ProtocolConfig'] = self.protocol_config_shrink
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('ProtocolConfig') is not None:
+            self.protocol_config_shrink = m.get('ProtocolConfig')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        return self
+
+
+class SetPolicyProtocolConfigResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyProtocolConfigResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyProtocolConfigResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyProtocolConfigResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class SetPolicyUserScopeRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        policy_id: str = None,
+        region_id: str = None,
+        scope_type: str = None,
+        user_group_ids: List[str] = None,
+        user_ids: List[str] = None,
+    ):
+        self.instance_id = instance_id
+        self.policy_id = policy_id
+        self.region_id = region_id
+        self.scope_type = scope_type
+        self.user_group_ids = user_group_ids
+        self.user_ids = user_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        if self.user_group_ids is not None:
+            result['UserGroupIds'] = self.user_group_ids
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
+        if m.get('UserGroupIds') is not None:
+            self.user_group_ids = m.get('UserGroupIds')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class SetPolicyUserScopeResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyUserScopeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SetPolicyUserScopeResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SetPolicyUserScopeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class StartInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         region_id: str = None,
         security_group_ids: List[str] = None,
         vswitch_id: str = None,
@@ -16575,7 +28052,311 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class VerifyInstanceADAuthServerRequest(TeaModel):
+    def __init__(
+        self,
+        account: str = None,
+        base_dn: str = None,
+        domain: str = None,
+        filter: str = None,
+        instance_id: str = None,
+        is_ssl: str = None,
+        password: str = None,
+        port: str = None,
+        region_id: str = None,
+        server: str = None,
+        standby_server: str = None,
+    ):
+        self.account = account
+        self.base_dn = base_dn
+        self.domain = domain
+        self.filter = filter
+        self.instance_id = instance_id
+        self.is_ssl = is_ssl
+        self.password = password
+        self.port = port
+        self.region_id = region_id
+        self.server = server
+        self.standby_server = standby_server
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account is not None:
+            result['Account'] = self.account
+        if self.base_dn is not None:
+            result['BaseDN'] = self.base_dn
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.filter is not None:
+            result['Filter'] = self.filter
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.is_ssl is not None:
+            result['IsSSL'] = self.is_ssl
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.standby_server is not None:
+            result['StandbyServer'] = self.standby_server
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Account') is not None:
+            self.account = m.get('Account')
+        if m.get('BaseDN') is not None:
+            self.base_dn = m.get('BaseDN')
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('Filter') is not None:
+            self.filter = m.get('Filter')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('IsSSL') is not None:
+            self.is_ssl = m.get('IsSSL')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('StandbyServer') is not None:
+            self.standby_server = m.get('StandbyServer')
+        return self
+
+
+class VerifyInstanceADAuthServerResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VerifyInstanceADAuthServerResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: VerifyInstanceADAuthServerResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VerifyInstanceADAuthServerResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class VerifyInstanceLDAPAuthServerRequest(TeaModel):
+    def __init__(
+        self,
+        account: str = None,
+        base_dn: str = None,
+        filter: str = None,
+        instance_id: str = None,
+        is_ssl: str = None,
+        password: str = None,
+        port: str = None,
+        region_id: str = None,
+        server: str = None,
+        standby_server: str = None,
+    ):
+        self.account = account
+        self.base_dn = base_dn
+        self.filter = filter
+        self.instance_id = instance_id
+        self.is_ssl = is_ssl
+        self.password = password
+        self.port = port
+        self.region_id = region_id
+        self.server = server
+        self.standby_server = standby_server
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account is not None:
+            result['Account'] = self.account
+        if self.base_dn is not None:
+            result['BaseDN'] = self.base_dn
+        if self.filter is not None:
+            result['Filter'] = self.filter
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.is_ssl is not None:
+            result['IsSSL'] = self.is_ssl
+        if self.password is not None:
+            result['Password'] = self.password
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.standby_server is not None:
+            result['StandbyServer'] = self.standby_server
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Account') is not None:
+            self.account = m.get('Account')
+        if m.get('BaseDN') is not None:
+            self.base_dn = m.get('BaseDN')
+        if m.get('Filter') is not None:
+            self.filter = m.get('Filter')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('IsSSL') is not None:
+            self.is_ssl = m.get('IsSSL')
+        if m.get('Password') is not None:
+            self.password = m.get('Password')
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('StandbyServer') is not None:
+            self.standby_server = m.get('StandbyServer')
+        return self
+
+
+class VerifyInstanceLDAPAuthServerResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VerifyInstanceLDAPAuthServerResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: VerifyInstanceLDAPAuthServerResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = VerifyInstanceLDAPAuthServerResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/PKG-INFO` & `alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-yundun-bastionhost20191209
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/alibabacloud_yundun_bastionhost20191209.egg-info/SOURCES.txt` & `alibabacloud_yundun-bastionhost20191209-1.2.0/alibabacloud_yundun_bastionhost20191209.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209-1.1.2/setup.py` & `alibabacloud_yundun-bastionhost20191209-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_yundun-bastionhost20191209.
 
-Created on 28/02/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_yundun_bastionhost20191209"
 NAME = "alibabacloud_yundun-bastionhost20191209" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python"
```

