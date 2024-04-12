# Comparing `tmp/brainglobe-workflows-1.1.4.tar.gz` & `tmp/brainglobe_workflows-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-workflows-1.1.4.tar", last modified: Thu Feb 22 18:49:19 2024, max compression
+gzip compressed data, was "brainglobe_workflows-1.1.5.tar", last modified: Fri Apr 12 17:50:37 2024, max compression
```

## Comparing `brainglobe-workflows-1.1.4.tar` & `brainglobe_workflows-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.724640 brainglobe-workflows-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-02-22 18:49:19.724640 brainglobe-workflows-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/asv.conf.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.716640 brainglobe-workflows-1.1.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/benchmarks/cellfinder_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.720640 brainglobe-workflows-1.1.4/brainglobe_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.720640 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/analyse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/prep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.720640 brainglobe-workflows-1.1.4/brainglobe_workflows/cellfinder_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/cellfinder_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/cellfinder_core/cellfinder_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.720640 brainglobe-workflows-1.1.4/brainglobe_workflows/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/configs/cellfinder.json
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/brainglobe_workflows/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 18:49:19.720640 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-02-22 18:49:18.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-22 18:49:19.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:49:18.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-22 18:49:18.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 18:49:17.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-02-22 18:49:18.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-22 18:49:18.000000 brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-02-22 18:49:09.000000 brainglobe-workflows-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 18:49:19.724640 brainglobe-workflows-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/asv.conf.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.798472 brainglobe_workflows-1.1.5/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/benchmarks/cellfinder_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.798472 brainglobe_workflows-1.1.5/brainglobe_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13592 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/prep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/cellfinder_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/configs/cellfinder.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/brainglobe_workflows/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-12 17:50:37.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 17:50:35.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-12 17:50:36.000000 brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-12 17:50:29.000000 brainglobe_workflows-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 17:50:37.802471 brainglobe_workflows-1.1.5/setup.cfg
```

### Comparing `brainglobe-workflows-1.1.4/.gitignore` & `brainglobe_workflows-1.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/LICENSE` & `brainglobe_workflows-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/PKG-INFO` & `brainglobe_workflows-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-workflows
-Version: 1.1.4
+Version: 1.1.5
 Summary: A collection of end-to-end data analysis workflows executed using BrainGlobe tools.
 Author: Christian Niedworok, Charly Rousseau
 Author-email: Adam Tyson <code@adamltyson.com>, BrainGlobe developers <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, BrainGlobe developers.
         All rights reserved.
```

### Comparing `brainglobe-workflows-1.1.4/README.md` & `brainglobe_workflows-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/asv.conf.json` & `brainglobe_workflows-1.1.5/asv.conf.json`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/benchmarks/cellfinder_core.py` & `brainglobe_workflows-1.1.5/benchmarks/cellfinder_core.py`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/analyse.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/analyse.py`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/main.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/main.py`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/parser.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 from brainreg.core.cli import atlas_parse, geometry_parser, niftyreg_parse
 from brainreg.core.cli import backend_parse as brainreg_backend_parse
 from cellfinder.core.download.cli import (
     download_directory_parser,
     model_parser,
 )
-from cellfinder.core.tools.source_files import source_custom_config_cellfinder
+from cellfinder.core.tools.source_files import user_specific_configuration_path
 
 from brainglobe_workflows import __version__
 
 # TODO: Gradually move all paths as strings to Path objects
 
 models = {
     "18": "18-layer",
@@ -384,15 +384,15 @@
 
 def config_parse(parser):
     config_opt_parser = parser.add_argument_group("Config options")
     config_opt_parser.add_argument(
         "--config",
         dest="registration_config",
         type=str,
-        default=source_custom_config_cellfinder(),
+        default=user_specific_configuration_path(),
         help="To supply your own, custom configuration file.",
     )
 
     return parser
 
 
 def figures_parse(parser):
```

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/brainmapper/prep.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/brainmapper/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import json
 import logging
 import os
 from argparse import Namespace
 from pathlib import PurePath
 
-from bg_atlasapi import BrainGlobeAtlas
+from brainglobe_atlasapi import BrainGlobeAtlas
 from brainglobe_utils.general.exceptions import CommandLineInputError
 from brainglobe_utils.general.list import check_unique_list, common_member
 from brainglobe_utils.general.system import (
     catch_input_file_error,
     ensure_directory_exists,
 )
 from brainreg.core.paths import Paths as BrainRegPaths
```

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/cellfinder_core/cellfinder_core.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/cellfinder_core/cellfinder_core.py`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/configs/cellfinder.json` & `brainglobe_workflows-1.1.5/brainglobe_workflows/configs/cellfinder.json`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows/utils.py` & `brainglobe_workflows-1.1.5/brainglobe_workflows/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/PKG-INFO` & `brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-workflows
-Version: 1.1.4
+Version: 1.1.5
 Summary: A collection of end-to-end data analysis workflows executed using BrainGlobe tools.
 Author: Christian Niedworok, Charly Rousseau
 Author-email: Adam Tyson <code@adamltyson.com>, BrainGlobe developers <code@adamltyson.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, BrainGlobe developers.
         All rights reserved.
```

### Comparing `brainglobe-workflows-1.1.4/brainglobe_workflows.egg-info/SOURCES.txt` & `brainglobe_workflows-1.1.5/brainglobe_workflows.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-workflows-1.1.4/pyproject.toml` & `brainglobe_workflows-1.1.5/pyproject.toml`

 * *Files identical despite different names*

