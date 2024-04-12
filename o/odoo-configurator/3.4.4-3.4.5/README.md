# Comparing `tmp/odoo-configurator-3.4.4.tar.gz` & `tmp/odoo-configurator-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo-configurator-3.4.4.tar", last modified: Wed Feb  7 10:12:03 2024, max compression
+gzip compressed data, was "odoo-configurator-3.4.5.tar", last modified: Thu Mar 14 15:35:06 2024, max compression
```

## Comparing `odoo-configurator-3.4.4.tar` & `odoo-configurator-3.4.5.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22260 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/logo_scalizer.png
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.124660 odoo-configurator-3.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.128661 odoo-configurator-3.4.4/src/odoo_configurator/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.132660 odoo-configurator-3.4.4/src/odoo_configurator/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7008 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/account.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5415 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/call.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11977 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/datas.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13987 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/import_configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/imports.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1487 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/mattermost.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5425 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/modules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/roles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/system_parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/translations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/users.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/apps/website.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/bitwarden.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8708 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/configurator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8695 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/import_manager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3495 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/keepass.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/logging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9622 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/odoo_configurator/odoo_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22260 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-07 10:12:03.000000 odoo-configurator-3.4.4/src/odoo_configurator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/src/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/0_base.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 10:12:03.136660 odoo-configurator-3.4.4/src/templates/14.0/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/14.0/0_base.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/1_base_auto_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/1_base_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_account.yml
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_account_14.yml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_account_entreprise.yml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_crm.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_event.yml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_expense.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_ged.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_hr.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_maintenance.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_marketing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_mrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_purchase.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_sale.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_sale_subscription.yml
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_sign.yml
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/src/templates/2_base_website.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-02-07 10:11:50.000000 odoo-configurator-3.4.4/start_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.447342 odoo-configurator-3.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-03-14 15:35:06.447342 odoo-configurator-3.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/logo_scalizer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 15:35:06.447342 odoo-configurator-3.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.435342 odoo-configurator-3.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.439343 odoo-configurator-3.4.5/src/odoo_configurator/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.443343 odoo-configurator-3.4.5/src/odoo_configurator/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7008 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5415 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2079 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/call.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      293 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11977 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/datas.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1439 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14343 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/import_configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2238 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/imports.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1487 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/mattermost.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5425 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/modules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/system_parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1780 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/translations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1312 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/users.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      513 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/apps/website.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1563 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/bitwarden.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8708 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/configurator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8695 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/import_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3495 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/keepass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9622 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/odoo_configurator/odoo_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.447342 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22346 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-14 15:35:06.000000 odoo-configurator-3.4.5/src/odoo_configurator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.443343 odoo-configurator-3.4.5/src/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/0_base.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 15:35:06.443343 odoo-configurator-3.4.5/src/templates/14.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/14.0/0_base.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/1_base_auto_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/1_base_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_account.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_account_14.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_account_entreprise.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_crm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_event.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_expense.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_ged.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_hr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_maintenance.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_marketing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_mrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_purchase.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_sale.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_sale_subscription.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_sign.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/src/templates/2_base_website.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      247 2024-03-14 15:34:56.000000 odoo-configurator-3.4.5/start_config.py
```

### Comparing `odoo-configurator-3.4.4/LICENSE` & `odoo-configurator-3.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/PKG-INFO` & `odoo-configurator-3.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.4.4
+Version: 3.4.5
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,14 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://github.com/ScalizerOrg/odoo-configurator
+Project-URL: Changelog, https://github.com/ScalizerOrg/odoo-configurator/CHANGELOG.md
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `odoo-configurator-3.4.4/README.md` & `odoo-configurator-3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/logo_scalizer.png` & `odoo-configurator-3.4.5/logo_scalizer.png`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/pyproject.toml` & `odoo-configurator-3.4.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "odoo-configurator"
-version = "3.4.4"
+version = "3.4.5"
 description = "Configure and update Odoo database with YAML files"
 readme = "README.md"
 authors = [{ name = "Michel Perrocheau", email = "myrrkel@gmail.com" },
 { name = "David Halgand", email = "david@scalizer.fr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
@@ -30,10 +30,11 @@
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["twine", "bumpver", "pip-tools", "pytest", "check-manifest"]
 
 [project.urls]
 Homepage = "https://github.com/ScalizerOrg/odoo-configurator"
+Changelog = "https://github.com/ScalizerOrg/odoo-configurator/CHANGELOG.md"
 
 [project.scripts]
 odoo-configurator = "odoo_configurator.__main__:main"
```

### Comparing `odoo-configurator-3.4.4/requirements.txt` & `odoo-configurator-3.4.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/__main__.py` & `odoo-configurator-3.4.5/src/odoo_configurator/__main__.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/account.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/account.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/base.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/base.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/call.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/call.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/config.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/config.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/datas.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/datas.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/defaults.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/defaults.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/import_configurator.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/import_configurator.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             rec_name = self.get_record_name(record, model)
             prefix = self.get_record_prefix(record)
             if prefix:
                 rec_name = '%s %s' % (prefix, rec_name)
 
             xmlid = self.get_xmlid(model, record.get('id'))
             if not xmlid:
-                xmlid = self.compute_xml_id(record)  # Todo
+                xmlid = self.compute_xml_id(record, model)
             res += '\n%s%s:' % (" " * 4 * 2, rec_name)
             res += '\n%s%s: %s' % (" " * 4 * 3, 'model', model)
             res += '\n%s%s: %s' % (" " * 4 * 3, 'force_id', xmlid)
             res += '\n%s%s:' % (" " * 4 * 3, 'values')
 
             field_names = sort_fields(self.model_fields.keys())
             for key in field_names:
@@ -229,14 +229,22 @@
     def get_xmlid(self, model, res_id):
         if (model, res_id) in self.rec_to_xmlid_cache:
             return self.rec_to_xmlid_cache[(model, res_id)]
         xmlid = self.get_xml_id_from_id(model, res_id)
         self.rec_to_xmlid_cache[(model, res_id)] = xmlid
         return xmlid
 
+    def compute_xml_id(self, record, model, retry=0):
+        xml_id = 'external_config.%s_%s' % (model.replace('.', '_'), str(record['id']+retry).zfill(5))
+        if not self._connection.get_id_from_xml_id(xml_id, no_raise=True):
+            return xml_id
+        else:
+            retry += 1
+            return self.compute_xml_id(record, model, retry)
+
     def apply(self):
         super(ImportConfigurator, self).apply()
         for key in self._datas:
             if isinstance(self._datas.get(key), dict) or isinstance(self._datas.get(key), OrderedDict):
                 action_name = 'import_configurator_model_file'
                 configurator_model_files = self._datas.get(key).get(action_name, {})
                 if configurator_model_files:
```

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/imports.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/imports.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/mattermost.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/mattermost.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/modules.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/modules.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/roles.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/roles.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/system_parameter.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/system_parameter.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/translations.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/translations.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/users.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/users.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/apps/website.py` & `odoo-configurator-3.4.5/src/odoo_configurator/apps/website.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/bitwarden.py` & `odoo-configurator-3.4.5/src/odoo_configurator/bitwarden.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/configurator.py` & `odoo-configurator-3.4.5/src/odoo_configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/import_manager.py` & `odoo-configurator-3.4.5/src/odoo_configurator/import_manager.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/keepass.py` & `odoo-configurator-3.4.5/src/odoo_configurator/keepass.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator/odoo_connection.py` & `odoo-configurator-3.4.5/src/odoo_configurator/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator.egg-info/PKG-INFO` & `odoo-configurator-3.4.5/src/odoo_configurator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-configurator
-Version: 3.4.4
+Version: 3.4.5
 Summary: Configure and update Odoo database with YAML files
 Author-email: Michel Perrocheau <myrrkel@gmail.com>, David Halgand <david@scalizer.fr>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -166,14 +166,15 @@
           If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
         
 Project-URL: Homepage, https://github.com/ScalizerOrg/odoo-configurator
+Project-URL: Changelog, https://github.com/ScalizerOrg/odoo-configurator/CHANGELOG.md
 Keywords: odoo,configurator,xmlprc,yaml
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Odoo
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `odoo-configurator-3.4.4/src/odoo_configurator.egg-info/SOURCES.txt` & `odoo-configurator-3.4.5/src/odoo_configurator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/templates/1_base_auto_entreprise.yml` & `odoo-configurator-3.4.5/src/templates/1_base_auto_entreprise.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/templates/2_base_account.yml` & `odoo-configurator-3.4.5/src/templates/2_base_account.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/templates/2_base_account_14.yml` & `odoo-configurator-3.4.5/src/templates/2_base_account_14.yml`

 * *Files identical despite different names*

### Comparing `odoo-configurator-3.4.4/src/templates/2_base_sale.yml` & `odoo-configurator-3.4.5/src/templates/2_base_sale.yml`

 * *Files identical despite different names*

