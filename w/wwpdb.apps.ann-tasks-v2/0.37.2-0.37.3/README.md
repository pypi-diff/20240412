# Comparing `tmp/wwpdb.apps.ann_tasks_v2-0.37.2.tar.gz` & `tmp/wwpdb_apps_ann_tasks_v2-0.37.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.37.2.tar", last modified: Sun Mar 17 16:20:42 2024, max compression
+gzip compressed data, was "wwpdb_apps_ann_tasks_v2-0.37.3.tar", last modified: Fri Apr 12 17:50:21 2024, max compression
```

## Comparing `wwpdb.apps.ann_tasks_v2-0.37.2.tar` & `wwpdb_apps_ann_tasks_v2-0.37.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.129980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (127)     5712 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6865 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33886 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.133980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14499 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12364 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12679 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (127)    10620 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    15912 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.137980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24814 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    80925 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33069 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6107 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8388 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.141980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)   178553 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15293 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    65098 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-03-17 16:18:08.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-17 16:20:42.145980 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-03-17 16:20:42.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5537 2024-03-17 16:20:42.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-17 16:20:42.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-17 16:19:55.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-03-17 16:20:42.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-03-17 16:20:42.000000 wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2540 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.645779 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (127)    39726 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46849 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5712 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7708 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4947 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4344 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3727 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3138 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6865 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33886 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16936 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (127)      998 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3945 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2573 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4448 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4053 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19613 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5646 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.649778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6295 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14499 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2942 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3345 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12364 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12679 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10620 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12969 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18806 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11248 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15912 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9923 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3057 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3231 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4323 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3336 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4763 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5394 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4764 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3305 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3716 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3561 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21849 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6954 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3694 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8475 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3526 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1540 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2010 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4025 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.653778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8209 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24946 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8612 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    81504 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33069 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3094 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3037 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (127)    33282 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3759 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6619 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6242 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1509 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3451 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4026 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8388 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3396 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4790 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3021 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4071 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3053 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10304 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5085 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.657778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5627 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46092 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   178553 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15293 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    65098 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16955 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 17:48:14.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 17:50:21.661778 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5537 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 17:49:39.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      323 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-12 17:50:21.000000 wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.2
+Version: 0.37.3
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/setup.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/Check.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
                 ("pdbx_struct_assembly_gen", "Assembly Gen Details", "row-wise"),
                 ("pdbx_struct_oper_list", "Assembly Oper List Details", "row-wise"),
                 ("pdbx_struct_assembly_depositor_info", "Author Assembly Details", "row-wise"),
                 ("pdbx_struct_assembly_auth_evidence", "Author Assembly Evidence", "row-wise"),
                 # ('pdbx_depui_status_flags', 'DepUI Flags', 'row-wise'),
                 ("pdbx_SG_project", "Structural genomics", "row-wise"),
                 ("pdbx_database_related", "Related entries", "row-wise"),
+                ("pdbx_initial_refinement_model", "Starting models", "row-wise"),
                 ("pdbx_contact_author", "Contact authors", "row-wise"),
                 # ('citation','Primary citation','column-wise'),
                 ("pdbx_validate_close_contact", "Close contacts", "row-wise"),
                 ("pdbx_validate_symm_contact", "Close symmetry contacts", "row-wise"),
                 ("struct_conn", "Links", "row-wise"),
                 # ('symmetry', 'Symmetry', 'row-wise'),
                 # ('cell', 'Cell constants', 'row-wise'),
@@ -312,18 +313,21 @@
         for ii, (catName, catNameAbbrev, catStyle) in enumerate(catList):
             # For only popuated categories
             if catName in cD and (len(cD[catName]) > 0):
                 active = "in" if isFirst else ""
                 idSection = idPrefix + "-sec-" + str(ii)
                 oL.append('<div class="accordion-group">')
                 oL.append('<div class="accordion-heading">')
+
+                abbrev = "%s [%s]" % (catNameAbbrev, catName)
+
                 if isMulti:
-                    oL.append('<a class="accordion-toggle" data-toggle="collapse" href="#%s"> <h4>%s</h4></a>' % (idSection, catNameAbbrev))
+                    oL.append('<a class="accordion-toggle" data-toggle="collapse" href="#%s"> <h4>%s</h4></a>' % (idSection, abbrev))
                 else:
-                    oL.append('<a class="accordion-toggle" data-toggle="collapse" data-parent="#%s" href="#%s"><h4>%s</h4></a>' % (idTop, idSection, catNameAbbrev))
+                    oL.append('<a class="accordion-toggle" data-toggle="collapse" data-parent="#%s" href="#%s"><h4>%s</h4></a>' % (idTop, idSection, abbrev))
                 oL.append("</div>")
                 oL.append('<div id="%s" class="accordion-body collapse %s">' % (idSection, active))
                 oL.append('<div  class="accordion-inner">')
                 #
                 oL.append('<table class="table table-striped table-bordered table-condensed">')
                 if catStyle == "column-wise":
                     self.__renderTableColumnWise(catName, cD[catName][0], oL)
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         ("pdbx_contact_author", "table"),
         ("pdbx_SG_project", "table"),
         ("audit_author", "table"),
         ("pdbx_database_status", "table"),
         ("pdbx_depui_status_flags", "table"),
         ("pdbx_database_proc", "table"),
         ("pdbx_database_related", "table"),
+        ("pdbx_initial_refinement_model", "table"),
         ("pdbx_related_exp_data_set", "table"),
         ("database_PDB_rev", "table"),
         ("pdbx_database_PDB_obs_spr", "table"),
         ("pdbx_database_PDB_remark", "table"),
         ("struct_ref", "table"),
         ("struct_keywords", "table"),
         ("pdbx_struct_assembly", "table"),
@@ -284,26 +285,36 @@
         ],
         "pdbx_database_PDB_obs_spr": [
             ("_pdbx_database_PDB_obs_spr.id", "%s", "str", ""),
             ("_pdbx_database_PDB_obs_spr.date", "%s", "str", ""),
             ("_pdbx_database_PDB_obs_spr.pdb_id", "%s", "str", ""),
             ("_pdbx_database_PDB_obs_spr.replace_pdb_id", "%s", "str", ""),
         ],
-        "pdbx_database_PDB_remark": [("_pdbx_database_PDB_remark.id", "%s", "str", ""), ("_pdbx_database_PDB_remark.text", "%s", "str", "")],
+        "pdbx_database_PDB_remark": [
+            ("_pdbx_database_PDB_remark.id", "%s", "str", ""),
+            ("_pdbx_database_PDB_remark.text", "%s", "str", "")],
         "pdbx_entity_instance_feature": [
             ("_pdbx_entity_instance_feature.ordinal", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.comp_id", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.auth_comp_id", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.feature_type", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.asym_id", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.auth_asym_id", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.auth_seq_num", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.details", "%s", "str", ""),
             ("_pdbx_entity_instance_feature.seq_num", "%s", "str", ""),
         ],
+        "pdbx_initial_refinement_model": [
+            ("_pdbx_initial_refinement_model.id", "%s", "str", ""),
+            ("_pdbx_initial_refinement_model.type", "%s", "str", ""),
+            ("_pdbx_initial_refinement_model.source_name", "%s", "str", ""),
+            ("_pdbx_initial_refinement_model.accession_code", "%s", "str", ""),
+            ("_pdbx_initial_refinement_model.details", "%s", "str", ""),
+            ("_pdbx_initial_refinement_model.entity_id_list", "%s", "str", ""),
+        ],
         "struct_ref": [
             ("_struct_ref.id", "%s", "str", ""),
             ("_struct_ref.entity_id", "%s", "str", ""),
             ("_struct_ref.db_name", "%s", "str", ""),
             ("_struct_ref.pdbx_db_accession", "%s", "str", ""),
             ("_struct_ref.db_code", "%s", "str", ""),
             ("_struct_ref.pdbx_db_isoform", "%s", "str", ""),
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/GetCovalentBond.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
           </tr>
         </table>
         <br/>
         <table class="table table-bordered table-striped width100">
           <tr>
             <th colspan="5">Atom1</th>
             <th colspan="5">Atom2</th>
+            <th rowspan="2">Leaving<br/>atoms</th>
             <th rowspan="2">Distance</th>
           </tr>
           <tr>
             <th>Chain ID</th>
             <th>Residue</th>
             <th>Number</th>
             <th>Atom</th>
@@ -125,21 +126,24 @@
                 atom += "(" + tupL[5] + ")"
             #
             tablerow += "<td>" + tupL[0] + "</td>" + "<td>" + tupL[1] + "</td>" + "<td>" + tupL[2] + tupL[3] + "</td>" + "<td>" + atom + "</td>" + "<td>" + tupL[6] + "</td>"
             atom = tupL[11]
             if tupL[12]:
                 atom += "(" + tupL[12] + ")"
             #
-            tablerow += "<td>" + tupL[7] + "</td>" + "<td>" + tupL[8] + "</td>" + "<td>" + tupL[9] + tupL[10] + "</td>" + "<td>" + atom + "</td>" + "<td>" + tupL[13] + "</td>"
+            tablerow += "<td>" + tupL[7] + "</td>" + "<td>" + tupL[8] \
+                + "</td>" + "<td>" + tupL[9] + tupL[10] + "</td>" + "<td>" \
+                + atom + "</td>" + "<td>" + tupL[13] + "</td>" + "<td>" \
+                + tupL[14] + "</td>"
             #
             tupL[6] = tupL[6].replace("_", "-")
             tupL[13] = tupL[13].replace("_", "-")
             bond_id = "covalent_bond_" + str(count)
             #
-            tablerow += "<td>" + tupL[14] + '&nbsp; &nbsp; &nbsp; &nbsp; <input type="checkbox" id="' + bond_id + '" name="' + bond_id + '" value="' + "_".join(tupL) + '"/></td>'
+            tablerow += "<td>" + tupL[15] + '&nbsp; &nbsp; &nbsp; &nbsp; <input type="checkbox" id="' + bond_id + '" name="' + bond_id + '" value="' + "_".join(tupL) + '"/></td>'
             #
             tablerow += "</tr>\n"
             count += 1
         #
         return htmlTemplate % (str(count), tablerow)
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/utils/UpdateCovalentBond.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.37.2
+Version: 0.37.3
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.37.2/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb_apps_ann_tasks_v2-0.37.3/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

