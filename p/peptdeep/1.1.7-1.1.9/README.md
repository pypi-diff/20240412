# Comparing `tmp/peptdeep-1.1.7.tar.gz` & `tmp/peptdeep-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptdeep-1.1.7.tar", last modified: Sat Mar 16 09:16:50 2024, max compression
+gzip compressed data, was "peptdeep-1.1.9.tar", last modified: Fri Apr 12 07:35:22 2024, max compression
```

## Comparing `peptdeep-1.1.7.tar` & `peptdeep-1.1.9.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.849167 peptdeep-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-03-16 09:16:12.000000 peptdeep-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-16 09:16:12.000000 peptdeep-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-03-16 09:16:50.849167 peptdeep-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32817 2024-03-16 09:16:12.000000 peptdeep-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.829167 peptdeep-1.1.7/peptdeep/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.829167 peptdeep-1.1.7/peptdeep/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/cli_argparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.829167 peptdeep-1.1.7/peptdeep/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/constants/_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/constants/default_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/constants/model_const.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.829167 peptdeep-1.1.7/peptdeep/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.833167 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/legacy/thermo_raw/pyrawfilereader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.833167 peptdeep-1.1.7/peptdeep/mass_spec/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/mass_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/mass_spec/mass_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14429 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/mass_spec/match.py
--rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/mass_spec/ms_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.833167 peptdeep-1.1.7/peptdeep/model/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31674 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/building_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/ccs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/featurize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/generic_property_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    30801 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/model_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/model_shop.py
--rw-r--r--   0 runner    (1001) docker     (127)    26804 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/ms2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/model/rt.py
--rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/pipeline_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41087 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/pretrained_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.833167 peptdeep-1.1.7/peptdeep/protein/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/protein/fasta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.837167 peptdeep-1.1.7/peptdeep/psm_frag_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/psm_frag_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/psm_frag_reader/maxquant_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/psm_frag_reader/psm_frag_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/psm_frag_reader/psmlabel_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.837167 peptdeep-1.1.7/peptdeep/rescore/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/rescore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/rescore/fdr.py
--rw-r--r--   0 runner    (1001) docker     (127)    39861 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/rescore/feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/rescore/percolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.837167 peptdeep-1.1.7/peptdeep/spec_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/spec_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/spec_lib/library_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/spec_lib/predict_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/spec_lib/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.837167 peptdeep-1.1.7/peptdeep/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/utils/device_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/utils/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.837167 peptdeep-1.1.7/peptdeep/webui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/library_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.841167 peptdeep-1.1.7/peptdeep/webui/logos/
--rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/logos/peptdeep.ico
--rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/logos/peptdeep.png
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/main_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/model_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/rescore_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/server_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/settings_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/startpage.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/transfer_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-03-16 09:16:12.000000 peptdeep-1.1.7/peptdeep/webui/ui_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.829167 peptdeep-1.1.7/peptdeep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-16 09:16:50.000000 peptdeep-1.1.7/peptdeep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 09:16:50.849167 peptdeep-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-03-16 09:16:12.000000 peptdeep-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 09:16:50.841167 peptdeep-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-16 09:16:12.000000 peptdeep-1.1.7/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-16 09:16:12.000000 peptdeep-1.1.7/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.230252 peptdeep-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-12 07:34:59.000000 peptdeep-1.1.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 07:34:59.000000 peptdeep-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-04-12 07:35:22.230252 peptdeep-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32817 2024-04-12 07:34:59.000000 peptdeep-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/cli_argparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/default_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/constants/model_const.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26311 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/legacy/thermo_raw/pyrawfilereader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/mass_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/mass_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14429 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14666 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/mass_spec/ms_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31677 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/building_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/ccs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/featurize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/generic_property_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31129 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/model_shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26804 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/ms2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/model/rt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18783 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/pipeline_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41087 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/pretrained_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/protein/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/protein/fasta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.214252 peptdeep-1.1.9/peptdeep/psm_frag_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/maxquant_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/psm_frag_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6069 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/psm_frag_reader/psmlabel_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/rescore/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39861 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16641 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/rescore/percolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/spec_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12033 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/library_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/predict_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/spec_lib/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/_pyinstaller_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/device_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/utils/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16159 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/library_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.218252 peptdeep-1.1.9/peptdeep/webui/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)   118381 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    20283 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/main_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/model_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/rescore_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/server_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/settings_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/startpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/transfer_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-04-12 07:34:59.000000 peptdeep-1.1.9/peptdeep/webui/ui_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.210252 peptdeep-1.1.9/peptdeep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40528 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 07:35:22.000000 peptdeep-1.1.9/peptdeep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:35:22.230252 peptdeep-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-12 07:34:59.000000 peptdeep-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:35:22.222252 peptdeep-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 07:34:59.000000 peptdeep-1.1.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-12 07:34:59.000000 peptdeep-1.1.9/tests/test_gui.py
```

### Comparing `peptdeep-1.1.7/LICENSE.txt` & `peptdeep-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/PKG-INFO` & `peptdeep-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.1.7
+Version: 1.1.9
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `peptdeep-1.1.7/README.md` & `peptdeep-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/__init__.py` & `peptdeep-1.1.9/peptdeep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #     from . import protein # rely on spec_lib, import after
 # except (ImportError,RuntimeError, OSError):
 #     # happends when installation
 #     pass
 
 __project__ = "peptdeep"
-__version__ = "1.1.7"
+__version__ = "1.1.9"
 __license__ = "Apache 2.0"
 __description__ = "The AlphaX deep learning framework for Proteomics"
 __author__ = "Mann Labs"
 __author_email__ = "jalew.zwf@qq.com"
 __github__ = "https://github.com/MannLabs/peptdeep"
 __doc__ = "https://alphapeptdeep.readthedocs.io/en/latest/"
 __pypi__ = "https://pypi.org/project/peptdeep/"
```

### Comparing `peptdeep-1.1.7/peptdeep/__pycache__/__init__.cpython-39.pyc` & `peptdeep-1.1.9/peptdeep/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar 16 09:16:12 2024 UTC, .py size: 1673 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 5c63 f565 8906 0000  a.......\c.e....
+00000000: 610d 0d0a 0000 0000 23e4 1866 8906 0000  a.......#..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6407 5a07 6408  Z.d.Z.d.Z.d.Z.d.
 00000050: 5a08 6700 6409 a201 5a09 640a 5a0a 6700  Z.g.d...Z.d.Z.g.
 00000060: 640b a201 5a0b 640c 6701 5a0c 640d 640e  d...Z.d.g.Z.d.d.
 00000070: 6506 6507 6508 640f 9c05 5a0d 6410 6411  e.e.e.d...Z.d.d.
 00000080: 6412 9c02 5a0e 6413 5300 2914 da08 7065  d...Z.d.S.)...pe
-00000090: 7074 6465 6570 7a05 312e 312e 377a 0a41  ptdeepz.1.1.7z.A
+00000090: 7074 6465 6570 7a05 312e 312e 397a 0a41  ptdeepz.1.1.9z.A
 000000a0: 7061 6368 6520 322e 307a 3154 6865 2041  pache 2.0z1The A
 000000b0: 6c70 6861 5820 6465 6570 206c 6561 726e  lphaX deep learn
 000000c0: 696e 6720 6672 616d 6577 6f72 6b20 666f  ing framework fo
 000000d0: 7220 5072 6f74 656f 6d69 6373 7a09 4d61  r Proteomicsz.Ma
 000000e0: 6e6e 204c 6162 737a 106a 616c 6577 2e7a  nn Labsz.jalew.z
 000000f0: 7766 4071 712e 636f 6d7a 2468 7474 7073  wf@qq.comz$https
 00000100: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d61  ://github.com/Ma
```

### Comparing `peptdeep-1.1.7/peptdeep/cli.py` & `peptdeep-1.1.9/peptdeep/cli.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/cli_argparse.py` & `peptdeep-1.1.9/peptdeep/cli_argparse.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/constants/default_settings.yaml` & `peptdeep-1.1.9/peptdeep/constants/default_settings.yaml`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/constants/model_const.yaml` & `peptdeep-1.1.9/peptdeep/constants/model_const.yaml`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/gui.py` & `peptdeep-1.1.9/peptdeep/gui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt` & `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/THERMO_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll` & `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll` & `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/legacy/thermo_raw/pyrawfilereader.py` & `peptdeep-1.1.9/peptdeep/legacy/thermo_raw/pyrawfilereader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/mass_spec/mass_calibration.py` & `peptdeep-1.1.9/peptdeep/mass_spec/mass_calibration.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/mass_spec/match.py` & `peptdeep-1.1.9/peptdeep/mass_spec/match.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/mass_spec/ms_reader.py` & `peptdeep-1.1.9/peptdeep/mass_spec/ms_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/building_block.py` & `peptdeep-1.1.9/peptdeep/model/building_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,18 +590,18 @@
         )
         
     def forward(self, 
         aa_indices, mod_x, charges
     ):
         mod_x = self.mod_nn(mod_x)
         x = self.aa_emb(aa_indices)
-        charge_x = charges.unsqueeze(1).repeat(
+        charge_x = charges[:, None, None].repeat(
             1, mod_x.size(1), self.charge_dim
         )
-        return self.pos_encoder(torch.cat((x, mod_x,charge_x), 2))
+        return self.pos_encoder(torch.cat((x, mod_x, charge_x), 2))
 
 class Input_26AA_Mod_LSTM(torch.nn.Module):
     """
     Applies an LSTM network to a AA (26 AA letters) sequence & modifications
     """
     def __init__(self,
         out_features,
```

### Comparing `peptdeep-1.1.7/peptdeep/model/ccs.py` & `peptdeep-1.1.9/peptdeep/model/ccs.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/charge.py` & `peptdeep-1.1.9/peptdeep/model/charge.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/featurize.py` & `peptdeep-1.1.9/peptdeep/model/featurize.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/generic_property_prediction.py` & `peptdeep-1.1.9/peptdeep/model/generic_property_prediction.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/model_interface.py` & `peptdeep-1.1.9/peptdeep/model/model_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,23 @@
 # `transformers.optimization.get_cosine_schedule_with_warmup` will import tensorflow,
 # resulting in some package version issues.
 # Here we copy the code from transformers.optimization
 def _get_cosine_schedule_with_warmup_lr_lambda(
     current_step: int, *, num_warmup_steps: int, num_training_steps: int, num_cycles: float
 ):
     if current_step < num_warmup_steps:
-        return float(current_step) / float(max(1, num_warmup_steps))
-    progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
-    return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
+        return float(current_step+1) / float(max(1, num_warmup_steps))
+    progress = float(current_step - num_warmup_steps) / float(num_training_steps - num_warmup_steps)
+    return (
+        max(1e-10, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
+    )
+    # if current_step < num_warmup_steps:
+    #     return float(current_step) / float(max(1, num_warmup_steps))
+    # progress = float(current_step - num_warmup_steps) / float(max(1, num_training_steps - num_warmup_steps))
+    # return max(0.0, 0.5 * (1.0 + math.cos(math.pi * float(num_cycles) * 2.0 * progress)))
 
 
 def get_cosine_schedule_with_warmup(
     optimizer, num_warmup_steps: int, num_training_steps: int, num_cycles: float = 0.5, last_epoch: int = -1
 ):
     """
     Create a schedule with a learning rate that decreases following the values of the cosine function between the
```

### Comparing `peptdeep-1.1.7/peptdeep/model/ms2.py` & `peptdeep-1.1.9/peptdeep/model/ms2.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/model/rt.py` & `peptdeep-1.1.9/peptdeep/model/rt.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/pipeline_api.py` & `peptdeep-1.1.9/peptdeep/pipeline_api.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/pretrained_models.py` & `peptdeep-1.1.9/peptdeep/pretrained_models.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/protein/fasta.py` & `peptdeep-1.1.9/peptdeep/protein/fasta.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/psm_frag_reader/maxquant_frag_reader.py` & `peptdeep-1.1.9/peptdeep/psm_frag_reader/maxquant_frag_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/psm_frag_reader/psm_frag_reader.py` & `peptdeep-1.1.9/peptdeep/psm_frag_reader/psm_frag_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/psm_frag_reader/psmlabel_reader.py` & `peptdeep-1.1.9/peptdeep/psm_frag_reader/psmlabel_reader.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/rescore/fdr.py` & `peptdeep-1.1.9/peptdeep/rescore/fdr.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/rescore/feature_extractor.py` & `peptdeep-1.1.9/peptdeep/rescore/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/rescore/percolator.py` & `peptdeep-1.1.9/peptdeep/rescore/percolator.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/settings.py` & `peptdeep-1.1.9/peptdeep/settings.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/spec_lib/library_factory.py` & `peptdeep-1.1.9/peptdeep/spec_lib/library_factory.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/spec_lib/predict_lib.py` & `peptdeep-1.1.9/peptdeep/spec_lib/predict_lib.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/utils/__init__.py` & `peptdeep-1.1.9/peptdeep/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/utils/device_utils.py` & `peptdeep-1.1.9/peptdeep/utils/device_utils.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/utils/logger.py` & `peptdeep-1.1.9/peptdeep/utils/logger.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/utils/regression.py` & `peptdeep-1.1.9/peptdeep/utils/regression.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/library_ui.py` & `peptdeep-1.1.9/peptdeep/webui/library_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/logos/peptdeep.ico` & `peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.ico`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/logos/peptdeep.png` & `peptdeep-1.1.9/peptdeep/webui/logos/peptdeep.png`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/main_ui.py` & `peptdeep-1.1.9/peptdeep/webui/main_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/model_ui.py` & `peptdeep-1.1.9/peptdeep/webui/model_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/rescore_ui.py` & `peptdeep-1.1.9/peptdeep/webui/rescore_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/server.py` & `peptdeep-1.1.9/peptdeep/webui/server.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/server_ui.py` & `peptdeep-1.1.9/peptdeep/webui/server_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/settings_ui.py` & `peptdeep-1.1.9/peptdeep/webui/settings_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/startpage.py` & `peptdeep-1.1.9/peptdeep/webui/startpage.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/transfer_ui.py` & `peptdeep-1.1.9/peptdeep/webui/transfer_ui.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep/webui/ui_utils.py` & `peptdeep-1.1.9/peptdeep/webui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/peptdeep.egg-info/PKG-INFO` & `peptdeep-1.1.9/peptdeep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptdeep
-Version: 1.1.7
+Version: 1.1.9
 Summary: The AlphaX deep learning framework for Proteomics
 Home-page: https://github.com/MannLabs/peptdeep
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache 2.0
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `peptdeep-1.1.7/peptdeep.egg-info/SOURCES.txt` & `peptdeep-1.1.9/peptdeep.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 peptdeep/rescore/feature_extractor.py
 peptdeep/rescore/percolator.py
 peptdeep/spec_lib/__init__.py
 peptdeep/spec_lib/library_factory.py
 peptdeep/spec_lib/predict_lib.py
 peptdeep/spec_lib/translate.py
 peptdeep/utils/__init__.py
+peptdeep/utils/_pyinstaller_hooks.py
 peptdeep/utils/device_utils.py
 peptdeep/utils/logger.py
 peptdeep/utils/regression.py
 peptdeep/webui/__init__.py
 peptdeep/webui/library_ui.py
 peptdeep/webui/main_ui.py
 peptdeep/webui/model_ui.py
```

### Comparing `peptdeep-1.1.7/peptdeep.egg-info/requires.txt` & `peptdeep-1.1.9/peptdeep.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peptdeep-1.1.7/setup.py` & `peptdeep-1.1.9/setup.py`

 * *Files identical despite different names*

