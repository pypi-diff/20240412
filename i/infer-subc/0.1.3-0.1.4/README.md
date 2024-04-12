# Comparing `tmp/infer-subc-0.1.3.tar.gz` & `tmp/infer-subc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infer-subc-0.1.3.tar", last modified: Thu Apr  4 18:10:38 2024, max compression
+gzip compressed data, was "infer-subc-0.1.4.tar", last modified: Fri Apr 12 14:40:39 2024, max compression
```

## Comparing `infer-subc-0.1.3.tar` & `infer-subc-0.1.4.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.142079 infer-subc-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.086079 infer-subc-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.090079 infer-subc-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-04 18:10:33.000000 infer-subc-0.1.3/.github/workflows/ci.yml.disable
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-04 18:10:33.000000 infer-subc-0.1.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-04 18:10:33.000000 infer-subc-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-04 18:10:33.000000 infer-subc-0.1.3/20230221_MSI_3Dmeasurements.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-04 18:10:33.000000 infer-subc-0.1.3/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-04 18:10:33.000000 infer-subc-0.1.3/ABOUT_THIS_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-04 18:10:33.000000 infer-subc-0.1.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-04 18:10:33.000000 infer-subc-0.1.3/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-04 18:10:33.000000 infer-subc-0.1.3/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-04 18:10:33.000000 infer-subc-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 18:10:33.000000 infer-subc-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-04 18:10:33.000000 infer-subc-0.1.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-04 18:10:38.142079 infer-subc-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-04 18:10:33.000000 infer-subc-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/config.md
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/framework.md
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/infer_subc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/infer_subc/core/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/core/file_io.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/core/img.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/infer_subc/napari/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/napari/organelle_config.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/napari/plugin.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/infer_subc/organelles/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/cellmask.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/cytoplasm.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/er.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/golgi.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/lipid.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/lysosome.md
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/mitochondria.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/nuclei.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles/peroxisome.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/organelles.md
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/infer_subc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/utils/batch.md
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/utils/etc.md
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/utils/stats.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/utils/utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/infer_subc/workflow.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.094079 infer-subc-0.1.3/docs/nbs/
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/nbs/overview.md
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 18:10:33.000000 infer-subc-0.1.3/docs/pipeline.md
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-04 18:10:33.000000 infer-subc-0.1.3/env_create.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.098079 infer-subc-0.1.3/infer_subc/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 18:10:37.000000 infer-subc-0.1.3/infer_subc/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.098079 infer-subc-0.1.3/infer_subc/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/core/file_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    44069 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/core/img.py
--rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/core/zslice.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.098079 infer-subc-0.1.3/infer_subc/organelles/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/cellmask.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/cytoplasm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/er.py
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/golgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/lipid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/lysosome.py
--rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/membrane.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/mitochondria.py
--rw-r--r--   0 runner    (1001) docker     (127)    13732 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/nuclei.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/peroxisome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles/qc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.102079 infer-subc-0.1.3/infer_subc/organelles_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74584 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/all_functions.json
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks.json
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_A.json
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_B.json
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_C.json
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_D.json
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.2.lyso.json
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.3.mito.json
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.4.golgi.json
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.5.perox.json
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.6.ER.json
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/conf_0.7.LD.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.106079 infer-subc-0.1.3/infer_subc/organelles_config/depricate/
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/infer_nuclei.json
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/infer_soma.json
--rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/og_all_functions.json
--rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/depricate/test_functions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/function_guide.md
--rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/function_params.md
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/organelles_config/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.106079 infer-subc-0.1.3/infer_subc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/_aicsimage_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)    82781 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    65577 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/utils/stats_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.106079 infer-subc-0.1.3/infer_subc/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/batch_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/segmenter_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/workflow_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/workflow_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/workflow_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-04 18:10:33.000000 infer-subc-0.1.3/infer_subc/workflow/workflow_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.142079 infer-subc-0.1.3/infer_subc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-04 18:10:37.000000 infer-subc-0.1.3/infer_subc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-04 18:10:38.000000 infer-subc-0.1.3/infer_subc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 18:10:37.000000 infer-subc-0.1.3/infer_subc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 18:10:37.000000 infer-subc-0.1.3/infer_subc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 18:10:37.000000 infer-subc-0.1.3/infer_subc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-04 18:10:33.000000 infer-subc-0.1.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.134079 infer-subc-0.1.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/00.0_framework_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/00.1_pipeline_setup.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    37131 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/01_B_infer_masks_from-composite_multiple-cells.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1584253 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/01_infer_nuclei_from-label.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    85913 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/01a_infer_cytoplasm_from-composite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    72544 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    46033 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/02a_infer_nucleus_from-cytoplasm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/02b_infer_cellmask_from-membrane.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    52882 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/03_infer_cytoplasm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44996 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/03a_infer_cellmask_from-cytoplasm.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    67155 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/04_infer_neurites_soma_from-cellmask.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   685988 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/05_infer_lysosome.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   715292 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/06_infer_mitochondria.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   159659 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/07_infer_golgi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   412905 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/08_infer_peroxisome.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   313176 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/09_infer_ER.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   266369 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/10_infer_lipid_droplet.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    66928 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.1_individual_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   468409 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.1_organelle_morphology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1191024 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.2_cell_region_morphology.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  3168006 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.3_distribution_measurements.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   155099 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.4_organelle_contacts.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   176046 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11.5_combined_measurements_function.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1374535 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/11_regionprops.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/12_batch_process.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    85559 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/13_fn_prototypes_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    89112 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/14_workflow_defs_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  6995353 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/15.1_quantification_summary.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    45690 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/15_final_workflow.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   119964 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/seg-qualitycheck_running-quant.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.138079 infer-subc-0.1.3/notebooks/todelete/
--rw-r--r--   0 runner    (1001) docker     (127)    16278 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/00.1_pipeline_setup_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/00.2_extract_optimal_Z.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    53320 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/01_infer_nuclei_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    67064 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/02_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    66972 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/02a_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    67033 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/02b_infer_neurites_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    67027 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/02c_infer_wholecell_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    86025 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/03_infer_cytosol_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   121185 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/04_infer_lysosome_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   154818 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/05_infer_mitochondria_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    96854 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/06_infer_golgi_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    92224 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/07_infer_peroxisome_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   126036 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   127295 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/09_infer_lipid_body_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   415241 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/10_batch_process_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   345416 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/10_batch_process_3Dv2.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    70614 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/999_fn_prototypes_json.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/A_spectral_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/_centrosome_routines.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/_graveyard.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    73532 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/new02a_infer_soma_3D.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   478607 2024-04-04 18:10:33.000000 infer-subc-0.1.3/notebooks/todelete/test_soma_seg.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-04 18:10:33.000000 infer-subc-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-04 18:10:33.000000 infer-subc-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 18:10:38.142079 infer-subc-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-04 18:10:33.000000 infer-subc-0.1.3/test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:38.142079 infer-subc-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 18:10:33.000000 infer-subc-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 18:10:33.000000 infer-subc-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 18:10:33.000000 infer-subc-0.1.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-04 18:10:33.000000 infer-subc-0.1.3/windows_notes.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.596498 infer-subc-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.544498 infer-subc-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.548498 infer-subc-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-12 14:40:34.000000 infer-subc-0.1.4/.github/workflows/ci.yml.disable
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-12 14:40:34.000000 infer-subc-0.1.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-12 14:40:34.000000 infer-subc-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-12 14:40:34.000000 infer-subc-0.1.4/20230221_MSI_3Dmeasurements.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-12 14:40:34.000000 infer-subc-0.1.4/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-12 14:40:34.000000 infer-subc-0.1.4/ABOUT_THIS_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-12 14:40:34.000000 infer-subc-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 14:40:34.000000 infer-subc-0.1.4/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 14:40:34.000000 infer-subc-0.1.4/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-12 14:40:34.000000 infer-subc-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 14:40:34.000000 infer-subc-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-12 14:40:34.000000 infer-subc-0.1.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-12 14:40:39.596498 infer-subc-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-12 14:40:34.000000 infer-subc-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.548498 infer-subc-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/framework.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.548498 infer-subc-0.1.4/docs/infer_subc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.548498 infer-subc-0.1.4/docs/infer_subc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/core/file_io.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/core/img.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.548498 infer-subc-0.1.4/docs/infer_subc/napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/napari/organelle_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/napari/plugin.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.552498 infer-subc-0.1.4/docs/infer_subc/organelles/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/cellmask.md
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/cytoplasm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/er.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/golgi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/lipid.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/lysosome.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/mitochondria.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/nuclei.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles/peroxisome.md
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/organelles.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.552498 infer-subc-0.1.4/docs/infer_subc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/utils/batch.md
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/utils/etc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/utils/stats.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/utils/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/infer_subc/workflow.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.552498 infer-subc-0.1.4/docs/nbs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/nbs/overview.md
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-12 14:40:34.000000 infer-subc-0.1.4/docs/pipeline.md
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-12 14:40:34.000000 infer-subc-0.1.4/env_create.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.552498 infer-subc-0.1.4/infer_subc/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.552498 infer-subc-0.1.4/infer_subc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16837 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/core/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44069 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/core/img.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3062 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/core/zslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.556498 infer-subc-0.1.4/infer_subc/organelles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/cellmask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/cytoplasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6954 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/er.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/golgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/lipid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/lysosome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/membrane.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/mitochondria.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13732 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/nuclei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/peroxisome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles/qc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.560498 infer-subc-0.1.4/infer_subc/organelles_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74599 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/all_functions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_C.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_D.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.2.lyso.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.3.mito.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.4.golgi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.5.perox.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.6.ER.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/conf_0.7.LD.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.560498 infer-subc-0.1.4/infer_subc/organelles_config/depricate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/infer_nuclei.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/infer_soma.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18306 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/og_all_functions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18237 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/depricate/test_functions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/function_guide.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17259 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/function_params.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/organelles_config/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.564498 infer-subc-0.1.4/infer_subc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/_aicsimage_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10483 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82781 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65577 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/utils/stats_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.564498 infer-subc-0.1.4/infer_subc/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10350 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/batch_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/segmenter_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/workflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/workflow_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8127 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/workflow_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-12 14:40:34.000000 infer-subc-0.1.4/infer_subc/workflow/workflow_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.596498 infer-subc-0.1.4/infer_subc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 14:40:39.000000 infer-subc-0.1.4/infer_subc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-12 14:40:34.000000 infer-subc-0.1.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.588498 infer-subc-0.1.4/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/00.0_framework_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/00.1_pipeline_setup.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    37131 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/01_B_infer_masks_from-composite_multiple-cells.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1584253 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/01_infer_nuclei_from-label.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    85913 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/01a_infer_cytoplasm_from-composite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    72544 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    46033 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/02a_infer_nucleus_from-cytoplasm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8490 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/02b_infer_cellmask_from-membrane.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    52882 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/03_infer_cytoplasm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44996 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/03a_infer_cellmask_from-cytoplasm.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67155 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/04_infer_neurites_soma_from-cellmask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   685988 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/05_infer_lysosome.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   715292 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/06_infer_mitochondria.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   159659 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/07_infer_golgi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   412905 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/08_infer_peroxisome.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   313176 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/09_infer_ER.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   266369 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/10_infer_lipid_droplet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    66928 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.1_individual_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   468409 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.1_organelle_morphology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1191024 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.2_cell_region_morphology.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3168006 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.3_distribution_measurements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   155099 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.4_organelle_contacts.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   176046 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11.5_combined_measurements_function.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1374535 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/11_regionprops.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14696 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/12_batch_process.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    85559 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/13_fn_prototypes_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    89112 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/14_workflow_defs_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  6995353 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/15.1_quantification_summary.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    45690 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/15_final_workflow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   119964 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/seg-qualitycheck_running-quant.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.596498 infer-subc-0.1.4/notebooks/todelete/
+-rw-r--r--   0 runner    (1001) docker     (127)    16278 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/00.1_pipeline_setup_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/00.2_extract_optimal_Z.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    53320 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/01_infer_nuclei_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67064 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/02_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    66972 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/02a_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67033 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/02b_infer_neurites_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    67027 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/02c_infer_wholecell_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    86025 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/03_infer_cytosol_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   121185 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/04_infer_lysosome_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   154818 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/05_infer_mitochondria_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    96854 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/06_infer_golgi_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    92224 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/07_infer_peroxisome_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   126036 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   127295 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/09_infer_lipid_body_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   415241 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/10_batch_process_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   345416 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/10_batch_process_3Dv2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    70614 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/999_fn_prototypes_json.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/A_spectral_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/_centrosome_routines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/_graveyard.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    73532 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/new02a_infer_soma_3D.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   478607 2024-04-12 14:40:34.000000 infer-subc-0.1.4/notebooks/todelete/test_soma_seg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 14:40:34.000000 infer-subc-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-12 14:40:34.000000 infer-subc-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:40:39.596498 infer-subc-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 14:40:34.000000 infer-subc-0.1.4/test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:39.596498 infer-subc-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:40:34.000000 infer-subc-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-12 14:40:34.000000 infer-subc-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-12 14:40:34.000000 infer-subc-0.1.4/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-12 14:40:34.000000 infer-subc-0.1.4/windows_notes.md
```

### Comparing `infer-subc-0.1.3/.github/workflows/ci.yml.disable` & `infer-subc-0.1.4/.github/workflows/ci.yml.disable`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/.github/workflows/publish.yml` & `infer-subc-0.1.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/.gitignore` & `infer-subc-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/20230221_MSI_3Dmeasurements.csv` & `infer-subc-0.1.4/20230221_MSI_3Dmeasurements.csv`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx` & `infer-subc-0.1.4/202303063_MCZ-SR_3Dmeasurement-prioritylist.xlsx`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/ABOUT_THIS_TEMPLATE.md` & `infer-subc-0.1.4/ABOUT_THIS_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/CONTRIBUTING.md` & `infer-subc-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/LICENSE` & `infer-subc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/Makefile` & `infer-subc-0.1.4/Makefile`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/PKG-INFO` & `infer-subc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infer-subc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A plugin that enables organelle segmentation
 Author-email: Andy Henrie <ergonyc@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `infer-subc-0.1.3/README.md` & `infer-subc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/config.md` & `infer-subc-0.1.4/docs/config.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/framework.md` & `infer-subc-0.1.4/docs/framework.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/index.md` & `infer-subc-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/infer_subc/organelles.md` & `infer-subc-0.1.4/docs/infer_subc/organelles.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/infer_subc/overview.md` & `infer-subc-0.1.4/docs/infer_subc/overview.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/infer_subc/workflow.md` & `infer-subc-0.1.4/docs/infer_subc/workflow.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/nbs/overview.md` & `infer-subc-0.1.4/docs/nbs/overview.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/docs/pipeline.md` & `infer-subc-0.1.4/docs/pipeline.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/__init__.py` & `infer-subc-0.1.4/infer_subc/__init__.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/cli.py` & `infer-subc-0.1.4/infer_subc/cli.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/core/file_io.py` & `infer-subc-0.1.4/infer_subc/core/file_io.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/core/img.py` & `infer-subc-0.1.4/infer_subc/core/img.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/core/zslice.py` & `infer-subc-0.1.4/infer_subc/core/zslice.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/__init__.py` & `infer-subc-0.1.4/infer_subc/organelles/__init__.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/cellmask.py` & `infer-subc-0.1.4/infer_subc/organelles/cellmask.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/cytoplasm.py` & `infer-subc-0.1.4/infer_subc/organelles/cytoplasm.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/er.py` & `infer-subc-0.1.4/infer_subc/organelles/er.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/golgi.py` & `infer-subc-0.1.4/infer_subc/organelles/golgi.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/lipid.py` & `infer-subc-0.1.4/infer_subc/organelles/lipid.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/lysosome.py` & `infer-subc-0.1.4/infer_subc/organelles/lysosome.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/membrane.py` & `infer-subc-0.1.4/infer_subc/organelles/membrane.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,19 +231,21 @@
                                      method=Watershed_Method)
     cm_B = masked_inverted_watershed(raw_img_B, 
                                      choose_nuc, 
                                      thresh_img_B,
                                      method=Watershed_Method)
     
     cm_combo = cm_A.astype(bool) + cm_B.astype(bool)
-    out_img = close_and_fill(in_img=cm_combo,
+    cm_out = close_and_fill(in_img=cm_combo,
                              Min_Hole_Width=Min_Hole_Width,
                              Max_Hole_Width=Max_Hole_Width,
                              Method=Method,
                              Size=Size)
+    
+    out_img = np.stack([nuc, cm_out], axis=0)
 
     return out_img
 
 def invert_pm_watershed(raw_img: np.ndarray, nuc_labels: np.ndarray, PM_Channel: int, Method: str):
     pm_img = select_channel_from_raw(raw_img, PM_Channel)
     invert_pm_img = abs(np.max(pm_img) - pm_img)
     out_img = masked_inverted_watershed(img_in=min_max_intensity_normalization(invert_pm_img),
```

### Comparing `infer-subc-0.1.3/infer_subc/organelles/mitochondria.py` & `infer-subc-0.1.4/infer_subc/organelles/mitochondria.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/nuclei.py` & `infer-subc-0.1.4/infer_subc/organelles/nuclei.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/peroxisome.py` & `infer-subc-0.1.4/infer_subc/organelles/peroxisome.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles/qc.py` & `infer-subc-0.1.4/infer_subc/organelles/qc.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/all_functions.json` & `infer-subc-0.1.4/infer_subc/organelles_config/all_functions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999633773964131%*

 * *Differences: {"'double_watershed_closing'": "{'parameters': {'Min_Hole_Width': {'max': 10000}, "*

 * *                               "'Max_Hole_Width': {'max': 10000}}}",*

 * * "'fill_filter_and_mix_nuc'": "{'parameters': {'Min_Hole_Width': {'max': 1000}, 'Max_Hole_Width': "*

 * *                              "{'max': 1000}}}",*

 * * "'find_nuc'": "{'parameters': {'Min_Hole_Width': {'max': 1000}, 'Max_Hole_Width': {'max': 1000}}}",*

 * * "'masked_object_thresh_bind_pm'": "{'parameters': {'Thresh_Adj': {'max': 10}}}"}*

```diff
@@ -284,15 +284,15 @@
     },
     "double_watershed_closing": {
         "name": "Watershed for cellmask",
         "parameters": {
             "Max_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 10000,
                 "min": 4,
                 "widget_type": "slider"
             },
             "Method": {
                 "data_type": "str",
                 "options": [
                     "Ball",
@@ -300,15 +300,15 @@
                     "None"
                 ],
                 "widget_type": "drop-down"
             },
             "Min_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 10000,
                 "min": 0,
                 "widget_type": "slider"
             },
             "Size": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 25,
@@ -524,15 +524,15 @@
     },
     "fill_filter_and_mix_nuc": {
         "name": "Combine nucleus and thresh and fill holes",
         "parameters": {
             "Max_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 1000,
                 "min": 4,
                 "widget_type": "slider"
             },
             "Method": {
                 "data_type": "str",
                 "options": [
                     "Ball",
@@ -540,15 +540,15 @@
                     "None"
                 ],
                 "widget_type": "drop-down"
             },
             "Min_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 1000,
                 "min": 0,
                 "widget_type": "slider"
             },
             "Size": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 25,
@@ -589,29 +589,29 @@
                 "max": 15.0,
                 "min": 0,
                 "widget_type": "slider"
             },
             "Max_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 1000,
                 "min": 4,
                 "widget_type": "slider"
             },
             "Median_Size": {
                 "data_type": "int",
                 "increment": 1,
                 "max": 15,
                 "min": 0,
                 "widget_type": "slider"
             },
             "Min_Hole_Width": {
                 "data_type": "int",
                 "increment": 1,
-                "max": 40,
+                "max": 1000,
                 "min": 0,
                 "widget_type": "slider"
             },
             "Nuc_Channel": {
                 "data_type": "int",
                 "options": [
                     0,
@@ -1769,15 +1769,15 @@
                     9
                 ],
                 "widget_type": "drop-down"
             },
             "Thresh_Adj": {
                 "data_type": "float",
                 "increment": 0.1,
-                "max": 5,
+                "max": 10,
                 "min": 0,
                 "widget_type": "slider"
             }
         },
         "python::function": "masked_object_thresh_bind_pm",
         "python::module": "infer_subc.organelles.membrane"
     },
```

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_A.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_A.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_B.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_B.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_C.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_C.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.1.masks_D.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.1.masks_D.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'5'": "OrderedDict([('category', 'export'), ('function', 'stack_layers'), ('parameter_values', "*

 * *        "None), ('parent', [2, 4]), ('annotation', 'stacks nuclei and cellmask for batch "*

 * *        "processing and export')])"}*

```diff
@@ -56,9 +56,19 @@
         "function": "choose_cell",
         "parameter_values": null,
         "parent": [
             1,
             2,
             3
         ]
+    },
+    "5": {
+        "annotation": "stacks nuclei and cellmask for batch processing and export",
+        "category": "export",
+        "function": "stack_layers",
+        "parameter_values": null,
+        "parent": [
+            2,
+            4
+        ]
     }
 }
```

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.2.lyso.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.2.lyso.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.3.mito.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.3.mito.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.4.golgi.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.4.golgi.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.5.perox.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.5.perox.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.6.ER.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.6.ER.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/conf_0.7.LD.json` & `infer-subc-0.1.4/infer_subc/organelles_config/conf_0.7.LD.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.1.soma_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.2.nuclei_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.3.cytosol_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.4.lysosome_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.5.mitochondria_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.6.golgi_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.7.peroxisome_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.8.er_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_1.9.lipid_stepbystep_from_raw.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_2.1.soma_stepbystep.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_2.2.nuclei_stepbystep.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/conf_infer_fixed_infer_organelles_batch2.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/infer_nuclei.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/infer_nuclei.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/infer_soma.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/infer_soma.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/og_all_functions.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/og_all_functions.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/depricate/test_functions.json` & `infer-subc-0.1.4/infer_subc/organelles_config/depricate/test_functions.json`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/function_guide.md` & `infer-subc-0.1.4/infer_subc/organelles_config/function_guide.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/function_params.md` & `infer-subc-0.1.4/infer_subc/organelles_config/function_params.md`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/organelles_config/helper.py` & `infer-subc-0.1.4/infer_subc/organelles_config/helper.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/utils/_aicsimage_reader.py` & `infer-subc-0.1.4/infer_subc/utils/_aicsimage_reader.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/utils/batch.py` & `infer-subc-0.1.4/infer_subc/utils/batch.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/utils/directories.py` & `infer-subc-0.1.4/infer_subc/utils/directories.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/utils/stats.py` & `infer-subc-0.1.4/infer_subc/utils/stats.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/utils/stats_helpers.py` & `infer-subc-0.1.4/infer_subc/utils/stats_helpers.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/batch_workflow.py` & `infer-subc-0.1.4/infer_subc/workflow/batch_workflow.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/segmenter_function.py` & `infer-subc-0.1.4/infer_subc/workflow/segmenter_function.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/workflow.py` & `infer-subc-0.1.4/infer_subc/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/workflow_config.py` & `infer-subc-0.1.4/infer_subc/workflow/workflow_config.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/workflow_definition.py` & `infer-subc-0.1.4/infer_subc/workflow/workflow_definition.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/workflow_engine.py` & `infer-subc-0.1.4/infer_subc/workflow/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc/workflow/workflow_step.py` & `infer-subc-0.1.4/infer_subc/workflow/workflow_step.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/infer_subc.egg-info/PKG-INFO` & `infer-subc-0.1.4/infer_subc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infer-subc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A plugin that enables organelle segmentation
 Author-email: Andy Henrie <ergonyc@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
```

### Comparing `infer-subc-0.1.3/infer_subc.egg-info/SOURCES.txt` & `infer-subc-0.1.4/infer_subc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/mkdocs.yml` & `infer-subc-0.1.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/00.0_framework_overview.ipynb` & `infer-subc-0.1.4/notebooks/00.0_framework_overview.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/00.1_pipeline_setup.ipynb` & `infer-subc-0.1.4/notebooks/00.1_pipeline_setup.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/01_B_infer_masks_from-composite_multiple-cells.ipynb` & `infer-subc-0.1.4/notebooks/01_B_infer_masks_from-composite_multiple-cells.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/01_infer_nuclei_from-label.ipynb` & `infer-subc-0.1.4/notebooks/01_infer_nuclei_from-label.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/01a_infer_cytoplasm_from-composite.ipynb` & `infer-subc-0.1.4/notebooks/01a_infer_cytoplasm_from-composite.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb` & `infer-subc-0.1.4/notebooks/02_infer_cellmask_from-composite_with-nuclei.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/02a_infer_nucleus_from-cytoplasm.ipynb` & `infer-subc-0.1.4/notebooks/02a_infer_nucleus_from-cytoplasm.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/02b_infer_cellmask_from-membrane.ipynb` & `infer-subc-0.1.4/notebooks/02b_infer_cellmask_from-membrane.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/03_infer_cytoplasm.ipynb` & `infer-subc-0.1.4/notebooks/03_infer_cytoplasm.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/03a_infer_cellmask_from-cytoplasm.ipynb` & `infer-subc-0.1.4/notebooks/03a_infer_cellmask_from-cytoplasm.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/04_infer_neurites_soma_from-cellmask.ipynb` & `infer-subc-0.1.4/notebooks/04_infer_neurites_soma_from-cellmask.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/05_infer_lysosome.ipynb` & `infer-subc-0.1.4/notebooks/05_infer_lysosome.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/06_infer_mitochondria.ipynb` & `infer-subc-0.1.4/notebooks/06_infer_mitochondria.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/07_infer_golgi.ipynb` & `infer-subc-0.1.4/notebooks/07_infer_golgi.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/08_infer_peroxisome.ipynb` & `infer-subc-0.1.4/notebooks/08_infer_peroxisome.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/09_infer_ER.ipynb` & `infer-subc-0.1.4/notebooks/09_infer_ER.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/10_infer_lipid_droplet.ipynb` & `infer-subc-0.1.4/notebooks/10_infer_lipid_droplet.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.1_individual_measurements.ipynb` & `infer-subc-0.1.4/notebooks/11.1_individual_measurements.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.1_organelle_morphology.ipynb` & `infer-subc-0.1.4/notebooks/11.1_organelle_morphology.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.2_cell_region_morphology.ipynb` & `infer-subc-0.1.4/notebooks/11.2_cell_region_morphology.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.3_distribution_measurements.ipynb` & `infer-subc-0.1.4/notebooks/11.3_distribution_measurements.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.4_organelle_contacts.ipynb` & `infer-subc-0.1.4/notebooks/11.4_organelle_contacts.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11.5_combined_measurements_function.ipynb` & `infer-subc-0.1.4/notebooks/11.5_combined_measurements_function.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/11_regionprops.ipynb` & `infer-subc-0.1.4/notebooks/11_regionprops.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/12_batch_process.ipynb` & `infer-subc-0.1.4/notebooks/12_batch_process.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/13_fn_prototypes_json.ipynb` & `infer-subc-0.1.4/notebooks/13_fn_prototypes_json.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/14_workflow_defs_json.ipynb` & `infer-subc-0.1.4/notebooks/14_workflow_defs_json.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/15.1_quantification_summary.ipynb` & `infer-subc-0.1.4/notebooks/15.1_quantification_summary.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/15_final_workflow.ipynb` & `infer-subc-0.1.4/notebooks/15_final_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/seg-qualitycheck_running-quant.ipynb` & `infer-subc-0.1.4/notebooks/seg-qualitycheck_running-quant.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/00.1_pipeline_setup_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/00.1_pipeline_setup_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/00.2_extract_optimal_Z.ipynb` & `infer-subc-0.1.4/notebooks/todelete/00.2_extract_optimal_Z.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/01_infer_nuclei_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/01_infer_nuclei_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/02_infer_soma_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/02_infer_soma_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/02a_infer_soma_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/02a_infer_soma_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/02b_infer_neurites_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/02b_infer_neurites_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/02c_infer_wholecell_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/02c_infer_wholecell_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/03_infer_cytosol_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/03_infer_cytosol_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/04_infer_lysosome_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/04_infer_lysosome_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/05_infer_mitochondria_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/05_infer_mitochondria_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/06_infer_golgi_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/06_infer_golgi_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/07_infer_peroxisome_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/07_infer_peroxisome_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/08_infer_endoplasmic_reticulum_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/09_infer_lipid_body_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/09_infer_lipid_body_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/10_batch_process_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/10_batch_process_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/10_batch_process_3Dv2.ipynb` & `infer-subc-0.1.4/notebooks/todelete/10_batch_process_3Dv2.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/999_fn_prototypes_json.ipynb` & `infer-subc-0.1.4/notebooks/todelete/999_fn_prototypes_json.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/A_spectral_test.ipynb` & `infer-subc-0.1.4/notebooks/todelete/A_spectral_test.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/_centrosome_routines.py` & `infer-subc-0.1.4/notebooks/todelete/_centrosome_routines.py`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/_graveyard.ipynb` & `infer-subc-0.1.4/notebooks/todelete/_graveyard.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/new02a_infer_soma_3D.ipynb` & `infer-subc-0.1.4/notebooks/todelete/new02a_infer_soma_3D.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/notebooks/todelete/test_soma_seg.ipynb` & `infer-subc-0.1.4/notebooks/todelete/test_soma_seg.ipynb`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/pyproject.toml` & `infer-subc-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/test.yaml` & `infer-subc-0.1.4/test.yaml`

 * *Files identical despite different names*

### Comparing `infer-subc-0.1.3/windows_notes.md` & `infer-subc-0.1.4/windows_notes.md`

 * *Files identical despite different names*

