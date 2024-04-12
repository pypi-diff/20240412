# Comparing `tmp/pmpsdb_client-1.1.2.tar.gz` & `tmp/pmpsdb_client-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmpsdb_client-1.1.2.tar", last modified: Wed Apr 12 18:39:54 2023, max compression
+gzip compressed data, was "pmpsdb_client-1.2.tar", last modified: Fri Apr 12 21:45:34 2024, max compression
```

## Comparing `pmpsdb_client-1.1.2.tar` & `pmpsdb_client-1.2.tar`

### file list

```diff
@@ -1,49 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)      166 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.857101 pmpsdb_client-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.857101 pmpsdb_client-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     5841 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2586 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)    16356 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/kfe-motion.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/pmpsdb_client/
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     4308 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/beam_class.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/pmpsdb_client/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2221 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/cli/epics_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     1127 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/cli/run_gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     6324 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/cli/transfer_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/device_map.ui
--rw-r--r--   0 runner    (1001) docker     (122)     3070 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/export_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10735 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/ftp_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    34883 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     8845 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/ioc_data.py
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/pmpsdb_kfe.yml
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/pmpsdb_lfe.yml
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/pmpsdb_rix.yml
--rw-r--r--   0 runner    (1001) docker     (122)       66 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/pmpsdb_tmo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/pmpsdb_tst.yml
--rw-r--r--   0 runner    (1001) docker     (122)     8746 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/tables.ui
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/pmpsdb_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      389 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     1398 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pmpsdb_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5841 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-12 18:39:54.000000 pmpsdb_client-1.1.2/pmpsdb_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-12 18:39:54.861101 pmpsdb_client-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    16356 2023-04-12 18:39:35.000000 pmpsdb_client-1.1.2/tst-motion.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.697441 pmpsdb_client-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.689441 pmpsdb_client-1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.689441 pmpsdb_client-1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-12 21:45:34.697441 pmpsdb_client-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.689441 pmpsdb_client-1.2/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16356 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/kfe-motion.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.693441 pmpsdb_client-1.2/pmpsdb_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/beam_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.693441 pmpsdb_client-1.2/pmpsdb_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/cli/epics_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/cli/run_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/cli/transfer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/device_map.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/ftp_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34884 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/ioc_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/plc_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/pmpsdb_kfe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/pmpsdb_lfe.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/pmpsdb_rix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/pmpsdb_tmo.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/pmpsdb_tst.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/ssh_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/tables.ui
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.693441 pmpsdb_client-1.2/pmpsdb_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pmpsdb_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:45:34.697441 pmpsdb_client-1.2/pmpsdb_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 21:45:34.000000 pmpsdb_client-1.2/pmpsdb_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:45:34.697441 pmpsdb_client-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    16356 2024-04-12 21:45:22.000000 pmpsdb_client-1.2/tst-motion.json
```

### Comparing `pmpsdb_client-1.1.2/.github/workflows/standard.yml` & `pmpsdb_client-1.2/.github/workflows/standard.yml`

 * *Files 12% similar despite different names*

```diff
@@ -16,10 +16,10 @@
       # automatically if the repository name is the same as the import name.
       package-name: "pmpsdb_client"
       # Extras that will be installed for both conda/pip:
       testing-extras: ""
       # Extras to be installed only for conda-based testing:
       conda-testing-extras: ""
       # Extras to be installed only for pip-based testing:
-      pip-testing-extras: "PyQt5"
+      pip-testing-extras: ""
       # Set if using setuptools-scm for the conda-build workflow
       use-setuptools-scm: true
```

### Comparing `pmpsdb_client-1.1.2/.pre-commit-config.yaml` & `pmpsdb_client-1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/LICENSE.md` & `pmpsdb_client-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/PKG-INFO` & `pmpsdb_client-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmpsdb_client
-Version: 1.1.2
+Version: 1.2.0
 Summary: Client application for interfacing with the PMPS database and the deployed PLC files.
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2022, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,16 +45,25 @@
         
 Keywords: pmps,pmpsdb,lcls
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.md
+Requires-Dist: fabric
+Requires-Dist: ophyd
+Requires-Dist: pcdscalc
+Requires-Dist: pcdsutils
+Requires-Dist: prettytable
+Requires-Dist: qtpy
+Provides-Extra: test
+Requires-Dist: PyQt5; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: setuptools-scm; extra == "test"
 
 # pmpsdb_client
 
 ## Overview
 This is a gui and cli application for managing the deployment and inspection of
 PMPS database files on production PLCs at LCLS.
 It provides tools to make deployment and verification of deployment seamless and easy.
```

### Comparing `pmpsdb_client-1.1.2/README.md` & `pmpsdb_client-1.2/README.md`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/kfe-motion.json` & `pmpsdb_client-1.2/kfe-motion.json`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/beam_class.py` & `pmpsdb_client-1.2/pmpsdb_client/beam_class.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/cli/__init__.py` & `pmpsdb_client-1.2/pmpsdb_client/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,20 +43,26 @@
     helper function as needed.
     """
     if args.version:
         from ..version import version
         print(version)
         return 0
     if args.verbose:
-        logging.basicConfig(level=logging.DEBUG)
+        logging.basicConfig(
+            level=logging.DEBUG,
+            format="%(asctime)s %(levelname)s: %(name)s %(message)s",
+        )
     else:
         logging.basicConfig(
             level=logging.INFO,
             format='%(levelname)s: %(message)s',
         )
+        # Noisy log messages from ssh transport layer
+        for module in ("fabric", "paramiko", "intake"):
+            logging.getLogger(module).setLevel(logging.WARNING)
     if args.export_dir:
         from ..export_data import set_export_dir
         set_export_dir(args.export_dir)
     if args.subparser == 'gui':
         from .run_gui import run_gui
         return run_gui(args)
     if args.subparser == 'list-files':
```

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/cli/epics_tools.py` & `pmpsdb_client-1.2/pmpsdb_client/cli/epics_tools.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/cli/parser.py` & `pmpsdb_client-1.2/pmpsdb_client/cli/parser.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/cli/run_gui.py` & `pmpsdb_client-1.2/pmpsdb_client/cli/run_gui.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/cli/transfer_tools.py` & `pmpsdb_client-1.2/pmpsdb_client/cli/transfer_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 """
 import argparse
 import logging
 import os.path
 from typing import Optional
 
 from ..export_data import ExportFile, get_latest_exported_files
-from ..ftp_data import (compare_file, download_file_text, list_file_info,
+from ..plc_data import (compare_file, download_file_text, list_file_info,
                         upload_filename)
 
 logger = logging.getLogger(__name__)
 
 
 def cli_list_files(args: argparse.Namespace) -> int:
     """Show all files uploaded to a PLC."""
     return _list_files(hostname=args.hostname)
 
 
 def _list_files(hostname: str) -> int:
     infos = list_file_info(hostname=hostname)
     for data in infos:
         print(
-            f'{data.filename} uploaded at {data.create_time.ctime()} '
+            f'{data.filename} uploaded at {data.last_changed.ctime()} '
             f'({data.size} bytes)'
         )
     if not infos:
         logger.warning('No files found')
     return 0
```

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/device_map.ui` & `pmpsdb_client-1.2/pmpsdb_client/device_map.ui`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/export_data.py` & `pmpsdb_client-1.2/pmpsdb_client/export_data.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/ftp_data.py` & `pmpsdb_client-1.2/pmpsdb_client/ftp_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 PLCs. In order for this to work, the PLC needs to be configured to run its
 FTP server.
 """
 from __future__ import annotations
 
 import datetime
 import ftplib
-import json
 import logging
 import os
-import typing
 from contextlib import contextmanager
 from dataclasses import dataclass
+from typing import BinaryIO, Iterator, TypeVar
+
+from .data_types import FileInfo
 
 DEFAULT_PW = (
     ('Administrator', '1'),
     ('webguest', '1'),
 )
 DIRECTORY = 'pmps'
 
 logger = logging.getLogger(__name__)
+T = TypeVar("T")
 
 
 @contextmanager
-def ftp(hostname: str, directory: typing.Optional[str] = None) -> ftplib.FTP:
+def ftp(hostname: str, directory: str | None = None) -> Iterator[ftplib.FTP]:
     """
     Context manager that manages an FTP connection.
 
     The connection will be opened and closed cleanly.
     This will be used as a helper in other functions.
 
     Parameters
@@ -46,15 +48,15 @@
     ftp : ftplib.FTP
         An active FTP instance that can be used to read and write files.
     """
     logger.debug('ftp(%s, %s)', hostname, directory)
     # Default directory
     directory = directory or DIRECTORY
     # Create without connecting
-    ftp_obj = ftplib.FTP(hostname, timeout=2.0)
+    ftp_obj = ftplib.FTP(hostname, timeout=1.0)
     # Beckhoff docs recommend active mode
     ftp_obj.set_pasv(False)
     # Best-effort login using default passwords
     rval = None
     for user, pwd in DEFAULT_PW:
         try:
             logger.debug('Try user=%s', user)
@@ -82,51 +84,49 @@
     except Exception:
         # Rude cleanup
         ftp_obj.close()
 
 
 def list_filenames(
     hostname: str,
-    directory: typing.Optional[str] = None,
+    directory: str | None = None,
 ) -> list[str]:
     """
     List the filenames that are currently saved on the PLC.
 
     Parameters
     ----------
     hostname : str
-        The plc hostname to upload to.
+        The plc hostname to check.
     directory : str, optional
         The ftp subdirectory to read and write from
         A default directory pmps is used if this argument is omitted.
 
     Returns
     -------
     filenames : list of str
         The filenames on the PLC.
     """
     logger.debug('list_filenames(%s, %s)', hostname, directory)
     with ftp(hostname=hostname, directory=directory) as ftp_obj:
         return ftp_obj.nlst()
 
 
-@dataclass
-class PLCFile:
+@dataclass(frozen=True)
+class FTPFileInfo(FileInfo):
     """
     Information about a file on the PLC as learned through ftp.
 
-    In the context of pmps, the create_time is the last time we
-    updated the database export file.
+    Contains very few fields: ftp doesn't give us a lot of info.
+    See data_types.FileInfo for the field information.
+    This protocol is what limits the amount of fields we can assume
+    are available when we don't know the PLC's type.
     """
-    filename: str
-    create_time: datetime.datetime
-    size: int
-
     @classmethod
-    def from_list_line(cls, line: str) -> PLCFile:
+    def from_list_line(cls: type[T], line: str) -> T:
         """
         Create a PLCFile from the output of the ftp LIST command.
 
         The output of this command is a series of lines representing
         information about the files in a directory.
 
         Here is a sample line of output:
@@ -146,23 +146,23 @@
             month=int(month),
             day=int(day),
             hour=int(hour),
             minute=int(minute),
         )
         return cls(
             filename=filename,
-            create_time=full_datetime,
             size=int(size),
+            last_changed=full_datetime,
         )
 
 
 def list_file_info(
     hostname: str,
-    directory: typing.Optional[str] = None,
-) -> list[PLCFile]:
+    directory: str | None = None,
+) -> list[FTPFileInfo]:
     """
     Gather pertinent information about all the files.
 
     Parameters
     ----------
     hostname : str
         The plc hostname to connect to.
@@ -176,22 +176,22 @@
         Information about our files, such as their creation times, sizes, and
         filenames.
     """
     logger.debug('list_file_info(%s, %s)', hostname, directory)
     lines = []
     with ftp(hostname=hostname, directory=directory) as ftp_obj:
         ftp_obj.retrlines('LIST', lines.append)
-    return [PLCFile.from_list_line(line) for line in lines]
+    return [FTPFileInfo.from_list_line(line) for line in lines]
 
 
 def upload_file(
     hostname: str,
     target_filename: str,
-    fd: typing.BinaryIO,
-    directory: typing.Optional[str] = None,
+    fd: BinaryIO,
+    directory: str | None = None,
 ):
     """
     Upload an open file to a PLC.
 
     Parameters
     ----------
     hostname : str
@@ -215,26 +215,28 @@
     with ftp(hostname=hostname, directory=directory) as ftp_obj:
         ftp_obj.storbinary(f'STOR {target_filename}', fd)
 
 
 def upload_filename(
     hostname: str,
     filename: str,
-    dest_filename: typing.Optional[str] = None,
-    directory: typing.Optional[str] = None,
+    dest_filename: str | None = None,
+    directory: str | None = None,
 ):
     """
     Open and upload a file on your filesystem to a PLC.
 
     Parameters
     ----------
     hostname : str
         The plc hostname to upload to.
     filename : str
-        The name of the file on both your filesystem and on the PLC.
+        The name of the file on your filesystem.
+    dest_filename : str, optional
+        The name of the file on the PLC. If omitted, same as filename.
     directory : str, optional
         The ftp subdirectory to read and write from
         A default directory pmps is used if this argument is omitted.
     """
     logger.debug(
         'upload_file(%s, %s, %s, %s)',
         hostname,
@@ -250,15 +252,15 @@
             directory=directory,
         )
 
 
 def download_file_text(
     hostname: str,
     filename: str,
-    directory: typing.Optional[str] = None,
+    directory: str | None = None,
 ) -> str:
     """
     Download a file from the PLC to use in Python.
 
     The result is a single string, suitable for operations like
     json.loads
 
@@ -286,112 +288,7 @@
     byte_chunks = []
     with ftp(hostname=hostname, directory=directory) as ftp_obj:
         ftp_obj.retrbinary(f'RETR {filename}', byte_chunks.append)
     contents = ''
     for chunk in byte_chunks:
         contents += chunk.decode('ascii')
     return contents
-
-
-def download_file_json_dict(
-    hostname: str,
-    filename: str,
-    directory: typing.Optional[str] = None,
-) -> dict[str, dict[str, typing.Any]]:
-    """
-    Download a file from the PLC and interpret it as a json dictionary.
-
-    The result is suitable for comparing to json blobs exported from the
-    pmps database.
-
-    Parameters
-    ----------
-    hostname : str
-        The plc hostname to download from.
-    filename : str
-        The name of the file on the PLC.
-    directory : str, optional
-        The ftp subdirectory to read and write from
-        A default directory pmps is used if this argument is omitted.
-
-    Returns
-    -------
-    data : dict
-        The dictionary data from the file stored on the plc.
-    """
-    logger.debug(
-        'download_file_json_dict(%s, %s, %s)',
-        hostname,
-        filename,
-        directory,
-    )
-    return json.loads(
-        download_file_text(
-            hostname=hostname,
-            filename=filename,
-            directory=directory,
-        )
-    )
-
-
-def local_file_json_dict(filename: str) -> dict[str, dict[str, typing.Any]]:
-    """
-    Return the json dict from a local file.
-
-    Suitable for comparisons to files from the database or from the plc.
-
-    Parameters
-    ----------
-    filename : str
-        The name of the file on the local filesystem.
-
-    Returns
-    -------
-    data : dict
-        The dictionary data from the file stored on the local drive.
-    """
-    logger.debug('local_file_json_dict(%s)', filename)
-    with open(filename, 'r') as fd:
-        return json.load(fd)
-
-
-def compare_file(
-    hostname: str,
-    local_filename: str,
-    plc_filename: typing.Optional[str] = None,
-    directory: typing.Optional[str] = None,
-) -> bool:
-    """
-    Compare a file saved locally to one on the PLC.
-
-    Parameters
-    ----------
-    hostname : str
-        The plc hostname to download from.
-    local_filename: str
-        The full path the local file to compare with.
-    plc_filename: str, optional
-        The filename as saved on the PLC. If omitted, the local_filename's
-        basename will be used.
-    directory : str, optional
-        The ftp subdirectory to read and write from
-        A default directory pmps is used if this argument is omitted.
-
-    Returns
-    -------
-    same_file : bool
-        True if the contents of these two files are the same.
-    """
-    logger.debug(
-        'compare_file(%s, %s, %s, %s)',
-        hostname,
-        local_filename,
-        plc_filename,
-        directory,
-    )
-    local_data = local_file_json_dict(filename=local_filename)
-    plc_data = download_file_json_dict(
-        hostname=hostname,
-        filename=plc_filename,
-        directory=directory,
-    )
-    return local_data == plc_data
```

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/gui.py` & `pmpsdb_client-1.2/pmpsdb_client/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from qtpy.QtWidgets import (QAction, QDialog, QFileDialog, QInputDialog,
                             QLabel, QListWidget, QListWidgetItem, QMainWindow,
                             QMessageBox, QStatusBar, QTableWidget,
                             QTableWidgetItem, QWidget)
 
 from .beam_class import summarize_beam_class_bitmask
 from .export_data import ExportFile, get_export_dir, get_latest_exported_files
-from .ftp_data import (download_file_json_dict, download_file_text,
-                       list_file_info, upload_filename)
 from .ioc_data import AllStateBP, PLCDBControls
+from .plc_data import (download_file_json_dict, download_file_text,
+                       list_file_info, upload_filename)
 
 logger = logging.getLogger(__name__)
 
 PARAMETER_HEADER_ORDER = [
     'name',
     'id',
     'nRate',
@@ -574,15 +574,15 @@
         else:
             logger.debug('%s found file info %s', hostname, info)
             text = 'No upload found'
             self.ok_rows[row] = True
         filename = hostname_to_filename(hostname)
         for file_info in info:
             if file_info.filename == filename:
-                text = file_info.create_time.ctime()
+                text = file_info.last_changed.ctime()
                 break
         self.plc_table.item(row, PLCTableColumns.UPLOAD).setText(text)
         if update_export:
             self.update_export_times()
 
     def update_plc_row_by_hostname(self, hostname: str) -> None:
         """
```

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/ioc_data.py` & `pmpsdb_client-1.2/pmpsdb_client/ioc_data.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/tables.ui` & `pmpsdb_client-1.2/pmpsdb_client/tables.ui`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client/version.py` & `pmpsdb_client-1.2/pmpsdb_client/version.py`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client.egg-info/PKG-INFO` & `pmpsdb_client-1.2/pmpsdb_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pmpsdb-client
-Version: 1.1.2
+Name: pmpsdb_client
+Version: 1.2.0
 Summary: Client application for interfacing with the PMPS database and the deployed PLC files.
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2022, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -45,16 +45,25 @@
         
 Keywords: pmps,pmpsdb,lcls
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE.md
+Requires-Dist: fabric
+Requires-Dist: ophyd
+Requires-Dist: pcdscalc
+Requires-Dist: pcdsutils
+Requires-Dist: prettytable
+Requires-Dist: qtpy
+Provides-Extra: test
+Requires-Dist: PyQt5; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: setuptools-scm; extra == "test"
 
 # pmpsdb_client
 
 ## Overview
 This is a gui and cli application for managing the deployment and inspection of
 PMPS database files on production PLCs at LCLS.
 It provides tools to make deployment and verification of deployment seamless and easy.
```

### Comparing `pmpsdb_client-1.1.2/pmpsdb_client.egg-info/SOURCES.txt` & `pmpsdb_client-1.2/pmpsdb_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,32 @@
 README.md
 dev-requirements.txt
 kfe-motion.json
 pyproject.toml
 requirements.txt
 tst-motion.json
 .github/workflows/standard.yml
+conda-recipe/meta.yaml
 pmpsdb_client/__init__.py
 pmpsdb_client/__main__.py
 pmpsdb_client/_version.py
 pmpsdb_client/beam_class.py
+pmpsdb_client/data_types.py
 pmpsdb_client/device_map.ui
 pmpsdb_client/export_data.py
 pmpsdb_client/ftp_data.py
 pmpsdb_client/gui.py
 pmpsdb_client/ioc_data.py
+pmpsdb_client/plc_data.py
 pmpsdb_client/pmpsdb_kfe.yml
 pmpsdb_client/pmpsdb_lfe.yml
 pmpsdb_client/pmpsdb_rix.yml
 pmpsdb_client/pmpsdb_tmo.yml
 pmpsdb_client/pmpsdb_tst.yml
+pmpsdb_client/ssh_data.py
 pmpsdb_client/tables.ui
 pmpsdb_client/version.py
 pmpsdb_client.egg-info/PKG-INFO
 pmpsdb_client.egg-info/SOURCES.txt
 pmpsdb_client.egg-info/dependency_links.txt
 pmpsdb_client.egg-info/entry_points.txt
 pmpsdb_client.egg-info/requires.txt
```

### Comparing `pmpsdb_client-1.1.2/pyproject.toml` & `pmpsdb_client-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pmpsdb_client-1.1.2/tst-motion.json` & `pmpsdb_client-1.2/tst-motion.json`

 * *Files identical despite different names*

