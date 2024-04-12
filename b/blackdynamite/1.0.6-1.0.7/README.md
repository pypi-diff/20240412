# Comparing `tmp/blackdynamite-1.0.6.tar.gz` & `tmp/blackdynamite-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackdynamite-1.0.6.tar", max compression
+gzip compressed data, was "blackdynamite-1.0.7.tar", max compression
```

## Comparing `blackdynamite-1.0.6.tar` & `blackdynamite-1.0.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     6239 2024-04-12 19:51:37.743664 blackdynamite-1.0.6/BlackDynamite/BDstat.py
--rw-r--r--   0        0        0     1917 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/__init__.py
--rwxr-xr-x   0        0        0     7541 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/base.py
--rw-r--r--   0        0        0    23960 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/base_zeo.py
--rw-r--r--   0        0        0     2272 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bd_constraints.py
--rw-r--r--   0        0        0     2943 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bdlogging.py
--rwxr-xr-x   0        0        0    16147 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/bdparser.py
--rw-r--r--   0        0        0      781 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/__init__.py
--rwxr-xr-x   0        0        0     2995 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/bashCoat.py
--rwxr-xr-x   0        0        0     3998 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/pbsCoat.py
--rwxr-xr-x   0        0        0     3330 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/sgeCoat.py
--rwxr-xr-x   0        0        0     3410 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/coating/slurmCoat.py
--rwxr-xr-x   0        0        0     2388 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/conffile_zeo.py
--rw-r--r--   0        0        0     8943 2024-04-12 19:51:37.744664 blackdynamite-1.0.6/BlackDynamite/constraints_zeo.py
--rwxr-xr-x   0        0        0    13219 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/graphhelper.py
--rwxr-xr-x   0        0        0     1502 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/job.py
--rwxr-xr-x   0        0        0     1562 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/jobselector.py
--rw-r--r--   0        0        0     1909 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/loader.py
--rw-r--r--   0        0        0     4010 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/lowercase_btree.py
--rw-r--r--   0        0        0     3451 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/runLM.py
--rwxr-xr-x   0        0        0    14819 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/run_zeo.py
--rwxr-xr-x   0        0        0     1855 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/runselector.py
--rw-r--r--   0        0        0      736 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/__init__.py
--rw-r--r--   0        0        0      572 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/bash_completion.sh
--rwxr-xr-x   0        0        0      706 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/bd_zeo_server.py
--rwxr-xr-x   0        0        0     8370 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/canYouDigIt.py
--rwxr-xr-x   0        0        0     5550 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/cleanRuns.py
--rw-r--r--   0        0        0     1073 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createDB.py
--rw-r--r--   0        0        0     2941 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createJobs.py
--rwxr-xr-x   0        0        0     2466 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createRuns.py
--rwxr-xr-x   0        0        0     3306 2024-04-12 19:51:37.745664 blackdynamite-1.0.6/BlackDynamite/scripts/createUser.py
--rwxr-xr-x   0        0        0     3708 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/enterRun.py
--rw-r--r--   0        0        0     2201 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/fix_zeodb.py
--rw-r--r--   0        0        0     3886 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/getJobInfo.py
--rwxr-xr-x   0        0        0     8249 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/getRunInfo.py
--rwxr-xr-x   0        0        0     2788 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/launchRuns.py
--rwxr-xr-x   0        0        0     3032 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/mvRuns.py
--rwxr-xr-x   0        0        0     2404 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/open_zeodb.py
--rwxr-xr-x   0        0        0     1309 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/plotRuns.py
--rwxr-xr-x   0        0        0     2738 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/pushQuantity.py
--rwxr-xr-x   0        0        0     2676 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/saveBDStudy.py
--rw-r--r--   0        0        0     8821 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/streamlitInfo.py
--rwxr-xr-x   0        0        0     3438 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/studyInfo.py
--rwxr-xr-x   0        0        0     2417 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/scripts/updateRuns.py
--rw-r--r--   0        0        0     1229 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/selector.py
--rw-r--r--   0        0        0     7586 2024-04-12 19:51:37.746664 blackdynamite-1.0.6/BlackDynamite/zeoobject.py
--rw-r--r--   0        0        0    35149 2024-04-12 19:51:37.747664 blackdynamite-1.0.6/COPYING.txt
--rw-r--r--   0        0        0    12873 2024-04-12 19:51:37.747664 blackdynamite-1.0.6/README.md
--rw-r--r--   0        0        0     1142 2024-04-12 19:51:43.361613 blackdynamite-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 blackdynamite-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6239 2024-04-12 20:42:33.816377 blackdynamite-1.0.7/BlackDynamite/BDstat.py
+-rw-r--r--   0        0        0     1917 2024-04-12 20:42:33.816377 blackdynamite-1.0.7/BlackDynamite/__init__.py
+-rwxr-xr-x   0        0        0     7541 2024-04-12 20:42:33.816377 blackdynamite-1.0.7/BlackDynamite/base.py
+-rw-r--r--   0        0        0    23960 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/base_zeo.py
+-rw-r--r--   0        0        0     2272 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/bd_constraints.py
+-rw-r--r--   0        0        0     2943 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/bdlogging.py
+-rwxr-xr-x   0        0        0    16147 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/bdparser.py
+-rw-r--r--   0        0        0      781 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/coating/__init__.py
+-rwxr-xr-x   0        0        0     2995 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/coating/bashCoat.py
+-rwxr-xr-x   0        0        0     3998 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/coating/pbsCoat.py
+-rwxr-xr-x   0        0        0     3330 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/coating/sgeCoat.py
+-rwxr-xr-x   0        0        0     3410 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/coating/slurmCoat.py
+-rwxr-xr-x   0        0        0     2388 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/conffile_zeo.py
+-rw-r--r--   0        0        0     8943 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/constraints_zeo.py
+-rwxr-xr-x   0        0        0    13219 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/graphhelper.py
+-rwxr-xr-x   0        0        0     1502 2024-04-12 20:42:33.817376 blackdynamite-1.0.7/BlackDynamite/job.py
+-rwxr-xr-x   0        0        0     1562 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/jobselector.py
+-rw-r--r--   0        0        0     1909 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/loader.py
+-rw-r--r--   0        0        0     4010 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/lowercase_btree.py
+-rw-r--r--   0        0        0     3451 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/runLM.py
+-rwxr-xr-x   0        0        0    14819 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/run_zeo.py
+-rwxr-xr-x   0        0        0     1855 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/runselector.py
+-rw-r--r--   0        0        0      736 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/bash_completion.sh
+-rwxr-xr-x   0        0        0      706 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/bd_zeo_server.py
+-rwxr-xr-x   0        0        0     8370 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/canYouDigIt.py
+-rwxr-xr-x   0        0        0     5550 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/cleanRuns.py
+-rw-r--r--   0        0        0     1073 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/createDB.py
+-rw-r--r--   0        0        0     2941 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/createJobs.py
+-rwxr-xr-x   0        0        0     2466 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/createRuns.py
+-rwxr-xr-x   0        0        0     3306 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/createUser.py
+-rwxr-xr-x   0        0        0     3708 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/enterRun.py
+-rw-r--r--   0        0        0     2245 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/fix_zeodb.py
+-rw-r--r--   0        0        0     3886 2024-04-12 20:42:33.818376 blackdynamite-1.0.7/BlackDynamite/scripts/getJobInfo.py
+-rwxr-xr-x   0        0        0     8249 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/getRunInfo.py
+-rwxr-xr-x   0        0        0     2788 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/launchRuns.py
+-rwxr-xr-x   0        0        0     3032 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/mvRuns.py
+-rwxr-xr-x   0        0        0     2404 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/open_zeodb.py
+-rwxr-xr-x   0        0        0     1309 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/plotRuns.py
+-rwxr-xr-x   0        0        0     2738 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/pushQuantity.py
+-rwxr-xr-x   0        0        0     2676 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/saveBDStudy.py
+-rw-r--r--   0        0        0     8821 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/streamlitInfo.py
+-rwxr-xr-x   0        0        0     3438 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/studyInfo.py
+-rwxr-xr-x   0        0        0     2417 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/scripts/updateRuns.py
+-rw-r--r--   0        0        0     1229 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/selector.py
+-rw-r--r--   0        0        0     7586 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/BlackDynamite/zeoobject.py
+-rw-r--r--   0        0        0    35149 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/COPYING.txt
+-rw-r--r--   0        0        0    12873 2024-04-12 20:42:33.819376 blackdynamite-1.0.7/README.md
+-rw-r--r--   0        0        0     1142 2024-04-12 20:42:38.976287 blackdynamite-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    14176 1970-01-01 00:00:00.000000 blackdynamite-1.0.7/PKG-INFO
```

### Comparing `blackdynamite-1.0.6/BlackDynamite/BDstat.py` & `blackdynamite-1.0.7/BlackDynamite/BDstat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/__init__.py` & `blackdynamite-1.0.7/BlackDynamite/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/base.py` & `blackdynamite-1.0.7/BlackDynamite/base.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/base_zeo.py` & `blackdynamite-1.0.7/BlackDynamite/base_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/bd_constraints.py` & `blackdynamite-1.0.7/BlackDynamite/bd_constraints.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/bdlogging.py` & `blackdynamite-1.0.7/BlackDynamite/bdlogging.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/bdparser.py` & `blackdynamite-1.0.7/BlackDynamite/bdparser.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/coating/__init__.py` & `blackdynamite-1.0.7/BlackDynamite/coating/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/coating/bashCoat.py` & `blackdynamite-1.0.7/BlackDynamite/coating/bashCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/coating/pbsCoat.py` & `blackdynamite-1.0.7/BlackDynamite/coating/pbsCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/coating/sgeCoat.py` & `blackdynamite-1.0.7/BlackDynamite/coating/sgeCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/coating/slurmCoat.py` & `blackdynamite-1.0.7/BlackDynamite/coating/slurmCoat.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/conffile_zeo.py` & `blackdynamite-1.0.7/BlackDynamite/conffile_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/constraints_zeo.py` & `blackdynamite-1.0.7/BlackDynamite/constraints_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/graphhelper.py` & `blackdynamite-1.0.7/BlackDynamite/graphhelper.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/job.py` & `blackdynamite-1.0.7/BlackDynamite/job.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/jobselector.py` & `blackdynamite-1.0.7/BlackDynamite/jobselector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/loader.py` & `blackdynamite-1.0.7/BlackDynamite/loader.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/lowercase_btree.py` & `blackdynamite-1.0.7/BlackDynamite/lowercase_btree.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/runLM.py` & `blackdynamite-1.0.7/BlackDynamite/runLM.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/run_zeo.py` & `blackdynamite-1.0.7/BlackDynamite/run_zeo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/runselector.py` & `blackdynamite-1.0.7/BlackDynamite/runselector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/__init__.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/bash_completion.sh` & `blackdynamite-1.0.7/BlackDynamite/scripts/bash_completion.sh`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/bd_zeo_server.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/bd_zeo_server.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/canYouDigIt.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/canYouDigIt.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/cleanRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/cleanRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/createDB.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/createDB.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/createJobs.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/createJobs.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/createRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/createRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/createUser.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/createUser.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/enterRun.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/enterRun.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/fix_zeodb.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/fix_zeodb.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ################################################################
 def check_types(obj, desc):
     for name, e in desc.entries.items():
         if name not in obj.entries:
             raise RuntimeError('missing entry in run')
         _e = obj.entries[name]
-        if _e is not None and type(_e) != e:
+        if _e is not None and not isinstance(_e, e):
             raise RuntimeError(
                 f'incompatible types {name}: {_e}, {type(_e)} should be {e}')
 
 
 ################################################################
 def clean_run_entries(base):
     study = base.root.schemas[base.schema]
@@ -73,17 +73,19 @@
 ################################################################
 
 
 def main(argv=None):
     parser = BD.bdparser.BDParser()
     params = parser.parseBDParameters(argv)
     base = BD.Base(**params)
+    reconstruct_indexes(base)
+    base.commit()
     clean_job_entries(base)
+    base.commit()
     clean_run_entries(base)
-    reconstruct_indexes(base)
     base.commit()
 
 ################################################################
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/getJobInfo.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/getJobInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/getRunInfo.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/getRunInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/launchRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/launchRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/mvRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/mvRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/open_zeodb.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/open_zeodb.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/plotRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/plotRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/pushQuantity.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/pushQuantity.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/saveBDStudy.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/saveBDStudy.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/streamlitInfo.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/streamlitInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/studyInfo.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/studyInfo.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/scripts/updateRuns.py` & `blackdynamite-1.0.7/BlackDynamite/scripts/updateRuns.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/selector.py` & `blackdynamite-1.0.7/BlackDynamite/selector.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/BlackDynamite/zeoobject.py` & `blackdynamite-1.0.7/BlackDynamite/zeoobject.py`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/COPYING.txt` & `blackdynamite-1.0.7/COPYING.txt`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/README.md` & `blackdynamite-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blackdynamite-1.0.6/pyproject.toml` & `blackdynamite-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blackdynamite"
-version = "1.0.6"
+version = "1.0.7"
 description = "Scientific Parametric Study Tool"
 authors = ["Guillaume Anciaux <guillaume.anciaux@epfl.ch>"]
 license = "GPL"
 readme = "README.md"
 packages = [{include = "BlackDynamite"}]
 homepage = "https://gitlab.com/ganciaux/blackdynamite"
 repository = "https://gitlab.com/ganciaux/blackdynamite"
```

### Comparing `blackdynamite-1.0.6/PKG-INFO` & `blackdynamite-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackdynamite
-Version: 1.0.6
+Version: 1.0.7
 Summary: Scientific Parametric Study Tool
 Home-page: https://gitlab.com/ganciaux/blackdynamite
 License: GPL
 Author: Guillaume Anciaux
 Author-email: guillaume.anciaux@epfl.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

