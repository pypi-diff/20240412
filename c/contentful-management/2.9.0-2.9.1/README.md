# Comparing `tmp/contentful_management-2.9.0.tar.gz` & `tmp/contentful_management-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/contentful_management-2.9.0.tar", last modified: Tue Jan  7 10:20:03 2020, max compression
+gzip compressed data, was "dist/contentful_management-2.9.1.tar", last modified: Tue Jan  7 10:28:50 2020, max compression
```

## Comparing `contentful_management-2.9.0.tar` & `contentful_management-2.9.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:20:03.000000 contentful_management-2.9.0/
--rw-r--r--   0 contentdave   (501) staff       (20)     1102 2020-01-07 10:20:03.000000 contentful_management-2.9.0/PKG-INFO
--rw-r--r--   0 contentdave   (501) staff       (20)    30393 2019-02-19 18:58:46.000000 contentful_management-2.9.0/README.rst
-drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management/
--rw-r--r--   0 contentdave   (501) staff       (20)      798 2020-01-07 10:16:36.000000 contentful_management-2.9.0/contentful_management/__init__.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2768 2018-06-13 09:47:41.000000 contentful_management-2.9.0/contentful_management/api_key.py
--rw-r--r--   0 contentdave   (501) staff       (20)      692 2019-02-11 10:08:20.000000 contentful_management-2.9.0/contentful_management/api_keys_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1480 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/api_usage.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2065 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/api_usages_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1123 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/array.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2085 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/asset.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1178 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/assets_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)    29396 2020-01-07 10:16:19.000000 contentful_management-2.9.0/contentful_management/client.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2429 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/client_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     5455 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1452 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_editor_interfaces_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      730 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_entries_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2650 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_field.py
--rw-r--r--   0 contentdave   (501) staff       (20)     3568 2018-10-15 14:53:14.000000 contentful_management-2.9.0/contentful_management/content_type_field_types.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1653 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_field_validation.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1649 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_resource_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1555 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_type_snapshots_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1226 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/content_types_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1864 2018-08-15 12:47:00.000000 contentful_management-2.9.0/contentful_management/editor_interface.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2017 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/editor_interfaces_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2019 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/entries_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     3671 2019-01-17 10:43:01.000000 contentful_management-2.9.0/contentful_management/entry.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1576 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/entry_resource_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      960 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/entry_snapshots_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     5600 2019-02-19 18:58:46.000000 contentful_management-2.9.0/contentful_management/environment.py
--rw-r--r--   0 contentdave   (501) staff       (20)      715 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/environment_assets_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      771 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/environment_content_types_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      721 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/environment_entries_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      921 2018-08-15 09:50:16.000000 contentful_management-2.9.0/contentful_management/environment_locales_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1554 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/environment_resource_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      748 2018-08-15 11:58:56.000000 contentful_management-2.9.0/contentful_management/environment_ui_extensions_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      746 2018-08-14 14:22:14.000000 contentful_management-2.9.0/contentful_management/environments_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     6825 2018-08-14 13:40:24.000000 contentful_management-2.9.0/contentful_management/errors.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2059 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/locale.py
--rw-r--r--   0 contentdave   (501) staff       (20)      819 2018-08-15 09:50:16.000000 contentful_management-2.9.0/contentful_management/locales_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2189 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/organization.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1423 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/organizations_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1604 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/personal_access_token.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1641 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/personal_access_tokens_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1158 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/preview_api_key.py
--rw-r--r--   0 contentdave   (501) staff       (20)      791 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/preview_api_keys_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)    15095 2019-02-11 10:33:37.000000 contentful_management-2.9.0/contentful_management/resource.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2829 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/resource_builder.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1570 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/role.py
--rw-r--r--   0 contentdave   (501) staff       (20)      797 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/roles_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2285 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/snapshot.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1646 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/snapshots_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     7746 2018-10-31 10:39:10.000000 contentful_management-2.9.0/contentful_management/space.py
--rw-r--r--   0 contentdave   (501) staff       (20)      886 2018-08-14 14:01:48.000000 contentful_management-2.9.0/contentful_management/space_api_keys_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      680 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/space_environments_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1240 2018-08-14 11:57:36.000000 contentful_management-2.9.0/contentful_management/space_membership.py
--rw-r--r--   0 contentdave   (501) staff       (20)      781 2018-08-14 11:57:08.000000 contentful_management-2.9.0/contentful_management/space_memberships_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1062 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/space_preview_api_keys_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1423 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/space_resource_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      857 2018-08-15 09:34:56.000000 contentful_management-2.9.0/contentful_management/space_roles_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      984 2018-08-14 13:40:24.000000 contentful_management-2.9.0/contentful_management/space_space_memberships_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      890 2018-08-16 09:17:25.000000 contentful_management-2.9.0/contentful_management/space_webhooks_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1830 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/spaces_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2600 2018-08-16 11:26:39.000000 contentful_management-2.9.0/contentful_management/ui_extension.py
--rw-r--r--   0 contentdave   (501) staff       (20)      680 2018-08-15 11:58:56.000000 contentful_management-2.9.0/contentful_management/ui_extensions_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      912 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/upload.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1839 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/uploads_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1202 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/usage_period.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1755 2018-11-13 10:52:17.000000 contentful_management-2.9.0/contentful_management/usage_periods_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1384 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/user.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1395 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/users_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     6017 2019-02-11 10:33:37.000000 contentful_management-2.9.0/contentful_management/utils.py
--rw-r--r--   0 contentdave   (501) staff       (20)     4023 2018-08-16 10:07:27.000000 contentful_management-2.9.0/contentful_management/webhook.py
--rw-r--r--   0 contentdave   (501) staff       (20)     2035 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhook_call.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1344 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhook_health.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1371 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhook_resource_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      749 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhook_webhooks_call_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      911 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhook_webhooks_health_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1364 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhooks_call_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)     1442 2018-05-15 15:03:07.000000 contentful_management-2.9.0/contentful_management/webhooks_health_proxy.py
--rw-r--r--   0 contentdave   (501) staff       (20)      853 2018-08-16 09:17:04.000000 contentful_management-2.9.0/contentful_management/webhooks_proxy.py
-drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/
--rw-r--r--   0 contentdave   (501) staff       (20)     1102 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/PKG-INFO
--rw-r--r--   0 contentdave   (501) staff       (20)     3575 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/SOURCES.txt
--rw-r--r--   0 contentdave   (501) staff       (20)        1 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/dependency_links.txt
--rw-r--r--   0 contentdave   (501) staff       (20)        1 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/not-zip-safe
--rw-r--r--   0 contentdave   (501) staff       (20)       38 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/requires.txt
--rw-r--r--   0 contentdave   (501) staff       (20)       22 2020-01-07 10:20:03.000000 contentful_management-2.9.0/contentful_management.egg-info/top_level.txt
--rw-r--r--   0 contentdave   (501) staff       (20)       38 2020-01-07 10:20:03.000000 contentful_management-2.9.0/setup.cfg
--rwxr-xr-x   0 contentdave   (501) staff       (20)     3040 2018-10-31 10:46:55.000000 contentful_management-2.9.0/setup.py
+drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:28:50.000000 contentful_management-2.9.1/
+-rw-r--r--   0 contentdave   (501) staff       (20)      804 2020-01-07 10:28:50.000000 contentful_management-2.9.1/PKG-INFO
+-rw-r--r--   0 contentdave   (501) staff       (20)    30393 2019-02-19 18:58:46.000000 contentful_management-2.9.1/README.rst
+drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:28:50.000000 contentful_management-2.9.1/contentful_management/
+-rw-r--r--   0 contentdave   (501) staff       (20)      798 2020-01-07 10:28:00.000000 contentful_management-2.9.1/contentful_management/__init__.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2768 2018-06-13 09:47:41.000000 contentful_management-2.9.1/contentful_management/api_key.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      692 2019-02-11 10:08:20.000000 contentful_management-2.9.1/contentful_management/api_keys_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1480 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/api_usage.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2065 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/api_usages_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1123 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/array.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2085 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/asset.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1178 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/assets_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)    29396 2020-01-07 10:16:19.000000 contentful_management-2.9.1/contentful_management/client.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2429 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/client_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     5455 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1452 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_editor_interfaces_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      730 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_entries_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2650 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_field.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     3568 2018-10-15 14:53:14.000000 contentful_management-2.9.1/contentful_management/content_type_field_types.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1653 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_field_validation.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1649 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_resource_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1555 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_type_snapshots_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1226 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/content_types_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1864 2018-08-15 12:47:00.000000 contentful_management-2.9.1/contentful_management/editor_interface.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2017 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/editor_interfaces_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2019 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/entries_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     3671 2019-01-17 10:43:01.000000 contentful_management-2.9.1/contentful_management/entry.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1576 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/entry_resource_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      960 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/entry_snapshots_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     5600 2019-02-19 18:58:46.000000 contentful_management-2.9.1/contentful_management/environment.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      715 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/environment_assets_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      771 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/environment_content_types_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      721 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/environment_entries_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      921 2018-08-15 09:50:16.000000 contentful_management-2.9.1/contentful_management/environment_locales_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1554 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/environment_resource_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      748 2018-08-15 11:58:56.000000 contentful_management-2.9.1/contentful_management/environment_ui_extensions_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      746 2018-08-14 14:22:14.000000 contentful_management-2.9.1/contentful_management/environments_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     6825 2018-08-14 13:40:24.000000 contentful_management-2.9.1/contentful_management/errors.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2059 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/locale.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      819 2018-08-15 09:50:16.000000 contentful_management-2.9.1/contentful_management/locales_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2189 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/organization.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1423 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/organizations_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1604 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/personal_access_token.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1641 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/personal_access_tokens_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1158 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/preview_api_key.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      791 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/preview_api_keys_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)    15095 2019-02-11 10:33:37.000000 contentful_management-2.9.1/contentful_management/resource.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2829 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/resource_builder.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1570 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/role.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      797 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/roles_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2285 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/snapshot.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1646 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/snapshots_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     7746 2018-10-31 10:39:10.000000 contentful_management-2.9.1/contentful_management/space.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      886 2018-08-14 14:01:48.000000 contentful_management-2.9.1/contentful_management/space_api_keys_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      680 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/space_environments_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1240 2018-08-14 11:57:36.000000 contentful_management-2.9.1/contentful_management/space_membership.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      781 2018-08-14 11:57:08.000000 contentful_management-2.9.1/contentful_management/space_memberships_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1062 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/space_preview_api_keys_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1423 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/space_resource_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      857 2018-08-15 09:34:56.000000 contentful_management-2.9.1/contentful_management/space_roles_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      984 2018-08-14 13:40:24.000000 contentful_management-2.9.1/contentful_management/space_space_memberships_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      890 2018-08-16 09:17:25.000000 contentful_management-2.9.1/contentful_management/space_webhooks_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1830 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/spaces_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2600 2018-08-16 11:26:39.000000 contentful_management-2.9.1/contentful_management/ui_extension.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      680 2018-08-15 11:58:56.000000 contentful_management-2.9.1/contentful_management/ui_extensions_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      912 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/upload.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1839 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/uploads_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1202 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/usage_period.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1755 2018-11-13 10:52:17.000000 contentful_management-2.9.1/contentful_management/usage_periods_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1384 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/user.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1395 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/users_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     6017 2019-02-11 10:33:37.000000 contentful_management-2.9.1/contentful_management/utils.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     4023 2018-08-16 10:07:27.000000 contentful_management-2.9.1/contentful_management/webhook.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     2035 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhook_call.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1344 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhook_health.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1371 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhook_resource_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      749 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhook_webhooks_call_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      911 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhook_webhooks_health_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1364 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhooks_call_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)     1442 2018-05-15 15:03:07.000000 contentful_management-2.9.1/contentful_management/webhooks_health_proxy.py
+-rw-r--r--   0 contentdave   (501) staff       (20)      853 2018-08-16 09:17:04.000000 contentful_management-2.9.1/contentful_management/webhooks_proxy.py
+drwxr-xr-x   0 contentdave   (501) staff       (20)        0 2020-01-07 10:28:50.000000 contentful_management-2.9.1/contentful_management.egg-info/
+-rw-r--r--   0 contentdave   (501) staff       (20)      804 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/PKG-INFO
+-rw-r--r--   0 contentdave   (501) staff       (20)     3575 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/SOURCES.txt
+-rw-r--r--   0 contentdave   (501) staff       (20)        1 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/dependency_links.txt
+-rw-r--r--   0 contentdave   (501) staff       (20)        1 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/not-zip-safe
+-rw-r--r--   0 contentdave   (501) staff       (20)       38 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/requires.txt
+-rw-r--r--   0 contentdave   (501) staff       (20)       22 2020-01-07 10:28:49.000000 contentful_management-2.9.1/contentful_management.egg-info/top_level.txt
+-rw-r--r--   0 contentdave   (501) staff       (20)       38 2020-01-07 10:28:50.000000 contentful_management-2.9.1/setup.cfg
+-rwxr-xr-x   0 contentdave   (501) staff       (20)     2748 2020-01-07 10:28:25.000000 contentful_management-2.9.1/setup.py
```

### Comparing `contentful_management-2.9.0/README.rst` & `contentful_management-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/__init__.py` & `contentful_management-2.9.1/contentful_management/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,10 +11,10 @@
 from .upload import Upload  # noqa: F401
 from .webhook import Webhook  # noqa: F401
 from .resource import Link  # noqa: F401
 from .content_type import ContentType  # noqa: F401
 from .content_type_field import ContentTypeField  # noqa: F401
 
 
-__version__ = "2.9.0"
+__version__ = "2.9.1"
 __author__ = "Contentful GmbH (David Litvak Bruno)"
 __email__ = "david.litvak@contentful.com"
```

### Comparing `contentful_management-2.9.0/contentful_management/api_key.py` & `contentful_management-2.9.1/contentful_management/api_key.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/api_keys_proxy.py` & `contentful_management-2.9.1/contentful_management/api_keys_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/api_usage.py` & `contentful_management-2.9.1/contentful_management/api_usage.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/api_usages_proxy.py` & `contentful_management-2.9.1/contentful_management/api_usages_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/array.py` & `contentful_management-2.9.1/contentful_management/array.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/asset.py` & `contentful_management-2.9.1/contentful_management/asset.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/assets_proxy.py` & `contentful_management-2.9.1/contentful_management/assets_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/client.py` & `contentful_management-2.9.1/contentful_management/client.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/client_proxy.py` & `contentful_management-2.9.1/contentful_management/client_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type.py` & `contentful_management-2.9.1/contentful_management/content_type.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_editor_interfaces_proxy.py` & `contentful_management-2.9.1/contentful_management/content_type_editor_interfaces_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_entries_proxy.py` & `contentful_management-2.9.1/contentful_management/content_type_entries_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_field.py` & `contentful_management-2.9.1/contentful_management/content_type_field.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_field_types.py` & `contentful_management-2.9.1/contentful_management/content_type_field_types.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_field_validation.py` & `contentful_management-2.9.1/contentful_management/content_type_field_validation.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_resource_proxy.py` & `contentful_management-2.9.1/contentful_management/content_type_resource_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_type_snapshots_proxy.py` & `contentful_management-2.9.1/contentful_management/content_type_snapshots_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/content_types_proxy.py` & `contentful_management-2.9.1/contentful_management/content_types_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/editor_interface.py` & `contentful_management-2.9.1/contentful_management/editor_interface.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/editor_interfaces_proxy.py` & `contentful_management-2.9.1/contentful_management/editor_interfaces_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/entries_proxy.py` & `contentful_management-2.9.1/contentful_management/entries_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/entry.py` & `contentful_management-2.9.1/contentful_management/entry.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/entry_resource_proxy.py` & `contentful_management-2.9.1/contentful_management/entry_resource_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/entry_snapshots_proxy.py` & `contentful_management-2.9.1/contentful_management/entry_snapshots_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment.py` & `contentful_management-2.9.1/contentful_management/environment.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_assets_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_assets_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_content_types_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_content_types_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_entries_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_entries_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_locales_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_locales_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_resource_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_resource_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environment_ui_extensions_proxy.py` & `contentful_management-2.9.1/contentful_management/environment_ui_extensions_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/environments_proxy.py` & `contentful_management-2.9.1/contentful_management/environments_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/errors.py` & `contentful_management-2.9.1/contentful_management/errors.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/locale.py` & `contentful_management-2.9.1/contentful_management/locale.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/locales_proxy.py` & `contentful_management-2.9.1/contentful_management/locales_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/organization.py` & `contentful_management-2.9.1/contentful_management/organization.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/organizations_proxy.py` & `contentful_management-2.9.1/contentful_management/organizations_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/personal_access_token.py` & `contentful_management-2.9.1/contentful_management/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/personal_access_tokens_proxy.py` & `contentful_management-2.9.1/contentful_management/personal_access_tokens_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/preview_api_key.py` & `contentful_management-2.9.1/contentful_management/preview_api_key.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/preview_api_keys_proxy.py` & `contentful_management-2.9.1/contentful_management/preview_api_keys_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/resource.py` & `contentful_management-2.9.1/contentful_management/resource.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/resource_builder.py` & `contentful_management-2.9.1/contentful_management/resource_builder.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/role.py` & `contentful_management-2.9.1/contentful_management/role.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/roles_proxy.py` & `contentful_management-2.9.1/contentful_management/roles_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/snapshot.py` & `contentful_management-2.9.1/contentful_management/snapshot.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/snapshots_proxy.py` & `contentful_management-2.9.1/contentful_management/snapshots_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space.py` & `contentful_management-2.9.1/contentful_management/space.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_api_keys_proxy.py` & `contentful_management-2.9.1/contentful_management/space_api_keys_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_environments_proxy.py` & `contentful_management-2.9.1/contentful_management/space_environments_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_membership.py` & `contentful_management-2.9.1/contentful_management/space_membership.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_memberships_proxy.py` & `contentful_management-2.9.1/contentful_management/space_memberships_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_preview_api_keys_proxy.py` & `contentful_management-2.9.1/contentful_management/space_preview_api_keys_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_resource_proxy.py` & `contentful_management-2.9.1/contentful_management/space_resource_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_roles_proxy.py` & `contentful_management-2.9.1/contentful_management/space_roles_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_space_memberships_proxy.py` & `contentful_management-2.9.1/contentful_management/space_space_memberships_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/space_webhooks_proxy.py` & `contentful_management-2.9.1/contentful_management/space_webhooks_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/spaces_proxy.py` & `contentful_management-2.9.1/contentful_management/spaces_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/ui_extension.py` & `contentful_management-2.9.1/contentful_management/ui_extension.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/ui_extensions_proxy.py` & `contentful_management-2.9.1/contentful_management/ui_extensions_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/upload.py` & `contentful_management-2.9.1/contentful_management/upload.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/uploads_proxy.py` & `contentful_management-2.9.1/contentful_management/uploads_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/usage_period.py` & `contentful_management-2.9.1/contentful_management/usage_period.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/usage_periods_proxy.py` & `contentful_management-2.9.1/contentful_management/usage_periods_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/user.py` & `contentful_management-2.9.1/contentful_management/user.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/users_proxy.py` & `contentful_management-2.9.1/contentful_management/users_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/utils.py` & `contentful_management-2.9.1/contentful_management/utils.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook.py` & `contentful_management-2.9.1/contentful_management/webhook.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook_call.py` & `contentful_management-2.9.1/contentful_management/webhook_call.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook_health.py` & `contentful_management-2.9.1/contentful_management/webhook_health.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook_resource_proxy.py` & `contentful_management-2.9.1/contentful_management/webhook_resource_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook_webhooks_call_proxy.py` & `contentful_management-2.9.1/contentful_management/webhook_webhooks_call_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhook_webhooks_health_proxy.py` & `contentful_management-2.9.1/contentful_management/webhook_webhooks_health_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhooks_call_proxy.py` & `contentful_management-2.9.1/contentful_management/webhooks_call_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhooks_health_proxy.py` & `contentful_management-2.9.1/contentful_management/webhooks_health_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management/webhooks_proxy.py` & `contentful_management-2.9.1/contentful_management/webhooks_proxy.py`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/contentful_management.egg-info/PKG-INFO` & `contentful_management-2.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 Metadata-Version: 1.1
-Name: contentful-management
-Version: 2.9.0
+Name: contentful_management
+Version: 2.9.1
 Summary: Contentful Management API Client
 Home-page: https://github.com/contentful/contentful-management.py
 Author: Contentful GmbH (David Litvak Bruno)
 Author-email: david.litvak@contentful.com
 License: MIT
 Description: UNKNOWN
 Keywords: contentful management cma cms content
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.1
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `contentful_management-2.9.0/contentful_management.egg-info/SOURCES.txt` & `contentful_management-2.9.1/contentful_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `contentful_management-2.9.0/setup.py` & `contentful_management-2.9.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -87,21 +87,15 @@
     keywords='contentful management cma cms content',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Topic :: Software Development :: Libraries',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.1',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
     ],
     test_suite='tests',
     tests_require=test_requirements
 )
```

