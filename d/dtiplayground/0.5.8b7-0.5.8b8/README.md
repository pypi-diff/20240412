# Comparing `tmp/dtiplayground-0.5.8b7.tar.gz` & `tmp/dtiplayground-0.5.8b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtiplayground-0.5.8b7.tar", last modified: Thu Mar 28 19:50:45 2024, max compression
+gzip compressed data, was "dtiplayground-0.5.8b8.tar", last modified: Fri Apr 12 20:28:52 2024, max compression
```

## Comparing `dtiplayground-0.5.8b7.tar` & `dtiplayground-0.5.8b8.tar`

### file list

```diff
@@ -1,203 +1,239 @@
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.484537 dtiplayground-0.5.8b7/
--rw-r--r--   0 styner   (26802) res       (1001)     1132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/LICENSE
--rw-r--r--   0 styner   (26802) res       (1001)      386 2024-03-28 19:50:45.485537 dtiplayground-0.5.8b7/PKG-INFO
--rw-r--r--   0 styner   (26802) res       (1001)      326 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/README.rst
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.410536 dtiplayground-0.5.8b7/bin/
--rwxr-xr-x   0 styner   (26802) res       (1001)      126 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriatlas
--rwxr-xr-x   0 styner   (26802) res       (1001)     6914 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriatlas.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      130 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriautotract
--rwxr-xr-x   0 styner   (26802) res       (1001)    38839 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriautotract.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      133 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmrifiberprofile
--rwxr-xr-x   0 styner   (26802) res       (1001)    37702 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/bin/dmrifiberprofile.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriplayground
--rwxr-xr-x   0 styner   (26802) res       (1001)     6543 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriplayground.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      147 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriplaygroundlab
--rwxr-xr-x   0 styner   (26802) res       (1001)      125 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriprep
--rwxr-xr-x   0 styner   (26802) res       (1001)    11984 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/bin/dmriprep.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:41.663490 dtiplayground-0.5.8b7/dtiplayground/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:41.736491 dtiplayground-0.5.8b7/dtiplayground/api/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    13478 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/application.py
--rw-r--r--   0 styner   (26802) res       (1001)     6162 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/dmriatlasbuilder.py
--rw-r--r--   0 styner   (26802) res       (1001)    15605 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/dmriprep.py
--rw-r--r--   0 styner   (26802) res       (1001)     2396 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/server.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:41.740491 dtiplayground-0.5.8b7/dtiplayground/api/static/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/static/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:41.746491 dtiplayground-0.5.8b7/dtiplayground/api/static/spa/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/static/spa/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)  1215620 2024-02-29 18:44:07.000000 dtiplayground-0.5.8b7/dtiplayground/api/static/spa/spa.zip
--rw-r--r--   0 styner   (26802) res       (1001)     4904 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/api/utils.py
--rw-r--r--   0 styner   (26802) res       (1001)      321 2024-03-28 19:50:23.000000 dtiplayground-0.5.8b7/dtiplayground/config.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.213521 dtiplayground-0.5.8b7/dtiplayground/dmri/
--rwxr-xr-x   0 styner   (26802) res       (1001)      314 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.253522 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/
--rwxr-xr-x   0 styner   (26802) res       (1001)      249 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)     2065 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/app.py
--rwxr-xr-x   0 styner   (26802) res       (1001)    72751 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/atlasbuilder.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.279522 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/
--rwxr-xr-x   0 styner   (26802) res       (1001)     1843 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    29281 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/template.json
--rwxr-xr-x   0 styner   (26802) res       (1001)    24909 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/utils.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.337523 dtiplayground-0.5.8b7/dtiplayground/dmri/common/
--rwxr-xr-x   0 styner   (26802) res       (1001)     5542 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    24510 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/appbase.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.404523 dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    77533 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/fslinstaller.py
--rw-r--r--   0 styner   (26802) res       (1001)    97554 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/fslinstaller_py2.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     2151 2024-03-07 20:32:29.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/software_paths.yml
--rw-r--r--   0 styner   (26802) res       (1001)    29194 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/dwi.py
--rw-r--r--   0 styner   (26802) res       (1001)    21885 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/module.py
--rw-r--r--   0 styner   (26802) res       (1001)    23986 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/pipeline.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.424524 dtiplayground-0.5.8b7/dtiplayground/dmri/common/study/
--rwxr-xr-x   0 styner   (26802) res       (1001)     1444 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/study/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     2018 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/study/loaders.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.527525 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/
--rwxr-xr-x   0 styner   (26802) res       (1001)      597 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     2897 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/base.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1090 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/brainsfit.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      394 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/crop_dti.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     4132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dti_reg.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      748 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtiaverage.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      493 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtiestim.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1624 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtiprocess.py
--rw-r--r--   0 styner   (26802) res       (1001)     2775 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtitractstat.py
--rw-r--r--   0 styner   (26802) res       (1001)     3867 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fiberpostprocess.py
--rw-r--r--   0 styner   (26802) res       (1001)     2690 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fiberprocess.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     8801 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fsl.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      435 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/greedy_atlas.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1141 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/image_math.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      221 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/itk_transform_tools.py
--rw-r--r--   0 styner   (26802) res       (1001)     2140 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/niral_utilities.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     3174 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      663 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/unu.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.534525 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.574526 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.586526 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/
--rw-r--r--   0 styner   (26802) res       (1001)    12320 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.py
--rw-r--r--   0 styner   (26802) res       (1001)     3293 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.yml
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.623526 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/
--rw-r--r--   0 styner   (26802) res       (1001)      796 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py
--rw-r--r--   0 styner   (26802) res       (1001)      346 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.yml
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)      102 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    12436 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/protocols.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.636526 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)      792 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/module_template.py
--rw-r--r--   0 styner   (26802) res       (1001)      338 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/module_template.yml
--rwxr-xr-x   0 styner   (26802) res       (1001)     1717 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.643526 dtiplayground-0.5.8b7/dtiplayground/dmri/playground/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/playground/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)     3004 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/playground/app.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.658527 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/
--rw-r--r--   0 styner   (26802) res       (1001)     2574 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)      341 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)    19346 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/app.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.666527 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/data/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/data/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1966 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/data/software_paths.yml
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.682527 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.736528 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/
--rwxr-xr-x   0 styner   (26802) res       (1001)    12259 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     2505 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml
--rw-r--r--   0 styner   (26802) res       (1001)     1273 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.750528 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/
--rwxr-xr-x   0 styner   (26802) res       (1001)     6566 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1508 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml
--rw-r--r--   0 styner   (26802) res       (1001)      673 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.792528 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/
--rw-r--r--   0 styner   (26802) res       (1001)    15616 2024-03-08 22:38:42.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py
--rw-r--r--   0 styner   (26802) res       (1001)     4381 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml
--rw-r--r--   0 styner   (26802) res       (1001)     2491 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.809528 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/
--rwxr-xr-x   0 styner   (26802) res       (1001)     7795 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     2062 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml
--rw-r--r--   0 styner   (26802) res       (1001)     1073 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.857529 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/
--rw-r--r--   0 styner   (26802) res       (1001)     5846 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py
--rw-r--r--   0 styner   (26802) res       (1001)     2343 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml
--rw-r--r--   0 styner   (26802) res       (1001)     1248 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.884529 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/
--rwxr-xr-x   0 styner   (26802) res       (1001)    12921 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1230 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml
--rw-r--r--   0 styner   (26802) res       (1001)      675 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.971531 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/
--rw-r--r--   0 styner   (26802) res       (1001)     1199 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py
--rw-r--r--   0 styner   (26802) res       (1001)      552 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml
--rw-r--r--   0 styner   (26802) res       (1001)      226 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:44.986531 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/
--rw-r--r--   0 styner   (26802) res       (1001)     8945 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py
--rw-r--r--   0 styner   (26802) res       (1001)     1778 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml
--rw-r--r--   0 styner   (26802) res       (1001)      929 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.010531 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/
--rwxr-xr-x   0 styner   (26802) res       (1001)    15789 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1637 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml
--rw-r--r--   0 styner   (26802) res       (1001)      954 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.025531 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/
--rw-r--r--   0 styner   (26802) res       (1001)     1939 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py
--rw-r--r--   0 styner   (26802) res       (1001)      417 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.yml
--rw-r--r--   0 styner   (26802) res       (1001)      349 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.040531 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/
--rw-r--r--   0 styner   (26802) res       (1001)    19190 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py
--rw-r--r--   0 styner   (26802) res       (1001)      481 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.yml
--rw-r--r--   0 styner   (26802) res       (1001)      343 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/README.md
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.092532 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/
--rw-r--r--   0 styner   (26802) res       (1001)     1227 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)     9061 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py
--rwxr-xr-x   0 styner   (26802) res       (1001)     1943 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.138532 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/
--rw-r--r--   0 styner   (26802) res       (1001)      618 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md
--rwxr-xr-x   0 styner   (26802) res       (1001)    19435 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      955 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml
--rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.144533 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      997 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.202533 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/
--rw-r--r--   0 styner   (26802) res       (1001)      235 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/README.md
--rw-r--r--   0 styner   (26802) res       (1001)     1745 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py
--rw-r--r--   0 styner   (26802) res       (1001)      356 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.yml
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)       88 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/__init__.py
--rwxr-xr-x   0 styner   (26802) res       (1001)      655 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/protocols.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.219534 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)      101 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/module_template.md
--rw-r--r--   0 styner   (26802) res       (1001)      818 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/module_template.py
--rw-r--r--   0 styner   (26802) res       (1001)      330 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/module_template.yml
--rwxr-xr-x   0 styner   (26802) res       (1001)     5440 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/protocol_template.yml
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.225534 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/__init__.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.235534 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/modules/
--rw-r--r--   0 styner   (26802) res       (1001)      102 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/modules/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)      655 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/protocols.py
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.268534 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/
--rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/__init__.py
--rw-r--r--   0 styner   (26802) res       (1001)      792 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/module_template.py
--rw-r--r--   0 styner   (26802) res       (1001)      338 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/module_template.yml
--rwxr-xr-x   0 styner   (26802) res       (1001)     2666 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/protocol_template.yml
-drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-03-28 19:50:45.481537 dtiplayground-0.5.8b7/dtiplayground.egg-info/
--rw-r--r--   0 styner   (26802) res       (1001)      386 2024-03-28 19:50:40.000000 dtiplayground-0.5.8b7/dtiplayground.egg-info/PKG-INFO
--rw-r--r--   0 styner   (26802) res       (1001)     8775 2024-03-28 19:50:41.000000 dtiplayground-0.5.8b7/dtiplayground.egg-info/SOURCES.txt
--rw-r--r--   0 styner   (26802) res       (1001)        1 2024-03-28 19:50:40.000000 dtiplayground-0.5.8b7/dtiplayground.egg-info/dependency_links.txt
--rw-r--r--   0 styner   (26802) res       (1001)      205 2024-03-28 19:50:40.000000 dtiplayground-0.5.8b7/dtiplayground.egg-info/requires.txt
--rw-r--r--   0 styner   (26802) res       (1001)       14 2024-03-28 19:50:40.000000 dtiplayground-0.5.8b7/dtiplayground.egg-info/top_level.txt
--rw-r--r--   0 styner   (26802) res       (1001)      103 2024-03-28 19:50:45.488537 dtiplayground-0.5.8b7/setup.cfg
--rw-r--r--   0 styner   (26802) res       (1001)     1525 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b7/setup.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.211020 dtiplayground-0.5.8b8/
+-rwxr-xr-x   0 styner   (26802) res       (1001)      185 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/.gitignore
+-rw-r--r--   0 styner   (26802) res       (1001)      104 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/.readthedocs.yaml
+-rw-r--r--   0 styner   (26802) res       (1001)     1132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/LICENSE
+-rw-r--r--   0 styner   (26802) res       (1001)      386 2024-04-12 20:28:52.211020 dtiplayground-0.5.8b8/PKG-INFO
+-rwxr-xr-x   0 styner   (26802) res       (1001)    17857 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)      326 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/README.rst
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.968017 dtiplayground-0.5.8b8/bin/
+-rwxr-xr-x   0 styner   (26802) res       (1001)      126 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriatlas
+-rwxr-xr-x   0 styner   (26802) res       (1001)     6914 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriatlas.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      130 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriautotract
+-rwxr-xr-x   0 styner   (26802) res       (1001)    38839 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriautotract.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      133 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmrifiberprofile
+-rwxr-xr-x   0 styner   (26802) res       (1001)    37702 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b8/bin/dmrifiberprofile.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriplayground
+-rwxr-xr-x   0 styner   (26802) res       (1001)     6543 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriplayground.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      147 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriplaygroundlab
+-rwxr-xr-x   0 styner   (26802) res       (1001)      125 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriprep
+-rwxr-xr-x   0 styner   (26802) res       (1001)    11984 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/bin/dmriprep.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.979017 dtiplayground-0.5.8b8/dockerfiles/
+-rw-r--r--   0 styner   (26802) res       (1001)      819 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dockerfiles/Dockerfile
+-rw-r--r--   0 styner   (26802) res       (1001)      997 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dockerfiles/Dockerfile.centos7
+-rw-r--r--   0 styner   (26802) res       (1001)     1378 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dockerfiles/docker-compose.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.016017 dtiplayground-0.5.8b8/docs/
+-rw-r--r--   0 styner   (26802) res       (1001)     1233 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/DMRIAtlasBuilder.rst
+-rw-r--r--   0 styner   (26802) res       (1001)     8725 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b8/docs/DMRIFiberProfile.rst
+-rw-r--r--   0 styner   (26802) res       (1001)     6506 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/DMRIPrep.rst
+-rw-r--r--   0 styner   (26802) res       (1001)      531 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/DMRIViewer.rst
+-rw-r--r--   0 styner   (26802) res       (1001)      634 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/Makefile
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.174019 dtiplayground-0.5.8b8/docs/_static/
+-rw-r--r--   0 styner   (26802) res       (1001)   123406 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/dmriatlas_ui.png
+-rw-r--r--   0 styner   (26802) res       (1001)   149150 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/dmriprep_ui.png
+-rw-r--r--   0 styner   (26802) res       (1001)   242770 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/dtilab_viewer_dwi.png
+-rw-r--r--   0 styner   (26802) res       (1001)   513705 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/dtilab_viewer_tract.png
+-rw-r--r--   0 styner   (26802) res       (1001)    38100 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/niral_logo.jpg
+-rw-r--r--   0 styner   (26802) res       (1001)   132063 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/niral_logo.png
+-rw-r--r--   0 styner   (26802) res       (1001)        1 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/_static/overrides.css
+-rw-r--r--   0 styner   (26802) res       (1001)     1875 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/conf.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.180019 dtiplayground-0.5.8b8/docs/ext/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/ext/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2797 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/ext/github_link.py
+-rw-r--r--   0 styner   (26802) res       (1001)      665 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/docs/index.rst
+-rw-r--r--   0 styner   (26802) res       (1001)     4458 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/installation.rst
+-rw-r--r--   0 styner   (26802) res       (1001)       41 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/license.rst
+-rw-r--r--   0 styner   (26802) res       (1001)      801 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/make.bat
+-rw-r--r--   0 styner   (26802) res       (1001)       16 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/docs/requirements.txt
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.331009 dtiplayground-0.5.8b8/dtiplayground/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.355009 dtiplayground-0.5.8b8/dtiplayground/api/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    13478 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/application.py
+-rw-r--r--   0 styner   (26802) res       (1001)     6162 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/dmriatlasbuilder.py
+-rw-r--r--   0 styner   (26802) res       (1001)    14846 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/api/dmrifiberprofile.py
+-rw-r--r--   0 styner   (26802) res       (1001)    15605 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/dmriprep.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2547 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/api/server.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.359009 dtiplayground-0.5.8b8/dtiplayground/api/static/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/static/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.364009 dtiplayground-0.5.8b8/dtiplayground/api/static/spa/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/static/spa/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)  1215620 2024-04-12 20:25:35.000000 dtiplayground-0.5.8b8/dtiplayground/api/static/spa/spa.zip
+-rw-r--r--   0 styner   (26802) res       (1001)     4904 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/api/utils.py
+-rw-r--r--   0 styner   (26802) res       (1001)      321 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/config.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.398010 dtiplayground-0.5.8b8/dtiplayground/dmri/
+-rwxr-xr-x   0 styner   (26802) res       (1001)      314 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.412010 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/
+-rwxr-xr-x   0 styner   (26802) res       (1001)      249 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2065 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/app.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)    72751 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/atlasbuilder.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.422010 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1843 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    29281 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/template.json
+-rwxr-xr-x   0 styner   (26802) res       (1001)    24909 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/utils.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.442010 dtiplayground-0.5.8b8/dtiplayground/dmri/common/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     5542 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    24510 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/appbase.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.459010 dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    77533 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/fslinstaller.py
+-rw-r--r--   0 styner   (26802) res       (1001)    97554 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/fslinstaller_py2.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2151 2024-03-07 20:32:29.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/software_paths.yml
+-rw-r--r--   0 styner   (26802) res       (1001)    29194 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/dwi.py
+-rw-r--r--   0 styner   (26802) res       (1001)    21885 2024-03-28 19:48:20.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/module.py
+-rw-r--r--   0 styner   (26802) res       (1001)    24087 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/pipeline.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.467011 dtiplayground-0.5.8b8/dtiplayground/dmri/common/study/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1444 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/study/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2018 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/study/loaders.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.568012 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/
+-rwxr-xr-x   0 styner   (26802) res       (1001)      597 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2897 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/base.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1090 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/brainsfit.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      394 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/crop_dti.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     4132 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dti_reg.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      748 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtiaverage.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      493 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtiestim.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1624 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtiprocess.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2775 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtitractstat.py
+-rw-r--r--   0 styner   (26802) res       (1001)     3867 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fiberpostprocess.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2690 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fiberprocess.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     8801 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fsl.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      435 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/greedy_atlas.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1141 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/image_math.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      221 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/itk_transform_tools.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2140 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/niral_utilities.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     3174 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      663 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/unu.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.578012 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    18489 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/app.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.582012 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.593012 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/
+-rw-r--r--   0 styner   (26802) res       (1001)    14674 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.py
+-rw-r--r--   0 styner   (26802) res       (1001)     4234 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.yml
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.603012 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/
+-rw-r--r--   0 styner   (26802) res       (1001)      796 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py
+-rw-r--r--   0 styner   (26802) res       (1001)      346 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.yml
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)      102 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    13420 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/protocols.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.616012 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)      792 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/module_template.py
+-rw-r--r--   0 styner   (26802) res       (1001)      338 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/module_template.yml
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2435 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.622012 dtiplayground-0.5.8b8/dtiplayground/dmri/playground/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/playground/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)     3004 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/playground/app.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.635013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/
+-rw-r--r--   0 styner   (26802) res       (1001)     2574 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)      341 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)    19346 2024-02-29 20:39:48.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/app.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.642013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/data/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/data/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1966 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/data/software_paths.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.205020 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/docs/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2110 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/docs/objects.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.645013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.659013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/
+-rwxr-xr-x   0 styner   (26802) res       (1001)    12259 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2505 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml
+-rw-r--r--   0 styner   (26802) res       (1001)     1273 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.672013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     8121 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1839 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      673 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.685013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/
+-rw-r--r--   0 styner   (26802) res       (1001)    15616 2024-03-08 22:38:42.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py
+-rw-r--r--   0 styner   (26802) res       (1001)     4381 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml
+-rw-r--r--   0 styner   (26802) res       (1001)     2491 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.699013 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/
+-rwxr-xr-x   0 styner   (26802) res       (1001)     7953 2024-04-12 20:28:32.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2062 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml
+-rw-r--r--   0 styner   (26802) res       (1001)     1073 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.737014 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/
+-rw-r--r--   0 styner   (26802) res       (1001)     5846 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py
+-rw-r--r--   0 styner   (26802) res       (1001)     2343 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml
+-rw-r--r--   0 styner   (26802) res       (1001)     1248 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.750014 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/
+-rwxr-xr-x   0 styner   (26802) res       (1001)    12921 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1230 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      675 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.763014 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/
+-rw-r--r--   0 styner   (26802) res       (1001)     1199 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py
+-rw-r--r--   0 styner   (26802) res       (1001)      552 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      226 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.776014 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/
+-rw-r--r--   0 styner   (26802) res       (1001)     8945 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py
+-rw-r--r--   0 styner   (26802) res       (1001)     1778 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      929 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.789014 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/
+-rwxr-xr-x   0 styner   (26802) res       (1001)    15789 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1637 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      954 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.801015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/
+-rw-r--r--   0 styner   (26802) res       (1001)     1939 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py
+-rw-r--r--   0 styner   (26802) res       (1001)      417 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      349 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.814015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/
+-rw-r--r--   0 styner   (26802) res       (1001)    19190 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py
+-rw-r--r--   0 styner   (26802) res       (1001)      481 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.yml
+-rw-r--r--   0 styner   (26802) res       (1001)      343 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.826015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/
+-rw-r--r--   0 styner   (26802) res       (1001)     1227 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)     9061 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)     1943 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.839015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/
+-rw-r--r--   0 styner   (26802) res       (1001)      618 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md
+-rwxr-xr-x   0 styner   (26802) res       (1001)    19435 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      955 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml
+-rwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.845015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      997 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.859015 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/
+-rw-r--r--   0 styner   (26802) res       (1001)      235 2024-02-05 20:46:15.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/README.md
+-rw-r--r--   0 styner   (26802) res       (1001)     1745 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py
+-rw-r--r--   0 styner   (26802) res       (1001)      356 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.yml
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)       88 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/__init__.py
+-rwxr-xr-x   0 styner   (26802) res       (1001)      655 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/protocols.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.874016 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)      101 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/module_template.md
+-rw-r--r--   0 styner   (26802) res       (1001)      818 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/module_template.py
+-rw-r--r--   0 styner   (26802) res       (1001)      330 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/module_template.yml
+-rwxr-xr-x   0 styner   (26802) res       (1001)     5440 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/protocol_template.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.880016 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/__init__.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.884016 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/modules/
+-rw-r--r--   0 styner   (26802) res       (1001)      102 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/modules/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)      655 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/protocols.py
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:51.918016 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/
+-rw-r--r--   0 styner   (26802) res       (1001)        0 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/__init__.py
+-rw-r--r--   0 styner   (26802) res       (1001)      792 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/module_template.py
+-rw-r--r--   0 styner   (26802) res       (1001)      338 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/module_template.yml
+-rwxr-xr-x   0 styner   (26802) res       (1001)     2666 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/protocol_template.yml
+drwxr-xr-x   0 styner   (26802) res       (1001)        0 2024-04-12 20:28:52.199020 dtiplayground-0.5.8b8/dtiplayground.egg-info/
+-rw-r--r--   0 styner   (26802) res       (1001)      386 2024-04-12 20:28:50.000000 dtiplayground-0.5.8b8/dtiplayground.egg-info/PKG-INFO
+-rw-r--r--   0 styner   (26802) res       (1001)    17646 2024-04-12 20:28:51.000000 dtiplayground-0.5.8b8/dtiplayground.egg-info/SOURCES.txt
+-rw-r--r--   0 styner   (26802) res       (1001)        1 2024-04-12 20:28:50.000000 dtiplayground-0.5.8b8/dtiplayground.egg-info/dependency_links.txt
+-rw-r--r--   0 styner   (26802) res       (1001)      205 2024-04-12 20:28:50.000000 dtiplayground-0.5.8b8/dtiplayground.egg-info/requires.txt
+-rw-r--r--   0 styner   (26802) res       (1001)       14 2024-04-12 20:28:50.000000 dtiplayground-0.5.8b8/dtiplayground.egg-info/top_level.txt
+-rw-r--r--   0 styner   (26802) res       (1001)      278 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/requirements-headless.txt
+-rwxr-xr-x   0 styner   (26802) res       (1001)      233 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/requirements.txt
+-rw-r--r--   0 styner   (26802) res       (1001)      103 2024-04-12 20:28:52.215020 dtiplayground-0.5.8b8/setup.cfg
+-rw-r--r--   0 styner   (26802) res       (1001)     1525 2024-02-05 20:46:16.000000 dtiplayground-0.5.8b8/setup.py
```

### Comparing `dtiplayground-0.5.8b7/LICENSE` & `dtiplayground-0.5.8b8/LICENSE`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/bin/dmriatlas.py` & `dtiplayground-0.5.8b8/bin/dmriatlas.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/bin/dmriautotract.py` & `dtiplayground-0.5.8b8/bin/dmriautotract.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/bin/dmrifiberprofile.py` & `dtiplayground-0.5.8b8/bin/dmrifiberprofile.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/bin/dmriplayground.py` & `dtiplayground-0.5.8b8/bin/dmriplayground.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/bin/dmriprep.py` & `dtiplayground-0.5.8b8/bin/dmriprep.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/application.py` & `dtiplayground-0.5.8b8/dtiplayground/api/application.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/dmriatlasbuilder.py` & `dtiplayground-0.5.8b8/dtiplayground/api/dmriatlasbuilder.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/dmriprep.py` & `dtiplayground-0.5.8b8/dtiplayground/api/dmriprep.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/server.py` & `dtiplayground-0.5.8b8/dtiplayground/api/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 logger=dtiplayground.dmri.common.logger.write 
 color= dtiplayground.dmri.common.Color
 
 ### APIs
 from dtiplayground.api.application import ApplicationAPI 
 from dtiplayground.api.dmriatlasbuilder import DMRIAtlasbuilderAPI
 from dtiplayground.api.dmriprep import DMRIPrepAPI
+from dtiplayground.api.dmrifiberprofile import DMRIFiberProfileAPI
 
 class DTIPlaygroundServer(object):
     def __init__(self,*args,**kwargs):
         kwargs.setdefault('config_dir', Path.home().joinpath('.niral-dti').__str__())
         kwargs.setdefault('host', '127.0.0.1')
         kwargs.setdefault('port', 6543)
         kwargs.setdefault('static_url_path','/')
@@ -49,14 +50,15 @@
         self.app=Flask(__name__, static_folder=self.static_folder, static_url_path=self.static_url_path)
         CORS(self.app)
 
         self.app.config['SUBMODULES']={}
         self.app.config['SUBMODULES']['ApplicationAPI']=ApplicationAPI(self)
         self.app.config['SUBMODULES']['DMRIAtlasbuilderAPI']=DMRIAtlasbuilderAPI(self)
         self.app.config['SUBMODULES']['DMRIPrepAPI']=DMRIPrepAPI(self)
+        self.app.config['SUBMODULES']['DMRIFiberProfile']=DMRIFiberProfileAPI(self)
 
         @self.app.route('/', defaults={'path': ''})
         @self.app.route('/<path>') ## for routers
         def catch_all(path):
             return self.app.send_static_file("index.html")
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/static/spa/spa.zip` & `dtiplayground-0.5.8b8/dtiplayground/api/static/spa/spa.zip`

 * *Format-specific differences are supported for ZIP archives but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Zip archive data, at least v1.0 to extract, compression method=store*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 504b 0304 0a00 0000 0000 846d 5d58 0000  PK.........m]X..
 00000010: 0000 0000 0000 0000 0000 0400 1c00 7370  ..............sp
-00000020: 612f 5554 0900 0377 d0e0 6577 d0e0 6575  a/UT...w..ew..eu
+00000020: 612f 5554 0900 0377 d0e0 65be 9819 6675  a/UT...w..e...fu
 00000030: 780b 0001 04b2 6800 0004 e903 0000 504b  x.....h.......PK
 00000040: 0304 1400 0000 0800 836d 5d58 d898 15d8  .........m]X....
 00000050: 97fa 0000 e3fb 0000 0f00 1c00 7370 612f  ............spa/
 00000060: 6661 7669 636f 6e2e 6963 6f55 5409 0003  favicon.icoUT...
 00000070: 76d0 e065 75d0 e065 7578 0b00 0104 b268  v..eu..eux.....h
 00000080: 0000 04e9 0300 0064 bd75 501c cdf7 3dbc  .......d.uP...=.
 00000090: bbb8 2fee 6ec1 21b8 2fee ee04 87e0 1a08  ../.n.!./.......
@@ -4014,16 +4014,16 @@
 0000fad0: ec6c 2c8c 4d63 add2 d22d cd3a 6e92 d21d  .l,.Mc...-.:n...
 0000fae0: 32ee c07a 1bc5 7376 d4eb 8b9b ab0c 5c42  2..z..sv......\B
 0000faf0: 5e07 a409 16e4 0a4c 2e4f d155 e3f4 3619  ^......L.O.U..6.
 0000fb00: dc70 17bb e7f2 3f4a e35c c782 dfb0 b000  .p....?J.\......
 0000fb10: 4f03 ae87 0a7c 59e6 ff7f b9fd ff00 504b  O....|Y.......PK
 0000fb20: 0304 0a00 0000 0000 836d 5d58 0000 0000  .........m]X....
 0000fb30: 0000 0000 0000 0000 0a00 1c00 7370 612f  ............spa/
-0000fb40: 6963 6f6e 732f 5554 0900 0376 d0e0 6577  icons/UT...v..ew
-0000fb50: d0e0 6575 780b 0001 04b2 6800 0004 e903  ..eux.....h.....
+0000fb40: 6963 6f6e 732f 5554 0900 0376 d0e0 65be  icons/UT...v..e.
+0000fb50: 9819 6675 780b 0001 04b2 6800 0004 e903  ..fux.....h.....
 0000fb60: 0000 504b 0304 0a00 0000 0000 836d 5d58  ..PK.........m]X
 0000fb70: bed7 87fc 2430 0000 2430 0000 1d00 1c00  ....$0..$0......
 0000fb80: 7370 612f 6963 6f6e 732f 6661 7669 636f  spa/icons/favico
 0000fb90: 6e2d 3132 3878 3132 382e 706e 6755 5409  n-128x128.pngUT.
 0000fba0: 0003 76d0 e065 76d0 e065 7578 0b00 0104  ..v..ev..eux....
 0000fbb0: b268 0000 04e9 0300 0089 504e 470d 0a1a  .h........PNG...
 0000fbc0: 0a00 0000 0d49 4844 5200 0000 8000 0000  .....IHDR.......
@@ -5594,15 +5594,15 @@
 00015d90: 46b0 0f17 5b41 b11b 5137 c459 e74f 687b  F...[A..Q7.Y.Oh{
 00015da0: de04 7a3a 13fb df78 f8e5 abc9 1961 0809  ..z:...x.....a..
 00015db0: 02af 4871 4d89 7aed e4f1 1bc7 da3c c1fc  ..HqM.z......<..
 00015dc0: efcd f4f8 7f31 ffb3 bab6 0dd5 cb00 0000  .....1..........
 00015dd0: 0049 454e 44ae 4260 8250 4b03 040a 0000  .IEND.B`.PK.....
 00015de0: 0000 0084 6d5d 5800 0000 0000 0000 0000  ....m]X.........
 00015df0: 0000 000b 001c 0073 7061 2f61 7373 6574  .......spa/asset
-00015e00: 732f 5554 0900 0377 d0e0 6577 d0e0 6575  s/UT...w..ew..eu
+00015e00: 732f 5554 0900 0377 d0e0 65be 9819 6675  s/UT...w..e...fu
 00015e10: 780b 0001 04b2 6800 0004 e903 0000 504b  x.....h.......PK
 00015e20: 0304 1400 0000 0800 846d 5d58 6863 2571  .........m]Xhc%q
 00015e30: 934f 0000 d44f 0000 3000 1c00 7370 612f  .O...O..0...spa/
 00015e40: 6173 7365 7473 2f4b 464f 6b43 6e71 4575  assets/KFOkCnqEu
 00015e50: 3932 4672 314d 6d67 5678 4949 7a51 2e33  92Fr1MmgVxIIzQ.3
 00015e60: 3465 3935 3832 632e 776f 6666 5554 0900  4e9582c.woffUT..
 00015e70: 0377 d0e0 6577 d0e0 6575 780b 0001 04b2  .w..ew..eux.....
```

#### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/static/spa/spa.zip` & `dtiplayground-0.5.8b8/dtiplayground/api/static/spa/spa.zip`

```diff
@@ -1,10 +1,10 @@
 00000000: 504b 0304 0a00 0000 0000 846d 5d58 0000  PK.........m]X..
 00000010: 0000 0000 0000 0000 0000 0400 1c00 7370  ..............sp
-00000020: 612f 5554 0900 0377 d0e0 6577 d0e0 6575  a/UT...w..ew..eu
+00000020: 612f 5554 0900 0377 d0e0 65be 9819 6675  a/UT...w..e...fu
 00000030: 780b 0001 04b2 6800 0004 e903 0000 504b  x.....h.......PK
 00000040: 0304 1400 0000 0800 836d 5d58 d898 15d8  .........m]X....
 00000050: 97fa 0000 e3fb 0000 0f00 1c00 7370 612f  ............spa/
 00000060: 6661 7669 636f 6e2e 6963 6f55 5409 0003  favicon.icoUT...
 00000070: 76d0 e065 75d0 e065 7578 0b00 0104 b268  v..eu..eux.....h
 00000080: 0000 04e9 0300 0064 bd75 501c cdf7 3dbc  .......d.uP...=.
 00000090: bbb8 2fee 6ec1 21b8 2fee ee04 87e0 1a08  ../.n.!./.......
@@ -4014,16 +4014,16 @@
 0000fad0: ec6c 2c8c 4d63 add2 d22d cd3a 6e92 d21d  .l,.Mc...-.:n...
 0000fae0: 32ee c07a 1bc5 7376 d4eb 8b9b ab0c 5c42  2..z..sv......\B
 0000faf0: 5e07 a409 16e4 0a4c 2e4f d155 e3f4 3619  ^......L.O.U..6.
 0000fb00: dc70 17bb e7f2 3f4a e35c c782 dfb0 b000  .p....?J.\......
 0000fb10: 4f03 ae87 0a7c 59e6 ff7f b9fd ff00 504b  O....|Y.......PK
 0000fb20: 0304 0a00 0000 0000 836d 5d58 0000 0000  .........m]X....
 0000fb30: 0000 0000 0000 0000 0a00 1c00 7370 612f  ............spa/
-0000fb40: 6963 6f6e 732f 5554 0900 0376 d0e0 6577  icons/UT...v..ew
-0000fb50: d0e0 6575 780b 0001 04b2 6800 0004 e903  ..eux.....h.....
+0000fb40: 6963 6f6e 732f 5554 0900 0376 d0e0 65be  icons/UT...v..e.
+0000fb50: 9819 6675 780b 0001 04b2 6800 0004 e903  ..fux.....h.....
 0000fb60: 0000 504b 0304 0a00 0000 0000 836d 5d58  ..PK.........m]X
 0000fb70: bed7 87fc 2430 0000 2430 0000 1d00 1c00  ....$0..$0......
 0000fb80: 7370 612f 6963 6f6e 732f 6661 7669 636f  spa/icons/favico
 0000fb90: 6e2d 3132 3878 3132 382e 706e 6755 5409  n-128x128.pngUT.
 0000fba0: 0003 76d0 e065 76d0 e065 7578 0b00 0104  ..v..ev..eux....
 0000fbb0: b268 0000 04e9 0300 0089 504e 470d 0a1a  .h........PNG...
 0000fbc0: 0a00 0000 0d49 4844 5200 0000 8000 0000  .....IHDR.......
@@ -5594,15 +5594,15 @@
 00015d90: 46b0 0f17 5b41 b11b 5137 c459 e74f 687b  F...[A..Q7.Y.Oh{
 00015da0: de04 7a3a 13fb df78 f8e5 abc9 1961 0809  ..z:...x.....a..
 00015db0: 02af 4871 4d89 7aed e4f1 1bc7 da3c c1fc  ..HqM.z......<..
 00015dc0: efcd f4f8 7f31 ffb3 bab6 0dd5 cb00 0000  .....1..........
 00015dd0: 0049 454e 44ae 4260 8250 4b03 040a 0000  .IEND.B`.PK.....
 00015de0: 0000 0084 6d5d 5800 0000 0000 0000 0000  ....m]X.........
 00015df0: 0000 000b 001c 0073 7061 2f61 7373 6574  .......spa/asset
-00015e00: 732f 5554 0900 0377 d0e0 6577 d0e0 6575  s/UT...w..ew..eu
+00015e00: 732f 5554 0900 0377 d0e0 65be 9819 6675  s/UT...w..e...fu
 00015e10: 780b 0001 04b2 6800 0004 e903 0000 504b  x.....h.......PK
 00015e20: 0304 1400 0000 0800 846d 5d58 6863 2571  .........m]Xhc%q
 00015e30: 934f 0000 d44f 0000 3000 1c00 7370 612f  .O...O..0...spa/
 00015e40: 6173 7365 7473 2f4b 464f 6b43 6e71 4575  assets/KFOkCnqEu
 00015e50: 3932 4672 314d 6d67 5678 4949 7a51 2e33  92Fr1MmgVxIIzQ.3
 00015e60: 3465 3935 3832 632e 776f 6666 5554 0900  4e9582c.woffUT..
 00015e70: 0377 d0e0 6577 d0e0 6575 780b 0001 04b2  .w..ew..eux.....
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/api/utils.py` & `dtiplayground-0.5.8b8/dtiplayground/api/utils.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/app.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/atlasbuilder.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/atlasbuilder.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/GreedyAtlasParameters.xml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/data/template.json` & `dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/data/template.json`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/atlasbuilder/utils.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/atlasbuilder/utils.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/__init__.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/__init__.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/appbase.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/appbase.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/fslinstaller.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/fslinstaller.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/fslinstaller_py2.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/fslinstaller_py2.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/data/software_paths.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/data/software_paths.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/dwi.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/dwi.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/module.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/module.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/pipeline.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
         # check the input type
         first_path = file_paths[0]
         ext = Path(first_path).suffix
         for fp in self.file_paths:
             logger("Loading Data Sheet: {}".format(str(fp)), common.Color.PROCESS)
             self.result_history[fp] = [{"output": {"file_path": str(Path(fp).absolute()),
                                                    }}]
+        if ext != '.csv':
+            raise Exception("Only csv files are supported for datasheets")
     def setOutputDirectory(self, output_dir=None):
         if output_dir is None:
             self.output_dir=Path(self.getImagePath()).parent
         else:
             self.output_dir=str(Path(output_dir).absolute())
         self.io['output_directory']=str(self.output_dir)
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/study/__init__.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/study/__init__.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/study/loaders.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/study/loaders.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/__init__.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/base.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/base.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/brainsfit.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/brainsfit.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dti_reg.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dti_reg.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtiaverage.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtiaverage.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtiprocess.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtiprocess.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/dtitractstat.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/dtitractstat.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fiberpostprocess.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fiberpostprocess.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fiberprocess.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fiberprocess.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/fsl.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/fsl.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/image_math.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/image_math.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/niral_utilities.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/niral_utilities.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/resample_dti_log_euclidean.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/common/tools/unu.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/common/tools/unu.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import os.path
+import shutil
 from pathlib import Path
 from typing import List
 
 import pandas as pd
 
 import dtiplayground.dmri.common as common
 import dtiplayground.dmri.fiberprofile as base
 from dtiplayground.dmri.common import tools
 
 logger = common.logger.write
 
-
+class CleanupMethod():
+    DURING = 'duringProcessing'
+    END = 'endOfProcessing'
+    NONE = 'noCleanup'
 class EXTRACT_Profile(base.modules.DTIFiberProfileModule):
     def __init__(self, config_dir, *args, **kwargs):
         super().__init__(config_dir)
 
     def generateDefaultProtocol(self, image_obj):
         super().generateDefaultProtocol(image_obj)
         ## todos
@@ -29,31 +34,40 @@
         protocol_options = args[0]
         self.software_info = protocol_options['software_info']['softwares']
 
         # Reading some parameters
         try:
             path_to_csv: str = inputParams["file_path"]
             output_base_dir: str = self.output_dir  # output directory string
-            atlas_path: str = self.protocol["atlas"]
-            if not isinstance(atlas_path, str):
-                raise ValueError(f"Atlas path must be a string specifying directory with tracts. Current value: {atlas_path}")
+
             tracts_string: str = self.protocol["tracts"]
             if not isinstance(tracts_string, str):
                 raise ValueError("Tracts must be a string of comma delimited tracts to profile")
-            tracts: List[str] = tracts_string.split(',')
+            tracts: List[str] = [tract.strip() for tract in tracts_string.split(',')]
+            if len(tracts) == 0:
+                raise ValueError("Tracts must be a non-empty list of tracts to profile")
+            atlas_path: str = self.protocol["atlas"]
+            if not isinstance(atlas_path, str):
+                for tract in tracts:
+                    if not os.path.isabs(tract):
+                        raise ValueError(
+                            f"Tract paths must all be absolute if no atlas path is provided. Atlas path current value: {atlas_path}. Either provide atlas dir or convert this path to absolute: {tract}")
             properties_to_profile: List[str] = [x.strip() for x in self.protocol["propertiesToProfile"].split(',')]
             result_case_columnwise: bool = self.protocol["resultCaseColumnwise"]
             input_is_dti: bool = self.protocol["inputIsDTI"]
             overwrite: bool = self.options['overwrite']
             use_displacement_field: bool = self.protocol["useDisplacementField"]
             step_size: str = str(self.protocol["stepSize"])
             plane_of_origin: str = self.protocol["planeOfOrigin"]
             support_bandwidth: str = str(self.protocol["supportBandwidth"])
             noNaN: str = self.protocol["noNaN"]
             mask: str = self.protocol["mask"]
+            cleanupMethod: str = self.protocol["cleanup"]
+            if cleanupMethod not in [CleanupMethod.DURING, CleanupMethod.NONE, CleanupMethod.END]:
+                raise ValueError(f"Invalid cleanup method: {cleanupMethod}")
         except KeyError as e:
             self.result['output']['success'] = False
             self.result['output']['error'] = f"Missing parameter {e}"
             logger(f"Missing parameter: {e}")
             exit(1)
         except ValueError as e:
             self.result['output']['success'] = False
@@ -125,16 +139,19 @@
             prop_output_path: Path = Path(output_base_dir).joinpath(prop)
             for tract in tracts:
                 # create the directory for the output for the scalar property
                 tract_name_stem: str = Path(tract).stem
                 tract_output_path: Path = prop_output_path.joinpath(tract_name_stem)
                 tract_output_path.mkdir(parents=True, exist_ok=True)
                 logger(f"Extracting profile for tract {tract}")
-                tract_absolute_filename = Path(atlas_path).joinpath(
-                    tract)  # concatenate the atlas path with the tract name
+                if tract[0] == '/': # tract is absolute path
+                    tract_absolute_filename = Path(tract)
+                else:
+                    tract_absolute_filename = Path(atlas_path).joinpath(
+                        tract)  # concatenate the atlas path with the tract name
                 # Create dataframe to track statistics for this tract
                 tract_stat_df: pd.DataFrame = None
                 for row_index, row in df.iterrows():
                     subject_id = row.iloc[0]
                     # Find path to scalar image in the dataframe
                     scalar_img_path = row[parameter_to_col_map[prop]]
                     fiberprocess_output_path: str = tract_output_path.joinpath(
@@ -165,39 +182,52 @@
                         options = []
                         if mask is not None:
                             options += ['--mask', mask]
                         if noNaN:
                             options += ['--noNan']
                         fiberpostprocess = tools.FiberPostProcess(self.software_info['fiberpostprocess']['path'])
                         fiberpostprocess.run(fiberprocess_output_path.__str__(), fiberpostprocess_output_path, options=options)
+
+                    # fiberpostprocess complete, delete the fiberprocess output
+                    if cleanupMethod == CleanupMethod.DURING:
+                        logger(f"Cleaning up fiberprocess output for subject {subject_id} and tract {tract}")
+                        Path(fiberprocess_output_path).unlink()
+
                     if Path(dtitractstat_output_path).exists() and not recompute_scalars:
                         logger(f"Skipping dtitractstat of scalar {prop} for subject {subject_id}")
                     else:
                         # run dtitractstat
                         options = ['--parameter_list', prop, '--scalarName', prop]
                         if row_index == 0:
                             logger(f"Generating parameterized fiber profile for tract {tract}")
                             tract_name_stem: str = Path(tract).stem
                             parameterized_fiber_output_path: Path = Path(parameterized_fibers_path).joinpath(
                                 tract_name_stem + "_parameterized.vtk")
                             if parameterized_fiber_output_path.exists() and not recompute_scalars:
                                 logger(f"Skipping parameterized fiber generation of tract {tract}")
                             else:
                                 logger(f"Generating parameterized fiber profile for tract {tract}")
-                                tract_absolute_filename = Path(atlas_path).joinpath(
-                                    tract)
+                                if tract[0] == '/':  # tract is absolute path
+                                    tract_absolute_filename = Path(tract)
+                                else:
+                                    tract_absolute_filename = Path(atlas_path).joinpath(
+                                        tract)  # concatenate the atlas path with the tract name
                                 options += ['-f', parameterized_fiber_output_path.__str__()]
                                 options += ['--step_size', step_size]
                                 options += ['--bandwidth', support_bandwidth]
                                 options += ['--auto_plane_origin', plane_of_origin.lower()]
+                                options += ['--remove_clean_fiber']
                                 if noNaN:
                                     options += ['--remove_nan_fibers']
                         dtitractstat = tools.DTITractStat(self.software_info['dtitractstat']['path'])
                         dtitractstat.run(fiberpostprocess_output_path, dtitractstat_output_path, options=options)
-
+                    # dtitractstat complete, delete the fiberpostprocess output
+                    if cleanupMethod == CleanupMethod.DURING:
+                        logger(f"Cleaning up fiberpostprocess output for subject {subject_id} and tract {tract}")
+                        Path(fiberpostprocess_output_path).unlink()
                     # extract fvp data
                     fvp_data = pd.read_csv(dtitractstat_output_path, skiprows=[0, 1, 2, 3])
 
                     # write fvp data to csv
                     if tract_stat_df is None:
                         if result_case_columnwise:
                             tract_stat_df = pd.DataFrame(columns=["Arc Length"])
@@ -209,15 +239,21 @@
                     if result_case_columnwise:
                         new_col = fvp_data["Parameter_Value"].tolist()
                         tract_stat_df[subject_id] = new_col
                     else:
                         new_row_list = [subject_id] + fvp_data["Parameter_Value"].tolist()
                         tract_stat_df.loc[len(tract_stat_df)] = dict(zip(tract_stat_df.columns, new_row_list))
 
+                    # dtitractstat output data stored, delete the dtitractstat file output
+                    if cleanupMethod == CleanupMethod.DURING:
+                        logger(f"Cleaning up dtitractstat output for subject {subject_id} and tract {tract}")
+                        Path(dtitractstat_output_path).unlink()
+                # save the tract_stat_df to a csv
                 tract_stat_df.to_csv(prop_output_path.joinpath(f'{tract_name_stem}_{prop}.csv'), index=False)
-
+                if cleanupMethod == CleanupMethod.END or cleanupMethod == CleanupMethod.DURING:
+                    shutil.rmtree(tract_output_path)
         self.result['output']['success'] = True
         return self.result
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/EXTRACT_Profile/EXTRACT_Profile.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: EXTRACT_Profile
 caption: EXTRACT_Profile
-description: Custom module
+description: Extract fiber tract statistics from images
 version: "0.1"
 dependency: []
 module_type: fiberprofile
 process_attributes:
     - utility
 result: null
 protocol: #define protocol parameters here
     atlas: # Not used directly. Added to beginning of each tract file path
-        type: directory
+        type: dirpath-remote
         caption: Atlas directory
         default_value: null
         description: Directory containing set of fiber tracts in the atlas to be analyzed
     tracts:
-        type: string
+        type: filepath-remote-mult
         caption: Comma delimited list of file names of tracts in atlas directory
         default_value: null
         description: Selected set of tracts to use. Must uniquely map to a VTK fiber file in the atlas location.
     inputIsDTI:
         type: boolean
         caption: Input is DTI
         default_value: true
@@ -32,15 +32,22 @@
         type: boolean
         caption: Use displacement field to transform image to atlas space
         default_value: true
         description: Convert image to atlas space using displacement field. If set to false, the image will not be transformed to atlas space.
     parameterToColumnHeaderMap: # Optional map of parameters (e.g., scalar names, case id) to column headers
         type: dictionary
         caption: Property to column header map
-        default_value: null
+        default_value:
+            Case ID: id
+            Original DTI Image: Original DTI image
+            Deformation Field: Concatenated Deformation field
+            FA: FA from original
+            MD: MD from original
+            AD: AD from original
+            RD: RD from original
         description: Map of parameters of column headers to use for each property to profile
     resultCaseColumnwise:
         type: boolean
         caption: Store cases as columns in result
         default_value: true
         description: In output CSV, store cases as columns instead of rows
     # TODO: Add support for a "per tract origin file" option where a user can specify their origins per tract in a file
@@ -52,14 +59,29 @@
               caption: Median
               description: Origin of profile will be median of tract
             - value: CoG
               caption: Center of gravity
               description: Origin of profile will be center of gravity
         default_value: Median
         description: Determines plane that sets the origin of the profile arc length
+    cleanup:
+        type: list
+        caption: Cleanup method
+        default_value: duringProcessing
+        candidates:
+            - value: duringProcessing
+              caption: During processing
+              description: Remove temporary files the moment they're no longer needed
+            - value: endOfProcessing
+              caption: End of processing
+              description: Remove temporary files after processing is complete
+            - value: noCleanup
+              caption: No cleanup
+              description: Do not remove temporary files
+        description: Remove temporary files after processing
     stepSize:
         type: integer
         caption: Step size
         default_value: 1
         description: How far long the tract to step for each new fiber profile location
     supportBandwidth:
         type: integer
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/modules/IDENTITY_Process/IDENTITY_Process.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/protocols.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/protocols.py`

 * *Files 7% similar despite different names*

```diff
@@ -119,14 +119,35 @@
             self.io = self.rawdata['io']
             self.protocol_filename = filename
             return True
         except Exception as e:
             logger("Exception occurred : {}".format(str(e)))
             traceback.print_exc()
             return False
+
+    def makeDefaultProtocols(self,pipeline=None,template=None,options={}):
+        self.checkDatasheet()
+        logger("Default protocols are being generated using image information",common.Color.PROCESS)
+        if template==None:
+            template=yaml.safe_load(open(self.template_filename,'r'))
+
+        ### generate default protocols
+        self.io={}
+        self.version=template['version']
+        for k,elm in template['options']['io'].items():
+            self.io[k]=elm['default_value']
+        if self.file_paths is not None:
+            self.io['input_datasheet']=self.file_paths[0]
+        if self.output_dir is not None:
+            self.io['output_directory']=str(self.output_dir)
+        if pipeline is not None:
+            self.pipeline=self.furnishPipeline(pipeline)
+        else:
+            self.pipeline=self.furnishPipeline(template['options']['execution']['pipeline']['default_value'])
+        logger("Default protocols are generated.",common.Color.OK)
      # Override default runPipeline method with fiberprofile specific functionality
     @common.measure_time
     def runPipeline(self,options={}): ## default is QC module (to be abstracted)
         try:
             if 'execution_id' in options: logger("Execution ID : {}".format(options['execution_id']))
             logger(str(options),common.Color.DEV)
             self.checkRunnable()
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/module_template.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/fiberprofile/templates/protocol_template.yml`

 * *Files 21% similar despite different names*

```diff
@@ -11,43 +11,64 @@
 ##  Written by SK Park, NIRAL, UNC SOM, 2022
 
 version: 0.1
 options:
 
   ### Template metadata
   system:
-    available_types: 
+    available_types:
       - boolean
       - integer
       - float
       - string
       - file
-      - directory 
+      - directory
       - list
       - queue
       - matrix
-      - object-array 
+      - object-array
 
   ### settings template
   settings: null # TBD
 
   ### io template
   io:
-    output_directory: 
-      type: directory # file dialog for ui
+    input_datasheet:
+      type: filepath-remote # file dialog for ui
+      caption: Input Data Sheet
+      default_value: null
+      description: Input data sheet containing file paths for the tensor/scalar images and deformation fields
+    output_directory:
+      type: dirpath-remote # file dialog for ui
       caption: Output Directory
       default_value: null
-      description: Output directory storing the results and generated files 
+      description: Output directory storing the results and generated files
     output_filename_base:
       type: string
       default_value: null
       caption: Output basename
       description: Final output base name
+    num_threads:
+      type: number
+      caption: Number of Threads to Use
+      default_value: 1
+      description: Number of threads to use for the process
   #### Execution related
   execution:
+    options:
+      overwrite:
+        type: boolean
+        caption: Overwrite
+        default_value: false
+        description: Overwrite the files
+      skip:
+        type: boolean
+        caption: Skip This Module
+        default_value: false
+        description: Skip this module and pass the data to the next module
     pipeline:
       type: queue
       caption: Pipeline Queue
       candidates: ## add elements from below list, each one is a key for a protocol
         - value: IDENTITY_Process
           caption: Identity Process
           description: Just pass image to the next module
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/playground/app.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/playground/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/app.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/app.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/data/software_paths.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/data/software_paths.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/BASELINE_Average.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BASELINE_Average/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,20 +27,27 @@
         # << TODOS>>
         protocol_options=args[0]
         self.num_threads=protocol_options['software_info']['parameters']['num_max_threads']
         self.software_info=protocol_options['software_info']['softwares']
         self.baseline_threshold=protocol_options['baseline_threshold']
         res=self.run_mask(method=self.protocol['method'],
                           #modality=self.protocol['modality'],
-                          averagingMethod=self.protocol['averagingMethod'])
+                          averagingMethod=self.protocol['averagingMethod'],
+                          customMaskPath=self.protocol['customMaskPath'])
         self.result['output']['success']=True
         return self.result
         
 
 ### User defined methods
+    
+    def verify_path(self, file_path):
+        if len(file_path) > 0 and file_path and Path(file_path).exists():
+            return True
+        else: return False
+
     def mask_antspynet(self,params):
         import ants 
         import antspynet
         logger("AntsPyNet is running ...",prep.Color.INFO)
         res=None
         input_image_path=Path(self.output_dir).joinpath("input.nii.gz").__str__()
         output_mask_path=Path(self.output_dir).joinpath("mask.nii.gz").__str__()
@@ -123,15 +130,39 @@
         mask.writeImage(output_mask_path_nrrd,dest_type='nrrd')
         self.addOutputFile(output_mask_path, 'Mask')
         self.addOutputFile(output_mask_path_nrrd, 'Mask')
         self.addGlobalVariable('mask_path',output_mask_path_nrrd)
         res=None
         return res
 
-    def run_mask(self, method, averagingMethod): #run_mask(self,method, modality,averagingMethod)
+    def custom_mask(self, params):
+        logger("Custom Mask is running ...",prep.Color.INFO)
+        input_image_base=Path(self.output_dir).joinpath("input").__str__()
+        output_image_base=Path(self.output_dir).joinpath("mask").__str__()
+
+        input_image_path=input_image_base+".nii.gz"
+        output_mask_path=output_image_base+".nii.gz"
+        output_mask_path_nrrd=output_image_base+".nrrd"
+        src_image=params['image']
+        custom_mask_path=params['customMaskPath']
+        if not self.verify_path(custom_mask_path):
+            logger("Mask path cannot be verified",prep.Color.ERROR)
+            return False
+        src_image.writeImage(input_image_path,dest_type='nifti')
+        mask=DWI(custom_mask_path)
+        mask.setSpaceDirection(self.getSourceImageInformation()['space'])
+        mask.writeImage(output_mask_path_nrrd,dest_type='nrrd')
+        mask.writeImage(output_mask_path,dest_type='nifti')
+        self.addOutputFile(output_mask_path, 'Mask')
+        self.addOutputFile(output_mask_path_nrrd, 'Mask')
+        self.addGlobalVariable('mask_path',output_mask_path_nrrd)
+        res=None
+        return res
+
+    def run_mask(self, method, averagingMethod, customMaskPath):
         res=None 
         params={}
         logger("Mask is being computed ... ",prep.Color.PROCESS)
         if method=='fsl':
             params={
                 'image': self.image,
                 'averagingMethod': averagingMethod
@@ -140,11 +171,17 @@
         elif method=='antspynet':
             params={
                 'image': self.image,
                 #'modality': modality,
                 'averagingMethod': averagingMethod
             }
             res=self.mask_antspynet(params)
+        elif method=='customMask':
+            params={
+                'image': self.image,
+                'customMaskPath': customMaskPath
+            }
+            res=self.custom_mask(params)
         logger("Mask generation is completed",prep.Color.OK)
         return res
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/BRAIN_Mask.yml`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,18 @@
         caption: Method
         candidates:
           - value: fsl
             caption: FSL
             description: Use FSL for Brainmasking
           # - value: antspynet
           #   caption: AntsPyNet
-          #   description: AntsPyNet's brain_extraction() method 
+          #   description: AntsPyNet's brain_extraction() method
+          - value: customMask
+            caption: Custom Brain Mask
+            description: Use custom Brainmasking
         default_value: fsl
         description: Method to extract the brain 
       averagingMethod:
         type: list
         caption: Average Method
         default_value: idwi
         description: Averaging method by which the source image is generated for the mask
@@ -39,7 +42,13 @@
             caption: T2
             description: T2 Modality 
           - value: fa
             caption: FA
             description: Fractional Anistropy
         default_value: t2
         description: Modality of the input image
+      customMaskPath: 
+        type: filepath-remote
+        caption: Custom Brain Mask
+        default_value: 
+        description: Provide custom mask to override default
+        if : { "method" : "customMask" }
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Mask/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/BRAIN_Tractography.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/BRAIN_Tractography/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,21 @@
                 logger('Mask not found, estimating whole image...',prep.Color.WARNING)
         else:
             logger('Mask not found, estimating whole image...',prep.Color.WARNING)
         # fitting and estimation of scalars
         dti_fit = dti.TensorModel(gtab,fit_method=fitMethod,**kwargs)
         logger("Running with {}, {}".format(fitMethod, kwargs),prep.Color.PROCESS)
         #fitted = dti_fit.fit(data) ## dti_fit.fit(data, mask) mask array (boolean)
-        fitted = dti_fit.fit(data,mask)
-        logger("Fitting completed",prep.Color.OK)
+        try:
+            fitted = dti_fit.fit(data,mask)
+            logger("Fitting completed",prep.Color.OK)
+        except ValueError as e:
+            logger("Mask is not the same shape as data.",prep.Color.ERROR)
+            raise ValueError
+
 
         ## convert 3x3 symmetric matrices to xx,xy,xz,yy,yz,zz vectors
         logger("Reducing 3x3 symmetric matrix to vector")
         def uppertriangle(matrix):
             outvec=[]
             for i in range(3):
                 for j in range(i,3):
```

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/DTI_Estimate.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Estimate/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/DTI_Register.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/DTI_Register/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/EDDYMOTION_Correct.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/EDDYMOTION_Correct/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IDENTITY_Process/IDENTITY_Process.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/IMAGE_Filter.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/IMAGE_Filter/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/INTERLACE_Check.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/INTERLACE_Check/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/MANUAL_Exclude/MANUAL_Exclude.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/QC_Report/QC_Report.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SLICE_Check/SLICE_Check.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/README.md`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/SUSCEPTIBILITY_Correct.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/SUSCEPTIBILITY_Correct/data/fsl_regb02b0.cnf`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/modules/UTIL_Merge/UTIL_Merge.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/protocols.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/module_template.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/preprocessing/templates/protocol_template.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/preprocessing/templates/protocol_template.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/protocols.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/protocols.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/module_template.py` & `dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/module_template.py`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/dtiplayground/dmri/tractography/templates/protocol_template.yml` & `dtiplayground-0.5.8b8/dtiplayground/dmri/tractography/templates/protocol_template.yml`

 * *Files identical despite different names*

### Comparing `dtiplayground-0.5.8b7/setup.py` & `dtiplayground-0.5.8b8/setup.py`

 * *Files identical despite different names*

