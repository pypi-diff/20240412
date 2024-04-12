# Comparing `tmp/ubkg_api-1.4.0.tar.gz` & `tmp/ubkg_api-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubkg_api-1.4.0.tar", last modified: Wed Sep  6 14:20:12 2023, max compression
+gzip compressed data, was "ubkg_api-2.1.1.tar", last modified: Fri Apr 12 19:14:51 2024, max compression
```

## Comparing `ubkg_api-1.4.0.tar` & `ubkg_api-2.1.1.tar`

### file list

```diff
@@ -1,58 +1,93 @@
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.152554 ubkg_api-1.4.0/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1087 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/LICENSE
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1516 2023-09-06 14:20:12.152554 ubkg_api-1.4.0/PKG-INFO
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      943 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/README.md
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      759 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/pyproject.toml
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)       38 2023-09-06 14:20:12.152554 ubkg_api-1.4.0/setup.cfg
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.139553 ubkg_api-1.4.0/src/
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.142553 ubkg_api-1.4.0/src/ubkg_api/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3883 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/app.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.144554 ubkg_api-1.4.0/src/ubkg_api/common_routes/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/__init__.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.145553 ubkg_api-1.4.0/src/ubkg_api/common_routes/codes/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/codes/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1400 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/codes/codes_controller.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)    24379 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/common_neo4j_logic.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.145553 ubkg_api-1.4.0/src/ubkg_api/common_routes/concepts/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/concepts/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     4978 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/concepts/concepts_controller.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.146554 ubkg_api-1.4.0/src/ubkg_api/common_routes/semantics/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/semantics/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      770 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/semantics/semantics_controller.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.146554 ubkg_api-1.4.0/src/ubkg_api/common_routes/terms/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/terms/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1799 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/terms/terms_controller.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.147554 ubkg_api-1.4.0/src/ubkg_api/common_routes/tui/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/tui/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      686 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/tui/tui_controller.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      364 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/common_routes/validate.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.151554 ubkg_api-1.4.0/src/ubkg_api/models/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/__init__.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1900 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/base_model_.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2518 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/codes_codes_obj.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2037 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/concept_detail.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2069 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/concept_prefterm.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2615 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/concept_sab_rel.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3336 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/concept_sab_rel_depth.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1909 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/concept_term.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5645 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3704 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3677 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/qqst.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1988 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/sab_definition.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3895 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3537 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/sab_relationship_concept_term.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1909 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/semantic_stn.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2314 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/sty_tui_stn.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1949 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/termtype_code.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)      809 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/typing_utils.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3507 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/models/util.py
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2067 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/src/ubkg_api/neo4j_connection_helper.py
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.143553 ubkg_api-1.4.0/src/ubkg_api.egg-info/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1516 2023-09-06 14:20:12.000000 ubkg_api-1.4.0/src/ubkg_api.egg-info/PKG-INFO
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1722 2023-09-06 14:20:12.000000 ubkg_api-1.4.0/src/ubkg_api.egg-info/SOURCES.txt
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        1 2023-09-06 14:20:12.000000 ubkg_api-1.4.0/src/ubkg_api.egg-info/dependency_links.txt
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)       66 2023-09-06 14:20:12.000000 ubkg_api-1.4.0/src/ubkg_api.egg-info/requires.txt
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)        9 2023-09-06 14:20:12.000000 ubkg_api-1.4.0/src/ubkg_api.egg-info/top_level.txt
-drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-09-06 14:20:12.152554 ubkg_api-1.4.0/tests/
--rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3136 2023-09-06 14:18:20.000000 ubkg_api-1.4.0/tests/test_controllers.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.550804 ubkg_api-2.1.1/
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1087 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/LICENSE
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-04-12 19:14:51.550354 ubkg_api-2.1.1/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)    11349 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/README.md
+-rw-r--r--   0 ZHY19      (503) staff       (20)      762 2024-04-12 19:01:18.000000 ubkg_api-2.1.1/pyproject.toml
+-rw-r--r--   0 ZHY19      (503) staff       (20)       38 2024-04-12 19:14:51.550848 ubkg_api-2.1.1/setup.cfg
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.432263 ubkg_api-2.1.1/src/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.440153 ubkg_api-2.1.1/src/ubkg_api/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5556 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/app.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.452606 ubkg_api-2.1.1/src/ubkg_api/common_routes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.456377 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2280 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/codes/codes_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    39519 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/common_neo4j_logic.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.459728 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)    17929 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/concepts/concepts_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.462044 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      479 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/database/database_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.462442 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.464546 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      803 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.468031 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6174 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/node_types/node_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.470199 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1009 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/property_types/property_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.472635 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1046 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.476111 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     7433 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/sabs/sabs_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.478830 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5563 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/semantics/semantics_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.481521 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      930 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/status/status_controller.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.484007 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2675 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/terms/terms_controller.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      364 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/common_routes/validate.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.535126 ubkg_api-2.1.1/src/ubkg_api/models/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1900 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/base_model_.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2518 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/codes_codes_obj.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2037 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_detail.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5760 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_graph.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1512 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_node.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     4715 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_path_hop.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2126 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2615 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3336 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel_depth.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1909 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/concept_term.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.542315 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3438 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/concept_path.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1946 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/semantic_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2351 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/deprecated/sty_tui_stn.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1418 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/node_type.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     5645 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3704 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3677 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/qqst.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1988 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_definition.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3895 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3537 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_term.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2198 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/semantictype.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1949 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/termtype_code.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)      809 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/typing_utils.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     3507 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/models/util.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     6991 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/neo4j_connection_helper.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.547371 ubkg_api-2.1.1/src/ubkg_api/utils/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/__init__.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.549597 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/
+-rw-r--r--   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/__init__.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2038 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/deprecated/path_get_endpoints.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     9744 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/http_error_string.py
+-rw-r--r--   0 ZHY19      (503) staff       (20)     1716 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/utils/http_parameter.py
+-rwxr-xr-x   0 ZHY19      (503) staff       (20)      185 2024-04-12 19:00:53.000000 ubkg_api-2.1.1/src/ubkg_api/wsgi.py
+drwxr-xr-x   0 ZHY19      (503) staff       (20)        0 2024-04-12 19:14:51.550014 ubkg_api-2.1.1/src/ubkg_api.egg-info/
+-rw-r--r--   0 ZHY19      (503) staff       (20)    12051 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/PKG-INFO
+-rw-r--r--   0 ZHY19      (503) staff       (20)     2979 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/SOURCES.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)        1 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/dependency_links.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       69 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/requires.txt
+-rw-r--r--   0 ZHY19      (503) staff       (20)       18 2024-04-12 19:14:51.000000 ubkg_api-2.1.1/src/ubkg_api.egg-info/top_level.txt
```

### Comparing `ubkg_api-1.4.0/LICENSE` & `ubkg_api-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/pyproject.toml` & `ubkg_api-2.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ubkg_api"
-version = "1.4.0"
+version = "2.1.1"
 authors = [
   { name="HuBMAP Consortium", email="api-developers@hubmapconsortium.org" },
 ]
 description = "A REST API in front of the Unified Biomedical Knowlegde Graph"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -16,13 +16,13 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "python_dateutil>=2.6.0",
     "setuptools>=21.0.0",
     "Flask==2.1.3",
-    "neo4j==4.4"
+    "neo4j==5.15.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/x-atlas-consortia/ubkg-api"
 "Bug Tracker" = "https://github.com/x-atlas-consortia/ubkg-api/issues"
```

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/base_model_.py` & `ubkg_api-2.1.1/src/ubkg_api/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/codes_codes_obj.py` & `ubkg_api-2.1.1/src/ubkg_api/models/codes_codes_obj.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/concept_detail.py` & `ubkg_api-2.1.1/src/ubkg_api/models/concept_detail.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/concept_prefterm.py` & `ubkg_api-2.1.1/src/ubkg_api/models/concept_prefterm.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,33 @@
 from .base_model_ import Model
 
 
 class ConceptPrefterm(Model):
     def __init__(self, concept=None, prefterm=None):
         """ConceptPrefterm - a model defined in OpenAPI
 
+        Represents a concept node in the UBKG.
+
         :param concept: The concept of this ConceptPrefterm.
         :type concept: str
-        :param prefterm: The prefterm of this ConceptPrefterm.
+        :param prefterm: The prefter  of this ConceptPrefterm.
         :type prefterm: str
         """
         self.openapi_types = {
             'concept': str,
             'prefterm': str
         }
 
         self.attribute_map = {
             'concept': 'concept',
             'prefterm': 'prefterm'
         }
 
         self._concept = concept
-        self._prefterm = prefterm
+        self._prefterm  = prefterm
 
     def serialize(self):
         return {
             "concept": self._concept,
             "prefterm": self._prefterm
         }
 
@@ -63,26 +65,26 @@
         :param concept: The concept of this ConceptPrefterm.
         :type concept: str
         """
 
         self._concept = concept
 
     @property
-    def prefterm(self):
-        """Gets the prefterm of this ConceptPrefterm.
+    def prefterm (self):
+        """Gets the prefterm  of this ConceptPrefterm.
 
 
-        :return: The prefterm of this ConceptPrefterm.
+        :return: The prefterm  of this ConceptPrefterm.
         :rtype: str
         """
         return self._prefterm
 
-    @prefterm.setter
-    def prefterm(self, prefterm):
-        """Sets the prefterm of this ConceptPrefterm.
+    @prefterm .setter
+    def prefterm(self, prefterm ):
+        """Sets the prefter  of this ConceptPrefterm.
 
 
-        :param prefterm: The prefterm of this ConceptPrefterm.
-        :type prefterm: str
+        :param prefterm : The prefterm of this ConceptPrefterm.
+        :type prefterm : str
         """
 
-        self._prefterm = prefterm
+        self._prefterm  = prefterm
```

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/concept_sab_rel.py` & `ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/concept_sab_rel_depth.py` & `ubkg_api-2.1.1/src/ubkg_api/models/concept_sab_rel_depth.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/concept_term.py` & `ubkg_api-2.1.1/src/ubkg_api/models/concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py` & `ubkg_api-2.1.1/src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/qconcept_tconcept_sab_rel.py` & `ubkg_api-2.1.1/src/ubkg_api/models/qconcept_tconcept_sab_rel.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/qqst.py` & `ubkg_api-2.1.1/src/ubkg_api/models/qqst.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/sab_definition.py` & `ubkg_api-2.1.1/src/ubkg_api/models/sab_definition.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/sab_relationship_concept_prefterm.py` & `ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_prefterm.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/sab_relationship_concept_term.py` & `ubkg_api-2.1.1/src/ubkg_api/models/sab_relationship_concept_term.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/semantic_stn.py` & `ubkg_api-2.1.1/src/ubkg_api/models/deprecated/semantic_stn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from __future__ import absolute_import
 
-from . import util
-from .base_model_ import Model
+from src.ubkg_api.models import util
+from src.ubkg_api.models.base_model_ import Model
 
 
 class SemanticStn(Model):
     def __init__(self, semantic=None, stn=None):
         """SemanticStn - a model defined in OpenAPI
 
         :param semantic: The semantic of this SemanticStn.
```

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/sty_tui_stn.py` & `ubkg_api-2.1.1/src/ubkg_api/models/deprecated/sty_tui_stn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 from __future__ import absolute_import
 
-from . import util
-from .base_model_ import Model
+from src.ubkg_api.models import util
+from src.ubkg_api.models.base_model_ import Model
 
 
 class StyTuiStn(Model):
     def __init__(self, sty=None, tui=None, stn=None):
         """StyTuiStn - a model defined in OpenAPI
 
         :param sty: The sty of this StyTuiStn.
```

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/termtype_code.py` & `ubkg_api-2.1.1/src/ubkg_api/models/termtype_code.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/typing_utils.py` & `ubkg_api-2.1.1/src/ubkg_api/models/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api/models/util.py` & `ubkg_api-2.1.1/src/ubkg_api/models/util.py`

 * *Files identical despite different names*

### Comparing `ubkg_api-1.4.0/src/ubkg_api.egg-info/SOURCES.txt` & `ubkg_api-2.1.1/src/ubkg_api.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,70 @@
 LICENSE
 README.md
 pyproject.toml
+src/__init__.py
 src/ubkg_api/__init__.py
 src/ubkg_api/app.py
 src/ubkg_api/neo4j_connection_helper.py
+src/ubkg_api/wsgi.py
 src/ubkg_api.egg-info/PKG-INFO
 src/ubkg_api.egg-info/SOURCES.txt
 src/ubkg_api.egg-info/dependency_links.txt
 src/ubkg_api.egg-info/requires.txt
 src/ubkg_api.egg-info/top_level.txt
 src/ubkg_api/common_routes/__init__.py
 src/ubkg_api/common_routes/common_neo4j_logic.py
 src/ubkg_api/common_routes/validate.py
 src/ubkg_api/common_routes/codes/__init__.py
 src/ubkg_api/common_routes/codes/codes_controller.py
 src/ubkg_api/common_routes/concepts/__init__.py
 src/ubkg_api/common_routes/concepts/concepts_controller.py
+src/ubkg_api/common_routes/database/__init__.py
+src/ubkg_api/common_routes/database/database_controller.py
+src/ubkg_api/common_routes/deprecated/__init__.py
+src/ubkg_api/common_routes/deprecated/tui/__init__.py
+src/ubkg_api/common_routes/deprecated/tui/tui_controller.py
+src/ubkg_api/common_routes/node_types/__init__.py
+src/ubkg_api/common_routes/node_types/node_types_controller.py
+src/ubkg_api/common_routes/property_types/__init__.py
+src/ubkg_api/common_routes/property_types/property_types_controller.py
+src/ubkg_api/common_routes/relationship_types/__init__.py
+src/ubkg_api/common_routes/relationship_types/relationship_types_controller.py
+src/ubkg_api/common_routes/sabs/__init__.py
+src/ubkg_api/common_routes/sabs/sabs_controller.py
 src/ubkg_api/common_routes/semantics/__init__.py
 src/ubkg_api/common_routes/semantics/semantics_controller.py
+src/ubkg_api/common_routes/status/__init__.py
+src/ubkg_api/common_routes/status/status_controller.py
 src/ubkg_api/common_routes/terms/__init__.py
 src/ubkg_api/common_routes/terms/terms_controller.py
-src/ubkg_api/common_routes/tui/__init__.py
-src/ubkg_api/common_routes/tui/tui_controller.py
 src/ubkg_api/models/__init__.py
 src/ubkg_api/models/base_model_.py
 src/ubkg_api/models/codes_codes_obj.py
 src/ubkg_api/models/concept_detail.py
+src/ubkg_api/models/concept_graph.py
+src/ubkg_api/models/concept_node.py
+src/ubkg_api/models/concept_path_hop.py
 src/ubkg_api/models/concept_prefterm.py
 src/ubkg_api/models/concept_sab_rel.py
 src/ubkg_api/models/concept_sab_rel_depth.py
 src/ubkg_api/models/concept_term.py
+src/ubkg_api/models/node_type.py
 src/ubkg_api/models/path_item_concept_relationship_sab_prefterm.py
 src/ubkg_api/models/qconcept_tconcept_sab_rel.py
 src/ubkg_api/models/qqst.py
 src/ubkg_api/models/sab_definition.py
 src/ubkg_api/models/sab_relationship_concept_prefterm.py
 src/ubkg_api/models/sab_relationship_concept_term.py
-src/ubkg_api/models/semantic_stn.py
-src/ubkg_api/models/sty_tui_stn.py
+src/ubkg_api/models/semantictype.py
 src/ubkg_api/models/termtype_code.py
 src/ubkg_api/models/typing_utils.py
 src/ubkg_api/models/util.py
-tests/test_controllers.py
+src/ubkg_api/models/deprecated/__init__.py
+src/ubkg_api/models/deprecated/concept_path.py
+src/ubkg_api/models/deprecated/semantic_stn.py
+src/ubkg_api/models/deprecated/sty_tui_stn.py
+src/ubkg_api/utils/__init__.py
+src/ubkg_api/utils/http_error_string.py
+src/ubkg_api/utils/http_parameter.py
+src/ubkg_api/utils/deprecated/__init__.py
+src/ubkg_api/utils/deprecated/path_get_endpoints.py
```

