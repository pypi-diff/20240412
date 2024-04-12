# Comparing `tmp/legend_pydataobj-1.5.1.tar.gz` & `tmp/legend_pydataobj-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legend_pydataobj-1.5.1.tar", last modified: Fri Mar  1 10:36:35 2024, max compression
+gzip compressed data, was "legend_pydataobj-1.6.0.tar", last modified: Fri Apr 12 16:18:11 2024, max compression
```

## Comparing `legend_pydataobj-1.5.1.tar` & `legend_pydataobj-1.6.0.tar`

### file list

```diff
@@ -1,78 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.731744 legend_pydataobj-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-03-01 10:36:35.731744 legend_pydataobj-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 10:36:35.731744 legend_pydataobj-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.715744 legend_pydataobj-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.731744 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.719744 legend_pydataobj-1.5.1/src/lgdo/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-01 10:36:35.000000 legend_pydataobj-1.5.1/src/lgdo/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.723744 legend_pydataobj-1.5.1/src/lgdo/compression/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/radware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/compression/varlen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.723744 legend_pydataobj-1.5.1/src/lgdo/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    55673 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.723744 legend_pydataobj-1.5.1/src/lgdo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)    15304 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/lgdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15538 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28228 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/types/waveformtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/src/lgdo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.727744 legend_pydataobj-1.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.727744 legend_pydataobj-1.5.1/tests/compression/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.727744 legend_pydataobj-1.5.1/tests/compression/sigcompress/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/sigcompress/special-wf-clipped.dat
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/test_radware_sigcompress.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/test_str2wfcodec.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/compression/test_uleb128_zigzag_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.727744 legend_pydataobj-1.5.1/tests/lh5/
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/lh5/test_lh5_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    30121 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/lh5/test_lh5_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/lh5/test_lh5_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/test_lgdo_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 10:36:35.731744 legend_pydataobj-1.5.1/tests/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_arrayofequalsizedarrays.py
--rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_fixedsizearray.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_table_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_vectorofvectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-01 10:36:17.000000 legend_pydataobj-1.5.1/tests/types/test_waveformtable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.512980 legend_pydataobj-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-04-12 16:18:11.512980 legend_pydataobj-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 16:18:11.512980 legend_pydataobj-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.492980 legend_pydataobj-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.508980 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44355 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.496980 legend_pydataobj-1.6.0/src/lgdo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-12 16:18:11.000000 legend_pydataobj-1.6.0/src/lgdo/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8018 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.500980 legend_pydataobj-1.6.0/src/lgdo/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24015 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/radware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15127 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/compression/varlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.500980 legend_pydataobj-1.6.0/src/lgdo/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.500980 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.500980 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/read/vector_of_vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.500980 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8460 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/_serializers/write/vector_of_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10780 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12369 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6670 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.504980 legend_pydataobj-1.6.0/src/lgdo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/lgdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16887 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/types/waveformtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/src/lgdo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.504980 legend_pydataobj-1.6.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.504980 legend_pydataobj-1.6.0/tests/compression/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.504980 legend_pydataobj-1.6.0/tests/compression/sigcompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/sigcompress/special-wf-clipped.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48214 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/test_radware_sigcompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/test_str2wfcodec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/compression/test_uleb128_zigzag_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.508980 legend_pydataobj-1.6.0/tests/lh5/
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_datatype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14032 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/lh5/test_lh5_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/test_lgdo_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 16:18:11.508980 legend_pydataobj-1.6.0/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_arrayofequalsizedarrays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8134 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_fixedsizearray.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_table_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_vectorofvectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_vovutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-12 16:18:05.000000 legend_pydataobj-1.6.0/tests/types/test_waveformtable.py
```

### Comparing `legend_pydataobj-1.5.1/LICENSE` & `legend_pydataobj-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/PKG-INFO` & `legend_pydataobj-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.5.1
+Version: 1.6.0
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.5.1/README.md` & `legend_pydataobj-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/pyproject.toml` & `legend_pydataobj-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     "pylegendtestdata",
     "pytest>=6.0",
     "pytest-cov",
 ]
 
 [project.scripts]
 lh5ls = "lgdo.cli:lh5ls"
+lh5concat = "lgdo.cli:lh5concat"
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 license-files = [
     "LICENSE",
 ]
```

### Comparing `legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/PKG-INFO` & `legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: legend_pydataobj
-Version: 1.5.1
+Version: 1.6.0
 Summary: LEGEND Python Data Objects
 Author: The LEGEND Collaboration
 Maintainer: The LEGEND Collaboration
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `legend_pydataobj-1.5.1/src/legend_pydataobj.egg-info/SOURCES.txt` & `legend_pydataobj-1.6.0/src/legend_pydataobj.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -19,46 +19,70 @@
 src/lgdo/compression/__init__.py
 src/lgdo/compression/base.py
 src/lgdo/compression/generic.py
 src/lgdo/compression/radware.py
 src/lgdo/compression/utils.py
 src/lgdo/compression/varlen.py
 src/lgdo/lh5/__init__.py
+src/lgdo/lh5/core.py
+src/lgdo/lh5/datatype.py
+src/lgdo/lh5/exceptions.py
 src/lgdo/lh5/iterator.py
 src/lgdo/lh5/store.py
 src/lgdo/lh5/tools.py
 src/lgdo/lh5/utils.py
+src/lgdo/lh5/_serializers/__init__.py
+src/lgdo/lh5/_serializers/read/__init__.py
+src/lgdo/lh5/_serializers/read/array.py
+src/lgdo/lh5/_serializers/read/composite.py
+src/lgdo/lh5/_serializers/read/encoded.py
+src/lgdo/lh5/_serializers/read/ndarray.py
+src/lgdo/lh5/_serializers/read/scalar.py
+src/lgdo/lh5/_serializers/read/utils.py
+src/lgdo/lh5/_serializers/read/vector_of_vectors.py
+src/lgdo/lh5/_serializers/write/__init__.py
+src/lgdo/lh5/_serializers/write/array.py
+src/lgdo/lh5/_serializers/write/composite.py
+src/lgdo/lh5/_serializers/write/scalar.py
+src/lgdo/lh5/_serializers/write/vector_of_vectors.py
 src/lgdo/types/__init__.py
 src/lgdo/types/array.py
 src/lgdo/types/arrayofequalsizedarrays.py
 src/lgdo/types/encoded.py
 src/lgdo/types/fixedsizearray.py
 src/lgdo/types/lgdo.py
 src/lgdo/types/scalar.py
 src/lgdo/types/struct.py
 src/lgdo/types/table.py
 src/lgdo/types/vectorofvectors.py
+src/lgdo/types/vovutils.py
 src/lgdo/types/waveformtable.py
 tests/conftest.py
 tests/test_cli.py
 tests/test_lgdo_utils.py
 tests/compression/conftest.py
 tests/compression/test_compression.py
 tests/compression/test_radware_sigcompress.py
 tests/compression/test_str2wfcodec.py
 tests/compression/test_uleb128_zigzag_diff.py
 tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat
 tests/compression/sigcompress/special-wf-clipped.dat
+tests/lh5/conftest.py
+tests/lh5/test_core.py
+tests/lh5/test_lh5_datatype.py
 tests/lh5/test_lh5_iterator.py
 tests/lh5/test_lh5_store.py
+tests/lh5/test_lh5_tools.py
 tests/lh5/test_lh5_utils.py
+tests/lh5/test_lh5_write.py
 tests/types/test_array.py
 tests/types/test_arrayofequalsizedarrays.py
 tests/types/test_encoded.py
 tests/types/test_fixedsizearray.py
 tests/types/test_representations.py
 tests/types/test_scalar.py
 tests/types/test_struct.py
 tests/types/test_table.py
 tests/types/test_table_eval.py
 tests/types/test_vectorofvectors.py
+tests/types/test_vovutils.py
 tests/types/test_waveformtable.py
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/__init__.py` & `legend_pydataobj-1.6.0/src/lgdo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,20 @@
   attribute
 * :class:`.Array`: basic :class:`numpy.ndarray`. Access data via the
   :attr:`nda` attribute.
 * :class:`.FixedSizeArray`: basic :class:`numpy.ndarray`. Access data via the
   :attr:`nda` attribute.
 * :class:`.ArrayOfEqualSizedArrays`: multi-dimensional :class:`numpy.ndarray`.
   Access data via the :attr:`nda` attribute.
-* :class:`.VectorOfVectors`: a variable length array of variable length arrays.
-  Implemented as a pair of :class:`.Array`: :attr:`flattened_data` holding the
-  raw data, and :attr:`cumulative_length` whose ith element is the sum of the
-  lengths of the vectors with ``index <= i``
+* :class:`.VectorOfVectors`: an n-dimensional variable length array of variable
+  length arrays.  Implemented as a pair of datasets: :attr:`flattened_data`
+  holding the raw data (:class:`.Array` or :class:`.VectorOfVectors`, if the
+  vector dimension is greater than 2), and :attr:`cumulative_length` (always an
+  :class:`.Array`) whose i-th element is the sum of the lengths of the vectors
+  with ``index <= i``
 * :class:`.VectorOfEncodedVectors`: an array of variable length *encoded*
   arrays. Implemented as a :class:`.VectorOfVectors` :attr:`encoded_data`
   holding the encoded vectors and an :class:`.Array` :attr:`decoded_size`
   specifying the size of each decoded vector. Mainly used to represent a list
   of compressed waveforms.
 * :class:`.ArrayOfEncodedEqualSizedArrays`: an array of equal sized encoded
   arrays. Similar to :class:`.VectorOfEncodedVectors` except for
@@ -33,14 +35,15 @@
   types with the same length (number of rows)
 
 Currently the primary on-disk format for LGDO object is LEGEND HDF5 (LH5) files. IO
 is done via the class :class:`.lh5_store.LH5Store`. LH5 files can also be
 browsed easily in python like any `HDF5 <https://www.hdfgroup.org>`_ file using
 `h5py <https://www.h5py.org>`_.
 """
+
 from __future__ import annotations
 
 from ._version import version as __version__
 from .lh5_store import LH5Iterator, LH5Store, load_dfs, load_nda, ls, show
 from .types import (
     LGDO,
     Array,
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/__init__.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 interface for encoding/decoding :class:`~.lgdo.LGDO`\ s.
 
 >>> from lgdo import WaveformTable, compression
 >>> wftbl = WaveformTable(...)
 >>> enc_wft = compression.encode(wftable, RadwareSigcompress(codec_shift=-23768)
 >>> compression.decode(enc_wft) # == wftbl
 """
+
 from __future__ import annotations
 
 from .base import WaveformCodec
 from .generic import decode, encode
 from .radware import RadwareSigcompress
 from .varlen import ULEB128ZigZagDiff
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/base.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/base.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/generic.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/generic.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/radware.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/radware.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/utils.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/compression/varlen.py` & `legend_pydataobj-1.6.0/src/lgdo/compression/varlen.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/lgdo_utils.py` & `legend_pydataobj-1.6.0/src/lgdo/lgdo_utils.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/lh5/iterator.py` & `legend_pydataobj-1.6.0/src/lgdo/lh5/iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             one for each file. Ignore if a selection list is provided.
         field_mask
             mask of which fields to read. See :meth:`LH5Store.read` for
             more details.
         buffer_len
             number of entries to read at a time while iterating through files.
         friend
-            a ''friend'' LH5Iterator that will be read in parallel with this.
+            a \"friend\" LH5Iterator that will be read in parallel with this.
             The friend should have the same length and entry list. A single
             LH5 table containing columns from both iterators will be returned.
         """
         self.lh5_st = LH5Store(base_path=base_path, keep_open=True)
 
         # List of files, with wildcards and env vars expanded
         if isinstance(lh5_files, str):
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/lh5/tools.py` & `legend_pydataobj-1.6.0/src/lgdo/lh5/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 import fnmatch
 import glob
-import inspect
 import logging
 import os
-from collections.abc import Iterable
-from typing import Any
+from copy import copy
 from warnings import warn
 
 import h5py
 import numpy as np
 import pandas as pd
 from numpy.typing import NDArray
 
 from . import utils
 from .store import LH5Store
 
 log = logging.getLogger(__name__)
 
 
-def ls(lh5_file: str | h5py.Group, lh5_group: str = "") -> list[str]:
+def ls(
+    lh5_file: str | h5py.Group,
+    lh5_group: str = "",
+    recursive: bool = False,
+) -> list[str]:
     """Return a list of LH5 groups in the input file and group, similar
     to ``ls`` or ``h5ls``. Supports wildcards in group names.
 
 
     Parameters
     ----------
     lh5_file
         name of file.
     lh5_group
         group to search. add a ``/`` to the end of the group name if you want to
         list all objects inside that group.
+    recursive
+        if ``True``, recurse into subgroups.
     """
 
     log.debug(
         f"Listing objects in '{lh5_file}'"
         + ("" if lh5_group == "" else f" (and group {lh5_group})")
     )
 
@@ -45,23 +49,38 @@
         lh5_file = lh5_st.gimme_file(lh5_file, "r")
         if lh5_group.startswith("/"):
             lh5_group = lh5_group[1:]
 
     if lh5_group == "":
         lh5_group = "*"
 
+    # get the first group in the group path
     splitpath = lh5_group.split("/", 1)
+    # filter out objects that don't match lh5_group pattern
     matchingkeys = fnmatch.filter(lh5_file.keys(), splitpath[0])
 
+    ret = []
+    # if there were no "/" in lh5_group just return the result
     if len(splitpath) == 1:
-        return matchingkeys
+        ret = matchingkeys
+
+    else:
+        for key in matchingkeys:
+            ret.extend([f"{key}/{path}" for path in ls(lh5_file[key], splitpath[1])])
+
+    if recursive:
+        rec_ret = copy(ret)
+        for obj in ret:
+            try:
+                rec_ret += ls(lh5_file, lh5_group=f"{obj}/", recursive=True)
+            except AttributeError:
+                continue
+
+        return rec_ret
 
-    ret = []
-    for key in matchingkeys:
-        ret.extend([f"{key}/{path}" for path in ls(lh5_file[key], splitpath[1])])
     return ret
 
 
 def show(
     lh5_file: str | h5py.Group,
     lh5_group: str = "/",
     attrs: bool = False,
@@ -165,59 +184,14 @@
         # break or move to next key
         if killme:
             break
 
         key = k_new
 
 
-def read_as(
-    name: str,
-    lh5_file: str | h5py.File | Iterable[str | h5py.File],
-    library: str,
-    **kwargs,
-) -> Any:
-    """Read LH5 data from disk straight into a third-party data format view.
-
-    This function is nothing more than a shortcut chained call to
-    :meth:`.LH5Store.read` and to :meth:`.LGDO.view_as`.
-
-    Parameters
-    ----------
-    name
-        LH5 object name on disk.
-    lh5_file
-        LH5 file name.
-    library
-        string ID of the third-party data format library (``np``, ``pd``,
-        ``ak``, etc).
-
-    See Also
-    --------
-    .LH5Store.read, .LGDO.view_as
-    """
-    # determine which keyword arguments should be forwarded to read() and which
-    # should be forwarded to view_as()
-    read_kwargs = inspect.signature(LH5Store.read).parameters.keys()
-
-    kwargs1 = {}
-    kwargs2 = {}
-    for k, v in kwargs.items():
-        if k in read_kwargs:
-            kwargs1[k] = v
-        else:
-            kwargs2[k] = v
-
-    # read the LGDO from disk
-    store = LH5Store()
-    obj, _ = store.read(name, lh5_file, **kwargs1)
-
-    # and finally return a view
-    return obj.view_as(library, **kwargs2)
-
-
 def load_nda(
     f_list: str | list[str],
     par_list: list[str],
     lh5_group: str = "",
     idx_list: list[NDArray | list | tuple] | None = None,
 ) -> dict[str, NDArray]:
     r"""Build a dictionary of :class:`numpy.ndarray`\ s from LH5 data.
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/lh5_store.py` & `legend_pydataobj-1.6.0/src/lgdo/lh5_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 .. warning::
     This subpackage is deprecated, use :mod:`lgdo.lh5`.
 """
+
 from __future__ import annotations
 
 import sys
 from collections.abc import Iterator
 from typing import Union
 from warnings import warn
 
@@ -23,23 +24,22 @@
     Struct,
     Table,  # noqa: F401
     VectorOfEncodedVectors,  # noqa: F401
     VectorOfVectors,
     WaveformTable,  # noqa: F401
 )
 
-DEFAULT_HDF5_COMPRESSION = None
 LGDO = Union[Array, Scalar, Struct, VectorOfVectors]
-DEFAULT_HDF5_SETTINGS: dict[str, ...] = {"shuffle": True, "compression": "gzip"}
 
 
 class LH5Iterator(lh5.LH5Iterator):
     """
     .. warning::
         This class is deprecated, use :class:`lgdo.lh5.iterator.LH5Iterator`.
+
     """
 
     def __init__(
         self,
         lh5_files: str | list[str],
         groups: str | list[str],
         base_path: str = "",
@@ -78,14 +78,15 @@
         wo_mode: str = "append",
         write_start: int = 0,
         **h5py_kwargs,
     ) -> None:
         """
         .. warning::
             This method is deprecated, use :meth:`lgdo.lh5.iterator.LH5Iterator.write`.
+
         """
         warn(
             "lgdo.lh5_store has moved to a subfolder lgdo.lh5 containing LH5Iterator. "
             "The object you are calling this function from uses the old LH5Iterator class."
             "Please replace 'from lgdo.lh5_store import LH5Iterator' with 'from lgdo.lh5 import LH5Iterator'."
             "lgdo.lh5_store will be removed in a future release.",
             DeprecationWarning,
@@ -114,14 +115,15 @@
         obj_buf: LGDO = None,
         obj_buf_start: int = 0,
         decompress: bool = True,
     ) -> tuple[LGDO, int]:
         """
         .. warning::
             This method is deprecated, use :meth:`lgdo.lh5.iterator.LH5Iterator.read`.
+
         """
         warn(
             "lgdo.lh5_store has moved to a subfolder lgdo.lh5 containing LH5Iterator. "
             "The object you are calling this function from uses the old LH5Iterator class."
             "Please replace 'from lgdo.lh5_store import LH5Iterator' with 'from lgdo.lh5 import LH5Iterator'."
             "lgdo.lh5_store will be removed in a future release.",
             DeprecationWarning,
@@ -140,14 +142,15 @@
         )
 
 
 class LH5Store(lh5.LH5Store):
     """
     .. warning::
         This class is deprecated, use :class:`lgdo.lh5.iterator.LH5Store`.
+
     """
 
     def __init__(self, base_path: str = "", keep_open: bool = False):
         warn(
             "lgdo.lh5_store has moved to a subfolder lgdo.lh5 containing LH5Store. "
             "Please replace 'from lgdo.lh5_store import LH5Store' with 'from lgdo.lh5 import LH5Store'."
             "lgdo.lh5_store will be removed in a future release.",
@@ -161,14 +164,15 @@
         name: str,
         lh5_file: str | h5py.File | list[str | h5py.File],
         **kwargs,
     ) -> tuple[LGDO, int]:
         """
         .. warning::
             This method is deprecated, use :meth:`lgdo.lh5.store.LH5Store.read`.
+
         """
         warn(
             "LH5Store.read_object() has been renamed to LH5Store.read(), "
             "Please update your code."
             "LH5Store.read_object() will be removed in a future release.",
             DeprecationWarning,
             stacklevel=2,
@@ -181,14 +185,15 @@
         name: str,
         lh5_file: str | h5py.File,
         **kwargs,
     ) -> tuple[LGDO, int]:
         """
         .. warning::
             This method is deprecated, use :meth:`lgdo.lh5.store.LH5Store.write`.
+
         """
         warn(
             "LH5Store.write_object() has been renamed to LH5Store.write(), "
             "Please update your code."
             "LH5Store.write_object() will be removed in a future release.",
             DeprecationWarning,
             stacklevel=2,
@@ -202,14 +207,15 @@
     lh5_group: str = "",
     idx_list: list[np.ndarray | list | tuple] | None = None,
 ) -> pd.DataFrame:
     """
     .. warning::
         This function is deprecated, use :meth:`lgdo.types.lgdo.LGDO.view_as` to
         view LGDO data as a Pandas data structure.
+
     """
     warn(
         "lgdo.lh5_store has moved to a subfolder lgdo.lh5. "
         "Please replace 'from lgdo.lh5_store import load_dfs' with 'from lgdo.lh5 import load_dfs'. "
         "lgdo.lh5_store will be removed in a future release.",
         DeprecationWarning,
         stacklevel=2,
@@ -223,14 +229,15 @@
     lh5_group: str = "",
     idx_list: list[np.ndarray | list | tuple] | None = None,
 ) -> dict[str, np.ndarray]:
     """
     .. warning::
         This function is deprecated, use :meth:`lgdo.types.lgdo.LGDO.view_as` to
         view LGDO data as a NumPy data structure.
+
     """
     warn(
         "lgdo.lh5_store has moved to a subfolder lgdo.lh5. "
         "Please replace 'from lgdo.lh5_store import load_nda' with 'from lgdo.lh5 import load_nda'. "
         "lgdo.lh5_store will be removed in a future release.",
         DeprecationWarning,
         stacklevel=2,
@@ -238,14 +245,15 @@
     return lh5.load_nda(f_list, par_list, lh5_group, idx_list)
 
 
 def ls(lh5_file: str | h5py.Group, lh5_group: str = "") -> list[str]:
     """
     .. warning::
         This function is deprecated, import :func:`lgdo.lh5.tools.ls`.
+
     """
     warn(
         "lgdo.lh5_store has moved to a subfolder lgdo.lh5. "
         "Please replace 'from lgdo.lh5_store import ls' with 'from lgdo.lh5 import ls'. "
         "lgdo.lh5_store will be removed in a future release.",
         DeprecationWarning,
         stacklevel=2,
@@ -259,14 +267,15 @@
     attrs: bool = False,
     indent: str = "",
     header: bool = True,
 ) -> None:
     """
     .. warning::
         This function is deprecated, import :func:`lgdo.lh5.tools.show`.
+
     """
     warn(
         "lgdo.lh5_store has moved to a subfolder lgdo.lh5. "
         "Please replace 'from lgdo.lh5_store import show' with 'from lgdo.lh5 import show'. "
         "lgdo.lh5_store will be removed in a future release.",
         DeprecationWarning,
         stacklevel=2,
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/logging.py` & `legend_pydataobj-1.6.0/src/lgdo/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements some helpers for setting up logging."""
+
 from __future__ import annotations
 
 import logging
 
 import colorlog
 
 DEBUG = logging.DEBUG
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/__init__.py` & `legend_pydataobj-1.6.0/src/lgdo/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """LEGEND Data Objects (LGDO) types."""
+
 from __future__ import annotations
 
 from .array import Array
 from .arrayofequalsizedarrays import ArrayOfEqualSizedArrays
 from .encoded import ArrayOfEncodedEqualSizedArrays, VectorOfEncodedVectors
 from .fixedsizearray import FixedSizeArray
 from .lgdo import LGDO
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/array.py` & `legend_pydataobj-1.6.0/src/lgdo/types/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implements a LEGEND Data Object representing an n-dimensional array and
 corresponding utilities.
 """
+
 from __future__ import annotations
 
 import logging
 from collections.abc import Iterator
 from typing import Any
 
 import awkward as ak
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/arrayofequalsizedarrays.py` & `legend_pydataobj-1.6.0/src/lgdo/types/arrayofequalsizedarrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implements a LEGEND Data Object representing an array of equal-sized arrays and
 corresponding utilities.
 """
+
 from __future__ import annotations
 
 from collections.abc import Iterator
 from typing import Any
 
 import awkward as ak
 import numpy as np
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/encoded.py` & `legend_pydataobj-1.6.0/src/lgdo/types/encoded.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,16 @@
         return (self.encoded_data[i], self.decoded_size[i])
 
     def __iter__(self) -> Iterator[tuple[NDArray, int]]:
         yield from zip(self.encoded_data, self.decoded_size)
 
     def __str__(self) -> str:
         string = ""
-        pos = 0
-        for vec, size in self:
+        for pos, res in enumerate(self):
+            vec, size = res[0], res[1]
             if pos != 0:
                 string += " "
 
             string += (
                 np.array2string(
                     vec,
                     prefix=" ",
@@ -196,16 +196,14 @@
                 )
                 + f" decoded_size = {size}"
             )
 
             if pos < len(self.encoded_data.cumulative_length):
                 string += ",\n"
 
-            pos += 1
-
         string = f"[{string}]"
 
         attrs = self.getattrs()
         if len(attrs) > 0:
             string += f" with attrs={attrs}"
 
         return string
@@ -396,16 +394,15 @@
         return self.encoded_data[i]
 
     def __iter__(self) -> Iterator[NDArray]:
         yield from self.encoded_data
 
     def __str__(self) -> str:
         string = ""
-        pos = 0
-        for vec in self:
+        for pos, vec in enumerate(self):
             if pos != 0:
                 string += " "
 
             string += np.array2string(
                 vec,
                 prefix=" ",
                 formatter={
@@ -414,16 +411,14 @@
                     else str(x)
                 },
             )
 
             if pos < len(self.encoded_data.cumulative_length):
                 string += ",\n"
 
-            pos += 1
-
         string = f"[{string}] decoded_size={self.decoded_size}"
 
         attrs = self.getattrs()
         if len(attrs) > 0:
             string += f" with attrs={attrs}"
 
         return string
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/fixedsizearray.py` & `legend_pydataobj-1.6.0/src/lgdo/types/fixedsizearray.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implements a LEGEND Data Object representing an n-dimensional array of fixed
 size and corresponding utilities.
 """
+
 from __future__ import annotations
 
 from typing import Any
 
 import numpy as np
 
 from .array import Array
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/lgdo.py` & `legend_pydataobj-1.6.0/src/lgdo/types/lgdo.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/scalar.py` & `legend_pydataobj-1.6.0/src/lgdo/types/scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/struct.py` & `legend_pydataobj-1.6.0/src/lgdo/types/struct.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implements a LEGEND Data Object representing a struct and corresponding
 utilities.
 """
+
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import numpy as np
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/table.py` & `legend_pydataobj-1.6.0/src/lgdo/types/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Implements a LEGEND Data Object representing a special struct of arrays of
 equal length and corresponding utilities.
 """
+
 from __future__ import annotations
 
 import logging
 from collections.abc import Mapping
 from typing import Any
 from warnings import warn
 
@@ -225,27 +226,57 @@
             "Instead use `view_as` to get the Table data as a pandas dataframe "
             "or awkward Array. ",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.view_as(library="pd", cols=cols, prefix=prefix)
 
+    def flatten(self, _prefix="") -> Table:
+        """Flatten the table, if nested.
+
+        Returns a new :class:`Table` (that references, not copies, the existing
+        columns) with columns in nested tables being moved to the first level
+        (and renamed appropriately).
+
+        Examples
+        --------
+        >>> repr(tbl)
+        "Table(dict={'a': Array([1 2 3], attrs={'datatype': 'array<1>{real}'}), 'tbl': Table(dict={'b': Array([4 5 6], attrs={'datatype': 'array<1>{real}'}), 'tbl1': Table(dict={'z': Array([9 9 9], attrs={'datatype': 'array<1>{real}'})}, attrs={'datatype': 'table{z}'})}, attrs={'datatype': 'table{b,tbl1}'})}, attrs={'datatype': 'table{a,tbl}'})"
+        >>> tbl.flatten().keys()
+        dict_keys(['a', 'tbl__b', 'tbl__tbl1__z'])
+        """
+        flat_table = Table(size=self.size)
+        for key, obj in self.items():
+            if isinstance(obj, Table):
+                flat_table.join(obj.flatten(_prefix=f"{_prefix}{key}__"))
+            else:
+                flat_table.add_column(_prefix + key, obj)
+
+        return flat_table
+
     def eval(
         self,
         expr: str,
         parameters: Mapping[str, str] | None = None,
     ) -> LGDO:
         """Apply column operations to the table and return a new LGDO.
 
         Internally uses :func:`numexpr.evaluate` if dealing with columns
         representable as NumPy arrays or :func:`eval` if
         :class:`.VectorOfVectors` are involved. In the latter case, the VoV
         columns are viewed as :class:`ak.Array` and the respective routines are
         therefore available.
 
+        To columns nested in subtables can be accessed by scoping with two
+        underscores (``__``). For example: ::
+
+          tbl.eval("a + tbl2__b")
+
+        computes the sum of column `a` and column `b` in the subtable `tbl2`.
+
         Parameters
         ----------
         expr
             if the expression only involves non-:class:`.VectorOfVectors`
             columns, the syntax is the one supported by
             :func:`numexpr.evaluate` (see `here
             <https://numexpr.readthedocs.io/projects/NumExpr3/en/latest/index.html>`_
@@ -281,23 +312,24 @@
             parameters = {}
 
         # get the valid python variable names in the expression
         c = compile(expr, "0vbb is real!", "eval")
 
         # make a dictionary of low-level objects (numpy or awkward)
         # for later computation
+        flat_self = self.flatten()
         self_unwrap = {}
         has_ak = False
         for obj in c.co_names:
-            if obj in self.keys():
-                if isinstance(self[obj], VectorOfVectors):
-                    self_unwrap[obj] = self[obj].view_as("ak", with_units=False)
+            if obj in flat_self:
+                if isinstance(flat_self[obj], VectorOfVectors):
+                    self_unwrap[obj] = flat_self[obj].view_as("ak", with_units=False)
                     has_ak = True
                 else:
-                    self_unwrap[obj] = self[obj].view_as("np", with_units=False)
+                    self_unwrap[obj] = flat_self[obj].view_as("np", with_units=False)
 
         # use numexpr if we are only dealing with numpy data types
         if not has_ak:
             out_data = ne.evaluate(
                 expr,
                 local_dict=(self_unwrap | parameters),
             )
@@ -315,15 +347,15 @@
                 f"evaluation resulted in {out_data.ndim}-dimensional data, "
                 "I don't know which LGDO this corresponds to"
             )
             raise RuntimeError(msg)
 
         # resort to good ol' eval()
         globs = {"ak": ak, "np": np}
-        out_data = eval(expr, globs, (self_unwrap | parameters))  # noqa: PGH001
+        out_data = eval(expr, globs, (self_unwrap | parameters))
 
         # need to convert back to LGDO
         if isinstance(out_data, ak.Array):
             if out_data.ndim == 1:
                 return Array(out_data.to_numpy())
             return VectorOfVectors(out_data)
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/vectorofvectors.py` & `legend_pydataobj-1.6.0/src/lgdo/types/vectorofvectors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,84 @@
 """
 Implements a LEGEND Data Object representing a variable-length array of
 variable-length arrays and corresponding utilities.
 """
+
 from __future__ import annotations
 
-import itertools
 import logging
-from collections.abc import Iterator
+from collections.abc import Iterator, Mapping, Sequence
 from typing import Any
 
 import awkward as ak
 import awkward_pandas as akpd
-import numba
 import numpy as np
 import pandas as pd
-from numpy.typing import DTypeLike, NDArray
+from numpy.typing import ArrayLike, DTypeLike, NDArray
 
 from .. import utils
-from ..utils import numba_defaults_kwargs as nb_kwargs
 from . import arrayofequalsizedarrays as aoesa
+from . import vovutils
 from .array import Array
 from .lgdo import LGDO
 
 log = logging.getLogger(__name__)
 
 
 class VectorOfVectors(LGDO):
-    """A variable-length array of variable-length arrays.
+    """A n-dimensional variable-length 1D array of variable-length 1D arrays.
+
+    If the vector is 2-dimensional, the internal representation is as two NumPy
+    arrays, one to store the flattened data contiguosly
+    (:attr:`flattened_data`) and one to store the cumulative sum of lengths of
+    each vector (:attr:`cumulative_length`). When the dimension is more than 2,
+    :attr:`flattened_data` is a :class:`VectorOfVectors` itself.
 
-    For now only a 1D vector of 1D vectors is supported. Internal representation
-    is as two NumPy arrays, one to store the flattened data contiguosly and one
-    to store the cumulative sum of lengths of each vector.
+    Examples
+    --------
+    >>> from lgdo import VectorOfVectors
+    >>> data = VectorOfVectors(
+    ...   [[[1, 2], [3, 4, 5]], [[2], [4, 8, 9, 7]], [[5, 3, 1]]],
+    ...   attrs={"units": "m"}
+    ... )
+    >>> print(data)
+    [[[1, 2], [3, 4, 5]],
+     [[2], [4, 8, 9, 7]],
+     [[5, 3, 1]]
+    ] with attrs={'units': 'm'}
+    >>> data.view_as("ak")
+    <Array [[[1, 2], [3, 4, 5]], ..., [[5, ..., 1]]] type='3 * var * var * int64'>
+
+    Note
+    ----
+    Many class methods are currently implemented only for 2D vectors and will
+    raise an exception on higher dimensional data.
     """
 
     def __init__(
         self,
-        array: ak.Array | list[list[int | float]] = None,
-        flattened_data: Array | NDArray = None,
-        cumulative_length: Array | NDArray = None,
-        shape_guess: tuple[int, int] | None = None,
-        dtype: DTypeLike = None,
+        data: ArrayLike | None = None,
+        flattened_data: ArrayLike | None = None,
+        cumulative_length: ArrayLike | VectorOfVectors | None = None,
+        shape_guess: Sequence[int, ...] | None = None,
+        dtype: DTypeLike | None = None,
         fill_val: int | float | None = None,
-        attrs: dict[str, Any] | None = None,
+        attrs: Mapping[str, Any] | None = None,
     ) -> None:
         """
         Parameters
         ----------
-        array
-            create a ``VectorOfVectors`` out of a Python list of lists or an
-            :class:`ak.Array`. Takes priority over `flattened_data` and
-            `cumulative_length`.
+        data
+            Any array-like structure accepted by the :class:`ak.Array`
+            constructor, with the exception that elements cannot be of type
+            ``OptionType``, ``UnionType`` or ``RecordType``.  Takes priority
+            over `flattened_data` and `cumulative_length`. The serialization of
+            the :class:`ak.Array` is performed through :func:`ak.to_buffers`.
+            Since the latter returns non-data-owning NumPy arrays, which would
+            prevent later modifications like resizing, a copy is performed.
         flattened_data
             if not ``None``, used as the internal array for
             `self.flattened_data`.  Otherwise, an internal `flattened_data` is
             allocated based on `cumulative_length` (or `shape_guess`) and `dtype`.
         cumulative_length
             if not ``None``, used as the internal array for
             `self.cumulative_length`. Should be `dtype` :any:`numpy.uint32`. If
@@ -70,132 +95,189 @@
             sets the type of data stored in `flattened_data`. Required if
             `flattened_data` and `array` are ``None``.
         fill_val
             fill all of `self.flattened_data` with this value.
         attrs
             a set of user attributes to be carried along with this LGDO.
         """
-        if array is not None:
-            if isinstance(array, ak.Array):
-                if array.ndim != 2:
-                    msg = (
-                        "cannot initialize a VectorOfVectors with "
-                        f"{array.ndim}-dimensional data"
-                    )
-                    raise ValueError(msg)
+        # sanitize
+        if cumulative_length is not None and not isinstance(cumulative_length, Array):
+            cumulative_length = Array(cumulative_length)
+        if flattened_data is not None and not isinstance(
+            flattened_data, (Array, VectorOfVectors)
+        ):
+            flattened_data = Array(flattened_data)
+
+        if data is not None:
+            if not isinstance(data, ak.Array):
+                data = ak.Array(data)
+
+            if data.ndim < 2:
+                msg = (
+                    "cannot initialize a VectorOfVectors with "
+                    f"{data.ndim}-dimensional data"
+                )
+                raise ValueError(msg)
 
-                form, length, container = ak.to_buffers(array)
+            # make sure it's not a record array
+            if not vovutils._ak_is_valid(data):
+                msg = "input array type is not supported!"
+                raise ValueError(msg)
 
-                self.__init__(
-                    flattened_data=container["node1-data"],
-                    cumulative_length=container["node0-offsets"][1:],
-                )
+            # array might be non-jagged! ('container' will hold a ndim NumPy array)
+            if not vovutils._ak_is_jagged(data):
+                data = ak.from_regular(data, axis=None)
+
+            # ak.to_buffer helps in de-serialization
+            # NOTE: ak.to_packed() needed?
+            form, length, container = ak.to_buffers(ak.to_packed(data))
+
+            # NOTE: node#-data is not even in the dict if the awkward array is empty
+            # NOTE: if the data arg was a numpy array, to_buffers() preserves
+            # the original dtype
+            # FIXME: have to copy the buffers, otherwise self will not own the
+            # data and self.resize() will fail. Is it possible to avoid this?
+            flattened_data = np.copy(
+                container.pop(f"node{data.ndim-1}-data", np.empty(0, dtype=dtype))
+            )
 
-            else:
-                cl_nda = np.cumsum([len(ll) for ll in array])
-                if dtype is None:
-                    if len(cl_nda) == 0 or cl_nda[-1] == 0:
-                        msg = "array can't be empty with dtype=None!"
-                        raise ValueError(msg)
-
-                    # Set dtype from the first element in the list
-                    # Find it efficiently, allowing for zero-length lists as some of the entries
-                    first_element = next(itertools.chain.from_iterable(array))
-                    dtype = type(first_element)
+            # if user-provided dtype is different than dtype from Awkward, cast
+            # NOTE: makes a copy only if needed
+            flattened_data = np.asarray(flattened_data, dtype=dtype)
+
+            # start from innermost VoV and build nested structure
+            for i in range(data.ndim - 2, -1, -1):
+                # NOTE: remember, omit the leading 0 from ak.Array offsets
+                cumulative_length = np.copy(container[f"node{i}-offsets"][1:])
+
+                if i != 0:
+                    # at the beginning of the loop: initialize innermost
+                    # flattened_data and replace current flattened_data
+                    # reference. in the following iterations flattened_data is
+                    # a VectorOfVectors
+                    flattened_data = VectorOfVectors(
+                        flattened_data=flattened_data,
+                        cumulative_length=cumulative_length,
+                    )
 
-                self.dtype = np.dtype(dtype)
-                self.cumulative_length = Array(cl_nda)
-                self.flattened_data = Array(
-                    np.fromiter(itertools.chain.from_iterable(array), dtype=self.dtype)
-                )
+                else:
+                    # at end we need to initialize self with the latest flattened_data
+                    self.__init__(
+                        flattened_data=flattened_data,
+                        cumulative_length=cumulative_length,
+                    )
 
         else:
+            self.flattened_data = None
+            self.cumulative_length = None
+
+            # let's first setup cumulative_length...
             if cumulative_length is None:
-                if shape_guess is None:
-                    # just make an empty vector
-                    self.cumulative_length = Array(np.empty((0,), dtype="uint32"))
                 # initialize based on shape_guess
-                elif shape_guess[1] <= 0:
-                    self.cumulative_length = Array(
-                        shape=(shape_guess[0],), dtype="uint32", fill_val=0
+                if shape_guess is None:
+                    # just make an empty 2D vector
+                    shape_guess = (0, 0)
+
+                # sanity check
+                if len(shape_guess) < 2:
+                    msg = "shape_guess must be a sequence of 2 integers or more"
+                    raise ValueError(msg)
+
+                # let's Awkward do the job here, we're lazy
+                if fill_val is not None:
+                    self.__init__(
+                        np.full(shape=shape_guess, fill_value=fill_val, dtype=dtype)
                     )
                 else:
-                    self.cumulative_length = Array(
-                        np.arange(
-                            shape_guess[1],
-                            np.prod(shape_guess) + 1,
-                            shape_guess[1],
-                            dtype="uint32",
-                        )
-                    )
+                    self.__init__(np.empty(shape=shape_guess, dtype=dtype))
             else:
-                self.cumulative_length = Array(cumulative_length)
+                # if it's user provided just use it
+                self.cumulative_length = cumulative_length
 
-            if flattened_data is None:
+            # ...then flattened_data
+            # NOTE: self.flattened_data might have already been initialized
+            # above
+            if flattened_data is None and self.flattened_data is None:
+                # this happens when the cumulative_length arg is not None
                 if dtype is None:
                     msg = "flattened_data and dtype cannot both be None!"
                     raise ValueError(msg)
 
-                length = 0
-                if cumulative_length is None:
-                    # just make an empty vector or use shape_guess
-                    length = 0 if shape_guess is None else np.prod(shape_guess)
-                else:
-                    # use cumulative_length
-                    length = cumulative_length[-1]
-
+                # now ready to initialize the object!
                 self.flattened_data = Array(
-                    shape=(length,), dtype=dtype, fill_val=fill_val
+                    shape=(self.cumulative_length[-1],), dtype=dtype, fill_val=fill_val
                 )
-            else:
-                self.flattened_data = Array(flattened_data)
+            elif self.flattened_data is None:
+                self.flattened_data = flattened_data
 
             # finally set dtype
             self.dtype = self.flattened_data.dtype
 
+        # set ndim
+        self.ndim = 2
+        pointer = self.flattened_data
+        while True:
+            if isinstance(pointer, Array):
+                break
+
+            self.ndim += 1
+            pointer = pointer.flattened_data
+
         super().__init__(attrs)
 
     def datatype_name(self) -> str:
         return "array"
 
     def form_datatype(self) -> str:
-        et = utils.get_element_type(self)
-        return "array<1>{array<1>{" + et + "}}"
+        eltype = (
+            "array<1>{" + utils.get_element_type(self) + "}"
+            if self.ndim == 2
+            else self.flattened_data.form_datatype()
+        )
+        return "array<1>{" + eltype + "}"
 
     def __len__(self) -> int:
-        """Return the number of stored vectors."""
+        """Return the number of stored vectors along the first axis (0)."""
         return len(self.cumulative_length)
 
     def __eq__(self, other: VectorOfVectors) -> bool:
         if isinstance(other, VectorOfVectors):
+            if self.ndim == 2 and len(self.cumulative_length) != 0:
+                fldata_eq = np.array_equal(
+                    self.flattened_data[: self.cumulative_length[-1]],
+                    other.flattened_data[: other.cumulative_length[-1]],
+                )
+            else:
+                fldata_eq = self.flattened_data == other.flattened_data
+
             return (
                 self.cumulative_length == other.cumulative_length
-                and (
-                    len(self.cumulative_length) == 0
-                    or np.all(
-                        self.flattened_data[: self.cumulative_length[-1]]
-                        == other.flattened_data[: other.cumulative_length[-1]]
-                    )
-                )
+                and fldata_eq
                 and self.dtype == other.dtype
                 and self.attrs == other.attrs
             )
 
         return False
 
-    def __getitem__(self, i: int) -> list:
-        """Return vector at index `i`."""
-        stop = self.cumulative_length[i]
-        if i in (0, -len(self)):
-            return self.flattened_data[0:stop]
+    def __getitem__(self, i: int) -> NDArray:
+        """Return a view of the vector at index `i` along the first axis."""
+        if self.ndim == 2:
+            stop = self.cumulative_length[i]
+            if i in (0, -len(self)):
+                return self.flattened_data[0:stop]
+
+            return self.flattened_data[self.cumulative_length[i - 1] : stop]
 
-        return self.flattened_data[self.cumulative_length[i - 1] : stop]
+        raise NotImplementedError
 
     def __setitem__(self, i: int, new: NDArray) -> None:
-        self.__getitem__(i)[:] = new
+        if self.ndim == 2:
+            self.__getitem__(i)[:] = new
+        else:
+            raise NotImplementedError
 
     def resize(self, new_size: int) -> None:
         """Resize vector along the first axis.
 
         `self.flattened_data` is resized only if `new_size` is smaller than the
         current vector length.
 
@@ -216,55 +298,62 @@
         >>> vov = VectorOfVectors([[1, 2], [3], [4, 5]])
         >>> vov.resize(2)
         >>> print(vov)
         [[1 2],
          [3],
         ]
         """
-
-        vidx = self.cumulative_length
-        old_s = len(self)
-        dlen = new_size - old_s
-        csum = vidx[-1] if len(self) > 0 else 0
-
-        # first resize the cumulative length
-        self.cumulative_length.resize(new_size)
-
-        # if new_size > size, new elements are filled with zeros, let's fix
-        # that
-        if dlen > 0:
-            self.cumulative_length[old_s:] = csum
-
-        # then resize the data array
-        # if dlen > 0 this has no effect
-        if len(self.cumulative_length) > 0:
-            self.flattened_data.resize(self.cumulative_length[-1])
+        if self.ndim == 2:
+            vidx = self.cumulative_length
+            old_s = len(self)
+            dlen = new_size - old_s
+            csum = vidx[-1] if len(self) > 0 else 0
+
+            # first resize the cumulative length
+            self.cumulative_length.resize(new_size)
+
+            # if new_size > size, new elements are filled with zeros, let's fix
+            # that
+            if dlen > 0:
+                self.cumulative_length[old_s:] = csum
+
+            # then resize the data array
+            # if dlen > 0 this has no effect
+            if len(self.cumulative_length) > 0:
+                self.flattened_data.resize(self.cumulative_length[-1])
+        else:
+            raise NotImplementedError
 
     def append(self, new: NDArray) -> None:
         """Append a 1D vector `new` at the end.
 
         Examples
         --------
         >>> vov = VectorOfVectors([[1, 2, 3], [4, 5]])
         >>> vov.append([8, 9])
         >>> print(vov)
         [[1 2 3],
          [4 5],
          [8 9],
         ]
         """
-        # first extend cumulative_length by +1
-        self.cumulative_length.resize(len(self) + 1)
-        # set it at the right value
-        newlen = self.cumulative_length[-2] + len(new) if len(self) > 1 else len(new)
-        self.cumulative_length[-1] = newlen
-        # then resize flattened_data to accommodate the new vector
-        self.flattened_data.resize(len(self.flattened_data) + len(new))
-        # finally set it
-        self[-1] = new
+        if self.ndim == 2:
+            # first extend cumulative_length by +1
+            self.cumulative_length.resize(len(self) + 1)
+            # set it at the right value
+            newlen = (
+                self.cumulative_length[-2] + len(new) if len(self) > 1 else len(new)
+            )
+            self.cumulative_length[-1] = newlen
+            # then resize flattened_data to accommodate the new vector
+            self.flattened_data.resize(len(self.flattened_data) + len(new))
+            # finally set it
+            self[-1] = new
+        else:
+            raise NotImplementedError
 
     def insert(self, i: int, new: NDArray) -> None:
         """Insert a vector at index `i`.
 
         `self.flattened_data` (and therefore `self.cumulative_length`) is
         resized in order to accommodate the new element.
 
@@ -279,25 +368,28 @@
         ]
 
         Warning
         -------
         This method involves a significant amount of memory re-allocation and
         is expected to perform poorly on large vectors.
         """
-        if i >= len(self):
-            msg = f"index {i} is out of bounds for vector owith size {len(self)}"
-            raise IndexError(msg)
+        if self.ndim == 2:
+            if i >= len(self):
+                msg = f"index {i} is out of bounds for vector owith size {len(self)}"
+                raise IndexError(msg)
 
-        self.flattened_data = Array(
-            np.insert(self.flattened_data, self.cumulative_length[i - 1], new)
-        )
-        self.cumulative_length = Array(
-            np.insert(self.cumulative_length, i, self.cumulative_length[i - 1])
-        )
-        self.cumulative_length[i:] += np.uint32(len(new))
+            self.flattened_data = Array(
+                np.insert(self.flattened_data, self.cumulative_length[i - 1], new)
+            )
+            self.cumulative_length = Array(
+                np.insert(self.cumulative_length, i, self.cumulative_length[i - 1])
+            )
+            self.cumulative_length[i:] += np.uint32(len(new))
+        else:
+            raise NotImplementedError
 
     def replace(self, i: int, new: NDArray) -> None:
         """Replace the vector at index `i` with `new`.
 
         `self.flattened_data` (and therefore `self.cumulative_length`) is
         resized, if the length of `new` is different from the vector currently
         at index `i`.
@@ -312,101 +404,114 @@
         ]
 
         Warning
         -------
         This method involves a significant amount of memory re-allocation and
         is expected to perform poorly on large vectors.
         """
-        if i >= len(self):
-            msg = f"index {i} is out of bounds for vector with size {len(self)}"
-            raise IndexError(msg)
-
-        vidx = self.cumulative_length
-        dlen = len(new) - len(self[i])
-
-        if dlen == 0:
-            # don't waste resources
-            self[i] = new
-        elif dlen < 0:
-            start = vidx[i - 1]
-            stop = start + len(new)
-            # set the already allocated indices
-            self.flattened_data[start:stop] = new
-            # then delete the extra indices
-            self.flattened_data = Array(
-                np.delete(self.flattened_data, np.s_[stop : vidx[i]])
-            )
-        else:
-            # set the already allocated indices
-            self.flattened_data[vidx[i - 1] : vidx[i]] = new[: len(self[i])]
-            # then insert the remaining
-            self.flattened_data = Array(
-                np.insert(self.flattened_data, vidx[i], new[len(self[i]) :])
-            )
+        if self.ndim == 2:
+            if i >= len(self):
+                msg = f"index {i} is out of bounds for vector with size {len(self)}"
+                raise IndexError(msg)
+
+            vidx = self.cumulative_length
+            dlen = len(new) - len(self[i])
+
+            if dlen == 0:
+                # don't waste resources
+                self[i] = new
+            elif dlen < 0:
+                start = vidx[i - 1]
+                stop = start + len(new)
+                # set the already allocated indices
+                self.flattened_data[start:stop] = new
+                # then delete the extra indices
+                self.flattened_data = Array(
+                    np.delete(self.flattened_data, np.s_[stop : vidx[i]])
+                )
+            else:
+                # set the already allocated indices
+                self.flattened_data[vidx[i - 1] : vidx[i]] = new[: len(self[i])]
+                # then insert the remaining
+                self.flattened_data = Array(
+                    np.insert(self.flattened_data, vidx[i], new[len(self[i]) :])
+                )
 
-        vidx[i:] = vidx[i:] + dlen
+            vidx[i:] = vidx[i:] + dlen
+        else:
+            raise NotImplementedError
 
-    def _set_vector_unsafe(self, i: int, vec: NDArray, lens: NDArray = None) -> None:
+    def _set_vector_unsafe(
+        self, i: int, vec: NDArray, lens: ArrayLike | None = None
+    ) -> None:
         r"""Insert vector `vec` at position `i`.
 
         Assumes that ``j = self.cumulative_length[i-1]`` is the index (in
         `self.flattened_data`) of the end of the `(i-1)`\ th vector and copies
         `vec` in ``self.flattened_data[j:sum(lens)]``. Finally updates
         ``self.cumulative_length[i]`` with the new flattened data array length.
 
         Vectors stored after index `i` can be overridden, producing unintended
         behavior. This method is typically used for fast sequential fill of a
         pre-allocated vector of vectors.
 
-        If vec is 1D array and lens is None, set using full array. If vec
-        is 2D, require lens to be included, and fill each array only up to
-        lengths in lens.
+        If i`vec` is 1D array and `lens` is ``None``, set using full array. If
+        `vec` is 2D, require `lens` to be included, and fill each array only up
+        to lengths in `lens`.
 
         Danger
         ------
         This method can lead to undefined behavior or vector invalidation if
         used improperly. Use it only if you know what you are doing.
 
         See Also
         --------
         append, replace, insert
         """
-        start = 0 if i == 0 else self.cumulative_length[i - 1]
-        if len(vec.shape) == 1:
-            vec = np.expand_dims(vec, axis=0)
-            if lens is None:
-                lens = np.array([vec.shape[1]], dtype="u4")
-        if not isinstance(lens, np.ndarray):
-            lens = np.array([lens], dtype="u4")
-        cum_lens = start + lens.cumsum()
-        _nb_fill(vec, lens, self.flattened_data.nda[start : cum_lens[-1]])
-        self.cumulative_length[i : i + len(lens)] = cum_lens
+        if self.ndim == 2:
+            # check if current vector is empty and get the start index in
+            # flattened_data
+            start = 0 if i == 0 else self.cumulative_length[i - 1]
+
+            # if the new element is 1D, convert to dummy 2D
+            if len(vec.shape) == 1:
+                vec = np.expand_dims(vec, axis=0)
+                if lens is None:
+                    lens = np.array([vec.shape[1]], dtype="u4")
+
+            # this in case lens is 02, convert to 1D
+            if not isinstance(lens, np.ndarray):
+                lens = np.array([lens], dtype="u4")
 
-    def __iter__(self) -> Iterator[NDArray]:
-        for j, stop in enumerate(self.cumulative_length):
-            if j == 0:
-                yield self.flattened_data[0:stop]
-            else:
-                yield self.flattened_data[self.cumulative_length[j - 1] : stop]
+            # calculate stop index in flattened_data
+            cum_lens = start + lens.cumsum()
 
-    def __str__(self) -> str:
-        string = ""
-        pos = 0
-        for vec in self:
-            if pos != 0:
-                string += " "
+            # fill with fast vectorized routine
+            vovutils._nb_fill(vec, lens, self.flattened_data.nda[start : cum_lens[-1]])
 
-            string += np.array2string(vec, prefix=" ")
+            # add new vector(s) length to cumulative_length
+            self.cumulative_length[i : i + len(lens)] = cum_lens
+        else:
+            raise NotImplementedError
 
-            if pos < len(self.cumulative_length):
-                string += ",\n"
+    def __iter__(self) -> Iterator[NDArray]:
+        if self.ndim == 2:
+            for j, stop in enumerate(self.cumulative_length):
+                if j == 0:
+                    yield self.flattened_data[0:stop]
+                else:
+                    yield self.flattened_data[self.cumulative_length[j - 1] : stop]
+        else:
+            raise NotImplementedError
 
-            pos += 1
+    def __str__(self) -> str:
+        string = self.view_as("ak").show(stream=None)
 
-        string = f"[{string}]"
+        string = string.strip().removesuffix("]")
+        string += "\n]"
 
         tmp_attrs = self.attrs.copy()
         tmp_attrs.pop("datatype")
         if len(tmp_attrs) > 0:
             string += f" with attrs={tmp_attrs}"
 
         return string
@@ -453,27 +558,30 @@
             output array will be such that both `fill_val` and the vector
             values can be represented in the same data structure.
         preserve_dtype
             whether the output array should have exactly the same dtype as the
             original vector of vectors. The type `fill_val` must be a
             compatible one.
         """
-        ak_arr = self.view_as("ak")
+        if self.ndim == 2:
+            ak_arr = self.view_as("ak")
 
-        if max_len is None:
-            max_len = int(ak.max(ak.count(ak_arr, axis=-1)))
+            if max_len is None:
+                max_len = int(ak.max(ak.count(ak_arr, axis=-1)))
 
-        nda = ak.fill_none(ak.pad_none(ak_arr, max_len, clip=True), fill_val).to_numpy(
-            allow_missing=False
-        )
+            nda = ak.fill_none(
+                ak.pad_none(ak_arr, max_len, clip=True), fill_val
+            ).to_numpy(allow_missing=False)
+
+            if preserve_dtype:
+                nda = nda.astype(self.flattened_data.dtype, copy=False)
 
-        if preserve_dtype:
-            nda = nda.astype(self.flattened_data.dtype, copy=False)
+            return aoesa.ArrayOfEqualSizedArrays(nda=nda, attrs=self.getattrs())
 
-        return aoesa.ArrayOfEqualSizedArrays(nda=nda, attrs=self.getattrs())
+        raise NotImplementedError
 
     def view_as(
         self,
         library: str,
         with_units: bool = False,
         fill_val: bool | int | float = np.nan,
         preserve_dtype: bool = False,
@@ -515,26 +623,34 @@
         attach_units = with_units and "units" in self.attrs
 
         if library == "ak":
             if attach_units:
                 msg = "Pint does not support Awkward yet, you must view the data with_units=False"
                 raise ValueError(msg)
 
+            # see https://github.com/scikit-hep/awkward/discussions/2848
+
             # cannot avoid making a copy here. we should add the leading 0 to
             # cumulative_length inside VectorOfVectors at some point in the
             # future
             offsets = np.empty(
                 len(self.cumulative_length) + 1, dtype=self.cumulative_length.dtype
             )
             offsets[1:] = self.cumulative_length
             offsets[0] = 0
 
+            content = (
+                ak.contents.NumpyArray(self.flattened_data.nda)
+                if self.ndim == 2
+                else self.flattened_data.view_as(library, with_units=with_units).layout
+            )
+
             layout = ak.contents.ListOffsetArray(
                 offsets=ak.index.Index(offsets),
-                content=ak.contents.NumpyArray(self.flattened_data.nda),
+                content=content,
             )
             return ak.Array(layout)
 
         if library == "np":
             if preserve_dtype:
                 return self.to_aoesa(fill_val=fill_val, preserve_dtype=True).view_as(
                     "np", with_units=with_units
@@ -547,267 +663,7 @@
                 msg = "Pint does not support Awkward yet, you must view the data with_units=False"
                 raise ValueError(msg)
 
             return akpd.from_awkward(self.view_as("ak"))
 
         msg = f"{library} is not a supported third-party format."
         raise ValueError(msg)
-
-
-def build_cl(
-    sorted_array_in: NDArray, cumulative_length_out: NDArray = None
-) -> NDArray:
-    """Build a cumulative length array from an array of sorted data.
-
-    Examples
-    --------
-    >>> build_cl(np.array([3, 3, 3, 4])
-    array([3., 4.])
-
-    For a `sorted_array_in` of indices, this is the inverse of
-    :func:`.explode_cl`, in the sense that doing
-    ``build_cl(explode_cl(cumulative_length))`` would recover the original
-    `cumulative_length`.
-
-    Parameters
-    ----------
-    sorted_array_in
-        array of data already sorted; each N matching contiguous entries will
-        be converted into a new row of `cumulative_length_out`.
-    cumulative_length_out
-        a pre-allocated array for the output `cumulative_length`. It will
-        always have length <= `sorted_array_in`, so giving them the same length
-        is safe if there is not a better guess.
-
-    Returns
-    -------
-    cumulative_length_out
-        the output cumulative length array. If the user provides a
-        `cumulative_length_out` that is too long, this return value is sliced
-        to contain only the used portion of the allocated memory.
-    """
-    if len(sorted_array_in) == 0:
-        return None
-    sorted_array_in = np.asarray(sorted_array_in)
-    if cumulative_length_out is None:
-        cumulative_length_out = np.zeros(len(sorted_array_in), dtype=np.uint64)
-    else:
-        cumulative_length_out.fill(0)
-    if len(cumulative_length_out) == 0 and len(sorted_array_in) > 0:
-        msg = "cumulative_length_out too short ({len(cumulative_length_out)})"
-        raise ValueError(msg)
-    return _nb_build_cl(sorted_array_in, cumulative_length_out)
-
-
-@numba.njit(**nb_kwargs)
-def _nb_build_cl(sorted_array_in: NDArray, cumulative_length_out: NDArray) -> NDArray:
-    """numbified inner loop for build_cl"""
-    ii = 0
-    last_val = sorted_array_in[0]
-    for val in sorted_array_in:
-        if val != last_val:
-            ii += 1
-            cumulative_length_out[ii] = cumulative_length_out[ii - 1]
-            if ii >= len(cumulative_length_out):
-                msg = "cumulative_length_out too short"
-                raise RuntimeError(msg)
-            last_val = val
-        cumulative_length_out[ii] += 1
-    ii += 1
-    return cumulative_length_out[:ii]
-
-
-@numba.guvectorize(
-    [
-        f"{data_type}[:,:],{size_type}[:],{data_type}[:]"
-        for data_type in [
-            "b1",
-            "i1",
-            "i2",
-            "i4",
-            "i8",
-            "u1",
-            "u2",
-            "u4",
-            "u8",
-            "f4",
-            "f8",
-            "c8",
-            "c16",
-        ]
-        for size_type in ["i4", "i8", "u4", "u8"]
-    ],
-    "(l,m),(l),(n)",
-    **nb_kwargs,
-)
-def _nb_fill(aoa_in: NDArray, len_in: NDArray, flattened_array_out: NDArray):
-    """Vectorized function to fill flattened array from array of arrays and
-    lengths. Values in aoa_in past lengths will not be copied.
-
-    Parameters
-    ----------
-    aoa_in
-        array of arrays containing values to be copied
-    len_in
-        array of vector lengths for each row of aoa_in
-    flattened_array_out
-        flattened array to copy values into. Must be longer than sum of
-        lengths in len_in
-    """
-
-    if len(flattened_array_out) < len_in.sum():
-        msg = "flattened array not large enough to hold values"
-        raise ValueError(msg)
-
-    start = 0
-    for i, ll in enumerate(len_in):
-        stop = start + ll
-        flattened_array_out[start:stop] = aoa_in[i, :ll]
-        start = stop
-
-
-def explode_cl(cumulative_length: NDArray, array_out: NDArray = None) -> NDArray:
-    """Explode a `cumulative_length` array.
-
-    Examples
-    --------
-    >>> explode_cl(np.array([2, 3]))
-    array([0., 0., 1.])
-
-    This is the inverse of :func:`.build_cl`, in the sense that doing
-    ``build_cl(explode_cl(cumulative_length))`` would recover the original
-    `cumulative_length`.
-
-    Parameters
-    ----------
-    cumulative_length
-        the cumulative length array to be exploded.
-    array_out
-        a pre-allocated array to hold the exploded cumulative length array.
-        The length should be equal to ``cumulative_length[-1]``.
-
-    Returns
-    -------
-    array_out
-        the exploded cumulative length array.
-    """
-    cumulative_length = np.asarray(cumulative_length)
-    out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if array_out is None:
-        array_out = np.empty(int(out_len), dtype=np.uint64)
-    if len(array_out) != out_len:
-        msg = f"bad lengths: cl[-1] ({cumulative_length[-1]}) != out ({len(array_out)})"
-        raise ValueError(msg)
-    return _nb_explode_cl(cumulative_length, array_out)
-
-
-@numba.njit(**nb_kwargs)
-def _nb_explode_cl(cumulative_length: NDArray, array_out: NDArray) -> NDArray:
-    """numbified inner loop for explode_cl"""
-    out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if len(array_out) != out_len:
-        msg = "bad lengths"
-        raise ValueError(msg)
-    start = 0
-    for ii in range(len(cumulative_length)):
-        nn = int(cumulative_length[ii] - start)
-        for jj in range(nn):
-            array_out[int(start + jj)] = ii
-        start = cumulative_length[ii]
-    return array_out
-
-
-def explode(
-    cumulative_length: NDArray, array_in: NDArray, array_out: NDArray = None
-) -> NDArray:
-    """Explode a data array using a `cumulative_length` array.
-
-    This is identical to :func:`.explode_cl`, except `array_in` gets exploded
-    instead of `cumulative_length`.
-
-    Examples
-    --------
-    >>> explode(np.array([2, 3]), np.array([3, 4]))
-    array([3., 3., 4.])
-
-    Parameters
-    ----------
-    cumulative_length
-        the cumulative length array to use for exploding.
-    array_in
-        the data to be exploded. Must have same length as `cumulative_length`.
-    array_out
-        a pre-allocated array to hold the exploded data. The length should be
-        equal to ``cumulative_length[-1]``.
-
-    Returns
-    -------
-    array_out
-        the exploded cumulative length array.
-    """
-    cumulative_length = np.asarray(cumulative_length)
-    array_in = np.asarray(array_in)
-    out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if array_out is None:
-        array_out = np.empty(out_len, dtype=array_in.dtype)
-    if len(cumulative_length) != len(array_in) or len(array_out) != out_len:
-        msg = (
-            f"bad lengths: cl ({len(cumulative_length)}) != in ({len(array_in)}) "
-            f"and cl[-1] ({cumulative_length[-1]}) != out ({len(array_out)})"
-        )
-        raise ValueError(msg)
-    return nb_explode(cumulative_length, array_in, array_out)
-
-
-@numba.njit(**nb_kwargs)
-def nb_explode(
-    cumulative_length: NDArray, array_in: NDArray, array_out: NDArray
-) -> NDArray:
-    """Numbified inner loop for :func:`.explode`."""
-    out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if len(cumulative_length) != len(array_in) or len(array_out) != out_len:
-        msg = "bad lengths"
-        raise ValueError(msg)
-    ii = 0
-    for jj in range(len(array_out)):
-        while ii < len(cumulative_length) and jj >= cumulative_length[ii]:
-            ii += 1
-        array_out[jj] = array_in[ii]
-    return array_out
-
-
-def explode_arrays(
-    cumulative_length: Array,
-    arrays: list[NDArray],
-    arrays_out: list[NDArray] | None = None,
-) -> list:
-    """Explode a set of arrays using a `cumulative_length` array.
-
-    Parameters
-    ----------
-    cumulative_length
-        the cumulative length array to use for exploding.
-    arrays
-        the data arrays to be exploded. Each array must have same length as
-        `cumulative_length`.
-    arrays_out
-        a list of pre-allocated arrays to hold the exploded data. The length of
-        the list should be equal to the length of `arrays`, and each entry in
-        arrays_out should have length ``cumulative_length[-1]``. If not
-        provided, output arrays are allocated for the user.
-
-    Returns
-    -------
-    arrays_out
-        the list of exploded cumulative length arrays.
-    """
-    cumulative_length = np.asarray(cumulative_length)
-    for ii in range(len(arrays)):
-        arrays[ii] = np.asarray(arrays[ii])
-    out_len = cumulative_length[-1] if len(cumulative_length) > 0 else 0
-    if arrays_out is None:
-        arrays_out = []
-        for array in arrays:
-            arrays_out.append(np.empty(out_len, dtype=array.dtype))
-    for ii in range(len(arrays)):
-        explode(cumulative_length, arrays[ii], arrays_out[ii])
-    return arrays_out
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/types/waveformtable.py` & `legend_pydataobj-1.6.0/src/lgdo/types/waveformtable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Implements a LEGEND Data Object representing a special
 :class:`~.lgdo.table.Table` to store blocks of one-dimensional time-series
 data.
 """
+
 from __future__ import annotations
 
 import logging
 from typing import Any
 
 import awkward as ak
 import numpy as np
```

### Comparing `legend_pydataobj-1.5.1/src/lgdo/utils.py` & `legend_pydataobj-1.6.0/src/lgdo/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Implements utilities for LEGEND Data Objects."""
+
 from __future__ import annotations
 
 import logging
 import os
 from collections.abc import Iterator, MutableMapping
 from typing import Any
 
 import numpy as np
 
-from . import types as lgdo
-
 log = logging.getLogger(__name__)
 
 
 def get_element_type(obj: object) -> str:
     """Get the LGDO element type of a scalar or array.
 
     For use in LGDO datatype attributes.
@@ -52,44 +51,14 @@
         return "string"
 
     # couldn't figure it out
     msg = "cannot determine lgdo element_type for object of type"
     raise ValueError(msg, type(obj).__name__)
 
 
-def copy(obj: lgdo.LGDO, dtype: np.dtype = None) -> lgdo.LGDO:
-    """Return a copy of an LGDO.
-
-    Parameters
-    ----------
-    obj
-        the LGDO to be copied.
-    dtype
-        NumPy dtype to be used for the copied object.
-
-    """
-    if dtype is None:
-        dtype = obj.dtype
-
-    if isinstance(obj, lgdo.Array):
-        return lgdo.Array(
-            np.array(obj.nda, dtype=dtype, copy=True), attrs=dict(obj.attrs)
-        )
-
-    if isinstance(obj, lgdo.VectorOfVectors):
-        return lgdo.VectorOfVectors(
-            flattened_data=copy(obj.flattened_data, dtype=dtype),
-            cumulative_length=copy(obj.cumulative_length),
-            attrs=dict(obj.attrs),
-        )
-
-    msg = f"copy of {type(obj)} not supported"
-    raise ValueError(msg)
-
-
 def getenv_bool(name: str, default: bool = False) -> bool:
     """Get environment value as a boolean, returning True for 1, t and true
     (caps-insensitive), and False for any other value and default if undefined.
     """
     val = os.getenv(name)
     if not val:
         return default
```

### Comparing `legend_pydataobj-1.5.1/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat` & `legend_pydataobj-1.6.0/tests/compression/sigcompress/LDQTA_r117_20200110T105115Z_cal_geds_raw-0.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/compression/sigcompress/special-wf-clipped.dat` & `legend_pydataobj-1.6.0/tests/compression/sigcompress/special-wf-clipped.dat`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/compression/test_compression.py` & `legend_pydataobj-1.6.0/tests/compression/test_compression.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/compression/test_radware_sigcompress.py` & `legend_pydataobj-1.6.0/tests/compression/test_radware_sigcompress.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/compression/test_str2wfcodec.py` & `legend_pydataobj-1.6.0/tests/compression/test_str2wfcodec.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/compression/test_uleb128_zigzag_diff.py` & `legend_pydataobj-1.6.0/tests/compression/test_uleb128_zigzag_diff.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/conftest.py` & `legend_pydataobj-1.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/lh5/test_lh5_iterator.py` & `legend_pydataobj-1.6.0/tests/lh5/test_lh5_iterator.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/lh5/test_lh5_utils.py` & `legend_pydataobj-1.6.0/tests/lh5/test_lh5_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,36 +8,14 @@
 
 
 @pytest.fixture(scope="module")
 def lgnd_file(lgnd_test_data):
     return lgnd_test_data.get_path("lh5/LDQTA_r117_20200110T105115Z_cal_geds_raw.lh5")
 
 
-def test_parse_datatype():
-    datatypes = [
-        ("real", ("scalar", None, "real")),
-        ("array<1>{bool}", ("array", (1,), "bool")),
-        ("fixedsizearray<2>{real}", ("fixedsizearray", (2,), "real")),
-        (
-            "arrayofequalsizedarrays<3,4>{complex}",
-            ("arrayofequalsizedarrays", (3, 4), "complex"),
-        ),
-        ("array<1>{array<1>{blob}}", ("array", (1,), "array<1>{blob}")),
-        (
-            "struct{field1,field2,fieldn}",
-            ("struct", None, ["field1", "field2", "fieldn"]),
-        ),
-        ("table{col1,col2,coln}", ("table", None, ["col1", "col2", "coln"])),
-    ]
-
-    for string, dt_tuple in datatypes:
-        pd_dt_tuple = utils.parse_datatype(string)
-        assert pd_dt_tuple == dt_tuple
-
-
 def test_expand_vars():
     # Check env variable expansion
     os.environ["PYGAMATESTBASEDIR"] = "a_random_string"
     assert utils.expand_vars("$PYGAMATESTBASEDIR/blah") == "a_random_string/blah"
 
     # Check user variable expansion
     assert (
```

### Comparing `legend_pydataobj-1.5.1/tests/types/test_array.py` & `legend_pydataobj-1.6.0/tests/types/test_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import awkward as ak
 import numpy as np
 import pandas as pd
 import pint
 import pytest
 
-from lgdo import Array, utils
+from lgdo import Array
 
 
 def test_datatype_name():
     array = Array()
     assert array.datatype_name() == "array"
 
 
@@ -28,20 +28,14 @@
 
 def test_resize():
     array = Array(nda=np.array([1, 2, 3, 4]))
     array.resize(3)
     assert (array.nda == np.array([1, 2, 3])).all()
 
 
-def test_copy():
-    a1 = Array(np.array([1, 2, 3, 4]))
-    a2 = utils.copy(a1)
-    assert a1 == a2
-
-
 def test_insert():
     a = Array(np.array([1, 2, 3, 4]))
     a.insert(2, [-1, -1])
     assert a == Array([1, 2, -1, -1, 3, 4])
 
 
 def test_view():
```

### Comparing `legend_pydataobj-1.5.1/tests/types/test_arrayofequalsizedarrays.py` & `legend_pydataobj-1.6.0/tests/types/test_arrayofequalsizedarrays.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_encoded.py` & `legend_pydataobj-1.6.0/tests/types/test_encoded.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_fixedsizearray.py` & `legend_pydataobj-1.6.0/tests/types/test_fixedsizearray.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_representations.py` & `legend_pydataobj-1.6.0/tests/types/test_representations.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_scalar.py` & `legend_pydataobj-1.6.0/tests/types/test_scalar.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_struct.py` & `legend_pydataobj-1.6.0/tests/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `legend_pydataobj-1.5.1/tests/types/test_table.py` & `legend_pydataobj-1.6.0/tests/types/test_table.py`

 * *Files 10% similar despite different names*

```diff
@@ -144,14 +144,31 @@
         ),
     )
 
     with pytest.raises(ValueError):
         tbl.view_as("pd", with_units=True)
 
 
+def test_flatten():
+    tbl = Table(
+        col_dict={
+            "a": lgdo.Array(np.array([1, 2, 3])),
+            "tbl": Table(
+                col_dict={
+                    "b": lgdo.Array(np.array([4, 5, 6])),
+                    "tbl1": Table(col_dict={"z": lgdo.Array(np.array([9, 9, 9]))}),
+                }
+            ),
+        }
+    )
+
+    fl_tbl = tbl.flatten()
+    assert sorted(fl_tbl.keys()) == ["a", "tbl__b", "tbl__tbl1__z"]
+
+
 def test_remove_column():
     col_dict = {
         "a": lgdo.Array(nda=np.array([1, 2, 3, 4])),
         "b": lgdo.Array(nda=np.array([5, 6, 7, 8])),
         "c": lgdo.Array(nda=np.array([9, 10, 11, 12])),
     }
```

### Comparing `legend_pydataobj-1.5.1/tests/types/test_table_eval.py` & `legend_pydataobj-1.6.0/tests/types/test_table_eval.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,23 +18,33 @@
                     [21, 22, 23, 24],
                     [25, 26, 27, 8],
                     [29, 210, 211, 212],
                     [213, 214, 215, 216],
                 ],
             ),
             "e": lgdo.VectorOfVectors([[1, 2, 3], [4], [], [8, 6]]),
+            "tbl": lgdo.Table(
+                col_dict={
+                    "z": lgdo.Array([1, 1, 1, 1]),
+                    "y": lgdo.Array([8, 8, 8, 8]),
+                }
+            ),
         }
     )
     r = obj.eval("sum(a)")
     assert isinstance(r, lgdo.Scalar)
 
     r = obj.eval("a + b")
     assert isinstance(r, lgdo.Array)
     assert np.array_equal(r.nda, obj.a.nda + obj.b.nda)
 
+    r = obj.eval("a + tbl__z")
+    assert isinstance(r, lgdo.Array)
+    assert np.array_equal(r.nda, obj.a.nda + obj.tbl.z.nda)
+
     r = obj.eval("((a - b) > 1) & ((b - a) < -1)")
     assert isinstance(r, lgdo.Array)
     assert r.dtype == "bool"
 
     r = obj.eval("a + d")
     assert isinstance(r, lgdo.ArrayOfEqualSizedArrays)
```

### Comparing `legend_pydataobj-1.5.1/tests/types/test_waveformtable.py` & `legend_pydataobj-1.6.0/tests/types/test_waveformtable.py`

 * *Files identical despite different names*

