# Comparing `tmp/dsms_sdk-1.3.3.tar.gz` & `tmp/dsms_sdk-1.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.3.3.tar", last modified: Thu Apr  4 10:06:06 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc0.tar", last modified: Fri Apr 12 08:33:16 2024, max compression
```

## Comparing `dsms_sdk-1.3.3.tar` & `dsms_sdk-1.4.0rc0.tar`

### file list

```diff
@@ -1,54 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.702700 dsms_sdk-1.3.3/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.706700 dsms_sdk-1.3.3/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/custom_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/properties/user_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.706700 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13099 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 10:06:06.000000 dsms_sdk-1.3.3/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 10:06:06.710700 dsms_sdk-1.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-04 10:05:58.000000 dsms_sdk-1.3.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.895386 dsms_sdk-1.4.0rc0/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7569 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16347 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.899386 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/properties/user_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16663 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-12 08:33:16.000000 dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-12 08:33:16.907386 dsms_sdk-1.4.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:16.903386 dsms_sdk-1.4.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-12 08:33:11.000000 dsms_sdk-1.4.0rc0/tests/test_utils.py
```

### Comparing `dsms_sdk-1.3.3/LICENSE` & `dsms_sdk-1.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/PKG-INFO` & `dsms_sdk-1.4.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.3.3
+Version: 1.4.0rc0
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: html5lib<2,>=1
+Requires-Dist: lru-cache<1
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic>=2
 Requires-Dist: pydantic-settings
+Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: pre-commit
 Requires-Dist: pre-commit==3.3.2; extra == "pre-commit"
```

### Comparing `dsms_sdk-1.3.3/README.md` & `dsms_sdk-1.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc0/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc0/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/core/context.py` & `dsms_sdk-1.4.0rc0/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc0/dsms/core/dsms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """DSMS connection module"""
 
+import os
 from typing import TYPE_CHECKING, Any, Dict, List
 
+from dotenv import load_dotenv
+
 from dsms.apps.utils import _get_available_apps
 from dsms.core.configuration import Configuration
 from dsms.core.context import Context
 from dsms.core.utils import _ping_dsms
 from dsms.knowledge.sparql_interface import SparqlInterface
 from dsms.knowledge.utils import _search
 
@@ -23,24 +26,64 @@
     from dsms.apps import App
     from dsms.core.context import Buffers
     from dsms.knowledge.kitem import KItem
     from dsms.knowledge.ktype import KType
 
 
 class DSMS:
-    """General class for connecting and interfacting with DSMS."""
+    """
+    General class for connecting and interfacing with DSMS.
+
+    This class provides methods to connect to and interact with a DSMS (Data
+    Space Management System) instance. It abstracts away the complexities of
+    establishing connections and executing queries.
+
+    Args:
+        config (Configuration, optional): An optional Configuration object
+            containing connection details. If not provided, default
+            configurations will be used.
+        env (str, optional): An optional string representing the path to the env-file.
+            This can be used to select environment-specific configurations. Defaults to None.
+        **kwargs: Configurations can also be set as additional keyword arguments instead of
+            passing the path to an env-file or the Configuration-object itself.
+
+    """
 
     _context = Context
 
-    def __init__(self, config: Configuration = None, **kwargs) -> None:
-        """Initialize the DSMS object."""
+    def __init__(
+        self,
+        config: "Optional[Configuration]" = None,
+        env: "Optional[str]" = None,
+        **kwargs,
+    ) -> None:
+        """Initialize the DSMS object.
+        Args:
+            config (Configuration, optional): An optional Configuration object
+                containing connection details. If not provided, default
+                configurations will be used.
+            env (str, optional): An optional string representing the path to the env-file.
+                This can be used to select environment-specific configurations. Content
+                of the env-file will be safely loaded using `python-dotenv`.
+                Hence the env-variables will be pruned once the kernel is closed.
+                Defaults to None.
+            **kwargs: Configurations can also be set as additional keyword arguments instead of
+                passing the path to an env-file or the Configuration-object itself.
+        """
 
         self._config = None
         self._context.dsms = self
 
+        if env:
+            if not os.path.exists(env):
+                raise OSError(f"File `{env}` does not exist")
+            loaded = load_dotenv(env, verbose=True)
+            if not loaded:
+                raise RuntimeError(f"Not able to parse .env file: {env}")
+
         if config is not None and not kwargs:
             self.config = config
         elif config is None:
             self.config = Configuration(**kwargs)
         else:
             raise ValueError(
                 """`config`-keyword is defined among others.
```

### Comparing `dsms_sdk-1.3.3/dsms/core/utils.py` & `dsms_sdk-1.4.0rc0/dsms/core/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Core utils of the DSMS core"""
 import re
-from typing import Any
+from importlib import import_module
+from typing import TYPE_CHECKING
 from urllib.parse import urljoin
 from uuid import UUID
 
 import requests
 from requests import Response
 
+if TYPE_CHECKING:
+    from typing import Any, Callable
+
 
 def _kitem_id2uri(kitem_id: UUID) -> str:
     "Convert a kitem id in the DSMS to the full resolvable URI"
     from dsms import Context
 
     return urljoin(str(Context.dsms.config.host_url), str(kitem_id))
 
@@ -23,15 +27,15 @@
 
 
 def _ping_dsms():
     """General check if the remote DSMS instance is up and running"""
     return _perform_request("api/knowledge/docs", "get")
 
 
-def _perform_request(route: str, method: str, **kwargs: Any) -> Response:
+def _perform_request(route: str, method: str, **kwargs: "Any") -> Response:
     """Perform a general request for a certain route and with a certain method.
     Kwargs are general arguments which can be passed to the `requests.request`-function.
     """
     from dsms import Context
 
     dsms = Context.dsms
     response = requests.request(
@@ -59,7 +63,13 @@
 
 def _name_to_camel(input_string):
     """Remove special characters and make a CamelCased-str"""
     words = re.findall(r"\w+", input_string)
     camel_case_words = [word.title() for word in words]
     camel_case_string = "".join(camel_case_words)
     return camel_case_string
+
+
+def get_callable(module: str) -> "Callable":
+    """Get callable from import-specification"""
+    module, classname = module.strip().split(":")
+    return getattr(import_module(module), classname)
```

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/kitem.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Knowledge Item implementation of the DSMS"""
 
+import json
 from datetime import datetime
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 from urllib.parse import urljoin
 from uuid import UUID, uuid4
 
 import pandas as pd
@@ -11,14 +12,15 @@
 
 from pydantic import (  # isort:skip
     BaseModel,
     ConfigDict,
     Field,
     ValidationInfo,
     field_validator,
+    model_validator,
 )
 
 
 from dsms.knowledge.properties import (  # isort:skip
     Affiliation,
     AffiliationsProperty,
     Annotation,
@@ -27,15 +29,14 @@
     AppsProperty,
     Attachment,
     AttachmentsProperty,
     Author,
     AuthorsProperty,
     ContactInfo,
     ContactsProperty,
-    CustomProperties,
     ExternalLink,
     ExternalLinksProperty,
     KProperty,
     HDF5Container,
     Column,
     LinkedKItem,
     LinkedKItemsProperty,
@@ -47,30 +48,70 @@
 from dsms.knowledge.ktype import KType  # isort:skip
 
 from dsms.knowledge.utils import (  # isort:skip
     _kitem_exists,
     _slug_is_available,
     _slugify,
     _inspect_hdf5,
+    _get_ktype_from_id,
 )
 
 from dsms.knowledge.sparql_interface.utils import _get_subgraph  # isort:skip
 
 if TYPE_CHECKING:
     from dsms import Context
     from dsms.core.dsms import DSMS
 
 
 class KItem(BaseModel):
-    """Knowledge Item of the DSMS."""
+    """
+    Knowledge Item of the DSMS.
+
+    Attributes:
+        name (str):
+            Human readable name of the KContext.dsms.
+        id (Optional[UUID]):
+            ID of the KItem. Defaults to a new UUID if not provided.
+        ktype_id (Union[Enum, str]):
+            Type ID of the KItem.
+        slug (Optional[str]):
+            Slug of the KContext.dsms. Minimum length: 4.
+        annotations (List[Annotation]):
+            Annotations of the KItem.
+        attachments (List[Union[Attachment, str]]):
+            File attachments of the DSMS.
+        linked_kitems (List[Union[LinkedKItem, "KItem"]]):
+            KItems linked to the current KItem.
+        affiliations (List[Affiliation]):
+            Affiliations related to a KItem.
+        authors (List[Union[Author, str]]):
+            Authorship of the KItem.
+        avatar_exists (Optional[bool]):
+            Whether the KItem holds an avatar or not.
+        contacts (List[ContactInfo]):
+            Contact information related to the KItem.
+        created_at (Optional[Union[str, datetime]]):
+            Time and date when the KItem was created.
+        updated_at (Optional[Union[str, datetime]]):
+            Time and date when the KItem was updated.
+        external_links (List[ExternalLink]):
+            External links related to the KItem.
+        kitem_apps (List[App]): Apps related to the KItem.
+        summary (Optional[Union[str, Summary]]):
+            Human readable summary text of the KItem.
+        user_groups (List[UserGroup]):
+                User groups able to access the KItem.
+        custom_properties (Optional[Any]):
+            Custom properties associated with the KItem.
+        hdf5 (Optional[Union[List[Column], pd.DataFrame, Dict[str, Union[List, Dict]]]]):
+            HDF5 interface.
+    """
 
     # public
-    name: str = Field(
-        ..., description="Human readable name of the KContext.dsms"
-    )
+    name: str = Field(..., description="Human readable name of the KItem")
     id: Optional[UUID] = Field(
         default_factory=uuid4,
         description="ID of the KItem",
     )
     ktype_id: Union[Enum, str] = Field(..., description="Type ID of the KItem")
     slug: Optional[str] = Field(
         None, description="Slug of the KContext.dsms", min_length=4
@@ -141,15 +182,15 @@
         """Initialize the KItem"""
         from dsms import DSMS
 
         # set dsms instance if not already done
         if not self.dsms:
             self.dsms = DSMS()
 
-        # initalize the kitem
+        # initialize the kitem
         super().__init__(**kwargs)
 
         # add kitem to buffer
         if (
             not _kitem_exists(self)
             and self.id not in self.context.buffers.created
         ):
@@ -294,29 +335,14 @@
     @classmethod
     def validate_user_groups(
         cls, value: List[UserGroup]
     ) -> UserGroupsProperty:
         """Validate user groups Field"""
         return UserGroupsProperty(value)
 
-    @field_validator("custom_properties")
-    @classmethod
-    def validate_custom_properties(cls, value: Any) -> CustomProperties:
-        """Validate custom properties Field"""
-        if isinstance(value, dict) and "content" in value:
-            value = CustomProperties(content=value["content"])
-        elif isinstance(value, dict):
-            value = CustomProperties(content=value)
-        elif not isinstance(value, (CustomProperties, dict, type(None))):
-            raise TypeError(
-                f"""`custom_properties` must be of type {CustomProperties} or {dict},
-                not {type(value)}."""
-            )
-        return value
-
     @field_validator("created_at")
     @classmethod
     def validate_created(cls, value: str) -> Any:
         """Convert the str for `created_at` in to a `datetime`-object"""
         from dsms import Context
 
         if isinstance(value, str):
@@ -337,28 +363,18 @@
             )
         return value
 
     @field_validator("ktype")
     @classmethod
     def validate_ktype(cls, value: KType, info: ValidationInfo) -> KType:
         """Validate the data attribute of the KItem"""
-        from dsms import Context
-
-        ktype_id = info.data.get("ktype_id")
 
         if not value:
-            if not isinstance(ktype_id, str):
-                value = Context.ktypes.get(ktype_id.value)
-            else:
-                value = Context.ktypes.get(ktype_id)
-
-            if not value:
-                raise TypeError(
-                    f"KType for `ktype_id={ktype_id}` does not exist."
-                )
+            ktype_id = info.data.get("ktype_id")
+            value = _get_ktype_from_id(ktype_id)
 
         return value
 
     @field_validator("slug")
     @classmethod
     def validate_slug(cls, value: str, info: ValidationInfo) -> str:
         """Validate slug"""
@@ -412,23 +428,49 @@
             columns = _inspect_hdf5(kitem_id)
             if columns:
                 hdf5 = HDF5Container([Column(**column) for column in columns])
             else:
                 hdf5 = None
         return hdf5
 
+    @model_validator(mode="after")
+    @classmethod
+    def validate_custom_properties(cls, self) -> "KItem":
+        """Validate the custom properties with respect to the KType of the KItem"""
+        if not isinstance(
+            self.custom_properties, (BaseModel, dict, type(None))
+        ):
+            raise TypeError(
+                f"""Custom properties must be one of the following types:
+                  {(BaseModel, dict, type(None))}. Not {type(self.custom_properties)}"""
+            )
+        # validate content with webform model
+        if self.ktype.webform and isinstance(self.custom_properties, dict):
+            content = (
+                self.custom_properties.get("content") or self.custom_properties
+            )
+            if isinstance(content, str):
+                try:
+                    content = json.loads(content)
+                except Exception as error:
+                    raise TypeError(
+                        f"Invalid type: {type(content)}"
+                    ) from error
+            self.custom_properties = self.ktype.webform(**content)
+        # set kitem id for custom properties
+        if isinstance(self.custom_properties, BaseModel):
+            self.custom_properties.kitem = self
+        return self
+
     def _set_kitem_for_properties(self) -> None:
         """Set kitem for CustomProperties and KProperties in order to
         remain the context for the buffer if any of these properties is changed.
         """
         for prop in self.__dict__.values():
-            if (
-                isinstance(prop, (KProperty, CustomProperties, Summary))
-                and not prop.kitem
-            ):
+            if isinstance(prop, (KProperty, Summary)) and not prop.kitem:
                 prop.kitem = self
 
     @property
     def dsms(cls) -> "DSMS":
         """DSMS context getter"""
         return cls.context.dsms
```

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Annotation,
     AnnotationsProperty,
 )
 from dsms.knowledge.properties.apps import App, AppsProperty
 from dsms.knowledge.properties.authors import Author, AuthorsProperty
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
 from dsms.knowledge.properties.contacts import ContactInfo, ContactsProperty
-from dsms.knowledge.properties.custom_properties import CustomProperties
+from dsms.knowledge.properties.custom_datatype import NumericalDataType
 from dsms.knowledge.properties.hdf5 import Column, HDF5Container
 from dsms.knowledge.properties.summary import Summary
 from dsms.knowledge.properties.user_groups import UserGroup, UserGroupsProperty
 
 from dsms.knowledge.properties.attachments import (  # isort:skip
     Attachment,
     AttachmentsProperty,
@@ -29,23 +29,21 @@
 )
 
 from dsms.knowledge.properties.external_links import (  # isort:skip
     ExternalLink,
     ExternalLinksProperty,
 )
 
-
 __all__ = [
     "Annotation",
     "AnnotationsProperty",
     "Attachment",
     "AttachmentsProperty",
     "Author",
     "AuthorsProperty",
-    "CustomProperties",
     "LinkedKItem",
     "LinkedKItemsProperty",
     "ContactInfo",
     "ContactsProperty",
     "ExternalLinksProperty",
     "ExternalLink",
     "AppsProperty",
@@ -55,8 +53,9 @@
     "UserGroupsProperty",
     "UserGroup",
     "Summary",
     "KProperty",
     "KPropertyItem",
     "HDF5Container",
     "Column",
+    "NumericalDataType",
 ]
```

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/affiliations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/annotations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/attachments.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/authors.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/contacts.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/custom_properties.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/hdf5.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,125 +1,120 @@
-"""Custom properties of a KItem"""
+"""HDF5 Properties of a KItem"""
+from typing import TYPE_CHECKING
 
-
-from typing import TYPE_CHECKING, Any, Optional
-from uuid import UUID
-
-from pydantic import BaseModel, ConfigDict, Field, model_validator
+import numpy as np
+import pandas as pd
+from pydantic import Field
+
+from dsms.knowledge.properties.base import KProperty, KPropertyItem
+from dsms.knowledge.utils import _get_hdf5_column
+
+from dsms.knowledge.semantics.units import (  # isort:skip
+    get_conversion_factor,
+    get_property_unit,
+)
 
 if TYPE_CHECKING:
-    from typing import Set, Union
+    from typing import Any, Callable, Dict, List, Optional
 
-    from dsms import Context, KItem
 
+class Column(KPropertyItem):
+    """
+    Column of an HDF5 data frame.
 
-class CustomProperties(BaseModel):
-    """Model for the custom properties of the KItem"""
+    Attributes:
+        column_id (int): Column ID in the data frame.
+        name (str): Name of the column in the data series.
+    """
 
-    id: Optional[UUID] = Field(None, description="ID of the KItem")
-    content: Any = Field({}, description="Constent of the custom kitem")
-    kitem: Optional[Any] = Field(
-        None, description="KItem related to the CustomProperties", exclude=True
-    )
+    column_id: int = Field(..., description="Column ID in the data frame")
 
-    model_config = ConfigDict(
-        extra="forbid", exclude={"kitem", "id"}, validate_assignment=True
+    name: str = Field(
+        ..., description="Name of the column in the data series."
     )
 
-    def __str__(self) -> str:
-        """Pretty print the custom properties"""
-        fields = ", ".join(
-            [
-                f"{key}={value}"
-                for key, value in self.__dict__.items()
-                if key not in self.exclude
-            ]
+    def get(self) -> "List[Any]":
+        """
+        Download the data for the column in a time series.
+
+        Returns:
+            List[Any]: List of data for the column.
+        """
+        return _get_hdf5_column(self.id, self.column_id)
+
+    def get_unit(self) -> "Dict[str, Any]":
+        """
+        Retrieve the unit of the column.
+
+        Returns:
+            Dict[str, Any]: Dictionary containing unit information.
+        """
+        return get_property_unit(self.id, self.name, is_hdf5_column=True)
+
+    def convert_to(
+        self,
+        unit_symbol_or_iri: str,
+        decimals: "Optional[int]" = None,
+        use_input_iri: bool = False,
+    ) -> "List[Any]":
+        """
+        Convert the data of the column to a different unit.
+
+        Args:
+            unit_symbol_or_iri (str): Symbol or IRI of the unit to convert to.
+            decimals (Optional[int]): Number of decimals to round the result to. Defaults to None.
+            use_input_iri (bool): If True, use IRI for unit comparison. Defaults to False.
+
+        Returns:
+            List[Any]: List of converted data.
+        """
+        unit = self.get_unit()
+        if use_input_iri:
+            input_str = unit.get("iri")
+        else:
+            input_str = unit.get("symbol")
+        factor = get_conversion_factor(
+            input_str, unit_symbol_or_iri, decimals=decimals
         )
-        return f"{self.__class__.__name__}({fields})"
+        data = self.get()
+        return list(np.array(data) * factor)
 
-    def __repr__(self) -> str:
-        """Pretty print the custom properties"""
-        return str(self)
-
-    def __hash__(self) -> int:
-        return hash(str(self))
-
-    def add(self, content: "Union[dict, Any]") -> None:
-        """Add data for custom properties"""
-        if isinstance(content, type(None)):
-            self.content = {}
-        elif self.data_schema and isinstance(content, dict):
-            self.content = self.data_schema(content)
-        elif not self.data_schema and isinstance(content, dict):
-            self.content = content
-        elif self.data_schema:
-            if isinstance(content, self.data_schema):
-                self.content = content
-            else:
-                raise TypeError(
-                    f"""Item `{content}` must be of type {self.data_schema} or {dict},
-                    not `{type(content)}`."""
-                )
-        else:
-            raise TypeError(
-                f"""Item `{content}` must be of type {self.data_schema} or {dict},
-                not `{type(content)}`."""
-            )
-        self._mark_as_updated()
-
-    def _mark_as_updated(self) -> None:
-        if self.kitem and self.id not in self.context.buffers.updated:
-            self.context.buffers.updated.update({self.id: self.kitem})
-
-    def delete(self) -> None:
-        """Delete data for custom properties"""
-        self.content = None
-        self._mark_as_updated()
-
-    def update(self, content: "Union[dict, Any]") -> None:
-        """Update data for custom properties"""
-        self.content = None
-        self.add(content)
-
-    def get(self) -> Any:
-        """Get data for custom properties"""
-        return self.content
-
-    @model_validator(mode="before")
-    @classmethod
-    def validate_kitem(cls, data: Any) -> "KItem":
-        """Validate the custom properties with respect to the KType of the KItem"""
-        kitem = data.get("kitem")
-        content = data.get("content")
-        if kitem:
-            data["id"] = kitem.id
-            if kitem.ktype.data_schema:
-                data["content"] = kitem.ktype.data_schema(**content)
-        return data
 
-    @property
-    def id(cls) -> Optional[UUID]:
-        """Identifier of the KItem related to the CustomProperies"""
-        if not cls.kitem:
-            raise ValueError("KItem not defined yet.")
-        return cls.kitem.id  # pylint: disable=E1101
+class HDF5Container(KProperty):
+    """HDF5 container of a data frame related to a KItem"""
 
+    # OVERRIDE
     @property
-    def data_schema(cls):
-        """Data schema related to the ktype of the associated kitem."""
-        if not cls.kitem:
-            raise ValueError("KItem not defined yet.")
-        return cls.kitem.ktype.data_schema  # pylint: disable=E1101
+    def k_property_item(cls) -> "Callable":
+        return Column
 
-    @property
-    def context(cls) -> "Context":
-        """Getter for Context"""
-        from dsms import (  # isort:skip
-            Context,
-        )
-
-        return Context
-
-    @property
-    def exclude(cls) -> "Optional[Set[str]]":
-        """Fields to be excluded from the JSON-schema"""
-        return cls.model_config.get("exclude")
+    # OVERRIDE
+    def _add(self, item: Column) -> Column:
+        """Side effect when an Column is added to the KProperty"""
+        return item
+
+    # OVERRIDE
+    def _update(self, item: Column) -> Column:
+        """Side effect when an Column is updated at the KProperty"""
+        return item
+
+    # OVERRIDE
+    def _delete(self, item: Column) -> None:
+        """Side effect when deleting the Column of a KItem"""
+
+    # OVERRIDE
+    def _get(self, item: Column) -> Column:
+        """Side effect when getting the Column for a specfic kitem"""
+        return item
+
+    def to_df(self) -> pd.DataFrame:
+        """Return hdf5 as pandas DataFrame"""
+        data = {column.name: column.get() for column in self}
+        return pd.DataFrame.from_dict(data)
+
+    def get(self, name: str) -> "Optional[Column]":
+        """Get a column with a certain name."""
+        response = None
+        for column in self:
+            if column.name == name:
+                response = column
+        return response
```

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/external_links.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/external_links.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/user_groups.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,45 @@
-"""HDF5 Properties of a KItem"""
+"""UserGroup KProperty"""
+
 from typing import TYPE_CHECKING
 
-import pandas as pd
 from pydantic import Field
 
 from dsms.knowledge.properties.base import KProperty, KPropertyItem
-from dsms.knowledge.utils import _get_hdf5_column
 
 if TYPE_CHECKING:
-    from typing import Any, Callable, List
-
+    from typing import Callable
 
-class Column(KPropertyItem):
-    """Column of an HDF5 data frame"""
 
-    column_id: int = Field(..., description="Column ID in the data frame")
+class UserGroup(KPropertyItem):
+    """Users groups related to a KItem."""
 
-    name: str = Field(
-        ..., description="Name of the column in the data series."
-    )
+    name: str = Field(..., description="Name of the user group")
+    group_id: str = Field(..., description="ID of the user group")
 
-    def get(self) -> "List[Any]":
-        """Download the data for the column in a time series"""
-        return _get_hdf5_column(self.id, self.column_id)
 
+class UserGroupsProperty(KProperty):
+    """KProperty for user_groups"""
 
-class HDF5Container(KProperty):
-    """HDF5 container of a data frame related to a KItem"""
-
-    # OVERRIDE
     @property
     def k_property_item(cls) -> "Callable":
-        return Column
+        """UserGroup data model"""
+        return UserGroup
 
     # OVERRIDE
-    def _add(self, item: Column) -> Column:
-        """Side effect when an Column is added to the KProperty"""
+    def _add(self, item: UserGroup) -> UserGroup:
+        """Side effect when an UserGroup is added to the KProperty"""
         return item
 
     # OVERRIDE
-    def _update(self, item: Column) -> Column:
-        """Side effect when an Column is updated at the KProperty"""
+    def _update(self, item: UserGroup) -> UserGroup:
+        """Side effect when an UserGroup is updated at the KProperty"""
         return item
 
     # OVERRIDE
-    def _delete(self, item: Column) -> None:
-        """Side effect when deleting the Column of a KItem"""
-
-    # OVERRIDE
-    def _get(self, item: Column) -> Column:
-        """Side effect when getting the Column for a specfic kitem"""
+    def _get(self, item: UserGroup) -> UserGroup:
+        """Side effect when getting the UserGroup for a specfic kitem"""
         return item
 
-    def to_df(self) -> pd.DataFrame:
-        """Return hdf5 as pandas DataFrame"""
-        data = {column.name: column.get() for column in self}
-        return pd.DataFrame.from_dict(data)
+    # OVERRIDE
+    def _delete(self, item: UserGroup) -> None:
+        """Side effect when deleting the UserGroup of a KItem"""
```

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/linked_kitems.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.3.3/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc0/dsms/knowledge/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,167 @@
 """DSMS knowledge utilities"""
 import io
 import json
 import re
+import warnings
 from enum import Enum
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 from uuid import UUID
 
 import pandas as pd
-from pydantic import BaseModel, create_model
 from requests import Response
 
-from dsms.core.utils import _name_to_camel, _perform_request
+from pydantic import (  # isort: skip
+    BaseModel,
+    ConfigDict,
+    Field,
+    create_model,
+    model_validator,
+)
+
+from dsms.core.utils import _name_to_camel, _perform_request  # isort:skip
+
+from dsms.knowledge.properties.custom_datatype import (  # isort:skip
+    NumericalDataType,
+)
 
 if TYPE_CHECKING:
     from dsms.core.context import Buffers
     from dsms.knowledge import KItem, KType
 
 
-def _parse_model(value: Dict[str, Any]) -> BaseModel:
+def _is_number(value):
+    try:
+        float(value)
+        return True
+    except Exception:
+        return False
+
+
+def _create_custom_properties_model(
+    value: Optional[Dict[str, Any]]
+) -> BaseModel:
     """Convert the dict with the model schema into a pydantic model."""
-    title = value.get("title")
-    properties = value.get("properties")
-    if not title:
-        raise KeyError("`data_schema` does not have any `title`.")
-    if isinstance(properties, type(None)):
-        raise KeyError("`data_schema` does not have any `properties`.")
+    from dsms import KItem
+
     fields = {}
-    for key, props in properties.items():
-        dtype = props.get("type")
-        default = props.get("default")
-        if dtype == "string":
-            dtype = str
-        elif dtype == "integer":
-            dtype = int
-        elif dtype == "float":
-            dtype = float
-        elif dtype == "bool":
-            dtype = bool
-        elif dtype == "object":
-            dtype = dict
-        else:
-            raise TypeError(f"Invalid `type={dtype}`")
-        fields[key] = (dtype, ... if not default else default)
-    return create_model(title, **fields)
+    if isinstance(value, dict):
+        title = _name_to_camel(value.get("title"))
+        for item in value.get("objects"):
+            for form_input in item.get("inputs"):
+                label = form_input.get("label")
+                dtype = form_input.get("widget")
+                default = form_input.get("defaultValue")
+                slug = _slugify(label)
+                if dtype in ("text", "file"):
+                    dtype = str
+                elif dtype in ("number", "slider"):
+                    dtype = NumericalDataType
+                elif dtype == "checkbox":
+                    dtype = bool
+                elif dtype in ("select", "radio"):
+                    dtype = Enum(
+                        _name_to_camel(label) + "Choices",
+                        {
+                            _name_to_camel(choice["value"]): choice["value"]
+                            for choice in form_input.get("choices")
+                        },
+                    )
+                elif dtype == "knowledge-select":
+                    warnings.warn(
+                        "knowledge-select not fully supported for KTypes yet."
+                    )
+                    dtype = str
+                fields[slug] = (dtype, default or None)
+    else:
+        title = "CustomPropertiesModel"
+    fields["kitem"] = (
+        Optional[KItem],
+        Field(None, exclude=True),
+    )
+
+    config = ConfigDict(
+        extra="allow", arbitrary_types_allowed=True, exclude={"kitem"}
+    )
+    validators = {
+        "validate_model": model_validator(mode="before")(_validate_model)
+    }
+    model = create_model(
+        title, __config__=config, __validators__=validators, **fields
+    )
+    setattr(model, "__str__", _print_properties)
+    setattr(model, "__repr__", _print_properties)
+    setattr(model, "__setattr__", __setattr_property__)
+    return model
+
+
+def _print_properties(self: Any) -> str:
+    fields = ", \n".join(
+        [
+            f"\t\t{key}={value}"
+            for key, value in self.model_dump().items()
+            if key not in self.model_config["exclude"]
+        ]
+    )
+    return f"{{\n{fields}\n\t\t}}"
+
+
+def __setattr_property__(self, key, value) -> None:
+    if _is_number(value):
+        # convert to convertable numeric object
+        value = _create_numerical_dtype(key, value, self.kitem)
+        # mark as updated
+        if self.kitem:
+            self.kitem.context.buffers.updated.update(
+                {self.kitem.id: self.kitem}
+            )
+    if key == "kitem":
+        # set kitem for convertable numeric datatype
+        for prop in self.model_dump().values():
+            if isinstance(prop, NumericalDataType) and not prop.kitem:
+                prop.kitem = value
+    # reassignment of extra fields does not work, seems to be a bug?
+    # have this workaround:
+    if key in self.__pydantic_extra__:
+        self.__pydantic_extra__[key] = value
+    super(BaseModel, self).__setattr__(key, value)
+
+
+def _create_numerical_dtype(
+    key: str, value: Union[int, float], kitem: "KItem"
+) -> NumericalDataType:
+    value = NumericalDataType(value)
+    value.name = key
+    value.kitem = kitem
+    return value
+
+
+def _validate_model(
+    cls, values: Dict[str, Any]  # pylint: disable=unused-argument
+) -> Dict[str, Any]:
+    for key, value in values.items():
+        if _is_number(value):
+            values[key] = _create_numerical_dtype(
+                key, value, values.get("kitem")
+            )
+    return values
+
+
+def _get_ktype_from_id(ktype_id: str) -> "KType":
+    from dsms import Context
+
+    if not isinstance(ktype_id, str):
+        value = Context.ktypes.get(ktype_id.value)
+    else:
+        value = Context.ktypes.get(ktype_id)
+
+    if not value:
+        raise TypeError(f"KType for `ktype_id={ktype_id}` does not exist.")
+    return value
 
 
 def _get_remote_ktypes() -> Enum:
     """Get the KTypes from the remote backend"""
     from dsms import (  # isort:skip
         Context,
         KType,
@@ -128,30 +242,34 @@
     """Update a KItem in the remote backend."""
     old_kitem = _get_kitem(kitem.id)
     differences = _get_kitems_diffs(old_kitem, kitem)
     dumped = kitem.model_dump_json(
         exclude={
             "authors",
             "annotations",
+            "custom_properties",
             "linked_kitems",
             "updated_at",
             "avatar_exists",
             "user_groups",
             "ktype_id",
             "attachments",
             "id",
             "kitem_apps",
             "created_at",
             "external_links",
             "hdf5",
         },
         exclude_none=True,
     )
+    custom_properties = kitem.custom_properties.model_dump_json()
     payload = json.loads(dumped)
-    payload.update(**differences)
+    payload.update(
+        custom_properties={"content": custom_properties}, **differences
+    )
     payload.update(
         external_links={
             link.label: str(link.url) for link in kitem.external_links
         }
     )
     response = _perform_request(
         f"api/knowledge/kitems/{kitem.id}", "put", json=payload
@@ -331,18 +449,18 @@
     except Exception as excep:
         raise RuntimeError(
             f"""Something went wrong while searching for KItems: {response.text}"""
         ) from excep
     return [KItem(**item) for item in dumped]
 
 
-def _slugify(input_string):
+def _slugify(input_string: str, replacement: str = ""):
     """Turn any arbitrary string into a slug."""
     slug = re.sub(
-        r"[^\w\s]", "", input_string
+        r"[^\w\s]", replacement, input_string
     )  # Remove all non-word characters (everything except numbers and letters)
     slug = re.sub(r"\s+", "", slug)  # Replace all runs of whitespace
     slug = slug.lower()  # Convert the string to lowercase.
     return slug
 
 
 def _slug_is_available(ktype_id: Union[str, UUID], value: str) -> bool:
```

### Comparing `dsms_sdk-1.3.3/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.3.3
+Version: 1.4.0rc0
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: html5lib<2,>=1
+Requires-Dist: lru-cache<1
 Requires-Dist: pandas<3,>=2
 Requires-Dist: pydantic>=2
 Requires-Dist: pydantic-settings
+Requires-Dist: python-dotenv
 Requires-Dist: rdflib<7,>=6
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: bumpver==2021.1114; extra == "dev"
 Requires-Dist: dunamai==1.7.0; extra == "dev"
 Provides-Extra: pre-commit
 Requires-Dist: pre-commit==3.3.2; extra == "pre-commit"
```

### Comparing `dsms_sdk-1.3.3/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc0/dsms_sdk.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,20 +19,29 @@
 dsms/knowledge/properties/affiliations.py
 dsms/knowledge/properties/annotations.py
 dsms/knowledge/properties/apps.py
 dsms/knowledge/properties/attachments.py
 dsms/knowledge/properties/authors.py
 dsms/knowledge/properties/base.py
 dsms/knowledge/properties/contacts.py
-dsms/knowledge/properties/custom_properties.py
 dsms/knowledge/properties/external_links.py
 dsms/knowledge/properties/hdf5.py
 dsms/knowledge/properties/linked_kitems.py
 dsms/knowledge/properties/summary.py
 dsms/knowledge/properties/user_groups.py
+dsms/knowledge/properties/custom_datatype/__init__.py
+dsms/knowledge/properties/custom_datatype/numerical.py
+dsms/knowledge/semantics/__init__.py
+dsms/knowledge/semantics/queries/__init__.py
+dsms/knowledge/semantics/queries/base.py
+dsms/knowledge/semantics/units/__init__.py
+dsms/knowledge/semantics/units/base.py
+dsms/knowledge/semantics/units/conversion.py
+dsms/knowledge/semantics/units/sparql.py
+dsms/knowledge/semantics/units/utils.py
 dsms/knowledge/sparql_interface/__init__.py
 dsms/knowledge/sparql_interface/sparql_interface.py
 dsms/knowledge/sparql_interface/subgraph.py
 dsms/knowledge/sparql_interface/utils.py
 dsms_sdk.egg-info/PKG-INFO
 dsms_sdk.egg-info/SOURCES.txt
 dsms_sdk.egg-info/dependency_links.txt
```

### Comparing `dsms_sdk-1.3.3/setup.cfg` & `dsms_sdk-1.4.0rc0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.3.3
+version = v1.4.0rc0
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
@@ -15,17 +15,20 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
+	html5lib>=1,<2
+	lru-cache<1
 	pandas>=2,<3
 	pydantic>=2
 	pydantic-settings
+	python-dotenv
 	rdflib>=6,<7
 	requests
 python_requires = >=3.8
 include_package_data = True
 
 [options.extras_require]
 dev =
```

### Comparing `dsms_sdk-1.3.3/tests/conftest.py` & `dsms_sdk-1.4.0rc0/tests/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import TYPE_CHECKING
 from urllib.parse import urljoin
 
 import pytest
 import responses
 
 if TYPE_CHECKING:
-    from typing import Any, Dict
+    from typing import Any, Dict, List
 
 
 class MockDB:
     """Mock database"""
 
     kitems = {
         "78dfd0c7-0348-412c-8eb6-c91a4d340477": {
@@ -63,27 +63,32 @@
         kitems: [
             {"method": responses.GET, "returns": {"status": 200, "json": {}}}
         ],
     }
 
 
 @pytest.fixture(scope="function")
+def passthru() -> "List[str]":
+    return [
+        "https://qudt.org/2.1/vocab/unit",
+        "http://qudt.org/2.1/vocab/unit",
+        "http://qudt.org/vocab/quantitykind",
+        "https://qudt.org/vocab/quantitykind",
+    ]
+
+
+@pytest.fixture(scope="function")
 def mock_callbacks(custom_address) -> "Dict[str, Any]":
     ktypes = urljoin(custom_address, "api/knowledge-type/")
 
     def return_ktypes(request):
         ktypes = [
             {
                 "name": "organization",
                 "id": "organization",
-                "data_schema": {
-                    "title": "Organization",
-                    "type": "object",
-                    "properties": {},
-                },
             },
         ]
         header = {"content_type": "application/json"}
         return (200, header, json.dumps(ktypes))
 
     def return_kitems(request):
         # Extract 'id' parameter from the URL
@@ -149,15 +154,19 @@
         ],
         **_get_kitems(),
         **_get_hdf5(),
     }
 
 
 @pytest.fixture(autouse=True, scope="function")
-def register_mocks(mock_responses, mock_callbacks, custom_address) -> str:
+def register_mocks(
+    mock_responses, mock_callbacks, passthru, custom_address
+) -> str:
+    for url in passthru:
+        responses.add_passthru(url)
     for url, endpoints in mock_responses.items():
         for response in endpoints:
             responses.add(
                 response["method"],
                 url,
                 **response["returns"],
             )
```

### Comparing `dsms_sdk-1.3.3/tests/test_kitem.py` & `dsms_sdk-1.4.0rc0/tests/test_kitem.py`

 * *Files 18% similar despite different names*

```diff
@@ -155,7 +155,38 @@
     kitem = KItem(
         id=get_mock_kitem_ids[0],
         name="foo123",
         ktype_id=dsms.ktypes.Organization,
     )
 
     assert kitem.ktype == Context.ktypes.get(dsms.ktypes.Organization.value)
+
+
+# @responses.activate
+# def test_ktype_custom_property_assignment(get_mock_kitem_ids, custom_address):
+#     from dsms.knowledge.properties.custom_datatype.numerical import NumericalDataType
+#     from dsms.core.dsms import DSMS
+#     from dsms.knowledge.kitem import KItem
+
+#     with pytest.warns(UserWarning, match="No authentication details"):
+#         dsms = DSMS(host_url=custom_address)
+
+#     kitem = KItem(
+#         id=get_mock_kitem_ids[0],
+#         name="foo123",
+#         ktype_id=dsms.ktypes.Organization,
+#         custom_properties={"material": "abcd", "tester": 123}
+#     )
+
+#     assert kitem.custom_properties.material == "abcd"
+#     assert kitem.custom_properties.tester == 123
+#     assert isinstance(kitem.custom_properties.tester, NumericalDataType)
+
+#     kitem.custom_properties = {"material": "def", "tester2": 123}
+
+#     assert kitem.custom_properties.material == "def"
+#     assert kitem.custom_properties.tester2 == 123
+#     assert isinstance(kitem.custom_properties.tester2, NumericalDataType)
+
+#     kitem.custom_properties.tester2 = 456
+#     assert kitem.custom_properties.tester2 == 456
+#     assert isinstance(kitem.custom_properties.tester2, NumericalDataType)
```

### Comparing `dsms_sdk-1.3.3/tests/test_utils.py` & `dsms_sdk-1.4.0rc0/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -105,7 +105,35 @@
         "user_groups_to_remove": [],
         "kitem_apps_to_remove": [
             obj.model_dump() for obj in kitem_old.kitem_apps
         ],
     }
     diffs = _get_kitems_diffs(kitem_old, kitem_new)
     assert sorted(diffs) == sorted(expected)
+
+
+@responses.activate
+def test_unit_conversion(custom_address):
+    """Test unit conversion test"""
+    from dsms import DSMS
+    from dsms.knowledge.semantics.units import get_conversion_factor
+
+    with pytest.warns(UserWarning, match="No authentication details"):
+        DSMS(host_url=custom_address)
+
+    assert get_conversion_factor("mm", "m", decimals=3) == 0.001
+
+    assert get_conversion_factor("km", "in", decimals=1) == 39370.1
+
+    assert get_conversion_factor("GPa", "MPa") == 1000
+
+    assert (
+        get_conversion_factor(
+            "http://qudt.org/vocab/unit/M",
+            "http://qudt.org/vocab/unit/IN",
+            decimals=1,
+        )
+        == 39.4
+    )
+
+    with pytest.raises(ValueError, match="Unit "):
+        get_conversion_factor("kPa", "cm")
```

