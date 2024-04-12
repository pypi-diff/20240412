# Comparing `tmp/fractal_tasks_core-0.9.4.tar.gz` & `tmp/fractal_tasks_core-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_tasks_core-0.9.4.tar", max compression
+gzip compressed data, was "fractal_tasks_core-1.0.0a0.tar", max compression
```

## Comparing `fractal_tasks_core-0.9.4.tar` & `fractal_tasks_core-1.0.0a0.tar`

### file list

```diff
@@ -1,31 +1,59 @@
--rw-r--r--   0        0        0     1584 2022-12-14 07:50:09.683341 fractal_tasks_core-0.9.4/LICENSE
--rw-r--r--   0        0        0     3697 2023-02-28 11:55:29.287745 fractal_tasks_core-0.9.4/README.md
--rw-r--r--   0        0        0       32 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/.gitignore
--rw-r--r--   0        0        0     3844 2023-04-11 14:35:05.288431 fractal_tasks_core-0.9.4/fractal_tasks_core/__FRACTAL_MANIFEST__.json
--rw-r--r--   0        0        0      165 2023-04-19 08:00:08.140294 fractal_tasks_core-0.9.4/fractal_tasks_core/__init__.py
--rw-r--r--   0        0        0     3005 2023-03-09 07:50:09.409308 fractal_tasks_core-0.9.4/fractal_tasks_core/_utils.py
--rw-r--r--   0        0        0    26138 2023-04-18 12:48:15.162857 fractal_tasks_core-0.9.4/fractal_tasks_core/cellpose_segmentation.py
--rw-r--r--   0        0        0     2543 2023-02-27 16:31:49.719523 fractal_tasks_core-0.9.4/fractal_tasks_core/compress_tif.py
--rw-r--r--   0        0        0     7687 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/copy_ome_zarr.py
--rw-r--r--   0        0        0    17556 2023-03-17 13:05:36.650239 fractal_tasks_core-0.9.4/fractal_tasks_core/create_ome_zarr.py
--rw-r--r--   0        0        0    20156 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.4/fractal_tasks_core/create_ome_zarr_multiplex.py
--rw-r--r--   0        0        0     9186 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/illumination_correction.py
--rw-r--r--   0        0        0    13467 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_ROI_overlaps.py
--rw-r--r--   0        0        0     8931 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_channels.py
--rw-r--r--   0        0        0     1403 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_glob.py
--rw-r--r--   0        0        0     9331 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_masked_loading.py
--rw-r--r--   0        0        0    12604 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_metadata_parsing.py
--rw-r--r--   0        0        0     3244 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_parse_filename_metadata.py
--rw-r--r--   0        0        0     3367 2023-01-17 14:38:05.370269 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_pyramid_creation.py
--rw-r--r--   0        0        0     3459 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_read_fractal_metadata.py
--rw-r--r--   0        0        0    12616 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_regions_of_interest.py
--rw-r--r--   0        0        0     7138 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_upscale_array.py
--rw-r--r--   0        0        0     3997 2023-02-21 13:59:08.836675 fractal_tasks_core-0.9.4/fractal_tasks_core/lib_zattrs_utils.py
--rw-r--r--   0        0        0     4658 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.4/fractal_tasks_core/maximum_intensity_projection.py
--rw-r--r--   0        0        0    24663 2023-04-18 13:44:35.575251 fractal_tasks_core-0.9.4/fractal_tasks_core/napari_workflows_wrapper.py
--rw-r--r--   0        0        0        0 2022-12-14 07:50:09.687341 fractal_tasks_core-0.9.4/fractal_tasks_core/tools/__init__.py
--rw-r--r--   0        0        0     3590 2023-03-14 12:50:49.873848 fractal_tasks_core-0.9.4/fractal_tasks_core/tools/lib_metadata_checks.py
--rw-r--r--   0        0        0     7262 2023-03-07 11:34:48.162824 fractal_tasks_core-0.9.4/fractal_tasks_core/yokogawa_to_ome_zarr.py
--rw-r--r--   0        0        0     2371 2023-04-19 08:00:08.136294 fractal_tasks_core-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     5046 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.4/setup.py
--rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 fractal_tasks_core-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1584 2024-04-12 10:04:31.506002 fractal_tasks_core-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0     3743 2024-04-12 10:04:31.506002 fractal_tasks_core-1.0.0a0/README.md
+-rw-r--r--   0        0        0       32 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/.gitignore
+-rw-r--r--   0        0        0    64078 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/__FRACTAL_MANIFEST__.json
+-rw-r--r--   0        0        0      200 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/cellvoyager/__init__.py
+-rw-r--r--   0        0        0     4552 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/cellvoyager/filenames.py
+-rw-r--r--   0        0        0    12515 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/cellvoyager/metadata.py
+-rw-r--r--   0        0        0    16707 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/channels.py
+-rw-r--r--   0        0        0      108 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/README.md
+-rw-r--r--   0        0        0       98 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/__init__.py
+-rw-r--r--   0        0        0     4607 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/check_manifest.py
+-rw-r--r--   0        0        0     5339 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/create_manifest.py
+-rw-r--r--   0        0        0     8166 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/lib_args_schemas.py
+-rw-r--r--   0        0        0     6406 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/lib_descriptions.py
+-rw-r--r--   0        0        0     3260 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/lib_signature_constraints.py
+-rw-r--r--   0        0        0     2827 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/lib_task_docs.py
+-rw-r--r--   0        0        0     2273 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/lib_titles.py
+-rw-r--r--   0        0        0     3610 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/task_list.py
+-rw-r--r--   0        0        0     2660 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/dev/task_models.py
+-rw-r--r--   0        0        0     5189 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/labels.py
+-rw-r--r--   0        0        0     9005 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/masked_loading.py
+-rw-r--r--   0        0        0      508 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/ngff/__init__.py
+-rw-r--r--   0        0        0    13113 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/ngff/specs.py
+-rw-r--r--   0        0        0     3974 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/ngff/zarr_utils.py
+-rw-r--r--   0        0        0     3788 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/pyramids.py
+-rw-r--r--   0        0        0      185 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/__init__.py
+-rw-r--r--   0        0        0     4501 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/_overlaps_common.py
+-rw-r--r--   0        0        0     1327 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/load_region.py
+-rw-r--r--   0        0        0    18609 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/v1.py
+-rw-r--r--   0        0        0     4910 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/v1_checks.py
+-rw-r--r--   0        0        0    13273 2024-04-12 10:04:31.510002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/v1_overlaps.py
+-rw-r--r--   0        0        0     3394 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tables/__init__.py
+-rw-r--r--   0        0        0    11579 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tables/v1.py
+-rw-r--r--   0        0        0       72 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/__init__.py
+-rw-r--r--   0        0        0     8392 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/_registration_utils.py
+-rw-r--r--   0        0        0     2407 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/_utils.py
+-rw-r--r--   0        0        0    13512 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/apply_registration_to_image.py
+-rw-r--r--   0        0        0     9371 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/calculate_registration_image_based.py
+-rw-r--r--   0        0        0    27519 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellpose_segmentation.py
+-rw-r--r--   0        0        0     8458 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellpose_transforms.py
+-rw-r--r--   0        0        0     7728 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_compute.py
+-rw-r--r--   0        0        0    18358 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py
+-rw-r--r--   0        0        0    21030 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py
+-rw-r--r--   0        0        0     2567 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/compress_tif.py
+-rw-r--r--   0        0        0    11207 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/copy_ome_zarr_hcs_plate.py
+-rw-r--r--   0        0        0     6384 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/find_registration_consensus.py
+-rw-r--r--   0        0        0    10249 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/illumination_correction.py
+-rw-r--r--   0        0        0     3603 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/image_based_registration_hcs_init.py
+-rw-r--r--   0        0        0    11691 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/import_ome_zarr.py
+-rw-r--r--   0        0        0     3039 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/init_group_by_well_for_multiplexing.py
+-rw-r--r--   0        0        0     4903 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/io_models.py
+-rw-r--r--   0        0        0     6188 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/maximum_intensity_projection.py
+-rw-r--r--   0        0        0    24797 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/napari_workflows_wrapper.py
+-rw-r--r--   0        0        0     7136 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/upscale_array.py
+-rw-r--r--   0        0        0     6101 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/utils.py
+-rw-r--r--   0        0        0     3890 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/fractal_tasks_core/zarr_utils.py
+-rw-r--r--   0        0        0     3431 2024-04-12 10:04:31.514002 fractal_tasks_core-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5764 1970-01-01 00:00:00.000000 fractal_tasks_core-1.0.0a0/PKG-INFO
```

### Comparing `fractal_tasks_core-0.9.4/LICENSE` & `fractal_tasks_core-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_tasks_core-0.9.4/README.md` & `fractal_tasks_core-1.0.0a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fractal Core Tasks
 
 [![PyPI version](https://img.shields.io/pypi/v/fractal-tasks-core?color=gree)](https://pypi.org/project/fractal-tasks-core/)
-[![CI Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci_pip.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci_pip.yml)
 [![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-tasks-core/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-tasks-core/blob/python-coverage-comment-action-data/htmlcov/index.html)
 [![Documentation Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal-tasks-core)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 Fractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.
 
 ![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)
@@ -31,8 +31,8 @@
 
 Some additional tasks are currently being worked on and some older tasks are still present in the fractal_tasks_core folder.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich by [@jluethi](https://github.com/jluethi) and [@gusqgm](https://github.com/gusqgm). The Fractal project is now developed at the [BioVisionCenter](https://www.biovisioncenter.uzh.ch/en.html) at the University of Zurich and the project lead is with [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](https://www.exact-lab.it/).
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/_utils.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,84 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Standard input/output interface for tasks
+Standard input/output interface for tasks.
 """
-# Starting from Python 3.9 (see PEP 585) we can use type hints like
-# `type[BaseModel]`. For versions 3.7 and 3.8, this is available through an
-# additional import
-from __future__ import annotations
-
 import json
 import logging
 from argparse import ArgumentParser
 from json import JSONEncoder
 from pathlib import Path
 from typing import Callable
-
-from pydantic import BaseModel
+from typing import Optional
 
 
 class TaskParameterEncoder(JSONEncoder):
     """
-    Custom JSONEncoder that transforms Path objects to strings
+    Custom JSONEncoder that transforms Path objects to strings.
     """
 
     def default(self, value):
+        """
+        Subclass implementation of `default`, to serialize Path objects as
+        strings.
+        """
         if isinstance(value, Path):
             return value.as_posix()
         return JSONEncoder.default(self, value)
 
 
 def run_fractal_task(
     *,
     task_function: Callable,
-    TaskArgsModel: type[BaseModel] = None,
-    logger_name: str = None,
+    logger_name: Optional[str] = None,
 ):
     """
-    Implement standard task interface and call task_function. If TaskArgsModel
-    is not None, validate arguments against given model.
+    Implement standard task interface and call task_function.
 
-    :param task_function: the callable function that runs the task
-    :param TaskArgsModel: a class specifying all types for task arguments
+    Args:
+        task_function: the callable function that runs the task.
+        logger_name: TBD
     """
 
     # Parse `-j` and `--metadata-out` arguments
     parser = ArgumentParser()
     parser.add_argument(
-        "-j", "--json", help="Read parameters from json file", required=True
+        "--args-json", help="Read parameters from json file", required=True
     )
     parser.add_argument(
-        "--metadata-out",
+        "--out-json",
         help="Output file to redirect serialised returned data",
         required=True,
     )
-    args = parser.parse_args()
+    parsed_args = parser.parse_args()
 
     # Set logger
     logger = logging.getLogger(logger_name)
 
     # Preliminary check
-    if Path(args.metadata_out).exists():
+    if Path(parsed_args.out_json).exists():
         logger.error(
-            f"Output file {args.metadata_out} already exists. Terminating"
+            f"Output file {parsed_args.out_json} already exists. Terminating"
         )
         exit(1)
 
     # Read parameters dictionary
-    with open(args.json, "r") as f:
+    with open(parsed_args.args_json, "r") as f:
         pars = json.load(f)
 
-    if TaskArgsModel is None:
-        # Run task without validating arguments' types
-        logger.info(f"START {task_function.__name__} task")
-        metadata_update = task_function(**pars)
-        logger.info(f"END {task_function.__name__} task")
-    else:
-        # Validating arguments' types and run task
-        task_args = TaskArgsModel(**pars)
-        logger.info(f"START {task_function.__name__} task")
-        metadata_update = task_function(**task_args.dict(exclude_unset=True))
-        logger.info(f"END {task_function.__name__} task")
+    # Run task
+    logger.info(f"START {task_function.__name__} task")
+    metadata_update = task_function(**pars)
+    logger.info(f"END {task_function.__name__} task")
 
     # Write output metadata to file, with custom JSON encoder
-    with open(args.metadata_out, "w") as fout:
-        json.dump(metadata_update, fout, cls=TaskParameterEncoder)
+    with open(parsed_args.out_json, "w") as fout:
+        json.dump(metadata_update, fout, cls=TaskParameterEncoder, indent=2)
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/cellpose_segmentation.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellpose_segmentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,178 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+# Joel Lüthi  <joel.luethi@fmi.ch>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Marco Franzon <marco.franzon@exact-lab.it>
-    Joel Lüthi  <joel.luethi@fmi.ch>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Image segmentation via Cellpose library
+Image segmentation via Cellpose library.
 """
-import json
 import logging
 import os
 import time
-from pathlib import Path
-from typing import Any
-from typing import Dict
+from typing import Literal
 from typing import Optional
-from typing import Sequence
 
 import anndata as ad
 import cellpose
 import dask.array as da
 import numpy as np
 import pandas as pd
 import zarr
-from anndata.experimental import write_elem
 from cellpose import models
+from pydantic.decorator import validate_arguments
 
 import fractal_tasks_core
-from fractal_tasks_core.lib_channels import ChannelNotFoundError
-from fractal_tasks_core.lib_channels import get_channel_from_image_zarr
-from fractal_tasks_core.lib_masked_loading import masked_loading_wrapper
-from fractal_tasks_core.lib_pyramid_creation import build_pyramid
-from fractal_tasks_core.lib_regions_of_interest import (
+from fractal_tasks_core.channels import ChannelInputModel
+from fractal_tasks_core.channels import ChannelNotFoundError
+from fractal_tasks_core.channels import get_channel_from_image_zarr
+from fractal_tasks_core.channels import OmeroChannel
+from fractal_tasks_core.labels import prepare_label_group
+from fractal_tasks_core.masked_loading import masked_loading_wrapper
+from fractal_tasks_core.ngff import load_NgffImageMeta
+from fractal_tasks_core.pyramids import build_pyramid
+from fractal_tasks_core.roi import (
     array_to_bounding_box_table,
 )
-from fractal_tasks_core.lib_regions_of_interest import (
+from fractal_tasks_core.roi import check_valid_ROI_indices
+from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
-from fractal_tasks_core.lib_regions_of_interest import is_ROI_table_valid
-from fractal_tasks_core.lib_ROI_overlaps import find_overlaps_in_ROI_indices
-from fractal_tasks_core.lib_ROI_overlaps import get_overlapping_pairs_3D
-from fractal_tasks_core.lib_zattrs_utils import extract_zyx_pixel_sizes
-from fractal_tasks_core.lib_zattrs_utils import rescale_datasets
+from fractal_tasks_core.roi import empty_bounding_box_table
+from fractal_tasks_core.roi import (
+    find_overlaps_in_ROI_indices,
+)
+from fractal_tasks_core.roi import get_overlapping_pairs_3D
+from fractal_tasks_core.roi import is_ROI_table_valid
+from fractal_tasks_core.roi import load_region
+from fractal_tasks_core.tables import write_table
+from fractal_tasks_core.tasks.cellpose_transforms import (
+    CellposeCustomNormalizer,
+)
+from fractal_tasks_core.tasks.cellpose_transforms import normalized_img
+from fractal_tasks_core.utils import rescale_datasets
 
 logger = logging.getLogger(__name__)
 
 __OME_NGFF_VERSION__ = fractal_tasks_core.__OME_NGFF_VERSION__
 
 
 def segment_ROI(
     x: np.ndarray,
     model: models.CellposeModel = None,
     do_3D: bool = True,
-    channels=[0, 0],
+    channels: list[int] = [0, 0],
     anisotropy: Optional[float] = None,
     diameter: float = 30.0,
     cellprob_threshold: float = 0.0,
     flow_threshold: float = 0.4,
+    normalize: CellposeCustomNormalizer = CellposeCustomNormalizer(),
     label_dtype: Optional[np.dtype] = None,
     augment: bool = False,
     net_avg: bool = False,
     min_size: int = 15,
+    batch_size: int = 8,
+    invert: bool = False,
+    tile: bool = True,
+    tile_overlap: float = 0.1,
+    resample: bool = True,
+    interp: bool = True,
+    stitch_threshold: float = 0.0,
 ) -> np.ndarray:
     """
     Internal function that runs Cellpose segmentation for a single ROI.
 
-    :param x: 4D numpy array
-    :param model: An instance of models.CellposeModel
-    :param do_3D: If true, cellpose runs in 3D mode: runs on xy, xz & yz
-                  planes, then averages the flows.
-    :param channels: Which channels to use. If only one channel is provided,
-                     [0, 0] should be used. If two channels are provided
-                     (the first dimension of x has lenth of 2), [[1, 2]]
-                     should be used (x[0, :, :, :] contains the membrane
-                     channel first & x[1, :, :, :] the nuclear channel).
-    :param anisotropy: Set anisotropy rescaling factor for Z dimension
-    :param diameter: Expected object diameter in pixels for cellpose
-    :param cellprob_threshold: Cellpose model parameter
-    :param flow_threshold: Cellpose model parameter
-    :param label_dtype: Label images are cast into this np.dtype
-    :param augment: Whether to use cellpose augmentation to tile images
-                    with overlap
-    :param net_avg: Whether to use cellpose net averaging to run the 4 built-in
-                    networks (useful for nuclei, cyto & cyto2, not sure it
-                    works for the others)
-    :param min_size: Minimum size of the segmented objects
+    Args:
+        x: 4D numpy array.
+        model: An instance of `models.CellposeModel`.
+        do_3D: If `True`, cellpose runs in 3D mode: runs on xy, xz & yz planes,
+            then averages the flows.
+        channels: Which channels to use. If only one channel is provided, `[0,
+            0]` should be used. If two channels are provided (the first
+            dimension of `x` has length of 2), `[1, 2]` should be used
+            (`x[0, :, :,:]` contains the membrane channel and
+            `x[1, :, :, :]` contains the nuclear channel).
+        anisotropy: Set anisotropy rescaling factor for Z dimension.
+        diameter: Expected object diameter in pixels for cellpose.
+        cellprob_threshold: Cellpose model parameter.
+        flow_threshold: Cellpose model parameter.
+        normalize: normalize data so 0.0=1st percentile and 1.0=99th
+            percentile of image intensities in each channel. This automatic
+            normalization can lead to issues when the image to be segmented
+            is very sparse.
+        label_dtype: Label images are cast into this `np.dtype`.
+        augment: Whether to use cellpose augmentation to tile images with
+            overlap.
+        net_avg: Whether to use cellpose net averaging to run the 4 built-in
+            networks (useful for `nuclei`, `cyto` and `cyto2`, not sure it
+            works for the others).
+        min_size: Minimum size of the segmented objects.
+        batch_size: number of 224x224 patches to run simultaneously on the GPU
+            (can make smaller or bigger depending on GPU memory usage)
+        invert: invert image pixel intensity before running network (if True,
+            image is also normalized)
+        tile: tiles image to ensure GPU/CPU memory usage limited (recommended)
+        tile_overlap: fraction of overlap of tiles when computing flows
+        resample: run dynamics at original image size (will be slower but
+            create more accurate boundaries)
+        interp: interpolate during 2D dynamics (not available in 3D)
+            (in previous versions it was False, now it defaults to True)
+        stitch_threshold: if stitch_threshold>0.0 and not do_3D and equal
+            image sizes, masks are stitched in 3D to return volume segmentation
     """
 
     # Write some debugging info
     logger.info(
         "[segment_ROI] START |"
         f" x: {type(x)}, {x.shape} |"
         f" {do_3D=} |"
         f" {model.diam_mean=} |"
         f" {diameter=} |"
-        f" {flow_threshold=}"
+        f" {flow_threshold=} |"
+        f" {normalize.type=}"
     )
 
+    # Optionally perform custom normalization
+    if normalize.type == "custom":
+        x = normalized_img(
+            x,
+            lower_p=normalize.lower_percentile,
+            upper_p=normalize.upper_percentile,
+            lower_bound=normalize.lower_bound,
+            upper_bound=normalize.upper_bound,
+        )
+
     # Actual labeling
     t0 = time.perf_counter()
     mask, _, _ = model.eval(
         x,
         channels=channels,
         do_3D=do_3D,
         net_avg=net_avg,
         augment=augment,
         diameter=diameter,
         anisotropy=anisotropy,
         cellprob_threshold=cellprob_threshold,
         flow_threshold=flow_threshold,
+        normalize=normalize.cellpose_normalize,
         min_size=min_size,
+        batch_size=batch_size,
+        invert=invert,
+        tile=tile,
+        tile_overlap=tile_overlap,
+        resample=resample,
+        interp=interp,
+        stitch_threshold=stitch_threshold,
     )
 
     if mask.ndim == 2:
         # If we get a 2D image, we still return it as a 3D array
         mask = np.expand_dims(mask, axis=0)
     t1 = time.perf_counter()
 
@@ -136,321 +187,311 @@
         f" {diameter=} |"
         f" {flow_threshold=}"
     )
 
     return mask.astype(label_dtype)
 
 
+@validate_arguments
 def cellpose_segmentation(
     *,
-    # Fractal arguments
-    input_paths: Sequence[str],
-    output_path: str,
-    component: str,
-    metadata: Dict[str, Any],
+    # Fractal argument
+    zarr_url: str,
     # Task-specific arguments
     level: int,
-    wavelength_id: Optional[str] = None,
-    channel_label: Optional[str] = None,
-    wavelength_id_c2: Optional[str] = None,
-    channel_label_c2: Optional[str] = None,
+    channel: ChannelInputModel,
+    channel2: Optional[ChannelInputModel] = None,
     input_ROI_table: str = "FOV_ROI_table",
     output_ROI_table: Optional[str] = None,
-    output_label_name: Optional[str] = None,  # "organoids"
+    output_label_name: Optional[str] = None,
     use_masks: bool = True,
     relabeling: bool = True,
     # Cellpose-related arguments
-    use_gpu: bool = True,
-    anisotropy: Optional[float] = None,
     diameter_level0: float = 30.0,
+    # https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/401 # noqa E501
+    model_type: Literal[tuple(models.MODEL_NAMES)] = "cyto2",
+    pretrained_model: Optional[str] = None,
     cellprob_threshold: float = 0.0,
     flow_threshold: float = 0.4,
-    model_type: str = "cyto2",
-    pretrained_model: Optional[str] = None,
+    normalize: CellposeCustomNormalizer = CellposeCustomNormalizer(),
+    anisotropy: Optional[float] = None,
     min_size: int = 15,
     augment: bool = False,
     net_avg: bool = False,
-) -> Dict[str, Any]:
+    use_gpu: bool = True,
+    batch_size: int = 8,
+    invert: bool = False,
+    tile: bool = True,
+    tile_overlap: float = 0.1,
+    resample: bool = True,
+    interp: bool = True,
+    stitch_threshold: float = 0.0,
+    # Overwrite option
+    overwrite: bool = True,
+) -> None:
     """
-    Run cellpose segmentation on the ROIs of a single OME-NGFF image
+    Run cellpose segmentation on the ROIs of a single OME-Zarr image.
 
-    Full documentation for all arguments is still TBD, especially because some
-    of them are standard arguments for Fractal tasks that should be documented
-    in a standard way. Here are some examples of valid arguments::
-
-        input_paths = ["/some/path/"]
-        output_path = "/some/path/"
-        component = "some_plate.zarr/B/03/0"
-        metadata = {"num_levels": 4, "coarsening_xy": 2}
-
-    :param input_paths: TBD (default arg for Fractal tasks)
-    :param output_path: TBD (default arg for Fractal tasks)
-    :param metadata: TBD (default arg for Fractal tasks)
-    :param component: TBD (default arg for Fractal tasks)
-    :param level: Pyramid level of the image to be segmented.
-    :param wavelength_id: Identifier of a channel based on the
-                          wavelength (e.g. ``A01_C01``). If not ``None``, then
-                          ``channel_label` must be ``None``.
-    :param channel_label: Identifier of a channel based on its label (e.g.
-                          ``DAPI``). If not ``None``, then ``wavelength_id``
-                          must be ``None``.
-    :param wavelength_id_c2: Identifier of a second channel in the same format
-                             as the first wavelength_id. If specified, cellpose
-                             runs in dual channel mode.  For dual channel
-                             segmentation of cells, the first channel should
-                             contain the membrane marker, the second channel
-                             should contain the nuclear marker.
-    :param channel_label_c2: Identifier of a second channel in the same
-                             format as the first wavelength_id. If specified,
-                             cellpose runs in dual channel mode.  For dual
-                             channel segmentation of cells, the first channel
-                             should contain the membrane marker, the second
-                             channel should contain the nuclear marker.
-    :param input_ROI_table: Name of the table that contains ROIs to which the
-                            task applies Cellpose segmentation (e.g.
-                            ``"organoid_rois"``).
-    :param output_ROI_table: If provided, the name of the ROI table used for
-                             label bounding boxes.
-    :param use_masks: If ``True``, try to use masked loading and fall back
-                      to ``use_masks=False`` if the ROI table is not suitable.
-    :param output_label_name: Name of the output label (e.g. ``"organoids"``).
-    :param relabeling: If ``True``, apply relabeling so that label values are
-                       unique across ROIs.
-    :param use_gpu: If ``False``, always use the CPU; if ``True``, use the GPU
-                    if possible (as defined in ``cellpose.core.use_gpu()``) and
-                    fall-back to the CPU otherwise.
-    :param anisotropy: Ratio of the pixel sizes along Z and XY axis (ignored if
-                       the image is not three-dimensional). If `None`, it is
-                       inferred from the OME-NGFF metadata.
-    :param diameter_level0: Initial diameter to be passed to
-                            ``CellposeModel.eval`` method (after rescaling from
-                            full-resolution to ``level``).
-    :param cellprob_threshold: Parameter of ``CellposeModel.eval`` method.
-    :param flow_threshold: Parameter of ``CellposeModel.eval`` method.
-    :param model_type: Parameter of ``CellposeModel`` class.
-    :param pretrained_model: Parameter of ``CellposeModel`` class (takes
-                             precedence over ``model_type``).
-    :param min_size: Minimum size of the segmented objects (in pixels). Use -1
-                     to turn off the size filter.
-    :param augment: Whether to use cellpose augmentation to tile images with
-                    overlap.
-    :param net_avg: Whether to use cellpose net averaging to run the 4 built-in
-                    networks (useful for nuclei, cyto & cyto2, not sure it
-                    works for the others).
+    Args:
+        zarr_url: Path or url to the individual OME-Zarr image to be processed.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        level: Pyramid level of the image to be segmented. Choose `0` to
+            process at full resolution.
+        channel: Primary channel for segmentation; requires either
+            `wavelength_id` (e.g. `A01_C01`) or `label` (e.g. `DAPI`).
+        channel2: Second channel for segmentation (in the same format as
+            `channel`). If specified, cellpose runs in dual channel mode.
+            For dual channel segmentation of cells, the first channel should
+            contain the membrane marker, the second channel should contain the
+            nuclear marker.
+        input_ROI_table: Name of the ROI table over which the task loops to
+            apply Cellpose segmentation. Examples: `FOV_ROI_table` => loop over
+            the field of views, `organoid_ROI_table` => loop over the organoid
+            ROI table (generated by another task), `well_ROI_table` => process
+            the whole well as one image.
+        output_ROI_table: If provided, a ROI table with that name is created,
+            which will contain the bounding boxes of the newly segmented
+            labels. ROI tables should have `ROI` in their name.
+        use_masks: If `True`, try to use masked loading and fall back to
+            `use_masks=False` if the ROI table is not suitable. Masked
+            loading is relevant when only a subset of the bounding box should
+            actually be processed (e.g. running within `organoid_ROI_table`).
+        output_label_name: Name of the output label image (e.g. `"organoids"`).
+        relabeling: If `True`, apply relabeling so that label values are
+            unique for all objects in the well.
+        diameter_level0: Expected diameter of the objects that should be
+            segmented in pixels at level 0. Initial diameter is rescaled using
+            the `level` that was selected. The rescaled value is passed as
+            the diameter to the `CellposeModel.eval` method.
+        model_type: Parameter of `CellposeModel` class. Defines which model
+            should be used. Typical choices are `nuclei`, `cyto`, `cyto2`, etc.
+        pretrained_model: Parameter of `CellposeModel` class (takes
+            precedence over `model_type`). Allows you to specify the path of
+            a custom trained cellpose model.
+        cellprob_threshold: Parameter of `CellposeModel.eval` method. Valid
+            values between -6 to 6. From Cellpose documentation: "Decrease this
+            threshold if cellpose is not returning as many ROIs as you’d
+            expect. Similarly, increase this threshold if cellpose is returning
+            too ROIs particularly from dim areas."
+        flow_threshold: Parameter of `CellposeModel.eval` method. Valid
+            values between 0.0 and 1.0. From Cellpose documentation: "Increase
+            this threshold if cellpose is not returning as many ROIs as you’d
+            expect. Similarly, decrease this threshold if cellpose is returning
+            too many ill-shaped ROIs."
+        normalize: By default, data is normalized so 0.0=1st percentile and
+            1.0=99th percentile of image intensities in each channel.
+            This automatic normalization can lead to issues when the image to
+            be segmented is very sparse. You can turn off the default
+            rescaling. With the "custom" option, you can either provide your
+            own rescaling percentiles or fixed rescaling upper and lower
+            bound integers.
+        anisotropy: Ratio of the pixel sizes along Z and XY axis (ignored if
+            the image is not three-dimensional). If `None`, it is inferred from
+            the OME-NGFF metadata.
+        min_size: Parameter of `CellposeModel` class. Minimum size of the
+            segmented objects (in pixels). Use `-1` to turn off the size
+            filter.
+        augment: Parameter of `CellposeModel` class. Whether to use cellpose
+            augmentation to tile images with overlap.
+        net_avg: Parameter of `CellposeModel` class. Whether to use cellpose
+            net averaging to run the 4 built-in networks (useful for `nuclei`,
+            `cyto` and `cyto2`, not sure it works for the others).
+        use_gpu: If `False`, always use the CPU; if `True`, use the GPU if
+            possible (as defined in `cellpose.core.use_gpu()`) and fall-back
+            to the CPU otherwise.
+        batch_size: number of 224x224 patches to run simultaneously on the GPU
+            (can make smaller or bigger depending on GPU memory usage)
+        invert: invert image pixel intensity before running network (if True,
+            image is also normalized)
+        tile: tiles image to ensure GPU/CPU memory usage limited (recommended)
+        tile_overlap: fraction of overlap of tiles when computing flows
+        resample: run dynamics at original image size (will be slower but
+            create more accurate boundaries)
+        interp: interpolate during 2D dynamics (not available in 3D)
+            (in previous versions it was False, now it defaults to True)
+        stitch_threshold: if stitch_threshold>0.0 and not do_3D and equal
+            image sizes, masks are stitched in 3D to return volume segmentation
+        overwrite: If `True`, overwrite the task output.
     """
 
     # Set input path
-    if len(input_paths) > 1:
-        raise NotImplementedError
-    in_path = Path(input_paths[0])
-    zarrurl = (in_path.resolve() / component).as_posix()
-    logger.info(f"{zarrurl=}")
-
-    # Preliminary check
-    if (channel_label is None and wavelength_id is None) or (
-        channel_label and wavelength_id
-    ):
-        raise ValueError(
-            f"One and only one of {channel_label=} and "
-            f"{wavelength_id=} arguments must be provided"
-        )
+    logger.info(f"{zarr_url=}")
 
-    # Prelminary checks on Cellpose model
-    if pretrained_model is None:
-        if model_type not in models.MODEL_NAMES:
-            raise ValueError(f"ERROR model_type={model_type} is not allowed.")
-    else:
+    # Preliminary checks on Cellpose model
+    if pretrained_model:
         if not os.path.exists(pretrained_model):
             raise ValueError(f"{pretrained_model=} does not exist.")
 
-    # Read useful parameters from metadata
-    num_levels = metadata["num_levels"]
-    coarsening_xy = metadata["coarsening_xy"]
-
-    plate, well = component.split(".zarr/")
+    # Read attributes from NGFF metadata
+    ngff_image_meta = load_NgffImageMeta(zarr_url)
+    num_levels = ngff_image_meta.num_levels
+    coarsening_xy = ngff_image_meta.coarsening_xy
+    full_res_pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=0)
+    actual_res_pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=level)
+    logger.info(f"NGFF image has {num_levels=}")
+    logger.info(f"NGFF image has {coarsening_xy=}")
+    logger.info(
+        f"NGFF image has full-res pixel sizes {full_res_pxl_sizes_zyx}"
+    )
+    logger.info(
+        f"NGFF image has level-{level} pixel sizes "
+        f"{actual_res_pxl_sizes_zyx}"
+    )
 
     # Find channel index
     try:
-        channel = get_channel_from_image_zarr(
-            image_zarr_path=zarrurl,
-            wavelength_id=wavelength_id,
-            label=channel_label,
+        tmp_channel: OmeroChannel = get_channel_from_image_zarr(
+            image_zarr_path=zarr_url,
+            wavelength_id=channel.wavelength_id,
+            label=channel.label,
         )
     except ChannelNotFoundError as e:
         logger.warning(
             "Channel not found, exit from the task.\n"
             f"Original error: {str(e)}"
         )
-        return {}
-    ind_channel = channel["index"]
+        return None
+    ind_channel = tmp_channel.index
 
     # Find channel index for second channel, if one is provided
-    if wavelength_id_c2 or channel_label_c2:
+    if channel2:
         try:
-            channel_c2 = get_channel_from_image_zarr(
-                image_zarr_path=zarrurl,
-                wavelength_id=wavelength_id_c2,
-                label=channel_label_c2,
+            tmp_channel_c2: OmeroChannel = get_channel_from_image_zarr(
+                image_zarr_path=zarr_url,
+                wavelength_id=channel2.wavelength_id,
+                label=channel2.label,
             )
         except ChannelNotFoundError as e:
             logger.warning(
-                f"Second channel with wavelength_id_c2:{wavelength_id_c2} and "
-                f"channel_label_c2: {channel_label_c2} not found, exit "
-                "from the task.\n"
+                f"Second channel with wavelength_id: {channel2.wavelength_id} "
+                f"and label: {channel2.label} not found, exit from the task.\n"
                 f"Original error: {str(e)}"
             )
-            return {}
-        ind_channel_c2 = channel_c2["index"]
+            return None
+        ind_channel_c2 = tmp_channel_c2.index
 
     # Set channel label
     if output_label_name is None:
         try:
-            channel_label = channel["label"]
+            channel_label = tmp_channel.label
             output_label_name = f"label_{channel_label}"
         except (KeyError, IndexError):
             output_label_name = f"label_{ind_channel}"
 
     # Load ZYX data
-    data_zyx = da.from_zarr(f"{zarrurl}/{level}")[ind_channel]
+    data_zyx = da.from_zarr(f"{zarr_url}/{level}")[ind_channel]
     logger.info(f"{data_zyx.shape=}")
-    if wavelength_id_c2 or channel_label_c2:
-        data_zyx_c2 = da.from_zarr(f"{zarrurl}/{level}")[ind_channel_c2]
+    if channel2:
+        data_zyx_c2 = da.from_zarr(f"{zarr_url}/{level}")[ind_channel_c2]
         logger.info(f"Second channel: {data_zyx_c2.shape=}")
 
     # Read ROI table
-    ROI_table_path = f"{zarrurl}/tables/{input_ROI_table}"
+    ROI_table_path = f"{zarr_url}/tables/{input_ROI_table}"
     ROI_table = ad.read_zarr(ROI_table_path)
 
     # Perform some checks on the ROI table
     valid_ROI_table = is_ROI_table_valid(
         table_path=ROI_table_path, use_masks=use_masks
     )
     if use_masks and not valid_ROI_table:
         logger.info(
             f"ROI table at {ROI_table_path} cannot be used for masked "
             "loading. Set use_masks=False."
         )
         use_masks = False
     logger.info(f"{use_masks=}")
 
-    # Read pixel sizes from zattrs file
-    full_res_pxl_sizes_zyx = extract_zyx_pixel_sizes(
-        f"{zarrurl}/.zattrs", level=0
-    )
-    actual_res_pxl_sizes_zyx = extract_zyx_pixel_sizes(
-        f"{zarrurl}/.zattrs", level=level
-    )
-
-    # Heuristic to determine reset_origin   # FIXME, see issue #339
-    if input_ROI_table in ["FOV_ROI_table", "well_ROI_table"]:
-        reset_origin = True
-    else:
-        reset_origin = False
-    logger.info(f"{reset_origin=}")
-
     # Create list of indices for 3D ROIs spanning the entire Z direction
     list_indices = convert_ROI_table_to_indices(
         ROI_table,
         level=level,
         coarsening_xy=coarsening_xy,
         full_res_pxl_sizes_zyx=full_res_pxl_sizes_zyx,
-        reset_origin=reset_origin,
     )
+    check_valid_ROI_indices(list_indices, input_ROI_table)
 
     # If we are not planning to use masked loading, fail for overlapping ROIs
     if not use_masks:
         overlap = find_overlaps_in_ROI_indices(list_indices)
         if overlap:
             raise ValueError(
                 f"ROI indices created from {input_ROI_table} table have "
                 "overlaps, but we are not using masked loading."
             )
 
     # Select 2D/3D behavior and set some parameters
-    do_3D = data_zyx.shape[0] > 1
+    do_3D = data_zyx.shape[0] > 1 and len(data_zyx.shape) == 3
     if do_3D:
         if anisotropy is None:
-            # Read pixel sizes from zattrs file
-            pxl_zyx = extract_zyx_pixel_sizes(
-                f"{zarrurl}/.zattrs", level=level
+            # Compute anisotropy as pixel_size_z/pixel_size_x
+            anisotropy = (
+                actual_res_pxl_sizes_zyx[0] / actual_res_pxl_sizes_zyx[2]
             )
-            pixel_size_z, pixel_size_y, pixel_size_x = pxl_zyx[:]
-            logger.info(f"{pxl_zyx=}")
-            if not np.allclose(pixel_size_x, pixel_size_y):
-                raise Exception(
-                    "ERROR: XY anisotropy detected"
-                    f"pixel_size_x={pixel_size_x}"
-                    f"pixel_size_y={pixel_size_y}"
-                )
-            anisotropy = pixel_size_z / pixel_size_x
-
-    # Load zattrs file
-    zattrs_file = f"{zarrurl}/.zattrs"
-    with open(zattrs_file, "r") as jsonfile:
-        zattrs = json.load(jsonfile)
-
-    # Preliminary checks on multiscales
-    multiscales = zattrs["multiscales"]
-    if len(multiscales) > 1:
-        raise NotImplementedError(
-            f"Found {len(multiscales)} multiscales, "
-            "but only one is currently supported."
-        )
-    if "coordinateTransformations" in multiscales[0].keys():
-        raise NotImplementedError(
-            "global coordinateTransformations at the multiscales "
-            "level are not currently supported"
-        )
+        logger.info(f"Anisotropy: {anisotropy}")
 
     # Rescale datasets (only relevant for level>0)
+    if ngff_image_meta.axes_names[0] != "c":
+        raise ValueError(
+            "Cannot set `remove_channel_axis=True` for multiscale "
+            f"metadata with axes={ngff_image_meta.axes_names}. "
+            'First axis should have name "c".'
+        )
     new_datasets = rescale_datasets(
-        datasets=multiscales[0]["datasets"],
+        datasets=[ds.dict() for ds in ngff_image_meta.datasets],
         coarsening_xy=coarsening_xy,
         reference_level=level,
+        remove_channel_axis=True,
     )
 
-    # Write zattrs for labels and for specific label
-    new_labels = [output_label_name]
-    try:
-        with open(f"{zarrurl}/labels/.zattrs", "r") as f_zattrs:
-            existing_labels = json.load(f_zattrs)["labels"]
-    except FileNotFoundError:
-        existing_labels = []
-    intersection = set(new_labels) & set(existing_labels)
-    logger.info(f"{new_labels=}")
-    logger.info(f"{existing_labels=}")
-    if intersection:
-        raise RuntimeError(
-            f"Labels {intersection} already exist but are also part of outputs"
-        )
-    labels_group = zarr.group(f"{zarrurl}/labels")
-    labels_group.attrs["labels"] = existing_labels + new_labels
-
-    label_group = labels_group.create_group(output_label_name)
-    label_group.attrs["image-label"] = {"version": __OME_NGFF_VERSION__}
-    label_group.attrs["multiscales"] = [
-        {
-            "name": output_label_name,
+    label_attrs = {
+        "image-label": {
             "version": __OME_NGFF_VERSION__,
-            "axes": [
-                ax for ax in multiscales[0]["axes"] if ax["type"] != "channel"
-            ],
-            "datasets": new_datasets,
-        }
-    ]
+            "source": {"image": "../../"},
+        },
+        "multiscales": [
+            {
+                "name": output_label_name,
+                "version": __OME_NGFF_VERSION__,
+                "axes": [
+                    ax.dict()
+                    for ax in ngff_image_meta.multiscale.axes
+                    if ax.type != "channel"
+                ],
+                "datasets": new_datasets,
+            }
+        ],
+    }
+
+    image_group = zarr.group(zarr_url)
+    label_group = prepare_label_group(
+        image_group,
+        output_label_name,
+        overwrite=overwrite,
+        label_attrs=label_attrs,
+        logger=logger,
+    )
 
-    # Open new zarr group for mask 0-th level
-    zarr.group(f"{zarrurl}/labels")
-    zarr.group(f"{zarrurl}/labels/{output_label_name}")
-    logger.info(f"Output label path: {zarrurl}/labels/{output_label_name}/0")
-    store = zarr.storage.FSStore(f"{zarrurl}/labels/{output_label_name}/0")
+    logger.info(
+        f"Helper function `prepare_label_group` returned {label_group=}"
+    )
+    logger.info(f"Output label path: {zarr_url}/labels/{output_label_name}/0")
+    store = zarr.storage.FSStore(f"{zarr_url}/labels/{output_label_name}/0")
     label_dtype = np.uint32
+
+    # Ensure that all output shapes & chunks are 3D (for 2D data: (1, y, x))
+    # https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/398
+    shape = data_zyx.shape
+    if len(shape) == 2:
+        shape = (1, *shape)
+    chunks = data_zyx.chunksize
+    if len(chunks) == 2:
+        chunks = (1, *chunks)
     mask_zarr = zarr.create(
-        shape=data_zyx.shape,
-        chunks=data_zyx.chunksize,
+        shape=shape,
+        chunks=chunks,
         dtype=label_dtype,
         store=store,
         overwrite=False,
         dimension_separator="/",
     )
 
     logger.info(
@@ -464,26 +505,26 @@
         model = models.CellposeModel(
             gpu=gpu, pretrained_model=pretrained_model
         )
     else:
         model = models.CellposeModel(gpu=gpu, model_type=model_type)
 
     # Initialize other things
-    logger.info(f"Start cellpose_segmentation task for {zarrurl}")
+    logger.info(f"Start cellpose_segmentation task for {zarr_url}")
     logger.info(f"relabeling: {relabeling}")
     logger.info(f"do_3D: {do_3D}")
     logger.info(f"use_gpu: {gpu}")
     logger.info(f"level: {level}")
     logger.info(f"model_type: {model_type}")
     logger.info(f"pretrained_model: {pretrained_model}")
     logger.info(f"anisotropy: {anisotropy}")
     logger.info("Total well shape/chunks:")
     logger.info(f"{data_zyx.shape}")
     logger.info(f"{data_zyx.chunks}")
-    if wavelength_id_c2 or channel_label_c2:
+    if channel2:
         logger.info("Dual channel input for cellpose model")
         logger.info(f"{data_zyx_c2.shape}")
         logger.info(f"{data_zyx_c2.chunks}")
 
     # Counters for relabeling
     if relabeling:
         num_labels_tot = 0
@@ -502,45 +543,67 @@
             slice(s_z, e_z),
             slice(s_y, e_y),
             slice(s_x, e_x),
         )
         logger.info(f"Now processing ROI {i_ROI+1}/{num_ROIs}")
 
         # Prepare single-channel or dual-channel input for cellpose
-        if wavelength_id_c2 or channel_label_c2:
+        if channel2:
             # Dual channel mode, first channel is the membrane channel
-            img_np = np.zeros((2, *data_zyx[region].shape))
-            img_np[0, :, :, :] = data_zyx[region].compute()
-            img_np[1, :, :, :] = data_zyx_c2[region].compute()
+            img_1 = load_region(
+                data_zyx,
+                region,
+                compute=True,
+                return_as_3D=True,
+            )
+            img_np = np.zeros((2, *img_1.shape))
+            img_np[0, :, :, :] = img_1
+            img_np[1, :, :, :] = load_region(
+                data_zyx_c2,
+                region,
+                compute=True,
+                return_as_3D=True,
+            )
             channels = [1, 2]
         else:
-            img_np = np.expand_dims(data_zyx[region].compute(), axis=0)
+            img_np = np.expand_dims(
+                load_region(data_zyx, region, compute=True, return_as_3D=True),
+                axis=0,
+            )
             channels = [0, 0]
 
         # Prepare keyword arguments for segment_ROI function
         kwargs_segment_ROI = dict(
             model=model,
             channels=channels,
             do_3D=do_3D,
             anisotropy=anisotropy,
             label_dtype=label_dtype,
             diameter=diameter_level0 / coarsening_xy**level,
             cellprob_threshold=cellprob_threshold,
             flow_threshold=flow_threshold,
+            normalize=normalize,
             min_size=min_size,
             augment=augment,
             net_avg=net_avg,
+            batch_size=batch_size,
+            invert=invert,
+            tile=tile,
+            tile_overlap=tile_overlap,
+            resample=resample,
+            interp=interp,
+            stitch_threshold=stitch_threshold,
         )
 
         # Prepare keyword arguments for preprocessing function
         preprocessing_kwargs = {}
         if use_masks:
             preprocessing_kwargs = dict(
                 region=region,
-                current_label_path=f"{zarrurl}/labels/{output_label_name}/0",
+                current_label_path=f"{zarr_url}/labels/{output_label_name}/0",
                 ROI_table_path=ROI_table_path,
                 ROI_positional_index=i_ROI,
             )
 
         # Call segment_ROI through the masked-loading wrapper, which includes
         # pre/post-processing functions if needed
         new_label_img = masked_loading_wrapper(
@@ -554,30 +617,29 @@
         # Shift labels and update relabeling counters
         if relabeling:
             num_labels_roi = np.max(new_label_img)
             new_label_img[new_label_img > 0] += num_labels_tot
             num_labels_tot += num_labels_roi
 
             # Write some logs
-            logger.info(
-                f"ROI {indices}, " f"{num_labels_roi=}, " f"{num_labels_tot=}"
-            )
+            logger.info(f"ROI {indices}, {num_labels_roi=}, {num_labels_tot=}")
 
             # Check that total number of labels is under control
             if num_labels_tot > np.iinfo(label_dtype).max:
-                raise Exception(
+                raise ValueError(
                     "ERROR in re-labeling:"
                     f"Reached {num_labels_tot} labels, "
                     f"but dtype={label_dtype}"
                 )
 
         if output_ROI_table:
-
             bbox_df = array_to_bounding_box_table(
-                new_label_img, actual_res_pxl_sizes_zyx
+                new_label_img,
+                actual_res_pxl_sizes_zyx,
+                origin_zyx=(s_z, s_y, s_x),
             )
 
             bbox_dataframe_list.append(bbox_df)
 
             overlap_list = []
             for df in bbox_dataframe_list:
                 overlap_list.extend(
@@ -592,112 +654,69 @@
         da.array(new_label_img).to_zarr(
             url=mask_zarr,
             region=region,
             compute=True,
         )
 
     logger.info(
-        f"End cellpose_segmentation task for {zarrurl}, "
+        f"End cellpose_segmentation task for {zarr_url}, "
         "now building pyramids."
     )
 
     # Starting from on-disk highest-resolution data, build and write to disk a
     # pyramid of coarser levels
     build_pyramid(
-        zarrurl=f"{zarrurl}/labels/{output_label_name}",
-        overwrite=False,
+        zarrurl=f"{zarr_url}/labels/{output_label_name}",
+        overwrite=overwrite,
         num_levels=num_levels,
         coarsening_xy=coarsening_xy,
-        chunksize=data_zyx.chunksize,
+        chunksize=chunks,
         aggregation_function=np.max,
     )
 
     logger.info("End building pyramids")
 
     if output_ROI_table:
+        # Handle the case where `bbox_dataframe_list` is empty (typically
+        # because list_indices is also empty)
+        if len(bbox_dataframe_list) == 0:
+            bbox_dataframe_list = [empty_bounding_box_table()]
         # Concatenate all ROI dataframes
         df_well = pd.concat(bbox_dataframe_list, axis=0, ignore_index=True)
         df_well.index = df_well.index.astype(str)
         # Extract labels and drop them from df_well
         labels = pd.DataFrame(df_well["label"].astype(str))
         df_well.drop(labels=["label"], axis=1, inplace=True)
         # Convert all to float (warning: some would be int, in principle)
         bbox_dtype = np.float32
         df_well = df_well.astype(bbox_dtype)
         # Convert to anndata
         bbox_table = ad.AnnData(df_well, dtype=bbox_dtype)
         bbox_table.obs = labels
+
         # Write to zarr group
-        group_tables = zarr.group(f"{in_path}/{component}/tables/")
-        write_elem(group_tables, output_ROI_table, bbox_table)
+        image_group = zarr.group(zarr_url)
         logger.info(
-            "Bounding box ROI table written to "
-            f"{in_path}/{component}/tables/{output_ROI_table}"
+            "Now writing bounding-box ROI table to "
+            f"{zarr_url}/tables/{output_ROI_table}"
         )
-
-        # WARNING: the following OME-NGFF metadata are based on a proposed
-        # change to the specs (https://github.com/ome/ngff/pull/64)
-
-        # Update OME-NGFF metadata for tables group
-        current_tables = group_tables.attrs.asdict().get("tables") or []
-        if output_ROI_table in current_tables:
-            # FIXME: move this check to an earlier stage of the task
-            raise ValueError(
-                f"{in_path}/{component}/tables/ already includes "
-                f"{output_ROI_table=} in {current_tables=}"
-            )
-        new_tables = current_tables + [output_ROI_table]
-        group_tables.attrs["tables"] = new_tables
-
-        # Update OME-NGFF metadata for current-table group
-        bbox_table_group = zarr.group(
-            f"{in_path}/{component}/tables/{output_ROI_table}"
-        )
-        bbox_table_group.attrs["type"] = "ngff:region_table"
-        bbox_table_group.attrs["region"] = {
-            "path": f"../labels/{output_label_name}"
+        table_attrs = {
+            "type": "masking_roi_table",
+            "region": {"path": f"../labels/{output_label_name}"},
+            "instance_key": "label",
         }
-        bbox_table_group.attrs["instance_key"] = "label"
-
-    return {}
+        write_table(
+            image_group,
+            output_ROI_table,
+            bbox_table,
+            overwrite=overwrite,
+            table_attrs=table_attrs,
+        )
 
 
 if __name__ == "__main__":
-
-    from pydantic import BaseModel
-    from pydantic import Extra
-    from fractal_tasks_core._utils import run_fractal_task
-
-    class TaskArguments(BaseModel, extra=Extra.forbid):
-        # Fractal arguments
-        input_paths: Sequence[str]
-        output_path: str
-        component: str
-        metadata: Dict[str, Any]
-        # Task-specific arguments
-        channel_label: Optional[str]
-        wavelength_id: Optional[str]
-        channel_label_c2: Optional[str]
-        channel_label_c2: Optional[str]
-        level: int
-        relabeling: bool = True
-        input_ROI_table: Optional[str]
-        output_ROI_table: Optional[str]
-        output_label_name: Optional[str]
-        # Cellpose-related arguments:
-        use_gpu: Optional[bool]
-        anisotropy: Optional[float]
-        diameter_level0: Optional[float]
-        cellprob_threshold: Optional[float]
-        flow_threshold: Optional[float]
-        model_type: Optional[str]
-        pretrained_model: Optional[str]
-        min_size: Optional[int]
-        augment: Optional[bool]
-        net_avg: Optional[bool]
-        use_masks: Optional[bool]
+    from fractal_tasks_core.tasks._utils import run_fractal_task
 
     run_fractal_task(
         task_function=cellpose_segmentation,
-        TaskArgsModel=TaskArguments,
         logger_name=logger.name,
     )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/compress_tif.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/compress_tif.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Marco Franzon <marco.franzon@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
+Task to compress tiff images.
 
-Task to compress tiff images (currently obsolete)
+**This task cannot be used in the current form, and it should first be
+aligned with the other tasks' structure.**
 """
 import glob
 import os
 
 from PIL import Image
 
 
-def compress_tif(in_path, out_path, delete_input=False):
+def compress_tif(in_path: str, out_path: str, delete_input: bool = False):
 
     """
-    Compress tiff files
+    Compress tiff files.
 
-    :param in_path: directory containing the input files
-    :type in_path: str
-    :param out_path: directory containing the output files
-    :type out_path: str
-    :param delete_input: delete input files
-    :type delete_input: bool
+    Args:
+        in_path: directory containing the input files.
+        out_path: directory containing the output files.
+        delete_input: delete input files.
     """
 
     # Sanitize input/output paths
     if not in_path.endswith("/"):
         in_path += "/"
     if not out_path.endswith("/"):
         out_path += "/"
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/create_ome_zarr.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,147 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Create structure for OME-NGFF zarr array
+Create structure for OME-NGFF zarr array.
 """
 import os
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
 from typing import Optional
-from typing import Sequence
 
 import pandas as pd
-import zarr
-from anndata.experimental import write_elem
+from pydantic.decorator import validate_arguments
 
 import fractal_tasks_core
-from fractal_tasks_core.lib_channels import check_well_channel_labels
-from fractal_tasks_core.lib_channels import define_omero_channels
-from fractal_tasks_core.lib_channels import validate_allowed_channel_input
-from fractal_tasks_core.lib_glob import glob_with_multiple_patterns
-from fractal_tasks_core.lib_metadata_parsing import parse_yokogawa_metadata
-from fractal_tasks_core.lib_parse_filename_metadata import parse_filename
-from fractal_tasks_core.lib_regions_of_interest import prepare_FOV_ROI_table
-from fractal_tasks_core.lib_regions_of_interest import prepare_well_ROI_table
-from fractal_tasks_core.lib_ROI_overlaps import remove_FOV_overlaps
-
+from fractal_tasks_core.cellvoyager.filenames import (
+    glob_with_multiple_patterns,
+)
+from fractal_tasks_core.cellvoyager.filenames import parse_filename
+from fractal_tasks_core.cellvoyager.metadata import (
+    parse_yokogawa_metadata,
+)
+from fractal_tasks_core.channels import check_unique_wavelength_ids
+from fractal_tasks_core.channels import define_omero_channels
+from fractal_tasks_core.channels import OmeroChannel
+from fractal_tasks_core.ngff.specs import NgffImageMeta
+from fractal_tasks_core.ngff.specs import Plate
+from fractal_tasks_core.ngff.specs import Well
+from fractal_tasks_core.roi import prepare_FOV_ROI_table
+from fractal_tasks_core.roi import prepare_well_ROI_table
+from fractal_tasks_core.roi import remove_FOV_overlaps
+from fractal_tasks_core.tables import write_table
+from fractal_tasks_core.tasks.io_models import InitArgsCellVoyager
+from fractal_tasks_core.zarr_utils import open_zarr_group_with_overwrite
 
 __OME_NGFF_VERSION__ = fractal_tasks_core.__OME_NGFF_VERSION__
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-def create_ome_zarr(
+@validate_arguments
+def cellvoyager_to_ome_zarr_init(
     *,
-    input_paths: Sequence[str],
-    output_path: str,
-    metadata: Dict[str, Any],
-    image_extension: str = "tif",
+    zarr_urls: list[str],
+    zarr_dir: str,
+    image_dirs: list[str],
+    allowed_channels: list[OmeroChannel],
     image_glob_patterns: Optional[list[str]] = None,
-    allowed_channels: Sequence[Dict[str, Any]],
-    num_levels: int = 2,
+    num_levels: int = 5,
     coarsening_xy: int = 2,
-    metadata_table: str = "mrf_mlf",
-) -> Dict[str, Any]:
+    image_extension: str = "tif",
+    metadata_table_file: Optional[str] = None,
+    overwrite: bool = False,
+) -> dict[str, Any]:
     """
-    Create a OME-NGFF zarr folder, without reading/writing image data
+    Create a OME-NGFF zarr folder, without reading/writing image data.
 
-    Find plates (for each folder in input_paths)
-        * glob image files
-        * parse metadata from image filename to identify plates
-        * identify populated channels
-
-    Create a zarr folder (for each plate)
-        * parse mlf metadata
-        * identify wells and field of view (FOV)
-        * create FOV ZARR
-        * verify that channels are uniform (i.e., same channels)
-
-    :param input_paths: TBD (common to all tasks)
-    :param output_path: TBD (common to all tasks)
-    :param metadata: TBD (common to all tasks)
-    :param image_extension: Filename extension of images (e.g. `"tif"` or
-                            `"png"`)
-    :param image_glob_patterns: If specified, only parse images with filenames
-                                that match with all these patterns. Patterns
-                                must be defined as in
-                                https://docs.python.org/3/library/fnmatch.html,
-                                e.g. `image_glob_pattern=["*_B03_*"]`.
-    :param num_levels: Number of resolution-pyramid levels
-    :param coarsening_xy: Linear coarsening factor between subsequent levels
-    :param allowed_channels: A list of channel dictionaries, where each channel
-                             must include the ``wavelength_id`` key and where
-                             the corresponding values should be unique across
-                             channels.
-    :param metadata_table: If equal to ``"mrf_mlf"``, parse Yokogawa metadata
-                           from mrf/mlf files in the input_path folder; else,
-                           the full path to a csv file containing
-                           the parsed metadata table.
+    Find plates (for each folder in input_paths):
+
+    - glob image files,
+    - parse metadata from image filename to identify plates,
+    - identify populated channels.
+
+    Create a zarr folder (for each plate):
+
+    - parse mlf metadata,
+    - identify wells and field of view (FOV),
+    - create FOV ZARR,
+    - verify that channels are uniform (i.e., same channels).
+
+    Args:
+        zarr_urls: List of paths or urls to the individual OME-Zarr image to
+            be processed. Not used by the converter task.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        zarr_dir: path of the directory where the new OME-Zarrs will be
+            created.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        image_dirs: list of paths to the folders that contains the Cellvoyager
+            image files. Each entry is a path to a folder that contains the
+            image files themselves for a multiwell plate and the
+            MeasurementData & MeasurementDetail metadata files.
+        allowed_channels: A list of `OmeroChannel` s, where each channel must
+            include the `wavelength_id` attribute and where the
+            `wavelength_id` values must be unique across the list.
+        image_glob_patterns: If specified, only parse images with filenames
+            that match with all these patterns. Patterns must be defined as in
+            https://docs.python.org/3/library/fnmatch.html, Example:
+            `image_glob_pattern=["*_B03_*"]` => only process well B03
+            `image_glob_pattern=["*_C09_*", "*F016*", "*Z[0-5][0-9]C*"]` =>
+            only process well C09, field of view 16 and Z planes 0-59.
+        num_levels: Number of resolution-pyramid levels. If set to `5`, there
+            will be the full-resolution level and 4 levels of
+            downsampled images.
+        coarsening_xy: Linear coarsening factor between subsequent levels.
+            If set to `2`, level 1 is 2x downsampled, level 2 is
+            4x downsampled etc.
+        image_extension: Filename extension of images (e.g. `"tif"` or `"png"`)
+        metadata_table_file: If `None`, parse Yokogawa metadata from mrf/mlf
+            files in the input_path folder; else, the full path to a csv file
+            containing the parsed metadata table.
+        overwrite: If `True`, overwrite the task output.
+
+    Returns:
+        A metadata dictionary containing important metadata about the OME-Zarr
+            plate, the images and some parameters required by downstream tasks
+            (like `num_levels`).
     """
 
-    # Preliminary checks on metadata_table
-    if metadata_table != "mrf_mlf" and not metadata_table.endswith(".csv"):
-        raise ValueError(
-            "metadata_table must be a known string or a "
-            "csv file containing a pandas dataframe"
-        )
-    if metadata_table.endswith(".csv") and not os.path.isfile(metadata_table):
-        raise FileNotFoundError(f"Missing file: {metadata_table=}")
+    # Preliminary checks on metadata_table_file
+    if metadata_table_file:
+        if not metadata_table_file.endswith(".csv"):
+            raise ValueError(f"{metadata_table_file=} is not a csv file")
+        if not os.path.isfile(metadata_table_file):
+            raise FileNotFoundError(f"{metadata_table_file=} does not exist")
 
     # Identify all plates and all channels, across all input folders
     plates = []
     actual_wavelength_ids = None
     dict_plate_paths = {}
-    dict_plate_prefixes: Dict[str, Any] = {}
+    dict_plate_prefixes: dict[str, Any] = {}
 
     # Preliminary checks on allowed_channels argument
-    validate_allowed_channel_input(allowed_channels)
-
-    for in_path_str in input_paths:
-        in_path = Path(in_path_str)
+    check_unique_wavelength_ids(allowed_channels)
 
+    for image_dir in image_dirs:
         # Glob image filenames
         patterns = [f"*.{image_extension}"]
         if image_glob_patterns:
             patterns.extend(image_glob_patterns)
         input_filenames = glob_with_multiple_patterns(
-            folder=in_path_str,
+            folder=image_dir,
             patterns=patterns,
         )
 
         tmp_wavelength_ids = []
         tmp_plates = []
         for fn in input_filenames:
             try:
@@ -140,15 +159,15 @@
                     f'Skipping "{Path(fn).name}". Original error: ' + str(e)
                 )
         tmp_plates = sorted(list(set(tmp_plates)))
         tmp_wavelength_ids = sorted(list(set(tmp_wavelength_ids)))
 
         info = (
             "Listing plates/channels:\n"
-            f"Folder:   {in_path_str}\n"
+            f"Folder:   {image_dir}\n"
             f"Patterns: {patterns}\n"
             f"Plates:   {tmp_plates}\n"
             f"Channels: {tmp_wavelength_ids}\n"
         )
 
         # Check that only one plate is found
         if len(tmp_plates) > 1:
@@ -174,81 +193,85 @@
             plates.append(plate)
 
         # Check that channels are the same as in previous plates
         if actual_wavelength_ids is None:
             actual_wavelength_ids = tmp_wavelength_ids[:]
         else:
             if actual_wavelength_ids != tmp_wavelength_ids:
-                raise Exception(
+                raise ValueError(
                     f"ERROR\n{info}\nERROR:"
                     f" expected channels {actual_wavelength_ids}"
                 )
 
         # Update dict_plate_paths
-        dict_plate_paths[plate] = in_path
+        dict_plate_paths[plate] = image_dir
 
     # Check that all channels are in the allowed_channels
     allowed_wavelength_ids = [
-        channel["wavelength_id"] for channel in allowed_channels
+        channel.wavelength_id for channel in allowed_channels
     ]
     if not set(actual_wavelength_ids).issubset(set(allowed_wavelength_ids)):
         msg = "ERROR in create_ome_zarr\n"
         msg += f"actual_wavelength_ids: {actual_wavelength_ids}\n"
         msg += f"allowed_wavelength_ids: {allowed_wavelength_ids}\n"
-        raise Exception(msg)
+        raise ValueError(msg)
 
     # Create actual_channels, i.e. a list of the channel dictionaries which are
     # present
     actual_channels = [
         channel
         for channel in allowed_channels
-        if channel["wavelength_id"] in actual_wavelength_ids
+        if channel.wavelength_id in actual_wavelength_ids
     ]
 
-    zarrurls: Dict[str, List[str]] = {"plate": [], "well": [], "image": []}
-
     ################################################################
+    # Create well/image OME-Zarr folders on disk, and prepare output
+    # metadata
+    parallelization_list = []
+
     for plate in plates:
         # Define plate zarr
-        zarrurl = f"{plate}.zarr"
+        relative_zarrurl = f"{plate}.zarr"
         in_path = dict_plate_paths[plate]
-        logger.info(f"Creating {zarrurl}")
-        group_plate = zarr.group(Path(output_path) / zarrurl)
-        zarrurls["plate"].append(zarrurl)
+        logger.info(f"Creating {relative_zarrurl}")
+        # Call zarr.open_group wrapper, which handles overwrite=True/False
+        group_plate = open_zarr_group_with_overwrite(
+            str(Path(zarr_dir) / relative_zarrurl),
+            overwrite=overwrite,
+        )
 
         # Obtain FOV-metadata dataframe
-
-        if metadata_table == "mrf_mlf":
+        if metadata_table_file is None:
             mrf_path = f"{in_path}/MeasurementDetail.mrf"
             mlf_path = f"{in_path}/MeasurementData.mlf"
 
             site_metadata, number_images_mlf = parse_yokogawa_metadata(
                 mrf_path,
                 mlf_path,
                 filename_patterns=image_glob_patterns,
             )
             site_metadata = remove_FOV_overlaps(site_metadata)
 
         # If a metadata table was passed, load it and use it directly
-        elif metadata_table.endswith(".csv"):
+        else:
             logger.warning(
                 "Since a custom metadata table was provided, there will "
                 "be no additional check on the number of image files."
             )
-            site_metadata = pd.read_csv(metadata_table)
+            site_metadata = pd.read_csv(metadata_table_file)
             site_metadata.set_index(["well_id", "FieldIndex"], inplace=True)
 
         # Extract pixel sizes and bit_depth
         pixel_size_z = site_metadata["pixel_size_z"][0]
         pixel_size_y = site_metadata["pixel_size_y"][0]
         pixel_size_x = site_metadata["pixel_size_x"][0]
         bit_depth = site_metadata["bit_depth"][0]
 
         if min(pixel_size_z, pixel_size_y, pixel_size_x) < 1e-9:
-            raise Exception(pixel_size_z, pixel_size_y, pixel_size_x)
+            raise ValueError(pixel_size_z, pixel_size_y, pixel_size_x)
 
         # Identify all wells
         plate_prefix = dict_plate_prefixes[plate]
 
         patterns = [f"{plate_prefix}_*.{image_extension}"]
         if image_glob_patterns:
             patterns.extend(image_glob_patterns)
@@ -267,15 +290,15 @@
             if image_glob_patterns:
                 patterns.extend(image_glob_patterns)
             well_images = glob_with_multiple_patterns(
                 folder=str(in_path), patterns=patterns
             )
 
             # Check number of images matches with expected one
-            if metadata_table == "mrf_mlf":
+            if metadata_table_file is None:
                 num_images_glob = len(well_images)
                 num_images_expected = number_images_mlf[well]
                 if num_images_glob != num_images_expected:
                     raise ValueError(
                         f"Wrong number of images for {well=}\n"
                         f"Expected {num_images_expected} (from mlf file)\n"
                         f"Found {num_images_glob} files\n"
@@ -291,15 +314,15 @@
                     well_wavelength_ids.append(
                         f"A{filename_metadata['A']}_C{filename_metadata['C']}"
                     )
                 except IndexError:
                     logger.info(f"Skipping {fpath}")
             well_wavelength_ids = sorted(list(set(well_wavelength_ids)))
             if well_wavelength_ids != actual_wavelength_ids:
-                raise Exception(
+                raise ValueError(
                     f"ERROR: well {well} in plate {plate} (prefix: "
                     f"{plate_prefix}) has missing channels.\n"
                     f"Expected: {actual_channels}\n"
                     f"Found: {well_wavelength_ids}.\n"
                 )
 
         well_rows_columns = [
@@ -310,41 +333,59 @@
         ]
         col_list = [
             well_row_column[1] for well_row_column in well_rows_columns
         ]
         row_list = sorted(list(set(row_list)))
         col_list = sorted(list(set(col_list)))
 
-        group_plate.attrs["plate"] = {
+        plate_attrs = {
             "acquisitions": [{"id": 0, "name": plate}],
             "columns": [{"name": col} for col in col_list],
             "rows": [{"name": row} for row in row_list],
+            "version": __OME_NGFF_VERSION__,
             "wells": [
                 {
                     "path": well_row_column[0] + "/" + well_row_column[1],
                     "rowIndex": row_list.index(well_row_column[0]),
                     "columnIndex": col_list.index(well_row_column[1]),
                 }
                 for well_row_column in well_rows_columns
             ],
         }
 
-        for row, column in well_rows_columns:
+        # Validate plate attrs:
+        Plate(**plate_attrs)
 
+        group_plate.attrs["plate"] = plate_attrs
+
+        for row, column in well_rows_columns:
+            parallelization_list.append(
+                {
+                    "zarr_url": f"{zarr_dir}/{plate}.zarr/{row}/{column}/0/",
+                    "init_args": InitArgsCellVoyager(
+                        image_dir=in_path,
+                        plate_prefix=plate_prefix,
+                        well_ID=f"{row}{column}",
+                        image_extension=image_extension,
+                        image_glob_patterns=image_glob_patterns,
+                    ).dict(),
+                }
+            )
             group_well = group_plate.create_group(f"{row}/{column}/")
 
-            group_well.attrs["well"] = {
+            well_attrs = {
                 "images": [{"path": "0"}],
                 "version": __OME_NGFF_VERSION__,
             }
 
-            group_image = group_well.create_group("0/")  # noqa: F841
-            zarrurls["well"].append(f"{plate}.zarr/{row}/{column}/")
-            zarrurls["image"].append(f"{plate}.zarr/{row}/{column}/0/")
+            # Validate well attrs:
+            Well(**well_attrs)
+            group_well.attrs["well"] = well_attrs
 
+            group_image = group_well.create_group("0/")  # noqa: F841
             group_image.attrs["multiscales"] = [
                 {
                     "version": __OME_NGFF_VERSION__,
                     "axes": [
                         {"name": "c", "type": "channel"},
                         {
                             "name": "z",
@@ -365,14 +406,15 @@
                     "datasets": [
                         {
                             "path": f"{ind_level}",
                             "coordinateTransformations": [
                                 {
                                     "type": "scale",
                                     "scale": [
+                                        1,
                                         pixel_size_z,
                                         pixel_size_y
                                         * coarsening_xy**ind_level,
                                         pixel_size_x
                                         * coarsening_xy**ind_level,
                                     ],
                                 }
@@ -380,73 +422,51 @@
                         }
                         for ind_level in range(num_levels)
                     ],
                 }
             ]
 
             group_image.attrs["omero"] = {
-                "id": 1,  # FIXME does this depend on the plate number?
+                "id": 1,  # TODO does this depend on the plate number?
                 "name": "TBD",
                 "version": __OME_NGFF_VERSION__,
                 "channels": define_omero_channels(
                     channels=actual_channels, bit_depth=bit_depth
                 ),
             }
 
-            # Create tables zarr group for ROI tables
-            group_tables = group_image.create_group("tables/")  # noqa: F841
-            well_id = row + column
+            # Validate Image attrs
+            NgffImageMeta(**group_image.attrs)
 
             # Prepare AnnData tables for FOV/well ROIs
+            well_id = row + column
             FOV_ROIs_table = prepare_FOV_ROI_table(site_metadata.loc[well_id])
             well_ROIs_table = prepare_well_ROI_table(
                 site_metadata.loc[well_id]
             )
 
-            # Write AnnData tables in the tables zarr group
-            write_elem(group_tables, "FOV_ROI_table", FOV_ROIs_table)
-            write_elem(group_tables, "well_ROI_table", well_ROIs_table)
-            group_tables.attrs["tables"] = ["FOV_ROI_table", "well_ROI_table"]
-
-    # Check that the different images in each well have unique channel labels.
-    # Since we currently merge all fields of view in the same image, this check
-    # is useless. It should remain there to catch an error in case we switch
-    # back to one-image-per-field-of-view mode
-    for well_path in zarrurls["well"]:
-        check_well_channel_labels(
-            well_zarr_path=str(Path(output_path) / well_path)
-        )
+            # Write AnnData tables into the `tables` zarr group
+            write_table(
+                group_image,
+                "FOV_ROI_table",
+                FOV_ROIs_table,
+                overwrite=overwrite,
+                table_attrs={"type": "roi_table"},
+            )
+            write_table(
+                group_image,
+                "well_ROI_table",
+                well_ROIs_table,
+                overwrite=overwrite,
+                table_attrs={"type": "roi_table"},
+            )
 
-    metadata_update = dict(
-        plate=zarrurls["plate"],
-        well=zarrurls["well"],
-        image=zarrurls["image"],
-        num_levels=num_levels,
-        coarsening_xy=coarsening_xy,
-        image_extension=image_extension,
-        image_glob_patterns=image_glob_patterns,
-        original_paths=input_paths[:],
-    )
-    return metadata_update
+    return dict(parallelization_list=parallelization_list)
 
 
 if __name__ == "__main__":
-    from pydantic import BaseModel
-    from pydantic import Extra
-    from fractal_tasks_core._utils import run_fractal_task
-
-    class TaskArguments(BaseModel, extra=Extra.forbid):
-        input_paths: Sequence[str]
-        output_path: str
-        metadata: Dict[str, Any]
-        image_extension: str
-        image_glob_patterns: Optional[list[str]]
-        allowed_channels: Sequence[Dict[str, Any]]
-        num_levels: Optional[int]
-        coarsening_xy: Optional[int]
-        metadata_table: Optional[str]
+    from fractal_tasks_core.tasks._utils import run_fractal_task
 
     run_fractal_task(
-        task_function=create_ome_zarr,
-        TaskArgsModel=TaskArguments,
+        task_function=cellvoyager_to_ome_zarr_init,
         logger_name=logger.name,
     )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/create_ome_zarr_multiplex.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/cellvoyager_to_ome_zarr_init_multiplex.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,154 +1,163 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Create OME-NGFF zarr group, for multiplexing dataset
+Create OME-NGFF zarr group, for multiplexing dataset.
 """
 import os
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
-from typing import Literal
 from typing import Optional
-from typing import Sequence
-from typing import Union
 
 import pandas as pd
 import zarr
-from anndata.experimental import write_elem
+from pydantic.decorator import validate_arguments
+from zarr.errors import ContainsGroupError
 
 import fractal_tasks_core
-from fractal_tasks_core.lib_channels import check_well_channel_labels
-from fractal_tasks_core.lib_channels import define_omero_channels
-from fractal_tasks_core.lib_channels import validate_allowed_channel_input
-from fractal_tasks_core.lib_glob import glob_with_multiple_patterns
-from fractal_tasks_core.lib_metadata_parsing import parse_yokogawa_metadata
-from fractal_tasks_core.lib_parse_filename_metadata import parse_filename
-from fractal_tasks_core.lib_regions_of_interest import prepare_FOV_ROI_table
-from fractal_tasks_core.lib_regions_of_interest import prepare_well_ROI_table
-from fractal_tasks_core.lib_ROI_overlaps import remove_FOV_overlaps
-
+from fractal_tasks_core.cellvoyager.filenames import (
+    glob_with_multiple_patterns,
+)
+from fractal_tasks_core.cellvoyager.filenames import parse_filename
+from fractal_tasks_core.cellvoyager.metadata import (
+    parse_yokogawa_metadata,
+)
+from fractal_tasks_core.channels import check_unique_wavelength_ids
+from fractal_tasks_core.channels import check_well_channel_labels
+from fractal_tasks_core.channels import define_omero_channels
+from fractal_tasks_core.ngff.specs import NgffImageMeta
+from fractal_tasks_core.ngff.specs import Plate
+from fractal_tasks_core.ngff.specs import Well
+from fractal_tasks_core.roi import prepare_FOV_ROI_table
+from fractal_tasks_core.roi import prepare_well_ROI_table
+from fractal_tasks_core.roi import remove_FOV_overlaps
+from fractal_tasks_core.tables import write_table
+from fractal_tasks_core.tasks.io_models import InitArgsCellVoyager
+from fractal_tasks_core.tasks.io_models import MultiplexingAcquisition
+from fractal_tasks_core.zarr_utils import open_zarr_group_with_overwrite
 
 __OME_NGFF_VERSION__ = fractal_tasks_core.__OME_NGFF_VERSION__
 
 import logging
 
 logger = logging.getLogger(__name__)
 
 
-def create_ome_zarr_multiplex(
+@validate_arguments
+def cellvoyager_to_ome_zarr_init_multiplex(
     *,
-    input_paths: Sequence[str],
-    output_path: str,
-    metadata: Dict[str, Any],
-    image_extension: str = "tif",
+    zarr_urls: list[str],
+    zarr_dir: str,
+    acquisitions: dict[str, MultiplexingAcquisition],
     image_glob_patterns: Optional[list[str]] = None,
-    allowed_channels: Dict[str, Sequence[Dict[str, Any]]],
-    num_levels: int = 2,
+    num_levels: int = 5,
     coarsening_xy: int = 2,
-    metadata_table: Union[Literal["mrf_mlf"], Dict[str, str]] = "mrf_mlf",
-) -> Dict[str, Any]:
+    image_extension: str = "tif",
+    metadata_table_files: Optional[dict[str, str]] = None,
+    overwrite: bool = False,
+) -> dict[str, Any]:
     """
-    Create OME-NGFF structure and metadata to host a multiplexing dataset
+    Create OME-NGFF structure and metadata to host a multiplexing dataset.
 
     This task takes a set of image folders (i.e. different acquisition cycles)
     and build the internal structure and metadata of a OME-NGFF zarr group,
     without actually loading/writing the image data.
 
-    Each input_paths should be treated as a different acquisition
+    Each element in input_paths should be treated as a different acquisition.
 
-    :param input_paths: list of image folders for different acquisition
-                        cycles, e.g. in the form `["/path/cycle1/",
-                        "/path/cycle2/"]`
-    :param output_path: parent folder for the output path, e.g.
-                        `"/outputpath/"`
-    :param metadata: standard fractal argument, not used in this task
-    :param image_extension: Filename extension of images (e.g. `tif` or `png`)
-    :param image_glob_patterns: If specified, only parse images with filenames
-                            that match with all these patterns. Patterns
-                            must be defined as in
-                            https://docs.python.org/3/library/fnmatch.html,
-                            e.g. `image_glob_pattern=["*_B03_*"]`.
-    :param allowed_channels: TBD
-    :param num_levels: number of resolution-pyramid levels
-    :param coarsening_xy: Linear coarsening factor between subsequent levels
-    :param metadata_table: If equal to ``"mrf_mlf"``, parse Yokogawa metadata
-                           from mrf/mlf files in the ``input_paths`` folders;
-                           else, a dictionary of key-value pairs like
-                           ``(acquisition, path)`` with ``acquisition`` a
-                           string and ``path`` pointing to a csv file
-                           containing the parsed metadata table.
+    Args:
+        zarr_urls: List of paths or urls to the individual OME-Zarr image to
+            be processed. Not used by the converter task.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        zarr_dir: path of the directory where the new OME-Zarrs will be
+            created.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        acquisitions: dictionary of acquisitions. Each key is the acquisition
+            identifier (normally 0, 1, 2, 3 etc.). Each item defines the
+            acquisition by providing the image_dir and the allowed_channels.
+        image_glob_patterns: If specified, only parse images with filenames
+            that match with all these patterns. Patterns must be defined as in
+            https://docs.python.org/3/library/fnmatch.html, Example:
+            `image_glob_pattern=["*_B03_*"]` => only process well B03
+            `image_glob_pattern=["*_C09_*", "*F016*", "*Z[0-5][0-9]C*"]` =>
+            only process well C09, field of view 16 and Z planes 0-59.
+        num_levels: Number of resolution-pyramid levels. If set to `5`, there
+            will be the full-resolution level and 4 levels of downsampled
+            images.
+        coarsening_xy: Linear coarsening factor between subsequent levels.
+            If set to `2`, level 1 is 2x downsampled, level 2 is 4x downsampled
+            etc.
+        image_extension: Filename extension of images
+            (e.g. `"tif"` or `"png"`).
+        metadata_table_files: If `None`, parse Yokogawa metadata from mrf/mlf
+            files in the input_path folder; else, a dictionary of key-value
+            pairs like `(acquisition, path)` with `acquisition` a string like
+            the key of the `acquisitions` dict and `path` pointing to a csv
+            file containing the parsed metadata table.
+        overwrite: If `True`, overwrite the task output.
+
+    Returns:
+        A metadata dictionary containing important metadata about the OME-Zarr
+            plate, the images and some parameters required by downstream tasks
+            (like `num_levels`).
     """
 
-    # Preliminary checks on metadata_table
-    if metadata_table != "mrf_mlf" and not isinstance(metadata_table, Dict):
-        raise ValueError(
-            "ERROR: metadata_table must be a known string or a "
-            "dict of csv file containing a pandas dataframe."
-            f"The metadata_table provided was {metadata_table}"
-        )
-    elif isinstance(metadata_table, Dict):
-        # Check that acquisition keys are string
-        for key, value in metadata_table.items():
-            if not isinstance(key, str):
-                raise ValueError(f"{metadata_table=} has non-string keys")
+    if metadata_table_files:
 
         # Checks on the dict:
-        # 1. Acquisitions as keys (same as keys of allowed_channels)
+        # 1. Acquisitions in acquisitions dict and metadata_table_files match
         # 2. Files end with ".csv"
         # 3. Files exist.
-        if set(allowed_channels.keys()) != set(metadata_table.keys()):
+        if set(acquisitions.keys()) != set(metadata_table_files.keys()):
             raise ValueError(
                 "Mismatch in acquisition keys between "
-                f"{allowed_channels.keys()=} and {metadata_table.keys()=}"
-            )
-        if not all([x.endswith(".csv") for x in metadata_table.values()]):
-            raise ValueError(
-                f"Some files in {metadata_table=} do not end with csv."
+                f"{acquisitions.keys()=} and "
+                f"{metadata_table_files.keys()=}"
             )
-        if not all([os.path.isfile(x) for x in metadata_table.values()]):
-            raise ValueError(f"Some files in {metadata_table=} do not exist.")
+        for f in metadata_table_files.values():
+            if not f.endswith(".csv"):
+                raise ValueError(
+                    f"{f} (in metadata_table_file) is not a csv file."
+                )
+            if not os.path.isfile(f):
+                raise ValueError(
+                    f"{f} (in metadata_table_file) does not exist."
+                )
 
-    # Preliminary checks on allowed_channels
+    # Preliminary checks on acquisitions
     # Note that in metadata the keys of dictionary arguments should be
     # strings (and not integers), so that they can be read from a JSON file
-    for key, value in allowed_channels.items():
+    for key, values in acquisitions.items():
         if not isinstance(key, str):
-            raise ValueError(f"{allowed_channels=} has non-string keys")
-        validate_allowed_channel_input(value)
+            raise ValueError(f"{acquisitions=} has non-string keys")
+        check_unique_wavelength_ids(values.allowed_channels)
 
     # Identify all plates and all channels, per input folders
-    dict_acquisitions: Dict = {}
-
-    for ind_in_path, in_path_str in enumerate(input_paths):
-        acquisition = str(ind_in_path)
-        in_path = Path(in_path_str)
+    dict_acquisitions: dict = {}
+    for acquisition, acq_input in acquisitions.items():
         dict_acquisitions[acquisition] = {}
 
         actual_wavelength_ids = []
         plates = []
         plate_prefixes = []
 
         # Loop over all images
         patterns = [f"*.{image_extension}"]
         if image_glob_patterns:
             patterns.extend(image_glob_patterns)
         input_filenames = glob_with_multiple_patterns(
-            folder=in_path_str,
+            folder=acq_input.image_dir,
             patterns=patterns,
         )
         for fn in input_filenames:
             try:
                 filename_metadata = parse_filename(Path(fn).name)
                 plate = filename_metadata["plate"]
                 plates.append(plate)
@@ -185,99 +194,104 @@
             logger.warning(
                 f"For {acquisition=}, we replace {original_plate=} with "
                 f"{plate=} (the one for acquisition 0)"
             )
 
         # Check that all channels are in the allowed_channels
         allowed_wavelength_ids = [
-            c["wavelength_id"] for c in allowed_channels[acquisition]
+            c.wavelength_id for c in acq_input.allowed_channels
         ]
         if not set(actual_wavelength_ids).issubset(
             set(allowed_wavelength_ids)
         ):
             msg = "ERROR in create_ome_zarr\n"
             msg += f"actual_wavelength_ids: {actual_wavelength_ids}\n"
             msg += f"allowed_wavelength_ids: {allowed_wavelength_ids}\n"
             raise ValueError(msg)
 
         # Create actual_channels, i.e. a list of the channel dictionaries which
         # are present
         actual_channels = [
             channel
-            for channel in allowed_channels[acquisition]
-            if channel["wavelength_id"] in actual_wavelength_ids
+            for channel in acq_input.allowed_channels
+            if channel.wavelength_id in actual_wavelength_ids
         ]
 
         logger.info(f"plate: {plate}")
         logger.info(f"actual_channels: {actual_channels}")
 
         dict_acquisitions[acquisition] = {}
         dict_acquisitions[acquisition]["plate"] = plate
         dict_acquisitions[acquisition]["original_plate"] = original_plate
         dict_acquisitions[acquisition]["plate_prefix"] = plate_prefix
-        dict_acquisitions[acquisition]["image_folder"] = in_path
-        dict_acquisitions[acquisition]["original_paths"] = [in_path]
+        dict_acquisitions[acquisition]["image_folder"] = acq_input.image_dir
+        dict_acquisitions[acquisition]["original_paths"] = [
+            acq_input.image_dir
+        ]
         dict_acquisitions[acquisition]["actual_channels"] = actual_channels
         dict_acquisitions[acquisition][
             "actual_wavelength_ids"
         ] = actual_wavelength_ids
 
-    acquisitions = sorted(list(dict_acquisitions.keys()))
+    parallelization_list = []
+    acquisitions_sorted = sorted(list(acquisitions.keys()))
     current_plates = [item["plate"] for item in dict_acquisitions.values()]
     if len(set(current_plates)) > 1:
         raise ValueError(f"{current_plates=}")
     plate = current_plates[0]
 
-    zarrurl = dict_acquisitions[acquisitions[0]]["plate"] + ".zarr"
-    full_zarrurl = str(Path(output_path) / zarrurl)
+    zarrurl = dict_acquisitions[acquisitions_sorted[0]]["plate"] + ".zarr"
+    full_zarrurl = str(Path(zarr_dir) / zarrurl)
     logger.info(f"Creating {full_zarrurl=}")
-    group_plate = zarr.group(full_zarrurl)
+    # Call zarr.open_group wrapper, which handles overwrite=True/False
+    group_plate = open_zarr_group_with_overwrite(
+        full_zarrurl, overwrite=overwrite
+    )
     group_plate.attrs["plate"] = {
         "acquisitions": [
             {
                 "id": int(acquisition),
                 "name": dict_acquisitions[acquisition]["original_plate"],
             }
-            for acquisition in acquisitions
+            for acquisition in acquisitions_sorted
         ]
     }
 
-    zarrurls: Dict[str, List[str]] = {"well": [], "image": []}
-    zarrurls["plate"] = [plate]
+    zarrurls: dict[str, list[str]] = {"well": [], "image": []}
+    zarrurls["plate"] = [f"{plate}.zarr"]
 
     ################################################################
-    logging.info(f"{acquisitions=}")
+    logging.info(f"{acquisitions_sorted=}")
 
-    for acquisition in acquisitions:
+    for acquisition in acquisitions_sorted:
 
         # Define plate zarr
         image_folder = dict_acquisitions[acquisition]["image_folder"]
         logger.info(f"Looking at {image_folder=}")
 
         # Obtain FOV-metadata dataframe
-        if metadata_table == "mrf_mlf":
+        if metadata_table_files is None:
             mrf_path = f"{image_folder}/MeasurementDetail.mrf"
             mlf_path = f"{image_folder}/MeasurementData.mlf"
             site_metadata, total_files = parse_yokogawa_metadata(
                 mrf_path, mlf_path, filename_patterns=image_glob_patterns
             )
             site_metadata = remove_FOV_overlaps(site_metadata)
-
-        elif isinstance(metadata_table, Dict):
-            site_metadata = pd.read_csv(metadata_table[acquisition])
+        else:
+            site_metadata = pd.read_csv(metadata_table_files[acquisition])
             site_metadata.set_index(["well_id", "FieldIndex"], inplace=True)
 
         # Extract pixel sizes and bit_depth
         pixel_size_z = site_metadata["pixel_size_z"][0]
         pixel_size_y = site_metadata["pixel_size_y"][0]
         pixel_size_x = site_metadata["pixel_size_x"][0]
         bit_depth = site_metadata["bit_depth"][0]
 
         if min(pixel_size_z, pixel_size_y, pixel_size_x) < 1e-9:
-            raise Exception(pixel_size_z, pixel_size_y, pixel_size_x)
+            raise ValueError(pixel_size_z, pixel_size_y, pixel_size_x)
 
         # Identify all wells
         plate_prefix = dict_acquisitions[acquisition]["plate_prefix"]
         patterns = [f"{plate_prefix}_*.{image_extension}"]
         if image_glob_patterns:
             patterns.extend(image_glob_patterns)
         plate_images = glob_with_multiple_patterns(
@@ -312,15 +326,15 @@
                 except IndexError:
                     logger.info(f"Skipping {fpath}")
             well_wavelength_ids = sorted(list(set(well_wavelength_ids)))
             actual_wavelength_ids = dict_acquisitions[acquisition][
                 "actual_wavelength_ids"
             ]
             if well_wavelength_ids != actual_wavelength_ids:
-                raise Exception(
+                raise ValueError(
                     f"ERROR: well {well} in plate {plate} (prefix: "
                     f"{plate_prefix}) has missing channels.\n"
                     f"Expected: {actual_wavelength_ids}\n"
                     f"Found: {well_wavelength_ids}.\n"
                 )
 
         well_rows_columns = [
@@ -342,47 +356,69 @@
             {
                 "path": well_row_column[0] + "/" + well_row_column[1],
                 "rowIndex": row_list.index(well_row_column[0]),
                 "columnIndex": col_list.index(well_row_column[1]),
             }
             for well_row_column in well_rows_columns
         ]
+        plate_attrs["version"] = __OME_NGFF_VERSION__
+        # Validate plate attrs
+        Plate(**plate_attrs)
         group_plate.attrs["plate"] = plate_attrs
 
         for row, column in well_rows_columns:
-
-            from zarr.errors import ContainsGroupError
-
+            parallelization_list.append(
+                {
+                    "zarr_url": (
+                        f"{zarr_dir}/{plate}.zarr/{row}/{column}/"
+                        f"{acquisition}/"
+                    ),
+                    "init_args": InitArgsCellVoyager(
+                        image_dir=acquisitions[acquisition].image_dir,
+                        plate_prefix=plate_prefix,
+                        well_ID=f"{row}{column}",
+                        image_extension=image_extension,
+                        image_glob_patterns=image_glob_patterns,
+                        acquisition=acquisition,
+                    ).dict(),
+                }
+            )
             try:
                 group_well = group_plate.create_group(f"{row}/{column}/")
                 logging.info(f"Created new group_well at {row}/{column}/")
-                group_well.attrs["well"] = {
+                well_attrs = {
                     "images": [
                         {
                             "path": f"{acquisition}",
                             "acquisition": int(acquisition),
                         }
                     ],
                     "version": __OME_NGFF_VERSION__,
                 }
+                # Validate well attrs:
+                Well(**well_attrs)
+                group_well.attrs["well"] = well_attrs
                 zarrurls["well"].append(f"{plate}.zarr/{row}/{column}")
             except ContainsGroupError:
                 group_well = zarr.open_group(
                     f"{full_zarrurl}/{row}/{column}/", mode="r+"
                 )
                 logging.info(
                     f"Loaded group_well from {full_zarrurl}/{row}/{column}"
                 )
                 current_images = group_well.attrs["well"]["images"] + [
                     {"path": f"{acquisition}", "acquisition": int(acquisition)}
                 ]
-                group_well.attrs["well"] = dict(
+                well_attrs = dict(
                     images=current_images,
                     version=group_well.attrs["well"]["version"],
                 )
+                # Validate well attrs:
+                Well(**well_attrs)
+                group_well.attrs["well"] = well_attrs
 
             group_image = group_well.create_group(
                 f"{acquisition}/"
             )  # noqa: F841
             logging.info(f"Created image group {row}/{column}/{acquisition}")
             image = f"{plate}.zarr/{row}/{column}/{acquisition}"
             zarrurls["image"].append(image)
@@ -411,14 +447,15 @@
                     "datasets": [
                         {
                             "path": f"{ind_level}",
                             "coordinateTransformations": [
                                 {
                                     "type": "scale",
                                     "scale": [
+                                        1,
                                         pixel_size_z,
                                         pixel_size_y
                                         * coarsening_xy**ind_level,
                                         pixel_size_x
                                         * coarsening_xy**ind_level,
                                     ],
                                 }
@@ -435,69 +472,50 @@
                 "version": __OME_NGFF_VERSION__,
                 "channels": define_omero_channels(
                     channels=actual_channels,
                     bit_depth=bit_depth,
                     label_prefix=acquisition,
                 ),
             }
-
-            # Create tables zarr group for ROI tables
-            group_tables = group_image.create_group("tables/")  # noqa: F841
-            well_id = row + column
+            # Validate Image attrs
+            NgffImageMeta(**group_image.attrs)
 
             # Prepare AnnData tables for FOV/well ROIs
+            well_id = row + column
             FOV_ROIs_table = prepare_FOV_ROI_table(site_metadata.loc[well_id])
             well_ROIs_table = prepare_well_ROI_table(
                 site_metadata.loc[well_id]
             )
 
-            # Write AnnData tables in the tables zarr group
-            write_elem(group_tables, "FOV_ROI_table", FOV_ROIs_table)
-            write_elem(group_tables, "well_ROI_table", well_ROIs_table)
-            group_tables.attrs["tables"] = ["FOV_ROI_table", "well_ROI_table"]
+            # Write AnnData tables into the `tables` zarr group
+            write_table(
+                group_image,
+                "FOV_ROI_table",
+                FOV_ROIs_table,
+                overwrite=overwrite,
+                table_attrs={"type": "roi_table"},
+            )
+            write_table(
+                group_image,
+                "well_ROI_table",
+                well_ROIs_table,
+                overwrite=overwrite,
+                table_attrs={"type": "roi_table"},
+            )
 
     # Check that the different images (e.g. different cycles) in the each well
     # have unique labels
     for well_path in zarrurls["well"]:
         check_well_channel_labels(
-            well_zarr_path=str(Path(output_path) / well_path)
+            well_zarr_path=str(Path(zarr_dir) / well_path)
         )
 
-    original_paths = {
-        acquisition: dict_acquisitions[acquisition]["original_paths"]
-        for acquisition in acquisitions
-    }
-
-    metadata_update = dict(
-        plate=zarrurls["plate"],
-        well=zarrurls["well"],
-        image=zarrurls["image"],
-        num_levels=num_levels,
-        coarsening_xy=coarsening_xy,
-        original_paths=original_paths,
-        image_extension=image_extension,
-        image_glob_patterns=image_glob_patterns,
-    )
-    return metadata_update
+    return dict(parallelization_list=parallelization_list)
 
 
 if __name__ == "__main__":
-    from pydantic import BaseModel
-    from pydantic import Extra
-    from fractal_tasks_core._utils import run_fractal_task
-
-    class TaskArguments(BaseModel, extra=Extra.forbid):
-        input_paths: Sequence[str]
-        output_path: str
-        metadata: Dict[str, Any]
-        image_extension: str
-        image_glob_pattern: Optional[list[str]]
-        allowed_channels: Dict[str, Sequence[Dict[str, Any]]]
-        num_levels: Optional[int]
-        coarsening_xy: Optional[int]
-        metadata_table: Optional[Union[Literal["mrf_mlf"], Dict[str, str]]]
+    from fractal_tasks_core.tasks._utils import run_fractal_task
 
     run_fractal_task(
-        task_function=create_ome_zarr_multiplex,
-        TaskArgsModel=TaskArguments,
+        task_function=cellvoyager_to_ome_zarr_init_multiplex,
         logger_name=logger.name,
     )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/illumination_correction.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/illumination_correction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,67 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Marco Franzon <marco.franzon@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Apply illumination correction to all fields of view
+Apply illumination correction to all fields of view.
 """
 import logging
 import time
 import warnings
 from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import Optional
-from typing import Sequence
 
 import anndata as ad
 import dask.array as da
 import numpy as np
 import zarr
+from pydantic.decorator import validate_arguments
 from skimage.io import imread
 
-from fractal_tasks_core.lib_channels import get_omero_channel_list
-from fractal_tasks_core.lib_pyramid_creation import build_pyramid
-from fractal_tasks_core.lib_regions_of_interest import (
+from fractal_tasks_core.channels import get_omero_channel_list
+from fractal_tasks_core.channels import OmeroChannel
+from fractal_tasks_core.ngff import load_NgffImageMeta
+from fractal_tasks_core.pyramids import build_pyramid
+from fractal_tasks_core.roi import check_valid_ROI_indices
+from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
-from fractal_tasks_core.lib_zattrs_utils import extract_zyx_pixel_sizes
 
 logger = logging.getLogger(__name__)
 
 
 def correct(
     img_stack: np.ndarray,
     corr_img: np.ndarray,
     background: int = 110,
 ):
     """
     Corrects a stack of images, using a given illumination profile (e.g. bright
     in the center of the image, dim outside).
 
-    img_stack is a four-dimensional (czyx) numpy array, with dummy size along c
-
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Args:
+        img_stack: 4D numpy array (czyx), with dummy size along c.
+        corr_img: 2D numpy array (yx)
+        background: Background value that is subtracted from the image before
+            the illumination correction is applied.
     """
 
     logger.info(f"Start correct, {img_stack.shape}")
 
     # Check shapes
     if corr_img.shape != img_stack.shape[2:] or img_stack.shape[0] != 1:
-        raise Exception(
+        raise ValueError(
             "Error in illumination_correction:\n"
             f"{img_stack.shape=}\n{corr_img.shape=}"
         )
 
     # Store info about dtype
     dtype = img_stack.dtype
     dtype_max = np.iinfo(dtype).max
@@ -87,144 +86,145 @@
 
     logger.info("End correct")
 
     # Cast back to original dtype and return
     return new_img_stack.astype(dtype)
 
 
+@validate_arguments
 def illumination_correction(
     *,
-    input_paths: Sequence[str],
-    output_path: str,
-    component: str,
-    metadata: Dict[str, Any],
-    overwrite: bool = False,
-    new_component: Optional[str] = None,
-    dict_corr: dict,
-    background: int = 100,
-) -> Dict[str, Any]:
+    # Fractal argument
+    zarr_url: str,
+    # Task-specific arguments
+    illumination_profiles_folder: str,
+    dict_corr: dict[str, str],
+    background: int = 110,
+    input_ROI_table: str = "FOV_ROI_table",
+    overwrite_input: bool = True,
+    suffix: str = "_illum_corr",
+) -> dict[str, Any]:
 
     """
-    FIXME docstring
-
-    Example inputs:
-    input_paths: ["/some/path"]
-    output_path: "/same/or/other/path/"
-    component: myplate.zarr/B/03/0/
-    new_component: myplate_new_name.zarr/B/03/0/
-    metadata: {...}
+    Applies illumination correction to the images in the OME-Zarr.
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Assumes that the illumination correction profiles were generated before
+    separately and that the same background subtraction was used during
+    calculation of the illumination correction (otherwise, it will not work
+    well & the correction may only be partial).
+
+    Args:
+        zarr_url: Path or url to the individual OME-Zarr image to be processed.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        illumination_profiles_folder: Path of folder of illumination profiles.
+        dict_corr: Dictionary where keys match the `wavelength_id` attributes
+            of existing channels (e.g.  `A01_C01` ) and values are the
+            filenames of the corresponding illumination profiles.
+        background: Background value that is subtracted from the image before
+            the illumination correction is applied. Set it to `0` if you don't
+            want any background subtraction.
+        input_ROI_table: Name of the ROI table that contains the information
+            about the location of the individual field of views (FOVs) to
+            which the illumination correction shall be applied. Defaults to
+            "FOV_ROI_table", the default name Fractal converters give the ROI
+            tables that list all FOVs separately. If you generated your
+            OME-Zarr with a different converter and used Import OME-Zarr to
+            generate the ROI tables, `image_ROI_table` is the right choice if
+            you only have 1 FOV per Zarr image and `grid_ROI_table` if you
+            have multiple FOVs per Zarr image and set the right grid options
+            during import.
+        overwrite_input: If `True`, the results of this task will overwrite
+            the input image data. If false, a new image is generated and the
+            illumination corrected data is saved there.
+        suffix: What suffix to append to the illumination corrected images.
+            Only relevant if `overwrite_input=False`.
     """
 
-    # Preliminary checks
-    if len(input_paths) > 1:
-        raise NotImplementedError
-    if (overwrite and new_component is not None) or (
-        new_component is None and not overwrite
-    ):
-        raise Exception(f"{overwrite=}, but {new_component=}")
-
-    if not overwrite:
-        msg = (
-            "We still have to harmonize illumination_correction("
-            "overwrite=False) with replicate_zarr_structure(..., "
-            "suffix=..)"
-        )
-        raise NotImplementedError(msg)
-
-    # Read some parameters from metadata
-    num_levels = metadata["num_levels"]
-    coarsening_xy = metadata["coarsening_xy"]
-
     # Defione old/new zarrurls
-    plate, well = component.split(".zarr/")
-    in_path = Path(input_paths[0])
-    zarrurl_old = (in_path / component).as_posix()
-    if overwrite:
-        zarrurl_new = zarrurl_old
+    if overwrite_input:
+        zarr_url_new = zarr_url
     else:
-        new_plate, new_well = new_component.split(".zarr/")
-        if new_well != well:
-            raise Exception(f"{well=}, {new_well=}")
-        zarrurl_new = (Path(output_path) / new_component).as_posix()
+        zarr_url_new = zarr_url + suffix
 
     t_start = time.perf_counter()
     logger.info("Start illumination_correction")
-    logger.info(f"  {overwrite=}")
-    logger.info(f"  {zarrurl_old=}")
-    logger.info(f"  {zarrurl_new=}")
+    logger.info(f"  {overwrite_input=}")
+    logger.info(f"  {zarr_url=}")
+    logger.info(f"  {zarr_url_new=}")
+
+    # Read attributes from NGFF metadata
+    ngff_image_meta = load_NgffImageMeta(zarr_url)
+    num_levels = ngff_image_meta.num_levels
+    coarsening_xy = ngff_image_meta.coarsening_xy
+    full_res_pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=0)
+    logger.info(f"NGFF image has {num_levels=}")
+    logger.info(f"NGFF image has {coarsening_xy=}")
+    logger.info(
+        f"NGFF image has full-res pixel sizes {full_res_pxl_sizes_zyx}"
+    )
 
     # Read channels from .zattrs
-    channels = get_omero_channel_list(image_zarr_path=zarrurl_old)
+    channels: list[OmeroChannel] = get_omero_channel_list(
+        image_zarr_path=zarr_url
+    )
     num_channels = len(channels)
 
     # Read FOV ROIs
-    FOV_ROI_table = ad.read_zarr(f"{zarrurl_old}/tables/FOV_ROI_table")
-
-    # Read pixel sizes from zattrs file
-    full_res_pxl_sizes_zyx = extract_zyx_pixel_sizes(
-        f"{zarrurl_old}/.zattrs", level=0
-    )
+    FOV_ROI_table = ad.read_zarr(f"{zarr_url}/tables/{input_ROI_table}")
 
     # Create list of indices for 3D FOVs spanning the entire Z direction
     list_indices = convert_ROI_table_to_indices(
         FOV_ROI_table,
         level=0,
         coarsening_xy=coarsening_xy,
         full_res_pxl_sizes_zyx=full_res_pxl_sizes_zyx,
     )
+    check_valid_ROI_indices(list_indices, input_ROI_table)
 
     # Extract image size from FOV-ROI indices. Note: this works at level=0,
     # where FOVs should all be of the exact same size (in pixels)
     ref_img_size = None
     for indices in list_indices:
         img_size = (indices[3] - indices[2], indices[5] - indices[4])
         if ref_img_size is None:
             ref_img_size = img_size
         else:
             if img_size != ref_img_size:
-                raise Exception(
+                raise ValueError(
                     "ERROR: inconsistent image sizes in list_indices"
                 )
     img_size_y, img_size_x = img_size[:]
 
-    # Load paths of correction matrices
-    root_path_corr = dict_corr.pop("root_path_corr")
-    if not root_path_corr.endswith("/"):
-        root_path_corr += "/"
-
     # Assemble dictionary of matrices and check their shapes
     corrections = {}
     for channel in channels:
-        wavelength_id = channel["wavelength_id"]
+        wavelength_id = channel.wavelength_id
         corrections[wavelength_id] = imread(
-            root_path_corr + dict_corr[wavelength_id]
+            (
+                Path(illumination_profiles_folder) / dict_corr[wavelength_id]
+            ).as_posix()
         )
         if corrections[wavelength_id].shape != (img_size_y, img_size_x):
-            raise Exception(
+            raise ValueError(
                 "Error in illumination_correction, "
                 "correction matrix has wrong shape."
             )
 
     # Lazily load highest-res level from original zarr array
-    data_czyx = da.from_zarr(f"{zarrurl_old}/0")
+    data_czyx = da.from_zarr(f"{zarr_url}/0")
 
     # Create zarr for output
-    if overwrite:
-        fov_path = zarrurl_old
-        new_zarr = zarr.open(f"{zarrurl_old}/0")
+    if overwrite_input:
+        new_zarr = zarr.open(f"{zarr_url_new}/0")
     else:
-        fov_path = zarrurl_new
         new_zarr = zarr.create(
             shape=data_czyx.shape,
             chunks=data_czyx.chunksize,
             dtype=data_czyx.dtype,
-            store=zarr.storage.FSStore(f"{zarrurl_new}/0"),
+            store=zarr.storage.FSStore(f"{zarr_url_new}/0"),
             overwrite=False,
             dimension_separator="/",
         )
 
     # Iterate over FOV ROIs
     num_ROIs = len(list_indices)
     for i_c, channel in enumerate(channels):
@@ -240,56 +240,46 @@
             logger.info(
                 f"Now processing ROI {i_ROI+1}/{num_ROIs} "
                 f"for channel {i_c+1}/{num_channels}"
             )
             # Execute illumination correction
             corrected_fov = correct(
                 data_czyx[region].compute(),
-                corrections[channel["wavelength_id"]],
+                corrections[channel.wavelength_id],
                 background=background,
             )
             # Write to disk
             da.array(corrected_fov).to_zarr(
                 url=new_zarr,
                 region=region,
                 compute=True,
             )
 
     # Starting from on-disk highest-resolution data, build and write to disk a
     # pyramid of coarser levels
     build_pyramid(
-        zarrurl=fov_path,
-        overwrite=overwrite,
+        zarrurl=zarr_url_new,
+        overwrite=True,
         num_levels=num_levels,
         coarsening_xy=coarsening_xy,
         chunksize=data_czyx.chunksize,
     )
 
     t_end = time.perf_counter()
     logger.info(f"End illumination_correction, elapsed: {t_end-t_start}")
 
-    return {}
+    if overwrite_input:
+        image_list_updates = dict(image_list_updates=[dict(zarr_url=zarr_url)])
+    else:
+        image_list_updates = dict(
+            image_list_updates=[dict(zarr_url=zarr_url_new, origin=zarr_url)]
+        )
+    return image_list_updates
 
 
 if __name__ == "__main__":
-
-    from pydantic import BaseModel
-    from pydantic import Extra
-    from fractal_tasks_core._utils import run_fractal_task
-
-    class TaskArguments(BaseModel, extra=Extra.forbid):
-        # Fractal arguments
-        input_paths: Sequence[str]
-        output_path: str
-        component: str
-        metadata: Dict[str, Any]
-        # Task-specific arguments
-        overwrite: Optional[bool]
-        new_component: Optional[str]
-        dict_corr: dict
-        background: Optional[int]
+    from fractal_tasks_core.tasks._utils import run_fractal_task
 
     run_fractal_task(
         task_function=illumination_correction,
-        TaskArgsModel=TaskArguments,
         logger_name=logger.name,
     )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_ROI_overlaps.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/v1_overlaps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,107 +1,49 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Joel Lüthi  <joel.luethi@fmi.ch>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Functions to identify and remove overlaps between regions of interest
+Functions to identify and remove ROI overlaps, based on V1 table specs.
 """
 import logging
+from typing import Callable
 from typing import Optional
 from typing import Sequence
+from typing import Union
 
 import pandas as pd
 
-logger = logging.getLogger(__name__)
-
-
-def is_overlapping_1D(
-    line1: Sequence[float], line2: Sequence[float], tol: float = 0
-) -> bool:
-    """
-    Given two intervals, finds whether they overlap
-
-    This is based on https://stackoverflow.com/a/70023212/19085332, and we
-    additionally use a finite tolerance for floating-point comparisons.
-
-    :param line1: The boundaries of the first interval , written as
-                  ``[x_min, x_max]``.
-    :param line2: The boundaries of the second interval , written as
-                  ``[x_min, x_max]``.
-    :param tol: Finite tolerance for floating-point comparisons.
-    """
-    return line1[0] <= line2[1] - tol and line2[0] <= line1[1] - tol
-
-
-def is_overlapping_2D(
-    box1: Sequence[float], box2: Sequence[float], tol: float = 0
-) -> bool:
-    """
-    Given two rectangular boxes, finds whether they overlap
-
-    This is based on https://stackoverflow.com/a/70023212/19085332, and we
-    additionally use a finite tolerance for floating-point comparisons.
-
-    :param box1: The boundaries of the first rectangle, written as
-                 ``[x_min, y_min, x_max, y_max]``.
-    :param box2: The boundaries of the second rectangle, written as
-                 ``[x_min, y_min, x_max, y_max]``.
-    :param tol: Finite tolerance for floating-point comparisons.
-    """
-    overlap_x = is_overlapping_1D(
-        [box1[0], box1[2]], [box2[0], box2[2]], tol=tol
-    )
-    overlap_y = is_overlapping_1D(
-        [box1[1], box1[3]], [box2[1], box2[3]], tol=tol
-    )
-    return overlap_x and overlap_y
-
+from fractal_tasks_core.roi._overlaps_common import _is_overlapping_3D_int
+from fractal_tasks_core.roi._overlaps_common import is_overlapping_1D
+from fractal_tasks_core.roi._overlaps_common import is_overlapping_2D
+from fractal_tasks_core.roi._overlaps_common import is_overlapping_3D
 
-def is_overlapping_3D(box1, box2, tol=0) -> bool:
-    """
-    Given two three-dimensional boxes, finds whether they overlap
-
-    This is based on https://stackoverflow.com/a/70023212/19085332, and we
-    additionally use a finite tolerance for floating-point comparisons.
 
-    :param box1: The boundaries of the first box, written as
-                 ``[x_min, y_min, z_min, x_max, y_max, z_max]``.
-    :param box2: The boundaries of the second box, written as
-                 ``[x_min, y_min, z_min, x_max, y_max, z_max]``.
-    :param tol: Finite tolerance for floating-point comparisons.
-    """
-
-    overlap_x = is_overlapping_1D(
-        [box1[0], box1[3]], [box2[0], box2[3]], tol=tol
-    )
-    overlap_y = is_overlapping_1D(
-        [box1[1], box1[4]], [box2[1], box2[4]], tol=tol
-    )
-    overlap_z = is_overlapping_1D(
-        [box1[2], box1[5]], [box2[2], box2[5]], tol=tol
-    )
-    return overlap_x and overlap_y and overlap_z
+logger = logging.getLogger(__name__)
 
 
-def get_overlapping_pair(tmp_df: pd.DataFrame, tol: float = 0) -> tuple[int]:
+def get_overlapping_pair(
+    tmp_df: pd.DataFrame, tol: float = 1e-10
+) -> Union[tuple[int, int], bool]:
     """
-    Finds the indices for the next overlapping FOVs pair
+    Finds the indices for the next overlapping FOVs pair.
 
-    Note: the returned indices are positional indices, starting from 0
+    Note: the returned indices are positional indices, starting from 0.
 
-    :param tmp_df: Dataframe with columns `["xmin", "ymin", "xmax", "ymax"]`.
-    :param tol: Finite tolerance for floating-point comparisons.
+    Args:
+        tmp_df: Dataframe with columns `["xmin", "ymin", "xmax", "ymax"]`.
+        tol: Finite tolerance for floating-point comparisons.
     """
 
     num_lines = len(tmp_df.index)
     for pos_ind_1 in range(num_lines):
         for pos_ind_2 in range(pos_ind_1):
             if is_overlapping_2D(
                 tmp_df.iloc[pos_ind_1], tmp_df.iloc[pos_ind_2], tol=tol
@@ -111,21 +53,22 @@
 
 
 def get_overlapping_pairs_3D(
     tmp_df: pd.DataFrame,
     full_res_pxl_sizes_zyx: Sequence[float],
 ):
     """
-    Finds the indices for the all overlapping FOVs pair, in three dimensions
+    Finds the indices for the all overlapping FOVs pair, in three dimensions.
 
-    Note: the returned indices are positional indices, starting from 0
+    Note: the returned indices are positional indices, starting from 0.
 
-    :param tmp_df: Dataframe with columns ``{x,y,z}_micrometer`` and
-                   ``len_{x,y,z}_micrometer``.
-    :param pixel_sizes: TBD
+    Args:
+        tmp_df: Dataframe with columns `{x,y,z}_micrometer` and
+            `len_{x,y,z}_micrometer`.
+        full_res_pxl_sizes_zyx: TBD
     """
 
     tol = 1e-10
     if tol > min(full_res_pxl_sizes_zyx) / 1e3:
         raise ValueError(f"{tol=} but {full_res_pxl_sizes_zyx=}")
 
     new_tmp_df = tmp_df.copy()
@@ -162,16 +105,26 @@
 
 
 def apply_shift_in_one_direction(
     tmp_df_well: pd.DataFrame,
     line_1: Sequence[float],
     line_2: Sequence[float],
     mu: str,
-    tol: float = 0,
+    tol: float = 1e-10,
 ):
+    """
+    TBD
+
+    Args:
+        tmp_df_well: TBD
+        line_1: TBD
+        line_2: TBD
+        mu: TBD
+        tol: TBD
+    """
     min_1, max_1 = line_1[:]
     min_2, max_2 = line_2[:]
     min_max = min(max_1, max_2)
     max_min = max(min_1, min_2)
     shift = min_max - max_min
     logging.debug(f"{mu}-shifting by {shift=}")
     ind = tmp_df_well.loc[:, f"{mu}min"] >= max_min - tol
@@ -184,17 +137,18 @@
     tmp_df_well.loc[ind, f"{mu}max"] += shift
     tmp_df_well.loc[ind, f"{mu}_micrometer"] += shift
     return tmp_df_well
 
 
 def remove_FOV_overlaps(df: pd.DataFrame):
     """
-    Given a metadata dataframe, shift its columns to remove FOV overlaps
+    Given a metadata dataframe, shift its columns to remove FOV overlaps.
 
-    :param df: Metadata dataframe
+    Args:
+        df: Metadata dataframe.
     """
 
     # Set tolerance (this should be much smaller than pixel size or expected
     # round-offs), and maximum number of iterations in constraint solver
     tol = 1e-10
     max_iterations = 200
 
@@ -212,15 +166,15 @@
     # Create columns with the original positions (not to be removed)
     df["x_micrometer_original"] = df["x_micrometer"]
     df["y_micrometer_original"] = df["y_micrometer"]
 
     # Check that tolerance is much smaller than pixel sizes
     min_pixel_size = df[["pixel_size_x", "pixel_size_y"]].min().min()
     if tol > min_pixel_size / 1e3:
-        raise Exception(
+        raise ValueError(
             f"In remove_FOV_overlaps, {tol=} but {min_pixel_size=}"
         )
 
     # Loop over wells
     wells = sorted(list(set([ind[0] for ind in df.index])))
     for well in wells:
 
@@ -317,68 +271,133 @@
 
     # Remove temporary columns that were added only as part of this function
     df.drop(list_columns, axis=1, inplace=True)
 
     return df
 
 
-def _is_overlapping_1D_int(
-    line1: Sequence[int],
-    line2: Sequence[int],
-) -> bool:
-    """
-    Given two integer intervals, find whether they overlap
-
-    This is the same as is_overlapping_1D (based on
-    https://stackoverflow.com/a/70023212/19085332), for integer-valued
-    intervals.
-
-    :param line1: The boundaries of the first interval , written as
-                  ``[x_min, x_max]``.
-    :param line2: The boundaries of the second interval , written as
-                  ``[x_min, x_max]``.
-    """
-    return line1[0] < line2[1] and line2[0] < line1[1]
-
-
-def _is_overlapping_3D_int(box1: list[int], box2: list[int]) -> bool:
-    """
-    Given two three-dimensional integer boxes, find whether they overlap
-
-    This is the same as is_overlapping_3D (based on
-    https://stackoverflow.com/a/70023212/19085332), for integer-valued
-    boxes.
-
-    :param box1: The boundaries of the first box, written as
-                 ``[x_min, y_min, z_min, x_max, y_max, z_max]``.
-    :param box2: The boundaries of the second box, written as
-                 ``[x_min, y_min, z_min, x_max, y_max, z_max]``.
-    """
-    overlap_x = _is_overlapping_1D_int([box1[0], box1[3]], [box2[0], box2[3]])
-    overlap_y = _is_overlapping_1D_int([box1[1], box1[4]], [box2[1], box2[4]])
-    overlap_z = _is_overlapping_1D_int([box1[2], box1[5]], [box2[2], box2[5]])
-    return overlap_x and overlap_y and overlap_z
-
-
 def find_overlaps_in_ROI_indices(
     list_indices: list[list[int]],
-) -> Optional[tuple[int]]:
+) -> Optional[tuple[int, int]]:
     """
-    Given a list of integer ROI indices, find whether there are overlaps
+    Given a list of integer ROI indices, find whether there are overlaps.
 
-    :param list_indices: List of ROI indices, where each element in the list
-                         should look like ``[start_z, end_z, start_y, end_y,
-                         start_x, end_x]``.
-    :returns: ``None`` if no overlap was detected, otherwise a tuple with the
-              positional indices of a pair of overlapping ROIs.
+    Args:
+        list_indices: List of ROI indices, where each element in the list
+            should look like
+            `[start_z, end_z, start_y, end_y, start_x, end_x]`.
+
+    Returns:
+        `None` if no overlap was detected, otherwise a tuple with the
+            positional indices of a pair of overlapping ROIs.
     """
 
     for ind_1, ROI_1 in enumerate(list_indices):
         s_z, e_z, s_y, e_y, s_x, e_x = ROI_1[:]
         box_1 = [s_x, s_y, s_z, e_x, e_y, e_z]
         for ind_2 in range(ind_1):
             ROI_2 = list_indices[ind_2]
             s_z, e_z, s_y, e_y, s_x, e_x = ROI_2[:]
             box_2 = [s_x, s_y, s_z, e_x, e_y, e_z]
             if _is_overlapping_3D_int(box_1, box_2):
                 return (ind_1, ind_2)
     return None
+
+
+def check_well_for_FOV_overlap(
+    site_metadata: pd.DataFrame,
+    selected_well: str,
+    plotting_function: Callable,
+    tol: float = 1e-10,
+):
+    """
+    This function is currently only used in tests and examples.
+
+    The `plotting_function` parameter is exposed so that other tools (see
+    examples in this repository) may use it to show the FOV ROIs.
+
+    Args:
+        site_metadata: TBD
+        selected_well: TBD
+        plotting_function: TBD
+        tol: TBD
+    """
+
+    df = site_metadata.loc[selected_well].copy()
+    df["xmin"] = df["x_micrometer"]
+    df["ymin"] = df["y_micrometer"]
+    df["xmax"] = df["x_micrometer"] + df["pixel_size_x"] * df["x_pixel"]
+    df["ymax"] = df["y_micrometer"] + df["pixel_size_y"] * df["y_pixel"]
+
+    xmin = list(df.loc[:, "xmin"])
+    ymin = list(df.loc[:, "ymin"])
+    xmax = list(df.loc[:, "xmax"])
+    ymax = list(df.loc[:, "ymax"])
+    num_lines = len(xmin)
+
+    list_overlapping_FOVs = []
+    for line_1 in range(num_lines):
+        min_x_1, max_x_1 = [a[line_1] for a in [xmin, xmax]]
+        min_y_1, max_y_1 = [a[line_1] for a in [ymin, ymax]]
+        for line_2 in range(line_1):
+            min_x_2, max_x_2 = [a[line_2] for a in [xmin, xmax]]
+            min_y_2, max_y_2 = [a[line_2] for a in [ymin, ymax]]
+            overlap = is_overlapping_2D(
+                (min_x_1, min_y_1, max_x_1, max_y_1),
+                (min_x_2, min_y_2, max_x_2, max_y_2),
+                tol=tol,
+            )
+            if overlap:
+                list_overlapping_FOVs.append(line_1)
+                list_overlapping_FOVs.append(line_2)
+
+    # Call plotting_function
+    plotting_function(
+        xmin, xmax, ymin, ymax, list_overlapping_FOVs, selected_well
+    )
+
+    if len(list_overlapping_FOVs) > 0:
+        # Increase values by one to switch from index to the label plotted
+        return {selected_well: [x + 1 for x in list_overlapping_FOVs]}
+
+
+def run_overlap_check(
+    site_metadata: pd.DataFrame,
+    tol: float = 1e-10,
+    plotting_function: Optional[Callable] = None,
+):
+    """
+    Run an overlap check over all wells and optionally plots overlaps.
+
+    This function is currently only used in tests and examples.
+
+    The `plotting_function` parameter is exposed so that other tools (see
+    examples in this repository) may use it to show the FOV ROIs. Its arguments
+    are: `[xmin, xmax, ymin, ymax, list_overlapping_FOVs, selected_well]`.
+
+    Args:
+        site_metadata: TBD
+        tol: TBD
+        plotting_function: TBD
+    """
+
+    if plotting_function is None:
+
+        def plotting_function(
+            xmin, xmax, ymin, ymax, list_overlapping_FOVs, selected_well
+        ):
+            pass
+
+    wells = site_metadata.index.unique(level="well_id")
+    overlapping_FOVs = []
+    for selected_well in wells:
+        overlap_curr_well = check_well_for_FOV_overlap(
+            site_metadata,
+            selected_well=selected_well,
+            tol=tol,
+            plotting_function=plotting_function,
+        )
+        if overlap_curr_well:
+            print(selected_well)
+            overlapping_FOVs.append(overlap_curr_well)
+
+    return overlapping_FOVs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_masked_loading.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/masked_loading.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,91 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Functions to use masked loading of ROIs before/after processing
+Functions to use masked loading of ROIs before/after processing.
 """
 import logging
 from pathlib import Path
 from typing import Callable
 from typing import Optional
 
 import anndata as ad
 import dask.array as da
 import numpy as np
 import zarr
 
-from fractal_tasks_core.lib_upscale_array import convert_region_to_low_res
-from fractal_tasks_core.lib_upscale_array import upscale_array
+from fractal_tasks_core.tables.v1 import MaskingROITableAttrs
+from fractal_tasks_core.upscale_array import convert_region_to_low_res
+from fractal_tasks_core.upscale_array import upscale_array
 
 logger = logging.getLogger(__name__)
 
 
 def _preprocess_input(
     image_array: np.ndarray,
     *,
-    region: tuple[slice],
+    region: tuple[slice, ...],
     current_label_path: str,
     ROI_table_path: str,
     ROI_positional_index: int,
 ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
-    Preprocess a four-dimensional cellpose input
+    Preprocess a four-dimensional cellpose input.
 
     This involves :
 
     - Loading the masking label array for the appropriate ROI;
-    - Extracting the appropriate label value from the ``ROI_table.obs``
+    - Extracting the appropriate label value from the `ROI_table.obs`
       dataframe;
     - Constructing the background mask, where the masking label matches with a
       specific label value;
-    - Setting the background of ``image_array`` to ``0``;
+    - Setting the background of `image_array` to `0`;
     - Loading the array which will be needed in postprocessing to restore
       background.
 
-    **NOTE 1**: This function relies on a change to OME-NGFF table specs
-    (https://github.com/ome/ngff/pull/64) which is still in-progress.
+    **NOTE 1**: This function relies on V1 of the Fractal table specifications,
+    see
+    https://fractal-analytics-platform.github.io/fractal-tasks-core/tables/.
 
     **NOTE 2**: The pre/post-processing functions and the
     masked_loading_wrapper are currently meant to work as part of the
     cellpose_segmentation task, with the plan of then making them more
     flexible; see
     https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/340.
 
     Naming of variables refers to a two-steps labeling, as in "first identify
     organoids, then look for nuclei inside each organoid") :
 
-    - ``"masking"`` refers to the labels that are used to identify the object
+    - `"masking"` refers to the labels that are used to identify the object
       vs background (e.g. the organoid labels); these labels already exist.
-    - ``"current"`` refers to the labels that are currently being computed in
-      the ``cellpose_segmentation`` task, e.g. the nuclear labels.
+    - `"current"` refers to the labels that are currently being computed in
+      the `cellpose_segmentation` task, e.g. the nuclear labels.
 
-    :param image_array: The 4D CZYX array with image data for a specific ROI.
-    :param region: The ZYX indices of the ROI, in a form like ``(slice(0, 1),
-                   slice(1000, 2000), slice(1000, 2000))``.
-    :param current_label_path: Path to the image used as current
-                               label, in a form like
-                               ``/somewhere/plate.zarr/A/01/0/labels/nuclei_in_organoids/0``.
-    :param ROI_table_path: Path of the AnnData table for the masking-label
-                           ROIs; this is used (together with
-                           ``ROI_positional_index``) to extract
-                           ``label_value``.
-    :param ROI_positional_index: Index of the current ROI, which is used to
-                                 extract ``label_value`` from
-                                 ``ROI_table_obs``.
-    :returns: A tuple with three arrays: the preprocessed image array, the
-              background mask, the current label.
+    Args:
+        image_array: The 4D CZYX array with image data for a specific ROI.
+        region: The ZYX indices of the ROI, in a form like
+            `(slice(0, 1), slice(1000, 2000), slice(1000, 2000))`.
+        current_label_path: Path to the image used as current label, in a form
+            like `/somewhere/plate.zarr/A/01/0/labels/nuclei_in_organoids/0`.
+        ROI_table_path: Path of the AnnData table for the masking-label ROIs;
+            this is used (together with `ROI_positional_index`) to extract
+            `label_value`.
+        ROI_positional_index: Index of the current ROI, which is used to
+            extract `label_value` from `ROI_table_obs`.
+    Returns:
+        A tuple with three arrays: the preprocessed image array, the background
+            mask, the current label.
     """
 
     logger.info(f"[_preprocess_input] {image_array.shape=}")
     logger.info(f"[_preprocess_input] {region=}")
 
     # Check that image data are 4D (CZYX) - FIXME issue 340
     if not image_array.ndim == 4:
@@ -96,16 +95,15 @@
         )
 
     # Load the ROI table and its metadata attributes
     ROI_table = ad.read_zarr(ROI_table_path)
     attrs = zarr.group(ROI_table_path).attrs
     logger.info(f"[_preprocess_input] {ROI_table_path=}")
     logger.info(f"[_preprocess_input] {attrs.asdict()=}")
-    if not attrs["type"] == "ngff:region_table":
-        raise ValueError("Wrong attributes for {ROI_table_path}:\n{attrs}")
+    MaskingROITableAttrs(**attrs.asdict())
     label_relative_path = attrs["region"]["path"]
     column_name = attrs["instance_key"]
 
     # Check that ROI_table.obs has the right column and extract label_value
     if column_name not in ROI_table.obs.columns:
         raise ValueError(
             'In _preprocess_input, "{column_name}" '
@@ -113,15 +111,15 @@
         )
     label_value = int(ROI_table.obs[column_name][ROI_positional_index])
 
     # Load masking-label array (lazily)
     masking_label_path = str(
         Path(ROI_table_path).parent / label_relative_path / "0"
     )
-    logger.critical(f"{masking_label_path=}")
+    logger.info(f"{masking_label_path=}")
     masking_label_array = da.from_zarr(masking_label_path)
     logger.info(
         f"[_preprocess_input] {masking_label_path=}, "
         f"{masking_label_array.shape=}"
     )
 
     # Load current-label array (lazily)
@@ -168,42 +166,45 @@
     background_3D = masking_label_region != label_value
     if (masking_label_region == label_value).sum() == 0:
         raise ValueError(
             f"Label {label_value} is not present in the extracted ROI"
         )
 
     # Set image background to zero
-    background_4D = np.expand_dims(background_3D, axis=0)
-    image_array[background_4D] = 0
+    n_channels = image_array.shape[0]
+    for i in range(n_channels):
+        image_array[i, background_3D] = 0
 
     return (image_array, background_3D, current_label_region)
 
 
 def _postprocess_output(
     *,
     modified_array: np.ndarray,
     original_array: np.ndarray,
     background: np.ndarray,
 ) -> np.ndarray:
     """
-    Postprocess cellpose output, mainly to restore its original background
+    Postprocess cellpose output, mainly to restore its original background.
 
     **NOTE**: The pre/post-processing functions and the
     masked_loading_wrapper are currently meant to work as part of the
     cellpose_segmentation task, with the plan of then making them more
     flexible; see
     https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/340.
 
-    :param modified_array: The 3D (ZYX) array with the correct object data and
-                           wrong background data.
-    :param original_array: The 3D (ZYX) array with the wrong object data and
-                           correct background data.
-    :param background: The 3D (ZYX) boolean array that defines the
-                       background.
-    :returns: The postprocessed array.
+    Args:
+        modified_array: The 3D (ZYX) array with the correct object data and
+            wrong background data.
+        original_array: The 3D (ZYX) array with the wrong object data and
+            correct background data.
+        background: The 3D (ZYX) boolean array that defines the background.
+
+    Returns:
+        The postprocessed array.
     """
     # Restore background
     modified_array[background] = original_array[background]
     return modified_array
 
 
 def masked_loading_wrapper(
@@ -213,23 +214,23 @@
     kwargs: Optional[dict] = None,
     use_masks: bool,
     preprocessing_kwargs: Optional[dict] = None,
 ):
     """
     Wrap a function with some pre/post-processing functions
 
-    :param function: The callable function to be wrapped.
-    :param image_array: The image array to be preprocessed and then used as
-                        positional argument for ``function``.
-    :param kwargs: Keyword arguments for ``function``.
-    :param use_masks: If ``False``, the wrapper only calls ``function(*args,
-                      **kwargs)``.
-    :param preprocessing_kwargs: Keyword arguments for the preprocessing
-                                 function (see call signature of
-                                 ``_preprocess_input()``).
+    Args:
+        function: The callable function to be wrapped.
+        image_array: The image array to be preprocessed and then used as
+            positional argument for `function`.
+        kwargs: Keyword arguments for `function`.
+        use_masks: If `False`, the wrapper only calls
+            `function(*args, **kwargs)`.
+        preprocessing_kwargs: Keyword arguments for the preprocessing function
+            (see call signature of `_preprocess_input()`).
     """
     # Optional preprocessing
     if use_masks:
         preprocessing_kwargs = preprocessing_kwargs or {}
         (
             image_array,
             background_3D,
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_metadata_parsing.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/cellvoyager/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,50 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Joel Lüthi  <joel.luethi@fmi.ch>
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Joel Lüthi  <joel.luethi@fmi.ch>
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Functions to create a metadata dataframe from Yokogawa files
+Functions to create a metadata dataframe from Yokogawa files.
 """
 import fnmatch
 import logging
 from pathlib import Path
 from typing import Optional
-from typing import Tuple
 from typing import Union
 
 import numpy as np
 import pandas as pd
 from defusedxml import ElementTree
 
 logger = logging.getLogger(__name__)
 
 
 def parse_yokogawa_metadata(
     mrf_path: Union[str, Path],
     mlf_path: Union[str, Path],
     *,
     filename_patterns: Optional[list[str]] = None,
-) -> Tuple[pd.DataFrame, dict[str, int]]:
+) -> tuple[pd.DataFrame, dict[str, int]]:
     """
-    Parse Yokogawa CV7000 metadata files and prepare site-level metadata
+    Parse Yokogawa CV7000 metadata files and prepare site-level metadata.
 
-    :param mrf_path: Full path to MeasurementDetail.mrf metadata file
-    :param mlf_path: Full path to MeasurementData.mlf metadata file
-    :param filename_patterns: List of patterns to filter the image filenames in
-                              the mlf metadata table. Patterns must be defined
-                              as in
-                              https://docs.python.org/3/library/fnmatch.html
+    Args:
+        mrf_path: Full path to MeasurementDetail.mrf metadata file.
+        mlf_path: Full path to MeasurementData.mlf metadata file.
+        filename_patterns:
+            List of patterns to filter the image filenames in the mlf metadata
+            table. Patterns must be defined as in
+            https://docs.python.org/3/library/fnmatch.html
     """
 
     # Convert paths to strings
     mrf_str = Path(mrf_path).as_posix()
     mlf_str = Path(mlf_path).as_posix()
 
     mrf_frame, mlf_frame, error_count = read_metadata_files(
@@ -119,24 +117,24 @@
     return site_metadata, number_of_files
 
 
 def read_metadata_files(
     mrf_path: str,
     mlf_path: str,
     filename_patterns: Optional[list[str]] = None,
-) -> Tuple[pd.DataFrame, pd.DataFrame, int]:
+) -> tuple[pd.DataFrame, pd.DataFrame, int]:
     """
     TBD
 
-    :param mrf_path: Full path to MeasurementDetail.mrf metadata file
-    :param mlf_path: Full path to MeasurementData.mlf metadata file
-    :param filename_patterns: List of patterns to filter the image filenames in
-                              the mlf metadata table. Patterns must be defined
-                              as in
-                              https://docs.python.org/3/library/fnmatch.html
+    Args:
+        mrf_path: Full path to MeasurementDetail.mrf metadata file.
+        mlf_path: Full path to MeasurementData.mlf metadata file.
+        filename_patterns: List of patterns to filter the image filenames in
+            the mlf metadata table. Patterns must be defined as in
+            https://docs.python.org/3/library/fnmatch.html.
     """
 
     # parsing of mrf & mlf files are based on the
     # yokogawa_image_collection_task v0.5 in drogon, written by Dario Vischi.
     # https://github.com/fmi-basel/job-system-workflows/blob/00bbf34448972d27f258a2c28245dd96180e8229/src/gliberal_workflows/tasks/yokogawa_image_collection_task/versions/version_0_5.py  # noqa
     # Now modified for Fractal use
 
@@ -152,15 +150,16 @@
     return mrf_frame, mlf_frame, error_count
 
 
 def read_mrf_file(mrf_path: str):
     """
     TBD
 
-    :param mrf_path: Full path to MeasurementDetail.mrf metadata file
+    Args:
+        mrf_path: Full path to MeasurementDetail.mrf metadata file.
     """
 
     # Prepare mrf dataframe
     mrf_columns = [
         "channel_id",
         "horiz_pixel_dim",
         "vert_pixel_dim",
@@ -192,24 +191,24 @@
         ]
 
     return mrf_frame
 
 
 def read_mlf_file(
     mlf_path: str,
-    filename_patterns=None,
-) -> Tuple[pd.DataFrame, int]:
+    filename_patterns: Optional[list[str]] = None,
+) -> tuple[pd.DataFrame, int]:
     """
     TBD
 
-    :param mlf_path: Full path to MeasurementData.mlf metadata file
-    :param filename_patterns: List of patterns to filter the image filenames in
-                              the mlf metadata table. Patterns must be defined
-                              as in
-                              https://docs.python.org/3/library/fnmatch.html
+    Args:
+        mlf_path: Full path to MeasurementData.mlf metadata file.
+        filename_patterns: List of patterns to filter the image filenames in
+            the mlf metadata table. Patterns must be defined as in
+            https://docs.python.org/3/library/fnmatch.html.
     """
 
     # Load the whole MeasurementData.mlf file
     mlf_frame_raw = pd.read_xml(mlf_path)
 
     # Remove all rows that do not match the given patterns
     logger.info(
@@ -258,36 +257,38 @@
     return mlf_frame, error_count
 
 
 def calculate_steps(site_series: pd.Series):
     """
     TBD
 
-    :param site_series: TBD
+    Args:
+        site_series: TBD
     """
 
     # site_series is the z_micrometer series for a given site of a given
     # channel. This function calculates the step size in Z
 
     # First diff is always NaN because there is nothing to compare it to
     steps = site_series.diff().dropna().astype(float)
     if not np.allclose(steps.iloc[0], np.array(steps)):
-        raise Exception(
+        raise NotImplementedError(
             "When parsing the Yokogawa mlf file, some sites "
             "had varying step size in Z. "
             "That is not supported for the OME-Zarr parsing"
         )
     return steps.mean()
 
 
-def get_z_steps(mlf_frame):
+def get_z_steps(mlf_frame: pd.DataFrame) -> pd.DataFrame:
     """
     TBD
 
-    :param mlf_frame: TBD
+    Args:
+        mlf_frame: TBD
     """
 
     # Process mlf_frame to extract Z information (pixel size & steps).
     # Run checks on consistencies & return site-based z step dataframe
     # Group by well, field & channel
     grouped_sites_z = (
         mlf_frame.loc[
@@ -332,40 +333,42 @@
 
     # Combine the two dataframes
     z_frame = pd.concat([z_data.mean(), z_steps], axis=1)
     z_frame.columns = ["pixel_size_z", "z_pixel"]
     return z_frame
 
 
-def get_earliest_time_per_site(mlf_frame) -> pd.DataFrame:
+def get_earliest_time_per_site(mlf_frame: pd.DataFrame) -> pd.DataFrame:
     """
     TBD
 
-    :param mlf_frame: TBD
+    Args:
+        mlf_frame: TBD
     """
 
     # Get the time information per site
     # Because a site will contain time information for each plane
     # of each channel, we just return the earliest time infromation
     # per site.
     return pd.to_datetime(
         mlf_frame.groupby(["well_id", "FieldIndex"]).min()["Time"], utc=True
     )
 
 
-def check_group_consistency(grouped_df, message: str = ""):
+def check_group_consistency(grouped_df: pd.DataFrame, message: str = ""):
     """
     TBD
 
-    :param grouped_df: TBD
-    :param message: TBD
+    Args:
+        grouped_df: TBD
+        message: TBD
     """
 
     # Check consistency in grouped df for multi-index, multi-column dataframes
     # raises an exception if there is variability
     diff_df = grouped_df.max() - grouped_df.min()
     if not np.isclose(np.sum(np.sum(diff_df)), 0.0):
-        raise Exception(
+        raise ValueError(
             "During metadata parsing, a consistency check failed: \n"
             f"{message}\n"
             f"Difference dataframe: \n{diff_df}"
         )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_pyramid_creation.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/pyramids.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,87 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Marco Franzon <marco.franzon@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Construct and write pyramid of lower-resolution levels
+Construct and write pyramid of lower-resolution levels.
 """
+import logging
 import pathlib
 from typing import Callable
+from typing import Optional
 from typing import Sequence
 from typing import Union
 
 import dask.array as da
 import numpy as np
 
+logger = logging.getLogger(__name__)
+
 
 def build_pyramid(
     *,
     zarrurl: Union[str, pathlib.Path],
     overwrite: bool = False,
     num_levels: int = 2,
     coarsening_xy: int = 2,
-    chunksize: Sequence[int] = None,
-    aggregation_function: Callable = None,
-):
+    chunksize: Optional[Sequence[int]] = None,
+    aggregation_function: Optional[Callable] = None,
+) -> None:
 
     """
     Starting from on-disk highest-resolution data, build and write to disk a
-    pyramid with (num_levels-1) coarsened levels.
+    pyramid with `(num_levels - 1)` coarsened levels.
     This function works for 2D, 3D or 4D arrays.
 
-    Example input:
-        zarrurl = "some/path/plate.zarr/B/03/0
-
-    :param zarrurl: path of the zarr group, which must already include level 0
-    :param overwrite: whether to overwrite existing pyramid levels
-    :param num_levels: total number of pyramid levels (including 0)
-    :param coarsening_xy: linear coarsening factor between subsequent levels
-    :param chunksize: shape of a single chunk
-    :param aggregation_function: function to be used when downsampling
+    Args:
+        zarrurl: Path of the image zarr group, not including the
+            multiscale-level path (e.g. `"some/path/plate.zarr/B/03/0"`).
+        overwrite: Whether to overwrite existing pyramid levels.
+        num_levels: Total number of pyramid levels (including 0).
+        coarsening_xy: Linear coarsening factor between subsequent levels.
+        chunksize: Shape of a single chunk.
+        aggregation_function: Function to be used when downsampling.
     """
 
     # Clean up zarrurl
     zarrurl = str(pathlib.Path(zarrurl))  # FIXME
+
+    # Select full-resolution multiscale level
     zarrurl_highres = f"{zarrurl}/0"
+    logger.info(f"[build_pyramid] High-resolution path: {zarrurl_highres}")
 
     # Lazily load highest-resolution data
     data_highres = da.from_zarr(zarrurl_highres)
+    logger.info(f"[build_pyramid] High-resolution data: {str(data_highres)}")
 
     # Check the number of axes and identify YX dimensions
     ndims = len(data_highres.shape)
     if ndims not in [2, 3, 4]:
-        raise Exception("{data_highres.shape=}, ndims not in [2,3,4]")
+        raise ValueError(f"{data_highres.shape=}, ndims not in [2,3,4]")
     y_axis = ndims - 2
     x_axis = ndims - 1
 
     # Set aggregation_function
     if aggregation_function is None:
         aggregation_function = np.mean
 
     # Compute and write lower-resolution levels
     previous_level = data_highres
     for ind_level in range(1, num_levels):
         # Verify that coarsening is doable
         if min(previous_level.shape[-2:]) < coarsening_xy:
-            raise Exception(
+            raise ValueError(
                 f"ERROR: at {ind_level}-th level, "
                 f"coarsening_xy={coarsening_xy} "
                 f"but previous level has shape {previous_level.shape}"
             )
         # Apply coarsening
         newlevel = da.coarsen(
             aggregation_function,
@@ -86,14 +91,18 @@
         ).astype(data_highres.dtype)
 
         # Apply rechunking
         if chunksize is None:
             newlevel_rechunked = newlevel
         else:
             newlevel_rechunked = newlevel.rechunk(chunksize)
+        logger.info(
+            f"[build_pyramid] Level {ind_level} data: "
+            f"{str(newlevel_rechunked)}"
+        )
 
         # Write zarr and store output (useful to construct next level)
         previous_level = newlevel_rechunked.to_zarr(
             zarrurl,
             component=f"{ind_level}",
             overwrite=overwrite,
             compute=True,
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_regions_of_interest.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/roi/v1.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Joel Lüthi <joel.luethi@uzh.ch>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Joel Lüthi <joel.luethi@uzh.ch>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Functions to handle regions of interests (via pandas and AnnData)
+Functions to produce/process ROI tables.
 """
 import logging
-from typing import Optional
+import math
 from typing import Sequence
 
 import anndata as ad
 import numpy as np
 import pandas as pd
-import zarr
+
+
+logger = logging.getLogger(__name__)
 
 
 def prepare_FOV_ROI_table(
-    df: pd.DataFrame, metadata: list[str] = ["time"]
+    df: pd.DataFrame, metadata: tuple[str, ...] = ("time",)
 ) -> ad.AnnData:
     """
-    Description
+    Prepare an AnnData table for fields-of-view ROIs.
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Args:
+        df:
+            Input dataframe, possibly prepared through
+            `parse_yokogawa_metadata`.
+        metadata:
+            Columns of `df` to be stored (if present) into AnnData table `obs`.
     """
 
     # Make a local copy of the dataframe, to avoid SettingWithCopyWarning
     df = df.copy()
 
     # Convert DataFrame index to str, to avoid
     # >> ImplicitModificationWarning: Transforming to str index
@@ -66,14 +70,18 @@
     # >> UserWarning: X converted to numpy array with dtype float64
     # when creating AnnData object
     df_roi = df.loc[:, positional_columns].astype(np.float32)
 
     # Create an AnnData object directly from the DataFrame
     adata = ad.AnnData(X=df_roi)
 
+    # Reset origin of the FOV ROI table, so that it matches with the well
+    # origin
+    adata = reset_origin(adata)
+
     # Save any metadata that is specified to the obs df
     for col in metadata:
         if col in df:
             # Cast all metadata to str.
             # Reason: AnnData Zarr writers don't support all pandas types.
             # e.g. pandas.core.arrays.datetimes.DatetimeArray can't be written
             adata.obs[col] = df[col].astype(str)
@@ -84,21 +92,25 @@
     adata.obs_names = "FOV_" + adata.obs.index
     adata.var_names = list(map(str, df_roi.columns))
 
     return adata
 
 
 def prepare_well_ROI_table(
-    df: pd.DataFrame, metadata: list[str] = ["time"]
+    df: pd.DataFrame, metadata: tuple[str, ...] = ("time",)
 ) -> ad.AnnData:
     """
-    Description
+    Prepare an AnnData table with a single well ROI.
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Args:
+        df:
+            Input dataframe, possibly prepared through
+            `parse_yokogawa_metadata`.
+        metadata:
+            Columns of `df` to be stored (if present) into AnnData table `obs`.
     """
 
     # Make a local copy of the dataframe, to avoid SettingWithCopyWarning
     df = df.copy()
 
     # Convert DataFrame index to str, to avoid
     # >> ImplicitModificationWarning: Transforming to str index
@@ -136,14 +148,17 @@
     # >> UserWarning: X converted to numpy array with dtype float64
     # when creating AnnData object
     df_roi = df.iloc[0:1, :].loc[:, positional_columns].astype(np.float32)
 
     # Create an AnnData object directly from the DataFrame
     adata = ad.AnnData(X=df_roi)
 
+    # Reset origin of the single-entry well ROI table
+    adata = reset_origin(adata)
+
     # Save any metadata that is specified to the obs df
     for col in metadata:
         if col in df:
             # Cast all metadata to str.
             # Reason: AnnData Zarr writers don't support all pandas types.
             # e.g. pandas.core.arrays.datetimes.DatetimeArray can't be written
             adata.obs[col] = df[col].astype(str)
@@ -158,18 +173,23 @@
 
 
 def convert_ROIs_from_3D_to_2D(
     adata: ad.AnnData,
     pixel_size_z: float,
 ) -> ad.AnnData:
     """
-    Description
+    TBD
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Note that this function is only relevant when the ROIs in adata span the
+    whole extent of the Z axis.
+    TODO: check this explicitly.
+
+    Args:
+        adata: TBD
+        pixel_size_z: TBD
     """
 
     # Compress a 3D stack of images to a single Z plane,
     # with thickness equal to pixel_size_z
     df = adata.to_df()
     df["len_z_micrometer"] = pixel_size_z
 
@@ -199,142 +219,166 @@
         "z_micrometer",
     ],
     cols_xyz_len: Sequence[str] = [
         "len_x_micrometer",
         "len_y_micrometer",
         "len_z_micrometer",
     ],
-    reset_origin: bool = True,
 ) -> list[list[int]]:
     """
-    Description
+    Convert a ROI AnnData table into integer array indices.
 
-    FIXME add docstring
-
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Args:
+        ROI: AnnData table with list of ROIs.
+        full_res_pxl_sizes_zyx:
+            Physical-unit pixel ZYX sizes at the full-resolution pyramid level.
+        level: Pyramid level.
+        coarsening_xy: Linear coarsening factor in the YX plane.
+        cols_xyz_pos: Column names for XYZ ROI positions.
+        cols_xyz_len: Column names for XYZ ROI edges.
+
+    Raises:
+        ValueError:
+            If any of the array indices is negative.
+
+    Returns:
+        Nested list of indices. The main list has one item per ROI. Each ROI
+            item is a list of six integers as in `[start_z, end_z, start_y,
+            end_y, start_x, end_x]`. The array-index interval for a given ROI
+            is `start_x:end_x` along X, and so on for Y and Z.
     """
     # Handle empty ROI table
     if len(ROI) == 0:
         return []
 
     # Set pyramid-level pixel sizes
     pxl_size_z, pxl_size_y, pxl_size_x = full_res_pxl_sizes_zyx
     prefactor = coarsening_xy**level
     pxl_size_x *= prefactor
     pxl_size_y *= prefactor
 
     x_pos, y_pos, z_pos = cols_xyz_pos[:]
     x_len, y_len, z_len = cols_xyz_len[:]
 
-    # FIXME: see discussion on ROI-table origin at
-    # https://github.com/fractal-analytics-platform/fractal-tasks-core/issues/339
-    if reset_origin:
-        origin_x = min(ROI[:, x_pos].X[:, 0])
-        origin_y = min(ROI[:, y_pos].X[:, 0])
-        origin_z = min(ROI[:, z_pos].X[:, 0])
-    else:
-        origin_x = 0.0
-        origin_y = 0.0
-        origin_z = 0.0
-
     list_indices = []
-    for FOV in ROI.obs_names:
-
+    for ROI_name in ROI.obs_names:
         # Extract data from anndata table
-        x_micrometer = ROI[FOV, x_pos].X[0, 0] - origin_x
-        y_micrometer = ROI[FOV, y_pos].X[0, 0] - origin_y
-        z_micrometer = ROI[FOV, z_pos].X[0, 0] - origin_z
-        len_x_micrometer = ROI[FOV, x_len].X[0, 0]
-        len_y_micrometer = ROI[FOV, y_len].X[0, 0]
-        len_z_micrometer = ROI[FOV, z_len].X[0, 0]
+        x_micrometer = ROI[ROI_name, x_pos].X[0, 0]
+        y_micrometer = ROI[ROI_name, y_pos].X[0, 0]
+        z_micrometer = ROI[ROI_name, z_pos].X[0, 0]
+        len_x_micrometer = ROI[ROI_name, x_len].X[0, 0]
+        len_y_micrometer = ROI[ROI_name, y_len].X[0, 0]
+        len_z_micrometer = ROI[ROI_name, z_len].X[0, 0]
 
         # Identify indices along the three dimensions
         start_x = x_micrometer / pxl_size_x
         end_x = (x_micrometer + len_x_micrometer) / pxl_size_x
         start_y = y_micrometer / pxl_size_y
         end_y = (y_micrometer + len_y_micrometer) / pxl_size_y
         start_z = z_micrometer / pxl_size_z
         end_z = (z_micrometer + len_z_micrometer) / pxl_size_z
         indices = [start_z, end_z, start_y, end_y, start_x, end_x]
 
         # Round indices to lower integer
         indices = list(map(round, indices))
 
+        # Fail for negative indices
+        if min(indices) < 0:
+            raise ValueError(
+                f"ROI {ROI_name} converted into negative array indices.\n"
+                f"ZYX position: {z_micrometer}, {y_micrometer}, "
+                f"{x_micrometer}\n"
+                f"ZYX pixel sizes: {pxl_size_z}, {pxl_size_y}, "
+                f"{pxl_size_x} ({level=})\n"
+                "Hint: As of fractal-tasks-core v0.12, FOV/well ROI "
+                "tables with non-zero origins (e.g. the ones created with "
+                "v0.11) are not supported."
+            )
+
         # Append ROI indices to to list
         list_indices.append(indices[:])
 
     return list_indices
 
 
-def _inspect_ROI_table(
-    path: str,
-    full_res_pxl_sizes_zyx: Sequence[float],
-    level: int = 0,
-    coarsening_xy: int = 2,
-) -> None:
+def empty_bounding_box_table() -> pd.DataFrame:
     """
-    Description
+    Construct an empty bounding-box ROI table of given shape.
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
-    """
+    This function mirrors the functionality of `array_to_bounding_box_table`,
+    for the specific case where the array includes no label. The advantages of
+    this function are that:
 
-    print(f"{full_res_pxl_sizes_zyx=}")
+    1. It does not require computing a whole array of zeros;
+    2. We avoid hardcoding column names in the task functions.
 
-    adata = ad.read_zarr(path)
-    df = adata.to_df()
-    print("table")
-    print(df)
-    print()
-
-    try:
-        list_indices = convert_ROI_table_to_indices(
-            adata,
-            level=level,
-            coarsening_xy=coarsening_xy,
-            full_res_pxl_sizes_zyx=full_res_pxl_sizes_zyx,
-            # verbose=True,
-        )
-        print()
-        print(f"level:         {level}")
-        print(f"coarsening_xy: {coarsening_xy}")
-        print("list_indices:")
-        for indices in list_indices:
-            print(indices)
-        print()
-    except KeyError as e:
-        print("Something went wrong in convert_ROI_table_to_indices\n", str(e))
+    Returns:
+        DataFrame with no rows, and with columns corresponding to the output of
+            `array_to_bounding_box_table`.
+    """
 
+    df_columns = [
+        "x_micrometer",
+        "y_micrometer",
+        "z_micrometer",
+        "len_x_micrometer",
+        "len_y_micrometer",
+        "len_z_micrometer",
+    ]
+    df = pd.DataFrame(columns=[x for x in df_columns] + ["label"])
     return df
 
 
 def array_to_bounding_box_table(
-    mask_array: np.ndarray, pxl_sizes_zyx: list[float]
+    mask_array: np.ndarray,
+    pxl_sizes_zyx: list[float],
+    origin_zyx: tuple[int, int, int] = (0, 0, 0),
 ) -> pd.DataFrame:
-
     """
-    Description
+    Construct bounding-box ROI table for a mask array.
 
-    :param dummy: this is just a placeholder
-    :type dummy: int
+    Args:
+        mask_array: Original array to construct bounding boxes.
+        pxl_sizes_zyx: Physical-unit pixel ZYX sizes.
+        origin_zyx: Shift ROI origin by this amount of ZYX pixels.
+
+    Returns:
+        DataFrame with each line representing the bounding-box ROI that
+            corresponds to a unique value of `mask_array`. ROI properties are
+            expressed in physical units (with columns defined as elsewhere this
+            module - see e.g. `prepare_well_ROI_table`), and positions are
+            optionally shifted (if `origin_zyx` is set). An additional column
+            `label` keeps track of the `mask_array` value corresponding to each
+            ROI.
     """
 
+    pxl_sizes_zyx_array = np.array(pxl_sizes_zyx)
+    z_origin, y_origin, x_origin = origin_zyx[:]
+
     labels = np.unique(mask_array)
     labels = labels[labels > 0]
     elem_list = []
     for label in labels:
+        # Compute bounding box
         label_match = np.where(mask_array == label)
-        # FIXME: multiplication of np.ndarray with list
-        zmin, ymin, xmin = np.min(label_match, axis=1) * pxl_sizes_zyx
-        zmax, ymax, xmax = (np.max(label_match, axis=1) + 1) * pxl_sizes_zyx
+        zmin, ymin, xmin = np.min(label_match, axis=1) * pxl_sizes_zyx_array
+        zmax, ymax, xmax = (
+            np.max(label_match, axis=1) + 1
+        ) * pxl_sizes_zyx_array
 
+        # Compute bounding-box edges
         length_x = xmax - xmin
         length_y = ymax - ymin
         length_z = zmax - zmin
+
+        # Shift origin
+        zmin += z_origin * pxl_sizes_zyx[0]
+        ymin += y_origin * pxl_sizes_zyx[1]
+        xmin += x_origin * pxl_sizes_zyx[2]
+
         elem_list.append((xmin, ymin, zmin, length_x, length_y, length_z))
 
     df_columns = [
         "x_micrometer",
         "y_micrometer",
         "z_micrometer",
         "len_x_micrometer",
@@ -347,54 +391,192 @@
     else:
         df = pd.DataFrame(np.array(elem_list), columns=df_columns)
         df["label"] = labels
 
     return df
 
 
-def is_ROI_table_valid(*, table_path: str, use_masks: bool) -> Optional[bool]:
+def convert_indices_to_regions(
+    index: list[int],
+) -> tuple[slice, slice, slice]:
+    """
+    Converts index tuples to region tuple
+
+    Args:
+        index: Tuple containing 6 entries of (z_start, z_end, y_start,
+            y_end, x_start, x_end).
+
+    Returns:
+        region: tuple of three slices (ZYX)
+    """
+    return (
+        slice(index[0], index[1]),
+        slice(index[2], index[3]),
+        slice(index[4], index[5]),
+    )
+
+
+def reset_origin(
+    ROI_table: ad.AnnData,
+    x_pos: str = "x_micrometer",
+    y_pos: str = "y_micrometer",
+    z_pos: str = "z_micrometer",
+) -> ad.AnnData:
+    """
+    Return a copy of a ROI table, with shifted-to-zero origin for some columns.
+
+    Args:
+        ROI_table: Original ROI table.
+        x_pos: Name of the column with X position of ROIs.
+        y_pos: Name of the column with Y position of ROIs.
+        z_pos: Name of the column with Z position of ROIs.
+
+    Returns:
+        A copy of the `ROI_table` AnnData table, where values of `x_pos`,
+            `y_pos` and `z_pos` columns have been shifted by their minimum
+            values.
     """
-    Verify some validity assumptions on a ROI table
+    new_table = ROI_table.copy()
 
-    This function reflects our current working assumptions (e.g. the presence
-    of some specific columns); this may change in future versions.
+    origin_x = min(new_table[:, x_pos].X[:, 0])
+    origin_y = min(new_table[:, y_pos].X[:, 0])
+    origin_z = min(new_table[:, z_pos].X[:, 0])
 
-    If ``use_masks=True``, we verify that the table is suitable to be used as
-    part of our masked-loading functions (see ``lib_masked_loading.py``); if
-    these checks fail, ``use_masks`` should be set to ``False`` upstream in the
-    parent function.
+    for FOV in new_table.obs_names:
+        new_table[FOV, x_pos] = new_table[FOV, x_pos].X[0, 0] - origin_x
+        new_table[FOV, y_pos] = new_table[FOV, y_pos].X[0, 0] - origin_y
+        new_table[FOV, z_pos] = new_table[FOV, z_pos].X[0, 0] - origin_z
 
-    :param table_path: Path of the AnnData ROI table to be checked.
-    :param use_masks: If ``True``, perform some additional checks related to
-                      masked loading.
-    :returns: Always ``None`` if ``use_masks=False``, otherwise return whether
-             the table is valid for masked loading.
+    return new_table
+
+
+def is_standard_roi_table(table: str) -> bool:
     """
+    True if the name of the table contains one of the standard Fractal tables
+
+    If a table name is well_ROI_table, FOV_ROI_table or contains either of the
+    two (e.g. registered_FOV_ROI_table), this function returns True.
+
+    Args:
+        table: table name
+
+    Returns:
+        bool of whether it's a standard ROI table
 
-    # Hard constraint: table columns must include some expected ones
-    table = ad.read_zarr(table_path)
-    columns = [
+    """
+    if "well_ROI_table" in table:
+        return True
+    elif "FOV_ROI_table" in table:
+        return True
+    else:
+        return False
+
+
+def get_single_image_ROI(
+    array_shape: tuple[int, int, int],
+    pixels_ZYX: list[float],
+) -> ad.AnnData:
+    """
+    Produce a table with a single ROI that covers the whole array
+
+    TODO: make this flexible with respect to the presence/absence of Z.
+
+    Args:
+        array_shape: ZYX shape of the image array.
+        pixels_ZYX: ZYX pixel sizes in micrometers.
+
+    Returns:
+        An `AnnData` table with a single ROI.
+    """
+    shape_z, shape_y, shape_x = array_shape[-3:]
+    ROI_table = ad.AnnData(
+        X=np.array(
+            [
+                [
+                    0.0,
+                    0.0,
+                    0.0,
+                    shape_x * pixels_ZYX[2],
+                    shape_y * pixels_ZYX[1],
+                    shape_z * pixels_ZYX[0],
+                ],
+            ],
+            dtype=np.float32,
+        )
+    )
+    ROI_table.obs_names = ["image_1"]
+    ROI_table.var_names = [
         "x_micrometer",
         "y_micrometer",
         "z_micrometer",
         "len_x_micrometer",
         "len_y_micrometer",
         "len_z_micrometer",
     ]
-    for column in columns:
-        if column not in table.var_names:
-            raise ValueError(f"Column {column} is not present in ROI table")
-    if not use_masks:
-        return None
-
-    # Soft constraint: the table can be used for masked loading (if not, return
-    # False)
-    attrs = zarr.group(table_path).attrs
-    logging.info(f"ROI table at {table_path} has attrs: {attrs}")
-    valid = set(("type", "region", "instance_key")).issubset(attrs.keys())
-    if valid:
-        valid = valid and attrs["type"] == "ngff:region_table"
-        valid = valid and "path" in attrs["region"].keys()
-    if valid:
-        return True
-    else:
-        return False
+    return ROI_table
+
+
+def get_image_grid_ROIs(
+    array_shape: tuple[int, int, int],
+    pixels_ZYX: list[float],
+    grid_YX_shape: tuple[int, int],
+) -> ad.AnnData:
+    """
+    Produce a table with ROIS placed on a rectangular grid.
+
+    The main goal of this ROI grid is to allow processing of smaller subset of
+    the whole array.
+
+    In a specific case (that is, if the image array was obtained by stitching
+    together a set of FOVs placed on a regular grid), the ROIs correspond to
+    the original FOVs.
+
+    TODO: make this flexible with respect to the presence/absence of Z.
+
+    Args:
+        array_shape: ZYX shape of the image array.
+        pixels_ZYX: ZYX pixel sizes in micrometers.
+        grid_YX_shape:
+
+    Returns:
+        An `AnnData` table with a single ROI.
+    """
+    shape_z, shape_y, shape_x = array_shape[-3:]
+    grid_size_y, grid_size_x = grid_YX_shape[:]
+    X = []
+    obs_names = []
+    counter = 0
+    start_z = 0
+    len_z = shape_z
+
+    # Find minimal len_y that covers [0,shape_y] with grid_size_y intervals
+    len_y = math.ceil(shape_y / grid_size_y)
+    len_x = math.ceil(shape_x / grid_size_x)
+    for ind_y in range(grid_size_y):
+        start_y = ind_y * len_y
+        tmp_len_y = min(shape_y, start_y + len_y) - start_y
+        for ind_x in range(grid_size_x):
+            start_x = ind_x * len_x
+            tmp_len_x = min(shape_x, start_x + len_x) - start_x
+            X.append(
+                [
+                    start_x * pixels_ZYX[2],
+                    start_y * pixels_ZYX[1],
+                    start_z * pixels_ZYX[0],
+                    tmp_len_x * pixels_ZYX[2],
+                    tmp_len_y * pixels_ZYX[1],
+                    len_z * pixels_ZYX[0],
+                ]
+            )
+            counter += 1
+            obs_names.append(f"ROI_{counter}")
+    ROI_table = ad.AnnData(X=np.array(X, dtype=np.float32))
+    ROI_table.obs_names = obs_names
+    ROI_table.var_names = [
+        "x_micrometer",
+        "y_micrometer",
+        "z_micrometer",
+        "len_x_micrometer",
+        "len_y_micrometer",
+        "len_z_micrometer",
+    ]
+    return ROI_table
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/lib_upscale_array.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/upscale_array.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,68 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Function to increase the shape of an array by replicating it
+Function to increase the shape of an array by replicating it.
 """
 import logging
 import warnings
+from typing import Optional
 from typing import Sequence
-from typing import Tuple
 
 import numpy as np
 
 
 def upscale_array(
     *,
     array: np.ndarray,
-    target_shape: Tuple[int],
-    axis: Sequence[int] = None,
+    target_shape: tuple[int, ...],
+    axis: Optional[Sequence[int]] = None,
     pad_with_zeros: bool = False,
     warn_if_inhomogeneous: bool = False,
 ) -> np.ndarray:
     """
     Upscale an array along a given list of axis (through repeated application
-    of ``np.repeat``), to match a target shape.
+    of `np.repeat`), to match a target shape.
+
+    Args:
+        array: The array to be upscaled.
+        target_shape: The shape of the rescaled array.
+        axis: The axis along which to upscale the array (if `None`, then all
+            axis are used).
+        pad_with_zeros: If `True`, pad the upscaled array with zeros to match
+            `target_shape`.
+        warn_if_inhomogeneous: If `True`, raise a warning when the conversion
+            factors are not identical across all dimensions.
 
-    :param array: The array to be upscaled
-    :param target_shape: The shape of the rescaled array
-    :param axis: The axis along which to upscale the array (if ``None``, then \
-                 all axis are used)
-    :param pad_with_zeros: If ``True``, pad the upscaled array with zeros to
-                           match ``target_shape``.
-    :param warn_if_inhomogeneous: If ``True``, raise a warning when the
-                                  conversion factors are not identical across
-                                  all dimensions.
-    :returns: The upscaled array, with shape ``target_shape``.
+    Returns:
+        The upscaled array, with shape `target_shape`.
     """
 
     # Default behavior: use all axis
     if axis is None:
         axis = list(range(len(target_shape)))
 
     array_shape = array.shape
     info = (
         f"Trying to upscale from {array_shape=} to {target_shape=}, "
         f"acting on {axis=}."
     )
 
     if len(array_shape) != len(target_shape):
         raise ValueError(f"{info} Dimensions-number mismatch.")
+    if axis == []:
+        raise ValueError(f"{info} Empty axis list")
     if min(axis) < 0:
         raise ValueError(f"{info} Negative axis specification not allowed.")
 
     # Check that upscale is doable
     for ind, dim in enumerate(array_shape):
         # Check that array is not larger than target (downscaling)
         if dim > target_shape[ind]:
@@ -88,15 +90,15 @@
         if upscale_factors[ax] < 1:
             raise ValueError(info)
     info = f"{info} Upscale factors: {upscale_factors}"
 
     # Raise a warning if upscaling is non-homogeneous across all axis
     if warn_if_inhomogeneous:
         if len(set(upscale_factors.values())) > 1:
-            warnings.warn(info)
+            warnings.warn(f"{info} (inhomogeneous)")
 
     # Upscale array, via np.repeat
     upscaled_array = array
     for ax in axis:
         upscaled_array = np.repeat(
             upscaled_array, upscale_factors[ax], axis=ax
         )
@@ -126,28 +128,30 @@
             raise ValueError(f"{info} {upscaled_array.shape=}.")
 
     return upscaled_array
 
 
 def convert_region_to_low_res(
     *,
-    highres_region: Tuple[slice],
-    lowres_shape: Tuple[int],
-    highres_shape: Tuple[int],
-) -> Tuple[slice]:
+    highres_region: tuple[slice, ...],
+    lowres_shape: tuple[int, ...],
+    highres_shape: tuple[int, ...],
+) -> tuple[slice, ...]:
     """
     Convert a region defined for a high-resolution array to the corresponding
-    region for a low-resolution array
+    region for a low-resolution array.
+
+    Args:
+        highres_region: A region of the high-resolution array, defined in a
+            form like `(slice(0, 2), slice(1000, 2000), slice(1000, 2000))`.
+        highres_shape: The shape of the high-resolution array.
+        lowres_shape: The shape of the low-resolution array.
 
-    :param highres_region: A region of the high-resolution array, defined in a
-                           form like ``(slice(0, 2), slice(1000, 2000),
-                           slice(1000, 2000))``.
-    :param highres_shape: The shape of the high-resolution array.
-    :param lowres_shape: The shape of the low-resolution array.
-    :return: Region for low-resolution array.
+    Returns:
+        Region for low-resolution array.
     """
 
     error_msg = (
         f"Cannot convert {highres_region=}, "
         f"given {lowres_shape=} and {highres_shape=}."
     )
```

### Comparing `fractal_tasks_core-0.9.4/fractal_tasks_core/napari_workflows_wrapper.py` & `fractal_tasks_core-1.0.0a0/fractal_tasks_core/tasks/napari_workflows_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,138 +1,152 @@
+# Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
+# University of Zurich
+#
+# Original authors:
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Marco Franzon <marco.franzon@exact-lab.it>
+#
+# This file is part of Fractal and was originally developed by eXact lab S.r.l.
+# <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
+# Institute for Biomedical Research and Pelkmans Lab from the University of
+# Zurich.
 """
-Copyright 2022 (C)
-    Friedrich Miescher Institute for Biomedical Research and
-    University of Zurich
-
-    Original authors:
-    Tommaso Comparin <tommaso.comparin@exact-lab.it>
-    Marco Franzon <marco.franzon@exact-lab.it>
-
-    This file is part of Fractal and was originally developed by eXact lab
-    S.r.l.  <exact-lab.it> under contract with Liberali Lab from the Friedrich
-    Miescher Institute for Biomedical Research and Pelkmans Lab from the
-    University of Zurich.
-
-Wrapper of napari-workflows
+Wrapper of napari-workflows.
 """
-import json
 import logging
-from pathlib import Path
 from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Sequence
 
 import anndata as ad
 import dask.array as da
 import napari_workflows
 import numpy as np
 import pandas as pd
 import zarr
-from anndata.experimental import write_elem
 from napari_workflows._io_yaml_v1 import load_workflow
+from pydantic.decorator import validate_arguments
 
 import fractal_tasks_core
-from fractal_tasks_core.lib_channels import get_channel_from_image_zarr
-from fractal_tasks_core.lib_pyramid_creation import build_pyramid
-from fractal_tasks_core.lib_regions_of_interest import (
+from fractal_tasks_core.channels import get_channel_from_image_zarr
+from fractal_tasks_core.labels import prepare_label_group
+from fractal_tasks_core.ngff import load_NgffImageMeta
+from fractal_tasks_core.pyramids import build_pyramid
+from fractal_tasks_core.roi import check_valid_ROI_indices
+from fractal_tasks_core.roi import (
     convert_ROI_table_to_indices,
 )
-from fractal_tasks_core.lib_upscale_array import upscale_array
-from fractal_tasks_core.lib_zattrs_utils import extract_zyx_pixel_sizes
-from fractal_tasks_core.lib_zattrs_utils import rescale_datasets
+from fractal_tasks_core.roi import load_region
+from fractal_tasks_core.tables import write_table
+from fractal_tasks_core.tasks.io_models import (
+    NapariWorkflowsInput,
+)
+from fractal_tasks_core.tasks.io_models import (
+    NapariWorkflowsOutput,
+)
+from fractal_tasks_core.upscale_array import upscale_array
+from fractal_tasks_core.utils import rescale_datasets
 
 
 __OME_NGFF_VERSION__ = fractal_tasks_core.__OME_NGFF_VERSION__
 
 
 logger = logging.getLogger(__name__)
 
 
 class OutOfTaskScopeError(NotImplementedError):
     """
-    Encapsulates features that are out-of-scope for the current wrapper task
+    Encapsulates features that are out-of-scope for the current wrapper task.
     """
 
     pass
 
 
+@validate_arguments
 def napari_workflows_wrapper(
     *,
-    # Default arguments for fractal tasks:
-    input_paths: Sequence[str],
-    output_path: str,
-    component: str,
-    metadata: Dict[str, Any],
+    # Fractal argument
+    zarr_url: str,
     # Task-specific arguments:
     workflow_file: str,
-    input_specs: Dict[str, Dict[str, str]],
-    output_specs: Dict[str, Dict[str, str]],
+    input_specs: dict[str, NapariWorkflowsInput],
+    output_specs: dict[str, NapariWorkflowsOutput],
     input_ROI_table: str = "FOV_ROI_table",
     level: int = 0,
     relabeling: bool = True,
     expected_dimensions: int = 3,
+    overwrite: bool = True,
 ):
     """
-    Run a napari-workflow on the ROIs of a single OME-NGFF image
+    Run a napari-workflow on the ROIs of a single OME-NGFF image.
 
-    Full documentation for all arguments is still TBD, especially because some
-    of them are standard arguments for Fractal tasks that should be documented
-    in a standard way. Here are some examples::
-
-        input_paths = ["/some/path/"]
-        output_path = "/some/path/"
-        component = "some_plate.zarr/B/03/0"
-        metadata = {"num_levels": 4, "coarsening_xy": 2}
-
-        # Examples of allowed entries for input_specs and output_specs
-        input_specs = {
-            "in_1": {"type": "image", "wavelength_id": "A01_C02"},
-            "in_2": {"type": "image", "channel_label": "DAPI"},
-            "in_3": {"type": "label", "label_name": "label_DAPI"},
-        }
-        output_specs = {
-            "out_1": {"type": "label", "label_name": "label_DAPI_new"},
-            "out_2": {"type": "dataframe", "table_name": "measurements"},
-        }
-
-    :param input_paths: TBD (default arg for Fractal tasks)
-    :param output_path: TBD (default arg for Fractal tasks)
-    :param metadata: TBD (default arg for Fractal tasks)
-    :param component: TBD (default arg for Fractal tasks)
-    :param workflow_file: Absolute path to napari-workflows YAML file
-    :param input_specs: See examples above.
-    :param output_specs: See examples above.
-
-    :param level: Pyramid level of the image to be segmented.
-    :param expected_dimensions: Expected dimensions (either 2 or 3).
-
-    :param relabeling: If ``True``, apply relabeling so that label values are
-                       unique across ROIs.
-    :param input_ROI_table: name of the table that contains ROIs to which the\
-                            task applies the napari-worfklow
-    """
+    This task takes images and labels and runs a napari-workflow on them that
+    can produce a label and tables as output.
+
+    Examples of allowed entries for `input_specs` and `output_specs`:
 
+    ```
+    input_specs = {
+        "in_1": {"type": "image", "channel": {"wavelength_id": "A01_C02"}},
+        "in_2": {"type": "image", "channel": {"label": "DAPI"}},
+        "in_3": {"type": "label", "label_name": "label_DAPI"},
+    }
+
+    output_specs = {
+        "out_1": {"type": "label", "label_name": "label_DAPI_new"},
+        "out_2": {"type": "dataframe", "table_name": "measurements"},
+    }
+    ```
+
+    Args:
+        zarr_url: Path or url to the individual OME-Zarr image to be processed.
+            (standard argument for Fractal tasks, managed by Fractal server).
+        workflow_file: Absolute path to napari-workflows YAML file
+        input_specs: A dictionary of `NapariWorkflowsInput` values.
+        output_specs: A dictionary of `NapariWorkflowsOutput` values.
+        input_ROI_table: Name of the ROI table over which the task loops to
+            apply napari workflows.
+            Examples:
+            `FOV_ROI_table`
+            => loop over the field of views;
+            `organoid_ROI_table`
+            => loop over the organoid ROI table (generated by another task);
+            `well_ROI_table`
+            => process the whole well as one image.
+        level: Pyramid level of the image to be used as input for
+            napari-workflows. Choose `0` to process at full resolution.
+            Levels > 0 are currently only supported for workflows that only
+            have intensity images as input and only produce a label images as
+            output.
+        relabeling: If `True`, apply relabeling so that label values are
+            unique across all ROIs in the well.
+        expected_dimensions: Expected dimensions (either `2` or `3`). Useful
+            when loading 2D images that are stored in a 3D array with shape
+            `(1, size_x, size_y)` [which is the default way Fractal stores 2D
+            images], but you want to make sure the napari workflow gets a 2D
+            array to process. Also useful to set to `2` when loading a 2D
+            OME-Zarr that is saved as `(size_x, size_y)`.
+        overwrite: If `True`, overwrite the task output.
+    """
     wf: napari_workflows.Worfklow = load_workflow(workflow_file)
     logger.info(f"Loaded workflow from {workflow_file}")
 
     # Validation of input/output specs
     if not (set(wf.leafs()) <= set(output_specs.keys())):
         msg = f"Some item of {wf.leafs()=} is not part of {output_specs=}."
         logger.warning(msg)
     if not (set(wf.roots()) <= set(input_specs.keys())):
         msg = f"Some item of {wf.roots()=} is not part of {input_specs=}."
         logger.error(msg)
         raise ValueError(msg)
     list_outputs = sorted(output_specs.keys())
 
     # Characterization of workflow and scope restriction
-    input_types = [params["type"] for (name, params) in input_specs.items()]
-    output_types = [params["type"] for (name, params) in output_specs.items()]
+    input_types = [in_params.type for (name, in_params) in input_specs.items()]
+    output_types = [
+        out_params.type for (name, out_params) in output_specs.items()
+    ]
     are_inputs_all_images = set(input_types) == {"image"}
     are_outputs_all_labels = set(output_types) == {"label"}
     are_outputs_all_dataframes = set(output_types) == {"dataframe"}
     is_labeling_workflow = are_inputs_all_images and are_outputs_all_labels
     is_measurement_only_workflow = are_outputs_all_dataframes
     # Level-related constraint
     logger.info(f"This workflow acts at {level=}")
@@ -152,92 +166,72 @@
             "This is a measurement-output-only workflow, setting "
             "relabeling=False."
         )
         relabeling = False
     if relabeling:
         max_label_for_relabeling = 0
 
-    # Pre-processing of task inputs
-    if len(input_paths) > 1:
-        raise NotImplementedError("We currently only support a single in_path")
-    in_path = Path(input_paths[0]).as_posix()
-    num_levels = metadata["num_levels"]
-    coarsening_xy = metadata["coarsening_xy"]
     label_dtype = np.uint32
 
-    # Load zattrs file and multiscales
-    zattrs_file = f"{in_path}/{component}/.zattrs"
-    with open(zattrs_file, "r") as jsonfile:
-        zattrs = json.load(jsonfile)
-    multiscales = zattrs["multiscales"]
-    if len(multiscales) > 1:
-        raise NotImplementedError(
-            f"Found {len(multiscales)} multiscales, "
-            "but only one is currently supported."
-        )
-    if "coordinateTransformations" in multiscales[0].keys():
-        raise NotImplementedError(
-            "global coordinateTransformations at the multiscales "
-            "level are not currently supported"
-        )
-
     # Read ROI table
-    zarrurl = f"{in_path}/{component}"
-    ROI_table = ad.read_zarr(f"{in_path}/{component}/tables/{input_ROI_table}")
+    ROI_table = ad.read_zarr(f"{zarr_url}/tables/{input_ROI_table}")
+
+    # Load image metadata
+    ngff_image_meta = load_NgffImageMeta(zarr_url)
+    num_levels = ngff_image_meta.num_levels
+    coarsening_xy = ngff_image_meta.coarsening_xy
 
     # Read pixel sizes from zattrs file
-    full_res_pxl_sizes_zyx = extract_zyx_pixel_sizes(zattrs_file, level=0)
+    full_res_pxl_sizes_zyx = ngff_image_meta.get_pixel_sizes_zyx(level=0)
 
     # Create list of indices for 3D FOVs spanning the entire Z direction
     list_indices = convert_ROI_table_to_indices(
         ROI_table,
         level=level,
         coarsening_xy=coarsening_xy,
         full_res_pxl_sizes_zyx=full_res_pxl_sizes_zyx,
     )
+    check_valid_ROI_indices(list_indices, input_ROI_table)
     num_ROIs = len(list_indices)
     logger.info(
         f"Completed reading ROI table {input_ROI_table},"
         f" found {num_ROIs} ROIs."
     )
 
     # Input preparation: "image" type
     image_inputs = [
-        (name, params)
-        for (name, params) in input_specs.items()
-        if params["type"] == "image"
+        (name, in_params)
+        for (name, in_params) in input_specs.items()
+        if in_params.type == "image"
     ]
     input_image_arrays = {}
     if image_inputs:
-        img_array = da.from_zarr(f"{in_path}/{component}/{level}")
+        img_array = da.from_zarr(f"{zarr_url}/{level}")
         # Loop over image inputs and assign corresponding channel of the image
         for (name, params) in image_inputs:
-            if "wavelength_id" in params and "channel_label" in params:
-                raise ValueError(
-                    "One and only one among channel_label and wavelength_id"
-                    f" attributes must be provided, but input {name} in "
-                    f"input_specs has {params=}."
-                )
             channel = get_channel_from_image_zarr(
-                image_zarr_path=f"{in_path}/{component}",
-                wavelength_id=params.get("wavelength_id", None),
-                label=params.get("channel_label", None),
+                image_zarr_path=zarr_url,
+                wavelength_id=params.channel.wavelength_id,
+                label=params.channel.label,
             )
-            channel_index = channel["index"]
+            channel_index = channel.index
             input_image_arrays[name] = img_array[channel_index]
 
             # Handle dimensions
             shape = input_image_arrays[name].shape
             if expected_dimensions == 3 and shape[0] == 1:
                 logger.warning(
                     f"Input {name} has shape {shape} "
                     f"but {expected_dimensions=}"
                 )
             if expected_dimensions == 2:
-                if shape[0] == 1:
+                if len(shape) == 2:
+                    # We already load the data as a 2D array
+                    pass
+                elif shape[0] == 1:
                     input_image_arrays[name] = input_image_arrays[name][
                         0, :, :
                     ]
                 else:
                     msg = (
                         f"Input {name} has shape {shape} "
                         f"but {expected_dimensions=}"
@@ -245,17 +239,17 @@
                     logger.error(msg)
                     raise ValueError(msg)
             logger.info(f"Prepared input with {name=} and {params=}")
         logger.info(f"{input_image_arrays=}")
 
     # Input preparation: "label" type
     label_inputs = [
-        (name, params)
-        for (name, params) in input_specs.items()
-        if params["type"] == "label"
+        (name, in_params)
+        for (name, in_params) in input_specs.items()
+        if in_params.type == "label"
     ]
     if label_inputs:
         # Set target_shape for upscaling labels
         if not image_inputs:
             logger.warning(
                 f"{len(label_inputs)=} but num_image_inputs=0. "
                 "Label array(s) will not be upscaled."
@@ -263,53 +257,73 @@
             upscale_labels = False
         else:
             target_shape = list(input_image_arrays.values())[0].shape
             upscale_labels = True
         # Loop over label inputs and load corresponding (upscaled) image
         input_label_arrays = {}
         for (name, params) in label_inputs:
-            label_name = params["label_name"]
+            label_name = params.label_name
             label_array_raw = da.from_zarr(
-                f"{in_path}/{component}/labels/{label_name}/{level}"
+                f"{zarr_url}/labels/{label_name}/{level}"
             )
             input_label_arrays[name] = label_array_raw
-            if upscale_labels:
-                input_label_arrays[name] = upscale_array(
-                    array=input_label_arrays[name],
-                    target_shape=target_shape,
-                    axis=[1, 2],
-                    pad_with_zeros=True,
-                )
+
             # Handle dimensions
             shape = input_label_arrays[name].shape
             if expected_dimensions == 3 and shape[0] == 1:
                 logger.warning(
                     f"Input {name} has shape {shape} "
                     f"but {expected_dimensions=}"
                 )
             if expected_dimensions == 2:
-                if shape[0] == 1:
+                if len(shape) == 2:
+                    # We already load the data as a 2D array
+                    pass
+                elif shape[0] == 1:
                     input_label_arrays[name] = input_label_arrays[name][
                         0, :, :
                     ]
                 else:
                     msg = (
                         f"Input {name} has shape {shape} "
                         f"but {expected_dimensions=}"
                     )
                     logger.error(msg)
                     raise ValueError(msg)
+
+            if upscale_labels:
+                # Check that dimensionality matches the image
+                if len(input_label_arrays[name].shape) != len(target_shape):
+                    raise ValueError(
+                        f"Label {name} has shape "
+                        f"{input_label_arrays[name].shape}. "
+                        "But the corresponding image has shape "
+                        f"{target_shape}. Those dimensionalities do not "
+                        f"match. Is {expected_dimensions=} the correct "
+                        "setting?"
+                    )
+                if expected_dimensions == 3:
+                    upscaling_axes = [1, 2]
+                else:
+                    upscaling_axes = [0, 1]
+                input_label_arrays[name] = upscale_array(
+                    array=input_label_arrays[name],
+                    target_shape=target_shape,
+                    axis=upscaling_axes,
+                    pad_with_zeros=True,
+                )
+
             logger.info(f"Prepared input with {name=} and {params=}")
         logger.info(f"{input_label_arrays=}")
 
     # Output preparation: "label" type
     label_outputs = [
-        (name, params)
-        for (name, params) in output_specs.items()
-        if params["type"] == "label"
+        (name, out_params)
+        for (name, out_params) in output_specs.items()
+        if out_params.type == "label"
     ]
     if label_outputs:
         # Preliminary scope checks
         if len(label_outputs) > 1:
             raise OutOfTaskScopeError(
                 "Multiple label outputs would break label-inputs-only "
                 f"workflows (found {len(label_outputs)=})."
@@ -327,29 +341,29 @@
         #    re-load the pixel sizes and re-build ROI indices, and (B) use the
         #    first input label to determine output-label array properties
         if image_inputs:
             reference_array = list(input_image_arrays.values())[0]
         elif label_inputs:
             reference_array = list(input_label_arrays.values())[0]
             # Re-load pixel size, matching to the correct level
-            input_label_name = label_inputs[0][1]["label_name"]
-            zattrs_file = (
-                f"{in_path}/{component}/labels/{input_label_name}/.zattrs"
-            )
-            # Read pixel sizes from zattrs file
-            full_res_pxl_sizes_zyx = extract_zyx_pixel_sizes(
-                zattrs_file, level=0
+            input_label_name = label_inputs[0][1].label_name
+            ngff_label_image_meta = load_NgffImageMeta(
+                f"{zarr_url}/labels/{input_label_name}"
+            )
+            full_res_pxl_sizes_zyx = ngff_label_image_meta.get_pixel_sizes_zyx(
+                level=0
             )
             # Create list of indices for 3D FOVs spanning the whole Z direction
             list_indices = convert_ROI_table_to_indices(
                 ROI_table,
                 level=level,
                 coarsening_xy=coarsening_xy,
                 full_res_pxl_sizes_zyx=full_res_pxl_sizes_zyx,
             )
+            check_valid_ROI_indices(list_indices, input_ROI_table)
             num_ROIs = len(list_indices)
             logger.info(
                 f"Re-create ROI indices from ROI table {input_ROI_table}, "
                 f"using {full_res_pxl_sizes_zyx=}. "
                 "This is necessary because label-input-only workflows may "
                 "have label inputs that are at a different resolution and "
                 "are not upscaled."
@@ -372,87 +386,93 @@
                     f"{expected_dimensions=}"
                 )
             label_shape = (1, label_shape[0], label_shape[1])
             label_chunksize = (1, label_chunksize[0], label_chunksize[1])
         logger.info(f"{label_shape=}")
         logger.info(f"{label_chunksize=}")
 
-        # Create labels zarr group and combine existing/new labels in .zattrs
-        new_labels = [params["label_name"] for (name, params) in label_outputs]
-        zarrurl = f"{in_path}/{component}"
-        try:
-            with open(f"{zarrurl}/labels/.zattrs", "r") as f_zattrs:
-                existing_labels = json.load(f_zattrs)["labels"]
-        except FileNotFoundError:
-            existing_labels = []
-        intersection = set(new_labels) & set(existing_labels)
-        logger.info(f"{new_labels=}")
-        logger.info(f"{existing_labels=}")
-        if intersection:
-            raise OutOfTaskScopeError(
-                f"Labels {intersection} already exist "
-                "but are part of outputs"
-            )
-        labels_group = zarr.group(f"{zarrurl}/labels")
-        labels_group.attrs["labels"] = existing_labels + new_labels
-
         # Loop over label outputs and (1) set zattrs, (2) create zarr group
-        output_label_zarr_groups: Dict[str, Any] = {}
-        for (name, params) in label_outputs:
-            label_name = params["label_name"]
+        output_label_zarr_groups: dict[str, Any] = {}
+        for (name, out_params) in label_outputs:
 
             # (1a) Rescale OME-NGFF datasets (relevant for level>0)
+            if not ngff_image_meta.multiscale.axes[0].name == "c":
+                raise ValueError(
+                    "Cannot set `remove_channel_axis=True` for multiscale "
+                    f"metadata with axes={ngff_image_meta.multiscale.axes}. "
+                    'First axis should have name "c".'
+                )
             new_datasets = rescale_datasets(
-                datasets=multiscales[0]["datasets"],
+                datasets=[
+                    ds.dict() for ds in ngff_image_meta.multiscale.datasets
+                ],
                 coarsening_xy=coarsening_xy,
                 reference_level=level,
+                remove_channel_axis=True,
             )
-            # (1b) Write zattrs for specific label
-            label_group = labels_group.create_group(label_name)
-            label_group.attrs["image-label"] = {
-                "version": __OME_NGFF_VERSION__
-            }
-            label_group.attrs["multiscales"] = [
-                {
-                    "name": label_name,
+
+            # (1b) Prepare attrs for label group
+            label_name = out_params.label_name
+            label_attrs = {
+                "image-label": {
                     "version": __OME_NGFF_VERSION__,
-                    "axes": [
-                        ax
-                        for ax in multiscales[0]["axes"]
-                        if ax["type"] != "channel"
-                    ],
-                    "datasets": new_datasets,
-                }
-            ]
-            # (2) Create zarr group at level=0
-            store = zarr.storage.FSStore(
-                f"{in_path}/{component}/labels/{label_name}/0"
+                    "source": {"image": "../../"},
+                },
+                "multiscales": [
+                    {
+                        "name": label_name,
+                        "version": __OME_NGFF_VERSION__,
+                        "axes": [
+                            ax.dict()
+                            for ax in ngff_image_meta.multiscale.axes
+                            if ax.type != "channel"
+                        ],
+                        "datasets": new_datasets,
+                    }
+                ],
+            }
+
+            # (2) Prepare label group
+            image_group = zarr.group(zarr_url)
+            label_group = prepare_label_group(
+                image_group,
+                label_name,
+                overwrite=overwrite,
+                label_attrs=label_attrs,
+                logger=logger,
+            )
+            logger.info(
+                "Helper function `prepare_label_group` returned "
+                f"{label_group=}"
             )
+
+            # (3) Create zarr group at level=0
+            store = zarr.storage.FSStore(f"{zarr_url}/labels/{label_name}/0")
             mask_zarr = zarr.create(
                 shape=label_shape,
                 chunks=label_chunksize,
                 dtype=label_dtype,
                 store=store,
-                overwrite=False,
+                overwrite=overwrite,
                 dimension_separator="/",
             )
             output_label_zarr_groups[name] = mask_zarr
-            logger.info(f"Prepared output with {name=} and {params=}")
+            logger.info(f"Prepared output with {name=} and {out_params=}")
         logger.info(f"{output_label_zarr_groups=}")
 
     # Output preparation: "dataframe" type
     dataframe_outputs = [
-        (name, params)
-        for (name, params) in output_specs.items()
-        if params["type"] == "dataframe"
+        (name, out_params)
+        for (name, out_params) in output_specs.items()
+        if out_params.type == "dataframe"
     ]
-    output_dataframe_lists: Dict[str, List] = {}
-    for (name, params) in dataframe_outputs:
+    output_dataframe_lists: dict[str, list] = {}
+    for (name, out_params) in dataframe_outputs:
         output_dataframe_lists[name] = []
-        logger.info(f"Prepared output with {name=} and {params=}")
+        logger.info(f"Prepared output with {name=} and {out_params=}")
         logger.info(f"{output_dataframe_lists=}")
 
     #####
 
     for i_ROI, indices in enumerate(list_indices):
         s_z, e_z, s_y, e_y, s_x, e_x = indices[:]
         region = (slice(s_z, e_z), slice(s_y, e_y), slice(s_x, e_x))
@@ -460,39 +480,44 @@
         logger.info(f"ROI {i_ROI+1}/{num_ROIs}: {region=}")
 
         # Always re-load napari worfklow
         wf = load_workflow(workflow_file)
 
         # Set inputs
         for input_name in input_specs.keys():
-            input_type = input_specs[input_name]["type"]
-            # Handle expected_dimensions
-            if expected_dimensions == 2:
-                actual_region = region[1:]
-            else:
-                actual_region = region
+            input_type = input_specs[input_name].type
 
             if input_type == "image":
                 wf.set(
                     input_name,
-                    input_image_arrays[input_name][actual_region].compute(),
+                    load_region(
+                        input_image_arrays[input_name],
+                        region,
+                        compute=True,
+                        return_as_3D=False,
+                    ),
                 )
             elif input_type == "label":
                 wf.set(
                     input_name,
-                    input_label_arrays[input_name][actual_region],
+                    load_region(
+                        input_label_arrays[input_name],
+                        region,
+                        compute=True,
+                        return_as_3D=False,
+                    ),
                 )
 
         # Get outputs
         outputs = wf.get(list_outputs)
 
         # Iterate first over dataframe outputs (to use the correct
         # max_label_for_relabeling, if needed)
         for ind_output, output_name in enumerate(list_outputs):
-            if output_specs[output_name]["type"] != "dataframe":
+            if output_specs[output_name].type != "dataframe":
                 continue
             df = outputs[ind_output]
             if relabeling:
                 df["label"] += max_label_for_relabeling
                 logger.info(
                     f'ROI {i_ROI+1}/{num_ROIs}: Relabeling "{name}" dataframe'
                     "output, with {max_label_for_relabeling=}"
@@ -500,15 +525,15 @@
 
             # Append the new-ROI dataframe to the all-ROIs list
             output_dataframe_lists[output_name].append(df)
 
         # After all dataframe outputs, iterate over label outputs (which
         # actually can be only 0 or 1)
         for ind_output, output_name in enumerate(list_outputs):
-            if output_specs[output_name]["type"] != "label":
+            if output_specs[output_name].type != "label":
                 continue
             mask = outputs[ind_output]
 
             # Check dimensions
             if len(mask.shape) != expected_dimensions:
                 msg = (
                     f"Output {output_name} has shape {mask.shape} "
@@ -545,21 +570,22 @@
                     f"new {max_label_for_relabeling=}"
                 )
 
             da.array(mask).to_zarr(
                 url=output_label_zarr_groups[output_name],
                 region=region,
                 compute=True,
+                overwrite=overwrite,
             )
         logger.info(f"ROI {i_ROI+1}/{num_ROIs}: output handling complete")
 
     # Output handling: "dataframe" type (for each output, concatenate ROI
     # dataframes, clean up, and store in a AnnData table on-disk)
-    for (name, params) in dataframe_outputs:
-        table_name = params["table_name"]
+    for (name, out_params) in dataframe_outputs:
+        table_name = out_params.table_name
         # Concatenate all FOV dataframes
         list_dfs = output_dataframe_lists[name]
         if len(list_dfs) == 0:
             measurement_table = ad.AnnData()
         else:
             df_well = pd.concat(list_dfs, axis=0, ignore_index=True)
             # Extract labels and drop them from df_well
@@ -568,61 +594,44 @@
             # Convert all to float (warning: some would be int, in principle)
             measurement_dtype = np.float32
             df_well = df_well.astype(measurement_dtype)
             df_well.index = df_well.index.map(str)
             # Convert to anndata
             measurement_table = ad.AnnData(df_well, dtype=measurement_dtype)
             measurement_table.obs = labels
+
         # Write to zarr group
-        group_tables = zarr.group(f"{in_path}/{component}/tables/")
-        write_elem(group_tables, table_name, measurement_table)
-        # Update OME-NGFF metadata
-        current_tables = group_tables.attrs.asdict().get("tables") or []
-        if table_name in current_tables:
-            # FIXME: move this check to an earlier stage of the task
-            raise ValueError(
-                f"{in_path}/{component}/tables/ already includes "
-                f"{table_name=} in {current_tables=}"
-            )
-        new_tables = current_tables + [table_name]
-        group_tables.attrs["tables"] = new_tables
-        # FIXME: also include table metadata, see issue #333
+        image_group = zarr.group(zarr_url)
+        table_attrs = dict(
+            type="feature_table",
+            region=dict(path=f"../labels/{out_params.label_name}"),
+            instance_key="label",
+        )
+        write_table(
+            image_group,
+            table_name,
+            measurement_table,
+            overwrite=overwrite,
+            table_attrs=table_attrs,
+        )
 
     # Output handling: "label" type (for each output, build and write to disk
     # pyramid of coarser levels)
-    for (name, params) in label_outputs:
-        label_name = params["label_name"]
+    for (name, out_params) in label_outputs:
+        label_name = out_params.label_name
         build_pyramid(
-            zarrurl=f"{zarrurl}/labels/{label_name}",
-            overwrite=False,
+            zarrurl=f"{zarr_url}/labels/{label_name}",
+            overwrite=overwrite,
             num_levels=num_levels,
             coarsening_xy=coarsening_xy,
             chunksize=label_chunksize,
             aggregation_function=np.max,
         )
 
-    return {}
-
 
 if __name__ == "__main__":
-    from pydantic import BaseModel
-    from pydantic import Extra
-    from fractal_tasks_core._utils import run_fractal_task
-
-    class TaskArguments(BaseModel, extra=Extra.forbid):
-        input_paths: Sequence[str]
-        output_path: str
-        metadata: Dict[str, Any]
-        component: str
-        workflow_file: str
-        input_specs: Dict[str, Dict[str, str]]
-        output_specs: Dict[str, Dict[str, str]]
-        input_ROI_table: Optional[str]
-        level: Optional[int]
-        relabeling: Optional[bool]
-        expected_dimensions: Optional[int]
+    from fractal_tasks_core.tasks._utils import run_fractal_task
 
     run_fractal_task(
         task_function=napari_workflows_wrapper,
-        TaskArgsModel=TaskArguments,
         logger_name=logger.name,
     )
```

### Comparing `fractal_tasks_core-0.9.4/PKG-INFO` & `fractal_tasks_core-1.0.0a0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 Metadata-Version: 2.1
 Name: fractal-tasks-core
-Version: 0.9.4
-Summary: 
+Version: 1.0.0a0
+Summary: Core bioimage-analysis library and tasks of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-tasks-core
 License: BSD-3-Clause
-Author: Jacopo Nespolo
-Author-email: jacopo.nespolo@exact-lab.it
+Author: Joel Lüthi 
+Author-email: joel.luethi@fmi.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: tools
-Requires-Dist: Pillow (>=9.1.1,<10.0.0)
-Requires-Dist: anndata (>=0.8.0,<0.9.0)
-Requires-Dist: cellpose (>=2.2,<2.3)
-Requires-Dist: dask (>=2023.1.0,<2023.2.0)
+Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: fractal-tasks
+Requires-Dist: Pillow (>=9.1.1) ; extra == "fractal-tasks"
+Requires-Dist: anndata (>=0.8.0,<0.11.0)
+Requires-Dist: cellpose (>=2.2,<2.3) ; extra == "fractal-tasks"
+Requires-Dist: dask (>=2023.1.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: imageio-ffmpeg (>=0.4.7,<0.5.0)
-Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
+Requires-Dist: docstring-parser (>=0.15,<0.16)
+Requires-Dist: fsspec (!=2023.9.0)
+Requires-Dist: imageio-ffmpeg (>=0.4.7,<0.5.0) ; extra == "fractal-tasks"
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: matplotlib ; extra == "tools"
-Requires-Dist: napari-segment-blobs-and-things-with-membranes (>=0.3.3,<0.4.0)
-Requires-Dist: napari-skimage-regionprops (>=0.8.1,<0.9.0)
-Requires-Dist: napari-tools-menu (>=0.1.19,<0.2.0)
-Requires-Dist: napari-workflows (>=0.2.8,<0.3.0)
-Requires-Dist: numpy (>=1.23.5,<1.24.0)
-Requires-Dist: pandas (>=1.2.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: scikit-image (>=0.19)
-Requires-Dist: torch (==1.12.1)
-Requires-Dist: zarr (>=2.13.6,<2.14.0)
-Project-URL: Documentation, https://fractal-tasks-core.readthedocs.io
+Requires-Dist: napari-segment-blobs-and-things-with-membranes (>=0.3.3,<0.4.0) ; extra == "fractal-tasks"
+Requires-Dist: napari-skimage-regionprops (>=0.8.1,<0.9.0) ; extra == "fractal-tasks"
+Requires-Dist: napari-tools-menu (>=0.1.19,<0.2.0) ; extra == "fractal-tasks"
+Requires-Dist: napari-workflows (>=0.2.8,<0.3.0) ; extra == "fractal-tasks"
+Requires-Dist: numpy (<2)
+Requires-Dist: pandas (>=1.2.0,<2)
+Requires-Dist: pydantic (<2)
+Requires-Dist: scikit-image (>=0.19) ; extra == "fractal-tasks"
+Requires-Dist: torch (<=2.0.0) ; extra == "fractal-tasks"
+Requires-Dist: zarr (>=2.13.6,<3)
+Project-URL: Changelog, https://github.com/fractal-analytics-platform/fractal-tasks-core/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://fractal-analytics-platform.github.io/fractal-tasks-core
+Project-URL: Repository, https://github.com/fractal-analytics-platform/fractal-tasks-core
 Description-Content-Type: text/markdown
 
 # Fractal Core Tasks
 
 [![PyPI version](https://img.shields.io/pypi/v/fractal-tasks-core?color=gree)](https://pypi.org/project/fractal-tasks-core/)
-[![CI Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci.yml)
+[![CI Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci_pip.yml/badge.svg)](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/ci_pip.yml)
 [![Coverage](https://raw.githubusercontent.com/fractal-analytics-platform/fractal-tasks-core/python-coverage-comment-action-data/badge.svg)](https://htmlpreview.github.io/?https://github.com/fractal-analytics-platform/fractal-tasks-core/blob/python-coverage-comment-action-data/htmlcov/index.html)
 [![Documentation Status](https://github.com/fractal-analytics-platform/fractal-tasks-core/actions/workflows/documentation.yaml/badge.svg)](https://fractal-analytics-platform.github.io/fractal-tasks-core)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 Fractal is a framework to process high-content imaging data at scale and prepare it for interactive visualization.
 
 ![Fractal_Overview](https://fractal-analytics-platform.github.io/assets/fractal_overview.jpg)
@@ -68,9 +71,9 @@
 
 Some additional tasks are currently being worked on and some older tasks are still present in the fractal_tasks_core folder.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa) & [@jacopo-exact](https://github.com/jacopo-exact) from [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich by [@jluethi](https://github.com/jluethi) and [@gusqgm](https://github.com/gusqgm). The Fractal project is now developed at the [BioVisionCenter](https://www.biovisioncenter.uzh.ch/en.html) at the University of Zurich and the project lead is with [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](https://www.exact-lab.it/).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

