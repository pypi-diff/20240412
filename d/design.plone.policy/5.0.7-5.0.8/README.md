# Comparing `tmp/design.plone.policy-5.0.7.tar.gz` & `tmp/design.plone.policy-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.7.tar", last modified: Wed Dec 13 09:24:47 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.8.tar", last modified: Thu Apr 11 16:10:33 2024, max compression
```

## Comparing `design.plone.policy-5.0.7.tar` & `design.plone.policy-5.0.8.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.252076 design.plone.policy-5.0.7/
--rw-r--r--   0 filippocampi   (501) staff       (20)     6119 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/CHANGES.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       73 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/CONTRIBUTORS.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)      585 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/DEVELOP.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)    18092 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/LICENSE.GPL
--rw-r--r--   0 filippocampi   (501) staff       (20)      670 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/LICENSE.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)      139 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/MANIFEST.in
--rw-r--r--   0 filippocampi   (501) staff       (20)    15669 2023-12-13 09:24:47.251710 design.plone.policy-5.0.7/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)     7466 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/README.rst
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.224052 design.plone.policy-5.0.7/docs/
--rw-r--r--   0 filippocampi   (501) staff       (20)     7993 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/docs/conf.py
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/docs/index.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)       31 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/requirements.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)      367 2023-12-13 09:24:47.252768 design.plone.policy-5.0.7/setup.cfg
--rw-r--r--   0 filippocampi   (501) staff       (20)     2887 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/setup.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.215997 design.plone.policy-5.0.7/src/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.224573 design.plone.policy-5.0.7/src/design/
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.228896 design.plone.policy-5.0.7/src/design/plone/
--rw-r--r--   0 filippocampi   (501) staff       (20)       80 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.234503 design.plone.policy-5.0.7/src/design/plone/policy/
--rw-r--r--   0 filippocampi   (501) staff       (20)      173 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.236731 design.plone.policy-5.0.7/src/design/plone/policy/browser/
--rw-r--r--   0 filippocampi   (501) staff       (20)      119 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    19901 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/config.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      540 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     5622 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/browser/trasparenza.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     1623 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      398 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/interfaces.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.238945 design.plone.policy-5.0.7/src/design/plone/policy/locales/
--rw-r--r--   0 filippocampi   (501) staff       (20)      611 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/README.rst
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/design.plone.policy.pot
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.217625 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.239394 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-r--r--   0 filippocampi   (501) staff       (20)     1748 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/update.py
--rwxr-xr-x   0 filippocampi   (501) staff       (20)      494 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/locales/update.sh
--rw-r--r--   0 filippocampi   (501) staff       (20)      273 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/permissions.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.218330 design.plone.policy-5.0.7/src/design/plone/policy/profiles/
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.242159 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/
--rw-r--r--   0 filippocampi   (501) staff       (20)      584 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/actions.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      175 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      122 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/catalog.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1027 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)     1742 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/registry.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      341 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/rolemap.xml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.243021 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/
--rw-r--r--   0 filippocampi   (501) staff       (20)      122 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      268 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/profiles/uninstall/registry.xml
--rw-r--r--   0 filippocampi   (501) staff       (20)      311 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/rejectanonymous.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.243786 design.plone.policy-5.0.7/src/design/plone/policy/restapi/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/__init__.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.245049 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      534 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)      996 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      250 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/configure.zcml
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.246507 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      519 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)     3611 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/get.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     2342 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/sensitive.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3499 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/setuphandlers.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     5214 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/testing.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.249389 design.plone.policy-5.0.7/src/design/plone/policy/tests/
--rw-r--r--   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/__init__.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4286 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4625 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_initial_structure.py
--rw-r--r--   0 filippocampi   (501) staff       (20)      795 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_registry_entries.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     4993 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_search_filters_api.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     3720 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/tests/test_setup.py
--rw-r--r--   0 filippocampi   (501) staff       (20)    15231 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/upgrades.py
--rw-r--r--   0 filippocampi   (501) staff       (20)     6017 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/upgrades.zcml
--rw-r--r--   0 filippocampi   (501) staff       (20)    13482 2023-12-13 09:24:46.000000 design.plone.policy-5.0.7/src/design/plone/policy/utils.py
-drwxr-xr-x   0 filippocampi   (501) staff       (20)        0 2023-12-13 09:24:47.250017 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/
--rw-r--r--   0 filippocampi   (501) staff       (20)    15669 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/PKG-INFO
--rw-r--r--   0 filippocampi   (501) staff       (20)     2700 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/SOURCES.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/dependency_links.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)       40 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/entry_points.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)       20 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        1 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/not-zip-safe
--rw-r--r--   0 filippocampi   (501) staff       (20)      504 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/requires.txt
--rw-r--r--   0 filippocampi   (501) staff       (20)        7 2023-12-13 09:24:47.000000 design.plone.policy-5.0.7/src/design.plone.policy.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6243 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      585 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/MANIFEST.in
+-rw-r--r--   0 mauro     (1000) mauro     (1000)    15836 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7466 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7993 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       31 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/requirements.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2926 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.408088 design.plone.policy-5.0.8/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      119 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    19901 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/browser/config.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/browser/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5622 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/browser/trasparenza.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1623 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      398 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/design.plone.policy.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.408088 design.plone.policy-5.0.8/src/design/plone/policy/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1748 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      494 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.408088 design.plone.policy-5.0.8/src/design/plone/policy/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      584 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/actions.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      175 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1100 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/metadata.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1742 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      341 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      268 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/profiles/uninstall/registry.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      311 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/rejectanonymous.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      534 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      996 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      250 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3611 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/get.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2342 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/sensitive.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3499 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     5214 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design/plone/policy/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4286 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4625 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/test_initial_structure.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      795 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/test_registry_entries.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4993 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3720 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    15231 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/upgrades.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6017 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/upgrades.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    13482 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design/plone/policy/utils.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2024-04-11 16:10:33.412088 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/
+-rw-r--r--   0 mauro     (1000) mauro     (1000)    15836 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2700 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      532 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2024-04-11 16:10:33.000000 design.plone.policy-5.0.8/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.7/CHANGES.rst` & `design.plone.policy-5.0.8/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+5.0.8 (2024-04-11)
+------------------
+
+- Add collective.volto.slimheader dependency and profile requirement.
+  [folix-01]
+
+
 5.0.7 (2023-12-13)
 ------------------
 
 - Update list of non searchable type in io-Comune
   [lucabel]
 - Do not return section children in @search-filters endpoint if they are types omitted from search results.
   [cekk]
```

### Comparing `design.plone.policy-5.0.7/DEVELOP.rst` & `design.plone.policy-5.0.8/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/LICENSE.GPL` & `design.plone.policy-5.0.8/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/LICENSE.rst` & `design.plone.policy-5.0.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/PKG-INFO` & `design.plone.policy-5.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.7
+Version: 5.0.8
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -28,14 +28,15 @@
 Requires-Dist: redturtle.volto
 Requires-Dist: design.plone.contenttypes>=6.0.0.dev0
 Requires-Dist: collective.feedback
 Requires-Dist: collective.volto.dropdownmenu
 Requires-Dist: collective.volto.formsupport[honeypot]
 Requires-Dist: collective.volto.secondarymenu
 Requires-Dist: collective.volto.socialsettings
+Requires-Dist: collective.volto.slimheader
 Requires-Dist: collective.volto.subsites
 Requires-Dist: collective.volto.subfooter
 Requires-Dist: eea.api.taxonomy
 Requires-Dist: redturtle.voltoplugin.editablefooter
 Requires-Dist: redturtle.faq
 Requires-Dist: redturtle.rssservice
 Requires-Dist: iw.rejectanonymous
@@ -298,14 +299,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.8 (2024-04-11)
+------------------
+
+- Add collective.volto.slimheader dependency and profile requirement.
+  [folix-01]
+
+
 5.0.7 (2023-12-13)
 ------------------
 
 - Update list of non searchable type in io-Comune
   [lucabel]
 - Do not return section children in @search-filters endpoint if they are types omitted from search results.
   [cekk]
```

### Comparing `design.plone.policy-5.0.7/README.rst` & `design.plone.policy-5.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/docs/conf.py` & `design.plone.policy-5.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/setup.py` & `design.plone.policy-5.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.7",
+    version="5.0.8",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -55,14 +55,15 @@
         "redturtle.volto",
         "design.plone.contenttypes>=6.0.0.dev0",
         "collective.feedback",
         "collective.volto.dropdownmenu",
         "collective.volto.formsupport[honeypot]",
         "collective.volto.secondarymenu",
         "collective.volto.socialsettings",
+        "collective.volto.slimheader",
         "collective.volto.subsites",
         "collective.volto.subfooter",
         "eea.api.taxonomy",
         "redturtle.voltoplugin.editablefooter",
         "redturtle.faq",
         "redturtle.rssservice",
         "iw.rejectanonymous",
```

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.8/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.8/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.8/src/design/plone/policy/browser/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.8/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.8/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.8/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files 5% similar despite different names*

#### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/metadata.xml`

```diff
@@ -8,12 +8,13 @@
     <dependency>profile-collective.volto.dropdownmenu:default</dependency>
     <dependency>profile-collective.volto.socialsettings:default</dependency>
     <dependency>profile-collective.volto.secondarymenu:default</dependency>
     <dependency>profile-collective.volto.subsites:default</dependency>
     <dependency>profile-redturtle.voltoplugin.editablefooter:default</dependency>
     <dependency>profile-collective.volto.formsupport:default</dependency>
     <dependency>profile-collective.volto.subfooter:default</dependency>
+    <dependency>profile-collective.volto.slimheader:default</dependency>
     <dependency>profile-eea.api.taxonomy:default</dependency>
     <dependency>profile-redturtle.faq:default</dependency>
     <dependency>profile-collective.feedback:default</dependency>
   </dependencies>
 </metadata>
```

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.8/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.8/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.8/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.8/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.8/src/design/plone/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.8/src/design/plone/policy/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.8/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.8/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_registry_entries.py` & `design.plone.policy-5.0.8/src/design/plone/policy/tests/test_registry_entries.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.8/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.8/src/design/plone/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.8/src/design/plone/policy/upgrades.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.8/src/design/plone/policy/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.8/src/design/plone/policy/utils.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.7/src/design.plone.policy.egg-info/PKG-INFO` & `design.plone.policy-5.0.8/src/design.plone.policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: design.plone.policy
-Version: 5.0.7
+Version: 5.0.8
 Summary: Pacchetto per creare un sito Agid su Plone
 Home-page: https://github.com/collective/design.plone.policy
 Author: RedTurtle Technology
 Author-email: sviluppo@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/design.plone.policy
 Project-URL: Source, https://github.com/RedTurtle/design.plone.policy
@@ -28,14 +28,15 @@
 Requires-Dist: redturtle.volto
 Requires-Dist: design.plone.contenttypes>=6.0.0.dev0
 Requires-Dist: collective.feedback
 Requires-Dist: collective.volto.dropdownmenu
 Requires-Dist: collective.volto.formsupport[honeypot]
 Requires-Dist: collective.volto.secondarymenu
 Requires-Dist: collective.volto.socialsettings
+Requires-Dist: collective.volto.slimheader
 Requires-Dist: collective.volto.subsites
 Requires-Dist: collective.volto.subfooter
 Requires-Dist: eea.api.taxonomy
 Requires-Dist: redturtle.voltoplugin.editablefooter
 Requires-Dist: redturtle.faq
 Requires-Dist: redturtle.rssservice
 Requires-Dist: iw.rejectanonymous
@@ -298,14 +299,21 @@
 
 - RedTurtle Technology, sviluppo@redturtle.it
 
 
 Changelog
 =========
 
+5.0.8 (2024-04-11)
+------------------
+
+- Add collective.volto.slimheader dependency and profile requirement.
+  [folix-01]
+
+
 5.0.7 (2023-12-13)
 ------------------
 
 - Update list of non searchable type in io-Comune
   [lucabel]
 - Do not return section children in @search-filters endpoint if they are types omitted from search results.
   [cekk]
```

### Comparing `design.plone.policy-5.0.7/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.8/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

