# Comparing `tmp/seam-0.3.0.tar.gz` & `tmp/seam-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.3.0.tar", max compression
+gzip compressed data, was "seam-0.3.1.tar", max compression
```

## Comparing `seam-0.3.0.tar` & `seam-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1087 2024-04-11 09:49:56.083822 seam-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4228 2024-04-11 09:49:56.083822 seam-0.3.0/README.rst
--rw-r--r--   0        0        0      726 2024-04-11 09:49:56.083822 seam-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       97 2024-04-11 09:49:56.083822 seam-0.3.0/seam/__init__.py
--rw-r--r--   0        0        0    11938 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes.py
--rw-r--r--   0        0        0      903 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes_simulate.py
--rw-r--r--   0        0        0     3979 2024-04-11 09:49:56.083822 seam-0.3.0/seam/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1746 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs.py
--rw-r--r--   0        0        0     2505 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_access_groups.py
--rw-r--r--   0        0        0      718 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credential_pools.py
--rw-r--r--   0        0        0     1782 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4763 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_credentials.py
--rw-r--r--   0        0        0     2172 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_entrances.py
--rw-r--r--   0        0        0      955 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_systems.py
--rw-r--r--   0        0        0     6476 2024-04-11 09:49:56.083822 seam-0.3.0/seam/acs_users.py
--rw-r--r--   0        0        0     3169 2024-04-11 09:49:56.083822 seam-0.3.0/seam/action_attempts.py
--rw-r--r--   0        0        0     5751 2024-04-11 09:49:56.083822 seam-0.3.0/seam/client_sessions.py
--rw-r--r--   0        0        0     3292 2024-04-11 09:49:56.083822 seam-0.3.0/seam/connect_webviews.py
--rw-r--r--   0        0        0     2520 2024-04-11 09:49:56.083822 seam-0.3.0/seam/connected_accounts.py
--rw-r--r--   0        0        0     4761 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices.py
--rw-r--r--   0        0        0      517 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices_simulate.py
--rw-r--r--   0        0        0     3323 2024-04-11 09:49:56.083822 seam-0.3.0/seam/devices_unmanaged.py
--rw-r--r--   0        0        0     2385 2024-04-11 09:49:56.083822 seam-0.3.0/seam/events.py
--rw-r--r--   0        0        0     4181 2024-04-11 09:49:56.083822 seam-0.3.0/seam/locks.py
--rw-r--r--   0        0        0      765 2024-04-11 09:49:56.083822 seam-0.3.0/seam/networks.py
--rw-r--r--   0        0        0      714 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors.py
--rw-r--r--   0        0        0     4350 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      594 2024-04-11 09:49:56.083822 seam-0.3.0/seam/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1063 2024-04-11 09:49:56.083822 seam-0.3.0/seam/phones.py
--rw-r--r--   0        0        0     1185 2024-04-11 09:49:56.083822 seam-0.3.0/seam/phones_simulate.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:49:56.083822 seam-0.3.0/seam/routes.py
--rw-r--r--   0        0        0     3175 2024-04-11 09:49:56.083822 seam-0.3.0/seam/seam.py
--rw-r--r--   0        0        0     8926 2024-04-11 09:49:56.083822 seam-0.3.0/seam/thermostats.py
--rw-r--r--   0        0        0     6930 2024-04-11 09:49:56.083822 seam-0.3.0/seam/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    64645 2024-04-11 09:49:56.083822 seam-0.3.0/seam/types.py
--rw-r--r--   0        0        0     6700 2024-04-11 09:49:56.083822 seam-0.3.0/seam/user_identities.py
--rw-r--r--   0        0        0     2903 2024-04-11 09:49:56.083822 seam-0.3.0/seam/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-04-11 09:49:56.083822 seam-0.3.0/seam/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1815 2024-04-11 09:49:56.083822 seam-0.3.0/seam/webhooks.py
--rw-r--r--   0        0        0     1845 2024-04-11 09:49:56.083822 seam-0.3.0/seam/workspaces.py
--rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 seam-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-12 08:24:40.069915 seam-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     4228 2024-04-12 08:24:40.069915 seam-0.3.1/README.rst
+-rw-r--r--   0        0        0      726 2024-04-12 08:24:40.069915 seam-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-04-12 08:24:40.069915 seam-0.3.1/seam/__init__.py
+-rw-r--r--   0        0        0    11938 2024-04-12 08:24:40.069915 seam-0.3.1/seam/access_codes.py
+-rw-r--r--   0        0        0      903 2024-04-12 08:24:40.069915 seam-0.3.1/seam/access_codes_simulate.py
+-rw-r--r--   0        0        0     3979 2024-04-12 08:24:40.069915 seam-0.3.1/seam/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1746 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs.py
+-rw-r--r--   0        0        0     2505 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_access_groups.py
+-rw-r--r--   0        0        0      718 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_credential_pools.py
+-rw-r--r--   0        0        0     1782 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4763 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_credentials.py
+-rw-r--r--   0        0        0     2172 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_entrances.py
+-rw-r--r--   0        0        0      955 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_systems.py
+-rw-r--r--   0        0        0     6476 2024-04-12 08:24:40.069915 seam-0.3.1/seam/acs_users.py
+-rw-r--r--   0        0        0     3169 2024-04-12 08:24:40.073915 seam-0.3.1/seam/action_attempts.py
+-rw-r--r--   0        0        0     5751 2024-04-12 08:24:40.073915 seam-0.3.1/seam/client_sessions.py
+-rw-r--r--   0        0        0     3292 2024-04-12 08:24:40.073915 seam-0.3.1/seam/connect_webviews.py
+-rw-r--r--   0        0        0     2520 2024-04-12 08:24:40.073915 seam-0.3.1/seam/connected_accounts.py
+-rw-r--r--   0        0        0     4761 2024-04-12 08:24:40.073915 seam-0.3.1/seam/devices.py
+-rw-r--r--   0        0        0      517 2024-04-12 08:24:40.073915 seam-0.3.1/seam/devices_simulate.py
+-rw-r--r--   0        0        0     3323 2024-04-12 08:24:40.073915 seam-0.3.1/seam/devices_unmanaged.py
+-rw-r--r--   0        0        0     2385 2024-04-12 08:24:40.073915 seam-0.3.1/seam/events.py
+-rw-r--r--   0        0        0     4181 2024-04-12 08:24:40.073915 seam-0.3.1/seam/locks.py
+-rw-r--r--   0        0        0      765 2024-04-12 08:24:40.073915 seam-0.3.1/seam/networks.py
+-rw-r--r--   0        0        0      714 2024-04-12 08:24:40.073915 seam-0.3.1/seam/noise_sensors.py
+-rw-r--r--   0        0        0     4350 2024-04-12 08:24:40.073915 seam-0.3.1/seam/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      594 2024-04-12 08:24:40.073915 seam-0.3.1/seam/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1063 2024-04-12 08:24:40.073915 seam-0.3.1/seam/phones.py
+-rw-r--r--   0        0        0     1185 2024-04-12 08:24:40.073915 seam-0.3.1/seam/phones_simulate.py
+-rw-r--r--   0        0        0     1535 2024-04-12 08:24:40.073915 seam-0.3.1/seam/routes.py
+-rw-r--r--   0        0        0     3175 2024-04-12 08:24:40.073915 seam-0.3.1/seam/seam.py
+-rw-r--r--   0        0        0     8926 2024-04-12 08:24:40.073915 seam-0.3.1/seam/thermostats.py
+-rw-r--r--   0        0        0     6930 2024-04-12 08:24:40.073915 seam-0.3.1/seam/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64645 2024-04-12 08:24:40.073915 seam-0.3.1/seam/types.py
+-rw-r--r--   0        0        0     6700 2024-04-12 08:24:40.073915 seam-0.3.1/seam/user_identities.py
+-rw-r--r--   0        0        0     2903 2024-04-12 08:24:40.073915 seam-0.3.1/seam/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-04-12 08:24:40.073915 seam-0.3.1/seam/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1815 2024-04-12 08:24:40.073915 seam-0.3.1/seam/webhooks.py
+-rw-r--r--   0        0        0     1845 2024-04-12 08:24:40.073915 seam-0.3.1/seam/workspaces.py
+-rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 seam-0.3.1/PKG-INFO
```

### Comparing `seam-0.3.0/LICENSE.txt` & `seam-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/README.rst` & `seam-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/pyproject.toml` & `seam-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seam"
-version = "0.3.0"
+version = "0.3.1"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
```

### Comparing `seam-0.3.0/seam/access_codes.py` & `seam-0.3.1/seam/access_codes.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,129 +20,129 @@
     def unmanaged(self) -> AccessCodesUnmanaged:
         return self._unmanaged
 
     def create(
         self,
         *,
         device_id: str,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
-        code: Optional[str] = None,
-        sync: Optional[bool] = None,
+        allow_external_modification: Optional[bool] = None,
         attempt_for_offline_device: Optional[bool] = None,
+        code: Optional[str] = None,
         common_code_key: Optional[str] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
-        max_time_rounding: Optional[str] = None
+        max_time_rounding: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        starts_at: Optional[str] = None,
+        sync: Optional[bool] = None,
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> AccessCode:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if name is not None:
-            json_payload["name"] = name
-        if starts_at is not None:
-            json_payload["starts_at"] = starts_at
-        if ends_at is not None:
-            json_payload["ends_at"] = ends_at
-        if code is not None:
-            json_payload["code"] = code
-        if sync is not None:
-            json_payload["sync"] = sync
+        if allow_external_modification is not None:
+            json_payload["allow_external_modification"] = allow_external_modification
         if attempt_for_offline_device is not None:
             json_payload["attempt_for_offline_device"] = attempt_for_offline_device
+        if code is not None:
+            json_payload["code"] = code
         if common_code_key is not None:
             json_payload["common_code_key"] = common_code_key
-        if prefer_native_scheduling is not None:
-            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
-        if use_backup_access_code_pool is not None:
-            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
-        if allow_external_modification is not None:
-            json_payload["allow_external_modification"] = allow_external_modification
+        if ends_at is not None:
+            json_payload["ends_at"] = ends_at
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
-        if use_offline_access_code is not None:
-            json_payload["use_offline_access_code"] = use_offline_access_code
         if is_offline_access_code is not None:
             json_payload["is_offline_access_code"] = is_offline_access_code
         if is_one_time_use is not None:
             json_payload["is_one_time_use"] = is_one_time_use
         if max_time_rounding is not None:
             json_payload["max_time_rounding"] = max_time_rounding
+        if name is not None:
+            json_payload["name"] = name
+        if prefer_native_scheduling is not None:
+            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
+        if starts_at is not None:
+            json_payload["starts_at"] = starts_at
+        if sync is not None:
+            json_payload["sync"] = sync
+        if use_backup_access_code_pool is not None:
+            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
+        if use_offline_access_code is not None:
+            json_payload["use_offline_access_code"] = use_offline_access_code
 
         res = self.seam.make_request("POST", "/access_codes/create", json=json_payload)
 
         return AccessCode.from_dict(res["access_code"])
 
     def create_multiple(
         self,
         *,
         device_ids: List[str],
+        allow_external_modification: Optional[bool] = None,
+        attempt_for_offline_device: Optional[bool] = None,
         behavior_when_code_cannot_be_shared: Optional[str] = None,
-        preferred_code_length: Optional[float] = None,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
         code: Optional[str] = None,
-        attempt_for_offline_device: Optional[bool] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
-        max_time_rounding: Optional[str] = None
+        max_time_rounding: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        preferred_code_length: Optional[float] = None,
+        starts_at: Optional[str] = None,
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> List[AccessCode]:
         json_payload = {}
 
         if device_ids is not None:
             json_payload["device_ids"] = device_ids
+        if allow_external_modification is not None:
+            json_payload["allow_external_modification"] = allow_external_modification
+        if attempt_for_offline_device is not None:
+            json_payload["attempt_for_offline_device"] = attempt_for_offline_device
         if behavior_when_code_cannot_be_shared is not None:
             json_payload["behavior_when_code_cannot_be_shared"] = (
                 behavior_when_code_cannot_be_shared
             )
-        if preferred_code_length is not None:
-            json_payload["preferred_code_length"] = preferred_code_length
-        if name is not None:
-            json_payload["name"] = name
-        if starts_at is not None:
-            json_payload["starts_at"] = starts_at
-        if ends_at is not None:
-            json_payload["ends_at"] = ends_at
         if code is not None:
             json_payload["code"] = code
-        if attempt_for_offline_device is not None:
-            json_payload["attempt_for_offline_device"] = attempt_for_offline_device
-        if prefer_native_scheduling is not None:
-            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
-        if use_backup_access_code_pool is not None:
-            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
-        if allow_external_modification is not None:
-            json_payload["allow_external_modification"] = allow_external_modification
+        if ends_at is not None:
+            json_payload["ends_at"] = ends_at
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
-        if use_offline_access_code is not None:
-            json_payload["use_offline_access_code"] = use_offline_access_code
         if is_offline_access_code is not None:
             json_payload["is_offline_access_code"] = is_offline_access_code
         if is_one_time_use is not None:
             json_payload["is_one_time_use"] = is_one_time_use
         if max_time_rounding is not None:
             json_payload["max_time_rounding"] = max_time_rounding
+        if name is not None:
+            json_payload["name"] = name
+        if prefer_native_scheduling is not None:
+            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
+        if preferred_code_length is not None:
+            json_payload["preferred_code_length"] = preferred_code_length
+        if starts_at is not None:
+            json_payload["starts_at"] = starts_at
+        if use_backup_access_code_pool is not None:
+            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
+        if use_offline_access_code is not None:
+            json_payload["use_offline_access_code"] = use_offline_access_code
 
         res = self.seam.make_request(
             "POST", "/access_codes/create_multiple", json=json_payload
         )
 
         return [AccessCode.from_dict(item) for item in res["access_codes"]]
 
@@ -177,44 +177,44 @@
         )
 
         return AccessCode.from_dict(res["generated_code"])
 
     def get(
         self,
         *,
-        device_id: Optional[str] = None,
         access_code_id: Optional[str] = None,
-        code: Optional[str] = None
+        code: Optional[str] = None,
+        device_id: Optional[str] = None
     ) -> AccessCode:
         json_payload = {}
 
-        if device_id is not None:
-            json_payload["device_id"] = device_id
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if code is not None:
             json_payload["code"] = code
+        if device_id is not None:
+            json_payload["device_id"] = device_id
 
         res = self.seam.make_request("POST", "/access_codes/get", json=json_payload)
 
         return AccessCode.from_dict(res["access_code"])
 
     def list(
         self,
         *,
-        device_id: Optional[str] = None,
         access_code_ids: Optional[List[str]] = None,
+        device_id: Optional[str] = None,
         user_identifier_key: Optional[str] = None
     ) -> List[AccessCode]:
         json_payload = {}
 
-        if device_id is not None:
-            json_payload["device_id"] = device_id
         if access_code_ids is not None:
             json_payload["access_code_ids"] = access_code_ids
+        if device_id is not None:
+            json_payload["device_id"] = device_id
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
         res = self.seam.make_request("POST", "/access_codes/list", json=json_payload)
 
         return [AccessCode.from_dict(item) for item in res["access_codes"]]
 
@@ -230,69 +230,69 @@
 
         return AccessCode.from_dict(res["backup_access_code"])
 
     def update(
         self,
         *,
         access_code_id: str,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
-        code: Optional[str] = None,
-        sync: Optional[bool] = None,
-        attempt_for_offline_device: Optional[bool] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
         allow_external_modification: Optional[bool] = None,
+        attempt_for_offline_device: Optional[bool] = None,
+        code: Optional[str] = None,
+        device_id: Optional[str] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
+        is_managed: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
-        device_id: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        starts_at: Optional[str] = None,
+        sync: Optional[bool] = None,
         type: Optional[str] = None,
-        is_managed: Optional[bool] = None
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None
     ) -> None:
         json_payload = {}
 
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
-        if name is not None:
-            json_payload["name"] = name
-        if starts_at is not None:
-            json_payload["starts_at"] = starts_at
-        if ends_at is not None:
-            json_payload["ends_at"] = ends_at
-        if code is not None:
-            json_payload["code"] = code
-        if sync is not None:
-            json_payload["sync"] = sync
-        if attempt_for_offline_device is not None:
-            json_payload["attempt_for_offline_device"] = attempt_for_offline_device
-        if prefer_native_scheduling is not None:
-            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
-        if use_backup_access_code_pool is not None:
-            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
         if allow_external_modification is not None:
             json_payload["allow_external_modification"] = allow_external_modification
+        if attempt_for_offline_device is not None:
+            json_payload["attempt_for_offline_device"] = attempt_for_offline_device
+        if code is not None:
+            json_payload["code"] = code
+        if device_id is not None:
+            json_payload["device_id"] = device_id
+        if ends_at is not None:
+            json_payload["ends_at"] = ends_at
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
-        if use_offline_access_code is not None:
-            json_payload["use_offline_access_code"] = use_offline_access_code
+        if is_managed is not None:
+            json_payload["is_managed"] = is_managed
         if is_offline_access_code is not None:
             json_payload["is_offline_access_code"] = is_offline_access_code
         if is_one_time_use is not None:
             json_payload["is_one_time_use"] = is_one_time_use
         if max_time_rounding is not None:
             json_payload["max_time_rounding"] = max_time_rounding
-        if device_id is not None:
-            json_payload["device_id"] = device_id
+        if name is not None:
+            json_payload["name"] = name
+        if prefer_native_scheduling is not None:
+            json_payload["prefer_native_scheduling"] = prefer_native_scheduling
+        if starts_at is not None:
+            json_payload["starts_at"] = starts_at
+        if sync is not None:
+            json_payload["sync"] = sync
         if type is not None:
             json_payload["type"] = type
-        if is_managed is not None:
-            json_payload["is_managed"] = is_managed
+        if use_backup_access_code_pool is not None:
+            json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
+        if use_offline_access_code is not None:
+            json_payload["use_offline_access_code"] = use_offline_access_code
 
         self.seam.make_request("POST", "/access_codes/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/access_codes_simulate.py` & `seam-0.3.1/seam/access_codes_simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 class AccessCodesSimulate(AbstractAccessCodesSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create_unmanaged_access_code(
-        self, *, device_id: str, name: str, code: str
+        self, *, code: str, device_id: str, name: str
     ) -> UnmanagedAccessCode:
         json_payload = {}
 
+        if code is not None:
+            json_payload["code"] = code
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
-        if code is not None:
-            json_payload["code"] = code
 
         res = self.seam.make_request(
             "POST",
             "/access_codes/simulate/create_unmanaged_access_code",
             json=json_payload,
         )
```

### Comparing `seam-0.3.0/seam/access_codes_unmanaged.py` & `seam-0.3.1/seam/access_codes_unmanaged.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,31 +12,31 @@
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def convert_to_managed(
         self,
         *,
         access_code_id: str,
-        is_external_modification_allowed: Optional[bool] = None,
         allow_external_modification: Optional[bool] = None,
         force: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None,
         sync: Optional[bool] = None
     ) -> None:
         json_payload = {}
 
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
-        if is_external_modification_allowed is not None:
-            json_payload["is_external_modification_allowed"] = (
-                is_external_modification_allowed
-            )
         if allow_external_modification is not None:
             json_payload["allow_external_modification"] = allow_external_modification
         if force is not None:
             json_payload["force"] = force
+        if is_external_modification_allowed is not None:
+            json_payload["is_external_modification_allowed"] = (
+                is_external_modification_allowed
+            )
         if sync is not None:
             json_payload["sync"] = sync
 
         self.seam.make_request(
             "POST", "/access_codes/unmanaged/convert_to_managed", json=json_payload
         )
 
@@ -55,26 +55,26 @@
         )
 
         return None
 
     def get(
         self,
         *,
-        device_id: Optional[str] = None,
         access_code_id: Optional[str] = None,
-        code: Optional[str] = None
+        code: Optional[str] = None,
+        device_id: Optional[str] = None
     ) -> UnmanagedAccessCode:
         json_payload = {}
 
-        if device_id is not None:
-            json_payload["device_id"] = device_id
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if code is not None:
             json_payload["code"] = code
+        if device_id is not None:
+            json_payload["device_id"] = device_id
 
         res = self.seam.make_request(
             "POST", "/access_codes/unmanaged/get", json=json_payload
         )
 
         return UnmanagedAccessCode.from_dict(res["access_code"])
 
@@ -96,30 +96,30 @@
 
     def update(
         self,
         *,
         access_code_id: str,
         is_managed: bool,
         allow_external_modification: Optional[bool] = None,
-        is_external_modification_allowed: Optional[bool] = None,
-        force: Optional[bool] = None
+        force: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None
     ) -> None:
         json_payload = {}
 
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if is_managed is not None:
             json_payload["is_managed"] = is_managed
         if allow_external_modification is not None:
             json_payload["allow_external_modification"] = allow_external_modification
+        if force is not None:
+            json_payload["force"] = force
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
-        if force is not None:
-            json_payload["force"] = force
 
         self.seam.make_request(
             "POST", "/access_codes/unmanaged/update", json=json_payload
         )
 
         return None
```

### Comparing `seam-0.3.0/seam/acs.py` & `seam-0.3.1/seam/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/acs_access_groups.py` & `seam-0.3.1/seam/acs_access_groups.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/acs_credential_pools.py` & `seam-0.3.1/seam/acs_credential_pools.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/acs_credential_provisioning_automations.py` & `seam-0.3.1/seam/acs_credential_provisioning_automations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def launch(
         self,
         *,
-        user_identity_id: str,
         credential_manager_acs_system_id: str,
+        user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
         credential_manager_acs_user_id: Optional[str] = None
     ) -> AcsCredentialProvisioningAutomation:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if credential_manager_acs_system_id is not None:
             json_payload["credential_manager_acs_system_id"] = (
                 credential_manager_acs_system_id
             )
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
         if acs_credential_pool_id is not None:
             json_payload["acs_credential_pool_id"] = acs_credential_pool_id
         if create_credential_manager_user is not None:
             json_payload["create_credential_manager_user"] = (
                 create_credential_manager_user
             )
         if credential_manager_acs_user_id is not None:
```

### Comparing `seam-0.3.0/seam/acs_credentials.py` & `seam-0.3.1/seam/acs_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,63 +4,63 @@
 
 class AcsCredentials(AbstractAcsCredentials):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
-    def assign(self, *, acs_user_id: str, acs_credential_id: str) -> None:
+    def assign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         json_payload = {}
 
-        if acs_user_id is not None:
-            json_payload["acs_user_id"] = acs_user_id
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
+        if acs_user_id is not None:
+            json_payload["acs_user_id"] = acs_user_id
 
         self.seam.make_request("POST", "/acs/credentials/assign", json=json_payload)
 
         return None
 
     def create(
         self,
         *,
-        acs_user_id: str,
         access_method: str,
-        credential_manager_acs_system_id: Optional[str] = None,
+        acs_user_id: str,
+        allowed_acs_entrance_ids: Optional[List[str]] = None,
         code: Optional[str] = None,
+        credential_manager_acs_system_id: Optional[str] = None,
+        ends_at: Optional[str] = None,
         is_multi_phone_sync_credential: Optional[bool] = None,
-        allowed_acs_entrance_ids: Optional[List[str]] = None,
-        visionline_metadata: Optional[Dict[str, Any]] = None,
         starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None
+        visionline_metadata: Optional[Dict[str, Any]] = None
     ) -> AcsCredential:
         json_payload = {}
 
-        if acs_user_id is not None:
-            json_payload["acs_user_id"] = acs_user_id
         if access_method is not None:
             json_payload["access_method"] = access_method
+        if acs_user_id is not None:
+            json_payload["acs_user_id"] = acs_user_id
+        if allowed_acs_entrance_ids is not None:
+            json_payload["allowed_acs_entrance_ids"] = allowed_acs_entrance_ids
+        if code is not None:
+            json_payload["code"] = code
         if credential_manager_acs_system_id is not None:
             json_payload["credential_manager_acs_system_id"] = (
                 credential_manager_acs_system_id
             )
-        if code is not None:
-            json_payload["code"] = code
+        if ends_at is not None:
+            json_payload["ends_at"] = ends_at
         if is_multi_phone_sync_credential is not None:
             json_payload["is_multi_phone_sync_credential"] = (
                 is_multi_phone_sync_credential
             )
-        if allowed_acs_entrance_ids is not None:
-            json_payload["allowed_acs_entrance_ids"] = allowed_acs_entrance_ids
-        if visionline_metadata is not None:
-            json_payload["visionline_metadata"] = visionline_metadata
         if starts_at is not None:
             json_payload["starts_at"] = starts_at
-        if ends_at is not None:
-            json_payload["ends_at"] = ends_at
+        if visionline_metadata is not None:
+            json_payload["visionline_metadata"] = visionline_metadata
 
         res = self.seam.make_request(
             "POST", "/acs/credentials/create", json=json_payload
         )
 
         return AcsCredential.from_dict(res["acs_credential"])
 
@@ -105,21 +105,21 @@
                 is_multi_phone_sync_credential
             )
 
         res = self.seam.make_request("POST", "/acs/credentials/list", json=json_payload)
 
         return [AcsCredential.from_dict(item) for item in res["acs_credentials"]]
 
-    def unassign(self, *, acs_user_id: str, acs_credential_id: str) -> None:
+    def unassign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         json_payload = {}
 
-        if acs_user_id is not None:
-            json_payload["acs_user_id"] = acs_user_id
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
+        if acs_user_id is not None:
+            json_payload["acs_user_id"] = acs_user_id
 
         self.seam.make_request("POST", "/acs/credentials/unassign", json=json_payload)
 
         return None
 
     def update(self, *, acs_credential_id: str, code: str) -> None:
         json_payload = {}
```

### Comparing `seam-0.3.0/seam/acs_entrances.py` & `seam-0.3.1/seam/acs_entrances.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,23 +34,23 @@
         self.seam.make_request("POST", "/acs/entrances/grant_access", json=json_payload)
 
         return None
 
     def list(
         self,
         *,
-        acs_system_id: Optional[str] = None,
-        acs_credential_id: Optional[str] = None
+        acs_credential_id: Optional[str] = None,
+        acs_system_id: Optional[str] = None
     ) -> List[AcsEntrance]:
         json_payload = {}
 
-        if acs_system_id is not None:
-            json_payload["acs_system_id"] = acs_system_id
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
+        if acs_system_id is not None:
+            json_payload["acs_system_id"] = acs_system_id
 
         res = self.seam.make_request("POST", "/acs/entrances/list", json=json_payload)
 
         return [AcsEntrance.from_dict(item) for item in res["acs_entrances"]]
 
     def list_credentials_with_access(
         self, *, acs_entrance_id: str, include_if: Optional[List[str]] = None
```

### Comparing `seam-0.3.0/seam/acs_systems.py` & `seam-0.3.1/seam/acs_systems.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/acs_users.py` & `seam-0.3.1/seam/acs_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,59 +5,59 @@
 class AcsUsers(AbstractAcsUsers):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def add_to_access_group(
-        self, *, acs_user_id: str, acs_access_group_id: str
+        self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
         json_payload = {}
 
-        if acs_user_id is not None:
-            json_payload["acs_user_id"] = acs_user_id
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
+        if acs_user_id is not None:
+            json_payload["acs_user_id"] = acs_user_id
 
         self.seam.make_request(
             "POST", "/acs/users/add_to_access_group", json=json_payload
         )
 
         return None
 
     def create(
         self,
         *,
         acs_system_id: str,
-        acs_access_group_ids: Optional[List[str]] = None,
-        user_identity_id: Optional[str] = None,
         access_schedule: Optional[Dict[str, Any]] = None,
-        full_name: Optional[str] = None,
+        acs_access_group_ids: Optional[List[str]] = None,
         email: Optional[str] = None,
+        email_address: Optional[str] = None,
+        full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        email_address: Optional[str] = None
+        user_identity_id: Optional[str] = None
     ) -> AcsUser:
         json_payload = {}
 
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
-        if acs_access_group_ids is not None:
-            json_payload["acs_access_group_ids"] = acs_access_group_ids
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if access_schedule is not None:
             json_payload["access_schedule"] = access_schedule
-        if full_name is not None:
-            json_payload["full_name"] = full_name
+        if acs_access_group_ids is not None:
+            json_payload["acs_access_group_ids"] = acs_access_group_ids
         if email is not None:
             json_payload["email"] = email
-        if phone_number is not None:
-            json_payload["phone_number"] = phone_number
         if email_address is not None:
             json_payload["email_address"] = email_address
+        if full_name is not None:
+            json_payload["full_name"] = full_name
+        if phone_number is not None:
+            json_payload["phone_number"] = phone_number
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
 
         res = self.seam.make_request("POST", "/acs/users/create", json=json_payload)
 
         return AcsUser.from_dict(res["acs_user"])
 
     def delete(self, *, acs_user_id: str) -> None:
         json_payload = {}
@@ -78,29 +78,29 @@
         res = self.seam.make_request("POST", "/acs/users/get", json=json_payload)
 
         return AcsUser.from_dict(res["acs_user"])
 
     def list(
         self,
         *,
-        user_identity_id: Optional[str] = None,
-        user_identity_phone_number: Optional[str] = None,
+        acs_system_id: Optional[str] = None,
         user_identity_email_address: Optional[str] = None,
-        acs_system_id: Optional[str] = None
+        user_identity_id: Optional[str] = None,
+        user_identity_phone_number: Optional[str] = None
     ) -> List[AcsUser]:
         json_payload = {}
 
+        if acs_system_id is not None:
+            json_payload["acs_system_id"] = acs_system_id
+        if user_identity_email_address is not None:
+            json_payload["user_identity_email_address"] = user_identity_email_address
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
         if user_identity_phone_number is not None:
             json_payload["user_identity_phone_number"] = user_identity_phone_number
-        if user_identity_email_address is not None:
-            json_payload["user_identity_email_address"] = user_identity_email_address
-        if acs_system_id is not None:
-            json_payload["acs_system_id"] = acs_system_id
 
         res = self.seam.make_request("POST", "/acs/users/list", json=json_payload)
 
         return [AcsUser.from_dict(item) for item in res["acs_users"]]
 
     def list_accessible_entrances(self, *, acs_user_id: str) -> List[AcsEntrance]:
         json_payload = {}
@@ -111,22 +111,22 @@
         res = self.seam.make_request(
             "POST", "/acs/users/list_accessible_entrances", json=json_payload
         )
 
         return [AcsEntrance.from_dict(item) for item in res["acs_entrances"]]
 
     def remove_from_access_group(
-        self, *, acs_user_id: str, acs_access_group_id: str
+        self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
         json_payload = {}
 
-        if acs_user_id is not None:
-            json_payload["acs_user_id"] = acs_user_id
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
+        if acs_user_id is not None:
+            json_payload["acs_user_id"] = acs_user_id
 
         self.seam.make_request(
             "POST", "/acs/users/remove_from_access_group", json=json_payload
         )
 
         return None
 
@@ -163,33 +163,33 @@
         return None
 
     def update(
         self,
         *,
         acs_user_id: str,
         access_schedule: Optional[Dict[str, Any]] = None,
-        full_name: Optional[str] = None,
         email: Optional[str] = None,
-        phone_number: Optional[str] = None,
         email_address: Optional[str] = None,
-        hid_acs_system_id: Optional[str] = None
+        full_name: Optional[str] = None,
+        hid_acs_system_id: Optional[str] = None,
+        phone_number: Optional[str] = None
     ) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
         if access_schedule is not None:
             json_payload["access_schedule"] = access_schedule
-        if full_name is not None:
-            json_payload["full_name"] = full_name
         if email is not None:
             json_payload["email"] = email
-        if phone_number is not None:
-            json_payload["phone_number"] = phone_number
         if email_address is not None:
             json_payload["email_address"] = email_address
+        if full_name is not None:
+            json_payload["full_name"] = full_name
         if hid_acs_system_id is not None:
             json_payload["hid_acs_system_id"] = hid_acs_system_id
+        if phone_number is not None:
+            json_payload["phone_number"] = phone_number
 
         self.seam.make_request("POST", "/acs/users/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/action_attempts.py` & `seam-0.3.1/seam/action_attempts.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/client_sessions.py` & `seam-0.3.1/seam/client_sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create(
         self,
         *,
-        user_identifier_key: Optional[str] = None,
         connect_webview_ids: Optional[List[str]] = None,
         connected_account_ids: Optional[List[str]] = None,
-        user_identity_ids: Optional[List[str]] = None,
-        expires_at: Optional[str] = None
+        expires_at: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_ids: Optional[List[str]] = None
     ) -> ClientSession:
         json_payload = {}
 
-        if user_identifier_key is not None:
-            json_payload["user_identifier_key"] = user_identifier_key
         if connect_webview_ids is not None:
             json_payload["connect_webview_ids"] = connect_webview_ids
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if user_identity_ids is not None:
-            json_payload["user_identity_ids"] = user_identity_ids
         if expires_at is not None:
             json_payload["expires_at"] = expires_at
+        if user_identifier_key is not None:
+            json_payload["user_identifier_key"] = user_identifier_key
+        if user_identity_ids is not None:
+            json_payload["user_identity_ids"] = user_identity_ids
 
         res = self.seam.make_request(
             "POST", "/client_sessions/create", json=json_payload
         )
 
         return ClientSession.from_dict(res["client_session"])
 
@@ -62,88 +62,88 @@
         res = self.seam.make_request("POST", "/client_sessions/get", json=json_payload)
 
         return ClientSession.from_dict(res["client_session"])
 
     def get_or_create(
         self,
         *,
-        user_identifier_key: Optional[str] = None,
         connect_webview_ids: Optional[List[str]] = None,
         connected_account_ids: Optional[List[str]] = None,
-        user_identity_ids: Optional[List[str]] = None,
-        expires_at: Optional[str] = None
+        expires_at: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_ids: Optional[List[str]] = None
     ) -> ClientSession:
         json_payload = {}
 
-        if user_identifier_key is not None:
-            json_payload["user_identifier_key"] = user_identifier_key
         if connect_webview_ids is not None:
             json_payload["connect_webview_ids"] = connect_webview_ids
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if user_identity_ids is not None:
-            json_payload["user_identity_ids"] = user_identity_ids
         if expires_at is not None:
             json_payload["expires_at"] = expires_at
+        if user_identifier_key is not None:
+            json_payload["user_identifier_key"] = user_identifier_key
+        if user_identity_ids is not None:
+            json_payload["user_identity_ids"] = user_identity_ids
 
         res = self.seam.make_request(
             "POST", "/client_sessions/get_or_create", json=json_payload
         )
 
         return ClientSession.from_dict(res["client_session"])
 
     def grant_access(
         self,
         *,
         client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
-        connected_account_ids: Optional[List[str]] = None,
         connect_webview_ids: Optional[List[str]] = None,
+        connected_account_ids: Optional[List[str]] = None,
+        user_identifier_key: Optional[str] = None,
         user_identity_ids: Optional[List[str]] = None
     ) -> None:
         json_payload = {}
 
         if client_session_id is not None:
             json_payload["client_session_id"] = client_session_id
-        if user_identifier_key is not None:
-            json_payload["user_identifier_key"] = user_identifier_key
-        if connected_account_ids is not None:
-            json_payload["connected_account_ids"] = connected_account_ids
         if connect_webview_ids is not None:
             json_payload["connect_webview_ids"] = connect_webview_ids
+        if connected_account_ids is not None:
+            json_payload["connected_account_ids"] = connected_account_ids
+        if user_identifier_key is not None:
+            json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_ids is not None:
             json_payload["user_identity_ids"] = user_identity_ids
 
         self.seam.make_request(
             "POST", "/client_sessions/grant_access", json=json_payload
         )
 
         return None
 
     def list(
         self,
         *,
         client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         connect_webview_id: Optional[str] = None,
-        without_user_identifier_key: Optional[bool] = None,
-        user_identity_id: Optional[str] = None
+        user_identifier_key: Optional[str] = None,
+        user_identity_id: Optional[str] = None,
+        without_user_identifier_key: Optional[bool] = None
     ) -> List[ClientSession]:
         json_payload = {}
 
         if client_session_id is not None:
             json_payload["client_session_id"] = client_session_id
-        if user_identifier_key is not None:
-            json_payload["user_identifier_key"] = user_identifier_key
         if connect_webview_id is not None:
             json_payload["connect_webview_id"] = connect_webview_id
-        if without_user_identifier_key is not None:
-            json_payload["without_user_identifier_key"] = without_user_identifier_key
+        if user_identifier_key is not None:
+            json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
+        if without_user_identifier_key is not None:
+            json_payload["without_user_identifier_key"] = without_user_identifier_key
 
         res = self.seam.make_request("POST", "/client_sessions/list", json=json_payload)
 
         return [ClientSession.from_dict(item) for item in res["client_sessions"]]
 
     def revoke(self, *, client_session_id: str) -> None:
         json_payload = {}
```

### Comparing `seam-0.3.0/seam/connect_webviews.py` & `seam-0.3.1/seam/connect_webviews.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create(
         self,
         *,
-        device_selection_mode: Optional[str] = None,
-        custom_redirect_url: Optional[str] = None,
-        custom_redirect_failure_url: Optional[str] = None,
         accepted_providers: Optional[List[str]] = None,
-        provider_category: Optional[str] = None,
-        custom_metadata: Optional[Dict[str, Any]] = None,
         automatically_manage_new_devices: Optional[bool] = None,
+        custom_metadata: Optional[Dict[str, Any]] = None,
+        custom_redirect_failure_url: Optional[str] = None,
+        custom_redirect_url: Optional[str] = None,
+        device_selection_mode: Optional[str] = None,
+        provider_category: Optional[str] = None,
         wait_for_device_creation: Optional[bool] = None
     ) -> ConnectWebview:
         json_payload = {}
 
-        if device_selection_mode is not None:
-            json_payload["device_selection_mode"] = device_selection_mode
-        if custom_redirect_url is not None:
-            json_payload["custom_redirect_url"] = custom_redirect_url
-        if custom_redirect_failure_url is not None:
-            json_payload["custom_redirect_failure_url"] = custom_redirect_failure_url
         if accepted_providers is not None:
             json_payload["accepted_providers"] = accepted_providers
-        if provider_category is not None:
-            json_payload["provider_category"] = provider_category
-        if custom_metadata is not None:
-            json_payload["custom_metadata"] = custom_metadata
         if automatically_manage_new_devices is not None:
             json_payload["automatically_manage_new_devices"] = (
                 automatically_manage_new_devices
             )
+        if custom_metadata is not None:
+            json_payload["custom_metadata"] = custom_metadata
+        if custom_redirect_failure_url is not None:
+            json_payload["custom_redirect_failure_url"] = custom_redirect_failure_url
+        if custom_redirect_url is not None:
+            json_payload["custom_redirect_url"] = custom_redirect_url
+        if device_selection_mode is not None:
+            json_payload["device_selection_mode"] = device_selection_mode
+        if provider_category is not None:
+            json_payload["provider_category"] = provider_category
         if wait_for_device_creation is not None:
             json_payload["wait_for_device_creation"] = wait_for_device_creation
 
         res = self.seam.make_request(
             "POST", "/connect_webviews/create", json=json_payload
         )
 
@@ -66,22 +66,22 @@
         res = self.seam.make_request("POST", "/connect_webviews/get", json=json_payload)
 
         return ConnectWebview.from_dict(res["connect_webview"])
 
     def list(
         self,
         *,
-        user_identifier_key: Optional[str] = None,
-        custom_metadata_has: Optional[Dict[str, Any]] = None
+        custom_metadata_has: Optional[Dict[str, Any]] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[ConnectWebview]:
         json_payload = {}
 
-        if user_identifier_key is not None:
-            json_payload["user_identifier_key"] = user_identifier_key
         if custom_metadata_has is not None:
             json_payload["custom_metadata_has"] = custom_metadata_has
+        if user_identifier_key is not None:
+            json_payload["user_identifier_key"] = user_identifier_key
 
         res = self.seam.make_request(
             "POST", "/connect_webviews/list", json=json_payload
         )
 
         return [ConnectWebview.from_dict(item) for item in res["connect_webviews"]]
```

### Comparing `seam-0.3.0/seam/connected_accounts.py` & `seam-0.3.1/seam/connected_accounts.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/devices.py` & `seam-0.3.1/seam/devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,56 +43,56 @@
         res = self.seam.make_request("POST", "/devices/get", json=json_payload)
 
         return Device.from_dict(res["device"])
 
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
-        device_type: Optional[str] = None,
-        device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
-        limit: Optional[float] = None,
         created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
+        device_type: Optional[str] = None,
+        device_types: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None
+        limit: Optional[float] = None,
+        manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         json_payload = {}
 
+        if connect_webview_id is not None:
+            json_payload["connect_webview_id"] = connect_webview_id
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if connect_webview_id is not None:
-            json_payload["connect_webview_id"] = connect_webview_id
+        if created_before is not None:
+            json_payload["created_before"] = created_before
+        if custom_metadata_has is not None:
+            json_payload["custom_metadata_has"] = custom_metadata_has
+        if device_ids is not None:
+            json_payload["device_ids"] = device_ids
         if device_type is not None:
             json_payload["device_type"] = device_type
         if device_types is not None:
             json_payload["device_types"] = device_types
-        if manufacturer is not None:
-            json_payload["manufacturer"] = manufacturer
-        if device_ids is not None:
-            json_payload["device_ids"] = device_ids
+        if exclude_if is not None:
+            json_payload["exclude_if"] = exclude_if
+        if include_if is not None:
+            json_payload["include_if"] = include_if
         if limit is not None:
             json_payload["limit"] = limit
-        if created_before is not None:
-            json_payload["created_before"] = created_before
+        if manufacturer is not None:
+            json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
-        if custom_metadata_has is not None:
-            json_payload["custom_metadata_has"] = custom_metadata_has
-        if include_if is not None:
-            json_payload["include_if"] = include_if
-        if exclude_if is not None:
-            json_payload["exclude_if"] = exclude_if
 
         res = self.seam.make_request("POST", "/devices/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["devices"]]
 
     def list_device_providers(
         self, *, provider_category: Optional[str] = None
@@ -108,28 +108,28 @@
 
         return [DeviceProvider.from_dict(item) for item in res["device_providers"]]
 
     def update(
         self,
         *,
         device_id: str,
-        properties: Optional[Dict[str, Any]] = None,
-        name: Optional[str] = None,
+        custom_metadata: Optional[Dict[str, Any]] = None,
         is_managed: Optional[bool] = None,
-        custom_metadata: Optional[Dict[str, Any]] = None
+        name: Optional[str] = None,
+        properties: Optional[Dict[str, Any]] = None
     ) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if properties is not None:
-            json_payload["properties"] = properties
-        if name is not None:
-            json_payload["name"] = name
-        if is_managed is not None:
-            json_payload["is_managed"] = is_managed
         if custom_metadata is not None:
             json_payload["custom_metadata"] = custom_metadata
+        if is_managed is not None:
+            json_payload["is_managed"] = is_managed
+        if name is not None:
+            json_payload["name"] = name
+        if properties is not None:
+            json_payload["properties"] = properties
 
         self.seam.make_request("POST", "/devices/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/devices_simulate.py` & `seam-0.3.1/seam/devices_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/devices_unmanaged.py` & `seam-0.3.1/seam/devices_unmanaged.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,56 +23,56 @@
         )
 
         return UnmanagedDevice.from_dict(res["device"])
 
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
-        device_type: Optional[str] = None,
-        device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
-        limit: Optional[float] = None,
         created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
+        device_type: Optional[str] = None,
+        device_types: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None
+        limit: Optional[float] = None,
+        manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[UnmanagedDevice]:
         json_payload = {}
 
+        if connect_webview_id is not None:
+            json_payload["connect_webview_id"] = connect_webview_id
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if connect_webview_id is not None:
-            json_payload["connect_webview_id"] = connect_webview_id
+        if created_before is not None:
+            json_payload["created_before"] = created_before
+        if custom_metadata_has is not None:
+            json_payload["custom_metadata_has"] = custom_metadata_has
+        if device_ids is not None:
+            json_payload["device_ids"] = device_ids
         if device_type is not None:
             json_payload["device_type"] = device_type
         if device_types is not None:
             json_payload["device_types"] = device_types
-        if manufacturer is not None:
-            json_payload["manufacturer"] = manufacturer
-        if device_ids is not None:
-            json_payload["device_ids"] = device_ids
+        if exclude_if is not None:
+            json_payload["exclude_if"] = exclude_if
+        if include_if is not None:
+            json_payload["include_if"] = include_if
         if limit is not None:
             json_payload["limit"] = limit
-        if created_before is not None:
-            json_payload["created_before"] = created_before
+        if manufacturer is not None:
+            json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
-        if custom_metadata_has is not None:
-            json_payload["custom_metadata_has"] = custom_metadata_has
-        if include_if is not None:
-            json_payload["include_if"] = include_if
-        if exclude_if is not None:
-            json_payload["exclude_if"] = exclude_if
 
         res = self.seam.make_request(
             "POST", "/devices/unmanaged/list", json=json_payload
         )
 
         return [UnmanagedDevice.from_dict(item) for item in res["devices"]]
```

### Comparing `seam-0.3.0/seam/events.py` & `seam-0.3.1/seam/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,64 +7,64 @@
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def get(
         self,
         *,
+        device_id: Optional[str] = None,
         event_id: Optional[str] = None,
-        event_type: Optional[str] = None,
-        device_id: Optional[str] = None
+        event_type: Optional[str] = None
     ) -> Event:
         json_payload = {}
 
+        if device_id is not None:
+            json_payload["device_id"] = device_id
         if event_id is not None:
             json_payload["event_id"] = event_id
         if event_type is not None:
             json_payload["event_type"] = event_type
-        if device_id is not None:
-            json_payload["device_id"] = device_id
 
         res = self.seam.make_request("POST", "/events/get", json=json_payload)
 
         return Event.from_dict(res["event"])
 
     def list(
         self,
         *,
-        since: Optional[str] = None,
+        access_code_id: Optional[str] = None,
+        access_code_ids: Optional[List[str]] = None,
         between: Optional[List[str]] = None,
+        connected_account_id: Optional[str] = None,
         device_id: Optional[str] = None,
         device_ids: Optional[List[str]] = None,
-        access_code_id: Optional[str] = None,
-        access_code_ids: Optional[List[str]] = None,
         event_type: Optional[str] = None,
         event_types: Optional[List[str]] = None,
-        connected_account_id: Optional[str] = None,
-        limit: Optional[float] = None
+        limit: Optional[float] = None,
+        since: Optional[str] = None
     ) -> List[Event]:
         json_payload = {}
 
-        if since is not None:
-            json_payload["since"] = since
+        if access_code_id is not None:
+            json_payload["access_code_id"] = access_code_id
+        if access_code_ids is not None:
+            json_payload["access_code_ids"] = access_code_ids
         if between is not None:
             json_payload["between"] = between
+        if connected_account_id is not None:
+            json_payload["connected_account_id"] = connected_account_id
         if device_id is not None:
             json_payload["device_id"] = device_id
         if device_ids is not None:
             json_payload["device_ids"] = device_ids
-        if access_code_id is not None:
-            json_payload["access_code_id"] = access_code_id
-        if access_code_ids is not None:
-            json_payload["access_code_ids"] = access_code_ids
         if event_type is not None:
             json_payload["event_type"] = event_type
         if event_types is not None:
             json_payload["event_types"] = event_types
-        if connected_account_id is not None:
-            json_payload["connected_account_id"] = connected_account_id
         if limit is not None:
             json_payload["limit"] = limit
+        if since is not None:
+            json_payload["since"] = since
 
         res = self.seam.make_request("POST", "/events/list", json=json_payload)
 
         return [Event.from_dict(item) for item in res["events"]]
```

### Comparing `seam-0.3.0/seam/locks.py` & `seam-0.3.1/seam/locks.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,56 +21,56 @@
         res = self.seam.make_request("POST", "/locks/get", json=json_payload)
 
         return Device.from_dict(res["device"])
 
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
-        device_type: Optional[str] = None,
-        device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
-        limit: Optional[float] = None,
         created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
+        device_type: Optional[str] = None,
+        device_types: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None
+        limit: Optional[float] = None,
+        manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         json_payload = {}
 
+        if connect_webview_id is not None:
+            json_payload["connect_webview_id"] = connect_webview_id
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if connect_webview_id is not None:
-            json_payload["connect_webview_id"] = connect_webview_id
+        if created_before is not None:
+            json_payload["created_before"] = created_before
+        if custom_metadata_has is not None:
+            json_payload["custom_metadata_has"] = custom_metadata_has
+        if device_ids is not None:
+            json_payload["device_ids"] = device_ids
         if device_type is not None:
             json_payload["device_type"] = device_type
         if device_types is not None:
             json_payload["device_types"] = device_types
-        if manufacturer is not None:
-            json_payload["manufacturer"] = manufacturer
-        if device_ids is not None:
-            json_payload["device_ids"] = device_ids
+        if exclude_if is not None:
+            json_payload["exclude_if"] = exclude_if
+        if include_if is not None:
+            json_payload["include_if"] = include_if
         if limit is not None:
             json_payload["limit"] = limit
-        if created_before is not None:
-            json_payload["created_before"] = created_before
+        if manufacturer is not None:
+            json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
-        if custom_metadata_has is not None:
-            json_payload["custom_metadata_has"] = custom_metadata_has
-        if include_if is not None:
-            json_payload["include_if"] = include_if
-        if exclude_if is not None:
-            json_payload["exclude_if"] = exclude_if
 
         res = self.seam.make_request("POST", "/locks/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["devices"]]
 
     def lock_door(
         self,
```

### Comparing `seam-0.3.0/seam/networks.py` & `seam-0.3.1/seam/networks.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/noise_sensors.py` & `seam-0.3.1/seam/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/noise_sensors_noise_thresholds.py` & `seam-0.3.1/seam/noise_sensors_noise_thresholds.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,53 +12,53 @@
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create(
         self,
         *,
         device_id: str,
-        starts_daily_at: str,
         ends_daily_at: str,
-        sync: Optional[bool] = None,
+        starts_daily_at: str,
         name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
-        noise_threshold_nrs: Optional[float] = None
+        noise_threshold_nrs: Optional[float] = None,
+        sync: Optional[bool] = None
     ) -> NoiseThreshold:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if starts_daily_at is not None:
-            json_payload["starts_daily_at"] = starts_daily_at
         if ends_daily_at is not None:
             json_payload["ends_daily_at"] = ends_daily_at
-        if sync is not None:
-            json_payload["sync"] = sync
+        if starts_daily_at is not None:
+            json_payload["starts_daily_at"] = starts_daily_at
         if name is not None:
             json_payload["name"] = name
         if noise_threshold_decibels is not None:
             json_payload["noise_threshold_decibels"] = noise_threshold_decibels
         if noise_threshold_nrs is not None:
             json_payload["noise_threshold_nrs"] = noise_threshold_nrs
+        if sync is not None:
+            json_payload["sync"] = sync
 
         res = self.seam.make_request(
             "POST", "/noise_sensors/noise_thresholds/create", json=json_payload
         )
 
         return NoiseThreshold.from_dict(res["noise_threshold"])
 
     def delete(
-        self, *, noise_threshold_id: str, device_id: str, sync: Optional[bool] = None
+        self, *, device_id: str, noise_threshold_id: str, sync: Optional[bool] = None
     ) -> None:
         json_payload = {}
 
-        if noise_threshold_id is not None:
-            json_payload["noise_threshold_id"] = noise_threshold_id
         if device_id is not None:
             json_payload["device_id"] = device_id
+        if noise_threshold_id is not None:
+            json_payload["noise_threshold_id"] = noise_threshold_id
         if sync is not None:
             json_payload["sync"] = sync
 
         self.seam.make_request(
             "POST", "/noise_sensors/noise_thresholds/delete", json=json_payload
         )
 
@@ -91,40 +91,40 @@
         )
 
         return [NoiseThreshold.from_dict(item) for item in res["noise_thresholds"]]
 
     def update(
         self,
         *,
-        noise_threshold_id: str,
         device_id: str,
-        sync: Optional[bool] = None,
-        name: Optional[str] = None,
-        starts_daily_at: Optional[str] = None,
+        noise_threshold_id: str,
         ends_daily_at: Optional[str] = None,
+        name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
-        noise_threshold_nrs: Optional[float] = None
+        noise_threshold_nrs: Optional[float] = None,
+        starts_daily_at: Optional[str] = None,
+        sync: Optional[bool] = None
     ) -> None:
         json_payload = {}
 
-        if noise_threshold_id is not None:
-            json_payload["noise_threshold_id"] = noise_threshold_id
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if sync is not None:
-            json_payload["sync"] = sync
-        if name is not None:
-            json_payload["name"] = name
-        if starts_daily_at is not None:
-            json_payload["starts_daily_at"] = starts_daily_at
+        if noise_threshold_id is not None:
+            json_payload["noise_threshold_id"] = noise_threshold_id
         if ends_daily_at is not None:
             json_payload["ends_daily_at"] = ends_daily_at
+        if name is not None:
+            json_payload["name"] = name
         if noise_threshold_decibels is not None:
             json_payload["noise_threshold_decibels"] = noise_threshold_decibels
         if noise_threshold_nrs is not None:
             json_payload["noise_threshold_nrs"] = noise_threshold_nrs
+        if starts_daily_at is not None:
+            json_payload["starts_daily_at"] = starts_daily_at
+        if sync is not None:
+            json_payload["sync"] = sync
 
         self.seam.make_request(
             "POST", "/noise_sensors/noise_thresholds/update", json=json_payload
         )
 
         return None
```

### Comparing `seam-0.3.0/seam/noise_sensors_simulate.py` & `seam-0.3.1/seam/noise_sensors_simulate.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/phones.py` & `seam-0.3.1/seam/phones.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/phones_simulate.py` & `seam-0.3.1/seam/phones_simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,27 +8,27 @@
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create_sandbox_phone(
         self,
         *,
         user_identity_id: str,
+        assa_abloy_metadata: Optional[Dict[str, Any]] = None,
         custom_sdk_installation_id: Optional[str] = None,
-        phone_metadata: Optional[Dict[str, Any]] = None,
-        assa_abloy_metadata: Optional[Dict[str, Any]] = None
+        phone_metadata: Optional[Dict[str, Any]] = None
     ) -> Phone:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
+        if assa_abloy_metadata is not None:
+            json_payload["assa_abloy_metadata"] = assa_abloy_metadata
         if custom_sdk_installation_id is not None:
             json_payload["custom_sdk_installation_id"] = custom_sdk_installation_id
         if phone_metadata is not None:
             json_payload["phone_metadata"] = phone_metadata
-        if assa_abloy_metadata is not None:
-            json_payload["assa_abloy_metadata"] = assa_abloy_metadata
 
         res = self.seam.make_request(
             "POST", "/phones/simulate/create_sandbox_phone", json=json_payload
         )
 
         return Phone.from_dict(res["phone"])
```

### Comparing `seam-0.3.0/seam/routes.py` & `seam-0.3.1/seam/routes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from .types import AbstractRoutes
 from .access_codes import AccessCodes
+from .acs import Acs
 from .action_attempts import ActionAttempts
 from .client_sessions import ClientSessions
 from .connect_webviews import ConnectWebviews
 from .connected_accounts import ConnectedAccounts
 from .devices import Devices
 from .events import Events
 from .locks import Locks
 from .networks import Networks
+from .noise_sensors import NoiseSensors
 from .phones import Phones
 from .thermostats import Thermostats
 from .user_identities import UserIdentities
 from .webhooks import Webhooks
 from .workspaces import Workspaces
-from .acs import Acs
-from .noise_sensors import NoiseSensors
 
 
 class Routes(AbstractRoutes):
     def __init__(self):
         self.access_codes = AccessCodes(seam=self)
+        self.acs = Acs(seam=self)
         self.action_attempts = ActionAttempts(seam=self)
         self.client_sessions = ClientSessions(seam=self)
         self.connect_webviews = ConnectWebviews(seam=self)
         self.connected_accounts = ConnectedAccounts(seam=self)
         self.devices = Devices(seam=self)
         self.events = Events(seam=self)
         self.locks = Locks(seam=self)
         self.networks = Networks(seam=self)
+        self.noise_sensors = NoiseSensors(seam=self)
         self.phones = Phones(seam=self)
         self.thermostats = Thermostats(seam=self)
         self.user_identities = UserIdentities(seam=self)
         self.webhooks = Webhooks(seam=self)
         self.workspaces = Workspaces(seam=self)
-        self.acs = Acs(seam=self)
-        self.noise_sensors = NoiseSensors(seam=self)
 
     def make_request(self, method: str, path: str, **kwargs):
         raise NotImplementedError()
```

### Comparing `seam-0.3.0/seam/seam.py` & `seam-0.3.1/seam/seam.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/thermostats.py` & `seam-0.3.1/seam/thermostats.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,33 +84,33 @@
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def heat_cool(
         self,
         *,
         device_id: str,
-        heating_set_point_celsius: Optional[float] = None,
-        heating_set_point_fahrenheit: Optional[float] = None,
         cooling_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
+        heating_set_point_fahrenheit: Optional[float] = None,
         sync: Optional[bool] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if heating_set_point_celsius is not None:
-            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
-        if heating_set_point_fahrenheit is not None:
-            json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
         if cooling_set_point_celsius is not None:
             json_payload["cooling_set_point_celsius"] = cooling_set_point_celsius
         if cooling_set_point_fahrenheit is not None:
             json_payload["cooling_set_point_fahrenheit"] = cooling_set_point_fahrenheit
+        if heating_set_point_celsius is not None:
+            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
+        if heating_set_point_fahrenheit is not None:
+            json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
         if sync is not None:
             json_payload["sync"] = sync
 
         res = self.seam.make_request(
             "POST", "/thermostats/heat_cool", json=json_payload
         )
 
@@ -118,56 +118,56 @@
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
-        device_type: Optional[str] = None,
-        device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
-        limit: Optional[float] = None,
         created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
+        device_type: Optional[str] = None,
+        device_types: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
         include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None
+        limit: Optional[float] = None,
+        manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None
     ) -> List[Device]:
         json_payload = {}
 
+        if connect_webview_id is not None:
+            json_payload["connect_webview_id"] = connect_webview_id
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
-        if connect_webview_id is not None:
-            json_payload["connect_webview_id"] = connect_webview_id
+        if created_before is not None:
+            json_payload["created_before"] = created_before
+        if custom_metadata_has is not None:
+            json_payload["custom_metadata_has"] = custom_metadata_has
+        if device_ids is not None:
+            json_payload["device_ids"] = device_ids
         if device_type is not None:
             json_payload["device_type"] = device_type
         if device_types is not None:
             json_payload["device_types"] = device_types
-        if manufacturer is not None:
-            json_payload["manufacturer"] = manufacturer
-        if device_ids is not None:
-            json_payload["device_ids"] = device_ids
+        if exclude_if is not None:
+            json_payload["exclude_if"] = exclude_if
+        if include_if is not None:
+            json_payload["include_if"] = include_if
         if limit is not None:
             json_payload["limit"] = limit
-        if created_before is not None:
-            json_payload["created_before"] = created_before
+        if manufacturer is not None:
+            json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
-        if custom_metadata_has is not None:
-            json_payload["custom_metadata_has"] = custom_metadata_has
-        if include_if is not None:
-            json_payload["include_if"] = include_if
-        if exclude_if is not None:
-            json_payload["exclude_if"] = exclude_if
 
         res = self.seam.make_request("POST", "/thermostats/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["thermostats"]]
 
     def off(
         self,
@@ -216,19 +216,19 @@
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def update(
-        self, *, device_id: str, default_climate_setting: Dict[str, Any]
+        self, *, default_climate_setting: Dict[str, Any], device_id: str
     ) -> None:
         json_payload = {}
 
-        if device_id is not None:
-            json_payload["device_id"] = device_id
         if default_climate_setting is not None:
             json_payload["default_climate_setting"] = default_climate_setting
+        if device_id is not None:
+            json_payload["device_id"] = device_id
 
         self.seam.make_request("POST", "/thermostats/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/thermostats_climate_setting_schedules.py` & `seam-0.3.1/seam/thermostats_climate_setting_schedules.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,55 +12,55 @@
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create(
         self,
         *,
         device_id: str,
-        schedule_starts_at: str,
         schedule_ends_at: str,
-        schedule_type: Optional[str] = None,
-        name: Optional[str] = None,
-        automatic_heating_enabled: Optional[bool] = None,
+        schedule_starts_at: str,
         automatic_cooling_enabled: Optional[bool] = None,
-        hvac_mode_setting: Optional[str] = None,
+        automatic_heating_enabled: Optional[bool] = None,
         cooling_set_point_celsius: Optional[float] = None,
-        heating_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
-        manual_override_allowed: Optional[bool] = None
+        hvac_mode_setting: Optional[str] = None,
+        manual_override_allowed: Optional[bool] = None,
+        name: Optional[str] = None,
+        schedule_type: Optional[str] = None
     ) -> ClimateSettingSchedule:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
-        if schedule_starts_at is not None:
-            json_payload["schedule_starts_at"] = schedule_starts_at
         if schedule_ends_at is not None:
             json_payload["schedule_ends_at"] = schedule_ends_at
-        if schedule_type is not None:
-            json_payload["schedule_type"] = schedule_type
-        if name is not None:
-            json_payload["name"] = name
-        if automatic_heating_enabled is not None:
-            json_payload["automatic_heating_enabled"] = automatic_heating_enabled
+        if schedule_starts_at is not None:
+            json_payload["schedule_starts_at"] = schedule_starts_at
         if automatic_cooling_enabled is not None:
             json_payload["automatic_cooling_enabled"] = automatic_cooling_enabled
-        if hvac_mode_setting is not None:
-            json_payload["hvac_mode_setting"] = hvac_mode_setting
+        if automatic_heating_enabled is not None:
+            json_payload["automatic_heating_enabled"] = automatic_heating_enabled
         if cooling_set_point_celsius is not None:
             json_payload["cooling_set_point_celsius"] = cooling_set_point_celsius
-        if heating_set_point_celsius is not None:
-            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if cooling_set_point_fahrenheit is not None:
             json_payload["cooling_set_point_fahrenheit"] = cooling_set_point_fahrenheit
+        if heating_set_point_celsius is not None:
+            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if heating_set_point_fahrenheit is not None:
             json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
+        if hvac_mode_setting is not None:
+            json_payload["hvac_mode_setting"] = hvac_mode_setting
         if manual_override_allowed is not None:
             json_payload["manual_override_allowed"] = manual_override_allowed
+        if name is not None:
+            json_payload["name"] = name
+        if schedule_type is not None:
+            json_payload["schedule_type"] = schedule_type
 
         res = self.seam.make_request(
             "POST", "/thermostats/climate_setting_schedules/create", json=json_payload
         )
 
         return ClimateSettingSchedule.from_dict(res["climate_setting_schedule"])
 
@@ -114,54 +114,54 @@
             for item in res["climate_setting_schedules"]
         ]
 
     def update(
         self,
         *,
         climate_setting_schedule_id: str,
-        schedule_type: Optional[str] = None,
-        name: Optional[str] = None,
-        schedule_starts_at: Optional[str] = None,
-        schedule_ends_at: Optional[str] = None,
-        automatic_heating_enabled: Optional[bool] = None,
         automatic_cooling_enabled: Optional[bool] = None,
-        hvac_mode_setting: Optional[str] = None,
+        automatic_heating_enabled: Optional[bool] = None,
         cooling_set_point_celsius: Optional[float] = None,
-        heating_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
-        manual_override_allowed: Optional[bool] = None
+        hvac_mode_setting: Optional[str] = None,
+        manual_override_allowed: Optional[bool] = None,
+        name: Optional[str] = None,
+        schedule_ends_at: Optional[str] = None,
+        schedule_starts_at: Optional[str] = None,
+        schedule_type: Optional[str] = None
     ) -> None:
         json_payload = {}
 
         if climate_setting_schedule_id is not None:
             json_payload["climate_setting_schedule_id"] = climate_setting_schedule_id
-        if schedule_type is not None:
-            json_payload["schedule_type"] = schedule_type
-        if name is not None:
-            json_payload["name"] = name
-        if schedule_starts_at is not None:
-            json_payload["schedule_starts_at"] = schedule_starts_at
-        if schedule_ends_at is not None:
-            json_payload["schedule_ends_at"] = schedule_ends_at
-        if automatic_heating_enabled is not None:
-            json_payload["automatic_heating_enabled"] = automatic_heating_enabled
         if automatic_cooling_enabled is not None:
             json_payload["automatic_cooling_enabled"] = automatic_cooling_enabled
-        if hvac_mode_setting is not None:
-            json_payload["hvac_mode_setting"] = hvac_mode_setting
+        if automatic_heating_enabled is not None:
+            json_payload["automatic_heating_enabled"] = automatic_heating_enabled
         if cooling_set_point_celsius is not None:
             json_payload["cooling_set_point_celsius"] = cooling_set_point_celsius
-        if heating_set_point_celsius is not None:
-            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if cooling_set_point_fahrenheit is not None:
             json_payload["cooling_set_point_fahrenheit"] = cooling_set_point_fahrenheit
+        if heating_set_point_celsius is not None:
+            json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if heating_set_point_fahrenheit is not None:
             json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
+        if hvac_mode_setting is not None:
+            json_payload["hvac_mode_setting"] = hvac_mode_setting
         if manual_override_allowed is not None:
             json_payload["manual_override_allowed"] = manual_override_allowed
+        if name is not None:
+            json_payload["name"] = name
+        if schedule_ends_at is not None:
+            json_payload["schedule_ends_at"] = schedule_ends_at
+        if schedule_starts_at is not None:
+            json_payload["schedule_starts_at"] = schedule_starts_at
+        if schedule_type is not None:
+            json_payload["schedule_type"] = schedule_type
 
         self.seam.make_request(
             "POST", "/thermostats/climate_setting_schedules/update", json=json_payload
         )
 
         return None
```

### Comparing `seam-0.3.0/seam/types.py` & `seam-0.3.1/seam/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,358 +2,503 @@
 import abc
 from dataclasses import dataclass
 from seam.utils.deep_attr_dict import DeepAttrDict
 
 
 @dataclass
 class AccessCode:
-    common_code_key: str
-    is_scheduled_on_device: bool
-    type: str
-    is_waiting_for_code_assignment: bool
     access_code_id: str
-    device_id: str
-    name: str
     code: str
+    common_code_key: str
     created_at: str
-    errors: Any
-    warnings: Any
-    is_managed: bool
-    starts_at: str
+    device_id: str
     ends_at: str
-    status: str
-    is_backup_access_code_available: bool
+    errors: Any
     is_backup: bool
-    pulled_backup_access_code_id: str
+    is_backup_access_code_available: bool
     is_external_modification_allowed: bool
-    is_one_time_use: bool
+    is_managed: bool
     is_offline_access_code: bool
+    is_one_time_use: bool
+    is_scheduled_on_device: bool
+    is_waiting_for_code_assignment: bool
+    name: str
+    pulled_backup_access_code_id: str
+    starts_at: str
+    status: str
+    type: str
+    warnings: Any
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return AccessCode(
-            common_code_key=d.get("common_code_key", None),
-            is_scheduled_on_device=d.get("is_scheduled_on_device", None),
-            type=d.get("type", None),
-            is_waiting_for_code_assignment=d.get(
-                "is_waiting_for_code_assignment", None
-            ),
             access_code_id=d.get("access_code_id", None),
-            device_id=d.get("device_id", None),
-            name=d.get("name", None),
             code=d.get("code", None),
+            common_code_key=d.get("common_code_key", None),
             created_at=d.get("created_at", None),
-            errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            is_managed=d.get("is_managed", None),
-            starts_at=d.get("starts_at", None),
+            device_id=d.get("device_id", None),
             ends_at=d.get("ends_at", None),
-            status=d.get("status", None),
+            errors=d.get("errors", None),
+            is_backup=d.get("is_backup", None),
             is_backup_access_code_available=d.get(
                 "is_backup_access_code_available", None
             ),
-            is_backup=d.get("is_backup", None),
-            pulled_backup_access_code_id=d.get("pulled_backup_access_code_id", None),
             is_external_modification_allowed=d.get(
                 "is_external_modification_allowed", None
             ),
-            is_one_time_use=d.get("is_one_time_use", None),
+            is_managed=d.get("is_managed", None),
             is_offline_access_code=d.get("is_offline_access_code", None),
+            is_one_time_use=d.get("is_one_time_use", None),
+            is_scheduled_on_device=d.get("is_scheduled_on_device", None),
+            is_waiting_for_code_assignment=d.get(
+                "is_waiting_for_code_assignment", None
+            ),
+            name=d.get("name", None),
+            pulled_backup_access_code_id=d.get("pulled_backup_access_code_id", None),
+            starts_at=d.get("starts_at", None),
+            status=d.get("status", None),
+            type=d.get("type", None),
+            warnings=d.get("warnings", None),
         )
 
 
 @dataclass
-class UnmanagedAccessCode:
-    type: str
-    access_code_id: str
-    device_id: str
+class AcsAccessGroup:
+    access_group_type: str
+    access_group_type_display_name: str
+    acs_access_group_id: str
+    acs_system_id: str
+    created_at: str
+    external_type: str
+    external_type_display_name: str
     name: str
+    workspace_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsAccessGroup(
+            access_group_type=d.get("access_group_type", None),
+            access_group_type_display_name=d.get(
+                "access_group_type_display_name", None
+            ),
+            acs_access_group_id=d.get("acs_access_group_id", None),
+            acs_system_id=d.get("acs_system_id", None),
+            created_at=d.get("created_at", None),
+            external_type=d.get("external_type", None),
+            external_type_display_name=d.get("external_type_display_name", None),
+            name=d.get("name", None),
+            workspace_id=d.get("workspace_id", None),
+        )
+
+
+@dataclass
+class AcsCredential:
+    access_method: str
+    acs_credential_id: str
+    acs_credential_pool_id: str
+    acs_system_id: str
+    acs_user_id: str
     code: str
     created_at: str
-    errors: Any
-    warnings: Any
-    is_managed: bool
-    starts_at: str
+    display_name: str
     ends_at: str
-    status: str
+    errors: List[Dict[str, Any]]
+    external_type: str
+    external_type_display_name: str
+    is_multi_phone_sync_credential: bool
+    parent_acs_credential_id: str
+    starts_at: str
+    visionline_metadata: Dict[str, Any]
+    warnings: List[Dict[str, Any]]
+    workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return UnmanagedAccessCode(
-            type=d.get("type", None),
-            access_code_id=d.get("access_code_id", None),
-            device_id=d.get("device_id", None),
-            name=d.get("name", None),
+        return AcsCredential(
+            access_method=d.get("access_method", None),
+            acs_credential_id=d.get("acs_credential_id", None),
+            acs_credential_pool_id=d.get("acs_credential_pool_id", None),
+            acs_system_id=d.get("acs_system_id", None),
+            acs_user_id=d.get("acs_user_id", None),
             code=d.get("code", None),
             created_at=d.get("created_at", None),
+            display_name=d.get("display_name", None),
+            ends_at=d.get("ends_at", None),
             errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            is_managed=d.get("is_managed", None),
+            external_type=d.get("external_type", None),
+            external_type_display_name=d.get("external_type_display_name", None),
+            is_multi_phone_sync_credential=d.get(
+                "is_multi_phone_sync_credential", None
+            ),
+            parent_acs_credential_id=d.get("parent_acs_credential_id", None),
             starts_at=d.get("starts_at", None),
-            ends_at=d.get("ends_at", None),
-            status=d.get("status", None),
+            visionline_metadata=DeepAttrDict(d.get("visionline_metadata", None)),
+            warnings=d.get("warnings", None),
+            workspace_id=d.get("workspace_id", None),
+        )
+
+
+@dataclass
+class AcsCredentialPool:
+    acs_credential_pool_id: str
+    acs_system_id: str
+    created_at: str
+    display_name: str
+    external_type: str
+    external_type_display_name: str
+    workspace_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsCredentialPool(
+            acs_credential_pool_id=d.get("acs_credential_pool_id", None),
+            acs_system_id=d.get("acs_system_id", None),
+            created_at=d.get("created_at", None),
+            display_name=d.get("display_name", None),
+            external_type=d.get("external_type", None),
+            external_type_display_name=d.get("external_type_display_name", None),
+            workspace_id=d.get("workspace_id", None),
+        )
+
+
+@dataclass
+class AcsCredentialProvisioningAutomation:
+    acs_credential_provisioning_automation_id: str
+    created_at: str
+    credential_manager_acs_system_id: str
+    user_identity_id: str
+    workspace_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsCredentialProvisioningAutomation(
+            acs_credential_provisioning_automation_id=d.get(
+                "acs_credential_provisioning_automation_id", None
+            ),
+            created_at=d.get("created_at", None),
+            credential_manager_acs_system_id=d.get(
+                "credential_manager_acs_system_id", None
+            ),
+            user_identity_id=d.get("user_identity_id", None),
+            workspace_id=d.get("workspace_id", None),
+        )
+
+
+@dataclass
+class AcsEntrance:
+    acs_entrance_id: str
+    acs_system_id: str
+    created_at: str
+    display_name: str
+    latch_metadata: Dict[str, Any]
+    visionline_metadata: Dict[str, Any]
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsEntrance(
+            acs_entrance_id=d.get("acs_entrance_id", None),
+            acs_system_id=d.get("acs_system_id", None),
+            created_at=d.get("created_at", None),
+            display_name=d.get("display_name", None),
+            latch_metadata=DeepAttrDict(d.get("latch_metadata", None)),
+            visionline_metadata=DeepAttrDict(d.get("visionline_metadata", None)),
+        )
+
+
+@dataclass
+class AcsSystem:
+    acs_system_id: str
+    can_automate_enrollment: bool
+    connected_account_ids: List[str]
+    created_at: str
+    external_type: str
+    external_type_display_name: str
+    image_alt_text: str
+    image_url: str
+    name: str
+    system_type: str
+    system_type_display_name: str
+    workspace_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsSystem(
+            acs_system_id=d.get("acs_system_id", None),
+            can_automate_enrollment=d.get("can_automate_enrollment", None),
+            connected_account_ids=d.get("connected_account_ids", None),
+            created_at=d.get("created_at", None),
+            external_type=d.get("external_type", None),
+            external_type_display_name=d.get("external_type_display_name", None),
+            image_alt_text=d.get("image_alt_text", None),
+            image_url=d.get("image_url", None),
+            name=d.get("name", None),
+            system_type=d.get("system_type", None),
+            system_type_display_name=d.get("system_type_display_name", None),
+            workspace_id=d.get("workspace_id", None),
+        )
+
+
+@dataclass
+class AcsUser:
+    access_schedule: Dict[str, Any]
+    acs_system_id: str
+    acs_user_id: str
+    created_at: str
+    display_name: str
+    email: str
+    email_address: str
+    external_type: str
+    external_type_display_name: str
+    full_name: str
+    hid_acs_system_id: str
+    is_suspended: bool
+    phone_number: str
+    user_identity_email_address: str
+    user_identity_full_name: str
+    user_identity_id: str
+    user_identity_phone_number: str
+    workspace_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return AcsUser(
+            access_schedule=DeepAttrDict(d.get("access_schedule", None)),
+            acs_system_id=d.get("acs_system_id", None),
+            acs_user_id=d.get("acs_user_id", None),
+            created_at=d.get("created_at", None),
+            display_name=d.get("display_name", None),
+            email=d.get("email", None),
+            email_address=d.get("email_address", None),
+            external_type=d.get("external_type", None),
+            external_type_display_name=d.get("external_type_display_name", None),
+            full_name=d.get("full_name", None),
+            hid_acs_system_id=d.get("hid_acs_system_id", None),
+            is_suspended=d.get("is_suspended", None),
+            phone_number=d.get("phone_number", None),
+            user_identity_email_address=d.get("user_identity_email_address", None),
+            user_identity_full_name=d.get("user_identity_full_name", None),
+            user_identity_id=d.get("user_identity_id", None),
+            user_identity_phone_number=d.get("user_identity_phone_number", None),
+            workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class ActionAttempt:
-    status: str
-    action_type: str
     action_attempt_id: str
-    result: str
+    action_type: str
     error: Dict[str, Any]
+    result: str
+    status: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return ActionAttempt(
-            status=d.get("status", None),
-            action_type=d.get("action_type", None),
             action_attempt_id=d.get("action_attempt_id", None),
-            result=d.get("result", None),
+            action_type=d.get("action_type", None),
             error=DeepAttrDict(d.get("error", None)),
+            result=d.get("result", None),
+            status=d.get("status", None),
         )
 
 
 @dataclass
 class ClientSession:
     client_session_id: str
-    user_identifier_key: str
+    connect_webview_ids: List[str]
+    connected_account_ids: List[str]
     created_at: str
-    token: str
     device_count: float
-    connected_account_ids: List[str]
-    connect_webview_ids: List[str]
+    token: str
+    user_identifier_key: str
     user_identity_ids: List[str]
     workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return ClientSession(
             client_session_id=d.get("client_session_id", None),
-            user_identifier_key=d.get("user_identifier_key", None),
+            connect_webview_ids=d.get("connect_webview_ids", None),
+            connected_account_ids=d.get("connected_account_ids", None),
             created_at=d.get("created_at", None),
-            token=d.get("token", None),
             device_count=d.get("device_count", None),
-            connected_account_ids=d.get("connected_account_ids", None),
-            connect_webview_ids=d.get("connect_webview_ids", None),
+            token=d.get("token", None),
+            user_identifier_key=d.get("user_identifier_key", None),
             user_identity_ids=d.get("user_identity_ids", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class ClimateSettingSchedule:
+    automatic_cooling_enabled: bool
+    automatic_heating_enabled: bool
     climate_setting_schedule_id: str
-    schedule_type: str
-    device_id: str
-    name: str
-    schedule_starts_at: str
-    schedule_ends_at: str
+    cooling_set_point_celsius: float
+    cooling_set_point_fahrenheit: float
     created_at: str
+    device_id: str
     errors: Any
-    automatic_heating_enabled: bool
-    automatic_cooling_enabled: bool
-    hvac_mode_setting: str
-    cooling_set_point_celsius: float
     heating_set_point_celsius: float
-    cooling_set_point_fahrenheit: float
     heating_set_point_fahrenheit: float
+    hvac_mode_setting: str
     manual_override_allowed: bool
+    name: str
+    schedule_ends_at: str
+    schedule_starts_at: str
+    schedule_type: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return ClimateSettingSchedule(
+            automatic_cooling_enabled=d.get("automatic_cooling_enabled", None),
+            automatic_heating_enabled=d.get("automatic_heating_enabled", None),
             climate_setting_schedule_id=d.get("climate_setting_schedule_id", None),
-            schedule_type=d.get("schedule_type", None),
-            device_id=d.get("device_id", None),
-            name=d.get("name", None),
-            schedule_starts_at=d.get("schedule_starts_at", None),
-            schedule_ends_at=d.get("schedule_ends_at", None),
+            cooling_set_point_celsius=d.get("cooling_set_point_celsius", None),
+            cooling_set_point_fahrenheit=d.get("cooling_set_point_fahrenheit", None),
             created_at=d.get("created_at", None),
+            device_id=d.get("device_id", None),
             errors=d.get("errors", None),
-            automatic_heating_enabled=d.get("automatic_heating_enabled", None),
-            automatic_cooling_enabled=d.get("automatic_cooling_enabled", None),
-            hvac_mode_setting=d.get("hvac_mode_setting", None),
-            cooling_set_point_celsius=d.get("cooling_set_point_celsius", None),
             heating_set_point_celsius=d.get("heating_set_point_celsius", None),
-            cooling_set_point_fahrenheit=d.get("cooling_set_point_fahrenheit", None),
             heating_set_point_fahrenheit=d.get("heating_set_point_fahrenheit", None),
+            hvac_mode_setting=d.get("hvac_mode_setting", None),
             manual_override_allowed=d.get("manual_override_allowed", None),
+            name=d.get("name", None),
+            schedule_ends_at=d.get("schedule_ends_at", None),
+            schedule_starts_at=d.get("schedule_starts_at", None),
+            schedule_type=d.get("schedule_type", None),
         )
 
 
 @dataclass
 class ConnectWebview:
-    connect_webview_id: str
-    workspace_id: str
-    created_at: str
-    connected_account_id: str
-    url: str
-    device_selection_mode: str
-    accepted_providers: List[str]
     accepted_devices: List[str]
+    accepted_providers: List[str]
     any_device_allowed: bool
     any_provider_allowed: bool
+    authorized_at: str
+    automatically_manage_new_devices: bool
+    connect_webview_id: str
+    connected_account_id: str
+    created_at: str
+    custom_metadata: Dict[str, Any]
+    custom_redirect_failure_url: str
+    custom_redirect_url: str
+    device_selection_mode: str
     login_successful: bool
+    selected_provider: str
     status: str
-    custom_redirect_url: str
-    custom_redirect_failure_url: str
-    custom_metadata: Dict[str, Any]
-    automatically_manage_new_devices: bool
+    url: str
     wait_for_device_creation: bool
-    authorized_at: str
-    selected_provider: str
+    workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return ConnectWebview(
-            connect_webview_id=d.get("connect_webview_id", None),
-            workspace_id=d.get("workspace_id", None),
-            created_at=d.get("created_at", None),
-            connected_account_id=d.get("connected_account_id", None),
-            url=d.get("url", None),
-            device_selection_mode=d.get("device_selection_mode", None),
-            accepted_providers=d.get("accepted_providers", None),
             accepted_devices=d.get("accepted_devices", None),
+            accepted_providers=d.get("accepted_providers", None),
             any_device_allowed=d.get("any_device_allowed", None),
             any_provider_allowed=d.get("any_provider_allowed", None),
-            login_successful=d.get("login_successful", None),
-            status=d.get("status", None),
-            custom_redirect_url=d.get("custom_redirect_url", None),
-            custom_redirect_failure_url=d.get("custom_redirect_failure_url", None),
-            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
+            authorized_at=d.get("authorized_at", None),
             automatically_manage_new_devices=d.get(
                 "automatically_manage_new_devices", None
             ),
-            wait_for_device_creation=d.get("wait_for_device_creation", None),
-            authorized_at=d.get("authorized_at", None),
+            connect_webview_id=d.get("connect_webview_id", None),
+            connected_account_id=d.get("connected_account_id", None),
+            created_at=d.get("created_at", None),
+            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
+            custom_redirect_failure_url=d.get("custom_redirect_failure_url", None),
+            custom_redirect_url=d.get("custom_redirect_url", None),
+            device_selection_mode=d.get("device_selection_mode", None),
+            login_successful=d.get("login_successful", None),
             selected_provider=d.get("selected_provider", None),
+            status=d.get("status", None),
+            url=d.get("url", None),
+            wait_for_device_creation=d.get("wait_for_device_creation", None),
+            workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class ConnectedAccount:
-    connected_account_id: str
-    created_at: str
-    user_identifier: Dict[str, Any]
     account_type: str
     account_type_display_name: str
+    automatically_manage_new_devices: bool
+    connected_account_id: str
+    created_at: str
+    custom_metadata: Dict[str, Any]
     errors: Any
+    user_identifier: Dict[str, Any]
     warnings: Any
-    custom_metadata: Dict[str, Any]
-    automatically_manage_new_devices: bool
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return ConnectedAccount(
-            connected_account_id=d.get("connected_account_id", None),
-            created_at=d.get("created_at", None),
-            user_identifier=DeepAttrDict(d.get("user_identifier", None)),
             account_type=d.get("account_type", None),
             account_type_display_name=d.get("account_type_display_name", None),
-            errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
             automatically_manage_new_devices=d.get(
                 "automatically_manage_new_devices", None
             ),
+            connected_account_id=d.get("connected_account_id", None),
+            created_at=d.get("created_at", None),
+            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
+            errors=d.get("errors", None),
+            user_identifier=DeepAttrDict(d.get("user_identifier", None)),
+            warnings=d.get("warnings", None),
         )
 
 
 @dataclass
 class Device:
+    can_program_offline_access_codes: bool
+    can_program_online_access_codes: bool
+    can_remotely_lock: bool
+    can_remotely_unlock: bool
+    can_simulate_removal: bool
+    capabilities_supported: List[str]
+    connected_account_id: str
+    created_at: str
+    custom_metadata: Dict[str, Any]
     device_id: str
     device_type: Any
-    nickname: str
     display_name: str
-    capabilities_supported: List[str]
-    properties: Any
-    location: Dict[str, Any]
-    connected_account_id: str
-    workspace_id: str
     errors: List[Dict[str, Any]]
-    warnings: List[Dict[str, Any]]
-    created_at: str
     is_managed: bool
-    custom_metadata: Dict[str, Any]
-    can_remotely_unlock: bool
-    can_remotely_lock: bool
-    can_program_offline_access_codes: bool
-    can_program_online_access_codes: bool
-    can_simulate_removal: bool
+    location: Dict[str, Any]
+    nickname: str
+    properties: Any
+    warnings: List[Dict[str, Any]]
+    workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return Device(
-            device_id=d.get("device_id", None),
-            device_type=d.get("device_type", None),
-            nickname=d.get("nickname", None),
-            display_name=d.get("display_name", None),
-            capabilities_supported=d.get("capabilities_supported", None),
-            properties=DeepAttrDict(d.get("properties", None)),
-            location=DeepAttrDict(d.get("location", None)),
-            connected_account_id=d.get("connected_account_id", None),
-            workspace_id=d.get("workspace_id", None),
-            errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            created_at=d.get("created_at", None),
-            is_managed=d.get("is_managed", None),
-            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
-            can_remotely_unlock=d.get("can_remotely_unlock", None),
-            can_remotely_lock=d.get("can_remotely_lock", None),
             can_program_offline_access_codes=d.get(
                 "can_program_offline_access_codes", None
             ),
             can_program_online_access_codes=d.get(
                 "can_program_online_access_codes", None
             ),
+            can_remotely_lock=d.get("can_remotely_lock", None),
+            can_remotely_unlock=d.get("can_remotely_unlock", None),
             can_simulate_removal=d.get("can_simulate_removal", None),
-        )
-
-
-@dataclass
-class UnmanagedDevice:
-    device_id: str
-    device_type: Any
-    connected_account_id: str
-    capabilities_supported: List[str]
-    workspace_id: str
-    errors: List[Dict[str, Any]]
-    warnings: List[Dict[str, Any]]
-    created_at: str
-    is_managed: bool
-    properties: Dict[str, Any]
-    can_remotely_unlock: bool
-    can_remotely_lock: bool
-    can_program_offline_access_codes: bool
-    can_program_online_access_codes: bool
-    can_simulate_removal: bool
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return UnmanagedDevice(
+            capabilities_supported=d.get("capabilities_supported", None),
+            connected_account_id=d.get("connected_account_id", None),
+            created_at=d.get("created_at", None),
+            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
             device_id=d.get("device_id", None),
             device_type=d.get("device_type", None),
-            connected_account_id=d.get("connected_account_id", None),
-            capabilities_supported=d.get("capabilities_supported", None),
-            workspace_id=d.get("workspace_id", None),
+            display_name=d.get("display_name", None),
             errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            created_at=d.get("created_at", None),
             is_managed=d.get("is_managed", None),
+            location=DeepAttrDict(d.get("location", None)),
+            nickname=d.get("nickname", None),
             properties=DeepAttrDict(d.get("properties", None)),
-            can_remotely_unlock=d.get("can_remotely_unlock", None),
-            can_remotely_lock=d.get("can_remotely_lock", None),
-            can_program_offline_access_codes=d.get(
-                "can_program_offline_access_codes", None
-            ),
-            can_program_online_access_codes=d.get(
-                "can_program_online_access_codes", None
-            ),
-            can_simulate_removal=d.get("can_simulate_removal", None),
+            warnings=d.get("warnings", None),
+            workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class DeviceProvider:
     device_provider_name: str
     display_name: str
@@ -367,436 +512,291 @@
             display_name=d.get("display_name", None),
             image_url=d.get("image_url", None),
             provider_categories=d.get("provider_categories", None),
         )
 
 
 @dataclass
-class Event:
-    event_id: str
-    device_id: str
-    event_type: str
-    workspace_id: str
+class EnrollmentAutomation:
     created_at: str
-    occurred_at: str
+    credential_manager_acs_system_id: str
+    enrollment_automation_id: str
+    user_identity_id: str
+    workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return Event(
-            event_id=d.get("event_id", None),
-            device_id=d.get("device_id", None),
-            event_type=d.get("event_type", None),
-            workspace_id=d.get("workspace_id", None),
+        return EnrollmentAutomation(
             created_at=d.get("created_at", None),
-            occurred_at=d.get("occurred_at", None),
+            credential_manager_acs_system_id=d.get(
+                "credential_manager_acs_system_id", None
+            ),
+            enrollment_automation_id=d.get("enrollment_automation_id", None),
+            user_identity_id=d.get("user_identity_id", None),
+            workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
-class NoiseThreshold:
-    noise_threshold_id: str
+class Event:
+    created_at: str
     device_id: str
-    name: str
-    noise_threshold_nrs: float
-    starts_daily_at: str
-    ends_daily_at: str
-    noise_threshold_decibels: float
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return NoiseThreshold(
-            noise_threshold_id=d.get("noise_threshold_id", None),
-            device_id=d.get("device_id", None),
-            name=d.get("name", None),
-            noise_threshold_nrs=d.get("noise_threshold_nrs", None),
-            starts_daily_at=d.get("starts_daily_at", None),
-            ends_daily_at=d.get("ends_daily_at", None),
-            noise_threshold_decibels=d.get("noise_threshold_decibels", None),
-        )
-
-
-@dataclass
-class ServiceHealth:
-    service: str
-    status: str
-    description: str
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return ServiceHealth(
-            service=d.get("service", None),
-            status=d.get("status", None),
-            description=d.get("description", None),
-        )
-
-
-@dataclass
-class Webhook:
-    webhook_id: str
-    url: str
-    event_types: List[str]
-    secret: str
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return Webhook(
-            webhook_id=d.get("webhook_id", None),
-            url=d.get("url", None),
-            event_types=d.get("event_types", None),
-            secret=d.get("secret", None),
-        )
-
-
-@dataclass
-class Workspace:
+    event_id: str
+    event_type: str
+    occurred_at: str
     workspace_id: str
-    name: str
-    is_sandbox: bool
-    connect_partner_name: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return Workspace(
+        return Event(
+            created_at=d.get("created_at", None),
+            device_id=d.get("device_id", None),
+            event_id=d.get("event_id", None),
+            event_type=d.get("event_type", None),
+            occurred_at=d.get("occurred_at", None),
             workspace_id=d.get("workspace_id", None),
-            name=d.get("name", None),
-            is_sandbox=d.get("is_sandbox", None),
-            connect_partner_name=d.get("connect_partner_name", None),
         )
 
 
 @dataclass
-class AcsSystem:
-    acs_system_id: str
-    external_type: str
-    external_type_display_name: str
-    system_type: str
-    system_type_display_name: str
-    name: str
+class Network:
     created_at: str
+    display_name: str
+    network_id: str
     workspace_id: str
-    connected_account_ids: List[str]
-    image_url: str
-    image_alt_text: str
-    can_automate_enrollment: bool
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return AcsSystem(
-            acs_system_id=d.get("acs_system_id", None),
-            external_type=d.get("external_type", None),
-            external_type_display_name=d.get("external_type_display_name", None),
-            system_type=d.get("system_type", None),
-            system_type_display_name=d.get("system_type_display_name", None),
-            name=d.get("name", None),
+        return Network(
             created_at=d.get("created_at", None),
+            display_name=d.get("display_name", None),
+            network_id=d.get("network_id", None),
             workspace_id=d.get("workspace_id", None),
-            connected_account_ids=d.get("connected_account_ids", None),
-            image_url=d.get("image_url", None),
-            image_alt_text=d.get("image_alt_text", None),
-            can_automate_enrollment=d.get("can_automate_enrollment", None),
         )
 
 
 @dataclass
-class AcsAccessGroup:
-    acs_access_group_id: str
-    acs_system_id: str
-    workspace_id: str
+class NoiseThreshold:
+    device_id: str
+    ends_daily_at: str
     name: str
-    access_group_type: str
-    access_group_type_display_name: str
-    external_type: str
-    external_type_display_name: str
-    created_at: str
+    noise_threshold_decibels: float
+    noise_threshold_id: str
+    noise_threshold_nrs: float
+    starts_daily_at: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return AcsAccessGroup(
-            acs_access_group_id=d.get("acs_access_group_id", None),
-            acs_system_id=d.get("acs_system_id", None),
-            workspace_id=d.get("workspace_id", None),
+        return NoiseThreshold(
+            device_id=d.get("device_id", None),
+            ends_daily_at=d.get("ends_daily_at", None),
             name=d.get("name", None),
-            access_group_type=d.get("access_group_type", None),
-            access_group_type_display_name=d.get(
-                "access_group_type_display_name", None
-            ),
-            external_type=d.get("external_type", None),
-            external_type_display_name=d.get("external_type_display_name", None),
-            created_at=d.get("created_at", None),
+            noise_threshold_decibels=d.get("noise_threshold_decibels", None),
+            noise_threshold_id=d.get("noise_threshold_id", None),
+            noise_threshold_nrs=d.get("noise_threshold_nrs", None),
+            starts_daily_at=d.get("starts_daily_at", None),
         )
 
 
 @dataclass
-class AcsUser:
-    acs_user_id: str
-    acs_system_id: str
-    hid_acs_system_id: str
-    workspace_id: str
+class Phone:
+    can_program_offline_access_codes: bool
+    can_program_online_access_codes: bool
+    can_remotely_lock: bool
+    can_remotely_unlock: bool
+    can_simulate_removal: bool
+    capabilities_supported: List[str]
     created_at: str
+    custom_metadata: Dict[str, Any]
+    device_id: str
+    device_type: str
     display_name: str
-    external_type: str
-    external_type_display_name: str
-    is_suspended: bool
-    access_schedule: Dict[str, Any]
-    user_identity_id: str
-    user_identity_full_name: str
-    user_identity_email_address: str
-    user_identity_phone_number: str
-    full_name: str
-    email: str
-    email_address: str
-    phone_number: str
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return AcsUser(
-            acs_user_id=d.get("acs_user_id", None),
-            acs_system_id=d.get("acs_system_id", None),
-            hid_acs_system_id=d.get("hid_acs_system_id", None),
-            workspace_id=d.get("workspace_id", None),
-            created_at=d.get("created_at", None),
-            display_name=d.get("display_name", None),
-            external_type=d.get("external_type", None),
-            external_type_display_name=d.get("external_type_display_name", None),
-            is_suspended=d.get("is_suspended", None),
-            access_schedule=DeepAttrDict(d.get("access_schedule", None)),
-            user_identity_id=d.get("user_identity_id", None),
-            user_identity_full_name=d.get("user_identity_full_name", None),
-            user_identity_email_address=d.get("user_identity_email_address", None),
-            user_identity_phone_number=d.get("user_identity_phone_number", None),
-            full_name=d.get("full_name", None),
-            email=d.get("email", None),
-            email_address=d.get("email_address", None),
-            phone_number=d.get("phone_number", None),
-        )
-
-
-@dataclass
-class AcsEntrance:
-    acs_entrance_id: str
-    display_name: str
-    acs_system_id: str
-    created_at: str
-    latch_metadata: Dict[str, Any]
-    visionline_metadata: Dict[str, Any]
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return AcsEntrance(
-            acs_entrance_id=d.get("acs_entrance_id", None),
-            display_name=d.get("display_name", None),
-            acs_system_id=d.get("acs_system_id", None),
-            created_at=d.get("created_at", None),
-            latch_metadata=DeepAttrDict(d.get("latch_metadata", None)),
-            visionline_metadata=DeepAttrDict(d.get("visionline_metadata", None)),
-        )
-
-
-@dataclass
-class AcsCredentialProvisioningAutomation:
-    acs_credential_provisioning_automation_id: str
-    credential_manager_acs_system_id: str
-    user_identity_id: str
-    created_at: str
+    errors: List[Dict[str, Any]]
+    is_managed: bool
+    location: Dict[str, Any]
+    nickname: str
+    properties: Dict[str, Any]
+    warnings: List[Dict[str, Any]]
     workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return AcsCredentialProvisioningAutomation(
-            acs_credential_provisioning_automation_id=d.get(
-                "acs_credential_provisioning_automation_id", None
+        return Phone(
+            can_program_offline_access_codes=d.get(
+                "can_program_offline_access_codes", None
             ),
-            credential_manager_acs_system_id=d.get(
-                "credential_manager_acs_system_id", None
+            can_program_online_access_codes=d.get(
+                "can_program_online_access_codes", None
             ),
-            user_identity_id=d.get("user_identity_id", None),
+            can_remotely_lock=d.get("can_remotely_lock", None),
+            can_remotely_unlock=d.get("can_remotely_unlock", None),
+            can_simulate_removal=d.get("can_simulate_removal", None),
+            capabilities_supported=d.get("capabilities_supported", None),
             created_at=d.get("created_at", None),
+            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
+            device_id=d.get("device_id", None),
+            device_type=d.get("device_type", None),
+            display_name=d.get("display_name", None),
+            errors=d.get("errors", None),
+            is_managed=d.get("is_managed", None),
+            location=DeepAttrDict(d.get("location", None)),
+            nickname=d.get("nickname", None),
+            properties=DeepAttrDict(d.get("properties", None)),
+            warnings=d.get("warnings", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
-class AcsCredentialPool:
-    acs_credential_pool_id: str
-    acs_system_id: str
-    display_name: str
-    external_type: str
-    external_type_display_name: str
-    created_at: str
-    workspace_id: str
+class ServiceHealth:
+    description: str
+    service: str
+    status: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return AcsCredentialPool(
-            acs_credential_pool_id=d.get("acs_credential_pool_id", None),
-            acs_system_id=d.get("acs_system_id", None),
-            display_name=d.get("display_name", None),
-            external_type=d.get("external_type", None),
-            external_type_display_name=d.get("external_type_display_name", None),
-            created_at=d.get("created_at", None),
-            workspace_id=d.get("workspace_id", None),
+        return ServiceHealth(
+            description=d.get("description", None),
+            service=d.get("service", None),
+            status=d.get("status", None),
         )
 
 
 @dataclass
-class AcsCredential:
-    acs_credential_id: str
-    acs_user_id: str
-    acs_credential_pool_id: str
-    acs_system_id: str
-    parent_acs_credential_id: str
-    display_name: str
+class UnmanagedAccessCode:
+    access_code_id: str
     code: str
-    access_method: str
-    external_type: str
-    external_type_display_name: str
     created_at: str
-    workspace_id: str
-    starts_at: str
+    device_id: str
     ends_at: str
-    errors: List[Dict[str, Any]]
-    warnings: List[Dict[str, Any]]
-    is_multi_phone_sync_credential: bool
-    visionline_metadata: Dict[str, Any]
+    errors: Any
+    is_managed: bool
+    name: str
+    starts_at: str
+    status: str
+    type: str
+    warnings: Any
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return AcsCredential(
-            acs_credential_id=d.get("acs_credential_id", None),
-            acs_user_id=d.get("acs_user_id", None),
-            acs_credential_pool_id=d.get("acs_credential_pool_id", None),
-            acs_system_id=d.get("acs_system_id", None),
-            parent_acs_credential_id=d.get("parent_acs_credential_id", None),
-            display_name=d.get("display_name", None),
+        return UnmanagedAccessCode(
+            access_code_id=d.get("access_code_id", None),
             code=d.get("code", None),
-            access_method=d.get("access_method", None),
-            external_type=d.get("external_type", None),
-            external_type_display_name=d.get("external_type_display_name", None),
             created_at=d.get("created_at", None),
-            workspace_id=d.get("workspace_id", None),
-            starts_at=d.get("starts_at", None),
+            device_id=d.get("device_id", None),
             ends_at=d.get("ends_at", None),
             errors=d.get("errors", None),
+            is_managed=d.get("is_managed", None),
+            name=d.get("name", None),
+            starts_at=d.get("starts_at", None),
+            status=d.get("status", None),
+            type=d.get("type", None),
             warnings=d.get("warnings", None),
-            is_multi_phone_sync_credential=d.get(
-                "is_multi_phone_sync_credential", None
-            ),
-            visionline_metadata=DeepAttrDict(d.get("visionline_metadata", None)),
         )
 
 
 @dataclass
-class EnrollmentAutomation:
-    credential_manager_acs_system_id: str
-    user_identity_id: str
+class UnmanagedDevice:
+    can_program_offline_access_codes: bool
+    can_program_online_access_codes: bool
+    can_remotely_lock: bool
+    can_remotely_unlock: bool
+    can_simulate_removal: bool
+    capabilities_supported: List[str]
+    connected_account_id: str
     created_at: str
-    workspace_id: str
-    enrollment_automation_id: str
-
-    @staticmethod
-    def from_dict(d: Dict[str, Any]):
-        return EnrollmentAutomation(
-            credential_manager_acs_system_id=d.get(
-                "credential_manager_acs_system_id", None
-            ),
-            user_identity_id=d.get("user_identity_id", None),
-            created_at=d.get("created_at", None),
-            workspace_id=d.get("workspace_id", None),
-            enrollment_automation_id=d.get("enrollment_automation_id", None),
-        )
-
-
-@dataclass
-class Phone:
     device_id: str
-    device_type: str
-    nickname: str
-    display_name: str
-    capabilities_supported: List[str]
-    properties: Dict[str, Any]
-    location: Dict[str, Any]
-    workspace_id: str
+    device_type: Any
     errors: List[Dict[str, Any]]
-    warnings: List[Dict[str, Any]]
-    created_at: str
     is_managed: bool
-    custom_metadata: Dict[str, Any]
-    can_remotely_unlock: bool
-    can_remotely_lock: bool
-    can_program_offline_access_codes: bool
-    can_program_online_access_codes: bool
-    can_simulate_removal: bool
+    properties: Dict[str, Any]
+    warnings: List[Dict[str, Any]]
+    workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return Phone(
-            device_id=d.get("device_id", None),
-            device_type=d.get("device_type", None),
-            nickname=d.get("nickname", None),
-            display_name=d.get("display_name", None),
-            capabilities_supported=d.get("capabilities_supported", None),
-            properties=DeepAttrDict(d.get("properties", None)),
-            location=DeepAttrDict(d.get("location", None)),
-            workspace_id=d.get("workspace_id", None),
-            errors=d.get("errors", None),
-            warnings=d.get("warnings", None),
-            created_at=d.get("created_at", None),
-            is_managed=d.get("is_managed", None),
-            custom_metadata=DeepAttrDict(d.get("custom_metadata", None)),
-            can_remotely_unlock=d.get("can_remotely_unlock", None),
-            can_remotely_lock=d.get("can_remotely_lock", None),
+        return UnmanagedDevice(
             can_program_offline_access_codes=d.get(
                 "can_program_offline_access_codes", None
             ),
             can_program_online_access_codes=d.get(
                 "can_program_online_access_codes", None
             ),
+            can_remotely_lock=d.get("can_remotely_lock", None),
+            can_remotely_unlock=d.get("can_remotely_unlock", None),
             can_simulate_removal=d.get("can_simulate_removal", None),
+            capabilities_supported=d.get("capabilities_supported", None),
+            connected_account_id=d.get("connected_account_id", None),
+            created_at=d.get("created_at", None),
+            device_id=d.get("device_id", None),
+            device_type=d.get("device_type", None),
+            errors=d.get("errors", None),
+            is_managed=d.get("is_managed", None),
+            properties=DeepAttrDict(d.get("properties", None)),
+            warnings=d.get("warnings", None),
+            workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
 class UserIdentity:
-    user_identity_id: str
-    user_identity_key: str
-    email_address: str
-    phone_number: str
+    created_at: str
     display_name: str
+    email_address: str
     full_name: str
-    created_at: str
+    phone_number: str
+    user_identity_id: str
+    user_identity_key: str
     workspace_id: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
         return UserIdentity(
-            user_identity_id=d.get("user_identity_id", None),
-            user_identity_key=d.get("user_identity_key", None),
-            email_address=d.get("email_address", None),
-            phone_number=d.get("phone_number", None),
+            created_at=d.get("created_at", None),
             display_name=d.get("display_name", None),
+            email_address=d.get("email_address", None),
             full_name=d.get("full_name", None),
-            created_at=d.get("created_at", None),
+            phone_number=d.get("phone_number", None),
+            user_identity_id=d.get("user_identity_id", None),
+            user_identity_key=d.get("user_identity_key", None),
             workspace_id=d.get("workspace_id", None),
         )
 
 
 @dataclass
-class Network:
-    network_id: str
+class Webhook:
+    event_types: List[str]
+    secret: str
+    url: str
+    webhook_id: str
+
+    @staticmethod
+    def from_dict(d: Dict[str, Any]):
+        return Webhook(
+            event_types=d.get("event_types", None),
+            secret=d.get("secret", None),
+            url=d.get("url", None),
+            webhook_id=d.get("webhook_id", None),
+        )
+
+
+@dataclass
+class Workspace:
+    connect_partner_name: str
+    is_sandbox: bool
+    name: str
     workspace_id: str
-    display_name: str
-    created_at: str
 
     @staticmethod
     def from_dict(d: Dict[str, Any]):
-        return Network(
-            network_id=d.get("network_id", None),
+        return Workspace(
+            connect_partner_name=d.get("connect_partner_name", None),
+            is_sandbox=d.get("is_sandbox", None),
+            name=d.get("name", None),
             workspace_id=d.get("workspace_id", None),
-            display_name=d.get("display_name", None),
-            created_at=d.get("created_at", None),
         )
 
 
 class SeamApiException(Exception):
     def __init__(
         self,
         response,
@@ -810,327 +810,66 @@
             self.metadata = parsed_response.get("error", None)
 
         super().__init__(
             f"SeamApiException: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
         )
 
 
-class AbstractActionAttempts(abc.ABC):
-
-    @abc.abstractmethod
-    def get(
-        self,
-        *,
-        action_attempt_id: str,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
-    ) -> ActionAttempt:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(self, *, action_attempt_ids: List[str]) -> List[ActionAttempt]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def poll_until_ready(
-        self,
-        *,
-        action_attempt_id: str,
-        timeout: Optional[float] = 5.0,
-        polling_interval: Optional[float] = 0.5,
-    ) -> ActionAttempt:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def decide_and_wait(
-        self,
-        *,
-        action_attempt: ActionAttempt,
-        wait_for_action_attempt: Union[bool, Dict[str, float]],
-    ) -> ActionAttempt:
-        raise NotImplementedError()
-
-
-class AbstractClientSessions(abc.ABC):
-
-    @abc.abstractmethod
-    def create(
-        self,
-        *,
-        user_identifier_key: Optional[str] = None,
-        connect_webview_ids: Optional[List[str]] = None,
-        connected_account_ids: Optional[List[str]] = None,
-        user_identity_ids: Optional[List[str]] = None,
-        expires_at: Optional[str] = None,
-    ) -> ClientSession:
-        raise NotImplementedError()
+class AbstractAccessCodesSimulate(abc.ABC):
 
     @abc.abstractmethod
-    def delete(self, *, client_session_id: str) -> None:
+    def create_unmanaged_access_code(
+        self, *, code: str, device_id: str, name: str
+    ) -> UnmanagedAccessCode:
         raise NotImplementedError()
 
-    @abc.abstractmethod
-    def get(
-        self,
-        *,
-        client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
-    ) -> ClientSession:
-        raise NotImplementedError()
 
-    @abc.abstractmethod
-    def get_or_create(
-        self,
-        *,
-        user_identifier_key: Optional[str] = None,
-        connect_webview_ids: Optional[List[str]] = None,
-        connected_account_ids: Optional[List[str]] = None,
-        user_identity_ids: Optional[List[str]] = None,
-        expires_at: Optional[str] = None,
-    ) -> ClientSession:
-        raise NotImplementedError()
+class AbstractAccessCodesUnmanaged(abc.ABC):
 
     @abc.abstractmethod
-    def grant_access(
+    def convert_to_managed(
         self,
         *,
-        client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
-        connected_account_ids: Optional[List[str]] = None,
-        connect_webview_ids: Optional[List[str]] = None,
-        user_identity_ids: Optional[List[str]] = None,
+        access_code_id: str,
+        allow_external_modification: Optional[bool] = None,
+        force: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None,
+        sync: Optional[bool] = None,
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def list(
-        self,
-        *,
-        client_session_id: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
-        connect_webview_id: Optional[str] = None,
-        without_user_identifier_key: Optional[bool] = None,
-        user_identity_id: Optional[str] = None,
-    ) -> List[ClientSession]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def revoke(self, *, client_session_id: str) -> None:
-        raise NotImplementedError()
-
-
-class AbstractConnectWebviews(abc.ABC):
-
-    @abc.abstractmethod
-    def create(
-        self,
-        *,
-        device_selection_mode: Optional[str] = None,
-        custom_redirect_url: Optional[str] = None,
-        custom_redirect_failure_url: Optional[str] = None,
-        accepted_providers: Optional[List[str]] = None,
-        provider_category: Optional[str] = None,
-        custom_metadata: Optional[Dict[str, Any]] = None,
-        automatically_manage_new_devices: Optional[bool] = None,
-        wait_for_device_creation: Optional[bool] = None,
-    ) -> ConnectWebview:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def delete(self, *, connect_webview_id: str) -> None:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def get(self, *, connect_webview_id: str) -> ConnectWebview:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self,
-        *,
-        user_identifier_key: Optional[str] = None,
-        custom_metadata_has: Optional[Dict[str, Any]] = None,
-    ) -> List[ConnectWebview]:
-        raise NotImplementedError()
-
-
-class AbstractConnectedAccounts(abc.ABC):
-
-    @abc.abstractmethod
-    def delete(self, *, connected_account_id: str, sync: Optional[bool] = None) -> None:
+    def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
-        self, *, connected_account_id: Optional[str] = None, email: Optional[str] = None
-    ) -> ConnectedAccount:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self, *, custom_metadata_has: Optional[Dict[str, Any]] = None
-    ) -> List[ConnectedAccount]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def update(
         self,
         *,
-        connected_account_id: str,
-        automatically_manage_new_devices: Optional[bool] = None,
-        custom_metadata: Optional[Dict[str, Any]] = None,
-    ) -> ConnectedAccount:
-        raise NotImplementedError()
-
-
-class AbstractEvents(abc.ABC):
-
-    @abc.abstractmethod
-    def get(
-        self,
-        *,
-        event_id: Optional[str] = None,
-        event_type: Optional[str] = None,
-        device_id: Optional[str] = None,
-    ) -> Event:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self,
-        *,
-        since: Optional[str] = None,
-        between: Optional[List[str]] = None,
-        device_id: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
         access_code_id: Optional[str] = None,
-        access_code_ids: Optional[List[str]] = None,
-        event_type: Optional[str] = None,
-        event_types: Optional[List[str]] = None,
-        connected_account_id: Optional[str] = None,
-        limit: Optional[float] = None,
-    ) -> List[Event]:
-        raise NotImplementedError()
-
-
-class AbstractLocks(abc.ABC):
-
-    @abc.abstractmethod
-    def get(
-        self, *, device_id: Optional[str] = None, name: Optional[str] = None
-    ) -> Device:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self,
-        *,
-        connected_account_id: Optional[str] = None,
-        connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
-        device_type: Optional[str] = None,
-        device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
-        limit: Optional[float] = None,
-        created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
-        custom_metadata_has: Optional[Dict[str, Any]] = None,
-        include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None,
-    ) -> List[Device]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def lock_door(
-        self,
-        *,
-        device_id: str,
-        sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
-    ) -> ActionAttempt:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def unlock_door(
-        self,
-        *,
-        device_id: str,
-        sync: Optional[bool] = None,
-        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
-    ) -> ActionAttempt:
-        raise NotImplementedError()
-
-
-class AbstractNetworks(abc.ABC):
-
-    @abc.abstractmethod
-    def get(self, *, network_id: str) -> Network:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self,
-    ) -> List[Network]:
-        raise NotImplementedError()
-
-
-class AbstractWebhooks(abc.ABC):
-
-    @abc.abstractmethod
-    def create(self, *, url: str, event_types: Optional[List[str]] = None) -> Webhook:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def delete(self, *, webhook_id: str) -> None:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def get(self, *, webhook_id: str) -> Webhook:
+        code: Optional[str] = None,
+        device_id: Optional[str] = None,
+    ) -> UnmanagedAccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
-        self,
-    ) -> List[Webhook]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def update(self, *, webhook_id: str, event_types: List[str]) -> None:
+        self, *, device_id: str, user_identifier_key: Optional[str] = None
+    ) -> List[UnmanagedAccessCode]:
         raise NotImplementedError()
 
-
-class AbstractWorkspaces(abc.ABC):
-
     @abc.abstractmethod
-    def create(
+    def update(
         self,
         *,
-        name: str,
-        connect_partner_name: str,
-        is_sandbox: Optional[bool] = None,
-        webview_primary_button_color: Optional[str] = None,
-        webview_logo_shape: Optional[str] = None,
-    ) -> Workspace:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def get(
-        self,
-    ) -> Workspace:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def list(
-        self,
-    ) -> List[Workspace]:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def reset_sandbox(
-        self,
+        access_code_id: str,
+        is_managed: bool,
+        allow_external_modification: Optional[bool] = None,
+        force: Optional[bool] = None,
+        is_external_modification_allowed: Optional[bool] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractAcsAccessGroups(abc.ABC):
 
     @abc.abstractmethod
@@ -1165,42 +904,42 @@
 
 class AbstractAcsCredentialProvisioningAutomations(abc.ABC):
 
     @abc.abstractmethod
     def launch(
         self,
         *,
-        user_identity_id: str,
         credential_manager_acs_system_id: str,
+        user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
         credential_manager_acs_user_id: Optional[str] = None,
     ) -> AcsCredentialProvisioningAutomation:
         raise NotImplementedError()
 
 
 class AbstractAcsCredentials(abc.ABC):
 
     @abc.abstractmethod
-    def assign(self, *, acs_user_id: str, acs_credential_id: str) -> None:
+    def assign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create(
         self,
         *,
-        acs_user_id: str,
         access_method: str,
-        credential_manager_acs_system_id: Optional[str] = None,
+        acs_user_id: str,
+        allowed_acs_entrance_ids: Optional[List[str]] = None,
         code: Optional[str] = None,
+        credential_manager_acs_system_id: Optional[str] = None,
+        ends_at: Optional[str] = None,
         is_multi_phone_sync_credential: Optional[bool] = None,
-        allowed_acs_entrance_ids: Optional[List[str]] = None,
-        visionline_metadata: Optional[Dict[str, Any]] = None,
         starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
+        visionline_metadata: Optional[Dict[str, Any]] = None,
     ) -> AcsCredential:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, acs_credential_id: str) -> None:
         raise NotImplementedError()
 
@@ -1216,15 +955,15 @@
         acs_system_id: Optional[str] = None,
         user_identity_id: Optional[str] = None,
         is_multi_phone_sync_credential: Optional[bool] = None,
     ) -> List[AcsCredential]:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def unassign(self, *, acs_user_id: str, acs_credential_id: str) -> None:
+    def unassign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(self, *, acs_credential_id: str, code: str) -> None:
         raise NotImplementedError()
 
 
@@ -1238,16 +977,16 @@
     def grant_access(self, *, acs_entrance_id: str, acs_user_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
-        acs_system_id: Optional[str] = None,
         acs_credential_id: Optional[str] = None,
+        acs_system_id: Optional[str] = None,
     ) -> List[AcsEntrance]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_credentials_with_access(
         self, *, acs_entrance_id: str, include_if: Optional[List[str]] = None
     ) -> List[AcsCredential]:
@@ -1265,30 +1004,30 @@
         raise NotImplementedError()
 
 
 class AbstractAcsUsers(abc.ABC):
 
     @abc.abstractmethod
     def add_to_access_group(
-        self, *, acs_user_id: str, acs_access_group_id: str
+        self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create(
         self,
         *,
         acs_system_id: str,
-        acs_access_group_ids: Optional[List[str]] = None,
-        user_identity_id: Optional[str] = None,
         access_schedule: Optional[Dict[str, Any]] = None,
-        full_name: Optional[str] = None,
+        acs_access_group_ids: Optional[List[str]] = None,
         email: Optional[str] = None,
-        phone_number: Optional[str] = None,
         email_address: Optional[str] = None,
+        full_name: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        user_identity_id: Optional[str] = None,
     ) -> AcsUser:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, acs_user_id: str) -> None:
         raise NotImplementedError()
 
@@ -1296,28 +1035,28 @@
     def get(self, *, acs_user_id: str) -> AcsUser:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
+        acs_system_id: Optional[str] = None,
+        user_identity_email_address: Optional[str] = None,
         user_identity_id: Optional[str] = None,
         user_identity_phone_number: Optional[str] = None,
-        user_identity_email_address: Optional[str] = None,
-        acs_system_id: Optional[str] = None,
     ) -> List[AcsUser]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_accessible_entrances(self, *, acs_user_id: str) -> List[AcsEntrance]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def remove_from_access_group(
-        self, *, acs_user_id: str, acs_access_group_id: str
+        self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def revoke_access_to_all_entrances(self, *, acs_user_id: str) -> None:
         raise NotImplementedError()
 
@@ -1331,76 +1070,187 @@
 
     @abc.abstractmethod
     def update(
         self,
         *,
         acs_user_id: str,
         access_schedule: Optional[Dict[str, Any]] = None,
-        full_name: Optional[str] = None,
         email: Optional[str] = None,
-        phone_number: Optional[str] = None,
         email_address: Optional[str] = None,
+        full_name: Optional[str] = None,
         hid_acs_system_id: Optional[str] = None,
+        phone_number: Optional[str] = None,
     ) -> None:
         raise NotImplementedError()
 
 
-class AbstractAccessCodesSimulate(abc.ABC):
+class AbstractActionAttempts(abc.ABC):
 
     @abc.abstractmethod
-    def create_unmanaged_access_code(
-        self, *, device_id: str, name: str, code: str
-    ) -> UnmanagedAccessCode:
+    def get(
+        self,
+        *,
+        action_attempt_id: str,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+    ) -> ActionAttempt:
         raise NotImplementedError()
 
+    @abc.abstractmethod
+    def list(self, *, action_attempt_ids: List[str]) -> List[ActionAttempt]:
+        raise NotImplementedError()
 
-class AbstractAccessCodesUnmanaged(abc.ABC):
+    @abc.abstractmethod
+    def poll_until_ready(
+        self,
+        *,
+        action_attempt_id: str,
+        timeout: Optional[float] = 5.0,
+        polling_interval: Optional[float] = 0.5,
+    ) -> ActionAttempt:
+        raise NotImplementedError()
 
     @abc.abstractmethod
-    def convert_to_managed(
+    def decide_and_wait(
         self,
         *,
-        access_code_id: str,
-        is_external_modification_allowed: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
-        force: Optional[bool] = None,
-        sync: Optional[bool] = None,
-    ) -> None:
+        action_attempt: ActionAttempt,
+        wait_for_action_attempt: Union[bool, Dict[str, float]],
+    ) -> ActionAttempt:
         raise NotImplementedError()
 
+
+class AbstractClientSessions(abc.ABC):
+
     @abc.abstractmethod
-    def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
+    def create(
+        self,
+        *,
+        connect_webview_ids: Optional[List[str]] = None,
+        connected_account_ids: Optional[List[str]] = None,
+        expires_at: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_ids: Optional[List[str]] = None,
+    ) -> ClientSession:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def delete(self, *, client_session_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
-        device_id: Optional[str] = None,
-        access_code_id: Optional[str] = None,
-        code: Optional[str] = None,
-    ) -> UnmanagedAccessCode:
+        client_session_id: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+    ) -> ClientSession:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get_or_create(
+        self,
+        *,
+        connect_webview_ids: Optional[List[str]] = None,
+        connected_account_ids: Optional[List[str]] = None,
+        expires_at: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_ids: Optional[List[str]] = None,
+    ) -> ClientSession:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def grant_access(
+        self,
+        *,
+        client_session_id: Optional[str] = None,
+        connect_webview_ids: Optional[List[str]] = None,
+        connected_account_ids: Optional[List[str]] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_ids: Optional[List[str]] = None,
+    ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
-        self, *, device_id: str, user_identifier_key: Optional[str] = None
-    ) -> List[UnmanagedAccessCode]:
+        self,
+        *,
+        client_session_id: Optional[str] = None,
+        connect_webview_id: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+        user_identity_id: Optional[str] = None,
+        without_user_identifier_key: Optional[bool] = None,
+    ) -> List[ClientSession]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def revoke(self, *, client_session_id: str) -> None:
+        raise NotImplementedError()
+
+
+class AbstractConnectWebviews(abc.ABC):
+
+    @abc.abstractmethod
+    def create(
+        self,
+        *,
+        accepted_providers: Optional[List[str]] = None,
+        automatically_manage_new_devices: Optional[bool] = None,
+        custom_metadata: Optional[Dict[str, Any]] = None,
+        custom_redirect_failure_url: Optional[str] = None,
+        custom_redirect_url: Optional[str] = None,
+        device_selection_mode: Optional[str] = None,
+        provider_category: Optional[str] = None,
+        wait_for_device_creation: Optional[bool] = None,
+    ) -> ConnectWebview:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def delete(self, *, connect_webview_id: str) -> None:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get(self, *, connect_webview_id: str) -> ConnectWebview:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+        *,
+        custom_metadata_has: Optional[Dict[str, Any]] = None,
+        user_identifier_key: Optional[str] = None,
+    ) -> List[ConnectWebview]:
+        raise NotImplementedError()
+
+
+class AbstractConnectedAccounts(abc.ABC):
+
+    @abc.abstractmethod
+    def delete(self, *, connected_account_id: str, sync: Optional[bool] = None) -> None:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get(
+        self, *, connected_account_id: Optional[str] = None, email: Optional[str] = None
+    ) -> ConnectedAccount:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self, *, custom_metadata_has: Optional[Dict[str, Any]] = None
+    ) -> List[ConnectedAccount]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
-        access_code_id: str,
-        is_managed: bool,
-        allow_external_modification: Optional[bool] = None,
-        is_external_modification_allowed: Optional[bool] = None,
-        force: Optional[bool] = None,
-    ) -> None:
+        connected_account_id: str,
+        automatically_manage_new_devices: Optional[bool] = None,
+        custom_metadata: Optional[Dict[str, Any]] = None,
+    ) -> ConnectedAccount:
         raise NotImplementedError()
 
 
 class AbstractDevicesSimulate(abc.ABC):
 
     @abc.abstractmethod
     def remove(self, *, device_id: str) -> None:
@@ -1415,54 +1265,146 @@
     ) -> UnmanagedDevice:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
+        created_before: Optional[str] = None,
+        custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
+        include_if: Optional[List[str]] = None,
+        limit: Optional[float] = None,
         manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+    ) -> List[UnmanagedDevice]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def update(self, *, device_id: str, is_managed: bool) -> None:
+        raise NotImplementedError()
+
+
+class AbstractEvents(abc.ABC):
+
+    @abc.abstractmethod
+    def get(
+        self,
+        *,
+        device_id: Optional[str] = None,
+        event_id: Optional[str] = None,
+        event_type: Optional[str] = None,
+    ) -> Event:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+        *,
+        access_code_id: Optional[str] = None,
+        access_code_ids: Optional[List[str]] = None,
+        between: Optional[List[str]] = None,
+        connected_account_id: Optional[str] = None,
+        device_id: Optional[str] = None,
         device_ids: Optional[List[str]] = None,
+        event_type: Optional[str] = None,
+        event_types: Optional[List[str]] = None,
         limit: Optional[float] = None,
+        since: Optional[str] = None,
+    ) -> List[Event]:
+        raise NotImplementedError()
+
+
+class AbstractLocks(abc.ABC):
+
+    @abc.abstractmethod
+    def get(
+        self, *, device_id: Optional[str] = None, name: Optional[str] = None
+    ) -> Device:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+        *,
+        connect_webview_id: Optional[str] = None,
+        connected_account_id: Optional[str] = None,
+        connected_account_ids: Optional[List[str]] = None,
         created_before: Optional[str] = None,
-        user_identifier_key: Optional[str] = None,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
-        include_if: Optional[List[str]] = None,
+        device_ids: Optional[List[str]] = None,
+        device_type: Optional[str] = None,
+        device_types: Optional[List[str]] = None,
         exclude_if: Optional[List[str]] = None,
-    ) -> List[UnmanagedDevice]:
+        include_if: Optional[List[str]] = None,
+        limit: Optional[float] = None,
+        manufacturer: Optional[str] = None,
+        user_identifier_key: Optional[str] = None,
+    ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def update(self, *, device_id: str, is_managed: bool) -> None:
+    def lock_door(
+        self,
+        *,
+        device_id: str,
+        sync: Optional[bool] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+    ) -> ActionAttempt:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def unlock_door(
+        self,
+        *,
+        device_id: str,
+        sync: Optional[bool] = None,
+        wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
+    ) -> ActionAttempt:
+        raise NotImplementedError()
+
+
+class AbstractNetworks(abc.ABC):
+
+    @abc.abstractmethod
+    def get(self, *, network_id: str) -> Network:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+    ) -> List[Network]:
         raise NotImplementedError()
 
 
 class AbstractNoiseSensorsNoiseThresholds(abc.ABC):
 
     @abc.abstractmethod
     def create(
         self,
         *,
         device_id: str,
-        starts_daily_at: str,
         ends_daily_at: str,
-        sync: Optional[bool] = None,
+        starts_daily_at: str,
         name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
         noise_threshold_nrs: Optional[float] = None,
+        sync: Optional[bool] = None,
     ) -> NoiseThreshold:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(
-        self, *, noise_threshold_id: str, device_id: str, sync: Optional[bool] = None
+        self, *, device_id: str, noise_threshold_id: str, sync: Optional[bool] = None
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(self, *, noise_threshold_id: str) -> NoiseThreshold:
         raise NotImplementedError()
 
@@ -1472,22 +1414,22 @@
     ) -> List[NoiseThreshold]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
-        noise_threshold_id: str,
         device_id: str,
-        sync: Optional[bool] = None,
-        name: Optional[str] = None,
-        starts_daily_at: Optional[str] = None,
+        noise_threshold_id: str,
         ends_daily_at: Optional[str] = None,
+        name: Optional[str] = None,
         noise_threshold_decibels: Optional[float] = None,
         noise_threshold_nrs: Optional[float] = None,
+        starts_daily_at: Optional[str] = None,
+        sync: Optional[bool] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractNoiseSensorsSimulate(abc.ABC):
 
     @abc.abstractmethod
@@ -1498,40 +1440,40 @@
 class AbstractPhonesSimulate(abc.ABC):
 
     @abc.abstractmethod
     def create_sandbox_phone(
         self,
         *,
         user_identity_id: str,
+        assa_abloy_metadata: Optional[Dict[str, Any]] = None,
         custom_sdk_installation_id: Optional[str] = None,
         phone_metadata: Optional[Dict[str, Any]] = None,
-        assa_abloy_metadata: Optional[Dict[str, Any]] = None,
     ) -> Phone:
         raise NotImplementedError()
 
 
 class AbstractThermostatsClimateSettingSchedules(abc.ABC):
 
     @abc.abstractmethod
     def create(
         self,
         *,
         device_id: str,
-        schedule_starts_at: str,
         schedule_ends_at: str,
-        schedule_type: Optional[str] = None,
-        name: Optional[str] = None,
-        automatic_heating_enabled: Optional[bool] = None,
+        schedule_starts_at: str,
         automatic_cooling_enabled: Optional[bool] = None,
-        hvac_mode_setting: Optional[str] = None,
+        automatic_heating_enabled: Optional[bool] = None,
         cooling_set_point_celsius: Optional[float] = None,
-        heating_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
+        hvac_mode_setting: Optional[str] = None,
         manual_override_allowed: Optional[bool] = None,
+        name: Optional[str] = None,
+        schedule_type: Optional[str] = None,
     ) -> ClimateSettingSchedule:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, climate_setting_schedule_id: str) -> None:
         raise NotImplementedError()
 
@@ -1551,26 +1493,26 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
         climate_setting_schedule_id: str,
-        schedule_type: Optional[str] = None,
-        name: Optional[str] = None,
-        schedule_starts_at: Optional[str] = None,
-        schedule_ends_at: Optional[str] = None,
-        automatic_heating_enabled: Optional[bool] = None,
         automatic_cooling_enabled: Optional[bool] = None,
-        hvac_mode_setting: Optional[str] = None,
+        automatic_heating_enabled: Optional[bool] = None,
         cooling_set_point_celsius: Optional[float] = None,
-        heating_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
         heating_set_point_fahrenheit: Optional[float] = None,
+        hvac_mode_setting: Optional[str] = None,
         manual_override_allowed: Optional[bool] = None,
+        name: Optional[str] = None,
+        schedule_ends_at: Optional[str] = None,
+        schedule_starts_at: Optional[str] = None,
+        schedule_type: Optional[str] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractUserIdentitiesEnrollmentAutomations(abc.ABC):
 
     @abc.abstractmethod
@@ -1581,27 +1523,85 @@
     def get(self, *, enrollment_automation_id: str) -> EnrollmentAutomation:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def launch(
         self,
         *,
-        user_identity_id: str,
         credential_manager_acs_system_id: str,
+        user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
         credential_manager_acs_user_id: Optional[str] = None,
     ) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(self, *, user_identity_id: str) -> List[EnrollmentAutomation]:
         raise NotImplementedError()
 
 
+class AbstractWebhooks(abc.ABC):
+
+    @abc.abstractmethod
+    def create(self, *, url: str, event_types: Optional[List[str]] = None) -> Webhook:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def delete(self, *, webhook_id: str) -> None:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get(self, *, webhook_id: str) -> Webhook:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+    ) -> List[Webhook]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def update(self, *, event_types: List[str], webhook_id: str) -> None:
+        raise NotImplementedError()
+
+
+class AbstractWorkspaces(abc.ABC):
+
+    @abc.abstractmethod
+    def create(
+        self,
+        *,
+        connect_partner_name: str,
+        name: str,
+        is_sandbox: Optional[bool] = None,
+        webview_logo_shape: Optional[str] = None,
+        webview_primary_button_color: Optional[str] = None,
+    ) -> Workspace:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def get(
+        self,
+    ) -> Workspace:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def list(
+        self,
+    ) -> List[Workspace]:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def reset_sandbox(
+        self,
+    ) -> None:
+        raise NotImplementedError()
+
+
 class AbstractPhones(abc.ABC):
 
     @property
     @abc.abstractmethod
     def simulate(self) -> AbstractPhonesSimulate:
         raise NotImplementedError()
 
@@ -1652,40 +1652,40 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def heat_cool(
         self,
         *,
         device_id: str,
-        heating_set_point_celsius: Optional[float] = None,
-        heating_set_point_fahrenheit: Optional[float] = None,
         cooling_set_point_celsius: Optional[float] = None,
         cooling_set_point_fahrenheit: Optional[float] = None,
+        heating_set_point_celsius: Optional[float] = None,
+        heating_set_point_fahrenheit: Optional[float] = None,
         sync: Optional[bool] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
+        created_before: Optional[str] = None,
+        custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
+        include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
-        created_before: Optional[str] = None,
+        manufacturer: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
-        custom_metadata_has: Optional[Dict[str, Any]] = None,
-        include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None,
     ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def off(
         self,
         *,
@@ -1705,38 +1705,38 @@
         sync: Optional[bool] = None,
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
     ) -> ActionAttempt:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
-        self, *, device_id: str, default_climate_setting: Dict[str, Any]
+        self, *, default_climate_setting: Dict[str, Any], device_id: str
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractUserIdentities(abc.ABC):
 
     @property
     @abc.abstractmethod
     def enrollment_automations(self) -> AbstractUserIdentitiesEnrollmentAutomations:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def add_acs_user(self, *, user_identity_id: str, acs_user_id: str) -> None:
+    def add_acs_user(self, *, acs_user_id: str, user_identity_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create(
         self,
         *,
-        user_identity_key: Optional[str] = None,
         email_address: Optional[str] = None,
-        phone_number: Optional[str] = None,
         full_name: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        user_identity_key: Optional[str] = None,
     ) -> UserIdentity:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(self, *, user_identity_id: str) -> None:
         raise NotImplementedError()
 
@@ -1746,15 +1746,15 @@
         *,
         user_identity_id: Optional[str] = None,
         user_identity_key: Optional[str] = None,
     ) -> UserIdentity:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def grant_access_to_device(self, *, user_identity_id: str, device_id: str) -> None:
+    def grant_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self, *, credential_manager_acs_system_id: Optional[str] = None
     ) -> List[UserIdentity]:
         raise NotImplementedError()
@@ -1768,30 +1768,30 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_acs_users(self, *, user_identity_id: str) -> List[AcsUser]:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def remove_acs_user(self, *, user_identity_id: str, acs_user_id: str) -> None:
+    def remove_acs_user(self, *, acs_user_id: str, user_identity_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def revoke_access_to_device(self, *, user_identity_id: str, device_id: str) -> None:
+    def revoke_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
         user_identity_id: str,
-        user_identity_key: Optional[str] = None,
         email_address: Optional[str] = None,
-        phone_number: Optional[str] = None,
         full_name: Optional[str] = None,
+        phone_number: Optional[str] = None,
+        user_identity_key: Optional[str] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractAccessCodes(abc.ABC):
 
     @property
@@ -1805,52 +1805,52 @@
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create(
         self,
         *,
         device_id: str,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
-        code: Optional[str] = None,
-        sync: Optional[bool] = None,
+        allow_external_modification: Optional[bool] = None,
         attempt_for_offline_device: Optional[bool] = None,
+        code: Optional[str] = None,
         common_code_key: Optional[str] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        starts_at: Optional[str] = None,
+        sync: Optional[bool] = None,
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None,
     ) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def create_multiple(
         self,
         *,
         device_ids: List[str],
+        allow_external_modification: Optional[bool] = None,
+        attempt_for_offline_device: Optional[bool] = None,
         behavior_when_code_cannot_be_shared: Optional[str] = None,
-        preferred_code_length: Optional[float] = None,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
         code: Optional[str] = None,
-        attempt_for_offline_device: Optional[bool] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
-        allow_external_modification: Optional[bool] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        preferred_code_length: Optional[float] = None,
+        starts_at: Optional[str] = None,
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None,
     ) -> List[AccessCode]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def delete(
         self,
         *,
@@ -1864,56 +1864,56 @@
     def generate_code(self, *, device_id: str) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def get(
         self,
         *,
-        device_id: Optional[str] = None,
         access_code_id: Optional[str] = None,
         code: Optional[str] = None,
+        device_id: Optional[str] = None,
     ) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
-        device_id: Optional[str] = None,
         access_code_ids: Optional[List[str]] = None,
+        device_id: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
     ) -> List[AccessCode]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def pull_backup_access_code(self, *, access_code_id: str) -> AccessCode:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
         access_code_id: str,
-        name: Optional[str] = None,
-        starts_at: Optional[str] = None,
-        ends_at: Optional[str] = None,
-        code: Optional[str] = None,
-        sync: Optional[bool] = None,
-        attempt_for_offline_device: Optional[bool] = None,
-        prefer_native_scheduling: Optional[bool] = None,
-        use_backup_access_code_pool: Optional[bool] = None,
         allow_external_modification: Optional[bool] = None,
+        attempt_for_offline_device: Optional[bool] = None,
+        code: Optional[str] = None,
+        device_id: Optional[str] = None,
+        ends_at: Optional[str] = None,
         is_external_modification_allowed: Optional[bool] = None,
-        use_offline_access_code: Optional[bool] = None,
+        is_managed: Optional[bool] = None,
         is_offline_access_code: Optional[bool] = None,
         is_one_time_use: Optional[bool] = None,
         max_time_rounding: Optional[str] = None,
-        device_id: Optional[str] = None,
+        name: Optional[str] = None,
+        prefer_native_scheduling: Optional[bool] = None,
+        starts_at: Optional[str] = None,
+        sync: Optional[bool] = None,
         type: Optional[str] = None,
-        is_managed: Optional[bool] = None,
+        use_backup_access_code_pool: Optional[bool] = None,
+        use_offline_access_code: Optional[bool] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractDevices(abc.ABC):
 
     @property
@@ -1936,45 +1936,45 @@
     ) -> Device:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list(
         self,
         *,
+        connect_webview_id: Optional[str] = None,
         connected_account_id: Optional[str] = None,
         connected_account_ids: Optional[List[str]] = None,
-        connect_webview_id: Optional[str] = None,
+        created_before: Optional[str] = None,
+        custom_metadata_has: Optional[Dict[str, Any]] = None,
+        device_ids: Optional[List[str]] = None,
         device_type: Optional[str] = None,
         device_types: Optional[List[str]] = None,
-        manufacturer: Optional[str] = None,
-        device_ids: Optional[List[str]] = None,
+        exclude_if: Optional[List[str]] = None,
+        include_if: Optional[List[str]] = None,
         limit: Optional[float] = None,
-        created_before: Optional[str] = None,
+        manufacturer: Optional[str] = None,
         user_identifier_key: Optional[str] = None,
-        custom_metadata_has: Optional[Dict[str, Any]] = None,
-        include_if: Optional[List[str]] = None,
-        exclude_if: Optional[List[str]] = None,
     ) -> List[Device]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def list_device_providers(
         self, *, provider_category: Optional[str] = None
     ) -> List[DeviceProvider]:
         raise NotImplementedError()
 
     @abc.abstractmethod
     def update(
         self,
         *,
         device_id: str,
-        properties: Optional[Dict[str, Any]] = None,
-        name: Optional[str] = None,
-        is_managed: Optional[bool] = None,
         custom_metadata: Optional[Dict[str, Any]] = None,
+        is_managed: Optional[bool] = None,
+        name: Optional[str] = None,
+        properties: Optional[Dict[str, Any]] = None,
     ) -> None:
         raise NotImplementedError()
 
 
 class AbstractNoiseSensors(abc.ABC):
     pass
 
@@ -2029,29 +2029,29 @@
     def users(self) -> AbstractAcsUsers:
         raise NotImplementedError()
 
 
 @dataclass
 class AbstractRoutes(abc.ABC):
     access_codes: AbstractAccessCodes
+    acs: AbstractAcs
     action_attempts: AbstractActionAttempts
     client_sessions: AbstractClientSessions
     connect_webviews: AbstractConnectWebviews
     connected_accounts: AbstractConnectedAccounts
     devices: AbstractDevices
     events: AbstractEvents
     locks: AbstractLocks
     networks: AbstractNetworks
+    noise_sensors: AbstractNoiseSensors
     phones: AbstractPhones
     thermostats: AbstractThermostats
     user_identities: AbstractUserIdentities
     webhooks: AbstractWebhooks
     workspaces: AbstractWorkspaces
-    acs: AbstractAcs
-    noise_sensors: AbstractNoiseSensors
 
     @abc.abstractmethod
     def make_request(self, method: str, path: str, **kwargs) -> Any:
         raise NotImplementedError
 
 
 @dataclass
```

### Comparing `seam-0.3.0/seam/user_identities.py` & `seam-0.3.1/seam/user_identities.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,46 +19,46 @@
         self.seam = seam
         self._enrollment_automations = UserIdentitiesEnrollmentAutomations(seam=seam)
 
     @property
     def enrollment_automations(self) -> UserIdentitiesEnrollmentAutomations:
         return self._enrollment_automations
 
-    def add_acs_user(self, *, user_identity_id: str, acs_user_id: str) -> None:
+    def add_acs_user(self, *, acs_user_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
 
         self.seam.make_request(
             "POST", "/user_identities/add_acs_user", json=json_payload
         )
 
         return None
 
     def create(
         self,
         *,
-        user_identity_key: Optional[str] = None,
         email_address: Optional[str] = None,
+        full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        full_name: Optional[str] = None
+        user_identity_key: Optional[str] = None
     ) -> UserIdentity:
         json_payload = {}
 
-        if user_identity_key is not None:
-            json_payload["user_identity_key"] = user_identity_key
         if email_address is not None:
             json_payload["email_address"] = email_address
-        if phone_number is not None:
-            json_payload["phone_number"] = phone_number
         if full_name is not None:
             json_payload["full_name"] = full_name
+        if phone_number is not None:
+            json_payload["phone_number"] = phone_number
+        if user_identity_key is not None:
+            json_payload["user_identity_key"] = user_identity_key
 
         res = self.seam.make_request(
             "POST", "/user_identities/create", json=json_payload
         )
 
         return UserIdentity.from_dict(res["user_identity"])
 
@@ -85,21 +85,21 @@
         if user_identity_key is not None:
             json_payload["user_identity_key"] = user_identity_key
 
         res = self.seam.make_request("POST", "/user_identities/get", json=json_payload)
 
         return UserIdentity.from_dict(res["user_identity"])
 
-    def grant_access_to_device(self, *, user_identity_id: str, device_id: str) -> None:
+    def grant_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if device_id is not None:
             json_payload["device_id"] = device_id
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
 
         self.seam.make_request(
             "POST", "/user_identities/grant_access_to_device", json=json_payload
         )
 
         return None
 
@@ -149,60 +149,60 @@
 
         res = self.seam.make_request(
             "POST", "/user_identities/list_acs_users", json=json_payload
         )
 
         return [AcsUser.from_dict(item) for item in res["acs_users"]]
 
-    def remove_acs_user(self, *, user_identity_id: str, acs_user_id: str) -> None:
+    def remove_acs_user(self, *, acs_user_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
 
         self.seam.make_request(
             "POST", "/user_identities/remove_acs_user", json=json_payload
         )
 
         return None
 
-    def revoke_access_to_device(self, *, user_identity_id: str, device_id: str) -> None:
+    def revoke_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if device_id is not None:
             json_payload["device_id"] = device_id
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
 
         self.seam.make_request(
             "POST", "/user_identities/revoke_access_to_device", json=json_payload
         )
 
         return None
 
     def update(
         self,
         *,
         user_identity_id: str,
-        user_identity_key: Optional[str] = None,
         email_address: Optional[str] = None,
+        full_name: Optional[str] = None,
         phone_number: Optional[str] = None,
-        full_name: Optional[str] = None
+        user_identity_key: Optional[str] = None
     ) -> None:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
-        if user_identity_key is not None:
-            json_payload["user_identity_key"] = user_identity_key
         if email_address is not None:
             json_payload["email_address"] = email_address
-        if phone_number is not None:
-            json_payload["phone_number"] = phone_number
         if full_name is not None:
             json_payload["full_name"] = full_name
+        if phone_number is not None:
+            json_payload["phone_number"] = phone_number
+        if user_identity_key is not None:
+            json_payload["user_identity_key"] = user_identity_key
 
         self.seam.make_request("POST", "/user_identities/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/user_identities_enrollment_automations.py` & `seam-0.3.1/seam/user_identities_enrollment_automations.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         )
 
         return EnrollmentAutomation.from_dict(res["enrollment_automation"])
 
     def launch(
         self,
         *,
-        user_identity_id: str,
         credential_manager_acs_system_id: str,
+        user_identity_id: str,
         acs_credential_pool_id: Optional[str] = None,
         create_credential_manager_user: Optional[bool] = None,
         credential_manager_acs_user_id: Optional[str] = None
     ) -> None:
         json_payload = {}
 
-        if user_identity_id is not None:
-            json_payload["user_identity_id"] = user_identity_id
         if credential_manager_acs_system_id is not None:
             json_payload["credential_manager_acs_system_id"] = (
                 credential_manager_acs_system_id
             )
+        if user_identity_id is not None:
+            json_payload["user_identity_id"] = user_identity_id
         if acs_credential_pool_id is not None:
             json_payload["acs_credential_pool_id"] = acs_credential_pool_id
         if create_credential_manager_user is not None:
             json_payload["create_credential_manager_user"] = (
                 create_credential_manager_user
             )
         if credential_manager_acs_user_id is not None:
```

### Comparing `seam-0.3.0/seam/utils/deep_attr_dict.py` & `seam-0.3.1/seam/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.3.0/seam/webhooks.py` & `seam-0.3.1/seam/webhooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,18 @@
     ) -> List[Webhook]:
         json_payload = {}
 
         res = self.seam.make_request("POST", "/webhooks/list", json=json_payload)
 
         return [Webhook.from_dict(item) for item in res["webhooks"]]
 
-    def update(self, *, webhook_id: str, event_types: List[str]) -> None:
+    def update(self, *, event_types: List[str], webhook_id: str) -> None:
         json_payload = {}
 
-        if webhook_id is not None:
-            json_payload["webhook_id"] = webhook_id
         if event_types is not None:
             json_payload["event_types"] = event_types
+        if webhook_id is not None:
+            json_payload["webhook_id"] = webhook_id
 
         self.seam.make_request("POST", "/webhooks/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.3.0/seam/workspaces.py` & `seam-0.3.1/seam/workspaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
     def create(
         self,
         *,
-        name: str,
         connect_partner_name: str,
+        name: str,
         is_sandbox: Optional[bool] = None,
-        webview_primary_button_color: Optional[str] = None,
-        webview_logo_shape: Optional[str] = None
+        webview_logo_shape: Optional[str] = None,
+        webview_primary_button_color: Optional[str] = None
     ) -> Workspace:
         json_payload = {}
 
-        if name is not None:
-            json_payload["name"] = name
         if connect_partner_name is not None:
             json_payload["connect_partner_name"] = connect_partner_name
+        if name is not None:
+            json_payload["name"] = name
         if is_sandbox is not None:
             json_payload["is_sandbox"] = is_sandbox
-        if webview_primary_button_color is not None:
-            json_payload["webview_primary_button_color"] = webview_primary_button_color
         if webview_logo_shape is not None:
             json_payload["webview_logo_shape"] = webview_logo_shape
+        if webview_primary_button_color is not None:
+            json_payload["webview_primary_button_color"] = webview_primary_button_color
 
         res = self.seam.make_request("POST", "/workspaces/create", json=json_payload)
 
         return Workspace.from_dict(res["workspace"])
 
     def get(
         self,
```

### Comparing `seam-0.3.0/PKG-INFO` & `seam-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.3.0
+Version: 0.3.1
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

