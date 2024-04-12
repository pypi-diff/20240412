# Comparing `tmp/prismacloud-cli-0.8.5.tar.gz` & `tmp/prismacloud-cli-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-cli-0.8.5.tar", last modified: Fri Feb 16 14:17:31 2024, max compression
+gzip compressed data, was "prismacloud-cli-0.8.6.tar", last modified: Fri Apr 12 12:58:31 2024, max compression
```

## Comparing `prismacloud-cli-0.8.5.tar` & `prismacloud-cli-0.8.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.970881 prismacloud-cli-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-02-16 14:17:31.970881 prismacloud-cli-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.958881 prismacloud-cli-0.8.5/prismacloud/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.962880 prismacloud-cli-0.8.5/prismacloud/cli/
--rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.962880 prismacloud-cli-0.8.5/prismacloud/cli/cspm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_alert.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_current.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_iam.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_pov.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_rql.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_saas_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.966881 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_audits.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_defenders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_incidents.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_scans.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_users.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.966881 prismacloud-cli-0.8.5/prismacloud/cli/pccs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/pccs/cmd_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/pccs/cmd_reviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/pccs/cmd_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/prismacloud/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.970881 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-16 14:17:31.000000 prismacloud-cli-0.8.5/prismacloud_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-16 14:17:31.970881 prismacloud-cli-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 14:17:31.970881 prismacloud-cli-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-02-16 14:16:49.000000 prismacloud-cli-0.8.5/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.136698 prismacloud-cli-0.8.6/prismacloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.140698 prismacloud-cli-0.8.6/prismacloud/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)    16643 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12625 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.140698 prismacloud-cli-0.8.6/prismacloud/cli/cspm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_iam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_pov.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_rql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_saas_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.144698 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_audits.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_incidents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_scans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8836 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/prismacloud/cli/pccs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31896 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/prismacloud/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 12:58:31.000000 prismacloud-cli-0.8.6/prismacloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:58:31.148698 prismacloud-cli-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-12 12:57:45.000000 prismacloud-cli-0.8.6/tests/test_cli.py
```

### Comparing `prismacloud-cli-0.8.5/LICENSE` & `prismacloud-cli-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/PKG-INFO` & `prismacloud-cli-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.5
+Version: 0.8.6
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
@@ -27,15 +27,15 @@
 Requires-Dist: tabulate
 Requires-Dist: colorama
 Requires-Dist: update_checker
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic
 Requires-Dist: datetime
 Requires-Dist: pyyaml
-Requires-Dist: prismacloud-api==5.2.15
+Requires-Dist: prismacloud-api==5.2.16
 Requires-Dist: pytest
 Requires-Dist: pytest-benchmark
 
 # Prisma Cloud CLI
 
 [![Code Quality Check](https://github.com/PaloAltoNetworks/prismacloud-cli/actions/workflows/build.yml/badge.svg)](https://github.com/PaloAltoNetworks/prismacloud-cli/actions/workflows/build.yml)
```

### Comparing `prismacloud-cli-0.8.5/README.md` & `prismacloud-cli-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/__init__.py` & `prismacloud-cli-0.8.6/prismacloud/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/api.py` & `prismacloud-cli-0.8.6/prismacloud/cli/api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_alert.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_cloud.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_compliance.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_compliance.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_iam.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_iam.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_licenses.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_licenses.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_policy.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_policy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_pov.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_pov.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_resource.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_resource.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_rql.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_rql.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cspm/cmd_saas_version.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cspm/cmd_saas_version.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_audits.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_containers.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_defenders.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_discovery.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_discovery.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_host_auto_deploy.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_host_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_hosts.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_images.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_incidents.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_incidents.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_logs.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_monitor.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_monitor.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_policies.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_registry.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_scans.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/cwpp/cmd_stats.py` & `prismacloud-cli-0.8.6/prismacloud/cli/cwpp/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/pccs/cmd_repositories.py` & `prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud/cli/pccs/cmd_suppressions.py` & `prismacloud-cli-0.8.6/prismacloud/cli/pccs/cmd_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/prismacloud_cli.egg-info/PKG-INFO` & `prismacloud-cli-0.8.6/prismacloud_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.8.5
+Version: 0.8.6
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
@@ -27,15 +27,15 @@
 Requires-Dist: tabulate
 Requires-Dist: colorama
 Requires-Dist: update_checker
 Requires-Dist: pydantic-settings
 Requires-Dist: pydantic
 Requires-Dist: datetime
 Requires-Dist: pyyaml
-Requires-Dist: prismacloud-api==5.2.15
+Requires-Dist: prismacloud-api==5.2.16
 Requires-Dist: pytest
 Requires-Dist: pytest-benchmark
 
 # Prisma Cloud CLI
 
 [![Code Quality Check](https://github.com/PaloAltoNetworks/prismacloud-cli/actions/workflows/build.yml/badge.svg)](https://github.com/PaloAltoNetworks/prismacloud-cli/actions/workflows/build.yml)
```

### Comparing `prismacloud-cli-0.8.5/prismacloud_cli.egg-info/SOURCES.txt` & `prismacloud-cli-0.8.6/prismacloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.8.5/setup.py` & `prismacloud-cli-0.8.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         "tabulate",
         "colorama",
         "update_checker",
         "pydantic-settings",
         "pydantic",
         "datetime",
         "pyyaml",
-        "prismacloud-api==5.2.15",
+        "prismacloud-api==5.2.16",
         "pytest",
         "pytest-benchmark",
     ],
     name="prismacloud-cli",
     version=version,
     python_requires=">=3.7",
     author="Steven de Boer, Simon Melotte, Tom Kishel",
```

### Comparing `prismacloud-cli-0.8.5/tests/test_cli.py` & `prismacloud-cli-0.8.6/tests/test_cli.py`

 * *Files identical despite different names*

