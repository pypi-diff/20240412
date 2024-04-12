# Comparing `tmp/blackdynamite-1.0.5.tar.gz` & `tmp/blackdynamite-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackdynamite-1.0.5.tar", max compression
+gzip compressed data, was "blackdynamite-1.0.6.tar", max compression
```

## Comparing `blackdynamite-1.0.5.tar` & `blackdynamite-1.0.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0     6239 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/BDstat.py
--rw-r--r--   0        0        0     1917 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/__init__.py
--rwxr-xr-x   0        0        0     7541 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/base.py
--rw-r--r--   0        0        0    23960 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/base_zeo.py
--rw-r--r--   0        0        0     2272 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/bd_constraints.py
--rw-r--r--   0        0        0     2983 2023-03-07 17:01:30.782494 blackdynamite-1.0.5/BlackDynamite/bdlogging.py
--rwxr-xr-x   0        0        0    16147 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/bdparser.py
--rw-r--r--   0        0        0      781 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/coating/__init__.py
--rwxr-xr-x   0        0        0     2995 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/coating/bashCoat.py
--rwxr-xr-x   0        0        0     3998 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/coating/pbsCoat.py
--rwxr-xr-x   0        0        0     3330 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/coating/sgeCoat.py
--rwxr-xr-x   0        0        0     4450 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/coating/slurmCoat.py
--rwxr-xr-x   0        0        0     2388 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/conffile_zeo.py
--rw-r--r--   0        0        0     8943 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/constraints_zeo.py
--rwxr-xr-x   0        0        0    13219 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/graphhelper.py
--rwxr-xr-x   0        0        0     1502 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/job.py
--rwxr-xr-x   0        0        0     1562 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/jobselector.py
--rw-r--r--   0        0        0     1909 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/loader.py
--rw-r--r--   0        0        0     4010 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/lowercase_btree.py
--rw-r--r--   0        0        0     3451 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/runLM.py
--rwxr-xr-x   0        0        0    14819 2023-03-07 17:01:30.783495 blackdynamite-1.0.5/BlackDynamite/run_zeo.py
--rwxr-xr-x   0        0        0     1855 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/runselector.py
--rw-r--r--   0        0        0      736 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/__init__.py
--rw-r--r--   0        0        0      572 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/bash_completion.sh
--rwxr-xr-x   0        0        0      706 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/bd_zeo_server.py
--rwxr-xr-x   0        0        0     8370 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/canYouDigIt.py
--rwxr-xr-x   0        0        0     5550 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/cleanRuns.py
--rw-r--r--   0        0        0     1073 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/createDB.py
--rw-r--r--   0        0        0     2941 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/createJobs.py
--rwxr-xr-x   0        0        0     2466 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/createRuns.py
--rwxr-xr-x   0        0        0     3306 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/createUser.py
--rwxr-xr-x   0        0        0     3708 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/enterRun.py
--rw-r--r--   0        0        0     2201 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/fix_zeodb.py
--rw-r--r--   0        0        0     3886 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/getJobInfo.py
--rwxr-xr-x   0        0        0     8249 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/getRunInfo.py
--rwxr-xr-x   0        0        0     2788 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/launchRuns.py
--rwxr-xr-x   0        0        0     3032 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/mvRuns.py
--rwxr-xr-x   0        0        0     2404 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/open_zeodb.py
--rwxr-xr-x   0        0        0     1309 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/plotRuns.py
--rwxr-xr-x   0        0        0     2738 2023-03-07 17:01:30.784494 blackdynamite-1.0.5/BlackDynamite/scripts/pushQuantity.py
--rwxr-xr-x   0        0        0     2676 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/scripts/saveBDStudy.py
--rw-r--r--   0        0        0     8821 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/scripts/streamlitInfo.py
--rwxr-xr-x   0        0        0     3438 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/scripts/studyInfo.py
--rwxr-xr-x   0        0        0     2417 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/scripts/updateRuns.py
--rw-r--r--   0        0        0     1229 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/selector.py
--rw-r--r--   0        0        0     7586 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/BlackDynamite/zeoobject.py
--rw-r--r--   0        0        0    12873 2023-03-07 17:01:30.785495 blackdynamite-1.0.5/README.md
--rw-r--r--   0        0        0     1142 2023-03-07 17:01:40.732381 blackdynamite-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    14125 1970-01-01 00:00:00.000000 blackdynamite-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6239 2024-04-12 19:51:37.743664 blackdynamite-1.0.6/BlackDynamite/BDstat.py
+-rw-r--r--   0        0        0     1917 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/__init__.py
+-rwxr-xr-x   0        0        0     7541 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/base.py
+-rw-r--r--   0        0        0    23960 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/base_zeo.py
+-rw-r--r--   0        0        0     2272 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bd_constraints.py
+-rw-r--r--   0        0        0     2943 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bdlogging.py
+-rwxr-xr-x   0        0        0    16147 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bdparser.py
+-rw-r--r--   0        0        0      781 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/__init__.py
+-rwxr-xr-x   0        0        0     2995 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/bashCoat.py
+-rwxr-xr-x   0        0        0     3998 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/pbsCoat.py
+-rwxr-xr-x   0        0        0     3330 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/sgeCoat.py
+-rwxr-xr-x   0        0        0     3410 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/slurmCoat.py
+-rwxr-xr-x   0        0        0     2388 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/conffile_zeo.py
+-rw-r--r--   0        0        0     8943 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/constraints_zeo.py
+-rwxr-xr-x   0        0        0    13219 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/graphhelper.py
+-rwxr-xr-x   0        0        0     1502 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/job.py
+-rwxr-xr-x   0        0        0     1562 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/jobselector.py
+-rw-r--r--   0        0        0     1909 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/loader.py
+-rw-r--r--   0        0        0     4010 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/lowercase_btree.py
+-rw-r--r--   0        0        0     3451 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/runLM.py
+-rwxr-xr-x   0        0        0    14819 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/run_zeo.py
+-rwxr-xr-x   0        0        0     1855 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/runselector.py
+-rw-r--r--   0        0        0      736 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/bash_completion.sh
+-rwxr-xr-x   0        0        0      706 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/bd_zeo_server.py
+-rwxr-xr-x   0        0        0     8370 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/canYouDigIt.py
+-rwxr-xr-x   0        0        0     5550 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/cleanRuns.py
+-rw-r--r--   0        0        0     1073 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createDB.py
+-rw-r--r--   0        0        0     2941 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createJobs.py
+-rwxr-xr-x   0        0        0     2466 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createRuns.py
+-rwxr-xr-x   0        0        0     3306 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createUser.py
+-rwxr-xr-x   0        0        0     3708 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/enterRun.py
+-rw-r--r--   0        0        0     2201 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/fix_zeodb.py
+-rw-r--r--   0        0        0     3886 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/getJobInfo.py
+-rwxr-xr-x   0        0        0     8249 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/getRunInfo.py
+-rwxr-xr-x   0        0        0     2788 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/launchRuns.py
+-rwxr-xr-x   0        0        0     3032 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/mvRuns.py
+-rwxr-xr-x   0        0        0     2404 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/open_zeodb.py
+-rwxr-xr-x   0        0        0     1309 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/plotRuns.py
+-rwxr-xr-x   0        0        0     2738 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/pushQuantity.py
+-rwxr-xr-x   0        0        0     2676 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/saveBDStudy.py
+-rw-r--r--   0        0        0     8821 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/streamlitInfo.py
+-rwxr-xr-x   0        0        0     3438 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/studyInfo.py
+-rwxr-xr-x   0        0        0     2417 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/updateRuns.py
+-rw-r--r--   0        0        0     1229 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/selector.py
+-rw-r--r--   0        0        0     7586 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/zeoobject.py
+-rw-r--r--   0        0        0    35149 2024-04-12 19:51:37.747664 blackdynamite-1.0.6/COPYING.txt
+-rw-r--r--   0        0        0    12873 2024-04-12 19:51:37.747664 blackdynamite-1.0.6/README.md
+-rw-r--r--   0        0        0     1142 2024-04-12 19:51:43.361613 blackdynamite-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 blackdynamite-1.0.6/PKG-INFO
```

### Comparing `blackdynamite-1.0.5/BlackDynamite/BDstat.py` & `blackdynamite-1.0.6/BlackDynamite/BDstat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/__init__.py` & `blackdynamite-1.0.6/BlackDynamite/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/base.py` & `blackdynamite-1.0.6/BlackDynamite/base.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/base_zeo.py` & `blackdynamite-1.0.6/BlackDynamite/base_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/bd_constraints.py` & `blackdynamite-1.0.6/BlackDynamite/bd_constraints.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/bdlogging.py` & `blackdynamite-1.0.6/BlackDynamite/bdlogging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 # This program is free software: you can redistribute it and/or modify
 #     it under the terms of the GNU General Public License as published by
 #     the Free Software Foundation, either version 3 of the License, or
 #     (at your option) any later version.
 #
 #     This program is distributed in the hope that it will be useful,
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-from __future__ import print_function
-
 import logging
 import traceback
 import os
 import sys
 
 from . import __name__ as global_name
```

### Comparing `blackdynamite-1.0.5/BlackDynamite/bdparser.py` & `blackdynamite-1.0.6/BlackDynamite/bdparser.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/coating/__init__.py` & `blackdynamite-1.0.6/BlackDynamite/coating/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/coating/bashCoat.py` & `blackdynamite-1.0.6/BlackDynamite/coating/bashCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/coating/pbsCoat.py` & `blackdynamite-1.0.6/BlackDynamite/coating/pbsCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/coating/sgeCoat.py` & `blackdynamite-1.0.6/BlackDynamite/coating/sgeCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/conffile_zeo.py` & `blackdynamite-1.0.6/BlackDynamite/conffile_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/constraints_zeo.py` & `blackdynamite-1.0.6/BlackDynamite/constraints_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/graphhelper.py` & `blackdynamite-1.0.6/BlackDynamite/graphhelper.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/job.py` & `blackdynamite-1.0.6/BlackDynamite/job.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/jobselector.py` & `blackdynamite-1.0.6/BlackDynamite/jobselector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/loader.py` & `blackdynamite-1.0.6/BlackDynamite/loader.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/lowercase_btree.py` & `blackdynamite-1.0.6/BlackDynamite/lowercase_btree.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/runLM.py` & `blackdynamite-1.0.6/BlackDynamite/runLM.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/run_zeo.py` & `blackdynamite-1.0.6/BlackDynamite/run_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/runselector.py` & `blackdynamite-1.0.6/BlackDynamite/runselector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/__init__.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/bash_completion.sh` & `blackdynamite-1.0.6/BlackDynamite/scripts/bash_completion.sh`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/bd_zeo_server.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/bd_zeo_server.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/canYouDigIt.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/canYouDigIt.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/cleanRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/cleanRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/createDB.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/createDB.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/createJobs.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/createJobs.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/createRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/createRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/createUser.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/createUser.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/enterRun.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/enterRun.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/fix_zeodb.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/fix_zeodb.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/getJobInfo.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/getJobInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/getRunInfo.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/getRunInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/launchRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/launchRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/mvRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/mvRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/open_zeodb.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/open_zeodb.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/plotRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/plotRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/pushQuantity.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/pushQuantity.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/saveBDStudy.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/saveBDStudy.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/streamlitInfo.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/streamlitInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/studyInfo.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/studyInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/scripts/updateRuns.py` & `blackdynamite-1.0.6/BlackDynamite/scripts/updateRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/selector.py` & `blackdynamite-1.0.6/BlackDynamite/selector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/BlackDynamite/zeoobject.py` & `blackdynamite-1.0.6/BlackDynamite/zeoobject.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/README.md` & `blackdynamite-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.5/pyproject.toml` & `blackdynamite-1.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackdynamite"
-version = "1.0.5"
+version = "1.0.6"
 description = "Scientific Parametric Study Tool"
 authors = ["Guillaume Anciaux <guillaume.anciaux@epfl.ch>"]
 license = "GPL"
 readme = "README.md"
 packages = [{include = "BlackDynamite"}]
 homepage = "https://gitlab.com/ganciaux/blackdynamite"
 repository = "https://gitlab.com/ganciaux/blackdynamite"
```

### Comparing `blackdynamite-1.0.5/PKG-INFO` & `blackdynamite-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: blackdynamite
-Version: 1.0.5
+Version: 1.0.6
 Summary: Scientific Parametric Study Tool
 Home-page: https://gitlab.com/ganciaux/blackdynamite
 License: GPL
 Author: Guillaume Anciaux
 Author-email: guillaume.anciaux@epfl.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argcomplete (>=2.0.0)
 Requires-Dist: ipython (>=8.11.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.6.3,<4.0.0)
 Requires-Dist: numpy (>=1.24.1)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
```

