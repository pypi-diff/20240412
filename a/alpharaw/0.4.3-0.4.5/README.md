# Comparing `tmp/alpharaw-0.4.3.tar.gz` & `tmp/alpharaw-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpharaw-0.4.3.tar", last modified: Thu Feb 15 09:50:29 2024, max compression
+gzip compressed data, was "alpharaw-0.4.5.tar", last modified: Fri Apr 12 07:28:12 2024, max compression
```

## Comparing `alpharaw-0.4.3.tar` & `alpharaw-0.4.5.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.598669 alpharaw-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-02-15 09:50:04.000000 alpharaw-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-15 09:50:04.000000 alpharaw-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-02-15 09:50:29.598669 alpharaw-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-02-15 09:50:04.000000 alpharaw-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.570670 alpharaw-0.4.3/alpharaw/
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.574669 alpharaw-0.4.3/alpharaw/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.574669 alpharaw-0.4.3/alpharaw/dia/
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/dia/normal_dia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.574669 alpharaw-0.4.3/alpharaw/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.586670 alpharaw-0.4.3/alpharaw/ext/sciex/
--rw-r--r--   0 runner    (1001) docker     (127)    32256 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Compression.dll
--rw-r--r--   0 runner    (1001) docker     (127)   210432 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Client.dll
--rw-r--r--   0 runner    (1001) docker     (127)   178688 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Contracts.dll
--rw-r--r--   0 runner    (1001) docker     (127)    99328 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.AnalystDataProvider.dll
--rw-r--r--   0 runner    (1001) docker     (127)   110080 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Client.dll
--rw-r--r--   0 runner    (1001) docker     (127)   444928 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Common.dll
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.CommonInterfaces.dll
--rw-r--r--   0 runner    (1001) docker     (127)    47616 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Contracts.dll
--rw-r--r--   0 runner    (1001) docker     (127)   133120 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Core.dll
--rw-r--r--   0 runner    (1001) docker     (127)   109056 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Wiff2.dll
--rw-r--r--   0 runner    (1001) docker     (127)   175616 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.WiffReader.dll
--rw-r--r--   0 runner    (1001) docker     (127)   112128 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.dll
--rw-r--r--   0 runner    (1001) docker     (127)   749056 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.DataService.dll
--rw-r--r--   0 runner    (1001) docker     (127)   141072 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Devices.Types.dll
--rw-r--r--   0 runner    (1001) docker     (127)   163840 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.Methods.MassSpec.dll
--rw-r--r--   0 runner    (1001) docker     (127)   118272 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.dll
--rw-r--r--   0 runner    (1001) docker     (127)    32256 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Infrastructure.dll
--rw-r--r--   0 runner    (1001) docker     (127)    38912 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.InternalRawXYProcessing.dll
--rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Muni.dll
--rw-r--r--   0 runner    (1001) docker     (127)   216576 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.RawXYProcessing.dll
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.StructuredStorage.dll
--rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.UserLog.Types.dll
--rw-r--r--   0 runner    (1001) docker     (127)   107520 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Utility.dll
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.XmlHelpers.dll
--rw-r--r--   0 runner    (1001) docker     (127)   219136 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Clearcore.FMan.dll
--rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.Processing.dll
--rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.SimpleTypes.dll
--rw-r--r--   0 runner    (1001) docker     (127)    40960 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.XYData.dll
--rw-r--r--   0 runner    (1001) docker     (127)   221184 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.FMan.dll
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Wiff.dll
--rw-r--r--   0 runner    (1001) docker     (127)  3992576 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/SciexToolKit.dll
--rwxr-xr-x   0 runner    (1001) docker     (127)     4096 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/WiffOps4Python.dll
--rw-r--r--   0 runner    (1001) docker     (127)   140288 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/sciex/protobuf-net.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.590669 alpharaw-0.4.3/alpharaw/ext/thermo_fisher/
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/thermo_fisher/THERMO_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.Data.dll
--rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.RawFileReader.dll
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.590669 alpharaw-0.4.3/alpharaw/feature/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/centroids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/chem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/finding.py
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/hills.py
--rw-r--r--   0 runner    (1001) docker     (127)    36339 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/feature/isotope_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.590669 alpharaw-0.4.3/alpharaw/legacy_msdata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/legacy_msdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/legacy_msdata/mgf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.590669 alpharaw-0.4.3/alpharaw/match/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/match/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/match/mass_calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/match/match_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/match/psm_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/match/psm_match_alphatims.py
--rw-r--r--   0 runner    (1001) docker     (127)    12599 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/ms_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/mzml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.590669 alpharaw-0.4.3/alpharaw/raw_access/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/raw_access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/raw_access/clr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/raw_access/pysciexwifffilereader.py
--rw-r--r--   0 runner    (1001) docker     (127)    25602 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/raw_access/pythermorawfilereader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/sciex.py
--rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.594669 alpharaw-0.4.3/alpharaw/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/utils/centroiding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/utils/df_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/utils/ms_path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/utils/timstof.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.594669 alpharaw-0.4.3/alpharaw/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/viz/df_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/viz/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19774 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/viz/psm_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/viz/xic_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.594669 alpharaw-0.4.3/alpharaw/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/wrappers/alphapept_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-02-15 09:50:04.000000 alpharaw-0.4.3/alpharaw/wrappers/alphatims_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 09:50:29.574669 alpharaw-0.4.3/alpharaw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-15 09:50:29.000000 alpharaw-0.4.3/alpharaw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 09:50:29.598669 alpharaw-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-15 09:50:04.000000 alpharaw-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.595212 alpharaw-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-12 07:27:48.000000 alpharaw-0.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-12 07:27:48.000000 alpharaw-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-04-12 07:28:12.595212 alpharaw-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-12 07:27:48.000000 alpharaw-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.567212 alpharaw-0.4.5/alpharaw/
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.571212 alpharaw-0.4.5/alpharaw/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.571212 alpharaw-0.4.5/alpharaw/dia/
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/dia/normal_dia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.571212 alpharaw-0.4.5/alpharaw/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.583212 alpharaw-0.4.5/alpharaw/ext/sciex/
+-rw-r--r--   0 runner    (1001) docker     (127)    32256 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Compression.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   210432 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Client.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   178688 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Contracts.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    99328 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.AnalystDataProvider.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   110080 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Client.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   444928 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Common.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.CommonInterfaces.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    47616 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Contracts.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   133120 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Core.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   109056 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Wiff2.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   175616 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.WiffReader.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   112128 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   749056 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.DataService.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   141072 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Devices.Types.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   163840 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.Methods.MassSpec.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   118272 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    32256 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Infrastructure.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    38912 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.InternalRawXYProcessing.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    69632 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Muni.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   216576 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.RawXYProcessing.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.StructuredStorage.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.UserLog.Types.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   107520 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Utility.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.XmlHelpers.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   219136 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Clearcore.FMan.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    73728 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.Processing.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    11776 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.SimpleTypes.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    40960 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.XYData.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   221184 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.FMan.dll
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Wiff.dll
+-rw-r--r--   0 runner    (1001) docker     (127)  3992576 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/SciexToolKit.dll
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4096 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/WiffOps4Python.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   140288 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/sciex/protobuf-net.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.583212 alpharaw-0.4.5/alpharaw/ext/thermo_fisher/
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/thermo_fisher/THERMO_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   366080 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.Data.dll
+-rw-r--r--   0 runner    (1001) docker     (127)   620032 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.RawFileReader.dll
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.587212 alpharaw-0.4.5/alpharaw/feature/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/centroids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9721 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/chem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/finding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/hills.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36339 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/feature/isotope_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.587212 alpharaw-0.4.5/alpharaw/legacy_msdata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/legacy_msdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/legacy_msdata/mgf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.587212 alpharaw-0.4.5/alpharaw/match/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/mass_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/match_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20889 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/psm_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9833 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/psm_match_alphatims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/match/spec_finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/ms_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/mzml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.587212 alpharaw-0.4.5/alpharaw/raw_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/raw_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/raw_access/clr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/raw_access/pysciexwifffilereader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/raw_access/pythermorawfilereader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/sciex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13195 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.591212 alpharaw-0.4.5/alpharaw/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/utils/centroiding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/utils/df_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/utils/ms_path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/utils/timstof.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.591212 alpharaw-0.4.5/alpharaw/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13179 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/df_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/psm_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/xic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11092 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/viz/xic_plot_tims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.591212 alpharaw-0.4.5/alpharaw/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/wrappers/alphapept_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-12 07:27:48.000000 alpharaw-0.4.5/alpharaw/wrappers/alphatims_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:28:12.567212 alpharaw-0.4.5/alpharaw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 07:28:12.000000 alpharaw-0.4.5/alpharaw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:28:12.595212 alpharaw-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-12 07:27:48.000000 alpharaw-0.4.5/setup.py
```

### Comparing `alpharaw-0.4.3/LICENSE.txt` & `alpharaw-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/PKG-INFO` & `alpharaw-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpharaw
-Version: 0.4.3
+Version: 0.4.5
 Summary: An open-source Python package to unify raw MS data access and storage.
 Home-page: https://github.com/MannLabs/alpharaw
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alpharaw
```

### Comparing `alpharaw-0.4.3/README.md` & `alpharaw-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/__init__.py` & `alpharaw-0.4.5/alpharaw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     try:
         from .sciex import SciexWiffData
         from .thermo import ThermoRawData
     except (RuntimeError, ImportError):
         print("[WARN] pythonnet is not installed")
 
 __project__ = "alpharaw"
-__version__ = "0.4.3"
+__version__ = "0.4.5"
 __license__ = "Apache"
 __description__ = "An open-source Python package to unify raw MS data access and storage."
 __author__ = "Mann Labs"
 __author_email__ = "jalew.zwf@qq.com"
 __github__ = "https://github.com/MannLabs/alpharaw"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alpharaw-0.4.3/alpharaw/__pycache__/__init__.cpython-39.pyc` & `alpharaw-0.4.5/alpharaw/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Feb 15 09:50:04 2024 UTC, .py size: 1797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 4cde cd65 0507 0000  a.......L..e....
+00000000: 610d 0d0a 0000 0000 74e2 1866 0507 0000  a.......t..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a00 6500 a001 6402 a101 0100  d.l.Z.e...d.....
 00000040: 6403 6404 8400 5a02 6405 5a03 6406 5a04  d.d...Z.d.Z.d.Z.
 00000050: 6407 5a05 6408 5a06 6409 5a07 640a 5a08  d.Z.d.Z.d.Z.d.Z.
 00000060: 640b 5a09 6700 640c a201 5a0a 640d 5a0b  d.Z.g.d...Z.d.Z.
 00000070: 6700 640e a201 5a0c 640f 6509 6410 9c02  g.d...Z.d.e.d...
@@ -40,15 +40,15 @@
 00000270: 6572 2f77 6f72 6b2f 616c 7068 6172 6177  er/work/alpharaw
 00000280: 2f61 6c70 6861 7261 772f 616c 7068 6172  /alpharaw/alphar
 00000290: 6177 2f5f 5f69 6e69 745f 5f2e 7079 da10  aw/__init__.py..
 000002a0: 7265 6769 7374 6572 5f72 6561 6465 7273  register_readers
 000002b0: 0600 0000 7312 0000 0000 010c 010c 010c  ....s...........
 000002c0: 010c 0102 010c 0110 0110 0172 0f00 0000  ...........r....
 000002d0: da08 616c 7068 6172 6177 7a05 302e 342e  ..alpharawz.0.4.
-000002e0: 335a 0641 7061 6368 657a 4641 6e20 6f70  3Z.ApachezFAn op
+000002e0: 355a 0641 7061 6368 657a 4641 6e20 6f70  5Z.ApachezFAn op
 000002f0: 656e 2d73 6f75 7263 6520 5079 7468 6f6e  en-source Python
 00000300: 2070 6163 6b61 6765 2074 6f20 756e 6966   package to unif
 00000310: 7920 7261 7720 4d53 2064 6174 6120 6163  y raw MS data ac
 00000320: 6365 7373 2061 6e64 2073 746f 7261 6765  cess and storage
 00000330: 2e7a 094d 616e 6e20 4c61 6273 7a10 6a61  .z.Mann Labsz.ja
 00000340: 6c65 772e 7a77 6640 7171 2e63 6f6d 7a24  lew.zwf@qq.comz$
 00000350: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
```

### Comparing `alpharaw-0.4.3/alpharaw/cli.py` & `alpharaw-0.4.5/alpharaw/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,18 +38,18 @@
         url=alpharaw.__github__.center(50), 
         license=alpharaw.__license__.center(50),
     )
 )
     if ctx.invoked_subcommand is None:
         click.echo(run.get_help(ctx))
 
-@run.command("parse", help="Convert raw files into alpharaw_hdf format.")
+@run.command("parse", help="Convert raw files into alpharaw hdf5 (.hdf) format.")
 @click.option(
     "--raw_type", type=str, default="thermo_raw",
-    show_default=True, help=f"Only `thermo_raw` is supported currently.",
+    show_default=True, help=f"Only `thermo_raw`, `sciex_wiff` is supported currently.",
 )
 @click.option(
     "--raw", multiple=True, default=[],
     show_default=True, help="Raw files, can be `--raw raw1 --raw raw2 ...`."
 )
 def _parse(raw_type:str, raw:list):
     reader = ms_reader_provider.get_reader(raw_type)
```

### Comparing `alpharaw-0.4.3/alpharaw/dia/normal_dia.py` & `alpharaw-0.4.5/alpharaw/dia/normal_dia.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Compression.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Compression.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Client.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Client.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Contracts.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Acquisition.Contracts.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.AnalystDataProvider.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.AnalystDataProvider.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Client.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Client.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Common.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Common.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.CommonInterfaces.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.CommonInterfaces.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Contracts.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Contracts.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Core.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Core.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.Wiff2.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.Wiff2.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.WiffReader.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.WiffReader.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Data.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Data.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.DataService.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.DataService.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Devices.Types.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Devices.Types.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.Methods.MassSpec.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.Methods.MassSpec.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Domain.Acquisition.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Infrastructure.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Infrastructure.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.InternalRawXYProcessing.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.InternalRawXYProcessing.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Muni.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Muni.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.RawXYProcessing.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.RawXYProcessing.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.StructuredStorage.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.StructuredStorage.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.UserLog.Types.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.UserLog.Types.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.Utility.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.Utility.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Clearcore2.XmlHelpers.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Clearcore2.XmlHelpers.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Clearcore.FMan.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Clearcore.FMan.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.Processing.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.Processing.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.SimpleTypes.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.SimpleTypes.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Data.XYData.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Data.XYData.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.FMan.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.FMan.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/Sciex.Wiff.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/Sciex.Wiff.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/SciexToolKit.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/SciexToolKit.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/WiffOps4Python.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/WiffOps4Python.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/sciex/protobuf-net.dll` & `alpharaw-0.4.5/alpharaw/ext/sciex/protobuf-net.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/thermo_fisher/THERMO_LICENSE.txt` & `alpharaw-0.4.5/alpharaw/ext/thermo_fisher/THERMO_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.Data.dll` & `alpharaw-0.4.5/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.Data.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.RawFileReader.dll` & `alpharaw-0.4.5/alpharaw/ext/thermo_fisher/ThermoFisher.CommonCore.RawFileReader.dll`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/feature/centroids.py` & `alpharaw-0.4.5/alpharaw/feature/centroids.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/feature/chem.py` & `alpharaw-0.4.5/alpharaw/feature/chem.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/feature/finding.py` & `alpharaw-0.4.5/alpharaw/feature/finding.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/feature/hills.py` & `alpharaw-0.4.5/alpharaw/feature/hills.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/feature/isotope_pattern.py` & `alpharaw-0.4.5/alpharaw/feature/isotope_pattern.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/legacy_msdata/mgf.py` & `alpharaw-0.4.5/alpharaw/legacy_msdata/mgf.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/match/mass_calibration.py` & `alpharaw-0.4.5/alpharaw/match/mass_calibration.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/match/psm_match.py` & `alpharaw-0.4.5/alpharaw/match/psm_match.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     MSData_Base, ms_reader_provider,
     PEAK_MZ_DTYPE, PEAK_INTENSITY_DTYPE
 )
 
 from alpharaw.match.match_utils import (
     match_closest_peaks, match_highest_peaks, 
 )
+from alpharaw.match.spec_finder import (
+    find_dia_spec_idxes_same_window
+)
 from alpharaw.utils.ms_path_utils import parse_ms_files_to_dict
 
 from alpharaw.dia.normal_dia import NormalDIAGrouper
 
 
 class PepSpecMatch:
     """
@@ -475,15 +478,15 @@
                 len(psm_df_one_raw), -1, dtype=np.int32
             )
 
             for dia_group, group_df in grouper.dia_group_dfs:
                 psm_idxes = psm_groups[dia_group]
                 if len(psm_idxes) == 0: continue
                 psm_idxes = np.array(psm_idxes, dtype=np.int32)
-                spec_idxes = get_dia_spec_idxes(
+                spec_idxes = find_dia_spec_idxes_same_window(
                     group_df.rt.values,
                     psm_df_one_raw.rt.values[psm_idxes],
                     max_spec_per_query=self.max_spec_per_query
                 )
                 for i in range(spec_idxes.shape[-1]):
                     all_spec_idxes[
                         psm_idxes+psm_origin_len*i
@@ -525,22 +528,22 @@
         )
 
         return (
             self.psm_df, self.fragment_mz_df, 
             self.matched_intensity_df, self.matched_mz_err_df
         )
 
-@numba.njit
+@numba.jit(nogil=True)
 def match_one_raw_with_numba(
     spec_idxes, frag_start_idxes, frag_stop_idxes,
     all_frag_mzs, all_frag_mz_tols,
     all_spec_mzs, all_spec_intensities, 
     peak_start_idxes, peak_stop_idxes,
     matched_intensities, matched_mz_errs, 
-    matched_closest=True,
+    match_closest=True,
 ):
     """ 
     Internel function to match fragment mz values to spectrum mz values.
     Matched_mz_errs[i] = np.inf if no peaks are matched.
 
     Results will saved in place of matched_intensities 
     and matched_mz_errs.
@@ -554,15 +557,15 @@
         if peak_stop == peak_start: continue
         spec_mzs = all_spec_mzs[peak_start:peak_stop]
         spec_intens = all_spec_intensities[peak_start:peak_stop]
 
         frag_mzs = all_frag_mzs[frag_start:frag_stop,:].copy()
         frag_mz_tols = all_frag_mz_tols[frag_start:frag_stop,:].copy()
         
-        if matched_closest:
+        if match_closest:
             matched_idxes = match_closest_peaks(
                 spec_mzs, spec_intens, 
                 frag_mzs, frag_mz_tols
             ).reshape(-1)
         else:
             matched_idxes = match_highest_peaks(
                 spec_mzs, spec_intens, 
@@ -653,33 +656,7 @@
             ].copy().reshape(-1)[
                 frag_mz_values[
                     frag_start_idxes[i]:frag_stop_idxes[i],:
                 ].copy().reshape(-1)>=min_mz
             ]
         ))
     return np.array(scores,np.int32)
-
-@numba.njit    
-def get_dia_spec_idxes(
-    spec_rt_values:np.ndarray, 
-    query_rt_values:np.ndarray, 
-    max_spec_per_query:int,
-):
-    rt_idxes = np.searchsorted(spec_rt_values, query_rt_values)
-    
-    spec_idxes = np.full(
-        (len(rt_idxes),max_spec_per_query),
-        -1, dtype=np.int32
-    )
-    n = max_spec_per_query // 2
-
-    for iquery in range(len(rt_idxes)):
-        if rt_idxes[iquery] < n:
-            spec_idxes[iquery,:] = np.arange(0, max_spec_per_query)
-        else:
-            spec_idxes[iquery,:] = np.arange(
-                rt_idxes[iquery]-n, 
-                rt_idxes[iquery]-n+max_spec_per_query
-            )
-    return spec_idxes
-
-
```

### Comparing `alpharaw-0.4.3/alpharaw/match/psm_match_alphatims.py` & `alpharaw-0.4.5/alpharaw/match/psm_match_alphatims.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,33 +94,32 @@
 
     # : find closest MS2 for the given RT when slicing
     find_k_nearest_ms2_by_im = False
     k_im_nearest = 11
 
     def get_peak_df(self,
         precursor_mz:float,
-        rt:float,
+        rt_sec:float,
         im:float=0.0,
     )->pd.DataFrame:
         """
         Parameters
         ----------
         precursor_mz : float
             Precursor m/z value
-        rt : float
-            RT value in minutes
+        rt_sec : float
+            RT value in seconds
         im : float, optional
             Ion mobility, by default 0.0
 
         Returns
         -------
         pd.DataFrame
             peak_df in alphatims DF format
         """
-        rt_sec = rt*60
         rt_slice = slice(
             rt_sec-self.rt_sec_tol_to_slice_ms2,
             rt_sec+self.rt_sec_tol_to_slice_ms2,
         )
 
         if im == 0 or self.tims_data.scan_max_index == 1:
             im_slice = slice(None)
@@ -172,34 +171,34 @@
                 spec_df = spec_df[spec_df.rt_values.isin(closest_rts)]
         
         return spec_df
 
     def get_peaks(
         self,
         precursor_mz:float,
-        rt:float,
+        rt_sec:float,
         im:float=0.0,
     )->tuple:
         """
         Parameters
         ----------
         precursor_mz : float
             Precursor m/z value
-        rt : float
-            RT value in minutes
+        rt_sec : float
+            RT value in seconds
         im : float, optional
             Ion mobility, by default 0.0
 
         Returns
         -------
         tuple
             np.ndarray: peak m/z values
             np.ndarray: peak intensity values
         """
-        spec_df = self.get_peak_df(precursor_mz, rt, im)
+        spec_df = self.get_peak_df(precursor_mz, rt_sec, im)
         spec_df = spec_df.sort_values('mz_values').reset_index(drop=True)
         return (
             spec_df.mz_values.values, 
             spec_df.intensity_values.values
         )
 
     def load_ms_data(self,
```

### Comparing `alpharaw-0.4.3/alpharaw/ms_data_base.py` & `alpharaw-0.4.5/alpharaw/ms_data_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         """
         # A spectrum contains peaks
         self.spectrum_df:pd.DataFrame = pd.DataFrame()
         # A peak contains mz, intensity, and ...
         self.peak_df:pd.DataFrame = pd.DataFrame()
         self._raw_file_path = ''
         self.centroided = centroided
-        self.save_as_hdf = save_as_hdf
+        self._save_as_hdf = save_as_hdf
         self.creation_time = ''
         self.file_type = ''
         self.instrument = 'none'
 
     def _get_term_id(self, terminology:str):
         """
         Get terminology id from :data:`self.vocab`, -1 if not exist.
@@ -95,15 +95,15 @@
 
     def import_raw(self, _path:str):
         self.raw_file_path = _path
         raw_data = self._import(_path)
         self._set_dataframes(raw_data)
         self._check_df()
 
-        if self.save_as_hdf:
+        if self._save_as_hdf:
             self.save_hdf(_path+'.hdf')
 
     def load_raw(self, _path:str):
         self.import_raw(_path)
 
     def _save_meta_to_hdf(self, hdf:HDF_File):
         hdf.ms_data.meta = {
@@ -163,17 +163,20 @@
             raw_data['peak_intensity'],
             raw_data['peak_indices'][:-1],
             raw_data['peak_indices'][1:],
         )
 
         for col, val in raw_data.items():
             if col in self.column_dtypes:
-                self.spectrum_df[col] = np.array(
-                    val, dtype=self.column_dtypes[col]
-                )
+                if self.column_dtypes[col] == "O":
+                    self.spectrum_df[col] = list(val)
+                else:
+                    self.spectrum_df[col] = np.array(
+                        val, dtype=self.column_dtypes[col]
+                    )
 
     def _read_creation_time(self, raw_data):
         pass
 
     def _check_df(self):
         self._check_rt()
         # self._check_mobility()
```

### Comparing `alpharaw-0.4.3/alpharaw/mzml.py` & `alpharaw-0.4.5/alpharaw/mzml.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/raw_access/clr_utils.py` & `alpharaw-0.4.5/alpharaw/raw_access/clr_utils.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/raw_access/pysciexwifffilereader.py` & `alpharaw-0.4.5/alpharaw/raw_access/pysciexwifffilereader.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/raw_access/pythermorawfilereader.py` & `alpharaw-0.4.5/alpharaw/raw_access/pythermorawfilereader.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,19 @@
     def GetStatusLogForRetentionTime(self, rt):
         logEntry = self.source.GetStatusLogForRetentionTime(rt)
         return dict(zip(logEntry.Labels, logEntry.Values))
 
     def GetStatusLogForScanNum(self, scan):
         return self.GetStatusLogForRetentionTime(self.RTFromScanNum(scan))
 
+    def GetScanEventForScanNum(self, scanNumber):
+        return IScanEventBase(
+            self.source.GetScanEventForScanNumber(scanNumber)
+        )
+    
     def GetNumberOfMassRangesFromScanNum(self, scanNumber):
         """This function gets the number of MassRange data items in the scan."""
         return IScanEventBase(
             self.source.GetScanEventForScanNumber(scanNumber)
         ).MassRangeCount
 
     def GetMassRangeFromScanNum(self, scanNumber, massRangeIndex):
```

### Comparing `alpharaw-0.4.3/alpharaw/sciex.py` & `alpharaw-0.4.5/alpharaw/sciex.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/thermo.py` & `alpharaw-0.4.5/alpharaw/thermo.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 from .ms_data_base import ms_reader_provider
 
 __trailer_extra_list__ = [
     "injection_time", "cv",
     "max_ion_time", "agc_target", "energy_ev",
     "injection_optics_settling_time", 
     "funnel_rf_level", "faims_cv",
-    "activation", "analyzer",
-    "activation_id", "analyzer_id",
-    "scan_event_string",
 ]
 __auxiliary_item_dtypes__ = {
     "injection_time": np.float32, 
     "cv": np.float32,
     "max_ion_time": np.float32, 
     "agc_target": np.int64, 
     "energy_ev": np.float32,
@@ -31,16 +28,127 @@
     "detector": "U", 
     "activation": "U", 
     "analyzer": "U",
     "detector_id": np.uint8, 
     "activation_id": np.uint8, 
     "analyzer_id": np.uint8,
     "scan_event_string": "U",
+    "multinotch": "O",
 }
 
+class ThermoRawData(MSData_Base):
+    """
+    Loading Thermo Raw data as MSData_Base data structure.
+    """
+    def __init__(self, 
+        centroided : bool = True,
+        process_count : int = 10,
+        mp_batch_size : int = 5000,
+        save_as_hdf: bool = False,
+        dda : bool = False,
+        auxiliary_items : list = [],
+        **kwargs
+    ):
+        """
+        Parameters
+        ----------
+        centroided : bool, default = True
+            if peaks will be centroided after loading,
+            by default True
+
+        process_count : int, default = 8
+            number of processes to use for loading
+
+        mp_batch_size : int, default = 10000
+            number of spectra to load in each batch
+
+        save_as_hdf : bool, default = False
+            automatically save hdf after load raw data.
+        
+        dda : bool, default = False
+            is DDA data
+
+        auxiliary_items : list, default = []
+            Candidates are:
+            "injection_time", "cv",
+            "max_ion_time", "agc_target", "energy_ev",
+            "injection_optics_settling_time", 
+            "funnel_rf_level", "faims_cv",
+            "detector", "activation", "analyzer",
+            "detector_id", "activation_id", "analyzer_id",
+        """
+        super().__init__(
+            centroided, save_as_hdf=save_as_hdf,
+            **kwargs
+        )
+        self.file_type = 'thermo'
+        self.process_count = process_count
+        self.mp_batch_size = mp_batch_size
+        self.dda = dda
+        self.auxiliary_items = auxiliary_items
+        self.column_dtypes.update(__auxiliary_item_dtypes__)
+
+    def _import(
+        self,
+        raw_file_path: str,
+    ) -> dict:
+        rawfile = pyrawfilereader.RawFileReader(raw_file_path)
+        self.creation_time = rawfile.GetCreationDate()
+
+        # create batches for multiprocessing
+        first_spectrum_number = rawfile.FirstSpectrumNumber
+        last_spectrum_number = rawfile.LastSpectrumNumber
+
+        if self.process_count > 1:
+            mode = "spawn" if platform.system() != "Linux" else "forkserver"
+
+            batches = np.arange(
+                first_spectrum_number, last_spectrum_number + 1, self.mp_batch_size
+            )
+            batches = np.append(batches, last_spectrum_number + 1)
+
+            # use multiprocessing to load batches
+            _import_batch_partial = partial(
+                _import_batch, raw_file_path=raw_file_path, 
+                centroided = self.centroided, dda=self.dda,
+                auxiliary_items = self.auxiliary_items,
+            )
+            with mp.get_context(mode).Pool(processes=self.process_count) as pool:
+                batches = list(
+                    tqdm(pool.imap(_import_batch_partial, zip(batches[:-1], batches[1:])))
+                )
+
+            # collect peak indices
+            _peak_indices = np.concatenate([batch["_peak_indices"] for batch in batches])
+            peak_indices = np.empty(rawfile.LastSpectrumNumber + 1, np.int64)
+            peak_indices[0] = 0
+            peak_indices[1:] = np.cumsum(_peak_indices)
+
+            output_dict = {"peak_indices": peak_indices}
+
+            # concatenate other arrays
+            for key in batches[0].keys():
+                if key == "_peak_indices":
+                    continue
+                output_dict[key] = np.concatenate([batch[key] for batch in batches])
+        else:
+            output_dict = _import_batch(
+                (first_spectrum_number, last_spectrum_number+1),
+                raw_file_path, self.centroided, dda=self.dda,
+                auxiliary_items = self.auxiliary_items,
+            )
+            peak_indices = np.empty(rawfile.LastSpectrumNumber + 1, np.int64)
+            peak_indices[0] = 0
+            peak_indices[1:] = np.cumsum(output_dict["_peak_indices"])
+            output_dict["peak_indices"] = peak_indices
+        rawfile.Close()
+
+        return output_dict
+
+
 def _import_batch(
     start_stop_tuple: tuple,
     raw_file_path: str,
     centroided: bool,
     dda:bool,
     auxiliary_items:list,
 ) -> dict:
@@ -90,18 +198,21 @@
     precursor_charges = []
     ms_order_list = []
     ce_list = []
 
     auxiliary_dict = dict(
         (item, []) for item in auxiliary_items
     )
-    for item in __trailer_extra_list__:
-        if item in auxiliary_dict:
-            use_trailer_extra = True
-            break
+    if dda: 
+        use_trailer_extra = True
+    else:
+        for item in __trailer_extra_list__:
+            if item in auxiliary_dict:
+                use_trailer_extra = True
+                break
 
     for i in range(start, stop):
         if not centroided:
             masses, intensities = rawfile.GetProfileMassListFromScanNum(i)
         else:
             masses, intensities = rawfile.GetCentroidMassListFromScanNum(i)
         mz_values.append(masses.astype(PEAK_MZ_DTYPE))
@@ -110,14 +221,15 @@
         rt = rawfile.RTFromScanNum(i)
         rt_values.append(rt)
         ms_order = rawfile.GetMSOrderForScanNum(i)
         ms_order_list.append(ms_order)
 
         if use_trailer_extra:
             trailer_data = rawfile.GetTrailerExtraForScanNum(i)
+        scan_event = rawfile.GetScanEventForScanNum(i)
 
         if "injection_time" in auxiliary_dict:
             auxiliary_dict["injection_time"].append(
                 float(trailer_data["Ion Injection Time (ms):"])
             )
         if "max_ion_time" in auxiliary_dict:
             auxiliary_dict["max_ion_time"].append(
@@ -125,20 +237,21 @@
             )
         if "agc_target" in auxiliary_dict:
             auxiliary_dict["agc_target"].append(
                 float(trailer_data["AGC Target:"])
             )
         if "energy_ev" in auxiliary_dict:
             energy_ev = trailer_data["HCD Energy V:"]
-            if energy_ev:
-                auxiliary_dict["energy_ev"].append(
-                    float(energy_ev)
-                )
-            else:
-                auxiliary_dict["energy_ev"].append(0)
+            if not energy_ev:
+                energy_ev = trailer_data["HCD Energy eV:"]
+            if not energy_ev:
+                energy_ev = 0
+            auxiliary_dict["energy_ev"].append(
+                float(energy_ev)
+            )
         if "injection_optics_settling_time" in auxiliary_dict:
             auxiliary_dict["injection_optics_settling_time"].append(
                 float(trailer_data[
                     "Injection Optics Settling Time (ms):"
                 ])
             )
         if "funnel_rf_level" in auxiliary_dict:
@@ -147,60 +260,74 @@
             )
         if "faims_cv" in auxiliary_dict:
             auxiliary_dict["faims_cv"].append(
                 float(trailer_data["FAIMS CV:"])
             )
         if "activation" in auxiliary_dict:
             auxiliary_dict["activation"].append(
-                rawfile.GetActivationTypeForScanNum(i) 
+                rawfile.activationType[
+                    int(scan_event.GetActivation(0))
+                ]
                 if ms_order > 1 else "MS1"
             )
         if "activation_id" in auxiliary_dict:
             auxiliary_dict["activation_id"].append(
-                rawfile.GetActivationIDForScanNum(i)
+                int(scan_event.GetActivation(0))
                 if ms_order > 1 else 255
             )
         if "analyzer" in auxiliary_dict:
             auxiliary_dict["analyzer"].append(
-                rawfile.GetMassAnalyzerTypeForScanNum(i)
+                rawfile.massAnalyzerType[
+                    int(scan_event.MassAnalyzer)
+                ]
             )
         if "analyzer_id" in auxiliary_dict:
             auxiliary_dict["analyzer_id"].append(
-                rawfile.GetMassAnalyzerIDForScanNum(i)
+                int(scan_event.MassAnalyzer)
             )
         if "scan_event_string" in auxiliary_dict:
             auxiliary_dict["scan_event_string"].append(
                 rawfile.GetScanEventStringForScanNum(i)
             )
+        if "multinotch" in auxiliary_dict:
+            windows = []
+            for _ in range(scan_event.MassCount):
+                _mass = scan_event.GetMass(_)
+                _width = scan_event.GetIsolationWidth(_)
+                windows.append((_mass-_width/2, _mass+_width/2))
+            auxiliary_dict["multinotch"].append(np.array(windows))
 
         if ms_order == 1:
             ce_list.append(0)
             if "cv" in auxiliary_dict:
                 auxiliary_dict["cv"].append(0)
             precursor_mz_values.append(-1.0)
             isolation_mz_lowers.append(-1.0)
             isolation_mz_uppers.append(-1.0)
             precursor_charges.append(0)
         else:
             ce_list.append(rawfile.GetCollisionEnergyForScanNum(i))
             if "cv" in auxiliary_dict:
-                n_cvs = rawfile.GetNumberOfSourceFragmentsFromScanNum(i)
+                n_cvs = scan_event.SourceFragmentationInfoCount
                 if n_cvs > 0:
                     auxiliary_dict["cv"].append(
-                        rawfile.GetSourceFragmentValueFromScanNum(i, 0)
+                        scan_event.GetSourceFragmentationInfo(0)
                     )
                 else:
                     auxiliary_dict["cv"].append(0)
 
-            isolation_center = rawfile.GetPrecursorMassForScanNum(i)
-            isolation_width = rawfile.GetIsolationWidthForScanNum(i)
+            
+            isolation_center = scan_event.GetReaction(0).PrecursorMass
+            isolation_width = scan_event.GetIsolationWidth(0)
+            # isolation_center = rawfile.GetPrecursorMassForScanNum(i)
+            # isolation_width = rawfile.GetIsolationWidthForScanNum(i)
 
             if dda:
                 # GetMS2MonoMzAndChargeFromScanNum is slow
-                mono_mz, charge = rawfile.GetMS2MonoMzAndChargeFromScanNum(i)
+                mono_mz, charge = _get_mono_and_charge(trailer_data, scan_event)
                 if mono_mz <= 0:
                     mono_mz = isolation_center
             else:
                 mono_mz = isolation_center
                 charge = 0
 
             # In case that: ms1 = ms_order==2&NCE==0?
@@ -234,119 +361,14 @@
     for key, val in list(auxiliary_dict.items()):
         auxiliary_dict[key] = np.array(
             val, dtype=__auxiliary_item_dtypes__[key]
         ).copy()
     spec_dict.update(auxiliary_dict)
     return spec_dict
 
-class ThermoRawData(MSData_Base):
-    """
-    Loading Thermo Raw data as MSData_Base data structure.
-    """
-    def __init__(self, 
-        centroided : bool = True,
-        process_count : int = 10,
-        mp_batch_size : int = 5000,
-        save_as_hdf: bool = False,
-        dda : bool = False,
-        auxiliary_items : list = [],
-        **kwargs
-    ):
-        """
-        Parameters
-        ----------
-        centroided : bool, default = True
-            if peaks will be centroided after loading,
-            by default True
-
-        process_count : int, default = 8
-            number of processes to use for loading
-
-        mp_batch_size : int, default = 10000
-            number of spectra to load in each batch
-
-        save_as_hdf : bool, default = False
-            automatically save hdf after load raw data.
-        
-        dda : bool, default = False
-            is DDA data
-
-        auxiliary_items : list, default = []
-            Candidates are:
-            "injection_time", "cv",
-            "max_ion_time", "agc_target", "energy_ev",
-            "injection_optics_settling_time", 
-            "funnel_rf_level", "faims_cv",
-            "detector", "activation", "analyzer",
-            "detector_id", "activation_id", "analyzer_id",
-        """
-        super().__init__(
-            centroided, save_as_hdf=save_as_hdf,
-            **kwargs
-        )
-        self.file_type = 'thermo'
-        self.process_count = process_count
-        self.mp_batch_size = mp_batch_size
-        self.dda = dda
-        self.auxiliary_items = auxiliary_items
-        self.column_dtypes.update(__auxiliary_item_dtypes__)
-
-    def _import(
-        self,
-        raw_file_path: str,
-    ) -> dict:
-        rawfile = pyrawfilereader.RawFileReader(raw_file_path)
-        self.creation_time = rawfile.GetCreationDate()
-
-        # create batches for multiprocessing
-        first_spectrum_number = rawfile.FirstSpectrumNumber
-        last_spectrum_number = rawfile.LastSpectrumNumber
-
-        if self.process_count > 1:
-            mode = "spawn" if platform.system() != "Linux" else "forkserver"
-
-            batches = np.arange(
-                first_spectrum_number, last_spectrum_number + 1, self.mp_batch_size
-            )
-            batches = np.append(batches, last_spectrum_number + 1)
-
-            # use multiprocessing to load batches
-            _import_batch_partial = partial(
-                _import_batch, raw_file_path=raw_file_path, 
-                centroided = self.centroided, dda=self.dda,
-                auxiliary_items = self.auxiliary_items,
-            )
-            with mp.get_context(mode).Pool(processes=self.process_count) as pool:
-                batches = list(
-                    tqdm(pool.imap(_import_batch_partial, zip(batches[:-1], batches[1:])))
-                )
-
-            # collect peak indices
-            _peak_indices = np.concatenate([batch["_peak_indices"] for batch in batches])
-            peak_indices = np.empty(rawfile.LastSpectrumNumber + 1, np.int64)
-            peak_indices[0] = 0
-            peak_indices[1:] = np.cumsum(_peak_indices)
-
-            output_dict = {"peak_indices": peak_indices}
-
-            # concatenate other arrays
-            for key in batches[0].keys():
-                if key == "_peak_indices":
-                    continue
-                output_dict[key] = np.concatenate([batch[key] for batch in batches])
-        else:
-            output_dict = _import_batch(
-                (first_spectrum_number, last_spectrum_number+1),
-                raw_file_path, self.centroided, dda=self.dda,
-                auxiliary_items = self.auxiliary_items,
-            )
-            peak_indices = np.empty(rawfile.LastSpectrumNumber + 1, np.int64)
-            peak_indices[0] = 0
-            peak_indices[1:] = np.cumsum(output_dict["_peak_indices"])
-            output_dict["peak_indices"] = peak_indices
-        rawfile.Close()
-
-        return output_dict
-
+def _get_mono_and_charge(trailer_data, scan_event):
+    mono = float(trailer_data['Monoisotopic M/Z:'].strip())
+    charge = int(trailer_data['Charge State:'].strip())
+    return mono, charge
 
 ms_reader_provider.register_reader("thermo", ThermoRawData)
 ms_reader_provider.register_reader("thermo_raw", ThermoRawData)
```

### Comparing `alpharaw-0.4.3/alpharaw/utils/centroiding.py` & `alpharaw-0.4.5/alpharaw/utils/centroiding.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/utils/df_processing.py` & `alpharaw-0.4.5/alpharaw/utils/df_processing.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/utils/ms_path_utils.py` & `alpharaw-0.4.5/alpharaw/utils/ms_path_utils.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/utils/timstof.py` & `alpharaw-0.4.5/alpharaw/utils/timstof.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/viz/df_utils.py` & `alpharaw-0.4.5/alpharaw/viz/df_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     fragment_intensity_df:pd.DataFrame=None,
     include_precursor_isotopes:bool=False,
     max_isotope:int = 6,
     min_frag_mz:float = 100.0,
     match_mode:typing.Literal["closest","highest"]="closest",
 )->pd.DataFrame:
     
-    plot_df = make_xic_plot_df_for_peptide(
+    plot_df = make_query_plot_df_for_peptide(
         sequence, mods, mod_sites, charge,
         rt_sec=rt_sec, mobility=mobility,
         charged_frag_types=charged_frag_types,
         include_fragments=include_fragments,
         fragment_intensity_df=fragment_intensity_df,
         include_precursor_isotopes=include_precursor_isotopes,
         max_isotope=max_isotope,
@@ -63,15 +63,15 @@
         modified_sequence = plot_df.modified_sequence.values[0],
         mod_sites=mod_sites,
         query_intensities = plot_df.intensity.values 
             if "intensity" in plot_df.columns else None,
         match_mode = match_mode,    
     )
 
-def make_xic_plot_df_for_peptide(
+def make_query_plot_df_for_peptide(
     sequence: str,
     mods: str,
     mod_sites: str,
     charge: int,
     rt_sec: float = 0.0,
     mobility: float = 0.0,
     ms_level:int=2,
@@ -95,35 +95,35 @@
         columns = np.intersect1d(
             fragment_mz_df.columns.values,
             fragment_intensity_df.columns.values,
         )
         fragment_mz_df = fragment_mz_df[columns]
         fragment_intensity_df = fragment_intensity_df[columns]
         
-    return translate_precursor_fragment_df_to_plot_df(
+    return translate_frag_df_to_plot_df(
         precursor_df, fragment_mz_df,
         fragment_intensity_df=fragment_intensity_df,
         rt_sec=rt_sec,
         mobility=mobility,
         ms_level=ms_level,
         min_frag_mz=min_frag_mz,
     )
 
-def make_psm_plot_for_dfs(
+def make_psm_plot_for_frag_dfs(
     spec_masses:np.ndarray,
     spec_intensities:np.ndarray,
     precursor_df:pd.DataFrame, 
     fragment_mz_df:pd.DataFrame,
     fragment_intensity_df:pd.DataFrame = None,
     ppm:float = 20.0,
     min_frag_mz: float = 100.0,
     min_frag_intensity: float = 0.001,
     match_mode:typing.Literal["closest","highest"]="closest",
 ):
-    plot_df = translate_precursor_fragment_df_to_plot_df(
+    plot_df = translate_frag_df_to_plot_df(
         precursor_df, 
         fragment_mz_df,
         fragment_intensity_df=fragment_intensity_df,
         min_frag_mz = min_frag_mz,
         min_frag_intensity=min_frag_intensity
     )
 
@@ -137,15 +137,15 @@
         modified_sequence = plot_df.modified_sequence.values[0],
         mod_sites=precursor_df.mod_sites.values[0],
         query_intensities = plot_df.intensity.values 
             if "intensity" in plot_df.columns else None,
         match_mode = match_mode,    
     )
 
-def make_xic_plot_df(
+def make_query_plot_df(
     query_masses:np.ndarray,
     query_ion_names:typing.List[str],
     query_rt_sec:float, 
     precursor_mz:float,
     query_im:float = 0.0,
     query_intensities:np.ndarray = None,
 )->pd.DataFrame:
@@ -271,15 +271,15 @@
                 +mod_seq[i+1:]
             )
     if charge != 0:
         return mod_seq + f"({charge}+)"
     else:
         return mod_seq
 
-def translate_precursor_fragment_df_to_plot_df(
+def translate_frag_df_to_plot_df(
     precursor_df:pd.DataFrame, 
     fragment_mz_df:pd.DataFrame, 
     fragment_intensity_df:pd.DataFrame = None,
     rt_sec:float = 0.0, 
     mobility:float = 0.0,
     ms_level:int = 2,
     min_frag_mz:float = 100.0,
@@ -362,14 +362,18 @@
     if rt_sec:
         fragment_df["rt_sec"] = rt_sec
     if mobility:
         fragment_df["im"] = mobility
 
     if ms_level == 2:
         fragment_df["precursor_mz"] = precursor_df.precursor_mz.values[0]
+        for iso in isotope_names:
+            fragment_df[f"precursor_{iso}"] = precursor_df[iso].values[0]
+        if len(isotope_names) > 0:
+            fragment_df[f"precursor_mono_idx"] = precursor_df.mono_isotope_idx.values[0]
 
     return fragment_df
     
 def make_precursor_fragment_df(
     sequence: str,
     mods: str,
     mod_sites: str,
```

### Comparing `alpharaw-0.4.3/alpharaw/viz/plot_utils.py` & `alpharaw-0.4.5/alpharaw/viz/plot_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,68 @@
     )
 
 alphatims_labels = {
     'rt': "rt_values",
     'im': "mobility_values",
 }
 
-def plot_line_fast(
+
+def plot_line_tims(
+    tims_data:TimsTOF,
+    tims_raw_indices: np.ndarray,
+    tims_view_indices: np.array,
+    name: str,
+    legend_group:str,
+    marker_color: str,
+    view_dim:typing.Literal['rt','im']='rt', # or 'im'
+    intensity_scale:float=1.0,
+    rt_unit:str = "minute"
+):
+    """Plot an XIC as a lineplot.
+
+    Parameters
+    ----------
+    tims_data : alphatims.bruker.TimsTOF
+        An alphatims.bruker.TimsTOF data object.
+    selected_indices : np.ndarray
+        The raw indices of tims_data that are selected for this plot.
+    label : str
+        The label for the line plot.
+    remove_zeros : bool
+        If True, zeros are removed. Default: False.
+    trim : bool
+        If True, zeros on the left and right are trimmed. Default: True.
+
+    Returns
+    -------
+    go.Figure
+        the XIC line plot.
+    """
+
+    x_dimension = alphatims_labels[view_dim]
+
+    intensities = tims_data.bin_intensities(tims_raw_indices, [x_dimension])
+    if view_dim == 'rt': 
+        x_ticks = tims_data.rt_values[tims_view_indices]
+        intensities = intensities[tims_view_indices]
+        if rt_unit == "minute":
+            x_ticks /= 60.0
+    else: 
+        x_ticks = tims_data.mobility_values[tims_view_indices]
+        intensities = intensities[tims_view_indices]
+
+    return plot_line(
+        x_ticks, intensities*intensity_scale,
+        name=name, 
+        marker_color=marker_color,
+        legend_group=legend_group,
+        x_text=view_dim.upper(),
+    )
+
+def plot_line_tims_fast(
     tims_data:TimsTOF,
     tims_raw_indices: np.ndarray,
     tims_view_indices: np.array,
     name: str,
     legend_group:str,
     marker_color: str,
     view_dim:typing.Literal['rt','im']='rt', # or 'im'
@@ -87,15 +140,15 @@
 
 def plot_line(
     x_values: np.ndarray,
     y_values: np.ndarray,
     name: str,
     marker_color: str,
     legend_group:str,
-    x_text: str = "RT (Sec)",
+    x_text: str = "RT",
     hovertemplate: str='%{text} <br><b>Intensity:</b> %{y}',
 ):
     return go.Scatter(
         x=x_values,
         y=y_values,
         mode='lines',
         name=name,
```

### Comparing `alpharaw-0.4.3/alpharaw/viz/psm_plot.py` & `alpharaw-0.4.5/alpharaw/viz/psm_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import typing
 
 import plotly.graph_objects as go
 
 from .plot_utils import plot_scatter
 from .df_utils import (
-    make_psm_plot_df, make_xic_plot_df_for_peptide, 
+    make_psm_plot_df, make_query_plot_df_for_peptide, 
 )
 
 color_map:dict = defaultdict(lambda:"brown")
 color_map.update({
     '-': 'lightgrey', # umnatched peaks
     'a': 'darkskyblue',
     'b': 'blue', 
@@ -44,15 +44,15 @@
     plot_unmatched_peaks = True,
     match_mode:typing.Literal["closest","highest"]="closest",
     plot_template = 'plotly_white',
     plot_height = 600,
     query_left_margin:float = 100000.0,
     query_right_margin:float = 100000.0,
 ):
-    plot_df = make_xic_plot_df_for_peptide(
+    plot_df = make_query_plot_df_for_peptide(
         sequence, mods, mod_sites, charge,
         charged_frag_types=charged_frag_types,
         include_fragments=include_fragments,
         include_precursor_isotopes=include_precursor_isotopes,
         max_isotope=max_isotope,
         min_frag_mz=min_frag_mz,
     )
@@ -371,14 +371,16 @@
                     hovertext=None,
                     hovertemplate=None,
                     name='',
                 ),
                 row=self.row,
                 col=self.col,
             )
+        else:
+            plot_df = plot_df.query('ion_name != "-"')
 
         matched_df = plot_df.query('ion_name != "-"')
         for color, df in matched_df.groupby("color"):
             self._plot_one_ion_type_scatter(
                 df, color
             )
```

### Comparing `alpharaw-0.4.3/alpharaw/viz/xic_plot.py` & `alpharaw-0.4.5/alpharaw/viz/xic_plot_tims.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 from plotly.subplots import make_subplots
 
 from alphatims.bruker import (
     TimsTOF, 
 )
 
 from .plot_utils import (
-    plot_line_fast
+    plot_line_tims_fast
 )
 
-class XIC_Plot():
+class XIC_Plot_Tims():
     # hovermode = "x" | "y" | "closest" | False | "x unified" | "y unified"
     hovermode = 'closest'
     plot_height = 550
     colorscale_qualitative="Alphabet"
     colorscale_sequential="Viridis"
     theme_template='plotly_white'
     ms1_ppm = 20.0
     ms2_ppm = 20.0
     rt_sec_win = 30.0
     plot_rt_unit:str = "minute"
     im_win = 0.05
     fig:go.Figure = None
 
-    "list of XIC_Trace objects"
+    #list of XIC_Trace objects
     traces:list = []
 
     def plot(self, 
         tims_data:TimsTOF,
         query_df:pd.DataFrame,
         view_dim:typing.Literal["rt","im"]="rt",
         title:str="",
@@ -78,46 +78,47 @@
             cols=1,
             shared_xaxes=True,
             x_title=f'RT ({self.plot_rt_unit})' if view_dim == 'rt' else 'Mobility',
             y_title='intensity',
             vertical_spacing=0.2/rows,
         )
         self.traces = [
-            XIC_Trace(fig=self.fig, row=i+1) 
+            XIC_Trace_Tims(fig=self.fig, row=i+1) 
             for i in range(rows)
         ]
 
     def plot_query_masses(self,
         tims_data:TimsTOF,
         query_masses:np.ndarray,
         query_ion_names:typing.List[str],
         query_rt_sec:float, 
         query_im:float,
-        precursor_mz:float,
+        precursor_left_mz:float,
+        precursor_right_mz:float,
         marker_colors:list = None,
         view_dim:typing.Literal["rt","im"]="rt",
         query_intensities:np.ndarray = None,
         title="",
     ):
         self._init_plot(rows=1, view_dim=view_dim)
         mass_tols = query_masses*1e-6*(
-            self.ms1_ppm if precursor_mz == 0 else self.ms2_ppm
+            self.ms1_ppm if precursor_left_mz <= 0 else self.ms2_ppm
         )
         if marker_colors is None:
             marker_colors = self._get_color_set(len(query_masses))
         self.traces[0].add_traces(
             tims_data=tims_data,
             query_masses=query_masses,
             mass_tols=mass_tols,
             ion_names=query_ion_names,
             marker_colors=marker_colors,
             query_rt_sec=query_rt_sec,
             query_im=query_im,
-            precursor_mz=precursor_mz,
-            precursor_mz_tol=precursor_mz*1e-6*self.ms1_ppm,
+            precursor_left_mz=precursor_left_mz,
+            precursor_right_mz=precursor_right_mz,
             view_dim=view_dim,
             rt_sec_win=self.rt_sec_win,
             im_win=self.im_win,
             query_intensities=query_intensities,
         )
         self.fig.update_layout(
             template=self.theme_template,
@@ -142,16 +143,15 @@
         else:
             color_set = px.colors.sample_colorscale(
                 self.colorscale_sequential, 
                 samplepoints=n_query
             )
         return color_set
 
-
-class XIC_Trace():
+class XIC_Trace_Tims():
     label_format = '{ion_name} {mz:.3f}'
     legend_group = '{ion_name}' # {ion_name}, {mz} or None
     fig:go.Figure
     row:int = 1
     col:int = 1
     plot_rt_unit:str = "minute"
 
@@ -169,16 +169,16 @@
         tims_data:TimsTOF,
         query_masses:np.ndarray,
         mass_tols:np.ndarray,
         ion_names:typing.List[str],
         marker_colors:typing.List,
         query_rt_sec:float, 
         query_im:float,
-        precursor_mz:float = 0.0,
-        precursor_mz_tol:float = 0.02,
+        precursor_left_mz:float = -1.0,
+        precursor_right_mz:float = -1.0,
         view_dim:typing.Literal["rt","im"]="rt",
         rt_sec_win = 30.0,
         im_win = 0.05,
         query_intensities:np.ndarray = None,
     )->go.Figure:
         """Add traces for the query_masses.
 
@@ -198,16 +198,16 @@
         (
             rt_slice, im_slice, prec_mz_slice, view_indices
         ) = get_plotting_slices(
             tims_data=tims_data, 
             rt_sec=query_rt_sec, 
             rt_sec_win=rt_sec_win,
             im=query_im, im_win=im_win,
-            precursor_mz=precursor_mz, 
-            precursor_mz_tol=precursor_mz_tol,
+            precursor_left_mz=precursor_left_mz,
+            precursor_right_mz=precursor_right_mz,
             view_dim=view_dim,
         )
 
         if query_intensities is None:
             query_intensities = np.zeros_like(query_masses)
         else:
             query_intensities /= query_intensities.max()
@@ -265,17 +265,17 @@
             prec_mz_slice,
             slice(
                 query_mass - mass_tol, 
                 query_mass + mass_tol,
             ),
             'raw'
         ]
-        if len(frag_indices) == 0: return self.fig
+        if len(frag_indices) == 0: return
         self.fig.add_trace(
-            plot_line_fast(
+            plot_line_tims_fast(
                 tims_data, 
                 frag_indices,
                 view_indices,
                 name=label,
                 legend_group=legend_group,
                 marker_color=marker_color, 
                 view_dim=view_dim,
@@ -284,16 +284,16 @@
             row=self.row, col=self.col,
         )
 
 def get_plotting_slices(
     tims_data: TimsTOF,
     rt_sec:float, rt_sec_win:float=30.0,
     im:float = 0., im_win:float = 0.05,
-    precursor_mz:float = 0.0,
-    precursor_mz_tol:float = 0.02,
+    precursor_left_mz:float = -1.0,
+    precursor_right_mz:float = -1.0,
     view_dim:str = "rt",
 ):
     """
     Get plotting slices for target queries in TimsTOF data.
     Args:
         tims_data (TimsTOF): AlphaTims TimsTOF object.
         rt_sec (float): Query RT in seconds.
@@ -309,27 +309,27 @@
         rt_sec + rt_sec_win/2
     )
     im_slice = slice(
         im - im_win/2, 
         im + im_win/2
     )
 
-    if precursor_mz == 0:
+    if precursor_left_mz <= 0:
         prec_mz_slice = 0
         raw_indices = tims_data[
             rt_slice,
             im_slice,
             0,
             :,
             'raw'
         ]
     else:
         prec_mz_slice = slice(
-            precursor_mz - precursor_mz_tol,
-            precursor_mz + precursor_mz_tol,
+            precursor_left_mz,
+            precursor_right_mz,
         )
         raw_indices = tims_data[
             rt_slice,
             im_slice,
             prec_mz_slice,
             :,
             'raw'
```

### Comparing `alpharaw-0.4.3/alpharaw/wrappers/alphapept_wrapper.py` & `alpharaw-0.4.5/alpharaw/wrappers/alphapept_wrapper.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw/wrappers/alphatims_wrapper.py` & `alpharaw-0.4.5/alpharaw/wrappers/alphatims_wrapper.py`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/alpharaw.egg-info/PKG-INFO` & `alpharaw-0.4.5/alpharaw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpharaw
-Version: 0.4.3
+Version: 0.4.5
 Summary: An open-source Python package to unify raw MS data access and storage.
 Home-page: https://github.com/MannLabs/alpharaw
 Author: Mann Labs
 Author-email: jalew.zwf@qq.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alpharaw
```

### Comparing `alpharaw-0.4.3/alpharaw.egg-info/SOURCES.txt` & `alpharaw-0.4.5/alpharaw.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,24 +63,26 @@
 alpharaw/legacy_msdata/__init__.py
 alpharaw/legacy_msdata/mgf.py
 alpharaw/match/__init__.py
 alpharaw/match/mass_calibration.py
 alpharaw/match/match_utils.py
 alpharaw/match/psm_match.py
 alpharaw/match/psm_match_alphatims.py
+alpharaw/match/spec_finder.py
 alpharaw/raw_access/__init__.py
 alpharaw/raw_access/clr_utils.py
 alpharaw/raw_access/pysciexwifffilereader.py
 alpharaw/raw_access/pythermorawfilereader.py
 alpharaw/utils/__init__.py
 alpharaw/utils/centroiding.py
 alpharaw/utils/df_processing.py
 alpharaw/utils/ms_path_utils.py
 alpharaw/utils/timstof.py
 alpharaw/viz/__init__.py
 alpharaw/viz/df_utils.py
 alpharaw/viz/plot_utils.py
 alpharaw/viz/psm_plot.py
 alpharaw/viz/xic_plot.py
+alpharaw/viz/xic_plot_tims.py
 alpharaw/wrappers/__init__.py
 alpharaw/wrappers/alphapept_wrapper.py
 alpharaw/wrappers/alphatims_wrapper.py
```

### Comparing `alpharaw-0.4.3/alpharaw.egg-info/requires.txt` & `alpharaw-0.4.5/alpharaw.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpharaw-0.4.3/setup.py` & `alpharaw-0.4.5/setup.py`

 * *Files identical despite different names*

