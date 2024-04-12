# Comparing `tmp/alibabacloud_yundun-bastionhost20191209_py2-1.1.2.tar.gz` & `tmp/alibabacloud_yundun-bastionhost20191209_py2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_yundun-bastionhost20191209_py2-1.1.2.tar", last modified: Wed Feb 28 17:14:49 2024, max compression
+gzip compressed data, was "dist/alibabacloud_yundun-bastionhost20191209_py2-1.2.0.tar", last modified: Fri Apr 12 17:12:19 2024, max compression
```

## Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2.tar` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      256 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2562 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1078 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1161 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152107 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/client.py
--rw-r--r--   0 root         (0) root         (0)   588525 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2562 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      560 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2980 2024-02-28 17:14:49.000000 alibabacloud_yundun-bastionhost20191209_py2-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      664 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1078 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1161 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   245482 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/client.py
+-rw-r--r--   0 root         (0) root         (0)   974209 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2562 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      560 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-12 17:12:19.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-12 17:12:18.000000 alibabacloud_yundun-bastionhost20191209_py2-1.2.0/setup.py
```

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/LICENSE` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/PKG-INFO` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_yundun-bastionhost20191209_py2
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/README-CN.md` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/README.md` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/client.py` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -116,14 +116,48 @@
         @param request: AcceptOperationTicketRequest
 
         @return: AcceptOperationTicketResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.accept_operation_ticket_with_options(request, runtime)
 
+    def add_databases_to_group_with_options(self, request, runtime):
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
+    def add_databases_to_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.add_databases_to_group_with_options(request, runtime)
+
     def add_hosts_to_group_with_options(self, request, runtime):
         """
         You can call this operation to add one or more hosts to a host group. You can add multiple hosts to a host group to manage and grant permissions on the hosts in a centralized manner.
         # Limits
         You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds a limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limits when you call this operation.
         
 
@@ -230,14 +264,82 @@
         @param request: AddUsersToGroupRequest
 
         @return: AddUsersToGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.add_users_to_group_with_options(request, runtime)
 
+    def attach_database_accounts_to_user_with_options(self, request, runtime):
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
+    def attach_database_accounts_to_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.attach_database_accounts_to_user_with_options(request, runtime)
+
+    def attach_database_accounts_to_user_group_with_options(self, request, runtime):
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
+    def attach_database_accounts_to_user_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.attach_database_accounts_to_user_group_with_options(request, runtime)
+
     def attach_host_accounts_to_host_share_key_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_account_ids):
             query['HostAccountIds'] = request.host_account_ids
         if not UtilClient.is_unset(request.host_share_key_id):
             query['HostShareKeyId'] = request.host_share_key_id
@@ -454,15 +556,18 @@
 
     def config_instance_security_groups(self, request):
         runtime = util_models.RuntimeOptions()
         return self.config_instance_security_groups_with_options(request, runtime)
 
     def config_instance_white_list_with_options(self, request, runtime):
         """
-        The ID of the request, which is used to locate and troubleshoot issues.
+        ## Usage notes
+        You can call this operation to configure a whitelist of public IP addresses for a bastion host. By default, a bastion host is accessible from all public IP addresses. If you want to allow the requests from specific public IP addresses, you can call this operation to add trusted IP addresses to the whitelist of the bastion host.
+        ## Limits
+        You can call this operation up to 30 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
 
         @param request: ConfigInstanceWhiteListRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: ConfigInstanceWhiteListResponse
@@ -492,24 +597,121 @@
         return TeaCore.from_map(
             yundun_bastionhost_20191209_models.ConfigInstanceWhiteListResponse(),
             self.call_api(params, req, runtime)
         )
 
     def config_instance_white_list(self, request):
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
 
+    def create_database_with_options(self, request, runtime):
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
+    def create_database(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_database_with_options(request, runtime)
+
+    def create_database_account_with_options(self, request, runtime):
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
+    def create_database_account(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_database_account_with_options(request, runtime)
+
     def create_host_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.active_address_type):
             query['ActiveAddressType'] = request.active_address_type
         if not UtilClient.is_unset(request.comment):
             query['Comment'] = request.comment
@@ -666,14 +868,136 @@
             self.call_api(params, req, runtime)
         )
 
     def create_host_share_key(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_host_share_key_with_options(request, runtime)
 
+    def create_network_domain_with_options(self, request, runtime):
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
+    def create_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_network_domain_with_options(request, runtime)
+
+    def create_policy_with_options(self, request, runtime):
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
+    def create_policy(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_policy_with_options(request, runtime)
+
+    def create_rule_with_options(self, request, runtime):
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
+    def create_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_rule_with_options(request, runtime)
+
     def create_user_with_options(self, request, runtime):
         """
         ## Usage notes
         You can call this operation to add a user to a bastion host. You can add local users and Resource Access Management (RAM) users. After a Bastionhost administrator adds a user to a bastion host, the O&M personnel can log on to the bastion host as the user to perform O&M operations on the host on which they have permissions.
         ## Limits
         You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
@@ -862,14 +1186,78 @@
         @param request: CreateUserPublicKeyRequest
 
         @return: CreateUserPublicKeyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_user_public_key_with_options(request, runtime)
 
+    def delete_database_with_options(self, request, runtime):
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
+    def delete_database(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_database_with_options(request, runtime)
+
+    def delete_database_account_with_options(self, request, runtime):
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
+    def delete_database_account(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_database_account_with_options(request, runtime)
+
     def delete_host_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_id):
             query['HostId'] = request.host_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -897,18 +1285,18 @@
     def delete_host(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_host_with_options(request, runtime)
 
     def delete_host_account_with_options(self, request, runtime):
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
@@ -939,18 +1327,18 @@
             yundun_bastionhost_20191209_models.DeleteHostAccountResponse(),
             self.call_api(params, req, runtime)
         )
 
     def delete_host_account(self, request):
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
@@ -1038,14 +1426,110 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_host_share_key(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_host_share_key_with_options(request, runtime)
 
+    def delete_network_domain_with_options(self, request, runtime):
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
+    def delete_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_network_domain_with_options(request, runtime)
+
+    def delete_policy_with_options(self, request, runtime):
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
+    def delete_policy(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_policy_with_options(request, runtime)
+
+    def delete_rule_with_options(self, request, runtime):
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
+    def delete_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_rule_with_options(request, runtime)
+
     def delete_user_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -1254,14 +1738,82 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_regions(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_regions_with_options(request, runtime)
 
+    def detach_database_accounts_from_user_with_options(self, request, runtime):
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
+    def detach_database_accounts_from_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.detach_database_accounts_from_user_with_options(request, runtime)
+
+    def detach_database_accounts_from_user_group_with_options(self, request, runtime):
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
+    def detach_database_accounts_from_user_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.detach_database_accounts_from_user_group_with_options(request, runtime)
+
     def detach_host_accounts_from_host_share_key_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_account_ids):
             query['HostAccountIds'] = request.host_account_ids
         if not UtilClient.is_unset(request.host_share_key_id):
             query['HostShareKeyId'] = request.host_share_key_id
@@ -1472,14 +2024,46 @@
             self.call_api(params, req, runtime)
         )
 
     def disable_instance_public_access(self, request):
         runtime = util_models.RuntimeOptions()
         return self.disable_instance_public_access_with_options(request, runtime)
 
+    def disable_rule_with_options(self, request, runtime):
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
+    def disable_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.disable_rule_with_options(request, runtime)
+
     def enable_instance_public_access_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -1502,14 +2086,152 @@
             self.call_api(params, req, runtime)
         )
 
     def enable_instance_public_access(self, request):
         runtime = util_models.RuntimeOptions()
         return self.enable_instance_public_access_with_options(request, runtime)
 
+    def enable_rule_with_options(self, request, runtime):
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
+    def enable_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.enable_rule_with_options(request, runtime)
+
+    def generate_asset_operation_token_with_options(self, request, runtime):
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
+    def generate_asset_operation_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.generate_asset_operation_token_with_options(request, runtime)
+
+    def get_database_with_options(self, request, runtime):
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
+    def get_database(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_database_with_options(request, runtime)
+
+    def get_database_account_with_options(self, request, runtime):
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
+    def get_database_account(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_database_account_with_options(request, runtime)
+
     def get_host_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_id):
             query['HostId'] = request.host_id
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -1632,15 +2354,18 @@
 
     def get_host_share_key(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_host_share_key_with_options(request, runtime)
 
     def get_instance_adauth_server_with_options(self, request, runtime):
         """
-        The condition that is used to filter users.
+        ###
+        You can call this operation to query the settings of AD authentication on a bastion host. After you configure AD authentication on a bastion host, you can import AD-authenticated users into the bastion host. After the AD-authenticated users are imported into the bastion host, the AD-authenticated users can log on to the bastion host to perform O\\&M operations on servers.
+        ### Limit
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
         
 
         @param request: GetInstanceADAuthServerRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: GetInstanceADAuthServerResponse
@@ -1668,15 +2393,18 @@
         return TeaCore.from_map(
             yundun_bastionhost_20191209_models.GetInstanceADAuthServerResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_instance_adauth_server(self, request):
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
@@ -1710,17 +2438,17 @@
 
     def get_instance_ldapauth_server(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_instance_ldapauth_server_with_options(request, runtime)
 
     def get_instance_two_factor_with_options(self, request, runtime):
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
@@ -1748,26 +2476,186 @@
         return TeaCore.from_map(
             yundun_bastionhost_20191209_models.GetInstanceTwoFactorResponse(),
             self.call_api(params, req, runtime)
         )
 
     def get_instance_two_factor(self, request):
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
 
+    def get_network_domain_with_options(self, request, runtime):
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
+    def get_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_network_domain_with_options(request, runtime)
+
+    def get_policy_with_options(self, request, runtime):
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
+    def get_policy(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_with_options(request, runtime)
+
+    def get_policy_asset_scope_with_options(self, request, runtime):
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
+    def get_policy_asset_scope(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_asset_scope_with_options(request, runtime)
+
+    def get_policy_user_scope_with_options(self, request, runtime):
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
+    def get_policy_user_scope(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_policy_user_scope_with_options(request, runtime)
+
+    def get_rule_with_options(self, request, runtime):
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
+    def get_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_rule_with_options(request, runtime)
+
     def get_user_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -1858,14 +2746,262 @@
             self.call_api(params, req, runtime)
         )
 
     def list_approve_commands(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_approve_commands_with_options(request, runtime)
 
+    def list_database_accounts_with_options(self, request, runtime):
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
+    def list_database_accounts(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_with_options(request, runtime)
+
+    def list_database_accounts_for_user_with_options(self, request, runtime):
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
+    def list_database_accounts_for_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_for_user_with_options(request, runtime)
+
+    def list_database_accounts_for_user_group_with_options(self, request, runtime):
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
+    def list_database_accounts_for_user_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_database_accounts_for_user_group_with_options(request, runtime)
+
+    def list_databases_with_options(self, request, runtime):
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
+    def list_databases(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_with_options(request, runtime)
+
+    def list_databases_for_user_with_options(self, request, runtime):
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
+    def list_databases_for_user(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_for_user_with_options(request, runtime)
+
+    def list_databases_for_user_group_with_options(self, request, runtime):
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
+    def list_databases_for_user_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_databases_for_user_group_with_options(request, runtime)
+
     def list_host_accounts_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_account_name):
             query['HostAccountName'] = request.host_account_name
         if not UtilClient.is_unset(request.host_id):
             query['HostId'] = request.host_id
@@ -2368,14 +3504,220 @@
             self.call_api(params, req, runtime)
         )
 
     def list_hosts_for_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_hosts_for_user_group_with_options(request, runtime)
 
+    def list_network_domains_with_options(self, request, runtime):
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
+    def list_network_domains(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_network_domains_with_options(request, runtime)
+
+    def list_operation_database_accounts_with_options(self, request, runtime):
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
+    def list_operation_database_accounts(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_database_accounts_with_options(request, runtime)
+
+    def list_operation_databases_with_options(self, request, runtime):
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
+    def list_operation_databases(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_databases_with_options(request, runtime)
+
+    def list_operation_host_accounts_with_options(self, request, runtime):
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
+    def list_operation_host_accounts(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_host_accounts_with_options(request, runtime)
+
+    def list_operation_hosts_with_options(self, request, runtime):
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
+    def list_operation_hosts(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_operation_hosts_with_options(request, runtime)
+
     def list_operation_tickets_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.asset_address):
             query['AssetAddress'] = request.asset_address
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -2404,14 +3746,88 @@
             self.call_api(params, req, runtime)
         )
 
     def list_operation_tickets(self, request):
         runtime = util_models.RuntimeOptions()
         return self.list_operation_tickets_with_options(request, runtime)
 
+    def list_policies_with_options(self, request, runtime):
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
+    def list_policies(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_policies_with_options(request, runtime)
+
+    def list_rules_with_options(self, request, runtime):
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
+    def list_rules(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.list_rules_with_options(request, runtime)
+
     def list_tag_keys_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
@@ -2650,14 +4066,100 @@
         @param request: LockUsersRequest
 
         @return: LockUsersResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.lock_users_with_options(request, runtime)
 
+    def modify_database_with_options(self, request, runtime):
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
+    def modify_database(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_database_with_options(request, runtime)
+
+    def modify_database_account_with_options(self, request, runtime):
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
+    def modify_database_account(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_database_account_with_options(request, runtime)
+
     def modify_host_with_options(self, request, runtime):
         """
         You can call the ModifyHost operation to modify the basic information about a host in a data center, an Elastic Compute Service (ECS) instance, or a host in an ApsaraDB MyBase dedicated cluster.
         > The basic information about ECS instances and hosts in ApsaraDB MyBase dedicated clusters within your Alibaba Cloud account is synchronized to Bastionhost on a regular basis. After you modify the basic information about an ECS instance or a host in an ApsaraDB MyBase dedicated cluster, the modification result may be overwritten by the synchronized information.
         
 
         @param request: ModifyHostRequest
@@ -3102,14 +4604,142 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_instance_two_factor(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_instance_two_factor_with_options(request, runtime)
 
+    def modify_network_domain_with_options(self, request, runtime):
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
+    def modify_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_network_domain_with_options(request, runtime)
+
+    def modify_policy_with_options(self, request, runtime):
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
+    def modify_policy(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_policy_with_options(request, runtime)
+
+    def modify_rule_with_options(self, request, runtime):
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
+    def modify_rule(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_rule_with_options(request, runtime)
+
     def modify_user_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.comment):
             query['Comment'] = request.comment
         if not UtilClient.is_unset(request.display_name):
             query['DisplayName'] = request.display_name
@@ -3196,14 +4826,120 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_user_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_user_group_with_options(request, runtime)
 
+    def modify_user_public_key_with_options(self, request, runtime):
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
+    def modify_user_public_key(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_user_public_key_with_options(request, runtime)
+
+    def move_databases_to_network_domain_with_options(self, request, runtime):
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
+    def move_databases_to_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.move_databases_to_network_domain_with_options(request, runtime)
+
+    def move_hosts_to_network_domain_with_options(self, request, runtime):
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
+    def move_hosts_to_network_domain(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.move_hosts_to_network_domain_with_options(request, runtime)
+
     def move_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
@@ -3314,14 +5050,48 @@
         @param request: RejectOperationTicketRequest
 
         @return: RejectOperationTicketResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reject_operation_ticket_with_options(request, runtime)
 
+    def remove_databases_from_group_with_options(self, request, runtime):
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
+    def remove_databases_from_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.remove_databases_from_group_with_options(request, runtime)
+
     def remove_hosts_from_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.host_group_id):
             query['HostGroupId'] = request.host_group_id
         if not UtilClient.is_unset(request.host_ids):
             query['HostIds'] = request.host_ids
@@ -3404,14 +5174,46 @@
         @param request: RemoveUsersFromGroupRequest
 
         @return: RemoveUsersFromGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.remove_users_from_group_with_options(request, runtime)
 
+    def renew_asset_operation_token_with_options(self, request, runtime):
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
+    def renew_asset_operation_token(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.renew_asset_operation_token_with_options(request, runtime)
+
     def reset_host_account_credential_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.credential_type):
             query['CredentialType'] = request.credential_type
         if not UtilClient.is_unset(request.host_account_id):
             query['HostAccountId'] = request.host_account_id
@@ -3438,14 +5240,282 @@
             self.call_api(params, req, runtime)
         )
 
     def reset_host_account_credential(self, request):
         runtime = util_models.RuntimeOptions()
         return self.reset_host_account_credential_with_options(request, runtime)
 
+    def set_policy_access_time_range_config_with_options(self, tmp_req, runtime):
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
+    def set_policy_access_time_range_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_access_time_range_config_with_options(request, runtime)
+
+    def set_policy_approval_config_with_options(self, tmp_req, runtime):
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
+    def set_policy_approval_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_approval_config_with_options(request, runtime)
+
+    def set_policy_asset_scope_with_options(self, request, runtime):
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
+    def set_policy_asset_scope(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_asset_scope_with_options(request, runtime)
+
+    def set_policy_command_config_with_options(self, tmp_req, runtime):
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
+    def set_policy_command_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_command_config_with_options(request, runtime)
+
+    def set_policy_ipacl_config_with_options(self, tmp_req, runtime):
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
+    def set_policy_ipacl_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_ipacl_config_with_options(request, runtime)
+
+    def set_policy_protocol_config_with_options(self, tmp_req, runtime):
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
+    def set_policy_protocol_config(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_protocol_config_with_options(request, runtime)
+
+    def set_policy_user_scope_with_options(self, request, runtime):
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
+    def set_policy_user_scope(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.set_policy_user_scope_with_options(request, runtime)
+
     def start_instance_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
@@ -3595,7 +5665,101 @@
             yundun_bastionhost_20191209_models.UntagResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def untag_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
+
+    def verify_instance_adauth_server_with_options(self, request, runtime):
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
+    def verify_instance_adauth_server(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.verify_instance_adauth_server_with_options(request, runtime)
+
+    def verify_instance_ldapauth_server_with_options(self, request, runtime):
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
+    def verify_instance_ldapauth_server(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.verify_instance_ldapauth_server_with_options(request, runtime)
```

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209/models.py` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -219,14 +219,165 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AcceptOperationTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AddDatabasesToGroupRequest(TeaModel):
+    def __init__(self, database_ids=None, host_group_id=None, instance_id=None, region_id=None):
+        self.database_ids = database_ids  # type: list[str]
+        self.host_group_id = host_group_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AddDatabasesToGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_id=None, host_group_id=None, message=None):
+        self.code = code  # type: str
+        self.database_id = database_id  # type: str
+        self.host_group_id = host_group_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AddDatabasesToGroupResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[AddDatabasesToGroupResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AddDatabasesToGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: AddDatabasesToGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(AddDatabasesToGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_group_id=None, host_ids=None, instance_id=None, region_id=None):
         # The ID of the host group to which you want to add hosts.
         # 
         # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
         self.host_group_id = host_group_id  # type: str
         # The ID of the host that you want to add to the host group. The value is a JSON string. You can add up to 100 host IDs.
@@ -589,14 +740,484 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = AddUsersToGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class AttachDatabaseAccountsToUserRequestDatabases(TeaModel):
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class AttachDatabaseAccountsToUserRequest(TeaModel):
+    def __init__(self, databases=None, instance_id=None, region_id=None, user_id=None):
+        self.databases = databases  # type: list[AttachDatabaseAccountsToUserRequestDatabases]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_account_id=None, message=None):
+        self.code = code  # type: str
+        self.database_account_id = database_account_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserResponseBodyResultsDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_accounts=None, database_id=None, message=None, user_id=None):
+        self.code = code  # type: str
+        self.database_accounts = database_accounts  # type: list[AttachDatabaseAccountsToUserResponseBodyResultsDatabaseAccounts]
+        self.database_id = database_id  # type: str
+        self.message = message  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[AttachDatabaseAccountsToUserResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: AttachDatabaseAccountsToUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class AttachDatabaseAccountsToUserGroupRequest(TeaModel):
+    def __init__(self, databases=None, instance_id=None, region_id=None, user_group_id=None):
+        self.databases = databases  # type: list[AttachDatabaseAccountsToUserGroupRequestDatabases]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_account_id=None, message=None):
+        self.code = code  # type: str
+        self.database_account_id = database_account_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupResponseBodyResultsDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_accounts=None, database_id=None, message=None, user_group_id=None):
+        self.code = code  # type: str
+        self.database_accounts = database_accounts  # type: list[AttachDatabaseAccountsToUserGroupResponseBodyResultsDatabaseAccounts]
+        self.database_id = database_id  # type: str
+        self.message = message  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[AttachDatabaseAccountsToUserGroupResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: AttachDatabaseAccountsToUserGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(AttachDatabaseAccountsToUserGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_account_ids=None, host_share_key_id=None, instance_id=None, region_id=None):
         # The IDs of the host accounts.
         # 
         # > You must specify this parameter.
         self.host_account_ids = host_account_ids  # type: str
         # The ID of the shared key.
@@ -1807,19 +2428,19 @@
             temp_model = ConfigInstanceSecurityGroupsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ConfigInstanceWhiteListRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None, white_list=None):
-        # The ID of the bastion host for which a whitelist of public IP addresses is configured.
+        # The ID of the bastion host for which you want to configure a whitelist of public IP addresses.
         self.instance_id = instance_id  # type: str
-        # Configures a whitelist of public IP addresses for a bastion host.
+        # The region ID of the bastion host.
         self.region_id = region_id  # type: str
-        # ConfigInstanceWhiteList
+        # The public IP addresses that you want to add to the whitelist.
         self.white_list = white_list  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ConfigInstanceWhiteListRequest, self).to_map()
@@ -1844,15 +2465,17 @@
         if m.get('WhiteList') is not None:
             self.white_list = m.get('WhiteList')
         return self
 
 
 class ConfigInstanceWhiteListResponseBody(TeaModel):
     def __init__(self, instance_id=None, request_id=None):
+        # The ID of the bastion host for which a whitelist of public IP addresses is configured.
         self.instance_id = instance_id  # type: str
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ConfigInstanceWhiteListResponseBody, self).to_map()
@@ -1907,14 +2530,290 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ConfigInstanceWhiteListResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateDatabaseRequest(TeaModel):
+    def __init__(self, active_address_type=None, comment=None, database_name=None, database_port=None,
+                 database_private_address=None, database_public_address=None, database_type=None, instance_id=None, network_domain_id=None,
+                 polar_dbendpoint_type=None, region_id=None, source=None, source_instance_id=None, source_instance_region_id=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: int
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.polar_dbendpoint_type = polar_dbendpoint_type  # type: str
+        self.region_id = region_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_region_id = source_instance_region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatabaseRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_id=None, request_id=None):
+        self.database_id = database_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatabaseResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatabaseResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateDatabaseResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateDatabaseResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_name=None, database_id=None, database_schema=None, instance_id=None,
+                 login_attribute=None, password=None, region_id=None):
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.database_schema = database_schema  # type: str
+        self.instance_id = instance_id  # type: str
+        self.login_attribute = login_attribute  # type: str
+        self.password = password  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatabaseAccountRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, request_id=None):
+        self.database_account_id = database_account_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateDatabaseAccountResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateDatabaseAccountResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateDatabaseAccountResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateDatabaseAccountResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, active_address_type=None, comment=None, host_name=None, host_private_address=None,
                  host_public_address=None, instance_id=None, instance_region_id=None, network_domain_id=None, ostype=None,
                  region_id=None, source=None, source_instance_id=None):
         # The endpoint type of the host that you want to create. Valid values:
         # 
         # *   **Public**: public endpoint
@@ -2092,46 +2991,46 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateHostAccountRequest(TeaModel):
     def __init__(self, host_account_name=None, host_id=None, host_share_key_id=None, instance_id=None,
                  pass_phrase=None, password=None, private_key=None, protocol_name=None, region_id=None):
+        # The name of the host account.
+        self.host_account_name = host_account_name  # type: str
+        # The ID of the host to which you want to add a host account.
+        # 
+        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        self.host_id = host_id  # type: str
+        # The ID of the shared key.
+        self.host_share_key_id = host_share_key_id  # type: str
+        # The ID of the bastion host in which you want to add a host account to the host.
+        # 
+        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id  # type: str
         # The passphrase of the private key for the host account.
         # 
         # >  You can specify this parameter when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter.
-        self.host_account_name = host_account_name  # type: str
-        # The ID of the shared key.
-        self.host_id = host_id  # type: str
+        self.pass_phrase = pass_phrase  # type: str
+        # The password of the host account.
+        self.password = password  # type: str
+        # The private key of the host account. The value is a Base64-encoded string.
+        # 
+        # >  This parameter takes effect only when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter. You can configure a password and a private key for the host account at the same time. If both a password and a private key are configured for the host account, Bastionhost preferentially uses the private key to log on to the host.
+        self.private_key = private_key  # type: str
         # The protocol of the host to which you want to add a host account.
         # 
         # Valid values:
         # 
         # *   SSH
         # *   RDP
-        self.host_share_key_id = host_share_key_id  # type: str
-        # master
-        self.instance_id = instance_id  # type: str
-        # The private key of the host account. The value is a Base64-encoded string.
-        # 
-        # >  This parameter takes effect only when the ProtocolName parameter is set to SSH. If the ProtocolName parameter is set to RDP, you do not need to specify this parameter. You can configure a password and a private key for the host account at the same time. If both a password and a private key are configured for the host account, Bastionhost preferentially uses the private key to log on to the host.
-        self.pass_phrase = pass_phrase  # type: str
+        self.protocol_name = protocol_name  # type: str
         # The region ID of the bastion host in which you want to add a host account to the host.
         # 
         # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.password = password  # type: str
-        # The ID of the host to which you want to add a host account.
-        # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
-        self.private_key = private_key  # type: str
-        # The ID of the bastion host in which you want to add a host account to the host.
-        # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
-        self.protocol_name = protocol_name  # type: str
-        # The password of the host account.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateHostAccountRequest, self).to_map()
@@ -2180,17 +3079,17 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class CreateHostAccountResponseBody(TeaModel):
     def __init__(self, host_account_id=None, request_id=None):
-        # The ID of the request.
-        self.host_account_id = host_account_id  # type: str
         # The operation that you want to perform. Set the value to **CreateHostAccount**.
+        self.host_account_id = host_account_id  # type: str
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateHostAccountResponseBody, self).to_map()
@@ -2257,17 +3156,15 @@
         self.host_group_name = host_group_name  # type: str
         # The ID of the bastion host on which you want to create a host group.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
         # The region ID of the bastion host on which you want to create a host group.
         # 
-        # **\
-        # 
-        # **For more information about the mapping between region IDs and region names, see **Regions and zones[.](~~40654~~)
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateHostGroupRequest, self).to_map()
@@ -2478,14 +3375,549 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateHostShareKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateNetworkDomainRequestProxies(TeaModel):
+    def __init__(self, address=None, node_type=None, password=None, port=None, proxy_type=None, user=None):
+        self.address = address  # type: str
+        self.node_type = node_type  # type: str
+        self.password = password  # type: str
+        self.port = port  # type: int
+        self.proxy_type = proxy_type  # type: str
+        self.user = user  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateNetworkDomainRequestProxies, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, instance_id=None, network_domain_name=None, network_domain_type=None,
+                 proxies=None, region_id=None):
+        self.comment = comment  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_name = network_domain_name  # type: str
+        self.network_domain_type = network_domain_type  # type: str
+        self.proxies = proxies  # type: list[CreateNetworkDomainRequestProxies]
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(CreateNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, network_domain_id=None, request_id=None):
+        self.network_domain_id = network_domain_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateNetworkDomainResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NetworkDomainId') is not None:
+            self.network_domain_id = m.get('NetworkDomainId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreateNetworkDomainResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, instance_id=None, policy_name=None, priority=None, region_id=None):
+        self.comment = comment  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_name = policy_name  # type: str
+        self.priority = priority  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePolicyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, policy_id=None, request_id=None):
+        self.policy_id = policy_id  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreatePolicyResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class CreatePolicyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreatePolicyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreatePolicyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateRuleRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class CreateRuleRequestHostGroups(TeaModel):
+    def __init__(self, host_account_names=None, host_group_id=None):
+        self.host_account_names = host_account_names  # type: list[str]
+        self.host_group_id = host_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateRuleRequestHostGroups, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class CreateRuleRequestHosts(TeaModel):
+    def __init__(self, host_account_ids=None, host_id=None):
+        self.host_account_ids = host_account_ids  # type: list[str]
+        self.host_id = host_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateRuleRequestHosts, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class CreateRuleRequest(TeaModel):
+    def __init__(self, comment=None, databases=None, effective_end_time=None, effective_start_time=None,
+                 host_groups=None, hosts=None, instance_id=None, region_id=None, rule_name=None, user_group_ids=None,
+                 user_ids=None):
+        self.comment = comment  # type: str
+        self.databases = databases  # type: list[CreateRuleRequestDatabases]
+        self.effective_end_time = effective_end_time  # type: long
+        self.effective_start_time = effective_start_time  # type: long
+        self.host_groups = host_groups  # type: list[CreateRuleRequestHostGroups]
+        self.hosts = hosts  # type: list[CreateRuleRequestHosts]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_name = rule_name  # type: str
+        self.user_group_ids = user_group_ids  # type: list[str]
+        self.user_ids = user_ids  # type: list[str]
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
+        _map = super(CreateRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, rule_id=None):
+        self.request_id = request_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RuleId') is not None:
+            self.rule_id = m.get('RuleId')
+        return self
+
+
+class CreateRuleResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, comment=None, display_name=None, effective_end_time=None, effective_start_time=None,
                  email=None, instance_id=None, language=None, language_status=None, mobile=None, mobile_country_code=None,
                  need_reset_password=None, password=None, region_id=None, source=None, source_user_id=None, two_factor_methods=None,
                  two_factor_status=None, user_name=None):
         # The remarks of the user that you want to add. The remarks can be up to 500 characters in length.
         self.comment = comment  # type: str
@@ -2962,14 +4394,202 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateUserPublicKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteDatabaseRequest(TeaModel):
+    def __init__(self, database_id=None, instance_id=None, region_id=None):
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatabaseRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatabaseResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatabaseResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteDatabaseResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteDatabaseResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, instance_id=None, region_id=None):
+        self.database_account_id = database_account_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatabaseAccountRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteDatabaseAccountResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteDatabaseAccountResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteDatabaseAccountResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteDatabaseAccountResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_id=None, instance_id=None, region_id=None):
         # The ID of the host that you want to delete.
         # 
         # > You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
         self.host_id = host_id  # type: str
         # The ID of the bastion host on which you want to delete the host.
@@ -3374,14 +4994,296 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteHostShareKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteNetworkDomainRequest(TeaModel):
+    def __init__(self, instance_id=None, network_domain_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteNetworkDomainResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteNetworkDomainResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, policy_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeletePolicyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeletePolicyResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeletePolicyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeletePolicyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeletePolicyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, region_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteRuleResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DeleteRuleResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, region_id=None, user_id=None):
         # The ID of the bastion host to which the user to be deleted belongs.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
         # The region ID of the bastion host to which the user to be deleted belongs.
@@ -3582,17 +5484,17 @@
             temp_model = DeleteUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteUserPublicKeyRequest(TeaModel):
     def __init__(self, instance_id=None, public_key_id=None, region_id=None):
-        # The region ID of the bastion host on which you want to delete the public key from the user.
+        # The ID of the Bastionhost instance to which the users to be queried belong.
         # 
-        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
         self.instance_id = instance_id  # type: str
         # The ID of the public key.
         self.public_key_id = public_key_id  # type: str
         # The region ID of the bastion host. For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
@@ -4321,17 +6223,21 @@
             temp_model = DescribeInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeRegionsRequest(TeaModel):
     def __init__(self, accept_language=None, region_id=None):
-        # The ID of the region.
+        # The natural language in which responses are returned. Valid values:
+        # 
+        # *   **zh-CN**: Chinese. This is the default value.
+        # *   **en-US**: English.
+        # *   **ja**: Japanese.
         self.accept_language = accept_language  # type: str
-        # The ID of request.
+        # The ID of the region.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRegionsRequest, self).to_map()
@@ -4352,16 +6258,19 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeRegionsResponseBodyRegions(TeaModel):
     def __init__(self, local_name=None, region_endpoint=None, region_id=None):
+        # The name of the region.
         self.local_name = local_name  # type: str
+        # The endpoint of the region.
         self.region_endpoint = region_endpoint  # type: str
+        # The ID of the region.
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeRegionsResponseBodyRegions, self).to_map()
@@ -4386,17 +6295,17 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class DescribeRegionsResponseBody(TeaModel):
     def __init__(self, regions=None, request_id=None):
-        # DescribeRegions
+        # The information about regions where you can create bastion hosts.
         self.regions = regions  # type: list[DescribeRegionsResponseBodyRegions]
-        # Queries available regions where you can create bastion hosts.
+        # The ID of request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.regions:
             for k in self.regions:
                 if k:
                     k.validate()
@@ -4459,14 +6368,484 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeRegionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DetachDatabaseAccountsFromUserRequestDatabases(TeaModel):
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserRequest(TeaModel):
+    def __init__(self, databases=None, instance_id=None, region_id=None, user_id=None):
+        self.databases = databases  # type: list[DetachDatabaseAccountsFromUserRequestDatabases]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_account_id=None, message=None):
+        self.code = code  # type: str
+        self.database_account_id = database_account_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserResponseBodyResultsDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_accounts=None, database_id=None, message=None, user_id=None):
+        self.code = code  # type: str
+        self.database_accounts = database_accounts  # type: list[DetachDatabaseAccountsFromUserResponseBodyResultsDatabaseAccounts]
+        self.database_id = database_id  # type: str
+        self.message = message  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[DetachDatabaseAccountsFromUserResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DetachDatabaseAccountsFromUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class DetachDatabaseAccountsFromUserGroupRequest(TeaModel):
+    def __init__(self, databases=None, instance_id=None, region_id=None, user_group_id=None):
+        self.databases = databases  # type: list[DetachDatabaseAccountsFromUserGroupRequestDatabases]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_account_id=None, message=None):
+        self.code = code  # type: str
+        self.database_account_id = database_account_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupResponseBodyResultsDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_accounts=None, database_id=None, message=None, user_group_id=None):
+        self.code = code  # type: str
+        self.database_accounts = database_accounts  # type: list[DetachDatabaseAccountsFromUserGroupResponseBodyResultsDatabaseAccounts]
+        self.database_id = database_id  # type: str
+        self.message = message  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[DetachDatabaseAccountsFromUserGroupResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DetachDatabaseAccountsFromUserGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DetachDatabaseAccountsFromUserGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_account_ids=None, host_share_key_id=None, instance_id=None, region_id=None):
         # The IDs of the host accounts.
         self.host_account_ids = host_account_ids  # type: str
         # The ID of the shared key.
         self.host_share_key_id = host_share_key_id  # type: str
         # The ID of the bastion host. You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
@@ -5650,14 +8029,108 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DisableInstancePublicAccessResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DisableRuleRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DisableRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DisableRuleResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DisableRuleResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DisableRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DisableRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, region_id=None):
         # The ID of the bastion host.
         # 
         # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
         # The region ID of the bastion host.
@@ -5750,14 +8223,624 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = EnableInstancePublicAccessResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class EnableRuleRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(EnableRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(EnableRuleResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class EnableRuleResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: EnableRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(EnableRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, asset_account_id=None, asset_account_name=None, asset_account_password=None,
+                 asset_account_protocol_name=None, asset_id=None, asset_type=None, instance_id=None, region_id=None):
+        self.asset_account_id = asset_account_id  # type: str
+        self.asset_account_name = asset_account_name  # type: str
+        self.asset_account_password = asset_account_password  # type: str
+        self.asset_account_protocol_name = asset_account_protocol_name  # type: str
+        self.asset_id = asset_id  # type: str
+        self.asset_type = asset_type  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GenerateAssetOperationTokenRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, count_left=None, expire_time=None, has_count_limit=None, max_renew_count=None,
+                 renew_count=None, token=None, token_id=None):
+        self.count_left = count_left  # type: long
+        self.expire_time = expire_time  # type: long
+        self.has_count_limit = has_count_limit  # type: bool
+        self.max_renew_count = max_renew_count  # type: long
+        self.renew_count = renew_count  # type: long
+        self.token = token  # type: str
+        self.token_id = token_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GenerateAssetOperationTokenResponseBodyAssetOperationToken, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, asset_operation_token=None, request_id=None):
+        self.asset_operation_token = asset_operation_token  # type: GenerateAssetOperationTokenResponseBodyAssetOperationToken
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.asset_operation_token:
+            self.asset_operation_token.validate()
+
+    def to_map(self):
+        _map = super(GenerateAssetOperationTokenResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GenerateAssetOperationTokenResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GenerateAssetOperationTokenResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_id=None, instance_id=None, region_id=None):
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetDatabaseRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, database_id=None, database_name=None,
+                 database_port=None, database_private_address=None, database_public_address=None, database_type=None,
+                 network_domain_id=None, source=None, source_instance_id=None, source_instance_region_id=None,
+                 source_instance_state=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: long
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_region_id = source_instance_region_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetDatabaseResponseBodyDatabase, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database=None, request_id=None):
+        self.database = database  # type: GetDatabaseResponseBodyDatabase
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.database:
+            self.database.validate()
+
+    def to_map(self):
+        _map = super(GetDatabaseResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetDatabaseResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetDatabaseResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, instance_id=None, region_id=None):
+        self.database_account_id = database_account_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetDatabaseAccountRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, database_account_name=None, database_schema=None,
+                 has_password=None, login_attribute=None):
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_schema = database_schema  # type: str
+        self.has_password = has_password  # type: bool
+        self.login_attribute = login_attribute  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetDatabaseAccountResponseBodyDatabaseAccount, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account=None, request_id=None):
+        self.database_account = database_account  # type: GetDatabaseAccountResponseBodyDatabaseAccount
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.database_account:
+            self.database_account.validate()
+
+    def to_map(self):
+        _map = super(GetDatabaseAccountResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetDatabaseAccountResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetDatabaseAccountResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_id=None, instance_id=None, region_id=None):
         # The ID of the host that you want to query. You can specify only one host ID.
         # 
         # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
         self.host_id = host_id  # type: str
         # The ID of the bastion host in which you want to query the host.
@@ -6206,23 +9289,25 @@
             temp_model = GetHostAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetHostGroupRequest(TeaModel):
     def __init__(self, host_group_id=None, instance_id=None, region_id=None):
-        # The region ID of the Bastionhost instance where you want to query the host group.
+        # The ID of the host group.
         # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
         self.host_group_id = host_group_id  # type: str
-        # MyHostGroup
+        # The ID of the bastion host in which you want to query the details of the host group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
-        # The ID of the Bastionhost instance where you want to query the host group.
+        # The region ID of the bastion host in which you want to query the details of the host group.
         # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetHostGroupRequest, self).to_map()
@@ -6247,19 +9332,19 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetHostGroupResponseBodyHostGroup(TeaModel):
     def __init__(self, comment=None, host_group_id=None, host_group_name=None):
-        # The details of the host group returned.
-        self.comment = comment  # type: str
         # The description of the host group.
-        self.host_group_id = host_group_id  # type: str
+        self.comment = comment  # type: str
         # The ID of the host group.
+        self.host_group_id = host_group_id  # type: str
+        # The name of the host group.
         self.host_group_name = host_group_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetHostGroupResponseBodyHostGroup, self).to_map()
@@ -6284,19 +9369,17 @@
         if m.get('HostGroupName') is not None:
             self.host_group_name = m.get('HostGroupName')
         return self
 
 
 class GetHostGroupResponseBody(TeaModel):
     def __init__(self, host_group=None, request_id=None):
-        # The ID of the host group that you want to query.
-        # 
-        # >  You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        # The details of the host group returned.
         self.host_group = host_group  # type: GetHostGroupResponseBodyHostGroup
-        # my host group.
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.host_group:
             self.host_group.validate()
 
     def to_map(self):
@@ -6502,20 +9585,19 @@
             temp_model = GetHostShareKeyResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetInstanceADAuthServerRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None):
-        # The field that is used to indicate the email address of a user on the AD server.
+        # The ID of the bastion host. You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
-        # Indicates whether passwords are required. Valid values:
+        # The region ID of the bastion host.
         # 
-        # *   **true**: required
-        # *   **false**: not required
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceADAuthServerRequest, self).to_map()
@@ -6537,37 +9619,43 @@
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetInstanceADAuthServerResponseBodyAD(TeaModel):
     def __init__(self, account=None, base_dn=None, domain=None, email_mapping=None, filter=None, has_password=None,
                  is_ssl=None, mobile_mapping=None, name_mapping=None, port=None, server=None, standby_server=None):
-        # The port that is used to access the AD server.
+        # The distinguished name (DN) of the AD server account.
         self.account = account  # type: str
-        # The ID of the bastion host to query.
-        # 
-        # You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        # The Base DN of the AD server.
         self.base_dn = base_dn  # type: str
-        # The settings of AD authentication.
+        # The domain on the AD server.
         self.domain = domain  # type: str
-        # The address of the secondary AD server.
+        # The field that is used to indicate the email address of a user on the AD server.
         self.email_mapping = email_mapping  # type: str
-        # The field that is used to indicate the mobile phone number of a user on the AD server.
+        # The condition that is used to filter users.
         self.filter = filter  # type: str
-        # The address of the AD server.
+        # Indicates whether passwords are required. Valid values:
+        # 
+        # *   **true**:
+        # *   **false**\
         self.has_password = has_password  # type: bool
-        # The Base DN of the AD server.
+        # Indicates whether SSL is supported. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.is_ssl = is_ssl  # type: bool
-        # The field that is used to indicate the name of a user on the AD server.
+        # The field that is used to indicate the mobile phone number of a user on the AD server.
         self.mobile_mapping = mobile_mapping  # type: str
-        # The ID of the request, which is used to locate and troubleshoot issues.
+        # The field that is used to indicate the name of a user on the AD server.
         self.name_mapping = name_mapping  # type: str
-        # Queries the settings of Active Directory (AD) authentication on a bastion host.
+        # The port that is used to access the AD server.
         self.port = port  # type: long
+        # The address of the LDAP server.
         self.server = server  # type: str
+        # The address of the secondary LDAP server.
         self.standby_server = standby_server  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceADAuthServerResponseBodyAD, self).to_map()
@@ -6628,20 +9716,17 @@
         if m.get('StandbyServer') is not None:
             self.standby_server = m.get('StandbyServer')
         return self
 
 
 class GetInstanceADAuthServerResponseBody(TeaModel):
     def __init__(self, ad=None, request_id=None):
-        # The operation that you want to perform. Set the value to **GetInstanceADAuthServer**.
+        # The settings of AD authentication.
         self.ad = ad  # type: GetInstanceADAuthServerResponseBodyAD
-        # Indicates whether SSL is supported. Valid values:
-        # 
-        # *   **true**: supported
-        # *   **false**: not supported
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.ad:
             self.ad.validate()
 
     def to_map(self):
@@ -6897,17 +9982,21 @@
             temp_model = GetInstanceLDAPAuthServerResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetInstanceTwoFactorRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None):
-        # The ID of the request, which is used to locate and troubleshoot issues.
+        # The ID of the bastion host.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
-        # The operation that you want to perform. Set the value to **GetInstanceTwoFactor**.
+        # The region ID of the bastion host.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceTwoFactorRequest, self).to_map()
@@ -6928,17 +10017,24 @@
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         return self
 
 
 class GetInstanceTwoFactorResponseBodyConfig(TeaModel):
     def __init__(self, enable_two_factor=None, skip_two_factor_time=None, two_factor_methods=None):
-        # Queries the settings of two-factor authentication on a bastion host.
+        # Indicates whether two-factor authentication is enabled. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.enable_two_factor = enable_two_factor  # type: bool
+        # The duration within which two-factor authentication is not required after a local user passes two-factor authentication. Valid values: `0 to 168`. Unit: hours.
+        # 
+        # > If 0 is returned, a local user must pass two-factor authentication every time the local user logs on to the bastion host.
         self.skip_two_factor_time = skip_two_factor_time  # type: long
+        # The two-factor authentication methods.
         self.two_factor_methods = two_factor_methods  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetInstanceTwoFactorResponseBodyConfig, self).to_map()
@@ -6965,17 +10061,15 @@
         return self
 
 
 class GetInstanceTwoFactorResponseBody(TeaModel):
     def __init__(self, config=None, request_id=None):
         # The settings of two-factor authentication.
         self.config = config  # type: GetInstanceTwoFactorResponseBodyConfig
-        # The duration within which two-factor authentication is not required after a local user passes two-factor authentication. Valid values: `0 to 168`. Unit: hours.
-        # 
-        # >  If 0 is returned, a local user must pass two-factor authentication every time the local user logs on to the bastion host.
+        # The ID of the request, which is used to locate and troubleshoot issues.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.config:
             self.config.validate()
 
     def to_map(self):
@@ -7032,14 +10126,1575 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetInstanceTwoFactorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetNetworkDomainRequest(TeaModel):
+    def __init__(self, instance_id=None, network_domain_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetNetworkDomainResponseBodyNetworkDomainProxies(TeaModel):
+    def __init__(self, address=None, has_password=None, node_type=None, port=None, proxy_state=None,
+                 proxy_state_error_code=None, proxy_type=None, user=None):
+        self.address = address  # type: str
+        self.has_password = has_password  # type: bool
+        self.node_type = node_type  # type: str
+        self.port = port  # type: int
+        self.proxy_state = proxy_state  # type: str
+        self.proxy_state_error_code = proxy_state_error_code  # type: str
+        self.proxy_type = proxy_type  # type: str
+        self.user = user  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetNetworkDomainResponseBodyNetworkDomainProxies, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, default=None, network_domain_id=None, network_domain_name=None,
+                 network_domain_type=None, proxies=None):
+        self.comment = comment  # type: str
+        self.default = default  # type: bool
+        self.network_domain_id = network_domain_id  # type: str
+        self.network_domain_name = network_domain_name  # type: str
+        self.network_domain_type = network_domain_type  # type: str
+        self.proxies = proxies  # type: list[GetNetworkDomainResponseBodyNetworkDomainProxies]
+
+    def validate(self):
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetNetworkDomainResponseBodyNetworkDomain, self).to_map()
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
+        result['Proxies'] = []
+        if self.proxies is not None:
+            for k in self.proxies:
+                result['Proxies'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m=None):
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
+        self.proxies = []
+        if m.get('Proxies') is not None:
+            for k in m.get('Proxies'):
+                temp_model = GetNetworkDomainResponseBodyNetworkDomainProxies()
+                self.proxies.append(temp_model.from_map(k))
+        return self
+
+
+class GetNetworkDomainResponseBody(TeaModel):
+    def __init__(self, network_domain=None, request_id=None):
+        self.network_domain = network_domain  # type: GetNetworkDomainResponseBodyNetworkDomain
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.network_domain:
+            self.network_domain.validate()
+
+    def to_map(self):
+        _map = super(GetNetworkDomainResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.network_domain is not None:
+            result['NetworkDomain'] = self.network_domain.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NetworkDomain') is not None:
+            temp_model = GetNetworkDomainResponseBodyNetworkDomain()
+            self.network_domain = temp_model.from_map(m['NetworkDomain'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetNetworkDomainResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetNetworkDomainResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPolicyRequest(TeaModel):
+    def __init__(self, instance_id=None, policy_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime(TeaModel):
+    def __init__(self, days=None, hours=None):
+        self.days = days  # type: list[str]
+        self.hours = hours  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Days') is not None:
+            self.days = m.get('Days')
+        if m.get('Hours') is not None:
+            self.hours = m.get('Hours')
+        return self
+
+
+class GetPolicyResponseBodyPolicyAccessTimeRangeConfig(TeaModel):
+    def __init__(self, effective_time=None):
+        self.effective_time = effective_time  # type: list[GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime]
+
+    def validate(self):
+        if self.effective_time:
+            for k in self.effective_time:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyAccessTimeRangeConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        self.effective_time = []
+        if m.get('EffectiveTime') is not None:
+            for k in m.get('EffectiveTime'):
+                temp_model = GetPolicyResponseBodyPolicyAccessTimeRangeConfigEffectiveTime()
+                self.effective_time.append(temp_model.from_map(k))
+        return self
+
+
+class GetPolicyResponseBodyPolicyApprovalConfig(TeaModel):
+    def __init__(self, switch_status=None):
+        self.switch_status = switch_status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyApprovalConfig, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.switch_status is not None:
+            result['SwitchStatus'] = self.switch_status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SwitchStatus') is not None:
+            self.switch_status = m.get('SwitchStatus')
+        return self
+
+
+class GetPolicyResponseBodyPolicyCommandConfigApproval(TeaModel):
+    def __init__(self, commands=None):
+        self.commands = commands  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyCommandConfigApproval, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.commands is not None:
+            result['Commands'] = self.commands
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class GetPolicyResponseBodyPolicyCommandConfigDeny(TeaModel):
+    def __init__(self, acl_type=None, commands=None):
+        self.acl_type = acl_type  # type: str
+        self.commands = commands  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyCommandConfigDeny, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class GetPolicyResponseBodyPolicyCommandConfig(TeaModel):
+    def __init__(self, approval=None, deny=None):
+        self.approval = approval  # type: GetPolicyResponseBodyPolicyCommandConfigApproval
+        self.deny = deny  # type: GetPolicyResponseBodyPolicyCommandConfigDeny
+
+    def validate(self):
+        if self.approval:
+            self.approval.validate()
+        if self.deny:
+            self.deny.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyCommandConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Approval') is not None:
+            temp_model = GetPolicyResponseBodyPolicyCommandConfigApproval()
+            self.approval = temp_model.from_map(m['Approval'])
+        if m.get('Deny') is not None:
+            temp_model = GetPolicyResponseBodyPolicyCommandConfigDeny()
+            self.deny = temp_model.from_map(m['Deny'])
+        return self
+
+
+class GetPolicyResponseBodyPolicyIPAclConfig(TeaModel):
+    def __init__(self, acl_type=None, ips=None):
+        self.acl_type = acl_type  # type: str
+        self.ips = ips  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyIPAclConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('IPs') is not None:
+            self.ips = m.get('IPs')
+        return self
+
+
+class GetPolicyResponseBodyPolicyProtocolConfigRDP(TeaModel):
+    def __init__(self, clipboard_download=None, clipboard_upload=None, disk_redirection=None, record_keyboard=None):
+        self.clipboard_download = clipboard_download  # type: str
+        self.clipboard_upload = clipboard_upload  # type: str
+        self.disk_redirection = disk_redirection  # type: str
+        self.record_keyboard = record_keyboard  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyProtocolConfigRDP, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyResponseBodyPolicyProtocolConfigSSH(TeaModel):
+    def __init__(self, exec_command=None, sftpchannel=None, sftpdownload_file=None, sftpmkdir=None,
+                 sftpremove_file=None, sftprename_file=None, sftprmdir=None, sftpupload_file=None, sshchannel=None,
+                 x_11forwarding=None):
+        self.exec_command = exec_command  # type: str
+        self.sftpchannel = sftpchannel  # type: str
+        self.sftpdownload_file = sftpdownload_file  # type: str
+        self.sftpmkdir = sftpmkdir  # type: str
+        self.sftpremove_file = sftpremove_file  # type: str
+        self.sftprename_file = sftprename_file  # type: str
+        self.sftprmdir = sftprmdir  # type: str
+        self.sftpupload_file = sftpupload_file  # type: str
+        self.sshchannel = sshchannel  # type: str
+        self.x_11forwarding = x_11forwarding  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyProtocolConfigSSH, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyResponseBodyPolicyProtocolConfig(TeaModel):
+    def __init__(self, rdp=None, ssh=None):
+        self.rdp = rdp  # type: GetPolicyResponseBodyPolicyProtocolConfigRDP
+        self.ssh = ssh  # type: GetPolicyResponseBodyPolicyProtocolConfigSSH
+
+    def validate(self):
+        if self.rdp:
+            self.rdp.validate()
+        if self.ssh:
+            self.ssh.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBodyPolicyProtocolConfig, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, access_time_range_config=None, approval_config=None, command_config=None, comment=None,
+                 ipacl_config=None, policy_id=None, policy_name=None, priority=None, protocol_config=None):
+        self.access_time_range_config = access_time_range_config  # type: GetPolicyResponseBodyPolicyAccessTimeRangeConfig
+        self.approval_config = approval_config  # type: GetPolicyResponseBodyPolicyApprovalConfig
+        self.command_config = command_config  # type: GetPolicyResponseBodyPolicyCommandConfig
+        self.comment = comment  # type: str
+        self.ipacl_config = ipacl_config  # type: GetPolicyResponseBodyPolicyIPAclConfig
+        self.policy_id = policy_id  # type: str
+        self.policy_name = policy_name  # type: str
+        self.priority = priority  # type: long
+        self.protocol_config = protocol_config  # type: GetPolicyResponseBodyPolicyProtocolConfig
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
+        _map = super(GetPolicyResponseBodyPolicy, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, policy=None, request_id=None):
+        self.policy = policy  # type: GetPolicyResponseBodyPolicy
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.policy:
+            self.policy.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.policy is not None:
+            result['Policy'] = self.policy.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Policy') is not None:
+            temp_model = GetPolicyResponseBodyPolicy()
+            self.policy = temp_model.from_map(m['Policy'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetPolicyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetPolicyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPolicyResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPolicyAssetScopeRequest(TeaModel):
+    def __init__(self, instance_id=None, policy_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyAssetScopeResponseBodyAssetScopeDatabases(TeaModel):
+    def __init__(self, account_scope_type=None, database_account_ids=None, database_id=None):
+        self.account_scope_type = account_scope_type  # type: str
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeResponseBodyAssetScopeDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyAssetScopeResponseBodyAssetScopeHostGroups(TeaModel):
+    def __init__(self, account_names=None, account_scope_type=None, host_group_id=None):
+        self.account_names = account_names  # type: list[str]
+        self.account_scope_type = account_scope_type  # type: str
+        self.host_group_id = host_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeResponseBodyAssetScopeHostGroups, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyAssetScopeResponseBodyAssetScopeHosts(TeaModel):
+    def __init__(self, account_scope_type=None, host_account_ids=None, host_id=None):
+        self.account_scope_type = account_scope_type  # type: str
+        self.host_account_ids = host_account_ids  # type: list[str]
+        self.host_id = host_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeResponseBodyAssetScopeHosts, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyAssetScopeResponseBodyAssetScope(TeaModel):
+    def __init__(self, databases=None, host_groups=None, hosts=None, scope_type=None):
+        self.databases = databases  # type: list[GetPolicyAssetScopeResponseBodyAssetScopeDatabases]
+        self.host_groups = host_groups  # type: list[GetPolicyAssetScopeResponseBodyAssetScopeHostGroups]
+        self.hosts = hosts  # type: list[GetPolicyAssetScopeResponseBodyAssetScopeHosts]
+        self.scope_type = scope_type  # type: str
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
+        _map = super(GetPolicyAssetScopeResponseBodyAssetScope, self).to_map()
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
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
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
+        return self
+
+
+class GetPolicyAssetScopeResponseBody(TeaModel):
+    def __init__(self, asset_scope=None, request_id=None):
+        self.asset_scope = asset_scope  # type: GetPolicyAssetScopeResponseBodyAssetScope
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.asset_scope:
+            self.asset_scope.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.asset_scope is not None:
+            result['AssetScope'] = self.asset_scope.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AssetScope') is not None:
+            temp_model = GetPolicyAssetScopeResponseBodyAssetScope()
+            self.asset_scope = temp_model.from_map(m['AssetScope'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetPolicyAssetScopeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetPolicyAssetScopeResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyAssetScopeResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPolicyAssetScopeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetPolicyUserScopeRequest(TeaModel):
+    def __init__(self, instance_id=None, policy_id=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyUserScopeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetPolicyUserScopeResponseBodyUserScope(TeaModel):
+    def __init__(self, scope_type=None, user_group_ids=None, user_ids=None):
+        self.scope_type = scope_type  # type: str
+        self.user_group_ids = user_group_ids  # type: list[str]
+        self.user_ids = user_ids  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetPolicyUserScopeResponseBodyUserScope, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.scope_type is not None:
+            result['ScopeType'] = self.scope_type
+        if self.user_group_ids is not None:
+            result['UserGroupIds'] = self.user_group_ids
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ScopeType') is not None:
+            self.scope_type = m.get('ScopeType')
+        if m.get('UserGroupIds') is not None:
+            self.user_group_ids = m.get('UserGroupIds')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class GetPolicyUserScopeResponseBody(TeaModel):
+    def __init__(self, request_id=None, user_scope=None):
+        self.request_id = request_id  # type: str
+        self.user_scope = user_scope  # type: GetPolicyUserScopeResponseBodyUserScope
+
+    def validate(self):
+        if self.user_scope:
+            self.user_scope.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyUserScopeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.user_scope is not None:
+            result['UserScope'] = self.user_scope.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('UserScope') is not None:
+            temp_model = GetPolicyUserScopeResponseBodyUserScope()
+            self.user_scope = temp_model.from_map(m['UserScope'])
+        return self
+
+
+class GetPolicyUserScopeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetPolicyUserScopeResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetPolicyUserScopeResponse, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetPolicyUserScopeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetRuleRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, rule_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_id = rule_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+class GetRuleResponseBodyRuleDatabasesDatabaseAccounts(TeaModel):
+    def __init__(self, database_account_id=None):
+        self.database_account_id = database_account_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleDatabasesDatabaseAccounts, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.database_account_id is not None:
+            result['DatabaseAccountId'] = self.database_account_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountId') is not None:
+            self.database_account_id = m.get('DatabaseAccountId')
+        return self
+
+
+class GetRuleResponseBodyRuleDatabases(TeaModel):
+    def __init__(self, database_accounts=None, database_id=None):
+        self.database_accounts = database_accounts  # type: list[GetRuleResponseBodyRuleDatabasesDatabaseAccounts]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleDatabases, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['DatabaseAccounts'] = []
+        if self.database_accounts is not None:
+            for k in self.database_accounts:
+                result['DatabaseAccounts'].append(k.to_map() if k else None)
+        if self.database_id is not None:
+            result['DatabaseId'] = self.database_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.database_accounts = []
+        if m.get('DatabaseAccounts') is not None:
+            for k in m.get('DatabaseAccounts'):
+                temp_model = GetRuleResponseBodyRuleDatabasesDatabaseAccounts()
+                self.database_accounts.append(temp_model.from_map(k))
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class GetRuleResponseBodyRuleHostGroups(TeaModel):
+    def __init__(self, host_account_names=None, host_group_id=None):
+        self.host_account_names = host_account_names  # type: list[str]
+        self.host_group_id = host_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleHostGroups, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class GetRuleResponseBodyRuleHostsHostAccounts(TeaModel):
+    def __init__(self, host_account_id=None):
+        self.host_account_id = host_account_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleHostsHostAccounts, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.host_account_id is not None:
+            result['HostAccountId'] = self.host_account_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountId') is not None:
+            self.host_account_id = m.get('HostAccountId')
+        return self
+
+
+class GetRuleResponseBodyRuleHosts(TeaModel):
+    def __init__(self, host_accounts=None, host_id=None):
+        self.host_accounts = host_accounts  # type: list[GetRuleResponseBodyRuleHostsHostAccounts]
+        self.host_id = host_id  # type: str
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleHosts, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['HostAccounts'] = []
+        if self.host_accounts is not None:
+            for k in self.host_accounts:
+                result['HostAccounts'].append(k.to_map() if k else None)
+        if self.host_id is not None:
+            result['HostId'] = self.host_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
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
+    def __init__(self, user_group_id=None):
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleUserGroups, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_group_id is not None:
+            result['UserGroupId'] = self.user_group_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('UserGroupId') is not None:
+            self.user_group_id = m.get('UserGroupId')
+        return self
+
+
+class GetRuleResponseBodyRuleUsers(TeaModel):
+    def __init__(self, user_id=None):
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetRuleResponseBodyRuleUsers, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['UserId'] = self.user_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('UserId') is not None:
+            self.user_id = m.get('UserId')
+        return self
+
+
+class GetRuleResponseBodyRule(TeaModel):
+    def __init__(self, comment=None, databases=None, effective_end_time=None, effective_start_time=None,
+                 host_groups=None, hosts=None, rule_id=None, rule_name=None, user_groups=None, users=None):
+        self.comment = comment  # type: str
+        self.databases = databases  # type: list[GetRuleResponseBodyRuleDatabases]
+        self.effective_end_time = effective_end_time  # type: str
+        self.effective_start_time = effective_start_time  # type: str
+        self.host_groups = host_groups  # type: list[GetRuleResponseBodyRuleHostGroups]
+        self.hosts = hosts  # type: list[GetRuleResponseBodyRuleHosts]
+        self.rule_id = rule_id  # type: str
+        self.rule_name = rule_name  # type: str
+        self.user_groups = user_groups  # type: list[GetRuleResponseBodyRuleUserGroups]
+        self.users = users  # type: list[GetRuleResponseBodyRuleUsers]
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
+        _map = super(GetRuleResponseBodyRule, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, rule=None):
+        self.request_id = request_id  # type: str
+        self.rule = rule  # type: GetRuleResponseBodyRule
+
+    def validate(self):
+        if self.rule:
+            self.rule.validate()
+
+    def to_map(self):
+        _map = super(GetRuleResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
 class GetUserRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None, user_id=None):
         # The ID of the bastion host on which you want to query the user.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
         # The region ID of the bastion host on which you want to query the user.
@@ -7300,21 +11955,25 @@
             temp_model = GetUserResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetUserGroupRequest(TeaModel):
     def __init__(self, instance_id=None, region_id=None, user_group_id=None):
-        # The ID of the request.
+        # The ID of the bastion host in which you want to query the details of the user group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
-        # The name of the user group.
+        # The region ID of the bastion host in which you want to query the details of the user group.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
-        # All Bastionhost API requests must include common request parameters. For more information about common request parameters, see [Common parameters](~~315526~~).
+        # The ID of the user group.
         # 
-        # For more information about sample requests, see the "Examples" section of this topic.
+        # > You can call the [ListUserGroups](~~204509~~) operation to query the ID of the user group.
         self.user_group_id = user_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetUserGroupRequest, self).to_map()
@@ -7339,18 +11998,19 @@
         if m.get('UserGroupId') is not None:
             self.user_group_id = m.get('UserGroupId')
         return self
 
 
 class GetUserGroupResponseBodyUserGroup(TeaModel):
     def __init__(self, comment=None, user_group_id=None, user_group_name=None):
-        # GetUserGroup
+        # The description of the user group.
         self.comment = comment  # type: str
+        # The ID of the group.
         self.user_group_id = user_group_id  # type: str
-        # WB662865
+        # The name of the user group.
         self.user_group_name = user_group_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GetUserGroupResponseBodyUserGroup, self).to_map()
@@ -7375,17 +12035,17 @@
         if m.get('UserGroupName') is not None:
             self.user_group_name = m.get('UserGroupName')
         return self
 
 
 class GetUserGroupResponseBody(TeaModel):
     def __init__(self, request_id=None, user_group=None):
-        # Queries the details of a specified user group in a specified Bastionhost instance.
+        # The request ID.
         self.request_id = request_id  # type: str
-        # GetUserGroup
+        # The details of the user group returned.
         self.user_group = user_group  # type: GetUserGroupResponseBodyUserGroup
 
     def validate(self):
         if self.user_group:
             self.user_group.validate()
 
     def to_map(self):
@@ -7635,48 +12295,1242 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListApproveCommandsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListDatabaseAccountsRequest(TeaModel):
+    def __init__(self, database_account_name=None, database_id=None, instance_id=None, page_number=None,
+                 page_size=None, region_id=None):
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, database_account_name=None, database_id=None,
+                 database_schema=None, has_password=None):
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.database_schema = database_schema  # type: str
+        self.has_password = has_password  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsResponseBodyDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_accounts=None, request_id=None, total_count=None):
+        self.database_accounts = database_accounts  # type: list[ListDatabaseAccountsResponseBodyDatabaseAccounts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabaseAccountsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_name=None, database_id=None, instance_id=None, page_number=None,
+                 page_size=None, region_id=None, user_id=None):
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, database_account_name=None, database_id=None, is_authorized=None,
+                 protocol_name=None):
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.is_authorized = is_authorized  # type: bool
+        self.protocol_name = protocol_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserResponseBodyDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_accounts=None, request_id=None, total_count=None):
+        self.database_accounts = database_accounts  # type: list[ListDatabaseAccountsForUserResponseBodyDatabaseAccounts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabaseAccountsForUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_name=None, database_id=None, instance_id=None, page_number=None,
+                 page_size=None, region_id=None, user_group_id=None):
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, database_account_name=None, database_id=None, is_authorized=None,
+                 protocol_name=None):
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.is_authorized = is_authorized  # type: bool
+        self.protocol_name = protocol_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserGroupResponseBodyDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_accounts=None, request_id=None, total_count=None):
+        self.database_accounts = database_accounts  # type: list[ListDatabaseAccountsForUserGroupResponseBodyDatabaseAccounts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabaseAccountsForUserGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabaseAccountsForUserGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_type=None, host_group_id=None, instance_id=None, network_domain_id=None,
+                 page_number=None, page_size=None, region_id=None, source=None):
+        self.database_type = database_type  # type: str
+        self.host_group_id = host_group_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.source = source  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, database_id=None, database_name=None,
+                 database_port=None, database_private_address=None, database_public_address=None, database_type=None,
+                 network_domain_id=None, source=None, source_instance_id=None, source_instance_region_id=None,
+                 source_instance_state=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: int
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_region_id = source_instance_region_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesResponseBodyDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, databases=None, request_id=None, total_count=None):
+        self.databases = databases  # type: list[ListDatabasesResponseBodyDatabases]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabasesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_address=None, database_name=None, database_type=None, instance_id=None,
+                 network_domain_id=None, page_number=None, page_size=None, region_id=None, user_id=None):
+        self.database_address = database_address  # type: str
+        self.database_name = database_name  # type: str
+        self.database_type = database_type  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.user_id = user_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, database_id=None, database_name=None,
+                 database_port=None, database_private_address=None, database_public_address=None, database_type=None,
+                 network_domain_id=None, source=None, source_instance_id=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: long
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserResponseBodyDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, databases=None, request_id=None, total_count=None):
+        self.databases = databases  # type: list[ListDatabasesForUserResponseBodyDatabases]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabasesForUserResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_address=None, database_name=None, database_type=None, instance_id=None,
+                 network_domain_id=None, page_number=None, page_size=None, region_id=None, user_group_id=None):
+        self.database_address = database_address  # type: str
+        self.database_name = database_name  # type: str
+        self.database_type = database_type  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.user_group_id = user_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, database_account_count=None, database_id=None,
+                 database_name=None, database_port=None, database_private_address=None, database_public_address=None,
+                 database_type=None, network_domain_id=None, source=None, source_instance_id=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_account_count = database_account_count  # type: long
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: long
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserGroupResponseBodyDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, databases=None, request_id=None, total_count=None):
+        self.databases = databases  # type: list[ListDatabasesForUserGroupResponseBodyDatabases]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListDatabasesForUserGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListDatabasesForUserGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
 class ListHostAccountsRequest(TeaModel):
     def __init__(self, host_account_name=None, host_id=None, instance_id=None, page_number=None, page_size=None,
                  protocol_name=None, region_id=None):
-        # Indicates whether a password is configured for the host account.
-        # 
-        # Valid values:
-        # 
-        # *   true: A password is configured for the host account.
-        # *   false: No passwords are configured for the host account.
+        # The name of the host account that you want to query. The name can be up to 128 characters in length. Only exact match is supported.
         self.host_account_name = host_account_name  # type: str
-        # The protocol used by the host whose accounts you want to query.
-        # 
-        # Valid values:
+        # The ID of the specified host whose accounts you want to query.
         # 
-        # *   SSH
-        # *   RDP
+        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
         self.host_id = host_id  # type: str
-        # The ID of the shared key.
-        self.instance_id = instance_id  # type: str
-        # The operation that you want to perform.
+        # The ID of the bastion host in which you want to query accounts of the specified host.
         # 
-        # Set the value to **ListHostAccounts**.
+        # >  You can call the DescribeInstances operation to query the ID of the bastion host.
+        self.instance_id = instance_id  # type: str
+        # The number of the page to return. Default value: **1**.
         self.page_number = page_number  # type: str
         # The number of entries to return on each page.
         # 
         # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
         # 
         # >  We recommend that you do not leave this parameter empty.
         self.page_size = page_size  # type: str
-        # The name of the host account that you want to query. The name can be up to 128 characters in length. Only exact match is supported.
+        # The protocol used by the host whose accounts you want to query.
+        # 
+        # Valid values:
+        # 
+        # *   SSH
+        # *   RDP
         self.protocol_name = protocol_name  # type: str
-        # The ID of the specified host whose accounts you want to query.
+        # The region ID of the bastion host in which you want to query accounts of the specified host.
         # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListHostAccountsRequest, self).to_map()
@@ -7718,31 +13572,39 @@
             self.region_id = m.get('RegionId')
         return self
 
 
 class ListHostAccountsResponseBodyHostAccounts(TeaModel):
     def __init__(self, has_password=None, host_account_id=None, host_account_name=None, host_id=None,
                  host_share_key_id=None, host_share_key_name=None, private_key_fingerprint=None, protocol_name=None):
-        # The fingerprint of the private key for the host account.
+        # Indicates whether a password is configured for the host account.
+        # 
+        # Valid values:
+        # 
+        # *   true: A password is configured for the host account.
+        # *   false: No passwords are configured for the host account.
         self.has_password = has_password  # type: bool
-        # The ID of the request.
+        # The ID of the host account.
         self.host_account_id = host_account_id  # type: str
-        # The name of the shared key.
+        # The name of the host account.
         self.host_account_name = host_account_name  # type: str
+        # The ID of the host.
         self.host_id = host_id  # type: str
+        # The ID of the shared key.
         self.host_share_key_id = host_share_key_id  # type: str
+        # The name of the shared key.
         self.host_share_key_name = host_share_key_name  # type: str
+        # The fingerprint of the private key for the host account.
+        self.private_key_fingerprint = private_key_fingerprint  # type: str
         # The protocol that is used by the host.
         # 
         # Valid values:
         # 
         # *   SSH
         # *   RDP
-        self.private_key_fingerprint = private_key_fingerprint  # type: str
-        # The number of the page to return. Default value: **1**.
         self.protocol_name = protocol_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListHostAccountsResponseBodyHostAccounts, self).to_map()
@@ -7787,21 +13649,19 @@
         if m.get('ProtocolName') is not None:
             self.protocol_name = m.get('ProtocolName')
         return self
 
 
 class ListHostAccountsResponseBody(TeaModel):
     def __init__(self, host_accounts=None, request_id=None, total_count=None):
-        # The ID of the host account.
-        self.host_accounts = host_accounts  # type: list[ListHostAccountsResponseBodyHostAccounts]
         # An array that consists of the queried host accounts.
+        self.host_accounts = host_accounts  # type: list[ListHostAccountsResponseBodyHostAccounts]
+        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The ID of the bastion host in which you want to query accounts of the specified host.
-        # 
-        # >  You can call the DescribeInstances operation to query the ID of the bastion host.
+        # The total number of host accounts that are queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.host_accounts:
             for k in self.host_accounts:
                 if k:
                     k.validate()
@@ -8044,31 +13904,38 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListHostAccountsForUserRequest(TeaModel):
     def __init__(self, host_account_name=None, host_id=None, instance_id=None, page_number=None, page_size=None,
                  region_id=None, user_id=None):
-        # The number of the page to return. Default value: **1**.
+        # The name of the host account that you want to query. Exact match is supported.
         self.host_account_name = host_account_name  # type: str
-        # The ID of the host for which the host accounts were queried.
+        # The ID of the host to query.
+        # 
+        # > You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
         self.host_id = host_id  # type: str
-        # The total number of host accounts returned.
-        self.instance_id = instance_id  # type: str
-        # The ID of the user for which you want to query authorized host accounts.
+        # The ID of the bastion host on which you want to perform the query. The host accounts that the specified user is authorized to manage on the specified host are queried.
         # 
-        # >  You can call the [ListUsers](~~204522~~) operation to query the ID of the user ID.
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id  # type: str
+        # The number of the page to return. Default value: **1**.
         self.page_number = page_number  # type: str
-        # The name of the host account that you want to query. Exact match is supported.
+        # The number of entries to return on each page.\
+        # Maximum value: 100. Default value: 20. If you leave this parameter empty, 20 entries are returned on each page.
+        # 
+        # > We recommend that you do not leave this parameter empty.
         self.page_size = page_size  # type: str
-        # The name of the host account.
+        # The region ID of the bastion host on which you want to perform the query. The host accounts that the specified user is authorized to manage on the specified host are queried.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
-        # The region ID of the Bastionhost instance where you want to query the host accounts that the user is authorized to manage on the host.
+        # The ID of the user for which you want to query authorized host accounts.
         # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        # > You can call the [ListUsers](~~204522~~) operation to query the ID of the user.
         self.user_id = user_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListHostAccountsForUserRequest, self).to_map()
@@ -8110,31 +13977,29 @@
             self.user_id = m.get('UserId')
         return self
 
 
 class ListHostAccountsForUserResponseBodyHostAccounts(TeaModel):
     def __init__(self, host_account_id=None, host_account_name=None, host_id=None, is_authorized=None,
                  protocol_name=None):
-        # The protocol that is used by the host account. Valid values:
-        # 
-        # *   **SSH**\
-        # *   **RDP**\
-        self.host_account_id = host_account_id  # type: str
         # The ID of the host account.
+        self.host_account_id = host_account_id  # type: str
+        # The name of the host account.
         self.host_account_name = host_account_name  # type: str
-        # The ID of the request.
+        # The ID of the host for which the host accounts were queried.
         self.host_id = host_id  # type: str
-        # The ID of the host for which you want to query the host accounts that the user is authorized to manage.
+        # Indicates whether the user is authorized to manage the host account. Valid values:
         # 
-        # >  You can call the [ListHosts](~~200665~~) operation to query the ID of the host.
+        # *   **true**: yes
+        # *   **false**: no
         self.is_authorized = is_authorized  # type: bool
-        # Indicates whether the user is authorized to manage the host account. Valid values:
+        # The protocol that is used by the host. Valid values:
         # 
-        # *   **true**: The user is authorized to manage the host account.
-        # *   **false**: The user is not authorized to manage the host account.
+        # *   **SSH**\
+        # *   **RDP**\
         self.protocol_name = protocol_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListHostAccountsForUserResponseBodyHostAccounts, self).to_map()
@@ -8167,25 +14032,19 @@
         if m.get('ProtocolName') is not None:
             self.protocol_name = m.get('ProtocolName')
         return self
 
 
 class ListHostAccountsForUserResponseBody(TeaModel):
     def __init__(self, host_accounts=None, request_id=None, total_count=None):
-        # The host accounts returned.
+        # An array that consists of the queried host accounts.
         self.host_accounts = host_accounts  # type: list[ListHostAccountsForUserResponseBodyHostAccounts]
-        # The ID of the Bastionhost instance where you want to query the host accounts that the user is authorized to manage on the host.
-        # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        # The ID of the request.
         self.request_id = request_id  # type: str
-        # The number of entries to return on each page.
-        # 
-        # The value of the PageSize parameter must not exceed 100. Default value: 20. If you leave the PageSize parameter empty, 20 entries are returned on each page.
-        # 
-        # >  We recommend that you do not leave the PageSize parameter empty.
+        # The total number of host accounts that were queried.
         self.total_count = total_count  # type: int
 
     def validate(self):
         if self.host_accounts:
             for k in self.host_accounts:
                 if k:
                     k.validate()
@@ -10197,14 +16056,1080 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListHostsForUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListNetworkDomainsRequest(TeaModel):
+    def __init__(self, instance_id=None, network_domain_name=None, network_domain_type=None, page_number=None,
+                 page_size=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.network_domain_name = network_domain_name  # type: str
+        self.network_domain_type = network_domain_type  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListNetworkDomainsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, node_type=None, proxy_state=None):
+        self.node_type = node_type  # type: str
+        self.proxy_state = proxy_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListNetworkDomainsResponseBodyNetworkDomainsProxiesState, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('NodeType') is not None:
+            self.node_type = m.get('NodeType')
+        if m.get('ProxyState') is not None:
+            self.proxy_state = m.get('ProxyState')
+        return self
+
+
+class ListNetworkDomainsResponseBodyNetworkDomains(TeaModel):
+    def __init__(self, comment=None, default=None, network_domain_id=None, network_domain_name=None,
+                 network_domain_type=None, proxies_state=None):
+        self.comment = comment  # type: str
+        self.default = default  # type: bool
+        self.network_domain_id = network_domain_id  # type: str
+        self.network_domain_name = network_domain_name  # type: str
+        self.network_domain_type = network_domain_type  # type: str
+        self.proxies_state = proxies_state  # type: list[ListNetworkDomainsResponseBodyNetworkDomainsProxiesState]
+
+    def validate(self):
+        if self.proxies_state:
+            for k in self.proxies_state:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListNetworkDomainsResponseBodyNetworkDomains, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, network_domains=None, request_id=None, total_count=None):
+        self.network_domains = network_domains  # type: list[ListNetworkDomainsResponseBodyNetworkDomains]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.network_domains:
+            for k in self.network_domains:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListNetworkDomainsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListNetworkDomainsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListNetworkDomainsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_name=None, database_id=None, instance_id=None, page_number=None,
+                 page_size=None, region_id=None):
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationDatabaseAccountsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, dbname=None, database_account_id=None, database_account_name=None, database_id=None,
+                 has_password=None, login_attribute=None, protocol_name=None):
+        self.dbname = dbname  # type: str
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_id = database_id  # type: str
+        self.has_password = has_password  # type: str
+        self.login_attribute = login_attribute  # type: str
+        self.protocol_name = protocol_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationDatabaseAccountsResponseBodyDatabaseAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_accounts=None, request_id=None, total_count=None):
+        self.database_accounts = database_accounts  # type: list[ListOperationDatabaseAccountsResponseBodyDatabaseAccounts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.database_accounts:
+            for k in self.database_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListOperationDatabaseAccountsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListOperationDatabaseAccountsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListOperationDatabaseAccountsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_address=None, database_name=None, database_type=None, instance_id=None,
+                 page_number=None, page_size=None, region_id=None, source=None, source_instance_id=None,
+                 source_instance_state=None):
+        self.database_address = database_address  # type: str
+        self.database_name = database_name  # type: str
+        self.database_type = database_type  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationDatabasesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, database_id=None, database_name=None,
+                 database_port=None, database_private_address=None, database_public_address=None, database_type=None,
+                 source=None, source_instance_id=None, source_instance_region_id=None, source_instance_state=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: long
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.database_type = database_type  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_region_id = source_instance_region_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationDatabasesResponseBodyDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, databases=None, request_id=None, total_count=None):
+        self.databases = databases  # type: list[ListOperationDatabasesResponseBodyDatabases]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.databases:
+            for k in self.databases:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListOperationDatabasesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListOperationDatabasesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListOperationDatabasesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, host_account_name=None, host_id=None, instance_id=None, page_number=None, page_size=None,
+                 region_id=None):
+        self.host_account_name = host_account_name  # type: str
+        self.host_id = host_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationHostAccountsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, enable_sftpchannel=None, enable_sshchannel=None):
+        self.enable_sftpchannel = enable_sftpchannel  # type: bool
+        self.enable_sshchannel = enable_sshchannel  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationHostAccountsResponseBodyHostAccountsSSHConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('EnableSFTPChannel') is not None:
+            self.enable_sftpchannel = m.get('EnableSFTPChannel')
+        if m.get('EnableSSHChannel') is not None:
+            self.enable_sshchannel = m.get('EnableSSHChannel')
+        return self
+
+
+class ListOperationHostAccountsResponseBodyHostAccounts(TeaModel):
+    def __init__(self, has_password=None, host_account_id=None, host_account_name=None, host_id=None,
+                 host_share_key_id=None, private_key_fingerprint=None, protocol_name=None, sshconfig=None):
+        self.has_password = has_password  # type: bool
+        self.host_account_id = host_account_id  # type: str
+        self.host_account_name = host_account_name  # type: str
+        self.host_id = host_id  # type: str
+        self.host_share_key_id = host_share_key_id  # type: str
+        self.private_key_fingerprint = private_key_fingerprint  # type: str
+        self.protocol_name = protocol_name  # type: str
+        self.sshconfig = sshconfig  # type: ListOperationHostAccountsResponseBodyHostAccountsSSHConfig
+
+    def validate(self):
+        if self.sshconfig:
+            self.sshconfig.validate()
+
+    def to_map(self):
+        _map = super(ListOperationHostAccountsResponseBodyHostAccounts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, host_accounts=None, request_id=None, total_count=None):
+        self.host_accounts = host_accounts  # type: list[ListOperationHostAccountsResponseBodyHostAccounts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.host_accounts:
+            for k in self.host_accounts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListOperationHostAccountsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListOperationHostAccountsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListOperationHostAccountsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, host_address=None, host_name=None, instance_id=None, ostype=None, page_number=None,
+                 page_size=None, region_id=None, source=None, source_instance_id=None, source_instance_state=None):
+        self.host_address = host_address  # type: str
+        self.host_name = host_name  # type: str
+        self.instance_id = instance_id  # type: str
+        self.ostype = ostype  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationHostsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, active_address_type=None, comment=None, host_id=None, host_name=None,
+                 host_private_address=None, host_public_address=None, ostype=None, source=None, source_instance_id=None,
+                 source_instance_state=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.host_id = host_id  # type: str
+        self.host_name = host_name  # type: str
+        self.host_private_address = host_private_address  # type: str
+        self.host_public_address = host_public_address  # type: str
+        self.ostype = ostype  # type: str
+        self.source = source  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+        self.source_instance_state = source_instance_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListOperationHostsResponseBodyHosts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, hosts=None, request_id=None, total_count=None):
+        self.hosts = hosts  # type: list[ListOperationHostsResponseBodyHosts]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.hosts:
+            for k in self.hosts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListOperationHostsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListOperationHostsResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListOperationHostsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, asset_address=None, instance_id=None, page_number=None, page_size=None, region_id=None):
         self.asset_address = asset_address  # type: str
         self.instance_id = instance_id  # type: str
         self.page_number = page_number  # type: str
         self.page_size = page_size  # type: str
         self.region_id = region_id  # type: str
@@ -10416,14 +17341,353 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListOperationTicketsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListPoliciesRequest(TeaModel):
+    def __init__(self, instance_id=None, page_number=None, page_size=None, policy_name=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.policy_name = policy_name  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListPoliciesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, policy_id=None, policy_name=None, priority=None):
+        self.comment = comment  # type: str
+        self.policy_id = policy_id  # type: str
+        self.policy_name = policy_name  # type: str
+        self.priority = priority  # type: long
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListPoliciesResponseBodyPolicies, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, policies=None, request_id=None, total_count=None):
+        self.policies = policies  # type: list[ListPoliciesResponseBodyPolicies]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.policies:
+            for k in self.policies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListPoliciesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListPoliciesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListPoliciesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, page_number=None, page_size=None, region_id=None, rule_name=None,
+                 rule_state=None):
+        self.instance_id = instance_id  # type: str
+        self.page_number = page_number  # type: str
+        self.page_size = page_size  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_name = rule_name  # type: str
+        self.rule_state = rule_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListRulesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, effective_end_time=None, effective_start_time=None, rule_id=None,
+                 rule_name=None, rule_state=None):
+        self.comment = comment  # type: str
+        self.effective_end_time = effective_end_time  # type: long
+        self.effective_start_time = effective_start_time  # type: long
+        self.rule_id = rule_id  # type: str
+        self.rule_name = rule_name  # type: str
+        self.rule_state = rule_state  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ListRulesResponseBodyRules, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, rules=None, total_count=None):
+        self.request_id = request_id  # type: str
+        self.rules = rules  # type: list[ListRulesResponseBodyRules]
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.rules:
+            for k in self.rules:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ListRulesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ListRulesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ListRulesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, page_number=None, page_size=None, region_id=None, resource_type=None):
         # The number of the page to return.
         self.page_number = page_number  # type: int
         # The number of entries to return on each page.
         self.page_size = page_size  # type: int
         # The region ID of the bastion host.
@@ -10587,19 +17851,21 @@
             temp_model = ListTagKeysResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ListTagResourcesRequestTag(TeaModel):
     def __init__(self, key=None, value=None):
-        # The ID of the request.
+        # The key of tag N.
+        # 
+        # Valid values of N: 1 to 20.
         self.key = key  # type: str
-        # The type of the resource.
+        # The value of tag N.
         # 
-        # The returned value is INSTANCE, which indicates that the resource is a Bastionhost instance.
+        # Valid values of N: 1 to 20.
         self.value = value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTagResourcesRequestTag, self).to_map()
@@ -10620,27 +17886,25 @@
         if m.get('Value') is not None:
             self.value = m.get('Value')
         return self
 
 
 class ListTagResourcesRequest(TeaModel):
     def __init__(self, next_token=None, region_id=None, resource_id=None, resource_type=None, tag=None):
-        # The region ID of the Bastionhost instance.
+        # The token for starting the next query.
         self.next_token = next_token  # type: str
-        # The ID of the instance.
+        # The region ID of the Bastionhost instance.
         self.region_id = region_id  # type: str
-        # The value of the tag.
+        # The IDs of instances. The ID is up to 20.
         self.resource_id = resource_id  # type: list[str]
-        # The operation that you want to perform.
+        # The type of the resource.
         # 
-        # Set the value to **ListTagResources**.
+        # Set the value to INSTANCE, which indicates that the resource is a Bastionhost instance.
         self.resource_type = resource_type  # type: str
-        # The key of tag N.
-        # 
-        # Valid values of N: 1 to 20.
+        # The tags.
         self.tag = tag  # type: list[ListTagResourcesRequestTag]
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -10681,17 +17945,23 @@
                 temp_model = ListTagResourcesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
 
 class ListTagResourcesResponseBodyTagResources(TeaModel):
     def __init__(self, resource_id=None, resource_type=None, tag_key=None, tag_value=None):
+        # The ID of the instance.
         self.resource_id = resource_id  # type: str
+        # The type of the resource.
+        # 
+        # The returned value is INSTANCE, which indicates that the resource is a Bastionhost instance.
         self.resource_type = resource_type  # type: str
+        # The key of the tag.
         self.tag_key = tag_key  # type: str
+        # The value of the tag.
         self.tag_value = tag_value  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ListTagResourcesResponseBodyTagResources, self).to_map()
@@ -10720,19 +17990,21 @@
         if m.get('TagValue') is not None:
             self.tag_value = m.get('TagValue')
         return self
 
 
 class ListTagResourcesResponseBody(TeaModel):
     def __init__(self, next_token=None, request_id=None, tag_resources=None):
-        # Queries the tags bound to one or more Bastionhost instances.
+        # The token for starting the next query.
         self.next_token = next_token  # type: str
-        # ListTagResources
+        # The ID of the request.
         self.request_id = request_id  # type: str
-        # 58928
+        # The information about Bastionhost instances and the tags bound to Bastionhost instances.
+        # 
+        # The following information is included: instance ID, resource type, tag key, and tag value.
         self.tag_resources = tag_resources  # type: list[ListTagResourcesResponseBodyTagResources]
 
     def validate(self):
         if self.tag_resources:
             for k in self.tag_resources:
                 if k:
                     k.validate()
@@ -11655,14 +18927,260 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = LockUsersResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyDatabaseRequest(TeaModel):
+    def __init__(self, active_address_type=None, comment=None, database_id=None, database_name=None,
+                 database_port=None, database_private_address=None, database_public_address=None, instance_id=None,
+                 network_domain_id=None, region_id=None, source_instance_id=None):
+        self.active_address_type = active_address_type  # type: str
+        self.comment = comment  # type: str
+        self.database_id = database_id  # type: str
+        self.database_name = database_name  # type: str
+        self.database_port = database_port  # type: str
+        self.database_private_address = database_private_address  # type: str
+        self.database_public_address = database_public_address  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.region_id = region_id  # type: str
+        self.source_instance_id = source_instance_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatabaseRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatabaseResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatabaseResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyDatabaseResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyDatabaseResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_id=None, database_account_name=None, database_schema=None,
+                 instance_id=None, password=None, region_id=None):
+        self.database_account_id = database_account_id  # type: str
+        self.database_account_name = database_account_name  # type: str
+        self.database_schema = database_schema  # type: str
+        self.instance_id = instance_id  # type: str
+        self.password = password  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatabaseAccountRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyDatabaseAccountResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyDatabaseAccountResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyDatabaseAccountResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyDatabaseAccountResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, comment=None, host_id=None, host_name=None, host_private_address=None,
                  host_public_address=None, instance_id=None, network_domain_id=None, ostype=None, region_id=None):
         # The new description of the host. The description can be up to 500 characters in length.
         self.comment = comment  # type: str
         # The ID of the host.
         # 
@@ -11940,29 +19458,29 @@
             temp_model = ModifyHostAccountResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ModifyHostGroupRequest(TeaModel):
     def __init__(self, comment=None, host_group_id=None, host_group_name=None, instance_id=None, region_id=None):
-        # The new name of the host group. The name can be up to 128 characters in length.
+        # The new description of the host group. The value can be up to 500 characters in length.
         self.comment = comment  # type: str
-        # The region ID of the Bastionhost instance where you want to modify the information of the host group.
-        # 
-        # >  For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
-        self.host_group_id = host_group_id  # type: str
         # The ID of the host group that you want to modify.
         # 
-        # >  You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        # > You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
+        self.host_group_id = host_group_id  # type: str
+        # The new name of the host group. The name can be up to 128 characters in length.
         self.host_group_name = host_group_name  # type: str
-        # The ID of the request.
+        # The ID of the bastion host on which you want to modify the information about the host group.
+        # 
+        # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
-        # The ID of the Bastionhost instance where you want to modify the information of the host group.
+        # The region ID of the bastion host on which you want to modify the information about the host group.
         # 
-        # >  You can call the [DescribeInstances](~~153281~~) operation to query the ID of the Bastionhost instance.
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
         self.region_id = region_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ModifyHostGroupRequest, self).to_map()
@@ -13086,14 +20604,550 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyInstanceTwoFactorResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyNetworkDomainRequestProxies(TeaModel):
+    def __init__(self, address=None, node_type=None, password=None, port=None, proxy_type=None, user=None):
+        self.address = address  # type: str
+        self.node_type = node_type  # type: str
+        self.password = password  # type: str
+        self.port = port  # type: int
+        self.proxy_type = proxy_type  # type: str
+        self.user = user  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyNetworkDomainRequestProxies, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, instance_id=None, network_domain_id=None, network_domain_name=None,
+                 network_domain_type=None, proxies=None, region_id=None):
+        self.comment = comment  # type: str
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.network_domain_name = network_domain_name  # type: str
+        self.network_domain_type = network_domain_type  # type: str
+        self.proxies = proxies  # type: list[ModifyNetworkDomainRequestProxies]
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.proxies:
+            for k in self.proxies:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(ModifyNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyNetworkDomainResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyNetworkDomainResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, comment=None, instance_id=None, policy_id=None, policy_name=None, priority=None,
+                 region_id=None):
+        self.comment = comment  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.policy_name = policy_name  # type: str
+        self.priority = priority  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyPolicyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyPolicyResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyPolicyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyPolicyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyPolicyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_account_ids=None, database_id=None):
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyRuleRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('DatabaseAccountIds') is not None:
+            self.database_account_ids = m.get('DatabaseAccountIds')
+        if m.get('DatabaseId') is not None:
+            self.database_id = m.get('DatabaseId')
+        return self
+
+
+class ModifyRuleRequestHostGroups(TeaModel):
+    def __init__(self, host_account_names=None, host_group_id=None):
+        self.host_account_names = host_account_names  # type: list[str]
+        self.host_group_id = host_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyRuleRequestHostGroups, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountNames') is not None:
+            self.host_account_names = m.get('HostAccountNames')
+        if m.get('HostGroupId') is not None:
+            self.host_group_id = m.get('HostGroupId')
+        return self
+
+
+class ModifyRuleRequestHosts(TeaModel):
+    def __init__(self, host_account_ids=None, host_id=None):
+        self.host_account_ids = host_account_ids  # type: list[str]
+        self.host_id = host_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyRuleRequestHosts, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('HostAccountIds') is not None:
+            self.host_account_ids = m.get('HostAccountIds')
+        if m.get('HostId') is not None:
+            self.host_id = m.get('HostId')
+        return self
+
+
+class ModifyRuleRequest(TeaModel):
+    def __init__(self, comment=None, databases=None, effective_end_time=None, effective_start_time=None,
+                 host_groups=None, hosts=None, instance_id=None, region_id=None, rule_id=None, rule_name=None,
+                 user_group_ids=None, user_ids=None):
+        self.comment = comment  # type: str
+        self.databases = databases  # type: list[ModifyRuleRequestDatabases]
+        self.effective_end_time = effective_end_time  # type: long
+        self.effective_start_time = effective_start_time  # type: long
+        self.host_groups = host_groups  # type: list[ModifyRuleRequestHostGroups]
+        self.hosts = hosts  # type: list[ModifyRuleRequestHosts]
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.rule_id = rule_id  # type: str
+        self.rule_name = rule_name  # type: str
+        self.user_group_ids = user_group_ids  # type: list[str]
+        self.user_ids = user_ids  # type: list[str]
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
+        _map = super(ModifyRuleRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyRuleResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyRuleResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyRuleResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyRuleResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, comment=None, display_name=None, effective_end_time=None, effective_start_time=None,
                  email=None, instance_id=None, language=None, language_status=None, mobile=None, mobile_country_code=None,
                  need_reset_password=None, password=None, region_id=None, two_factor_methods=None, two_factor_status=None, user_id=None):
         # The new description of the user. The description can be up to 500 characters in length.
         self.comment = comment  # type: str
         # The new display name of the user. This display name can be up to 128 characters in length.
@@ -13421,14 +21475,429 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyUserGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyUserPublicKeyRequest(TeaModel):
+    def __init__(self, comment=None, instance_id=None, public_key=None, public_key_id=None, public_key_name=None,
+                 region_id=None):
+        # The new description of the user group. The description can be up to 500 characters in length.
+        self.comment = comment  # type: str
+        # The ID of the bastion host that is used to modify the public key of the user.
+        # 
+        # > You can call the [describeinstances](~~153281~~) operation to query the ID of the bastion host.
+        self.instance_id = instance_id  # type: str
+        # The new public key.
+        # 
+        # > The public key must be encoded in Base64.
+        self.public_key = public_key  # type: str
+        # The ID of the public key that you want to modify.
+        self.public_key_id = public_key_id  # type: str
+        # The name of the public key that you want to modify. This name can be up to 128 characters in length.
+        self.public_key_name = public_key_name  # type: str
+        # The region ID of the bastion host that is used to modify the public key of the user.
+        # 
+        # > For more information about the mapping between region IDs and region names, see [Regions and zones](~~40654~~).
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyUserPublicKeyRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        # The ID of the request, which is used to locate and troubleshoot issues.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyUserPublicKeyResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class ModifyUserPublicKeyResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyUserPublicKeyResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyUserPublicKeyResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, database_ids=None, instance_id=None, network_domain_id=None, region_id=None):
+        self.database_ids = database_ids  # type: list[str]
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MoveDatabasesToNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_id=None, message=None):
+        self.code = code  # type: str
+        self.database_id = database_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MoveDatabasesToNetworkDomainResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[MoveDatabasesToNetworkDomainResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(MoveDatabasesToNetworkDomainResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: MoveDatabasesToNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(MoveDatabasesToNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, host_ids=None, instance_id=None, network_domain_id=None, region_id=None):
+        self.host_ids = host_ids  # type: list[str]
+        self.instance_id = instance_id  # type: str
+        self.network_domain_id = network_domain_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MoveHostsToNetworkDomainRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, host_id=None, message=None):
+        self.code = code  # type: str
+        self.host_id = host_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(MoveHostsToNetworkDomainResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[MoveHostsToNetworkDomainResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(MoveHostsToNetworkDomainResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: MoveHostsToNetworkDomainResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(MoveHostsToNetworkDomainResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, region_id=None, resource_group_id=None, resource_id=None, resource_type=None):
         # The region ID of the bastion host.
         self.region_id = region_id  # type: str
         # The ID of the resource group to which the bastion host is moved.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the resource group ID of the bastion host.
@@ -13725,14 +22194,165 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RejectOperationTicketResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RemoveDatabasesFromGroupRequest(TeaModel):
+    def __init__(self, database_ids=None, host_group_id=None, instance_id=None, region_id=None):
+        self.database_ids = database_ids  # type: list[str]
+        self.host_group_id = host_group_id  # type: str
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RemoveDatabasesFromGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, code=None, database_id=None, host_group_id=None, message=None):
+        self.code = code  # type: str
+        self.database_id = database_id  # type: str
+        self.host_group_id = host_group_id  # type: str
+        self.message = message  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RemoveDatabasesFromGroupResponseBodyResults, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, results=None):
+        self.request_id = request_id  # type: str
+        self.results = results  # type: list[RemoveDatabasesFromGroupResponseBodyResults]
+
+    def validate(self):
+        if self.results:
+            for k in self.results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(RemoveDatabasesFromGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RemoveDatabasesFromGroupResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RemoveDatabasesFromGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, host_group_id=None, host_ids=None, instance_id=None, region_id=None):
         # The ID of the host group from which you want to remove hosts.
         # 
         # >  You can call the [ListHostGroups](~~201307~~) operation to query the ID of the host group.
         self.host_group_id = host_group_id  # type: str
         # The ID of the host that you want to remove from the host group. The value is a JSON string. You can add up to 100 host IDs.
@@ -14083,14 +22703,108 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RemoveUsersFromGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RenewAssetOperationTokenRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, token_id=None):
+        self.instance_id = instance_id  # type: str
+        self.region_id = region_id  # type: str
+        self.token_id = token_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RenewAssetOperationTokenRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(RenewAssetOperationTokenResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class RenewAssetOperationTokenResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: RenewAssetOperationTokenResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(RenewAssetOperationTokenResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, credential_type=None, host_account_id=None, instance_id=None, region_id=None):
         # The type of the logon credential that you want to delete. Valid values:
         # 
         # *   **Password**\
         # *   **PrivateKey**\
         self.credential_type = credential_type  # type: str
@@ -14196,14 +22910,1412 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ResetHostAccountCredentialResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime(TeaModel):
+    def __init__(self, days=None, hours=None):
+        self.days = days  # type: list[int]
+        self.hours = hours  # type: list[int]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Days') is not None:
+            self.days = m.get('Days')
+        if m.get('Hours') is not None:
+            self.hours = m.get('Hours')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig(TeaModel):
+    def __init__(self, effective_time=None):
+        self.effective_time = effective_time  # type: list[SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfigEffectiveTime]
+
+    def validate(self):
+        if self.effective_time:
+            for k in self.effective_time:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, access_time_range_config=None, instance_id=None, policy_id=None, region_id=None):
+        self.access_time_range_config = access_time_range_config  # type: SetPolicyAccessTimeRangeConfigRequestAccessTimeRangeConfig
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.access_time_range_config:
+            self.access_time_range_config.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, access_time_range_config_shrink=None, instance_id=None, policy_id=None, region_id=None):
+        self.access_time_range_config_shrink = access_time_range_config_shrink  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyAccessTimeRangeConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyAccessTimeRangeConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyAccessTimeRangeConfigResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, switch_status=None):
+        self.switch_status = switch_status  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyApprovalConfigRequestApprovalConfig, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.switch_status is not None:
+            result['SwitchStatus'] = self.switch_status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('SwitchStatus') is not None:
+            self.switch_status = m.get('SwitchStatus')
+        return self
+
+
+class SetPolicyApprovalConfigRequest(TeaModel):
+    def __init__(self, approval_config=None, instance_id=None, policy_id=None, region_id=None):
+        self.approval_config = approval_config  # type: SetPolicyApprovalConfigRequestApprovalConfig
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.approval_config:
+            self.approval_config.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyApprovalConfigRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, approval_config_shrink=None, instance_id=None, policy_id=None, region_id=None):
+        self.approval_config_shrink = approval_config_shrink  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyApprovalConfigShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyApprovalConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyApprovalConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyApprovalConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyApprovalConfigResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, account_scope_type=None, database_account_ids=None, database_id=None):
+        self.account_scope_type = account_scope_type  # type: str
+        self.database_account_ids = database_account_ids  # type: list[str]
+        self.database_id = database_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAssetScopeRequestDatabases, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, account_names=None, account_scope_type=None, host_group_id=None):
+        self.account_names = account_names  # type: list[str]
+        self.account_scope_type = account_scope_type  # type: str
+        self.host_group_id = host_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAssetScopeRequestHostGroups, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, account_scope_type=None, host_account_ids=None, host_id=None):
+        self.account_scope_type = account_scope_type  # type: str
+        self.host_account_ids = host_account_ids  # type: list[str]
+        self.host_id = host_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAssetScopeRequestHosts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, databases=None, host_groups=None, hosts=None, instance_id=None, policy_id=None,
+                 region_id=None, scope_type=None):
+        self.databases = databases  # type: list[SetPolicyAssetScopeRequestDatabases]
+        self.host_groups = host_groups  # type: list[SetPolicyAssetScopeRequestHostGroups]
+        self.hosts = hosts  # type: list[SetPolicyAssetScopeRequestHosts]
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+        self.scope_type = scope_type  # type: str
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
+        _map = super(SetPolicyAssetScopeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyAssetScopeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyAssetScopeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyAssetScopeResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyAssetScopeResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, commands=None):
+        self.commands = commands  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigRequestCommandConfigApproval, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.commands is not None:
+            result['Commands'] = self.commands
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class SetPolicyCommandConfigRequestCommandConfigDeny(TeaModel):
+    def __init__(self, acl_type=None, commands=None):
+        self.acl_type = acl_type  # type: str
+        self.commands = commands  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigRequestCommandConfigDeny, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('Commands') is not None:
+            self.commands = m.get('Commands')
+        return self
+
+
+class SetPolicyCommandConfigRequestCommandConfig(TeaModel):
+    def __init__(self, approval=None, deny=None):
+        self.approval = approval  # type: SetPolicyCommandConfigRequestCommandConfigApproval
+        self.deny = deny  # type: SetPolicyCommandConfigRequestCommandConfigDeny
+
+    def validate(self):
+        if self.approval:
+            self.approval.validate()
+        if self.deny:
+            self.deny.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigRequestCommandConfig, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, command_config=None, instance_id=None, policy_id=None, region_id=None):
+        self.command_config = command_config  # type: SetPolicyCommandConfigRequestCommandConfig
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.command_config:
+            self.command_config.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, command_config_shrink=None, instance_id=None, policy_id=None, region_id=None):
+        self.command_config_shrink = command_config_shrink  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyCommandConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyCommandConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyCommandConfigResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, acl_type=None, ips=None):
+        self.acl_type = acl_type  # type: str
+        self.ips = ips  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyIPAclConfigRequestIPAclConfig, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('AclType') is not None:
+            self.acl_type = m.get('AclType')
+        if m.get('IPs') is not None:
+            self.ips = m.get('IPs')
+        return self
+
+
+class SetPolicyIPAclConfigRequest(TeaModel):
+    def __init__(self, ipacl_config=None, instance_id=None, policy_id=None, region_id=None):
+        self.ipacl_config = ipacl_config  # type: SetPolicyIPAclConfigRequestIPAclConfig
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.ipacl_config:
+            self.ipacl_config.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyIPAclConfigRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, ipacl_config_shrink=None, instance_id=None, policy_id=None, region_id=None):
+        self.ipacl_config_shrink = ipacl_config_shrink  # type: str
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyIPAclConfigShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyIPAclConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyIPAclConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyIPAclConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyIPAclConfigResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, clipboard_download=None, clipboard_upload=None, disk_redirection=None, record_keyboard=None):
+        self.clipboard_download = clipboard_download  # type: str
+        self.clipboard_upload = clipboard_upload  # type: str
+        self.disk_redirection = disk_redirection  # type: str
+        self.record_keyboard = record_keyboard  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigRequestProtocolConfigRDP, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, exec_command=None, sftpchannel=None, sftpdownload_file=None, sftpmkdir=None,
+                 sftpremove_file=None, sftprename_file=None, sftprmdir=None, sftpupload_file=None, sshchannel=None,
+                 x_11forwarding=None):
+        self.exec_command = exec_command  # type: str
+        self.sftpchannel = sftpchannel  # type: str
+        self.sftpdownload_file = sftpdownload_file  # type: str
+        self.sftpmkdir = sftpmkdir  # type: str
+        self.sftpremove_file = sftpremove_file  # type: str
+        self.sftprename_file = sftprename_file  # type: str
+        self.sftprmdir = sftprmdir  # type: str
+        self.sftpupload_file = sftpupload_file  # type: str
+        self.sshchannel = sshchannel  # type: str
+        self.x_11forwarding = x_11forwarding  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigRequestProtocolConfigSSH, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, rdp=None, ssh=None):
+        self.rdp = rdp  # type: SetPolicyProtocolConfigRequestProtocolConfigRDP
+        self.ssh = ssh  # type: SetPolicyProtocolConfigRequestProtocolConfigSSH
+
+    def validate(self):
+        if self.rdp:
+            self.rdp.validate()
+        if self.ssh:
+            self.ssh.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigRequestProtocolConfig, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, policy_id=None, protocol_config=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.protocol_config = protocol_config  # type: SetPolicyProtocolConfigRequestProtocolConfig
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        if self.protocol_config:
+            self.protocol_config.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, policy_id=None, protocol_config_shrink=None, region_id=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.protocol_config_shrink = protocol_config_shrink  # type: str
+        self.region_id = region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigShrinkRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyProtocolConfigResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyProtocolConfigResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyProtocolConfigResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, policy_id=None, region_id=None, scope_type=None, user_group_ids=None,
+                 user_ids=None):
+        self.instance_id = instance_id  # type: str
+        self.policy_id = policy_id  # type: str
+        self.region_id = region_id  # type: str
+        self.scope_type = scope_type  # type: str
+        self.user_group_ids = user_group_ids  # type: list[str]
+        self.user_ids = user_ids  # type: list[str]
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyUserScopeRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SetPolicyUserScopeResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SetPolicyUserScopeResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SetPolicyUserScopeResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SetPolicyUserScopeResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, region_id=None, security_group_ids=None, vswitch_id=None):
         # The ID of the bastion host that you want to enable.
         # 
         # > You can call the [DescribeInstances](~~153281~~) operation to query the ID of the bastion host.
         self.instance_id = instance_id  # type: str
         # The region ID of the bastion host.
@@ -14768,7 +24880,272 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = UntagResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class VerifyInstanceADAuthServerRequest(TeaModel):
+    def __init__(self, account=None, base_dn=None, domain=None, filter=None, instance_id=None, is_ssl=None,
+                 password=None, port=None, region_id=None, server=None, standby_server=None):
+        self.account = account  # type: str
+        self.base_dn = base_dn  # type: str
+        self.domain = domain  # type: str
+        self.filter = filter  # type: str
+        self.instance_id = instance_id  # type: str
+        self.is_ssl = is_ssl  # type: str
+        self.password = password  # type: str
+        self.port = port  # type: str
+        self.region_id = region_id  # type: str
+        self.server = server  # type: str
+        self.standby_server = standby_server  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyInstanceADAuthServerRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyInstanceADAuthServerResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VerifyInstanceADAuthServerResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VerifyInstanceADAuthServerResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VerifyInstanceADAuthServerResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, account=None, base_dn=None, filter=None, instance_id=None, is_ssl=None, password=None,
+                 port=None, region_id=None, server=None, standby_server=None):
+        self.account = account  # type: str
+        self.base_dn = base_dn  # type: str
+        self.filter = filter  # type: str
+        self.instance_id = instance_id  # type: str
+        self.is_ssl = is_ssl  # type: str
+        self.password = password  # type: str
+        self.port = port  # type: str
+        self.region_id = region_id  # type: str
+        self.server = server  # type: str
+        self.standby_server = standby_server  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyInstanceLDAPAuthServerRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(VerifyInstanceLDAPAuthServerResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class VerifyInstanceLDAPAuthServerResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: VerifyInstanceLDAPAuthServerResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(VerifyInstanceLDAPAuthServerResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/PKG-INFO` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-yundun-bastionhost20191209-py2
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/alibabacloud_yundun_bastionhost20191209_py2.egg-info/SOURCES.txt` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/alibabacloud_yundun_bastionhost20191209_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_yundun-bastionhost20191209_py2-1.1.2/setup.py` & `alibabacloud_yundun-bastionhost20191209_py2-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_yundun-bastionhost20191209_py2.
 
-Created on 28/02/2024
+Created on 12/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_yundun_bastionhost20191209"
 NAME = "alibabacloud_yundun-bastionhost20191209_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Yundun-bastionhost (20191209) SDK Library for Python2"
```

